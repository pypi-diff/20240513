# Comparing `tmp/whylabs_toolkit-0.0.9.tar.gz` & `tmp/whylabs_toolkit-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whylabs_toolkit-0.0.9.tar", max compression
+gzip compressed data, was "whylabs_toolkit-0.1.0.tar", max compression
```

## Comparing `whylabs_toolkit-0.0.9.tar` & `whylabs_toolkit-0.1.0.tar`

### file list

```diff
@@ -1,36 +1,54 @@
--rw-r--r--   0        0        0    11357 2023-07-28 18:17:12.083372 whylabs_toolkit-0.0.9/LICENSE
--rw-r--r--   0        0        0     1409 2023-07-28 18:17:12.083372 whylabs_toolkit-0.0.9/README.md
--rw-r--r--   0        0        0      780 2023-07-28 18:17:12.083372 whylabs_toolkit-0.0.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/cli/__init__.py
--rw-r--r--   0        0        0      559 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/container/config_types.py
--rw-r--r--   0        0        0        0 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/helpers/__init__.py
--rw-r--r--   0        0        0      362 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/helpers/client.py
--rw-r--r--   0        0        0     2029 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/helpers/config.py
--rw-r--r--   0        0        0     1982 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/helpers/dataset_profiles.py
--rw-r--r--   0        0        0     2199 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/helpers/models.py
--rw-r--r--   0        0        0     4639 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/helpers/monitor_helpers.py
--rw-r--r--   0        0        0     5922 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/helpers/schema.py
--rw-r--r--   0        0        0      922 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/helpers/utils.py
--rw-r--r--   0        0        0      100 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/__init__.py
--rw-r--r--   0        0        0      178 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/manager/__init__.py
--rw-r--r--   0        0        0      557 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/manager/credentials.py
--rw-r--r--   0        0        0     5777 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/manager/manager.py
--rw-r--r--   0        0        0    10796 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/manager/monitor_setup.py
--rw-r--r--   0        0        0     1702 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/__init__.py
--rw-r--r--   0        0        0      998 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/analyzer/__init__.py
--rw-r--r--   0        0        0    14365 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/analyzer/algorithms.py
--rw-r--r--   0        0        0     4731 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/analyzer/analyzer.py
--rw-r--r--   0        0        0     3242 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/analyzer/baseline.py
--rw-r--r--   0        0        0     2071 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/analyzer/targets.py
--rw-r--r--   0        0        0     4115 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/column_schema.py
--rw-r--r--   0        0        0     3363 2023-07-28 18:17:12.091372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/commons.py
--rw-r--r--   0        0        0     2366 2023-07-28 18:17:12.091372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/document.py
--rw-r--r--   0        0        0     9201 2023-07-28 18:17:12.091372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/monitor.py
--rw-r--r--   0        0        0      574 2023-07-28 18:17:12.091372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/segments.py
--rw-r--r--   0        0        0      961 2023-07-28 18:17:12.091372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/utils.py
--rw-r--r--   0        0        0    75902 2023-07-28 18:17:12.091372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/schema/schema.json
--rw-r--r--   0        0        0        0 2023-07-28 18:17:12.091372 whylabs_toolkit-0.0.9/whylabs_toolkit/utils/__init__.py
--rw-r--r--   0        0        0      176 2023-07-28 18:17:12.091372 whylabs_toolkit-0.0.9/whylabs_toolkit/utils/granularity.py
--rw-r--r--   0        0        0     2461 1970-01-01 00:00:00.000000 whylabs_toolkit-0.0.9/setup.py
--rw-r--r--   0        0        0     2139 1970-01-01 00:00:00.000000 whylabs_toolkit-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2056 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/README.md
+-rw-r--r--   0        0        0     1288 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/cli/__init__.py
+-rw-r--r--   0        0        0      559 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/container/config_types.py
+-rw-r--r--   0        0        0        0 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/__init__.py
+-rw-r--r--   0        0        0      362 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/client.py
+-rw-r--r--   0        0        0     2029 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/config.py
+-rw-r--r--   0        0        0     1257 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/cron_validators.py
+-rw-r--r--   0        0        0     2488 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/dataset_profiles.py
+-rw-r--r--   0        0        0     2199 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/models.py
+-rw-r--r--   0        0        0     4699 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/monitor_helpers.py
+-rw-r--r--   0        0        0     5922 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/schema.py
+-rw-r--r--   0        0        0     1160 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/utils.py
+-rw-r--r--   0        0        0      100 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/__init__.py
+-rw-r--r--   0        0        0      113 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/constants.py
+-rw-r--r--   0        0        0        0 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/converters/__init__.py
+-rw-r--r--   0        0        0     1516 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/converters/granularity.py
+-rw-r--r--   0        0        0        0 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/helpers/__init__.py
+-rw-r--r--   0        0        0     1099 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/helpers/describe.py
+-rw-r--r--   0        0        0     2192 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/helpers/utils.py
+-rw-r--r--   0        0        0       62 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/models/__init__.py
+-rw-r--r--   0        0        0     9555 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/models/diagnosis_report.py
+-rw-r--r--   0        0        0      976 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/models/noisy_monitors.py
+-rw-r--r--   0        0        0    18045 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/monitor_diagnoser.py
+-rw-r--r--   0        0        0        0 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/recommendation/__init__.py
+-rw-r--r--   0        0        0     7234 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/recommendation/change_recommender.py
+-rw-r--r--   0        0        0      686 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/recommendation/manual_change.py
+-rw-r--r--   0        0        0     2187 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/recommendation/recommended_change.py
+-rw-r--r--   0        0        0     1809 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/recommendation/remove_columns.py
+-rw-r--r--   0        0        0     1392 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/targeting.py
+-rw-r--r--   0        0        0      178 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/manager/__init__.py
+-rw-r--r--   0        0        0      557 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/manager/credentials.py
+-rw-r--r--   0        0        0     5907 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/manager/manager.py
+-rw-r--r--   0        0        0    14684 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/manager/monitor_setup.py
+-rw-r--r--   0        0        0     1769 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/__init__.py
+-rw-r--r--   0        0        0     1048 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/analyzer/__init__.py
+-rw-r--r--   0        0        0    15205 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/analyzer/algorithms.py
+-rw-r--r--   0        0        0     5693 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/analyzer/analyzer.py
+-rw-r--r--   0        0        0     3242 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/analyzer/baseline.py
+-rw-r--r--   0        0        0     2232 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/analyzer/targets.py
+-rw-r--r--   0        0        0     4115 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/column_schema.py
+-rw-r--r--   0        0        0     3323 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/commons.py
+-rw-r--r--   0        0        0     2366 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/document.py
+-rw-r--r--   0        0        0     9610 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/monitor.py
+-rw-r--r--   0        0        0      574 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/segments.py
+-rw-r--r--   0        0        0      961 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/utils.py
+-rw-r--r--   0        0        0    78578 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/schema/schema.json
+-rw-r--r--   0        0        0        0 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/utils/__init__.py
+-rw-r--r--   0        0        0      176 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/utils/granularity.py
+-rw-r--r--   0        0        0     3661 1970-01-01 00:00:00.000000 whylabs_toolkit-0.1.0/setup.py
+-rw-r--r--   0        0        0     3212 1970-01-01 00:00:00.000000 whylabs_toolkit-0.1.0/PKG-INFO
```

### Comparing `whylabs_toolkit-0.0.9/LICENSE` & `whylabs_toolkit-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.9/README.md` & `whylabs_toolkit-0.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 pip install whylabs_toolkit
 ``` 
 
 ## Packages
 
 The available packages that we have enable different use-cases for the `whylabs_toolkit`. To get started, navigate to one of the following sections and find useful tutorials there.
 
-| Package             | Usage                |
-|---------------------|----------------------|
-| [Monitor Manager](/whylabs_toolkit/monitor/manager/README.md) | Author and modify existing WhyLabs monitor with Python |
-| [WhyLabs Helpers](/whylabs_toolkit/helpers/README.md) | Interact with and modify your Datasets and ML Models specs in WhyLabs. |
+| Package                                                                                                                   | Usage                                                                  |
+|---------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------|
+| [Monitor Manager](https://github.com/whylabs/whylabs-toolkit/blob/mainline/whylabs_toolkit/monitor/manager/README.md)     | Author and modify existing WhyLabs monitor with Python.                |
+| [Monitor Diagnoser](https://github.com/whylabs/whylabs-toolkit/blob/mainline/whylabs_toolkit/monitor/diagnoser/README.md) | Diagnose problems with monitors.                                       |
+| [WhyLabs Helpers](https://github.com/whylabs/whylabs-toolkit/blob/mainline/whylabs_toolkit/helpers/README.md)             | Interact with and modify your Datasets and ML Models specs in WhyLabs. |
 
 ## Development
 
 To start contributing, you will manage dependencies with [Poetry](https://python-poetry.org/) and also a handful of `Makefile` commands. To install all necessary dependencies and activate the virtual environment, run:
 
 ```bash
 make setup && poetry shell
