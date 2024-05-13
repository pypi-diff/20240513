# Comparing `tmp/dhuodata_lib-0.3.7.tar.gz` & `tmp/dhuodata_lib-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhuodata_lib-0.3.7.tar", last modified: Fri May 10 14:25:06 2024, max compression
+gzip compressed data, was "dhuodata_lib-0.3.8.tar", last modified: Mon May 13 20:02:36 2024, max compression
```

## Comparing `dhuodata_lib-0.3.7.tar` & `dhuodata_lib-0.3.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-10 14:25:06.038252 dhuodata_lib-0.3.7/
--rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-10 14:25:06.038252 dhuodata_lib-0.3.7/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata_lib-0.3.7/README.md
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-05-10 14:25:06.038252 dhuodata_lib-0.3.7/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-05-10 14:24:24.000000 dhuodata_lib-0.3.7/setup.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-10 14:25:06.038252 dhuodata_lib-0.3.7/src/
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-10 14:25:06.038252 dhuodata_lib-0.3.7/src/dhuodata_lib.egg-info/
--rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-10 14:25:06.000000 dhuodata_lib-0.3.7/src/dhuodata_lib.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      445 2024-05-10 14:25:06.000000 dhuodata_lib-0.3.7/src/dhuodata_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-05-10 14:25:06.000000 dhuodata_lib-0.3.7/src/dhuodata_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)      152 2024-05-10 14:25:06.000000 dhuodata_lib-0.3.7/src/dhuodata_lib.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-05-10 14:25:06.000000 dhuodata_lib-0.3.7/src/dhuodata_lib.egg-info/top_level.txt
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-10 14:25:06.038252 dhuodata_lib-0.3.7/src/dhuolib/
--rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.7/src/dhuolib/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.7/src/dhuolib/auth.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     8143 2024-05-10 14:10:57.000000 dhuodata_lib-0.3.7/src/dhuolib/clients.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      348 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.7/src/dhuolib/config.py
--rw-rw-r--   0 diego     (1000) diego     (1000)       95 2024-05-09 16:59:36.000000 dhuodata_lib-0.3.7/src/dhuolib/enums.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.7/src/dhuolib/predict.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     3341 2024-05-10 13:47:21.000000 dhuodata_lib-0.3.7/src/dhuolib/services.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      790 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.7/src/dhuolib/validations.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.7/src/dhuolib/worker.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-10 14:25:06.038252 dhuodata_lib-0.3.7/tests/
--rw-rw-r--   0 diego     (1000) diego     (1000)     5207 2024-05-10 14:23:03.000000 dhuodata_lib-0.3.7/tests/test_dhuolib.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-13 20:02:36.471445 dhuodata_lib-0.3.8/
+-rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-13 20:02:36.471445 dhuodata_lib-0.3.8/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata_lib-0.3.8/README.md
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-05-13 20:02:36.471445 dhuodata_lib-0.3.8/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-05-13 20:02:28.000000 dhuodata_lib-0.3.8/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-13 20:02:36.467446 dhuodata_lib-0.3.8/src/
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-13 20:02:36.471445 dhuodata_lib-0.3.8/src/dhuodata_lib.egg-info/
+-rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-13 20:02:36.000000 dhuodata_lib-0.3.8/src/dhuodata_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      445 2024-05-13 20:02:36.000000 dhuodata_lib-0.3.8/src/dhuodata_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-05-13 20:02:36.000000 dhuodata_lib-0.3.8/src/dhuodata_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)      152 2024-05-13 20:02:36.000000 dhuodata_lib-0.3.8/src/dhuodata_lib.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-05-13 20:02:36.000000 dhuodata_lib-0.3.8/src/dhuodata_lib.egg-info/top_level.txt
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-13 20:02:36.471445 dhuodata_lib-0.3.8/src/dhuolib/
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.8/src/dhuolib/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.8/src/dhuolib/auth.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     8805 2024-05-13 19:55:08.000000 dhuodata_lib-0.3.8/src/dhuolib/clients.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      348 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.8/src/dhuolib/config.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)       95 2024-05-09 16:59:36.000000 dhuodata_lib-0.3.8/src/dhuolib/enums.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.8/src/dhuolib/predict.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     3393 2024-05-13 18:03:54.000000 dhuodata_lib-0.3.8/src/dhuolib/services.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      790 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.8/src/dhuolib/validations.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.8/src/dhuolib/worker.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-13 20:02:36.471445 dhuodata_lib-0.3.8/tests/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     5248 2024-05-13 19:59:14.000000 dhuodata_lib-0.3.8/tests/test_dhuolib.py
```

### Comparing `dhuodata_lib-0.3.7/PKG-INFO` & `dhuodata_lib-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.3.7
+Version: 0.3.8
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Requires-Dist: oci==2.125.3
 Requires-Dist: pydantic==1.8.2
