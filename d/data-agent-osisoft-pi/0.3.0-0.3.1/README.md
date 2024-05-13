# Comparing `tmp/data-agent-osisoft-pi-0.3.0.tar.gz` & `tmp/data-agent-osisoft-pi-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-agent-osisoft-pi-0.3.0.tar", last modified: Tue Nov 28 18:06:02 2023, max compression
+gzip compressed data, was "data-agent-osisoft-pi-0.3.1.tar", last modified: Wed Nov 29 22:29:23 2023, max compression
```

## Comparing `data-agent-osisoft-pi-0.3.0.tar` & `data-agent-osisoft-pi-0.3.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:06:02.183160 data-agent-osisoft-pi-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:06:02.175160 data-agent-osisoft-pi-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:06:02.179160 data-agent-osisoft-pi-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      490 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      115 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13659 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2023-11-28 18:06:02.183160 data-agent-osisoft-pi-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:06:02.183160 data-agent-osisoft-pi-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:06:02.183160 data-agent-osisoft-pi-0.3.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      185 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (127)      992 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      254 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2023-11-28 18:06:02.187160 data-agent-osisoft-pi-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      716 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:06:02.175160 data-agent-osisoft-pi-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:06:02.183160 data-agent-osisoft-pi-0.3.0/src/data_agent_osisoft_pi/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/src/data_agent_osisoft_pi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16942 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/src/data_agent_osisoft_pi/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:06:02.183160 data-agent-osisoft-pi-0.3.0/src/data_agent_osisoft_pi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2023-11-28 18:06:02.000000 data-agent-osisoft-pi-0.3.0/src/data_agent_osisoft_pi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      859 2023-11-28 18:06:02.000000 data-agent-osisoft-pi-0.3.0/src/data_agent_osisoft_pi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 18:06:02.000000 data-agent-osisoft-pi-0.3.0/src/data_agent_osisoft_pi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-11-28 18:06:02.000000 data-agent-osisoft-pi-0.3.0/src/data_agent_osisoft_pi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 18:06:01.000000 data-agent-osisoft-pi-0.3.0/src/data_agent_osisoft_pi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-11-28 18:06:02.000000 data-agent-osisoft-pi-0.3.0/src/data_agent_osisoft_pi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-28 18:06:02.000000 data-agent-osisoft-pi-0.3.0/src/data_agent_osisoft_pi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:06:02.183160 data-agent-osisoft-pi-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/tests/test_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2023-11-28 18:05:32.000000 data-agent-osisoft-pi-0.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 22:29:23.738549 data-agent-osisoft-pi-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 22:29:23.730549 data-agent-osisoft-pi-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 22:29:23.734549 data-agent-osisoft-pi-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13659 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2023-11-29 22:29:23.738549 data-agent-osisoft-pi-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 22:29:23.734549 data-agent-osisoft-pi-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 22:29:23.734549 data-agent-osisoft-pi-0.3.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10096 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2023-11-29 22:29:23.738549 data-agent-osisoft-pi-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 22:29:23.730549 data-agent-osisoft-pi-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 22:29:23.738549 data-agent-osisoft-pi-0.3.1/src/data_agent_osisoft_pi/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/src/data_agent_osisoft_pi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17750 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/src/data_agent_osisoft_pi/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 22:29:23.738549 data-agent-osisoft-pi-0.3.1/src/data_agent_osisoft_pi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2023-11-29 22:29:23.000000 data-agent-osisoft-pi-0.3.1/src/data_agent_osisoft_pi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2023-11-29 22:29:23.000000 data-agent-osisoft-pi-0.3.1/src/data_agent_osisoft_pi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-29 22:29:23.000000 data-agent-osisoft-pi-0.3.1/src/data_agent_osisoft_pi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2023-11-29 22:29:23.000000 data-agent-osisoft-pi-0.3.1/src/data_agent_osisoft_pi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-29 22:29:23.000000 data-agent-osisoft-pi-0.3.1/src/data_agent_osisoft_pi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2023-11-29 22:29:23.000000 data-agent-osisoft-pi-0.3.1/src/data_agent_osisoft_pi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-29 22:29:23.000000 data-agent-osisoft-pi-0.3.1/src/data_agent_osisoft_pi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 22:29:23.738549 data-agent-osisoft-pi-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/tests/test_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2023-11-29 22:28:56.000000 data-agent-osisoft-pi-0.3.1/tox.ini
```

### Comparing `data-agent-osisoft-pi-0.3.0/.coveragerc` & `data-agent-osisoft-pi-0.3.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `data-agent-osisoft-pi-0.3.0/.github/workflows/ci.yml` & `data-agent-osisoft-pi-0.3.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `data-agent-osisoft-pi-0.3.0/.gitignore` & `data-agent-osisoft-pi-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `data-agent-osisoft-pi-0.3.0/.pre-commit-config.yaml` & `data-agent-osisoft-pi-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `data-agent-osisoft-pi-0.3.0/CONTRIBUTING.md` & `data-agent-osisoft-pi-0.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `data-agent-osisoft-pi-0.3.0/LICENSE.txt` & `data-agent-osisoft-pi-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `data-agent-osisoft-pi-0.3.0/PKG-INFO` & `data-agent-osisoft-pi-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-agent-osisoft-pi
-Version: 0.3.0
+Version: 0.3.1
 Summary: Osisoft PI historian plugin for `data-agent` package
 Home-page: https://github.com/imubit/data-agent-osisoft-pi/
 Author: Meir Tseitlin
 Author-email: meir@imubit.com
 License: LGPL v3
 Project-URL: Documentation, https://github.com/imubit/data-agent-osisoft-pi/
 Project-URL: Source, https://github.com/imubit/data-agent-osisoft-pi/
