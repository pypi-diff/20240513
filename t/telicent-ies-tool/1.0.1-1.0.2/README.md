# Comparing `tmp/telicent-ies-tool-1.0.1.tar.gz` & `tmp/telicent_ies_tool-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telicent-ies-tool-1.0.1.tar", last modified: Tue Mar 19 09:08:57 2024, max compression
+gzip compressed data, was "telicent_ies_tool-1.0.2.tar", last modified: Mon May 13 14:47:04 2024, max compression
```

## Comparing `telicent-ies-tool-1.0.1.tar` & `telicent_ies_tool-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:08:57.335946 telicent-ies-tool-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-03-19 09:08:50.000000 telicent-ies-tool-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-19 09:08:50.000000 telicent-ies-tool-1.0.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)    17426 2024-03-19 09:08:57.335946 telicent-ies-tool-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-03-19 09:08:50.000000 telicent-ies-tool-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:08:57.335946 telicent-ies-tool-1.0.1/ies_tool/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-19 09:08:50.000000 telicent-ies-tool-1.0.1/ies_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   267370 2024-03-19 09:08:50.000000 telicent-ies-tool-1.0.1/ies_tool/ies4.ttl
--rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-03-19 09:08:50.000000 telicent-ies-tool-1.0.1/ies_tool/iesExtensions.ttl
--rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-03-19 09:08:50.000000 telicent-ies-tool-1.0.1/ies_tool/ies_ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-19 09:08:50.000000 telicent-ies-tool-1.0.1/ies_tool/ies_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)   962532 2024-03-19 09:08:50.000000 telicent-ies-tool-1.0.1/ies_tool/ies_r4_2_0.shacl
--rw-r--r--   0 runner    (1001) docker     (127)    83277 2024-03-19 09:08:50.000000 telicent-ies-tool-1.0.1/ies_tool/ies_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-03-19 09:08:50.000000 telicent-ies-tool-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 09:08:57.335946 telicent-ies-tool-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:08:57.335946 telicent-ies-tool-1.0.1/telicent_ies_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17426 2024-03-19 09:08:57.000000 telicent-ies-tool-1.0.1/telicent_ies_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-19 09:08:57.000000 telicent-ies-tool-1.0.1/telicent_ies_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 09:08:57.000000 telicent-ies-tool-1.0.1/telicent_ies_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-19 09:08:57.000000 telicent-ies-tool-1.0.1/telicent_ies_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-19 09:08:57.000000 telicent-ies-tool-1.0.1/telicent_ies_tool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:08:57.335946 telicent-ies-tool-1.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-03-19 09:08:50.000000 telicent-ies-tool-1.0.1/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:47:04.624571 telicent_ies_tool-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-13 14:46:59.000000 telicent_ies_tool-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-13 14:46:59.000000 telicent_ies_tool-1.0.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)    25951 2024-05-13 14:47:04.624571 telicent_ies_tool-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11370 2024-05-13 14:46:59.000000 telicent_ies_tool-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:47:04.620571 telicent_ies_tool-1.0.2/ies_tool/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-13 14:46:59.000000 telicent_ies_tool-1.0.2/ies_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267370 2024-05-13 14:46:59.000000 telicent_ies_tool-1.0.2/ies_tool/ies4.ttl
+-rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-05-13 14:46:59.000000 telicent_ies_tool-1.0.2/ies_tool/iesExtensions.ttl
+-rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-05-13 14:46:59.000000 telicent_ies_tool-1.0.2/ies_tool/ies_ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-13 14:46:59.000000 telicent_ies_tool-1.0.2/ies_tool/ies_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   962532 2024-05-13 14:46:59.000000 telicent_ies_tool-1.0.2/ies_tool/ies_r4_2_0.shacl
+-rw-r--r--   0 runner    (1001) docker     (127)   122190 2024-05-13 14:46:59.000000 telicent_ies_tool-1.0.2/ies_tool/ies_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-13 14:46:59.000000 telicent_ies_tool-1.0.2/ies_tool/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-13 14:46:59.000000 telicent_ies_tool-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:47:04.624571 telicent_ies_tool-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:47:04.620571 telicent_ies_tool-1.0.2/telicent_ies_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25951 2024-05-13 14:47:04.000000 telicent_ies_tool-1.0.2/telicent_ies_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-13 14:47:04.000000 telicent_ies_tool-1.0.2/telicent_ies_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:47:04.000000 telicent_ies_tool-1.0.2/telicent_ies_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-13 14:47:04.000000 telicent_ies_tool-1.0.2/telicent_ies_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-13 14:47:04.000000 telicent_ies_tool-1.0.2/telicent_ies_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:47:04.620571 telicent_ies_tool-1.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-13 14:46:59.000000 telicent_ies_tool-1.0.2/test/test.py
```

### Comparing `telicent-ies-tool-1.0.1/LICENSE` & `telicent_ies_tool-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `telicent-ies-tool-1.0.1/ies_tool/__init__.py` & `telicent_ies_tool-1.0.2/ies_tool/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,7 +9,8 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
+
```

### Comparing `telicent-ies-tool-1.0.1/ies_tool/ies4.ttl` & `telicent_ies_tool-1.0.2/ies_tool/ies4.ttl`

 * *Files identical despite different names*

### Comparing `telicent-ies-tool-1.0.1/ies_tool/iesExtensions.ttl` & `telicent_ies_tool-1.0.2/ies_tool/iesExtensions.ttl`

 * *Files identical despite different names*

### Comparing `telicent-ies-tool-1.0.1/ies_tool/ies_ontology.py` & `telicent_ies_tool-1.0.2/ies_tool/ies_ontology.py`

 * *Files identical despite different names*

### Comparing `telicent-ies-tool-1.0.1/ies_tool/ies_plugin.py` & `telicent_ies_tool-1.0.2/ies_tool/ies_plugin.py`

 * *Files identical despite different names*

### Comparing `telicent-ies-tool-1.0.1/ies_tool/ies_r4_2_0.shacl` & `telicent_ies_tool-1.0.2/ies_tool/ies_r4_2_0.shacl`

 * *Files identical despite different names*

### Comparing `telicent-ies-tool-1.0.1/pyproject.toml` & `telicent_ies_tool-1.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 [build-system]
 requires = ["setuptools>=61.2.0", "wheel==0.41.3", "pip-tools==7.3.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "telicent-ies-tool"
-version = "1.0.1"
+version = "1.0.2"
 authors = [{name = "Telicent Ltd", email = "opensource@telicent.io"}]
 description = "A library for working with the IES data standard"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 readme = "README.md"
 dependencies = [
     "geohash-tools==0.2.0",
     "python-geohash==0.8.5",
-    "pyshacl==0.22.2",
+    "pyshacl==0.25.0",
     "requests==2.31.0",
-    "rdflib==6.3.2"
+    "rdflib==6.3.2",
+    "phonenumbers==8.13.35",
+    "pycountry==23.12.11",
+    "validators==0.28.1",
+    "iso4217parse==0.5.1"
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Software Development",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX",
@@ -95,14 +97,22 @@
     "__pypackages__",
     "_build",
     "buck-out",
     "build",
     "dist",
     "node_modules",
     "venv",
+    "ies_tool/*.ttl",
+    "module_to_check/*.shacl"
 ]
 line-length = 120
 
+# Module or directory that contains the files to check
+src = ["ies_tool"]
+
 [tool.mypy]
-no_implicit_optional = false
+python_version = "3.10"
+check_untyped_defs = true
+disallow_untyped_defs = false
 ignore_missing_imports = true
+ignore_errors = true
 modules = ["ies_tool"]
```

