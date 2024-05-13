# Comparing `tmp/sanauautomationsdk-1.0.8.tar.gz` & `tmp/sanauautomationsdk-1.0.9.tar.gz`

## Comparing `sanauautomationsdk-1.0.8.tar` & `sanauautomationsdk-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,67 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.8/src/__init__.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.8/src/SanauAutomationSDK/Api.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.8/src/SanauAutomationSDK/Base.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.8/src/SanauAutomationSDK/Client.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.8/src/SanauAutomationSDK/FileVault.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.8/src/SanauAutomationSDK/OGD.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.8/src/SanauAutomationSDK/Oked.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.8/src/SanauAutomationSDK/SanauAutomationSDK.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.8/src/SanauAutomationSDK/__init__.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.8/src/SanauAutomationSDK/config.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.8/src/SanauAutomationSDK/utils/decorators.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.8/tests/main.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.8/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.8/LICENSE
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.8/README.md
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/src/__init__.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/src/SanauAutomationSDK/Worker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/src/SanauAutomationSDK/__init__.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/src/SanauAutomationSDK/config.py
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/src/SanauAutomationSDK/api/Arm.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/src/SanauAutomationSDK/api/OneS.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/src/SanauAutomationSDK/api/Wrapper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/src/SanauAutomationSDK/api/__init__.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/src/SanauAutomationSDK/api/arm/handlers/AlertsHandler.py
+-rw-r--r--   0        0        0     3800 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/src/SanauAutomationSDK/api/arm/handlers/TasksHandler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/src/SanauAutomationSDK/api/arm/handlers/__init__.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/src/SanauAutomationSDK/api/arm/models/Task.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/src/SanauAutomationSDK/classes/ArmApiCredentials.py
+-rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/src/SanauAutomationSDK/controllers/JobsController.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/src/SanauAutomationSDK/utils/decorators.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/src/SanauAutomationSDK/utils/logutils.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/tests/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/tests/storage/logs/dispatcher.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/tests/storage/logs/health.log
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/tests/storage/logs/info.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/__init__.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/Worker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/__init__.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/config.py
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/api/Arm.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/api/OneS.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/api/Wrapper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/api/__init__.py
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/api/arm/handlers/AlertsHandler.py
+-rw-r--r--   0        0        0     5298 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/api/arm/handlers/DB1CHandler.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/api/arm/handlers/DatabasesHandler.py
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/api/arm/handlers/TasksHandler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/api/arm/handlers/__init__.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/api/arm/models/Alert.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/api/arm/models/DB1C.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/api/arm/models/Task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/api/arm/models/__init__.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/api/one_s/entities/ODataEntity.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/api/one_s/entities/User.py
+-rw-r--r--   0        0        0     6488 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/api/one_s/entities/common_entities.py
+-rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/api/one_s/handlers/ODataHandler.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/api/one_s/handlers/UsersHandler.py
+-rw-r--r--   0        0        0     7465 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/api/one_s/handlers/common_handlers.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/classes/ArmApiCredentials.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/classes/DatabaseCredentials.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/classes/OneSApiCredentials.py
+-rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/controllers/BaseController.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/controllers/CountriesController.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/controllers/DatabasesController.py
+-rw-r--r--   0        0        0     8326 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/controllers/JobsController.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/controllers/TestsController.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/database/DB.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/database/migrations/Migrations.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/database/models/BaseModel.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/database/models/Country.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/database/models/Database.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/database/models/Job.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/database/models/Test.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/exceptions/odata.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/storage/job_relations.json
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/utils/decorators.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/utils/logutils.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/LICENSE
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/README.md
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 sanauautomationsdk-1.0.9/PKG-INFO
```

### Comparing `sanauautomationsdk-1.0.8/src/SanauAutomationSDK/config.py` & `sanauautomationsdk-1.0.9/src/SanauAutomationSDK/config.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,31 @@
 # GET