```

### Comparing `whylabs_toolkit-0.0.9/whylabs_toolkit/container/config_types.py` & `whylabs_toolkit-0.1.0/whylabs_toolkit/container/config_types.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.9/whylabs_toolkit/helpers/config.py` & `whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/config.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.9/whylabs_toolkit/helpers/dataset_profiles.py` & `whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/dataset_profiles.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-# from whylabs_client.api.
+import logging
 from datetime import datetime
 from typing import Optional, Union
 
-from whylabs_client.api.dataset_profile_api import DeleteDatasetProfilesResponse
+from whylabs_client.api.dataset_profile_api import DeleteDatasetProfilesResponse, DeleteAnalyzerResultsResponse
 
 from whylabs_toolkit.helpers.utils import get_dataset_profile_api
 from whylabs_toolkit.helpers.config import Config
 
 date_or_millis = Union[datetime, int]
+logger = logging.getLogger(__name__)
 
 
 def validate_timestamp_in_millis(epoch_milliseconds: int) -> bool:
     if not isinstance(epoch_milliseconds, int):
         return False
     try:
         epoch_seconds = epoch_milliseconds / 1000
@@ -45,15 +46,26 @@
 
     profile_start_timestamp = process_date_input(date_input=start)
     profile_end_timestamp = process_date_input(date_input=end)
 
     org_id = org_id or config.get_default_org_id()
     dataset_id = dataset_id or config.get_default_dataset_id()
 
