# Comparing `tmp/RTS_Tunnel-0.1.tar.gz` & `tmp/RTS_Tunnel-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RTS_Tunnel-0.1.tar", last modified: Mon May 13 18:38:48 2024, max compression
+gzip compressed data, was "RTS_Tunnel-0.2.tar", last modified: Mon May 13 18:47:31 2024, max compression
```

## Comparing `RTS_Tunnel-0.1.tar` & `RTS_Tunnel-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 18:38:48.367967 RTS_Tunnel-0.1/
--rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 RTS_Tunnel-0.1/LICENCE
--rw-rw-rw-   0        0        0      716 2024-05-13 18:38:48.367463 RTS_Tunnel-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       16 2024-05-13 18:35:24.000000 RTS_Tunnel-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 18:38:48.366456 RTS_Tunnel-0.1/RTS_Tunnel.egg-info/
--rw-rw-rw-   0        0        0      716 2024-05-13 18:38:48.000000 RTS_Tunnel-0.1/RTS_Tunnel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2024-05-13 18:38:48.000000 RTS_Tunnel-0.1/RTS_Tunnel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 18:38:48.000000 RTS_Tunnel-0.1/RTS_Tunnel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-05-13 18:38:48.000000 RTS_Tunnel-0.1/RTS_Tunnel.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 18:38:48.000000 RTS_Tunnel-0.1/RTS_Tunnel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 18:38:48.367967 RTS_Tunnel-0.1/setup.cfg
--rw-rw-rw-   0        0        0      894 2024-05-13 18:37:05.000000 RTS_Tunnel-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:47:31.046620 RTS_Tunnel-0.2/
+-rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 RTS_Tunnel-0.2/LICENCE
+-rw-rw-rw-   0        0        0      716 2024-05-13 18:47:31.046620 RTS_Tunnel-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2024-05-13 18:35:24.000000 RTS_Tunnel-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 18:47:31.045112 RTS_Tunnel-0.2/RTS_Tunnel.egg-info/
+-rw-rw-rw-   0        0        0      716 2024-05-13 18:47:30.000000 RTS_Tunnel-0.2/RTS_Tunnel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2024-05-13 18:47:30.000000 RTS_Tunnel-0.2/RTS_Tunnel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 18:47:30.000000 RTS_Tunnel-0.2/RTS_Tunnel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-05-13 18:47:30.000000 RTS_Tunnel-0.2/RTS_Tunnel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 18:47:30.000000 RTS_Tunnel-0.2/RTS_Tunnel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 18:47:31.047122 RTS_Tunnel-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      894 2024-05-13 18:47:27.000000 RTS_Tunnel-0.2/setup.py
```

### Comparing `RTS_Tunnel-0.1/LICENCE` & `RTS_Tunnel-0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `RTS_Tunnel-0.1/PKG-INFO` & `RTS_Tunnel-0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RTS_Tunnel
-Version: 0.1
+Version: 0.2
 Summary: Work in progress, a tunneling system for RTS_DataBase.
 Home-page: https://github.com/RandomTimeLP/RTS_DataBase/
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: database
 Platform: UNKNOWN
```

### Comparing `RTS_Tunnel-0.1/RTS_Tunnel.egg-info/PKG-INFO` & `RTS_Tunnel-0.2/RTS_Tunnel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RTS-Tunnel
-Version: 0.1
+Version: 0.2
 Summary: Work in progress, a tunneling system for RTS_DataBase.
 Home-page: https://github.com/RandomTimeLP/RTS_DataBase/
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: database
 Platform: UNKNOWN
```

### Comparing `RTS_Tunnel-0.1/setup.py` & `RTS_Tunnel-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RTS_Tunnel',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     description='Work in progress, a tunneling system for RTS_DataBase.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='MIT with required credit to the author.',
```