-ONE_S_DATABASES = 'https://{domain}/botapi/v1/one_s/databases'
-ARM_EMPLOYEES = 'https://{domain}/botapi/v1/one_s/databases/{db_name}/employees'
-FILE_VAULT_DOWNLOAD_FILE = 'https://files.{domain}/download/file'
-NATIONAL_BANK = 'https://nationalbank.kz/rss/get_rates.cfm?fdate={currency_date}'
-OGD_EXCEL = 'https://kgd.gov.kz/sites/default/files/spravochniki/spravochnik_kodifikator_s_ukazaniem_bin_i_rekvizitami_dlya_zachisleniya_platezhey_v_byudzhet_po_organam_gosudarstvennyh_dohodov_respubliki_kazahstan.xlsx'
-DOMAINS = 'https://auth.sanau.kz/domains_without_devs'
-GET_ALERT = 'https://{domain}/botapi/v1/alert'
-OKEDS = 'https://{domain}/api/v3/python_integration/get_all_okeds'
+ONE_S_DATABASES = "https://{domain}/botapi/v1/one_s/databases"
+ONE_S_DATABASE = "https://{domain}/botapi/v1/one_s/database/{database}"
+ARM_EMPLOYEES = "https://{domain}/botapi/v1/one_s/databases/{db_name}/employees"
+MY_NEW_TASKS = "https://{domain}/botapi/v1/tasks/my?status=new"
+LAST_NEW_TASK = "https://{domain}/botapi/v1/tasks/last_new_task"
+TASKS = "https://{domain}/botapi/v1/tasks"
+TASKS_WITH_STATUS = "https://{domain}/botapi/v1/tasks?status={status}"
+FILE_VAULT_DOWNLOAD_FILE = 'https://files.sanau.kz/{domain.split(".")[0]}/download/file'
+NATIONAL_BANK = "https://nationalbank.kz/rss/get_rates.cfm?fdate={currency_date}"
+OGD_EXCEL = "https://kgd.gov.kz/sites/default/files/spravochniki/spravochnik_kodifikator_s_ukazaniem_bin_i_rekvizitami_dlya_zachisleniya_platezhey_v_byudzhet_po_organam_gosudarstvennyh_dohodov_respubliki_kazahstan.xlsx"
+DOMAINS = "https://auth.sanau.kz/domains_without_devs"
+GET_ALERT = "https://{domain}/botapi/v1/alert"
+OKEDS = "https://{domain}/api/v3/python_integration/get_all_okeds"
 
 # POST
-POST_ALERTS = 'https://{domain}/botapi/v1/alerts'
-FETCH_TAXATION_ORGANS = 'https://{domain}/api/v3/python_integration/fetch_taxation_organs'
+POST_ALERTS = "https://{domain}/botapi/v1/alerts"
+FETCH_TAXATION_ORGANS = "https://{domain}/api/v3/python_integration/fetch_taxation_organs"
+POST_TASK_COMMENT = "https://{domain}/botapi/v1/tasks/{task_id}/comments"
 
 # PUT
-RESOLVE_ALERT = 'https://{domain}/botapi/v1/alerts/resolve'
+RESOLVE_ALERT = "https://{domain}/botapi/v1/alerts/resolve"
+UPDATE_TASK_STATUS = "https://{domain}/botapi/v1/tasks/{task_id}"
 
 # DELETE
-RESOLVE_ALL_ALERTS = 'https://{domain}/botapi/v1/alerts/resolve_all'
+RESOLVE_ALL_ALERTS = "https://{domain}/botapi/v1/alerts/resolve_all"
+DELETE_TASK_COMMENTS = "https://{domain}/botapi/v1/tasks/{task_id}/comments/destroy_all"
+
+
+# ODATA
+ODATA_REQUEST_BASE_URL = "http://{server}/{database_name}/odata/standard.odata/"
```

### Comparing `sanauautomationsdk-1.0.8/src/SanauAutomationSDK/utils/decorators.py` & `sanauautomationsdk-1.0.9/unfinished_version/SanauAutomationSDK/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `sanauautomationsdk-1.0.8/LICENSE` & `sanauautomationsdk-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sanauautomationsdk-1.0.8/README.md` & `sanauautomationsdk-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sanauautomationsdk-1.0.8/pyproject.toml` & `sanauautomationsdk-1.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/SanauAutomationSDK/"]
 
 [project]
 name = "SanauAutomationSDK"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
     { name="victor.ten", email="prostobackoffice@gmail.com" },
     { name="NotFakeL1eN", email="notfakel1en@gmail.com" },
     { name="BaturinMaksim188", email="Baturinmaksim188@gmail.com"},
 ]
 description = "SDK that simplifies work with outsourcing"
 readme = "README.md"
 dependencies = [
     'requests',
+    'peewee',
 ]
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `sanauautomationsdk-1.0.8/PKG-INFO` & `sanauautomationsdk-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.3
 Name: SanauAutomationSDK
-Version: 1.0.8
+Version: 1.0.9
 Summary: SDK that simplifies work with outsourcing
 Project-URL: Homepage, https://github.com/sanau-kz/python-automation-sdk
 Project-URL: Issues, https://github.com/sanau-kz/python-automation-sdk/issues
 Author-email: "victor.ten" <prostobackoffice@gmail.com>, NotFakeL1eN <notfakel1en@gmail.com>, BaturinMaksim188 <Baturinmaksim188@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: peewee
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # <font color="#3498DB">Sanau Automation SDK</font>
 
 This is **package for python** that you can install by:  
 ```pip install SanauAutomationSDK```
```