-    result: DeleteDatasetProfilesResponse = api.delete_dataset_profiles(
+    result_profiles: DeleteDatasetProfilesResponse = api.delete_dataset_profiles(
         org_id=org_id,
         dataset_id=dataset_id,
         profile_start_timestamp=profile_start_timestamp,
         profile_end_timestamp=profile_end_timestamp,
     )
+    logger.info(f"Scheduled deletion for profiles on {dataset_id} for {org_id}")
 
-    return result
+    api.delete_analyzer_results(
+        org_id=org_id,
+        dataset_id=dataset_id,
+        start_timestamp=profile_start_timestamp,
+        end_timestamp=profile_end_timestamp,
+    )
+
+    logger.info("Deleted analyzer results for the same timestamps as the profiles")
+    logger.info(f"NOTE: Profile deletion happens every full hour on WhyLabs")
+
+    return result_profiles
```

### Comparing `whylabs_toolkit-0.0.9/whylabs_toolkit/helpers/models.py` & `whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/models.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.9/whylabs_toolkit/helpers/monitor_helpers.py` & `whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/monitor_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,33 +74,38 @@
         for analyzer in analyzer_ids:
             analyzers.append(api.get_analyzer(org_id=org_id, dataset_id=dataset_id, analyzer_id=analyzer))
         return analyzers
     else:
         return None
 
 
+def time_period_to_granularity(time_period: str) -> Granularity:
+    if time_period == "PT1H":
+        return Granularity.hourly
+
+    if time_period == "P1W":
+        return Granularity.weekly
+
+    if time_period == "P1M":
+        return Granularity.monthly
+
+    return Granularity.daily
+
+
 def get_model_granularity(
     org_id: Optional[str] = None, dataset_id: Optional[str] = None, config: Config = Config()
 ) -> Optional[Granularity]:
     org_id = org_id or config.get_default_org_id()
     dataset_id = dataset_id or config.get_default_dataset_id()
 
     api = get_models_api(config=config)
     model_meta = api.get_model(org_id=org_id, model_id=dataset_id)
 
-    time_period_to_gran = {
-        "H": Granularity.hourly,
-        "D": Granularity.daily,
-        "W": Granularity.weekly,
-        "M": Granularity.monthly,
-    }
     if model_meta:
-        for key, value in time_period_to_gran.items():
-            if key in model_meta["time_period"]:
-                return value
+        return time_period_to_granularity(model_meta["time_period"])
     return None
 
 
 def delete_monitor(
     monitor_id: str, org_id: Optional[str] = None, dataset_id: Optional[str] = None, config: Config = Config()
 ) -> None:
     org_id = org_id or config.get_default_org_id()
```

### Comparing `whylabs_toolkit-0.0.9/whylabs_toolkit/helpers/schema.py` & `whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/schema.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.9/whylabs_toolkit/helpers/utils.py` & `whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from whylabs_client.api.dataset_profile_api import DatasetProfileApi
+from whylabs_client.api.monitor_diagnostics_api import MonitorDiagnosticsApi
 from whylabs_client.api.models_api import ModelsApi
 from whylabs_client.api.notification_settings_api import NotificationSettingsApi
 from whylabs_client.api.monitor_api import MonitorApi
 
 from whylabs_toolkit.helpers.client import create_client
 from whylabs_toolkit.helpers.config import Config
 
@@ -17,7 +18,11 @@
 
 def get_notification_api(config: Config = Config()) -> NotificationSettingsApi:
     return NotificationSettingsApi(api_client=create_client(config=config))
 
 
 def get_monitor_api(config: Config = Config()) -> MonitorApi:
     return MonitorApi(api_client=create_client(config=config))
+
+
+def get_monitor_diagnostics_api(config: Config = Config()) -> MonitorDiagnosticsApi:
+    return MonitorDiagnosticsApi(api_client=create_client(config=config))
```

### Comparing `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/manager/credentials.py` & `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/manager/credentials.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/manager/manager.py` & `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/manager/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,21 +36,25 @@
         actions_dict_list = self.__notifications_api.list_notification_actions(org_id=self._setup.credentials.org_id)
         action_ids = []
         for action in actions_dict_list:
             action_ids.append(action.get("id"))
         return action_ids
 
     @staticmethod
-    def get_notification_request_payload(action: Union[SlackWebhook, EmailRecipient]) -> str:
+    def get_notification_request_payload(action: Union[SlackWebhook, EmailRecipient, PagerDuty]) -> str:
         if isinstance(action, SlackWebhook):
             return "slackWebhook"
         elif isinstance(action, EmailRecipient):
             return "email"
+        elif isinstance(action, PagerDuty):
+            return "pagerDutyKey"
         else:
-            raise ValueError(f"Can't work with {action} type. Available options are SlackWebhook and EmailRecipient.")
+            raise ValueError(
+                f"Can't work with {action} type. Available options are SlackWebhook, PagerDuty and EmailRecipient."
+            )
 
     def _update_notification_actions(self) -> None:
         """
         Updates the notification actions to be passed to WhyLabs based on the actions defined in the MonitorBuilder object.
         """
         if not self._setup.monitor:
             raise ValueError("You must call apply() on your MonitorSetup object!")
```

### Comparing `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/__init__.py` & `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,16 @@
     "ListComparisonOperator",
     "ListComparisonConfig",
     "ExperimentalConfig",
     "FixedThresholdsConfig",
     "ColumnListChangeConfig",
     "SeasonalConfig",
     "StddevConfig",
+    "ConjunctionConfig",
+    "DisjunctionConfig",
     # targets
     "DatasetMatrix",
     "ColumnMatrix",
     "Segment",
     "SegmentTag",
     "TargetLevel",
     # monitors
@@ -55,14 +57,15 @@
     "CronSchedule",
     "FixedCadenceSchedule",
     "Cadence",
     # monitor actions
     # "RawWebhook",
     "SlackWebhook",
     "EmailRecipient",
+    "PagerDuty",
     "GlobalAction",
     # big document
     "Document",
     # schema
     "EntitySchema",
     "ColumnSchema",
     "ColumnDataType",
```

### Comparing `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/analyzer/__init__.py` & `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/analyzer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     "ExperimentalConfig",
     "FixedThresholdsConfig",
     "ColumnListChangeConfig",
     "SeasonalConfig",
     "ListComparisonConfig",
     "FrequentStringComparisonConfig",
     "StddevConfig",
+    "ConjunctionConfig",
+    "DisjunctionConfig",
     # enums
     "DiffMode",
     "ThresholdType",
     "AlgorithmType",
     "DatasetMetric",
     "SimpleColumnMetric",
     "ComplexMetrics",
```

### Comparing `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/analyzer/algorithms.py` & `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/analyzer/algorithms.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     frequent_string_comparison = "frequent_string_comparison"
     diff = "diff"
     drift = "drift"
     stddev = "stddev"
     seasonal = "seasonal"
     fixed = "fixed"
     experimental = "experimental"
+    conjunction = "conjunction"
+    disjunction = "disjunction"
 
 
 class DatasetMetric(str, Enum):
     """Metrics that are applicable at the dataset level."""
 
     # ingestion health. null value if not ingested yet
     profile_count = "profile.count"
@@ -54,14 +56,17 @@
     classification_auc = "classification.auc"
 
     # regression metrics
     regression_mse = "regression.mse"
     regression_mae = "regression.mae"
     regression_rmse = "regression.rmse"
 
+    # other metrics
+    missing_data_point = "missingDatapoint"
+
 
 class SimpleColumnMetric(str, Enum):
     """Simple column metrics that are basically just a single number."""
 
     count = "count"  # type: ignore
     median = "median"
     max = "max"
@@ -231,27 +236,39 @@
     minLowerThreshold: Optional[float] = Field(
         None,
         description="Capping the minimum threshold by this value. This value only becomes effective if the calculated "
         "lower threshold from the calculation is lesser than this value",
     )
 
 
+class ThresholdType(str, Enum):
+    """By default, an anomaly will be generated when the target is above or below the baseline
+    by the specified threshold.
+
+    If its only desirable to alert when the target is above the
+    baseline and not the other way around, specify upper for your ThresholdType."""
+
+    lower = "lower"  # type: ignore
+    upper = "upper"  # type: ignore
+
+
 class StddevConfig(_ThresholdBaseConfig):
     """Calculates upper bounds and lower bounds based on stddev from a series of numbers.
 
     An analyzer using stddev for a window of time range.
 
     This calculation will fall back to Poisson distribution if there is only 1 value in the baseline.
     For 2 values, we use the formula sqrt((x_i - avg(x))^2 / n - 1)
     """
 
     type: Optional[Literal[AlgorithmType.stddev]] = Field(AlgorithmType.stddev)
     factor: Optional[float] = Field(
         3.0, description="The multiplier used with stddev to build the upper and lower bounds."
     )
+    thresholdType: Optional[ThresholdType]
     minBatchSize: Optional[int] = Field(
         1, title="MinBatchSize", ge=1, description="Minimum number of batches that is required"
     )
     baseline: Union[TrailingWindowBaseline, TimeRangeBaseline, ReferenceProfileId]
 
 
 class SeasonalConfig(_ThresholdBaseConfig):
@@ -286,14 +303,15 @@
         description="Maxinum number of data points to consider for calculating stddev. These are the data points"
         "preceeding the target batch."
     )
     stddevFactor: Optional[float] = Field(
         default=1.0,
         description="The multiplier factor for calculating upper bounds and lower bounds from the prediction.",
     )
