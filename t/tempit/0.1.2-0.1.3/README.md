# Comparing `tmp/tempit-0.1.2.tar.gz` & `tmp/tempit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tempit-0.1.2.tar", last modified: Sun May 12 18:23:18 2024, max compression
+gzip compressed data, was "tempit-0.1.3.tar", last modified: Sun May 12 18:33:39 2024, max compression
```

## Comparing `tempit-0.1.2.tar` & `tempit-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mcrespo    (501) staff       (20)        0 2024-05-12 18:23:18.932289 tempit-0.1.2/
--rw-r--r--   0 mcrespo    (501) staff       (20)     1068 2024-05-11 14:15:52.000000 tempit-0.1.2/LICENSE.txt
--rw-r--r--   0 mcrespo    (501) staff       (20)     3748 2024-05-12 18:23:18.932033 tempit-0.1.2/PKG-INFO
--rw-r--r--   0 mcrespo    (501) staff       (20)     3128 2024-05-12 10:42:15.000000 tempit-0.1.2/README.md
--rw-r--r--   0 mcrespo    (501) staff       (20)       38 2024-05-12 18:23:18.932341 tempit-0.1.2/setup.cfg
--rw-r--r--   0 mcrespo    (501) staff       (20)      808 2024-05-12 17:03:50.000000 tempit-0.1.2/setup.py
-drwxr-xr-x   0 mcrespo    (501) staff       (20)        0 2024-05-12 18:23:18.930832 tempit-0.1.2/tempit/
--rw-r--r--   0 mcrespo    (501) staff       (20)       47 2024-05-11 14:15:52.000000 tempit-0.1.2/tempit/__init__.py
--rw-r--r--   0 mcrespo    (501) staff       (20)     9442 2024-05-12 18:10:08.000000 tempit-0.1.2/tempit/core.py
--rw-r--r--   0 mcrespo    (501) staff       (20)     5353 2024-05-12 10:36:44.000000 tempit-0.1.2/tempit/utils.py
-drwxr-xr-x   0 mcrespo    (501) staff       (20)        0 2024-05-12 18:23:18.931822 tempit-0.1.2/tempit.egg-info/
--rw-r--r--   0 mcrespo    (501) staff       (20)     3748 2024-05-12 18:23:18.000000 tempit-0.1.2/tempit.egg-info/PKG-INFO
--rw-r--r--   0 mcrespo    (501) staff       (20)      250 2024-05-12 18:23:18.000000 tempit-0.1.2/tempit.egg-info/SOURCES.txt
--rw-r--r--   0 mcrespo    (501) staff       (20)        1 2024-05-12 18:23:18.000000 tempit-0.1.2/tempit.egg-info/dependency_links.txt
--rw-r--r--   0 mcrespo    (501) staff       (20)        7 2024-05-12 18:23:18.000000 tempit-0.1.2/tempit.egg-info/requires.txt
--rw-r--r--   0 mcrespo    (501) staff       (20)        7 2024-05-12 18:23:18.000000 tempit-0.1.2/tempit.egg-info/top_level.txt
-drwxr-xr-x   0 mcrespo    (501) staff       (20)        0 2024-05-12 18:23:18.931587 tempit-0.1.2/tests/
--rw-r--r--   0 mcrespo    (501) staff       (20)    12230 2024-05-12 18:04:54.000000 tempit-0.1.2/tests/test_tempit.py
+drwxr-xr-x   0 mcrespo    (501) staff       (20)        0 2024-05-12 18:33:39.152836 tempit-0.1.3/
+-rw-r--r--   0 mcrespo    (501) staff       (20)     1068 2024-05-11 14:15:52.000000 tempit-0.1.3/LICENSE.txt
+-rw-r--r--   0 mcrespo    (501) staff       (20)     3748 2024-05-12 18:33:39.152625 tempit-0.1.3/PKG-INFO
+-rw-r--r--   0 mcrespo    (501) staff       (20)     3128 2024-05-12 10:42:15.000000 tempit-0.1.3/README.md
+-rw-r--r--   0 mcrespo    (501) staff       (20)       38 2024-05-12 18:33:39.152878 tempit-0.1.3/setup.cfg
+-rw-r--r--   0 mcrespo    (501) staff       (20)      839 2024-05-12 18:31:57.000000 tempit-0.1.3/setup.py
+drwxr-xr-x   0 mcrespo    (501) staff       (20)        0 2024-05-12 18:33:39.151474 tempit-0.1.3/tempit/
+-rw-r--r--   0 mcrespo    (501) staff       (20)       47 2024-05-11 14:15:52.000000 tempit-0.1.3/tempit/__init__.py
+-rw-r--r--   0 mcrespo    (501) staff       (20)     9442 2024-05-12 18:10:08.000000 tempit-0.1.3/tempit/core.py
+-rw-r--r--   0 mcrespo    (501) staff       (20)     5353 2024-05-12 10:36:44.000000 tempit-0.1.3/tempit/utils.py
+drwxr-xr-x   0 mcrespo    (501) staff       (20)        0 2024-05-12 18:33:39.152413 tempit-0.1.3/tempit.egg-info/
+-rw-r--r--   0 mcrespo    (501) staff       (20)     3748 2024-05-12 18:33:39.000000 tempit-0.1.3/tempit.egg-info/PKG-INFO
+-rw-r--r--   0 mcrespo    (501) staff       (20)      250 2024-05-12 18:33:39.000000 tempit-0.1.3/tempit.egg-info/SOURCES.txt
+-rw-r--r--   0 mcrespo    (501) staff       (20)        1 2024-05-12 18:33:39.000000 tempit-0.1.3/tempit.egg-info/dependency_links.txt
+-rw-r--r--   0 mcrespo    (501) staff       (20)        7 2024-05-12 18:33:39.000000 tempit-0.1.3/tempit.egg-info/requires.txt
+-rw-r--r--   0 mcrespo    (501) staff       (20)        7 2024-05-12 18:33:39.000000 tempit-0.1.3/tempit.egg-info/top_level.txt
+drwxr-xr-x   0 mcrespo    (501) staff       (20)        0 2024-05-12 18:33:39.152224 tempit-0.1.3/tests/
+-rw-r--r--   0 mcrespo    (501) staff       (20)    12230 2024-05-12 18:04:54.000000 tempit-0.1.3/tests/test_tempit.py
```

### Comparing `tempit-0.1.2/LICENSE.txt` & `tempit-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tempit-0.1.2/PKG-INFO` & `tempit-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempit
-Version: 0.1.2
+Version: 0.1.3
 Summary: A dead simple time decorator
 Home-page: https://github.com/mcrespoae/tempit
 Author: mcrespoae
 Author-email: info@mariocrespo.es
 Keywords: tempit,time,decorator,performance,concurrency,parallel,benchmark
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tempit-0.1.2/README.md` & `tempit-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tempit-0.1.2/setup.py` & `tempit-0.1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup
 
