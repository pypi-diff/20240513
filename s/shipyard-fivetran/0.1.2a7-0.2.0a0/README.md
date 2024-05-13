# Comparing `tmp/shipyard_fivetran-0.1.2a7.tar.gz` & `tmp/shipyard_fivetran-0.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_fivetran-0.1.2a7.tar", max compression
+gzip compressed data, was "shipyard_fivetran-0.2.0a0.tar", max compression
```

## Comparing `shipyard_fivetran-0.1.2a7.tar` & `shipyard_fivetran-0.2.0a0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      508 2023-07-12 22:00:23.017075 shipyard_fivetran-0.1.2a7/pyproject.toml
--rw-r--r--   0        0        0       37 2023-06-21 19:54:18.755231 shipyard_fivetran-0.1.2a7/shipyard_fivetran/__init__.py
--rw-r--r--   0        0        0      257 2023-06-21 19:54:18.755602 shipyard_fivetran-0.1.2a7/shipyard_fivetran/cli/authtest.py
--rw-r--r--   0        0        0     3012 2023-07-10 20:44:53.454669 shipyard_fivetran-0.1.2a7/shipyard_fivetran/cli/sync.py
--rw-r--r--   0        0        0     2150 2023-07-10 20:44:53.455303 shipyard_fivetran-0.1.2a7/shipyard_fivetran/cli/update_connector.py
--rw-r--r--   0        0        0     9921 2023-06-21 19:54:18.755987 shipyard_fivetran-0.1.2a7/shipyard_fivetran/fivetran.py
--rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 shipyard_fivetran-0.1.2a7/PKG-INFO
+-rw-r--r--   0        0        0      708 2024-05-13 20:59:25.581677 shipyard_fivetran-0.2.0a0/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-06-21 19:54:18.755231 shipyard_fivetran-0.2.0a0/shipyard_fivetran/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-05 20:53:35.435162 shipyard_fivetran-0.2.0a0/shipyard_fivetran/cli/__init__.py
+-rw-r--r--   0        0        0      297 2024-02-05 20:53:35.435768 shipyard_fivetran-0.2.0a0/shipyard_fivetran/cli/authtest.py
+-rw-r--r--   0        0        0     3049 2024-05-13 21:05:14.273052 shipyard_fivetran-0.2.0a0/shipyard_fivetran/cli/sync.py
+-rw-r--r--   0        0        0     2188 2024-05-13 21:05:14.262784 shipyard_fivetran-0.2.0a0/shipyard_fivetran/cli/update_connector.py
+-rw-r--r--   0        0        0     9916 2024-05-13 21:05:14.268379 shipyard_fivetran-0.2.0a0/shipyard_fivetran/fivetran.py
+-rw-r--r--   0        0        0      643 1970-01-01 00:00:00.000000 shipyard_fivetran-0.2.0a0/PKG-INFO
```

### Comparing `shipyard_fivetran-0.1.2a7/shipyard_fivetran/cli/sync.py` & `shipyard_fivetran-0.2.0a0/shipyard_fivetran/cli/sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import argparse
-import sys
-import os
-import shipyard_utils as shipyard
 import datetime
-import pytz
+import os
+import sys
 
+import pytz
+import shipyard_utils as shipyard
+from shipyard_templates import ExitCodeException, ShipyardLogger
 
 from shipyard_fivetran import FivetranClient
-from shipyard_templates import ExitCodeException
+
+logger = ShipyardLogger.get_logger()
+
+EXIT_CODE_INVALID_POKE_INTERVAL = 101
 
 
 def create_pickle(connector_id):
     base_folder_name = shipyard.logs.determine_base_artifact_folder("fivetran")
     artifact_subfolder_paths = shipyard.logs.determine_artifact_subfolders(
         base_folder_name
     )