```

### Comparing `dhuodata_lib-0.3.7/README.md` & `dhuodata_lib-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.3.7/setup.py` & `dhuodata_lib-0.3.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 README = ""
 if os.path.exists("README.md"):
     README = open("README.md").read()
 
 setup(
     name="dhuodata-lib",
-    version="0.3.7",
+    version="0.3.8",
     long_description=README,
     long_description_content_type="text/markdown",
     author="DHuO Data Team",
     author_email="diego.salles@engdb.com.br",
     url="https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib",
     install_requires=REQUIRED_PACKAGES,
     extras_require={"interactive": DEV_PACKAGES},
```

### Comparing `dhuodata_lib-0.3.7/src/dhuodata_lib.egg-info/PKG-INFO` & `dhuodata_lib-0.3.8/src/dhuodata_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.3.7
+Version: 0.3.8
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Requires-Dist: oci==2.125.3
 Requires-Dist: pydantic==1.8.2
```

### Comparing `dhuodata_lib-0.3.7/src/dhuolib/clients.py` & `dhuodata_lib-0.3.8/src/dhuolib/clients.py`

 * *Files 12% similar despite different names*

```diff
@@ -131,42 +131,43 @@
         except FileNotFoundError as e:
             logger.error(f"Error: {e}")
             return {"error": str(e)}
 
     def create_batch_project(self, project_name: str):
         if project_name is None:
             raise ValueError("project_name is required")
+        self.project_name = project_name
         response = self.service.create_project(project_name)
         return response
 
     def deploy_batch_project(self, script_filename: str, requirements_filename: str):
         if self.project_name is None:
             raise ValueError("Batch project is required")
 
         if script_filename is None or requirements_filename is None:
             raise ValueError("script_filename and requirements_filename are required")
 
         try:
             with open(script_filename, "rb") as script_file, open(requirements_filename, "rb") as requirements_file:
                 encoded_script = base64.b64encode(script_file.read())
                 encoded_requirements = base64.b64encode(requirements_file.read())
-                response = self.service.deploy_script(
-                    self.project_name, encoded_script, encoded_requirements)
+                response = self.service.deploy_script(project_name=self.project_name,
+                                                      script_file_encode=encoded_script,
+                                                      requirements_file_enconde=encoded_requirements)
                 return response
         except FileNotFoundError as e:
             logger.error(f"Error: {e}")
             return {"error": str(e)}
 
     def pipeline_status_report(self):
         lst = []
         if self.project_name is None:
             raise ValueError("Batch project is required")
         response = self.service.get_pipeline_status(self.project_name)
-        json_objects = json.loads(response.content)
-        for data in json_objects:
+        for data in response["data"]:
             lst.append({
                 "date_log": data["date_log"],
                 "step": data["step"],
                 "status": data["status"]
             })
         return lst
 
@@ -183,22 +184,31 @@
     def _batch_run(self):
         if self.project_name is None:
             raise ValueError("Batch project is required")
 
         response = self.service.run_pipeline(self.project_name)
         return response
      
-    def predict_batch(self, cluster_size: int, script_filename: str, requirements_filename: str):
+    def batch_execute(self, cluster_size: int, script_filename: str, requirements_filename: str):
         if self.project_name is None:
             raise ValueError("Batch project is required")
-        response = self.deploy_batch_project(script_filename, requirements_filename)
+        response = self.deploy_batch_project(script_filename=script_filename, requirements_filename=requirements_filename)
+        if response['code'] != 201:
+            return 'Error deploying batch project see pipeline status for more information'
+        
         logger.info(f"Deploy_batch_project {response} deployed")
         while True:
             status = self.pipeline_status_report()
-            if all([s["status"] == "DEPLOY COMPLETED SUCCESSFULLY" for s in status]):
+            if any([s["status"] == "DEPLOY COMPLETED SUCCESSFULLY" for s in status]):
                 break
-            time.sleep(30)
-        response = self._create_cluster(cluster_size)
+            logger.info(f"Deploy_batch_project {status[len(status)-1]['date_log']}")
+            logger.info(f"Deploy_batch_project {status[len(status)-1]['status']}")
+            logger.info("Process is running...")
+            time.sleep(60)
+        response = self._create_cluster(cluster_size=cluster_size)
+        if response['code'] != 201:
+            return response
         logger.info(f"Create_cluster {response}")
         response = self._batch_run()
-        logger.info(f"Batch Run {response}")
-        
+        if response['code'] != 201:
+            return response
+        logger.info(f"Batch Run {response}")
```

### Comparing `dhuodata_lib-0.3.7/src/dhuolib/predict.py` & `dhuodata_lib-0.3.8/src/dhuolib/predict.py`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.3.7/src/dhuolib/services.py` & `dhuodata_lib-0.3.8/src/dhuolib/services.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,65 +5,65 @@
 
 class ServiceAPIML:
     def __init__(self, service_endpoint):
 
         if not isinstance(service_endpoint, str):
             raise ValueError("service_endpoint must be a string")
 
-        self.service_endpoint = f"{service_endpoint}/api/experiment"
+        self.service_endpoint = f"{service_endpoint}/api"
         self.headers = {"Content-Type": "application/json"}
 
     def create_experiment_by_conf_json(self, experiment_params='', files=None):
         if experiment_params is None and isinstance(experiment_params, dict):
             raise ValueError("json_data must be a dict")
 
         if files:
             return requests.post(
-                f"{self.service_endpoint}/save",
+                f"{self.service_endpoint}/experiment/save",
                 data=experiment_params,
                 files=files
             )
 
         response = requests.post(
-            f"{self.service_endpoint}/save",
+            f"{self.service_endpoint}/experiment/save",
             data=json.dumps(experiment_params),
             headers=self.headers,
         )
         return response.json()
 
     def run_experiment(self, params={}, files=None):
         if params is None and isinstance(params, str):
             raise ValueError("json_data must be a dict")
 
         response = requests.post(
-            f"{self.service_endpoint}/run", data=params, files=files
+            f"{self.service_endpoint}/experiment/run", data=params, files=files
         )
         return response.json()
 
     def create_model(self, model_params):
         if model_params is None and not isinstance(model_params, dict):
             raise ValueError("json_data must be a dict")
         response = requests.post(
-            f"{self.service_endpoint}/model",
+            f"{self.service_endpoint}/experiment/model",
             data=json.dumps(model_params),
             headers=self.headers,
         )
         return response.json()
 
     def predict_online(self, params={}, files=None):
         if params is None and not isinstance(params, dict):
             raise ValueError("json_data must be a dict")
         response = requests.post(
-            f"{self.service_endpoint}/predict_online", data=params, files=files
+            f"{self.service_endpoint}/experiment/predict_online", data=params, files=files
         )
         return response.json()
 
     def create_project(self, project_name):
         body = {
-            'name': project_name
+            'project_name': project_name
         }
         response = requests.post(
             f"{self.service_endpoint}/project", json=body)
 
         return response.json()
 
     def deploy_script(self, project_name: str, script_file_encode: str, requirements_file_enconde: str):
```

### Comparing `dhuodata_lib-0.3.7/src/dhuolib/validations.py` & `dhuodata_lib-0.3.8/src/dhuolib/validations.py`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.3.7/tests/test_dhuolib.py` & `dhuodata_lib-0.3.8/tests/test_dhuolib.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from dhuolib.clients import DhuolibClient
 import sys
 import unittest
 from unittest.mock import patch, mock_open
 import base64
+from dhuolib.config import logger
 
 sys.path.append("src")
 
 
 class TestDhuolibUtils(unittest.TestCase):
     def setUp(self):
-        self.end_point = "http://localhost:8000"
+        self.end_point = "http://localhost:5000"
         self.dhuolib = DhuolibClient(
-            service_endpoint=self.end_point, project_name="TestProject")
+            service_endpoint=self.end_point, project_name="Test Project")
         self.file_path = "tests/files/LogisticRegression_best.pickle"
 
     def test_1_deve_lancar_excecao_com_valores_run_params_incorretos(self):
         experiment_params = {
             "experiment_tags": {"version": "v1", "priority": "P1"},
         }
         response = self.dhuolib.create_experiment(experiment_params)
