# Comparing `tmp/kadet-0.3.1.tar.gz` & `tmp/kadet-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kadet-0.3.1.tar", max compression
+gzip compressed data, was "kadet-0.3.2.tar", max compression
```

## Comparing `kadet-0.3.1.tar` & `kadet-0.3.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
-drwxr-xr-x   0        0        0        0 2024-03-30 16:51:54.913657 kadet-0.3.1/LICENSES/
--rw-r--r--   0        0        0    10280 2024-03-30 16:51:54.913657 kadet-0.3.1/LICENSES/Apache-2.0.txt
--rw-r--r--   0        0        0     4673 2024-03-30 16:51:54.917657 kadet-0.3.1/README.md
--rw-r--r--   0        0        0     8447 2024-03-30 16:51:54.917657 kadet-0.3.1/kadet/__init__.py
--rw-r--r--   0        0        0     1129 2024-03-30 16:51:54.917657 kadet-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     5705 1970-01-01 00:00:00.000000 kadet-0.3.1/PKG-INFO
+drwxr-xr-x   0        0        0        0 2024-05-13 13:51:31.195899 kadet-0.3.2/LICENSES/
+-rw-r--r--   0        0        0    10280 2024-05-13 13:51:31.195899 kadet-0.3.2/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0     4673 2024-05-13 13:51:31.195899 kadet-0.3.2/README.md
+-rw-r--r--   0        0        0     8447 2024-05-13 13:51:31.195899 kadet-0.3.2/kadet/__init__.py
+-rw-r--r--   0        0        0     1130 2024-05-13 13:51:31.195899 kadet-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5704 1970-01-01 00:00:00.000000 kadet-0.3.2/PKG-INFO
```

### Comparing `kadet-0.3.1/LICENSES/Apache-2.0.txt` & `kadet-0.3.2/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `kadet-0.3.1/README.md` & `kadet-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `kadet-0.3.1/kadet/__init__.py` & `kadet-0.3.2/kadet/__init__.py`

 * *Files identical despite different names*

### Comparing `kadet-0.3.1/pyproject.toml` & `kadet-0.3.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kadet"
-version = "0.3.1"
+version = "0.3.2"
 description = "Easily define and reuse complex Python objects that serialize into JSON or YAML."
 homepage = "https://github.com/kapicorp/kadet"
 repository = "https://github.com/kapicorp/kadet"
 readme = "README.md"
 keywords = ["config", "kapitan", "kadet", "yaml", "json"]
 authors = ["Ricardo Amaro <ramaro@kapicorp.com>"]
 license = "Apache License 2.0"
@@ -18,15 +18,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
 python = '>=3.10'
 PyYAML = ">=5.3.1"
 typeguard = ">=3.0.0"
-python-box = "6.0.2"
+python-box = ">6.0.0"
 pydantic = ">=2.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^7.0.0"
```

### Comparing `kadet-0.3.1/PKG-INFO` & `kadet-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kadet
-Version: 0.3.1
+Version: 0.3.2
 Summary: Easily define and reuse complex Python objects that serialize into JSON or YAML.
 Home-page: https://github.com/kapicorp/kadet
 License: Apache-2.0
 Keywords: config,kapitan,kadet,yaml,json
 Author: Ricardo Amaro
 Author-email: ramaro@kapicorp.com
 Requires-Python: >=3.10
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: PyYAML (>=5.3.1)
 Requires-Dist: pydantic (>=2.0)
-Requires-Dist: python-box (==6.0.2)
+Requires-Dist: python-box (>6.0.0)
 Requires-Dist: typeguard (>=3.0.0)
 Project-URL: Repository, https://github.com/kapicorp/kadet
 Description-Content-Type: text/markdown
 
 # kadet
 
 Easily define and reuse complex Python objects that serialize into JSON or YAML.
```

