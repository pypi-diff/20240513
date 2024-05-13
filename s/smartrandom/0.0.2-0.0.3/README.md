# Comparing `tmp/smartrandom-0.0.2.tar.gz` & `tmp/smartrandom-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartrandom-0.0.2.tar", last modified: Wed May  8 04:03:00 2024, max compression
+gzip compressed data, was "smartrandom-0.0.3.tar", last modified: Mon May 13 00:45:27 2024, max compression
```

## Comparing `smartrandom-0.0.2.tar` & `smartrandom-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-08 04:03:00.619456 smartrandom-0.0.2/
--rw-r--r--   0 smart     (1000) smart     (1000)     1498 2024-05-08 03:52:29.000000 smartrandom-0.0.2/LICENSE
--rw-r--r--   0 smart     (1000) smart     (1000)     2838 2024-05-08 04:03:00.619456 smartrandom-0.0.2/PKG-INFO
--rw-r--r--   0 smart     (1000) smart     (1000)     1913 2024-05-08 03:58:36.000000 smartrandom-0.0.2/README.md
--rw-r--r--   0 smart     (1000) smart     (1000)     1084 2024-05-08 04:03:00.619456 smartrandom-0.0.2/setup.cfg
--rw-r--r--   0 smart     (1000) smart     (1000)       84 2024-05-08 03:52:29.000000 smartrandom-0.0.2/setup.py
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-08 04:03:00.612789 smartrandom-0.0.2/smartrandom/
--rw-r--r--   0 smart     (1000) smart     (1000)      377 2024-05-08 03:57:25.000000 smartrandom-0.0.2/smartrandom/__init__.py
--rw-r--r--   0 smart     (1000) smart     (1000)     1987 2024-05-08 03:57:25.000000 smartrandom-0.0.2/smartrandom/random_master.py
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-08 04:03:00.616123 smartrandom-0.0.2/smartrandom.egg-info/
--rw-r--r--   0 smart     (1000) smart     (1000)     2838 2024-05-08 04:03:00.000000 smartrandom-0.0.2/smartrandom.egg-info/PKG-INFO
--rw-r--r--   0 smart     (1000) smart     (1000)      263 2024-05-08 04:03:00.000000 smartrandom-0.0.2/smartrandom.egg-info/SOURCES.txt
--rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-08 04:03:00.000000 smartrandom-0.0.2/smartrandom.egg-info/dependency_links.txt
--rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-08 03:52:39.000000 smartrandom-0.0.2/smartrandom.egg-info/not-zip-safe
--rw-r--r--   0 smart     (1000) smart     (1000)       12 2024-05-08 04:03:00.000000 smartrandom-0.0.2/smartrandom.egg-info/top_level.txt
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-13 00:45:27.214796 smartrandom-0.0.3/
+-rw-r--r--   0 smart     (1000) smart     (1000)     1498 2024-05-08 03:52:29.000000 smartrandom-0.0.3/LICENSE
+-rw-r--r--   0 smart     (1000) smart     (1000)     3557 2024-05-13 00:45:27.214796 smartrandom-0.0.3/PKG-INFO
+-rw-r--r--   0 smart     (1000) smart     (1000)     2632 2024-05-13 00:43:28.000000 smartrandom-0.0.3/README.md
+-rw-r--r--   0 smart     (1000) smart     (1000)     1108 2024-05-13 00:45:27.218129 smartrandom-0.0.3/setup.cfg
+-rw-r--r--   0 smart     (1000) smart     (1000)       84 2024-05-08 03:52:29.000000 smartrandom-0.0.3/setup.py
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-13 00:45:27.214796 smartrandom-0.0.3/smartrandom/
+-rw-r--r--   0 smart     (1000) smart     (1000)      399 2024-05-13 00:44:17.000000 smartrandom-0.0.3/smartrandom/__init__.py
+-rw-r--r--   0 smart     (1000) smart     (1000)     1987 2024-05-08 03:57:25.000000 smartrandom-0.0.3/smartrandom/random_master.py
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-13 00:45:27.214796 smartrandom-0.0.3/smartrandom.egg-info/
+-rw-r--r--   0 smart     (1000) smart     (1000)     3557 2024-05-13 00:45:27.000000 smartrandom-0.0.3/smartrandom.egg-info/PKG-INFO
+-rw-r--r--   0 smart     (1000) smart     (1000)      263 2024-05-13 00:45:27.000000 smartrandom-0.0.3/smartrandom.egg-info/SOURCES.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-13 00:45:27.000000 smartrandom-0.0.3/smartrandom.egg-info/dependency_links.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-13 00:45:27.000000 smartrandom-0.0.3/smartrandom.egg-info/not-zip-safe
+-rw-r--r--   0 smart     (1000) smart     (1000)       12 2024-05-13 00:45:27.000000 smartrandom-0.0.3/smartrandom.egg-info/top_level.txt
```

### Comparing `smartrandom-0.0.2/LICENSE` & `smartrandom-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `smartrandom-0.0.2/PKG-INFO` & `smartrandom-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartrandom
-Version: 0.0.2
+Version: 0.0.3
 Summary: Random Data Generators
 Home-page: https://github.com/smartlegionlab/smartrandom/
 Author: A.A Suvorov
 Author-email: smartlegiondev@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://github.com/smartlegionlab/smartrandom/blob/master/README.md
 Project-URL: Release notes, https://github.com/smartlegionlab/smartrandom/releases
@@ -16,23 +16,31 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# smartrandom <sup>v0.0.2</sup>
+# smartrandom <sup>v0.0.3</sup>
 ---
 
 ## Random Data Generators:
 
 Allows you to generate random strings of a given length from letters, numbers, symbols.
 Helps to generate passwords, service codes (for example, for sending via SMS), hashes and much more.
 ---
 
+[![GitHub release (latest by date)](https://img.shields.io/github/v/release/smartlegionlab/smartrandom)](https://github.com/smartlegionlab/smartrandom/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/smartrandom?label=pypi%20downloads)](https://pypi.org/project/smartrandom/)
+![GitHub top language](https://img.shields.io/github/languages/top/smartlegionlab/smartrandom)
+[![PyPI](https://img.shields.io/pypi/v/smartrandom)](https://pypi.org/project/smartrandom)
+[![GitHub](https://img.shields.io/github/license/smartlegionlab/smartrandom)](https://github.com/smartlegionlab/smartrandom/blob/master/LICENSE)
+[![PyPI - Format](https://img.shields.io/pypi/format/smartrandom)](https://pypi.org/project/smartrandom)
+
+
 ## Help:
 
 ```python
 from smartrandom.random_master import RandomMaster
 
 random_string = RandomMaster.string.create(length=10)
 random_number_string = RandomMaster.number.create(length=10)