@@ -106,25 +107,25 @@
         mock_response.json.return_value = {"status": "success", "project_id": 123}
         response = self.dhuolib.create_batch_project(project_name)
         self.assertEqual(response, {"status": "success", "project_id": 123})
 
     def test_7_create_batch_project_raises_exception_on_none(self):
         with self.assertRaises(ValueError) as context:
             self.dhuolib.create_batch_project(None)
-        self.assertTrue("project_name is required" in str(context.exception))
+            self.assertIn("project_name is required" in str(context.exception))
 
     def test_8_deploy_batch_project_no_project_name(self):
         self.dhuolib = DhuolibClient(service_endpoint=self.end_point)
         with self.assertRaises(ValueError) as context:
             self.dhuolib.deploy_batch_project("script.py", "requirements.txt")
-        self.assertTrue("Batch project is required" in str(context.exception))
+            self.assertIn("Batch project is required" in str(context.exception))
 
     def test_9_deploy_batch_project_missing_files(self):
         with self.assertRaises(ValueError) as context:
             self.dhuolib.deploy_batch_project(None, None)
-        self.assertTrue(
+            self.assertIn(
             "script_filename and requirements_filename are required" in str(context.exception))
 
     def test_10_deploy_batch_project_file_not_found(self):
         with patch("builtins.open", side_effect=FileNotFoundError("File not found")):
             response = self.dhuolib.deploy_batch_project("script.py", "requirements.txt")
             self.assertEqual(response, {"error": "File not found"})
```