-VERSION = "0.1.2"
+VERSION = "0.1.3"
 setup(
     name="tempit",
     version=VERSION,
     author="mcrespoae",
     author_email="info@mariocrespo.es",
     packages=["tempit"],
     description="A dead simple time decorator",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/mcrespoae/tempit",
     install_requires=["joblib"],
+    setup_requires=["joblib"],
     python_requires=">=3.8",
     keywords=["tempit", "time", "decorator", "performance", "concurrency", "parallel", "benchmark"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `tempit-0.1.2/tempit/core.py` & `tempit-0.1.3/tempit/core.py`

 * *Files identical despite different names*

### Comparing `tempit-0.1.2/tempit/utils.py` & `tempit-0.1.3/tempit/utils.py`

 * *Files identical despite different names*

### Comparing `tempit-0.1.2/tempit.egg-info/PKG-INFO` & `tempit-0.1.3/tempit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempit
-Version: 0.1.2
+Version: 0.1.3
 Summary: A dead simple time decorator
 Home-page: https://github.com/mcrespoae/tempit
 Author: mcrespoae
 Author-email: info@mariocrespo.es
 Keywords: tempit,time,decorator,performance,concurrency,parallel,benchmark
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tempit-0.1.2/tests/test_tempit.py` & `tempit-0.1.3/tests/test_tempit.py`

 * *Files identical despite different names*

