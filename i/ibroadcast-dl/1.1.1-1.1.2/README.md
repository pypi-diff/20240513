# Comparing `tmp/ibroadcast_dl-1.1.1.tar.gz` & `tmp/ibroadcast_dl-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibroadcast_dl-1.1.1.tar", max compression
+gzip compressed data, was "ibroadcast_dl-1.1.2.tar", max compression
```

## Comparing `ibroadcast_dl-1.1.1.tar` & `ibroadcast_dl-1.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1653 2024-03-06 12:46:33.194399 ibroadcast_dl-1.1.1/README.md
--rw-r--r--   0        0        0       77 2024-03-06 12:46:33.194399 ibroadcast_dl-1.1.1/ibroadcastdl/__init__.py
--rw-r--r--   0        0        0       98 2024-03-06 12:46:33.194399 ibroadcast_dl-1.1.1/ibroadcastdl/__main__.py
--rw-r--r--   0        0        0     2670 2024-03-06 12:46:33.194399 ibroadcast_dl-1.1.1/ibroadcastdl/cli.py
--rw-r--r--   0        0        0     1760 2024-03-06 12:46:33.194399 ibroadcast_dl-1.1.1/ibroadcastdl/dl.py
--rw-r--r--   0        0        0      181 2024-03-06 12:46:33.194399 ibroadcast_dl-1.1.1/ibroadcastdl/exceptions.py
--rw-r--r--   0        0        0      754 2024-03-06 12:46:33.194399 ibroadcast_dl-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     2293 1970-01-01 00:00:00.000000 ibroadcast_dl-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1653 2024-05-13 13:36:55.732790 ibroadcast_dl-1.1.2/README.md
+-rw-r--r--   0        0        0       77 2024-05-13 13:36:55.732790 ibroadcast_dl-1.1.2/ibroadcastdl/__init__.py
+-rw-r--r--   0        0        0       98 2024-05-13 13:36:55.732790 ibroadcast_dl-1.1.2/ibroadcastdl/__main__.py
+-rw-r--r--   0        0        0     2670 2024-05-13 13:36:55.732790 ibroadcast_dl-1.1.2/ibroadcastdl/cli.py
+-rw-r--r--   0        0        0     1760 2024-05-13 13:36:55.732790 ibroadcast_dl-1.1.2/ibroadcastdl/dl.py
+-rw-r--r--   0        0        0      181 2024-05-13 13:36:55.732790 ibroadcast_dl-1.1.2/ibroadcastdl/exceptions.py
+-rw-r--r--   0        0        0      763 2024-05-13 13:36:55.732790 ibroadcast_dl-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2289 1970-01-01 00:00:00.000000 ibroadcast_dl-1.1.2/PKG-INFO
```

### Comparing `ibroadcast_dl-1.1.1/README.md` & `ibroadcast_dl-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ibroadcast_dl-1.1.1/ibroadcastdl/cli.py` & `ibroadcast_dl-1.1.2/ibroadcastdl/cli.py`

 * *Files identical despite different names*

### Comparing `ibroadcast_dl-1.1.1/ibroadcastdl/dl.py` & `ibroadcast_dl-1.1.2/ibroadcastdl/dl.py`

 * *Files identical despite different names*

### Comparing `ibroadcast_dl-1.1.1/pyproject.toml` & `ibroadcast_dl-1.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ibroadcast-dl"
-version = "1.1.1"
+version = "1.1.2"
 description = "Download / Sync library from iBroadcast on Linux machines"
 authors = ["Marco Ceppi <marco@ceppi.net>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
     { include = "ibroadcastdl" },
 ]
@@ -12,24 +12,24 @@
 [tool.poetry.scripts]
 ibroadcast-dl = 'ibroadcastdl.cli:app'
 
 [tool.poetry.dependencies]
 python = "^3.11"
 ibroadcast = "^1.1.2"
 pydantic = "^2.6.1"
-typer = "^0.9.0"
+typer = ">=0.9,<0.13"
 rich = "^13.7.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.2.0"
 isort = "^5.13.2"
 pytest = "^8.0.1"
 pylint = "^3.0.3"
-ruff = ">=0.2.2,<0.4.0"
-pytest-cov = "^4.1.0"
+ruff = ">=0.2.2,<0.5.0"
+pytest-cov = ">=4.1,<6.0"
 
 [tool.coverage.run]
 omit = [
     "ibroadcastdl/__main__.py",
 ]
 
 [build-system]
```

### Comparing `ibroadcast_dl-1.1.1/PKG-INFO` & `ibroadcast_dl-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ibroadcast-dl
-Version: 1.1.1
+Version: 1.1.2
 Summary: Download / Sync library from iBroadcast on Linux machines
 License: Apache-2.0
 Author: Marco Ceppi
 Author-email: marco@ceppi.net
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ibroadcast (>=1.1.2,<2.0.0)
 Requires-Dist: pydantic (>=2.6.1,<3.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
-Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: typer (>=0.9,<0.13)
 Description-Content-Type: text/markdown
 
 # iBroadcast Download / Sync
 
 This project was born from a need to download my library from iBroadcast onto my linux machine. Only the OSX and Windows app support this functionality. This project uses the existing [ibroadcast-python](https://pypi.org/project/ibroadcast/) library and extends the `iBroadcast` class to add a `download_library` method.
 
 In addition to using this as a Python library, it also has a small CLI to help automate doing library downloads.
```

