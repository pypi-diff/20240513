# Comparing `tmp/codescout-0.1.6.tar.gz` & `tmp/codescout-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codescout-0.1.6.tar", last modified: Mon May 13 17:36:11 2024, max compression
+gzip compressed data, was "codescout-0.1.7.tar", last modified: Mon May 13 17:39:03 2024, max compression
```

## Comparing `codescout-0.1.6.tar` & `codescout-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 17:36:11.190289 codescout-0.1.6/
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)    11357 2024-05-13 14:57:56.000000 codescout-0.1.6/LICENSE
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)       23 2024-05-13 17:02:21.000000 codescout-0.1.6/MANIFEST.in
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)    17271 2024-05-13 17:36:11.189872 codescout-0.1.6/PKG-INFO
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)     3751 2024-05-13 14:57:56.000000 codescout-0.1.6/README.md
-drwxr-xr-x   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 17:36:11.187634 codescout-0.1.6/codescout/
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)       32 2024-05-13 17:08:05.000000 codescout-0.1.6/codescout/__init__.py
--rwxr-xr-x   0 vfo001   (67203) eccc_rpnenv (66080)    20947 2024-05-13 15:13:31.000000 codescout-0.1.6/codescout/codescout.py
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)      700 2024-05-13 17:30:21.000000 codescout-0.1.6/pyproject.toml
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)       38 2024-05-13 17:36:11.190338 codescout-0.1.6/setup.cfg
-drwxr-xr-x   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 17:36:11.185470 codescout-0.1.6/src/
-drwxr-xr-x   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 17:36:11.189425 codescout-0.1.6/src/codescout.egg-info/
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)    17271 2024-05-13 17:36:11.188289 codescout-0.1.6/src/codescout.egg-info/PKG-INFO
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)      273 2024-05-13 17:36:11.188509 codescout-0.1.6/src/codescout.egg-info/SOURCES.txt
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)        1 2024-05-13 17:36:11.188902 codescout-0.1.6/src/codescout.egg-info/dependency_links.txt
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)       14 2024-05-13 17:36:11.189246 codescout-0.1.6/src/codescout.egg-info/requires.txt
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)        1 2024-05-13 17:36:11.189460 codescout-0.1.6/src/codescout.egg-info/top_level.txt
+drwxr-xr-x   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 17:39:03.771073 codescout-0.1.7/
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)    11357 2024-05-13 14:57:56.000000 codescout-0.1.7/LICENSE
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)       23 2024-05-13 17:02:21.000000 codescout-0.1.7/MANIFEST.in
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)    17271 2024-05-13 17:39:03.770607 codescout-0.1.7/PKG-INFO
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)     3751 2024-05-13 14:57:56.000000 codescout-0.1.7/README.md
+drwxr-xr-x   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 17:39:03.768098 codescout-0.1.7/codescout/
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 17:38:44.000000 codescout-0.1.7/codescout/__init__.py
+-rwxr-xr-x   0 vfo001   (67203) eccc_rpnenv (66080)    20947 2024-05-13 15:13:31.000000 codescout-0.1.7/codescout/codescout.py
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)      700 2024-05-13 17:38:53.000000 codescout-0.1.7/pyproject.toml
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)       38 2024-05-13 17:39:03.771227 codescout-0.1.7/setup.cfg
+drwxr-xr-x   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 17:39:03.766177 codescout-0.1.7/src/
+drwxr-xr-x   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 17:39:03.769970 codescout-0.1.7/src/codescout.egg-info/
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)    17271 2024-05-13 17:39:03.768635 codescout-0.1.7/src/codescout.egg-info/PKG-INFO
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)      273 2024-05-13 17:39:03.769011 codescout-0.1.7/src/codescout.egg-info/SOURCES.txt
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)        1 2024-05-13 17:39:03.769377 codescout-0.1.7/src/codescout.egg-info/dependency_links.txt
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)       14 2024-05-13 17:39:03.769758 codescout-0.1.7/src/codescout.egg-info/requires.txt
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)        1 2024-05-13 17:39:03.770105 codescout-0.1.7/src/codescout.egg-info/top_level.txt
```

### Comparing `codescout-0.1.6/LICENSE` & `codescout-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `codescout-0.1.6/PKG-INFO` & `codescout-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codescout
-Version: 0.1.6
+Version: 0.1.7
 Summary: Permet de creer des codes scouts
 Author-email: Vincent Fortin <vincent.fortin@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `codescout-0.1.6/README.md` & `codescout-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `codescout-0.1.6/codescout/codescout.py` & `codescout-0.1.7/codescout/codescout.py`

 * *Files identical despite different names*

### Comparing `codescout-0.1.6/pyproject.toml` & `codescout-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=40.8.0"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "codescout"
-version = "0.1.6"
+version = "0.1.7"
 description = "Permet de creer des codes scouts"
 readme = "README.md"
 authors = [{ name = "Vincent Fortin", email = "vincent.fortin@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     'Development Status :: 3 - Alpha',
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `codescout-0.1.6/src/codescout.egg-info/PKG-INFO` & `codescout-0.1.7/src/codescout.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codescout
-Version: 0.1.6
+Version: 0.1.7
 Summary: Permet de creer des codes scouts
 Author-email: Vincent Fortin <vincent.fortin@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

