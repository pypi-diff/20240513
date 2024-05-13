# Comparing `tmp/tpsimilarity-0.2.tar.gz` & `tmp/tpsimilarity-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tpsimilarity-0.2.tar", last modified: Mon May 13 11:42:23 2024, max compression
+gzip compressed data, was "tpsimilarity-0.3.tar", last modified: Mon May 13 12:18:46 2024, max compression
```

## Comparing `tpsimilarity-0.2.tar` & `tpsimilarity-0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 filsilva   (501) staff       (20)        0 2024-05-13 11:42:23.687273 tpsimilarity-0.2/
--rw-rw-r--   0 filsilva   (501) staff       (20)     1080 2024-01-15 19:55:19.000000 tpsimilarity-0.2/LICENSE
--rw-rw-r--   0 filsilva   (501) staff       (20)       43 2024-01-15 19:55:19.000000 tpsimilarity-0.2/MANIFEST.in
--rw-r--r--   0 filsilva   (501) staff       (20)     4246 2024-05-13 11:42:23.687147 tpsimilarity-0.2/PKG-INFO
--rw-rw-r--   0 filsilva   (501) staff       (20)     3705 2024-01-15 19:55:19.000000 tpsimilarity-0.2/README.md
--rw-rw-r--   0 filsilva   (501) staff       (20)       67 2024-04-02 14:03:38.000000 tpsimilarity-0.2/requirements.txt
--rw-r--r--   0 filsilva   (501) staff       (20)       38 2024-05-13 11:42:23.687325 tpsimilarity-0.2/setup.cfg
--rw-rw-r--   0 filsilva   (501) staff       (20)      846 2024-05-13 11:40:31.000000 tpsimilarity-0.2/setup.py
-drwxr-xr-x   0 filsilva   (501) staff       (20)        0 2024-05-13 11:42:23.686353 tpsimilarity-0.2/tpdistance/
--rw-r--r--   0 filsilva   (501) staff       (20)       61 2024-04-16 14:28:02.000000 tpsimilarity-0.2/tpdistance/__init__.py
--rw-r--r--   0 filsilva   (501) staff       (20)    12052 2024-05-13 11:41:41.000000 tpsimilarity-0.2/tpdistance/similarity.py
-drwxr-xr-x   0 filsilva   (501) staff       (20)        0 2024-05-13 11:42:23.686967 tpsimilarity-0.2/tpsimilarity.egg-info/
--rw-r--r--   0 filsilva   (501) staff       (20)     4246 2024-05-13 11:42:23.000000 tpsimilarity-0.2/tpsimilarity.egg-info/PKG-INFO
--rw-r--r--   0 filsilva   (501) staff       (20)      282 2024-05-13 11:42:23.000000 tpsimilarity-0.2/tpsimilarity.egg-info/SOURCES.txt
--rw-r--r--   0 filsilva   (501) staff       (20)        1 2024-05-13 11:42:23.000000 tpsimilarity-0.2/tpsimilarity.egg-info/dependency_links.txt
--rw-r--r--   0 filsilva   (501) staff       (20)       67 2024-05-13 11:42:23.000000 tpsimilarity-0.2/tpsimilarity.egg-info/requires.txt
--rw-r--r--   0 filsilva   (501) staff       (20)       11 2024-05-13 11:42:23.000000 tpsimilarity-0.2/tpsimilarity.egg-info/top_level.txt
+drwxr-xr-x   0 filsilva   (501) staff       (20)        0 2024-05-13 12:18:46.526239 tpsimilarity-0.3/
+-rw-rw-r--   0 filsilva   (501) staff       (20)     1080 2024-01-15 19:55:19.000000 tpsimilarity-0.3/LICENSE
+-rw-rw-r--   0 filsilva   (501) staff       (20)       43 2024-01-15 19:55:19.000000 tpsimilarity-0.3/MANIFEST.in
+-rw-r--r--   0 filsilva   (501) staff       (20)     4246 2024-05-13 12:18:46.526107 tpsimilarity-0.3/PKG-INFO
+-rw-rw-r--   0 filsilva   (501) staff       (20)     3705 2024-01-15 19:55:19.000000 tpsimilarity-0.3/README.md
+-rw-rw-r--   0 filsilva   (501) staff       (20)       67 2024-04-02 14:03:38.000000 tpsimilarity-0.3/requirements.txt
+-rw-r--r--   0 filsilva   (501) staff       (20)       38 2024-05-13 12:18:46.526305 tpsimilarity-0.3/setup.cfg
+-rw-rw-r--   0 filsilva   (501) staff       (20)      846 2024-05-13 12:18:39.000000 tpsimilarity-0.3/setup.py
+drwxr-xr-x   0 filsilva   (501) staff       (20)        0 2024-05-13 12:18:46.525286 tpsimilarity-0.3/tpsimilarity/
+-rw-r--r--   0 filsilva   (501) staff       (20)       61 2024-04-16 14:28:02.000000 tpsimilarity-0.3/tpsimilarity/__init__.py
+-rw-r--r--   0 filsilva   (501) staff       (20)    12052 2024-05-13 12:18:09.000000 tpsimilarity-0.3/tpsimilarity/similarity.py
+drwxr-xr-x   0 filsilva   (501) staff       (20)        0 2024-05-13 12:18:46.525904 tpsimilarity-0.3/tpsimilarity.egg-info/
+-rw-r--r--   0 filsilva   (501) staff       (20)     4246 2024-05-13 12:18:46.000000 tpsimilarity-0.3/tpsimilarity.egg-info/PKG-INFO
+-rw-r--r--   0 filsilva   (501) staff       (20)      286 2024-05-13 12:18:46.000000 tpsimilarity-0.3/tpsimilarity.egg-info/SOURCES.txt
+-rw-r--r--   0 filsilva   (501) staff       (20)        1 2024-05-13 12:18:46.000000 tpsimilarity-0.3/tpsimilarity.egg-info/dependency_links.txt
+-rw-r--r--   0 filsilva   (501) staff       (20)       67 2024-05-13 12:18:46.000000 tpsimilarity-0.3/tpsimilarity.egg-info/requires.txt
+-rw-r--r--   0 filsilva   (501) staff       (20)       13 2024-05-13 12:18:46.000000 tpsimilarity-0.3/tpsimilarity.egg-info/top_level.txt
```

### Comparing `tpsimilarity-0.2/LICENSE` & `tpsimilarity-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tpsimilarity-0.2/PKG-INFO` & `tpsimilarity-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tpsimilarity
-Version: 0.2
+Version: 0.3
 Summary: Package to compute TP similarities between nodes in a network.
 Home-page: https://github.com/attilavarga/tpsimilarity
 Author: Filipi N. Silva and Sadamori Kojaku and Attila Varga
 Author-email: filsilva@iu.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tpsimilarity-0.2/README.md` & `tpsimilarity-0.3/README.md`

 * *Files identical despite different names*

### Comparing `tpsimilarity-0.2/setup.py` & `tpsimilarity-0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as f:
     required_packages = f.read().splitlines()
 
 setuptools.setup(
     name="tpsimilarity",
-    version="0.2",
+    version="0.3",
     author="Filipi N. Silva and Sadamori Kojaku and Attila Varga",
     author_email="filsilva@iu.edu",
     description="Package to compute TP similarities between nodes in a network.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/attilavarga/tpsimilarity",
     packages=setuptools.find_packages(),
```

### Comparing `tpsimilarity-0.2/tpdistance/similarity.py` & `tpsimilarity-0.3/tpsimilarity/similarity.py`

 * *Files identical despite different names*

### Comparing `tpsimilarity-0.2/tpsimilarity.egg-info/PKG-INFO` & `tpsimilarity-0.3/tpsimilarity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tpsimilarity
-Version: 0.2
+Version: 0.3
 Summary: Package to compute TP similarities between nodes in a network.
 Home-page: https://github.com/attilavarga/tpsimilarity
 Author: Filipi N. Silva and Sadamori Kojaku and Attila Varga
 Author-email: filsilva@iu.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