```

### Comparing `smartrandom-0.0.2/setup.cfg` & `smartrandom-0.0.3/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = smartrandom
-version = 0.0.2
+version = attr: smartrandom.__version__
 author = A.A Suvorov
 author_email = smartlegiondev@gmail.com
 description = Random Data Generators
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/smartlegionlab/smartrandom/
 project_urls =
```

### Comparing `smartrandom-0.0.2/smartrandom/random_master.py` & `smartrandom-0.0.3/smartrandom/random_master.py`

 * *Files identical despite different names*

### Comparing `smartrandom-0.0.2/smartrandom.egg-info/PKG-INFO` & `smartrandom-0.0.3/smartrandom.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartrandom
-Version: 0.0.2
+Version: 0.0.3
 Summary: Random Data Generators
 Home-page: https://github.com/smartlegionlab/smartrandom/
 Author: A.A Suvorov
 Author-email: smartlegiondev@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://github.com/smartlegionlab/smartrandom/blob/master/README.md
 Project-URL: Release notes, https://github.com/smartlegionlab/smartrandom/releases
@@ -16,23 +16,31 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# smartrandom <sup>v0.0.2</sup>
+# smartrandom <sup>v0.0.3</sup>
 ---
 
 ## Random Data Generators:
 
 Allows you to generate random strings of a given length from letters, numbers, symbols.
 Helps to generate passwords, service codes (for example, for sending via SMS), hashes and much more.
 ---
 
+[![GitHub release (latest by date)](https://img.shields.io/github/v/release/smartlegionlab/smartrandom)](https://github.com/smartlegionlab/smartrandom/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/smartrandom?label=pypi%20downloads)](https://pypi.org/project/smartrandom/)
+![GitHub top language](https://img.shields.io/github/languages/top/smartlegionlab/smartrandom)
+[![PyPI](https://img.shields.io/pypi/v/smartrandom)](https://pypi.org/project/smartrandom)
+[![GitHub](https://img.shields.io/github/license/smartlegionlab/smartrandom)](https://github.com/smartlegionlab/smartrandom/blob/master/LICENSE)
+[![PyPI - Format](https://img.shields.io/pypi/format/smartrandom)](https://pypi.org/project/smartrandom)
+
+
 ## Help:
 
 ```python
 from smartrandom.random_master import RandomMaster
 
 random_string = RandomMaster.string.create(length=10)
 random_number_string = RandomMaster.number.create(length=10)
```