+    thresholdType: Optional[ThresholdType]
 
 
 class DriftConfig(AlgorithmConfig):
     """An analyzer using stddev for a window of time range.
 
     This analysis will detect whether the data drifts or not. By default, we use hellinger distance with a threshold
     of 0.7.
@@ -355,29 +373,36 @@
 class DiffMode(str, Enum):
     """Whether to use the absolute difference or the percentage to calculate the difference."""
 
     abs = "abs"
     pct = "pct"
 
 
-class ThresholdType(str, Enum):
-    """By default, an anomaly will be generated when the target is above or below the baseline
-    by the specified threshold.
-
-    If its only desirable to alert when the target is above the
-    baseline and not the other way around, specify upper for your ThresholdType."""
-
-    lower = "lower"  # type: ignore
-    upper = "upper"  # type: ignore
-
-
 class DiffConfig(AlgorithmConfig):
     """Detecting the differences between two numerical metrics."""
 
     type: Literal[AlgorithmType.diff] = AlgorithmType.diff
     mode: DiffMode
     thresholdType: Optional[ThresholdType]
     threshold: float = Field(
         description="The minimum threshold that will trigger an anomaly. The monitor detect the difference between"
         "the target's metric and the baseline metric. Both of these metrics MUST be in rolled up form",
     )
     baseline: Union[TrailingWindowBaseline, ReferenceProfileId, TimeRangeBaseline, SingleBatchBaseline]
+
+
+class ConjunctionConfig(NoExtrasBaseModel):
+    """Conjunction (ANDs) composite analyzer joining multiple analyzers."""
+
+    type: Literal[AlgorithmType.conjunction] = AlgorithmType.conjunction
+    analyzerIds: List[str] = Field(
+        description="The corresponding analyzer IDs for the conjunction.",
+    )
+
+
+class DisjunctionConfig(NoExtrasBaseModel):
+    """Disjunction (ORs) composite analyzer joining multiple analyzers."""
+
+    type: Literal[AlgorithmType.disjunction] = AlgorithmType.disjunction
+    analyzerIds: List[str] = Field(
+        description="The corresponding analyzer IDs for the disjunction.",
+    )
```

### Comparing `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/analyzer/analyzer.py` & `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/analyzer/analyzer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Schema for analyses."""
 from typing import Any, Dict, List, Optional, Union
 
-from pydantic import BaseModel, Field, constr
+from pydantic import BaseModel, Field, constr, validator
 
 from whylabs_toolkit.monitor.models.commons import NoExtrasBaseModel
 
 from ..commons import CronSchedule, FixedCadenceSchedule, Metadata
 from ..utils import anyOf_to_oneOf, duration_field
 from .algorithms import (
     ColumnListChangeConfig,
@@ -14,16 +14,19 @@
     FrequentStringComparisonConfig,
     DiffConfig,
     DriftConfig,
     ExperimentalConfig,
     FixedThresholdsConfig,
     SeasonalConfig,
     StddevConfig,
+    ConjunctionConfig,
+    DisjunctionConfig,
 )
 from .targets import ColumnMatrix, DatasetMatrix