```

### Comparing `data-agent-osisoft-pi-0.3.0/README.md` & `data-agent-osisoft-pi-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `data-agent-osisoft-pi-0.3.0/docs/Makefile` & `data-agent-osisoft-pi-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `data-agent-osisoft-pi-0.3.0/docs/conf.py` & `data-agent-osisoft-pi-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `data-agent-osisoft-pi-0.3.0/docs/index.md` & `data-agent-osisoft-pi-0.3.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `data-agent-osisoft-pi-0.3.0/setup.cfg` & `data-agent-osisoft-pi-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `data-agent-osisoft-pi-0.3.0/setup.py` & `data-agent-osisoft-pi-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `data-agent-osisoft-pi-0.3.0/src/data_agent_osisoft_pi/__init__.py` & `data-agent-osisoft-pi-0.3.1/src/data_agent_osisoft_pi/__init__.py`

 * *Files identical despite different names*

### Comparing `data-agent-osisoft-pi-0.3.0/src/data_agent_osisoft_pi/connector.py` & `data-agent-osisoft-pi-0.3.1/src/data_agent_osisoft_pi/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,20 @@
 clr.AddReference("OSIsoft.AFSDK")
 
 
 # from OSIsoft.AF import * # noqa: E402
 # from OSIsoft.AF.Asset import * # noqa: E402
 # from OSIsoft.AF.UnitsOfMeasure import * # noqa: E402
 from OSIsoft.AF.Data import AFBoundaryType  # noqa: E402
-from OSIsoft.AF.PI import PIPoint, PIPointType, PIServers  # noqa: E402
+from OSIsoft.AF.PI import (  # noqa: E402
+    PIPoint,
+    PIPointType,
+    PIServers,
+    PITimeoutException,
+)
 from OSIsoft.AF.Time import AFTime, AFTimeRange, AFTimeSpan  # noqa: E402
 
 # from System import TimeSpan # noqa: E402
 from System.Collections.Generic import List  # noqa: E402
 
 # from System.Net import NetworkCredential # noqa: E402
 
@@ -385,17 +390,25 @@
                             < time_range.EndTime
                             else time_range.EndTime
                         )
 
                         page_time_range = AFTimeRange(next_start_time, next_end_time)
 
                         # https://docs.aveva.com/bundle/af-sdk/page/html/M_OSIsoft_AF_PI_PIPoint_InterpolatedValues.htm
-                        records = pt.InterpolatedValues(
-                            page_time_range, time_span, "", False
-                        )
+                        try:
+                            records = pt.InterpolatedValues(
+                                page_time_range, time_span, "", False
+                            )
+                        except PITimeoutException as e:
+                            log.warn(
+                                f"Retrying after pt.InterpolatedValues timeout: {e}"
+                            )
+                            records = pt.InterpolatedValues(
+                                page_time_range, time_span, "", False
+                            )
 
                         if records.Count == 0:
                             break
 
                         total_values_to_read -= records.Count
 
                         formatted_data = {
@@ -432,17 +445,23 @@
                         page_time_range = AFTimeRange(
                             next_start_time, time_range.EndTime
                         )
 
                         values_to_read = min(self._page_size, total_values_to_read)
 
                         # https://docs.aveva.com/bundle/af-sdk/page/html/M_OSIsoft_AF_PI_PIPoint_RecordedValues.htm
-                        records = pt.RecordedValues(
-                            page_time_range, boundary, "", False, values_to_read
-                        )
+                        try:
+                            records = pt.RecordedValues(
+                                page_time_range, boundary, "", False, values_to_read
+                            )
+                        except PITimeoutException as e:
+                            log.warn(f"Retrying after pt.RecordedValues timeout: {e}")
+                            records = pt.RecordedValues(
+                                page_time_range, boundary, "", False, values_to_read
+                            )
 
                         if records.Count == 0:
                             break
 
                         total_values_to_read -= records.Count
 
                         formatted_data = {
```

### Comparing `data-agent-osisoft-pi-0.3.0/src/data_agent_osisoft_pi.egg-info/PKG-INFO` & `data-agent-osisoft-pi-0.3.1/src/data_agent_osisoft_pi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-agent-osisoft-pi
-Version: 0.3.0
+Version: 0.3.1
 Summary: Osisoft PI historian plugin for `data-agent` package
 Home-page: https://github.com/imubit/data-agent-osisoft-pi/
 Author: Meir Tseitlin
 Author-email: meir@imubit.com
 License: LGPL v3
 Project-URL: Documentation, https://github.com/imubit/data-agent-osisoft-pi/
 Project-URL: Source, https://github.com/imubit/data-agent-osisoft-pi/
```

### Comparing `data-agent-osisoft-pi-0.3.0/src/data_agent_osisoft_pi.egg-info/SOURCES.txt` & `data-agent-osisoft-pi-0.3.1/src/data_agent_osisoft_pi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data-agent-osisoft-pi-0.3.0/tests/test_connector.py` & `data-agent-osisoft-pi-0.3.1/tests/test_connector.py`

 * *Files identical despite different names*

### Comparing `data-agent-osisoft-pi-0.3.0/tox.ini` & `data-agent-osisoft-pi-0.3.1/tox.ini`

 * *Files identical despite different names*

