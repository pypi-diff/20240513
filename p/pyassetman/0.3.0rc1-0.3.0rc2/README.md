# Comparing `tmp/pyassetman-0.3.0rc1.tar.gz` & `tmp/pyassetman-0.3.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyassetman-0.3.0rc1.tar", last modified: Fri Feb 16 17:14:58 2024, max compression
+gzip compressed data, was "pyassetman-0.3.0rc2.tar", last modified: Mon May 13 18:58:31 2024, max compression
```

## Comparing `pyassetman-0.3.0rc1.tar` & `pyassetman-0.3.0rc2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 josh       (504) staff       (20)        0 2024-02-16 17:14:58.096577 pyassetman-0.3.0rc1/
--rw-r--r--   0 josh       (504) staff       (20)    11358 2024-01-09 01:17:06.000000 pyassetman-0.3.0rc1/LICENSE
--rw-r--r--   0 josh       (504) staff       (20)     5547 2024-02-16 17:14:58.096408 pyassetman-0.3.0rc1/PKG-INFO
--rw-r--r--   0 josh       (504) staff       (20)     5024 2024-01-09 01:17:06.000000 pyassetman-0.3.0rc1/README.md
-drwxr-xr-x   0 josh       (504) staff       (20)        0 2024-02-16 17:14:58.094492 pyassetman-0.3.0rc1/assetman/
--rwxr-xr-x   0 josh       (504) staff       (20)     9085 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc1/assetman/S3UploadThread.py
--rw-r--r--   0 josh       (504) staff       (20)      113 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc1/assetman/__init__.py
--rwxr-xr-x   0 josh       (504) staff       (20)    18782 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc1/assetman/compile.py
--rw-r--r--   0 josh       (504) staff       (20)    10536 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc1/assetman/compilers.py
--rw-r--r--   0 josh       (504) staff       (20)     7083 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc1/assetman/managers.py
--rw-r--r--   0 josh       (504) staff       (20)     4107 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc1/assetman/manifest.py
-drwxr-xr-x   0 josh       (504) staff       (20)        0 2024-02-16 17:14:58.094871 pyassetman-0.3.0rc1/assetman/parsers/
--rw-r--r--   0 josh       (504) staff       (20)        0 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc1/assetman/parsers/__init__.py
--rw-r--r--   0 josh       (504) staff       (20)     1103 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc1/assetman/parsers/base.py
--rw-r--r--   0 josh       (504) staff       (20)     2339 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc1/assetman/parsers/tornado_parser.py
--rw-r--r--   0 josh       (504) staff       (20)     2467 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc1/assetman/settings.py
--rw-r--r--   0 josh       (504) staff       (20)     2774 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc1/assetman/tools.py
-drwxr-xr-x   0 josh       (504) staff       (20)        0 2024-02-16 17:14:58.095497 pyassetman-0.3.0rc1/assetman/tornadoutils/
--rw-r--r--   0 josh       (504) staff       (20)      336 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc1/assetman/tornadoutils/RequestHandler.py
--rw-r--r--   0 josh       (504) staff       (20)      142 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc1/assetman/tornadoutils/__init__.py
--rw-r--r--   0 josh       (504) staff       (20)      651 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc1/assetman/tornadoutils/helpers.py
--rw-r--r--   0 josh       (504) staff       (20)     7154 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc1/assetman/tornadoutils/static.py
-drwxr-xr-x   0 josh       (504) staff       (20)        0 2024-02-16 17:14:58.096236 pyassetman-0.3.0rc1/pyassetman.egg-info/
--rw-r--r--   0 josh       (504) staff       (20)     5547 2024-02-16 17:14:58.000000 pyassetman-0.3.0rc1/pyassetman.egg-info/PKG-INFO
--rw-r--r--   0 josh       (504) staff       (20)      600 2024-02-16 17:14:58.000000 pyassetman-0.3.0rc1/pyassetman.egg-info/SOURCES.txt
--rw-r--r--   0 josh       (504) staff       (20)        1 2024-02-16 17:14:58.000000 pyassetman-0.3.0rc1/pyassetman.egg-info/dependency_links.txt
--rw-r--r--   0 josh       (504) staff       (20)       29 2024-02-16 17:14:58.000000 pyassetman-0.3.0rc1/pyassetman.egg-info/requires.txt
--rw-r--r--   0 josh       (504) staff       (20)        9 2024-02-16 17:14:58.000000 pyassetman-0.3.0rc1/pyassetman.egg-info/top_level.txt
--rw-r--r--   0 josh       (504) staff       (20)      723 2024-02-16 02:12:27.000000 pyassetman-0.3.0rc1/pyproject.toml
--rw-r--r--   0 josh       (504) staff       (20)       38 2024-02-16 17:14:58.096605 pyassetman-0.3.0rc1/setup.cfg
+drwxr-xr-x   0 josh       (504) staff       (20)        0 2024-05-13 18:58:31.567683 pyassetman-0.3.0rc2/
+-rw-r--r--   0 josh       (504) staff       (20)    11358 2024-01-09 01:17:06.000000 pyassetman-0.3.0rc2/LICENSE
+-rw-r--r--   0 josh       (504) staff       (20)     5577 2024-05-13 18:58:31.567494 pyassetman-0.3.0rc2/PKG-INFO
+-rw-r--r--   0 josh       (504) staff       (20)     5024 2024-01-09 01:17:06.000000 pyassetman-0.3.0rc2/README.md
+drwxr-xr-x   0 josh       (504) staff       (20)        0 2024-05-13 18:58:31.565343 pyassetman-0.3.0rc2/assetman/
+-rwxr-xr-x   0 josh       (504) staff       (20)     9085 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/S3UploadThread.py
+-rw-r--r--   0 josh       (504) staff       (20)      113 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/__init__.py
+-rwxr-xr-x   0 josh       (504) staff       (20)    18782 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/compile.py
+-rw-r--r--   0 josh       (504) staff       (20)    10542 2024-05-13 18:48:44.000000 pyassetman-0.3.0rc2/assetman/compilers.py
+-rw-r--r--   0 josh       (504) staff       (20)     7083 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/managers.py
+-rw-r--r--   0 josh       (504) staff       (20)     4107 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/manifest.py
+drwxr-xr-x   0 josh       (504) staff       (20)        0 2024-05-13 18:58:31.565786 pyassetman-0.3.0rc2/assetman/parsers/
+-rw-r--r--   0 josh       (504) staff       (20)        0 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/parsers/__init__.py
+-rw-r--r--   0 josh       (504) staff       (20)     1103 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/parsers/base.py
+-rw-r--r--   0 josh       (504) staff       (20)     2339 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/parsers/tornado_parser.py
+-rw-r--r--   0 josh       (504) staff       (20)     2467 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/settings.py
+-rw-r--r--   0 josh       (504) staff       (20)     2774 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/tools.py
+drwxr-xr-x   0 josh       (504) staff       (20)        0 2024-05-13 18:58:31.566546 pyassetman-0.3.0rc2/assetman/tornadoutils/
+-rw-r--r--   0 josh       (504) staff       (20)      336 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/tornadoutils/RequestHandler.py
+-rw-r--r--   0 josh       (504) staff       (20)      142 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/tornadoutils/__init__.py
+-rw-r--r--   0 josh       (504) staff       (20)      651 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/tornadoutils/helpers.py
+-rw-r--r--   0 josh       (504) staff       (20)     7154 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/tornadoutils/static.py
+drwxr-xr-x   0 josh       (504) staff       (20)        0 2024-05-13 18:58:31.567288 pyassetman-0.3.0rc2/pyassetman.egg-info/
+-rw-r--r--   0 josh       (504) staff       (20)     5577 2024-05-13 18:58:31.000000 pyassetman-0.3.0rc2/pyassetman.egg-info/PKG-INFO
+-rw-r--r--   0 josh       (504) staff       (20)      600 2024-05-13 18:58:31.000000 pyassetman-0.3.0rc2/pyassetman.egg-info/SOURCES.txt
+-rw-r--r--   0 josh       (504) staff       (20)        1 2024-05-13 18:58:31.000000 pyassetman-0.3.0rc2/pyassetman.egg-info/dependency_links.txt
+-rw-r--r--   0 josh       (504) staff       (20)       29 2024-05-13 18:58:31.000000 pyassetman-0.3.0rc2/pyassetman.egg-info/requires.txt
+-rw-r--r--   0 josh       (504) staff       (20)        9 2024-05-13 18:58:31.000000 pyassetman-0.3.0rc2/pyassetman.egg-info/top_level.txt
+-rw-r--r--   0 josh       (504) staff       (20)      772 2024-05-13 18:48:44.000000 pyassetman-0.3.0rc2/pyproject.toml
+-rw-r--r--   0 josh       (504) staff       (20)       38 2024-05-13 18:58:31.567719 pyassetman-0.3.0rc2/setup.cfg
```

### Comparing `pyassetman-0.3.0rc1/LICENSE` & `pyassetman-0.3.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyassetman-0.3.0rc1/PKG-INFO` & `pyassetman-0.3.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyassetman
-Version: 0.3.0rc1
+Version: 0.3.0rc2
 Summary: assetman assetmanager
 Author-email: Will McCutchen <wm@bit.ly>
