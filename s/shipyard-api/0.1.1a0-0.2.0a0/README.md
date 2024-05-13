# Comparing `tmp/shipyard_api-0.1.1a0.tar.gz` & `tmp/shipyard_api-0.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_api-0.1.1a0.tar", max compression
+gzip compressed data, was "shipyard_api-0.2.0a0.tar", max compression
```

## Comparing `shipyard_api-0.1.1a0.tar` & `shipyard_api-0.2.0a0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-18 03:07:13.745323 shipyard_api-0.1.1a0/README.md
--rw-r--r--   0        0        0      502 2024-05-04 16:19:05.680248 shipyard_api-0.1.1a0/pyproject.toml
--rw-r--r--   0        0        0       35 2024-04-18 03:07:13.747259 shipyard_api-0.1.1a0/shipyard_api/__init__.py
--rw-r--r--   0        0        0      695 2024-05-05 20:24:10.839576 shipyard_api-0.1.1a0/shipyard_api/cli/authtest.py
--rw-r--r--   0        0        0     1443 2024-04-18 03:07:13.747671 shipyard_api-0.1.1a0/shipyard_api/cli/get_logs.py
--rw-r--r--   0        0        0     2069 2024-05-05 20:24:10.874228 shipyard_api-0.1.1a0/shipyard_api/cli/trigger_fleet.py
--rw-r--r--   0        0        0     5702 2024-05-05 20:24:10.896006 shipyard_api-0.1.1a0/shipyard_api/client.py
--rw-r--r--   0        0        0      963 2024-05-04 16:10:17.090010 shipyard_api-0.1.1a0/shipyard_api/errors.py
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 shipyard_api-0.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-18 20:05:24.210595 shipyard_api-0.2.0a0/README.md
+-rw-r--r--   0        0        0      538 2024-05-13 21:31:06.669868 shipyard_api-0.2.0a0/pyproject.toml
+-rw-r--r--   0        0        0       35 2024-04-18 20:05:24.211332 shipyard_api-0.2.0a0/shipyard_api/__init__.py
+-rw-r--r--   0        0        0      695 2024-05-06 20:06:59.600682 shipyard_api-0.2.0a0/shipyard_api/cli/authtest.py
+-rw-r--r--   0        0        0     1443 2024-04-18 20:05:24.211506 shipyard_api-0.2.0a0/shipyard_api/cli/get_logs.py
+-rw-r--r--   0        0        0     2397 2024-05-13 18:01:57.037107 shipyard_api-0.2.0a0/shipyard_api/cli/trigger_fleet.py
+-rw-r--r--   0        0        0     9521 2024-05-13 21:31:06.670566 shipyard_api-0.2.0a0/shipyard_api/client.py
+-rw-r--r--   0        0        0     1064 2024-05-13 21:31:06.671101 shipyard_api-0.2.0a0/shipyard_api/errors.py
+-rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 shipyard_api-0.2.0a0/PKG-INFO
```

### Comparing `shipyard_api-0.1.1a0/shipyard_api/cli/authtest.py` & `shipyard_api-0.2.0a0/shipyard_api/cli/authtest.py`

 * *Files identical despite different names*

### Comparing `shipyard_api-0.1.1a0/shipyard_api/cli/get_logs.py` & `shipyard_api-0.2.0a0/shipyard_api/cli/get_logs.py`

 * *Files identical despite different names*

### Comparing `shipyard_api-0.1.1a0/shipyard_api/cli/trigger_fleet.py` & `shipyard_api-0.2.0a0/shipyard_api/cli/trigger_fleet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 import sys
 import shipyard_bp_utils as utils
 from shipyard_api import ShipyardClient
 from shipyard_templates import ShipyardLogger, ExitCodeException
-from shipyard_api.errors import EXIT_CODE_UNKNOWN_ERROR
+from shipyard_api.errors import EXIT_CODE_ARTIFACTS_ERROR, EXIT_CODE_UNKNOWN_ERROR
 from shipyard_bp_utils.artifacts import Artifact
 
 logger = ShipyardLogger.get_logger()
 
 
 def get_args():
     parser = argparse.ArgumentParser()
@@ -30,25 +30,34 @@
         logger.info("Successfully triggered fleet")
     except ExitCodeException as ec:
         logger.error(ec.message)
         sys.exit(ec.exit_code)
     except Exception as e:
         logger.error(f"An unexpected error occurred: {e}")
         sys.exit(EXIT_CODE_UNKNOWN_ERROR)
-    else:
+
+    try:
         logger.debug(
             "Response is being stored in the artifacts directory for downstream use"
         )
+        log_url = response.get("log")
+        logger.info(f"Fleet run log URL: {log_url}")
+
         artifact = Artifact("shipyard-api")
         artifact.responses.write_json("trigger_fleet_response", response)
         org_id = response.get("data").get("org_id")
         project_id = response.get("data").get("project_id")
         fleet_id = response.get("data").get("fleet_id")
         fleet_run_id = response.get("data").get("fleet_run_id")
         artifact.variables.write("org_id", "pickle", org_id)
         artifact.variables.write("project_id", "pickle", project_id)
         artifact.variables.write("fleet_id", "pickle", fleet_id)
         artifact.variables.write("fleet_run_id", "pickle", fleet_run_id)
+    except Exception as e:
+        logger.error(
+            f"An error occurred while writing the response and variables to the artifacts directory: {e}"
+        )
+        sys.exit(EXIT_CODE_ARTIFACTS_ERROR)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_api-0.1.1a0/PKG-INFO` & `shipyard_api-0.2.0a0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: shipyard-api
-Version: 0.1.1a0
+Version: 0.2.0a0
 Summary: 
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pandas (>=2.2.2,<3.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: shipyard-bp-utils (>=1.2.0,<2.0.0)
 Requires-Dist: shipyard-templates (>=0.8.0,<0.9.0)
 Description-Content-Type: text/markdown
```

