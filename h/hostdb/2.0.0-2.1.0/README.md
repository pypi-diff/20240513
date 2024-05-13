# Comparing `tmp/hostdb-2.0.0.tar.gz` & `tmp/hostdb-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hostdb-2.0.0.tar", last modified: Sat Dec 30 00:21:24 2023, max compression
+gzip compressed data, was "hostdb-2.1.0.tar", last modified: Mon May 13 00:44:55 2024, max compression
```

## Comparing `hostdb-2.0.0.tar` & `hostdb-2.1.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 00:21:24.346475 hostdb-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-12-30 00:21:11.000000 hostdb-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2023-12-30 00:21:24.346475 hostdb-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2023-12-30 00:21:11.000000 hostdb-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 00:21:24.342476 hostdb-2.0.0/hostdb/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-12-30 00:21:11.000000 hostdb-2.0.0/hostdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2023-12-30 00:21:11.000000 hostdb-2.0.0/hostdb/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2023-12-30 00:21:11.000000 hostdb-2.0.0/hostdb/hostdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2023-12-30 00:21:11.000000 hostdb-2.0.0/hostdb/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2023-12-30 00:21:11.000000 hostdb-2.0.0/hostdb/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2023-12-30 00:21:11.000000 hostdb-2.0.0/hostdb/naming.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 00:21:24.342476 hostdb-2.0.0/hostdb/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    14757 2023-12-30 00:21:11.000000 hostdb-2.0.0/hostdb/resources/wordlist
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2023-12-30 00:21:11.000000 hostdb-2.0.0/hostdb/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 00:21:24.342476 hostdb-2.0.0/hostdb/yaml_loaders/
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2023-12-30 00:21:11.000000 hostdb-2.0.0/hostdb/yaml_loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 00:21:24.346475 hostdb-2.0.0/hostdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2023-12-30 00:21:24.000000 hostdb-2.0.0/hostdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      495 2023-12-30 00:21:24.000000 hostdb-2.0.0/hostdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-30 00:21:24.000000 hostdb-2.0.0/hostdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-30 00:21:24.000000 hostdb-2.0.0/hostdb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-30 00:21:24.000000 hostdb-2.0.0/hostdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-30 00:21:24.000000 hostdb-2.0.0/hostdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      850 2023-12-30 00:21:24.346475 hostdb-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-12-30 00:21:11.000000 hostdb-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 00:21:24.346475 hostdb-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2023-12-30 00:21:11.000000 hostdb-2.0.0/tests/test_hostdb.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2023-12-30 00:21:11.000000 hostdb-2.0.0/tests/test_naming.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4166 2023-12-30 00:21:11.000000 hostdb-2.0.0/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:44:55.780712 hostdb-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 00:44:47.000000 hostdb-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-05-13 00:44:55.780712 hostdb-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-13 00:44:47.000000 hostdb-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:44:55.776712 hostdb-2.1.0/hostdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-13 00:44:47.000000 hostdb-2.1.0/hostdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-13 00:44:47.000000 hostdb-2.1.0/hostdb/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-13 00:44:47.000000 hostdb-2.1.0/hostdb/hostdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-13 00:44:47.000000 hostdb-2.1.0/hostdb/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-13 00:44:47.000000 hostdb-2.1.0/hostdb/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-13 00:44:47.000000 hostdb-2.1.0/hostdb/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 00:44:47.000000 hostdb-2.1.0/hostdb/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:44:55.776712 hostdb-2.1.0/hostdb/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    14757 2024-05-13 00:44:47.000000 hostdb-2.1.0/hostdb/resources/wordlist
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-13 00:44:47.000000 hostdb-2.1.0/hostdb/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:44:55.776712 hostdb-2.1.0/hostdb/yaml_loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-13 00:44:47.000000 hostdb-2.1.0/hostdb/yaml_loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:44:55.780712 hostdb-2.1.0/hostdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-05-13 00:44:55.000000 hostdb-2.1.0/hostdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-13 00:44:55.000000 hostdb-2.1.0/hostdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 00:44:55.000000 hostdb-2.1.0/hostdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-13 00:44:55.000000 hostdb-2.1.0/hostdb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-13 00:44:55.000000 hostdb-2.1.0/hostdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 00:44:55.000000 hostdb-2.1.0/hostdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-13 00:44:47.000000 hostdb-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-13 00:44:55.780712 hostdb-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-13 00:44:47.000000 hostdb-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:44:55.776712 hostdb-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-13 00:44:47.000000 hostdb-2.1.0/tests/test_hostdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-13 00:44:47.000000 hostdb-2.1.0/tests/test_naming.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4166 2024-05-13 00:44:47.000000 hostdb-2.1.0/tests/test_validation.py
```

### Comparing `hostdb-2.0.0/LICENSE` & `hostdb-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hostdb-2.0.0/PKG-INFO` & `hostdb-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: hostdb
-Version: 2.0.0
+Version: 2.1.0
 Summary: Hostdb manages homelab hosts using infrastructure as code principles.
 Home-page: https://github.com/allenporter/hostdb
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mashumaro[yaml]>=3.11
 Requires-Dist: ansible>=7.1.0