-Maintainer-email: Jehiah Czebotar <jehiah@gmail.com>, Josh Harshman <josh.harshman@bit.ly>
+Maintainer-email: Jehiah Czebotar <jehiah@gmail.com>, Josh Harshman <josh.harshman@bit.ly>, Oscar Luu <oscar.luu@bit.ly>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3>=1.10.0
```

### Comparing `pyassetman-0.3.0rc1/README.md` & `pyassetman-0.3.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `pyassetman-0.3.0rc1/assetman/S3UploadThread.py` & `pyassetman-0.3.0rc2/assetman/S3UploadThread.py`

 * *Files identical despite different names*

### Comparing `pyassetman-0.3.0rc1/assetman/compile.py` & `pyassetman-0.3.0rc2/assetman/compile.py`

 * *Files identical despite different names*

### Comparing `pyassetman-0.3.0rc1/assetman/compilers.py` & `pyassetman-0.3.0rc2/assetman/compilers.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,15 @@
             before, url_prefix, rel_path, after = match.groups()
             path = make_absolute_static_path(self.settings['static_dir'], rel_path)
             assert os.path.isfile(path), (path, str(self))
             if os.stat(path).st_size > MAX_FILE_SIZE:
                 logging.debug('Not inlining %s (%.2fKB)', path, os.stat(path).st_size / KB)
                 return match.group(0)
             else:
-                encoded = base64.b64encode(open(path).read())
+                encoded = base64.b64encode(open(path, 'rb').read())
                 mime_type, _ = mimetypes.guess_type(path)
                 if not mime_type and path.endswith('.otf'):
                     mime_type = 'application/octet-stream'
                 if not mime_type and path.endswith('.ttf'):
                     mime_type = 'font/ttf'
                 if not mime_type and path.endswith('.eot'):
                     mime_type = 'application/vnd.ms-fontobject'
```

### Comparing `pyassetman-0.3.0rc1/assetman/managers.py` & `pyassetman-0.3.0rc2/assetman/managers.py`

 * *Files identical despite different names*

### Comparing `pyassetman-0.3.0rc1/assetman/manifest.py` & `pyassetman-0.3.0rc2/assetman/manifest.py`

 * *Files identical despite different names*

### Comparing `pyassetman-0.3.0rc1/assetman/parsers/base.py` & `pyassetman-0.3.0rc2/assetman/parsers/base.py`

 * *Files identical despite different names*

### Comparing `pyassetman-0.3.0rc1/assetman/parsers/tornado_parser.py` & `pyassetman-0.3.0rc2/assetman/parsers/tornado_parser.py`

 * *Files identical despite different names*

### Comparing `pyassetman-0.3.0rc1/assetman/settings.py` & `pyassetman-0.3.0rc2/assetman/settings.py`

 * *Files identical despite different names*

### Comparing `pyassetman-0.3.0rc1/assetman/tools.py` & `pyassetman-0.3.0rc2/assetman/tools.py`

 * *Files identical despite different names*

### Comparing `pyassetman-0.3.0rc1/assetman/tornadoutils/helpers.py` & `pyassetman-0.3.0rc2/assetman/tornadoutils/helpers.py`

 * *Files identical despite different names*

### Comparing `pyassetman-0.3.0rc1/assetman/tornadoutils/static.py` & `pyassetman-0.3.0rc2/assetman/tornadoutils/static.py`

 * *Files identical despite different names*

### Comparing `pyassetman-0.3.0rc1/pyassetman.egg-info/PKG-INFO` & `pyassetman-0.3.0rc2/pyassetman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyassetman
-Version: 0.3.0rc1
+Version: 0.3.0rc2
 Summary: assetman assetmanager
 Author-email: Will McCutchen <wm@bit.ly>
-Maintainer-email: Jehiah Czebotar <jehiah@gmail.com>, Josh Harshman <josh.harshman@bit.ly>
+Maintainer-email: Jehiah Czebotar <jehiah@gmail.com>, Josh Harshman <josh.harshman@bit.ly>, Oscar Luu <oscar.luu@bit.ly>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3>=1.10.0
```

### Comparing `pyassetman-0.3.0rc1/pyassetman.egg-info/SOURCES.txt` & `pyassetman-0.3.0rc2/pyassetman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyassetman-0.3.0rc1/pyproject.toml` & `pyassetman-0.3.0rc2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyassetman"
 description = "assetman assetmanager"
-version = "0.3.0rc1"
+version = "0.3.0rc2"
 authors = [
   { name="Will McCutchen", email="wm@bit.ly" },
 ]
 maintainers = [
   { name="Jehiah Czebotar", email="jehiah@gmail.com"},
-  { name="Josh Harshman", email="josh.harshman@bit.ly"}
+  { name="Josh Harshman", email="josh.harshman@bit.ly"},
+  { name="Oscar Luu", email="oscar.luu@bit.ly"}
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
```

