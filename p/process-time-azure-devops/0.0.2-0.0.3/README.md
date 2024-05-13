# Comparing `tmp/process_time_azure_devops-0.0.2.tar.gz` & `tmp/process_time_azure_devops-0.0.3.tar.gz`

## Comparing `process_time_azure_devops-0.0.2.tar` & `process_time_azure_devops-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.2/azure-pipelines.yml
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.2/.github/workflows/pr.yml
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.2/.idea/.gitignore
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.2/.idea/process-time-azure-devops.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.2/.idea/vcs.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.2/src/__init__.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.2/src/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.2/src/arts/__init__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.2/src/arts/process_time_logo.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.2/src/models/ArgumentParseResult.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.2/src/models/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.2/src/parsers/__init__.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.2/src/parsers/get_last_attempt_to_deliver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.2/tests/generate_test_run.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.2/tests/test_get_last_attempt_to_deliver.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.2/LICENSE
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.2/README.md
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/azure-pipelines.yml
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/.github/workflows/pr.yml
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/.idea/.gitignore
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/.idea/misc.xml
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/.idea/modules.xml
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/.idea/process-time-azure-devops.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/.idea/vcs.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/src/process_time_azure_devops/__init__.py
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/src/process_time_azure_devops/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/src/process_time_azure_devops/arts/__init__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/src/process_time_azure_devops/arts/process_time_logo.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/src/process_time_azure_devops/models/ArgumentParseResult.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/src/process_time_azure_devops/models/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/src/process_time_azure_devops/parsers/__init__.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/src/process_time_azure_devops/parsers/get_last_attempt_to_deliver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/tests/generate_test_run.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/tests/test_get_last_attempt_to_deliver.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/LICENSE
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/README.md
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/PKG-INFO
```

### Comparing `process_time_azure_devops-0.0.2/azure-pipelines.yml` & `process_time_azure_devops-0.0.3/azure-pipelines.yml`

 * *Files 12% similar despite different names*

```diff
@@ -29,11 +29,11 @@
     orgname="worldpwn"
     echo "orgname=$orgname"
     token=$(System.AccessToken)
     project="process-time"
     echo "project=$project"
     pipeline_id=2
     echo "pipeline_id=$pipeline_id"
-    python src/__main__.py --org "$orgname" --token "$token" --project "$project" --pipeline-id "$pipeline_id"
+    python src/process_time_azure_devops/__main__.py --org "$orgname" --token "$token" --project "$project" --pipeline-id "$pipeline_id"
   displayName: 'Test — Example Run Trunk Based'
   env:
     System.AccessToken: $(System.AccessToken)
```

### Comparing `process_time_azure_devops-0.0.2/.github/workflows/pr.yml` & `process_time_azure_devops-0.0.3/.github/workflows/pr.yml`

 * *Files 25% similar despite different names*

```diff
@@ -53,11 +53,35 @@
           python-version: ${{ env.PYTHON_VERSION }}
       - name: Install Dependencies
         run: |
           python -m pip install --upgrade pip
           pip install .[test]
       - name: Test Help -h
         run: |
-          python src/__main__.py -h
+          python src/process_time_azure_devops/__main__.py -h
       - name: Test Help --help
         run: |
-          python src/__main__.py --help
+          python src/process_time_azure_devops/__main__.py --help
+  
+  test_install_and_use:
+    name: Tests — Install & use CLI Arguments
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
+        with:
+          python-version: ${{ env.PYTHON_VERSION }}
+      - name: Install Dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install .[test]
+      - name: Build
+        run: |
+          pip install build
+          python -m build .
+      - name: Install
+        run: |
+          pip install dist/process_time_azure_devops-0.0.3-py3-none-any.whl
+      - name: Test Help -h
+        run: |
+          pip list
+          python -m process_time_azure_devops -h
```

### Comparing `process_time_azure_devops-0.0.2/.github/workflows/publish.yml` & `process_time_azure_devops-0.0.3/.github/workflows/publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   release:
     types: [created]
   workflow_dispatch: 
 
     
 jobs:
   build:
-    name: Build
+    name: Build and Publish
     runs-on: ubuntu-latest
     permissions:
       id-token: write
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
```

### Comparing `process_time_azure_devops-0.0.2/src/__main__.py` & `process_time_azure_devops-0.0.3/src/process_time_azure_devops/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from azure.devops.v7_1.pipelines.pipelines_client import PipelinesClient
-from parsers.get_last_attempt_to_deliver import get_last_attempt_to_deliver
-from models.ArgumentParseResult import ArgumentParseResult
-from arts.process_time_logo import process_time_logo
+from process_time_azure_devops.parsers.get_last_attempt_to_deliver import get_last_attempt_to_deliver
+from process_time_azure_devops.models.ArgumentParseResult import ArgumentParseResult
+from process_time_azure_devops.arts.process_time_logo import process_time_logo
 from msrest.authentication import BasicAuthentication
 import getopt
 import sys
 import json
 
 
 def display_help():
```

### Comparing `process_time_azure_devops-0.0.2/src/parsers/get_last_attempt_to_deliver.py` & `process_time_azure_devops-0.0.3/src/process_time_azure_devops/parsers/get_last_attempt_to_deliver.py`

 * *Files identical despite different names*

### Comparing `process_time_azure_devops-0.0.2/tests/test_get_last_attempt_to_deliver.py` & `process_time_azure_devops-0.0.3/tests/test_get_last_attempt_to_deliver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from azure.devops.v7_1.pipelines.models import Run
-from src.parsers.get_last_attempt_to_deliver import get_last_attempt_to_deliver
+from process_time_azure_devops.parsers.get_last_attempt_to_deliver import get_last_attempt_to_deliver
 from tests.generate_test_run import generate_test_run
 
 
 def test_only_current_run_exist_should_return_current_run():
     current_run = generate_test_run(3, 'succeeded')
     pipelines = [current_run]
     result = get_last_attempt_to_deliver(pipelines)
```

### Comparing `process_time_azure_devops-0.0.2/.gitignore` & `process_time_azure_devops-0.0.3/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -154,7 +154,8 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+.DS_Store
```

### Comparing `process_time_azure_devops-0.0.2/LICENSE` & `process_time_azure_devops-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `process_time_azure_devops-0.0.2/pyproject.toml` & `process_time_azure_devops-0.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 requires = [
     "hatchling==1.24.2",
     "azure-devops==7.1.0b4",
 ]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
-packages = ["src"]
+packages = ["src/process_time_azure_devops"]
 
 [project]
 name = "process_time_azure_devops"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name="Andrei Kniazev" },
 ]
 description = "Will collect process time for projects that are hosted in Azure DevOps"
 readme = "README.md"
 requires-python = ">=3.8"
 license = "GPL-3.0-or-later"
```

### Comparing `process_time_azure_devops-0.0.2/PKG-INFO` & `process_time_azure_devops-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: process_time_azure_devops
-Version: 0.0.2
+Version: 0.0.3
 Summary: Will collect process time for projects that are hosted in Azure DevOps
 Project-URL: GitHub, https://github.com/worldpwn/process-time-azure-devops
 Project-URL: Issues, https://github.com/worldpwn/process-time-azure-devops/issues
 Author: Andrei Kniazev
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
```