@@ -60,38 +64,38 @@
     force_sync = force_sync.upper() == "TRUE"
     poke_interval = args.interval
 
     fivetran_client = FivetranClient(
         access_token=args.api_key, api_secret=args.api_secret
     )
     if (
-        not wait_for_completion
-        and int(os.environ.get("SHIPYARD_FLEET_DOWNSTREAM_COUNT")) > 0
+            not wait_for_completion
+            and int(os.environ.get("SHIPYARD_FLEET_DOWNSTREAM_COUNT")) > 0
     ):
         # This function is to support the legacy check status functionality
         create_pickle(args.connector_id)
     poke_interval = int(poke_interval) if poke_interval else 0
     if wait_for_completion:
         if 0 < poke_interval <= 60:
-            fivetran_client.logger.info(
+            logger.info(
                 f"Setting poke interval to {poke_interval} minute(s)"
             )
             poke_interval = poke_interval
         else:
-            fivetran_client.logger.error(
+            logger.error(
                 "Poke interval must be between 1 and 60 minutes"
             )
-            sys.exit(fivetran_client.EXIT_CODE_INVALID_POKE_INTERVAL)
+            sys.exit(EXIT_CODE_INVALID_POKE_INTERVAL)
     try:
         fivetran_client.trigger_sync(
             args.connector_id,
             force=force_sync,
             wait_for_completion=wait_for_completion,
             poke_interval=poke_interval * 60,
         )
     except ExitCodeException as e:
-        fivetran_client.logger.error(e)
+        logger.error(e)
         sys.exit(e.exit_code)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_fivetran-0.1.2a7/shipyard_fivetran/cli/update_connector.py` & `shipyard_fivetran-0.2.0a0/shipyard_fivetran/cli/update_connector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import argparse
 import sys
 import json
 
 from shipyard_fivetran import FivetranClient
-from shipyard_templates import ExitCodeException
+from shipyard_templates import ExitCodeException, ShipyardLogger
+
+logger = ShipyardLogger.get_logger()
 
 
 def get_args():
     parser = argparse.ArgumentParser(
         description="Update a connector using FivetranClient"
     )
     parser.add_argument("--api-key", type=str, help="Fivetran API access token")
@@ -57,13 +59,13 @@
 
     try:
         fivetran_client.update_connector(
             connector_id,
             **args_dict,
         )
     except ExitCodeException as e:
-        fivetran_client.logger.error(e)
+        logger.error(e)
         sys.exit(e.exit_code)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_fivetran-0.1.2a7/shipyard_fivetran/fivetran.py` & `shipyard_fivetran-0.2.0a0/shipyard_fivetran/fivetran.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import time
 
 from requests import request, auth
-from shipyard_templates import Etl, ExitCodeException
+from shipyard_templates import Etl, ExitCodeException, ShipyardLogger
+
+logger = ShipyardLogger.get_logger()
 
 
 class FivetranClient(Etl):
     """
     FivetranClient is a class for interacting with the Fivetran API.
     It inherits from the Etl class and implements the necessary methods for communicating with Fivetran.
 
@@ -23,15 +25,15 @@
             access_token (str): The access token for Fivetran API
             api_secret (str): The secret key for Fivetran API
         """
         self.api_secret = api_secret
         self.api_key = access_token
         self.auth = auth.HTTPBasicAuth(self.api_key, self.api_secret)
         super().__init__(self.api_key, api_secret=self.api_secret)
-        self.logger.info("FivetranClient initialized")
+        logger.debug("FivetranClient initialized")
 
     def _request(
         self, endpoint: str, method: str = "GET", payload: dict = None
     ) -> dict:
         """
         Private method to send a request to the Fivetran API.
 
@@ -66,15 +68,15 @@
                     "Content-Type": "application/json",
                     "Accept": "application/json;version=2",
                 },
                 auth=self.auth,
             )
         if resp.ok:
             return resp.json()
-        self.logger.error(f"Error: {resp.status_code} - {resp.text}")
+        logger.error(f"Error: {resp.status_code} - {resp.text}")
         if resp.status_code == 401:
             raise ExitCodeException(
                 f'{resp.json().get("message")}', self.EXIT_CODE_INVALID_CREDENTIALS
             )
         elif resp.json().get("code") == "NotFound_Integration":
             raise ExitCodeException(
                 f'{resp.json().get("message")}', self.EXIT_CODE_SYNC_INVALID_SOURCE_ID
@@ -102,55 +104,55 @@
             wait_for_completion (bool): Whether to wait for the sync to complete. Defaults to False.
             poke_interval (int): Interval in seconds to check for sync completion. Defaults to 30.
 
         Raises:
             ExitCodeException: If an error occurs while triggering sync.
         """
         if wait_for_completion:
-            self.logger.info(
+            logger.info(
                 "Getting connection details for last successful and failed syncs..."
             )
             prev_success, prev_failure = self._get_latest_success_and_failure(
                 connector_id
             )
-            self.logger.info(
+            logger.info(
                 f'The last success was {prev_success or "never"} and the last failure was {prev_failure or "never"}'
             )
         try:
             self._request(
                 endpoint=f"connectors/{connector_id}/force",
                 method="POST",
                 payload={"force": force},
             )
         except ExitCodeException as e:
             raise ExitCodeException(f"Error triggering sync: {e}", e.exit_code) from e
         else:
-            self.logger.info("Sync triggered successfully")
+            logger.info("Sync triggered successfully")
             if wait_for_completion:
                 new_success, new_failure = prev_success, prev_failure
                 while prev_success == new_success and prev_failure == new_failure:
-                    self.logger.info("Waiting for sync to complete...")
+                    logger.info("Waiting for sync to complete...")
                     time.sleep(poke_interval)
                     new_success, new_failure = self._get_latest_success_and_failure(
                         connector_id
                     )
-                self.logger.info("Sync completed")
-                self.logger.info("Checking for new failure")
+                logger.info("Sync completed")
+                logger.info("Checking for new failure")
                 if (
                     prev_failure
                     and new_failure != prev_failure
                     or not prev_failure
                     and new_failure
                 ):
                     raise ExitCodeException(
                         f"Sync failed at {new_failure}",
                         self.EXIT_CODE_SYNC_REFRESH_ERROR,
                     )
                 else:
-                    self.logger.info("No new failure detected")
+                    logger.info("No new failure detected")
 
     def determine_sync_status(self, connector_id: str) -> str:
         """
         Determine the sync status of a specific connector.
 
         Parameters:
             connector_id (str): The ID of the connector.
@@ -245,15 +247,15 @@
             try:
                 self._request(endpoint, method="PATCH", payload=payload)
             except ExitCodeException as e:
                 raise ExitCodeException(
                     f"Error updating connector: {e}", e.exit_code
                 ) from e
             else:
-                self.logger.info("Connector updated successfully")
+                logger.info("Connector updated successfully")
         else:
             raise ExitCodeException(
                 "No updates to connector were provided", self.EXIT_CODE_BAD_REQUEST
             )
 
     def connect(self) -> int:
         """
@@ -261,12 +263,12 @@
 
         Returns:
             int: 0 if connection is valid, 1 if connection is invalid
         """
         try:
             self._request(endpoint="users", method="GET")
         except Exception as e:
-            self.logger.error(f"Error connecting to FiveTran: {e}")
+            logger.error(f"Error connecting to FiveTran: {e}")
             return 1
         else:
-            self.logger.info("Connection Validated")
+            logger.info("Connection Validated")
             return 0
```

### Comparing `shipyard_fivetran-0.1.2a7/PKG-INFO` & `shipyard_fivetran-0.2.0a0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: shipyard-fivetran
-Version: 0.1.2a7
+Version: 0.2.0a0
 Summary: A local client for connecting and working with Fivetran
 License: Apache 2.0
 Author: JR
 Author-email: johnathan.rodriguez@shipyardapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pytz (==2023.3)
 Requires-Dist: requests (==2.31.0)
-Requires-Dist: shipyard-templates (==0.1.8)
+Requires-Dist: shipyard-templates (>=0.8.2,<0.9.0)
+Requires-Dist: shipyard-utils (==0.1.4)
```

