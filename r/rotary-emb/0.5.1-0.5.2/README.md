# Comparing `tmp/rotary_emb-0.5.1.tar.gz` & `tmp/rotary_emb-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotary_emb-0.5.1.tar", last modified: Thu May  9 12:03:14 2024, max compression
+gzip compressed data, was "rotary_emb-0.5.2.tar", last modified: Mon May 13 03:46:22 2024, max compression
```

## Comparing `rotary_emb-0.5.1.tar` & `rotary_emb-0.5.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:15.777793 rotary_emb-0.5.1/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       54 2024-05-09 12:03:14.141719 rotary_emb-0.5.1/PKG-INFO
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1612 2024-05-06 07:30:03.000000 rotary_emb-0.5.1/rotary.cpp
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1791 2024-05-06 07:30:03.000000 rotary_emb-0.5.1/rotary_cuda.cu
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:15.768891 rotary_emb-0.5.1/rotary_emb.egg-info/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       54 2024-05-09 12:03:13.000000 rotary_emb-0.5.1/rotary_emb.egg-info/PKG-INFO
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      170 2024-05-09 12:03:13.000000 rotary_emb-0.5.1/rotary_emb.egg-info/SOURCES.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        1 2024-05-09 12:03:13.000000 rotary_emb-0.5.1/rotary_emb.egg-info/dependency_links.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       11 2024-05-09 12:03:13.000000 rotary_emb-0.5.1/rotary_emb.egg-info/top_level.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       38 2024-05-09 12:03:14.145305 rotary_emb-0.5.1/setup.cfg
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5292 2024-05-09 12:02:39.000000 rotary_emb-0.5.1/setup.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:22.143622 rotary_emb-0.5.2/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       54 2024-05-13 03:46:22.280497 rotary_emb-0.5.2/PKG-INFO
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1612 2024-05-11 06:37:47.000000 rotary_emb-0.5.2/rotary.cpp
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1791 2024-05-11 06:37:47.000000 rotary_emb-0.5.2/rotary_cuda.cu
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:22.134768 rotary_emb-0.5.2/rotary_emb.egg-info/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       54 2024-05-13 03:46:21.000000 rotary_emb-0.5.2/rotary_emb.egg-info/PKG-INFO
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      170 2024-05-13 03:46:22.000000 rotary_emb-0.5.2/rotary_emb.egg-info/SOURCES.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        1 2024-05-13 03:46:21.000000 rotary_emb-0.5.2/rotary_emb.egg-info/dependency_links.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       11 2024-05-13 03:46:21.000000 rotary_emb-0.5.2/rotary_emb.egg-info/top_level.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       38 2024-05-13 03:46:22.284111 rotary_emb-0.5.2/setup.cfg
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5292 2024-05-13 03:32:16.000000 rotary_emb-0.5.2/setup.py
```

### Comparing `rotary_emb-0.5.1/rotary.cpp` & `rotary_emb-0.5.2/rotary.cpp`

 * *Files identical despite different names*

### Comparing `rotary_emb-0.5.1/rotary_cuda.cu` & `rotary_emb-0.5.2/rotary_cuda.cu`

 * *Files identical despite different names*

### Comparing `rotary_emb-0.5.1/setup.py` & `rotary_emb-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,14 +118,14 @@
 class CustomBdistWheel(bdist_wheel):
     def finalize_options(self):
         bdist_wheel.finalize_options(self)
         self.plat_name = 'manylinux2014_x86_64'
 
 setup(
     name="rotary_emb",
-    version="0.5.1",
+    version="0.5.2",
     ext_modules=ext_modules,
     cmdclass={
         "build_ext": BuildExtension,
         "bdist_wheel": CustomBdistWheel
     },
 )
```