+Requires-Dist: mashumaro[yaml]>=3.11
 
 # hostdb
 
 This is a library for managing homelab hosts using infrastructure as code
 principles. The primary motivation is to help manage bare metal machines and
 other network infrastructure in an inventory below the kubernetes cluster.
```

### Comparing `hostdb-2.0.0/README.md` & `hostdb-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `hostdb-2.0.0/hostdb/hostdb.py` & `hostdb-2.1.0/hostdb/hostdb.py`

 * *Files identical despite different names*

### Comparing `hostdb-2.0.0/hostdb/inventory.py` & `hostdb-2.1.0/hostdb/inventory.py`

 * *Files identical despite different names*

### Comparing `hostdb-2.0.0/hostdb/manifest.py` & `hostdb-2.1.0/hostdb/manifest.py`

 * *Files identical despite different names*

### Comparing `hostdb-2.0.0/hostdb/naming.py` & `hostdb-2.1.0/hostdb/naming.py`

 * *Files identical despite different names*

### Comparing `hostdb-2.0.0/hostdb/resources/wordlist` & `hostdb-2.1.0/hostdb/resources/wordlist`

 * *Files identical despite different names*

### Comparing `hostdb-2.0.0/hostdb/validation.py` & `hostdb-2.1.0/hostdb/validation.py`

 * *Files identical despite different names*

### Comparing `hostdb-2.0.0/hostdb/yaml_loaders/__init__.py` & `hostdb-2.1.0/hostdb/yaml_loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `hostdb-2.0.0/hostdb.egg-info/PKG-INFO` & `hostdb-2.1.0/hostdb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: hostdb
-Version: 2.0.0
+Version: 2.1.0
 Summary: Hostdb manages homelab hosts using infrastructure as code principles.
 Home-page: https://github.com/allenporter/hostdb
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mashumaro[yaml]>=3.11
 Requires-Dist: ansible>=7.1.0
+Requires-Dist: mashumaro[yaml]>=3.11
 
 # hostdb
 
 This is a library for managing homelab hosts using infrastructure as code
 principles. The primary motivation is to help manage bare metal machines and
 other network infrastructure in an inventory below the kubernetes cluster.
```

### Comparing `hostdb-2.0.0/setup.cfg` & `hostdb-2.1.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 [metadata]
 name = hostdb
-version = 2.0.0
+version = 2.1.0
 description = Hostdb manages homelab hosts using infrastructure as code principles.
 long_description = file: README.md
 long_description_content_type = text/markdown
-prodid = github.com/allenporter/hostdb
 url = https://github.com/allenporter/hostdb
 author = Allen Porter
 author_email = allen.porter@gmail.com
 license = Apache-2.0
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	License :: OSI Approved :: Apache Software License
+	Programming Language :: Python :: 3
+	Programming Language :: Python :: 3 :: Only
+prodid = github.com/allenporter/hostdb
 
 [options]
 packages = find:
-python_requires = >=3.10
 install_requires = 
-	mashumaro[yaml]>=3.11
 	ansible>=7.1.0
+	mashumaro[yaml]>=3.11
+python_requires = >=3.10
 include_package_data = True
 package_dir = 
 	= .
 
-[options.entry_points]
-console_scripts = 
-	hostdb = hostdb.tool.main:main
-
 [options.packages.find]
 where = .
 exclude = 
 	tests
 	tests.*
 
+[options.entry_points]
+console_scripts = 
+	hostdb = hostdb.tool.main:main
+
 [options.package_data]
 hostdb = 
+	py.typed
 	resources/wordlist
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `hostdb-2.0.0/tests/test_hostdb.py` & `hostdb-2.1.0/tests/test_hostdb.py`

 * *Files identical despite different names*

### Comparing `hostdb-2.0.0/tests/test_naming.py` & `hostdb-2.1.0/tests/test_naming.py`

 * *Files identical despite different names*

### Comparing `hostdb-2.0.0/tests/test_validation.py` & `hostdb-2.1.0/tests/test_validation.py`

 * *Files identical despite different names*

