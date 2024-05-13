# Comparing `tmp/diskcache_stubs-5.6.3.3.20240316.tar.gz` & `tmp/diskcache_stubs-5.6.3.3.20240401.tar.gz`

## Comparing `diskcache_stubs-5.6.3.3.20240316.tar` & `diskcache_stubs-5.6.3.3.20240401.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240316/ruff.toml
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240316/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240316/src/diskcache/__init__.pyi
--rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240316/src/diskcache/_typeshed.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240316/src/diskcache/cli.pyi
--rw-r--r--   0        0        0    16268 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240316/src/diskcache/core.pyi
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240316/src/diskcache/djangocache.pyi
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240316/src/diskcache/fanout.pyi
--rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240316/src/diskcache/persistent.pyi
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240316/src/diskcache/recipes.pyi
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240316/.gitignore
--rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240316/LICENSE
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240316/README.md
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240316/pyproject.toml
--rw-r--r--   0        0        0    14233 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240316/PKG-INFO
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240401/asd.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240401/ruff.toml
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240401/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240401/src/diskcache-stubs/__init__.pyi
+-rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240401/src/diskcache-stubs/_typeshed.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240401/src/diskcache-stubs/cli.pyi
+-rw-r--r--   0        0        0    16268 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240401/src/diskcache-stubs/core.pyi
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240401/src/diskcache-stubs/djangocache.pyi
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240401/src/diskcache-stubs/fanout.pyi
+-rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240401/src/diskcache-stubs/persistent.pyi
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240401/src/diskcache-stubs/recipes.pyi
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240401/.gitignore
+-rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240401/LICENSE
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240401/README.md
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240401/pyproject.toml
+-rw-r--r--   0        0        0    14472 2020-02-02 00:00:00.000000 diskcache_stubs-5.6.3.3.20240401/PKG-INFO
```

### Comparing `diskcache_stubs-5.6.3.3.20240316/ruff.toml` & `diskcache_stubs-5.6.3.3.20240401/ruff.toml`

 * *Files identical despite different names*

### Comparing `diskcache_stubs-5.6.3.3.20240316/.github/workflows/publish.yaml` & `diskcache_stubs-5.6.3.3.20240401/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `diskcache_stubs-5.6.3.3.20240316/src/diskcache/__init__.pyi` & `diskcache_stubs-5.6.3.3.20240401/src/diskcache-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `diskcache_stubs-5.6.3.3.20240316/src/diskcache/_typeshed.pyi` & `diskcache_stubs-5.6.3.3.20240401/src/diskcache-stubs/_typeshed.pyi`

 * *Files identical despite different names*

### Comparing `diskcache_stubs-5.6.3.3.20240316/src/diskcache/core.pyi` & `diskcache_stubs-5.6.3.3.20240401/src/diskcache-stubs/core.pyi`

 * *Files identical despite different names*

### Comparing `diskcache_stubs-5.6.3.3.20240316/src/diskcache/djangocache.pyi` & `diskcache_stubs-5.6.3.3.20240401/src/diskcache-stubs/djangocache.pyi`

 * *Files identical despite different names*

### Comparing `diskcache_stubs-5.6.3.3.20240316/src/diskcache/fanout.pyi` & `diskcache_stubs-5.6.3.3.20240401/src/diskcache-stubs/fanout.pyi`

 * *Files identical despite different names*

### Comparing `diskcache_stubs-5.6.3.3.20240316/src/diskcache/persistent.pyi` & `diskcache_stubs-5.6.3.3.20240401/src/diskcache-stubs/persistent.pyi`

 * *Files identical despite different names*

### Comparing `diskcache_stubs-5.6.3.3.20240316/src/diskcache/recipes.pyi` & `diskcache_stubs-5.6.3.3.20240401/src/diskcache-stubs/recipes.pyi`

 * *Files identical despite different names*

### Comparing `diskcache_stubs-5.6.3.3.20240316/.gitignore` & `diskcache_stubs-5.6.3.3.20240401/.gitignore`

 * *Files identical despite different names*

### Comparing `diskcache_stubs-5.6.3.3.20240316/LICENSE` & `diskcache_stubs-5.6.3.3.20240401/LICENSE`

 * *Files identical despite different names*

### Comparing `diskcache_stubs-5.6.3.3.20240316/README.md` & `diskcache_stubs-5.6.3.3.20240401/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # diskcache-stubs
 
 [![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-yellow.svg)](https://opensource.org/licenses/Apache-2.0)
 [![PyPI version](https://badge.fury.io/py/diskcache-stubs.svg)](https://badge.fury.io/py/diskcache-stubs)
 [![python version](https://img.shields.io/pypi/pyversions/diskcache-stubs.svg)](#)
 
+Warning: This library provides type hints only.
+If you need the runtime package,
+you can find it [`python-diskcache`](https://github.com/grantjenks/python-diskcache).
+
 ## how to install
 ```shell
 $ pip install diskcache-stubs
 ```
 
 ## TODO
 * [ ] `diskcache.core.Cache`
```

### Comparing `diskcache_stubs-5.6.3.3.20240316/pyproject.toml` & `diskcache_stubs-5.6.3.3.20240401/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 [project]
 name = "diskcache-stubs"
-version = "5.6.3.3.20240316"
+version = "5.6.3.3.20240401"
 description = "diskcache stubs"
 authors = [{ name = "phi", email = "phi.friday@gmail.com" }]
 dependencies = []
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">= 3"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: Implementation :: CPython",
     "Typing :: Stubs Only",
 ]
 
+[project.urls]
+Repository = "https://github.com/phi-friday/diskcache-stubs"
+
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
 dev-dependencies = ["diskcache>=5.6.3"]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/diskcache"]
+packages = ["src/diskcache-stubs"]
 
 [tool.pyright]
 pythonVersion = '3.8'
 pythonPlatform = 'Linux'
 diagnostic = 'basic'
-stubPath = "./src"
+stubPath = "./typings"
```

### Comparing `diskcache_stubs-5.6.3.3.20240316/PKG-INFO` & `diskcache_stubs-5.6.3.3.20240401/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.3
 Name: diskcache-stubs
-Version: 5.6.3.3.20240316
+Version: 5.6.3.3.20240401
 Summary: diskcache stubs
+Project-URL: Repository, https://github.com/phi-friday/diskcache-stubs
 Author-email: phi <phi.friday@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -215,14 +216,18 @@
 
 # diskcache-stubs
 
 [![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-yellow.svg)](https://opensource.org/licenses/Apache-2.0)
 [![PyPI version](https://badge.fury.io/py/diskcache-stubs.svg)](https://badge.fury.io/py/diskcache-stubs)
 [![python version](https://img.shields.io/pypi/pyversions/diskcache-stubs.svg)](#)
 
+Warning: This library provides type hints only.
+If you need the runtime package,
+you can find it [`python-diskcache`](https://github.com/grantjenks/python-diskcache).
+
 ## how to install
 ```shell
 $ pip install diskcache-stubs
 ```
 
 ## TODO
 * [ ] `diskcache.core.Cache`
```

