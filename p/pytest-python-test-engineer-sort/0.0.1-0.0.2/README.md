# Comparing `tmp/pytest_python_test_engineer_sort-0.0.1.tar.gz` & `tmp/pytest_python_test_engineer_sort-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_python_test_engineer_sort-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_python_test_engineer_sort-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_python_test_engineer_sort-0.0.1.tar` & `pytest_python_test_engineer_sort-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     4413 2024-05-12 09:34:08.153491 pytest_python_test_engineer_sort-0.0.1/.vscode/settings.json
--rw-r--r--   0        0        0     1099 2024-05-12 09:34:08.154706 pytest_python_test_engineer_sort-0.0.1/LICENSE
--rw-r--r--   0        0        0     6726 2024-05-12 09:34:08.155213 pytest_python_test_engineer_sort-0.0.1/README.md
--rw-r--r--   0        0        0      920 2024-05-13 16:51:51.983405 pytest_python_test_engineer_sort-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       81 2024-05-12 09:34:08.160718 pytest_python_test_engineer_sort-0.0.1/pytest.ini
--rw-r--r--   0        0        0      879 2024-05-12 09:34:08.160718 pytest_python_test_engineer_sort-0.0.1/pytest_sort.py
--rw-r--r--   0        0        0       26 2024-05-12 09:34:08.162500 pytest_python_test_engineer_sort-0.0.1/requirements.txt
--rw-r--r--   0        0        0      212 2024-05-12 09:34:08.166360 pytest_python_test_engineer_sort-0.0.1/src/test_sort.py
--rw-r--r--   0        0        0       31 2024-05-12 09:34:08.172168 pytest_python_test_engineer_sort-0.0.1/tests/conftest.py
--rw-r--r--   0        0        0     1320 2024-05-12 09:34:08.172168 pytest_python_test_engineer_sort-0.0.1/tests/test_plugin.py
--rw-r--r--   0        0        0     7005 1970-01-01 00:00:00.000000 pytest_python_test_engineer_sort-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      230 2024-05-13 17:00:24.203408 pytest_python_test_engineer_sort-0.0.2/.pypirc
+-rw-r--r--   0        0        0     4413 2024-05-12 09:34:08.153491 pytest_python_test_engineer_sort-0.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0     1099 2024-05-12 09:34:08.154706 pytest_python_test_engineer_sort-0.0.2/LICENSE
+-rw-r--r--   0        0        0     7133 2024-05-13 17:03:24.850035 pytest_python_test_engineer_sort-0.0.2/README.md
+-rw-r--r--   0        0        0      920 2024-05-13 17:03:41.187683 pytest_python_test_engineer_sort-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       81 2024-05-12 09:34:08.160718 pytest_python_test_engineer_sort-0.0.2/pytest.ini
+-rw-r--r--   0        0        0      879 2024-05-12 09:34:08.160718 pytest_python_test_engineer_sort-0.0.2/pytest_sort.py
+-rw-r--r--   0        0        0       26 2024-05-12 09:34:08.162500 pytest_python_test_engineer_sort-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      212 2024-05-12 09:34:08.166360 pytest_python_test_engineer_sort-0.0.2/src/test_sort.py
+-rw-r--r--   0        0        0       31 2024-05-12 09:34:08.172168 pytest_python_test_engineer_sort-0.0.2/tests/conftest.py
+-rw-r--r--   0        0        0     1320 2024-05-12 09:34:08.172168 pytest_python_test_engineer_sort-0.0.2/tests/test_plugin.py
+-rw-r--r--   0        0        0     7402 1970-01-01 00:00:00.000000 pytest_python_test_engineer_sort-0.0.2/PKG-INFO
```

### Comparing `pytest_python_test_engineer_sort-0.0.1/.vscode/settings.json` & `pytest_python_test_engineer_sort-0.0.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `pytest_python_test_engineer_sort-0.0.1/LICENSE` & `pytest_python_test_engineer_sort-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_python_test_engineer_sort-0.0.1/README.md` & `pytest_python_test_engineer_sort-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -175,8 +175,18 @@
 
 If these tests pass then we can feel assured that our plugin works satisfactorily as a plugin and we have also tested the functionality of the plugin code to sort test names alphabetically.
 
 If you change the plugin_sort.py or any other plugin file, uninstall the plugin, delete the dist folder and then rebuild and install.
 
 To uninstall the plugin:
 
-`pip uninstall .\dist\pytest_sort-0.0.1-py3-none-any.whl` (change .whl name as per your project).
+`pip uninstall .\dist\pytest_sort-0.0.1-py3-none-any.whl` (change .whl name as per your project).
+
+upload issues:
+
+- pip install keyring if using usb
+- CTRL+SHIFT+C/V for password on Windows
+- flit --repository testpypi publish
+- ensure git commit done
+
+https://github.com/pypa/flit/issues/122
+I'll leave this open for now because it could be better documented, and I'm considering whether we should support testpypi as a repository without the user needing to configure their .pypirc manually.
```

### Comparing `pytest_python_test_engineer_sort-0.0.1/pyproject.toml` & `pytest_python_test_engineer_sort-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "pytest-python-test-engineer-sort" # PyPi prefers dashes so replace underscores with dashes
 
 authors = [{ name = "Craig West", email = "craig@example.com" }]
 readme = "README.md"
 classifiers = ["License :: OSI Approved :: MIT License", "Framework :: Pytest"]
 # dynamic = ["version", "description"]
-version = "0.0.1"
+version = "0.0.2"
 description = "Sort plugin for Pytest"
 dependencies = ["pytest>=6.2.0"]
 requires-python = ">=3.7"
 
 
 [project.urls]
 Home = "https://github.com/python-test-engineer/Udemy-PyTest"
```

### Comparing `pytest_python_test_engineer_sort-0.0.1/pytest_sort.py` & `pytest_python_test_engineer_sort-0.0.2/pytest_sort.py`

 * *Files identical despite different names*

### Comparing `pytest_python_test_engineer_sort-0.0.1/tests/test_plugin.py` & `pytest_python_test_engineer_sort-0.0.2/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_python_test_engineer_sort-0.0.1/PKG-INFO` & `pytest_python_test_engineer_sort-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-python-test-engineer-sort
-Version: 0.0.1
+Version: 0.0.2
 Summary: Sort plugin for Pytest
 Author-email: Craig West <craig@example.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: Pytest
 Requires-Dist: pytest>=6.2.0
@@ -190,7 +190,17 @@
 If these tests pass then we can feel assured that our plugin works satisfactorily as a plugin and we have also tested the functionality of the plugin code to sort test names alphabetically.
 
 If you change the plugin_sort.py or any other plugin file, uninstall the plugin, delete the dist folder and then rebuild and install.
 
 To uninstall the plugin:
 
 `pip uninstall .\dist\pytest_sort-0.0.1-py3-none-any.whl` (change .whl name as per your project).
+
+upload issues:
+
+- pip install keyring if using usb
+- CTRL+SHIFT+C/V for password on Windows
+- flit --repository testpypi publish
+- ensure git commit done
+
+https://github.com/pypa/flit/issues/122
+I'll leave this open for now because it could be better documented, and I'm considering whether we should support testpypi as a repository without the user needing to configure their .pypirc manually.
```