+from whylabs_toolkit.helpers.cron_validators import validate_cron_expression
 
 
 class Analyzer(NoExtrasBaseModel):
     """Configuration for running an analysis.
 
     An analysis targets a metric (note that a metric could be a complex object) for one or multiple fields in
     one or multiple segments. The output is a list of 'anomalies' that might show issues with data.
@@ -51,25 +54,32 @@
         regex="[0-9a-zA-Z \\-_]+",
     )
     tags: Optional[  # type: ignore
         List[constr(min_length=3, max_length=32, regex="[0-9a-zA-Z\\-_]")]  # noqa
     ] = Field(  # noqa F722
         None, description="A list of tags that are associated with the analyzer."
     )
-    # disabling CronSchedule as it can be tricky on the BE
-    schedule: Optional[FixedCadenceSchedule] = Field(  # Optional[Union[CronSchedule, FixedCadenceSchedule]] = Field(
+
+    schedule: Optional[Union[FixedCadenceSchedule, CronSchedule]] = Field(
         None,
         description="A schedule for running the analyzer. If not set, the analyzer's considered disabled",
     )
     disabled: Optional[bool] = Field(
         None,
         description="Whether the analyzer is disabled. "
         "This allows user to keep the configuration"
         "around without having to delete the analyzer config",
     )
+    disableTargetRollup: Optional[bool] = Field(
+        None,
+        description="For customers with individual profile storage enabled on their account (contact us), this "
+        "allows a user to monitor individual profiles without rolling them up. When enabled, analysis "
+        "will be timestamped 1:1 with the profile's dataset timestamp rather than being truncated "
+        "to the dataset granularity. ",
+    )
     targetMatrix: Union[ColumnMatrix, DatasetMatrix] = Field(
         description="A matrix for possible locations of the target",
         discriminator="type",
     )
     dataReadinessDuration: Optional[str] = duration_field(
         title="DataReadinessDuration",
         description="ISO 8610 duration format. The duration determines how fast data is ready for the monitor. For "
@@ -87,27 +97,38 @@
         description="ISO 8610 duration format. How far back an analyzer will attempt to backfill late data. Note that "
         "we will only backfill batches not previously analyzed. If the batch was already analyzed, "
         "even with partial data, the backfill will ignore the new data unless you trigger an explicit "
         "backfill request. We support 48 hours for hourly data, 30 days for daily data, and 6 months for "
         "monthly data.",
     )
 
+    @validator("schedule", pre=True, always=True)
+    def validate_schedule(
+        cls, v: Optional[Union[FixedCadenceSchedule, CronSchedule]]
+    ) -> Optional[Union[FixedCadenceSchedule, CronSchedule]]:
+        """Validate the schedule."""
+        if isinstance(v, CronSchedule) and not validate_cron_expression(v.cron):
+            raise ValueError("CronSchedule must be no less granular than 1 hour and must have 5 fields.")
+        return v
+
     # NOT YET IMPLEMENTED:
     # ExperimentalConfig,
     # ColumnListChangeConfig,
 
     config: Union[
         DiffConfig,
         FixedThresholdsConfig,
         ListComparisonConfig,
         FrequentStringComparisonConfig,
         StddevConfig,
         DriftConfig,
         ComparisonConfig,
         SeasonalConfig,
+        ConjunctionConfig,
+        DisjunctionConfig,
     ] = Field(description="The configuration map of the analyzer", discriminator="type")
 
     class Config:
         """Updates JSON schema anyOf to oneOf."""
 
         # noinspection PyUnusedLocal
         @staticmethod
```

### Comparing `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/analyzer/baseline.py` & `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/analyzer/baseline.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/analyzer/targets.py` & `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/analyzer/targets.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,7 +64,12 @@
     )
     exclude: Optional[List[Union[ColumnGroups, COLUMN_NAME_TYPE]]] = Field(  # type: ignore
         None,
         description="List of blocked fields/features/columns. Could be a grouping as well. This setting is "
         "evaluated AFTER the 'include' field and thus should be used with caution.",
         max_items=1000,
     )
+    profileId: Optional[str] = Field(
+        default=None,
+        description="The unique profile ID for the reference profile",
+        max_length=100,
+    )
```

### Comparing `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/column_schema.py` & `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/column_schema.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/commons.py` & `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/commons.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from datetime import datetime
 from enum import Enum
 from typing import List, Literal, Optional
 
 from pydantic import BaseModel, Extra
 from pydantic.fields import Field
 
-CRON_REGEX = "(@(annually|yearly|monthly|weekly|daily|hourly))|" "((((\\d+,)+\\d+|(\\d+(\\/|-)\\d+)|\\d+|\\*) ?){5,7})"
+CRON_REGEX = (
+    "(@(annually|yearly|monthly|weekly|daily|hourly))|" "((((\\d+,)+\\d+|(\\d+(\\/|-)\\d+)|\\d+|\\*|\\*/\\d+) ?){5,7})"
+)
 DATASET_ID_REGEX = "[a-zA-Z0-9\\-_\\.]+"
 
 DATASET_ID_DEF = Field(
     title="DatasetId",
     description="The unique ID of an dataset. This is specific to WhyLabs. If the dataset ID "
     "does not exist, user will get a validation exception when saving the "
     "config with WhyLabs API",
@@ -46,15 +48,14 @@
     cron: str = Field(
         description="Cron expression",
         regex=CRON_REGEX,
     )
     exclusionRanges: Optional[List[TimeRange]] = Field(
         title="ExclusionRanges", description="The ranges of dates during which this Analyzer is NOT run."
     )
-    # TODO: support other mode of configuring scheduling
 
 
 class Cadence(str, Enum):
     """Cadence for an analyzer or monitor run."""
 
     hourly = "hourly"
     daily = "daily"
```

### Comparing `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/document.py` & `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/document.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/monitor.py` & `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,23 +43,34 @@
 
     type: Literal["slack"] = "slack"
     id: str = Field(description="The endpoint ID to which you wish to send notifications to")
     destination: str = Field(description="The Slack target webhook endpoint")
 
 
 class RawWebhook(NoExtrasBaseModel):
-    """Action to send a Slack webhook."""
+    """Action to send a Raw webhook."""
 
     type: Literal["raw"] = "raw"
     id: str = Field(description="The endpoint ID to which you wish to send notifications to")
     destination: Optional[str] = Field(
         default=None, description="Sending raw unformatted message in JSON format to a webhook"
     )
 
 
+class PagerDuty(NoExtrasBaseModel):
+    """Action to send a PagerDuty notification."""
+
+    type: Literal["pager_duty"] = "pager_duty"
+    id: str = Field(description="The PagerDuty endpoint ID to send notifications to")
+    destination: Optional[str] = Field(
+        default=None,
+        description="The secret key to access the PagerDuty endpoint. Required when the ID was not created",
+    )
+
+
 class AnomalyFilter(NoExtrasBaseModel):
     """Filter the anomalies based on certain criteria. If the alerts are filtered down to 0, the monitor won't fire."""
 
     includeColumns: Optional[List[COLUMN_NAME_TYPE]] = Field(  # type: ignore
         None,
         title="IncludeColumns",
         description="If set, we only include anomalies from these columns",
@@ -219,15 +230,15 @@
     )
     disabled: Optional[bool] = Field(None, description="Whether the monitor is enabled or not")
     severity: Optional[int] = Field(3, description="The severity of the monitor messages")
     mode: Union[EveryAnomalyMode, DigestMode] = Field(
         description="Notification mode and how we might handle different analysis",
         discriminator="type",
     )
-    actions: List[Union[GlobalAction, EmailRecipient, SlackWebhook]] = Field(
+    actions: List[Union[GlobalAction, EmailRecipient, SlackWebhook, PagerDuty]] = Field(
         description="List of destination for the outgoing messages",
         max_items=100,
     )
 
     class Config:
         """Updates JSON schema anyOf to oneOf."""
```

### Comparing `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/segments.py` & `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/segments.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/utils.py` & `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/utils.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/schema/schema.json` & `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/schema/schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978638264111335%*

 * *Differences: {"'definitions'": "{'ColumnMatrix': {'properties': {'profileId': OrderedDict([('title', "*

 * *                  "'ProfileId'), ('description', 'The unique profile ID for the reference "*

 * *                  "profile'), ('maxLength', 100), ('type', 'string')])}}, 'DatasetMetric': "*

 * *                  "{'enum': {insert: [(12, 'classification.fpr'), (13, 'classification.auroc')], "*

 * *                  "delete: [12]}}, 'StddevConfig': {'properties': {'thresholdType': "*

 * *                  "OrderedDict([('$ref', '#/definiti […]*

```diff
@@ -5,14 +5,16 @@
     "definitions": {
         "AlgorithmType": {
             "description": "Specify the algorithm type.",
             "enum": [
                 "expected",
                 "column_list",
                 "comparison",
+                "conjunction",
+                "disjunction",
                 "list_comparison",
                 "frequent_string_comparison",
                 "diff",
                 "drift",
                 "stddev",
                 "seasonal",
                 "fixed",
@@ -41,27 +43,35 @@
                 },
                 "config": {
                     "description": "The configuration map of the analyzer",
                     "discriminator": {
                         "mapping": {
                             "column_list": "#/definitions/ColumnListChangeConfig",
                             "comparison": "#/definitions/ComparisonConfig",
+                            "conjunction": "#/definitions/ConjunctionConfig",
                             "diff": "#/definitions/DiffConfig",
+                            "disjunction": "#/definitions/DisjunctionConfig",
                             "drift": "#/definitions/DriftConfig",
                             "experimental": "#/definitions/ExperimentalConfig",
                             "fixed": "#/definitions/FixedThresholdsConfig",
                             "frequent_string_comparison": "#/definitions/FrequentStringComparisonConfig",
                             "list_comparison": "#/definitions/ListComparisonConfig",
                             "seasonal": "#/definitions/SeasonalConfig",
                             "stddev": "#/definitions/StddevConfig"
                         },
                         "propertyName": "type"
                     },
                     "oneOf": [
                         {
+                            "$ref": "#/definitions/ConjunctionConfig"
+                        },
+                        {
+                            "$ref": "#/definitions/DisjunctionConfig"
+                        },
+                        {
                             "$ref": "#/definitions/DiffConfig"
                         },
                         {
                             "$ref": "#/definitions/ComparisonConfig"
                         },
                         {
                             "$ref": "#/definitions/ListComparisonConfig"
@@ -93,14 +103,19 @@
                 "dataReadinessDuration": {
                     "description": "ISO 8610 duration format. The duration determines how fast data is ready for the monitor. For example, if your pipeline takes 2 days to deliver profiles to WhyLabs, the value should beP2D. Note that this value will be used to evaluate missing data as well",
                     "example": "PT1H, P1D",
                     "pattern": "^P(?!$)(\\d+M)?(\\d+W)?(\\d+D)?(T(?=\\d+[HM])(\\d+H)?(\\d+M)?)?$",
                     "title": "DataReadinessDuration",
                     "type": "string"
                 },
+                "disableTargetRollup": {
+                    "description": "For customers with individual profile storage enabled on their account (contact us), this allows a user to monitor individual profiles without rolling them up. When enabled, analysis will be timestamped 1:1 with the profile's dataset timestamp rather than being truncated to the dataset granularity. ",
+                    "title": "Disabletargetrollup",
+                    "type": "boolean"
+                },
                 "disabled": {
                     "description": "Whether the analyzer is disabled. This allows user to keep the configurationaround without having to delete the analyzer config",
                     "title": "Disabled",
                     "type": "boolean"
                 },
                 "displayName": {
                     "description": "A display name for the analyzer if view through WhyLabs UI. Can only contain dashes, underscores,spaces, and alphanumeric characters",
@@ -431,14 +446,20 @@
                             }
                         ]
                     },
                     "maxItems": 1000,
                     "title": "Include",
                     "type": "array"
                 },
+                "profileId": {
+                    "description": "The unique profile ID for the reference profile",
+                    "maxLength": 100,
+                    "title": "ProfileId",
+                    "type": "string"
+                },
                 "segments": {
                     "description": "List of targeted segments. If not set, default to the overall segment",
                     "items": {
                         "$ref": "#/definitions/Segment"
                     },
                     "maxItems": 1000,
                     "title": "Segments",
@@ -595,14 +616,43 @@
                 "lt",
                 "ge",
                 "le"
             ],
             "title": "ComparisonOperator",
             "type": "string"
         },
+        "ConjunctionConfig": {
+            "additionalProperties": false,
+            "description": "Conjunction (ANDs) composite analyzer joining multiple analyzers\n    ",
+            "properties": {
+                "analyzerIds": {
+                    "description": "The corresponding analyzer IDs for the conjunction.",
+                    "items": {
+                        "pattern": "^[A-Za-z0-9_\\-]+$",
+                        "type": "string"
+                    },
+                    "maxItems": 10,
+                    "title": "AnalyzerIds",
+                    "type": "array"
+                },
+                "type": {
+                    "enum": [
+                        "conjunction"
+                    ],
+                    "title": "Type",
+                    "type": "string"
+                }
+            },
+            "required": [
+                "type",
+                "analyzerIds"
+            ],
+            "title": "ConjunctionConfig",
+            "type": "object"
+        },
         "CronSchedule": {
             "additionalProperties": false,
             "description": "Support for scheduling.",
             "properties": {
                 "cron": {
                     "description": "Cron expression",
                     "pattern": "(@(annually|yearly|monthly|weekly|daily|hourly))|((((\\d+,)+\\d+|(\\d+(\\/|-)\\d+)|\\d+|\\*) ?){5,7})",
@@ -678,15 +728,16 @@
                 "shape_row_count",
                 "input.count",
                 "output.count",
                 "classification.f1",
                 "classification.precision",
                 "classification.recall",
                 "classification.accuracy",
-                "classification.auc",
+                "classification.fpr",
+                "classification.auroc",
                 "regression.mse",
                 "regression.mae",
                 "regression.rmse"
             ],
             "title": "DatasetMetric",
             "type": "string"
         },
@@ -844,26 +895,55 @@
                 "byAnalyzer",
                 "byDay",
                 "byHour"
             ],
             "title": "DigestModeGrouping",
             "type": "string"
         },
+        "DisjunctionConfig": {
+            "additionalProperties": false,
+            "description": "Disjunction (ORs) composite analyzer joining multiple analyzers\n    ",
+            "properties": {
+                "analyzerIds": {
+                    "description": "The corresponding analyzer IDs for the conjunction.",
+                    "items": {
+                        "pattern": "^[A-Za-z0-9_\\-]+$",
+                        "type": "string"
+                    },
+                    "maxItems": 10,
+                    "title": "AnalyzerIds",
+                    "type": "array"
+                },
+                "type": {
+                    "enum": [
+                        "disjunction"
+                    ],
+                    "title": "Type",
+                    "type": "string"
+                }
+            },
+            "required": [
+                "type",
+                "analyzerIds"
+            ],
+            "title": "DisjunctionConfig",
+            "type": "object"
+        },
         "DriftConfig": {
             "additionalProperties": false,
             "description": "An analyzer using stddev for a window of time range.\n\nThis analysis will detect whether the data drifts or not. By default, we use hellinger distance with a threshold\nof 0.7.",
             "properties": {
                 "algorithm": {
                     "default": "hellinger",
                     "description": "The algorithm to use when calculating drift.",
                     "enum": [
                         "hellinger",
-                        "ks_test",
+                        "jensenshannon",
                         "kl_divergence",
-                        "variation_distance"
+                        "psi"
                     ],
                     "title": "Algorithm",
                     "type": "string"
                 },
                 "baseline": {
                     "description": "A baseline for running the analyzer.",
                     "discriminator": {
@@ -1729,17 +1809,15 @@
             "additionalProperties": false,
             "description": "An analyzer using stddev for a window of time range.\n\nThis will fall back to Poisson distribution if there is only 1 value in the baseline.\n\nThis only works with TrailingWindow baseline (TODO: add backend validation)",
             "properties": {
                 "algorithm": {
                     "default": "arima",
                     "description": "The algorithm implementation for seasonal analysis",
                     "enum": [
-                        "arima",
-                        "rego",
-                        "stastforecast"
+                        "arima"
                     ],
                     "title": "Algorithm",
                     "type": "string"
                 },
                 "alpha": {
                     "default": 0.05,
                     "description": "significance level for the confidence interval produced around predictions. If 0.05 then the algorithm will calculate a 95% confidence interval around predictions",
@@ -1810,14 +1888,17 @@
                     "description": "Ranges of time where we will apply standard deviation for confidence intervals rather than the confidence interval from the algorithm. This is to prevent data from specialevents from making the bands very wide for timeseries-based predictions.",
                     "items": {
                         "$ref": "#/definitions/TimeRange"
                     },
                     "title": "StddevTimeRanges",
                     "type": "array"
                 },
+                "thresholdType": {
+                    "$ref": "#/definitions/ThresholdType"
+                },
                 "type": {
                     "enum": [
                         "seasonal"
                     ],
                     "title": "Type",
                     "type": "string"
                 }
@@ -2102,14 +2183,17 @@
                     "type": "object"
                 },
                 "schemaVersion": {
                     "description": "The schema version of an algorithm. Typically this value is not required.",
                     "title": "SchemaVersion",
                     "type": "integer"
                 },
+                "thresholdType": {
+                    "$ref": "#/definitions/ThresholdType"
+                },
                 "type": {
                     "enum": [
                         "stddev"
                     ],
                     "title": "Type",
                     "type": "string"
                 }
```

### Comparing `whylabs_toolkit-0.0.9/setup.py` & `whylabs_toolkit-0.1.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,39 +3,54 @@
 
 packages = \
 ['whylabs_toolkit',
  'whylabs_toolkit.cli',
  'whylabs_toolkit.container',
  'whylabs_toolkit.helpers',
  'whylabs_toolkit.monitor',
+ 'whylabs_toolkit.monitor.diagnoser',
+ 'whylabs_toolkit.monitor.diagnoser.converters',
+ 'whylabs_toolkit.monitor.diagnoser.helpers',
+ 'whylabs_toolkit.monitor.diagnoser.models',
+ 'whylabs_toolkit.monitor.diagnoser.recommendation',
  'whylabs_toolkit.monitor.manager',
  'whylabs_toolkit.monitor.models',
  'whylabs_toolkit.monitor.models.analyzer',
  'whylabs_toolkit.utils']
 
 package_data = \
 {'': ['*'], 'whylabs_toolkit.monitor': ['schema/*']}
 
 install_requires = \
 ['jsonschema>=4.17.3,<5.0.0',
- 'pydantic>=1.10.4,<2.0.0',
- 'whylabs-client>=0.5,<0.6',
+ 'pydantic>=1.10.15,<2.0.0',
+ 'typing-extensions>=4.11.0,<5.0.0',
+ 'urllib3>=2.0.2,<2.1',
+ 'whylabs-client>=0.6.3,<0.7.0',
  'whylogs>=1.1.26,<2.0.0']
 
+extras_require = \
+{'diagnoser': ['pandas>=2.0.3,<3.0.0',
+               'numpy>=1.24.1,<2.0.0',
+               'tabulate>=0.8.9,<0.9.0',
+               'isodate>=0.6.1,<0.7.0',
+               'python-dateutil>=2.8.2,<3.0.0']}
+
 setup_kwargs = {
     'name': 'whylabs-toolkit',
-    'version': '0.0.9',
-    'description': 'Whylabs CLI and Helpers package.',
-    'long_description': "# WhyLabs Toolkit\n\nThe WhyLabs Toolkit package contains helper methods to help users interact with our internal APIs. Users will benefit from using it if they want to abstract some of WhyLabs' internal logic and also automate recurring API calls.\n\n\n## Basic usage\nTo start using the `whylabs_toolkit` package, install it from PyPI with:\n```bash\npip install whylabs_toolkit\n``` \n\n## Packages\n\nThe available packages that we have enable different use-cases for the `whylabs_toolkit`. To get started, navigate to one of the following sections and find useful tutorials there.\n\n| Package             | Usage                |\n|---------------------|----------------------|\n| [Monitor Manager](/whylabs_toolkit/monitor/manager/README.md) | Author and modify existing WhyLabs monitor with Python |\n| [WhyLabs Helpers](/whylabs_toolkit/helpers/README.md) | Interact with and modify your Datasets and ML Models specs in WhyLabs. |\n\n## Development\n\nTo start contributing, you will manage dependencies with [Poetry](https://python-poetry.org/) and also a handful of `Makefile` commands. To install all necessary dependencies and activate the virtual environment, run:\n\n```bash\nmake setup && poetry shell\n```\n\n## Get in touch\nIf you want to learn more how you can benefit from this package or if there is anything missing, please [contact our support](https://whylabs.ai/contact-us), we'll be more than happy to help you!",
-    'author': 'Anthony Naddeo',
-    'author_email': 'anthony.naddeo@gmail.com',
+    'version': '0.1.0',
+    'description': 'Whylabs Toolkit package.',
+    'long_description': "# WhyLabs Toolkit\n\nThe WhyLabs Toolkit package contains helper methods to help users interact with our internal APIs. Users will benefit from using it if they want to abstract some of WhyLabs' internal logic and also automate recurring API calls.\n\n\n## Basic usage\nTo start using the `whylabs_toolkit` package, install it from PyPI with:\n```bash\npip install whylabs_toolkit\n``` \n\n## Packages\n\nThe available packages that we have enable different use-cases for the `whylabs_toolkit`. To get started, navigate to one of the following sections and find useful tutorials there.\n\n| Package                                                                                                                   | Usage                                                                  |\n|---------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------|\n| [Monitor Manager](https://github.com/whylabs/whylabs-toolkit/blob/mainline/whylabs_toolkit/monitor/manager/README.md)     | Author and modify existing WhyLabs monitor with Python.                |\n| [Monitor Diagnoser](https://github.com/whylabs/whylabs-toolkit/blob/mainline/whylabs_toolkit/monitor/diagnoser/README.md) | Diagnose problems with monitors.                                       |\n| [WhyLabs Helpers](https://github.com/whylabs/whylabs-toolkit/blob/mainline/whylabs_toolkit/helpers/README.md)             | Interact with and modify your Datasets and ML Models specs in WhyLabs. |\n\n## Development\n\nTo start contributing, you will manage dependencies with [Poetry](https://python-poetry.org/) and also a handful of `Makefile` commands. To install all necessary dependencies and activate the virtual environment, run:\n\n```bash\nmake setup && poetry shell\n```\n\n## Get in touch\nIf you want to learn more how you can benefit from this package or if there is anything missing, please [contact our support](https://whylabs.ai/contact-us), we'll be more than happy to help you!",
+    'author': 'Murilo Mendonca',
+    'author_email': 'murilommen@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'extras_require': extras_require,
     'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

