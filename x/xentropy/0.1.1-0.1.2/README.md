# Comparing `tmp/xentropy-0.1.1.tar.gz` & `tmp/xentropy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xentropy-0.1.1.tar", last modified: Thu May  9 12:04:24 2024, max compression
+gzip compressed data, was "xentropy-0.1.2.tar", last modified: Mon May 13 03:47:38 2024, max compression
```

## Comparing `xentropy-0.1.1.tar` & `xentropy-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:02:26.330063 xentropy-0.1.1/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       80 2024-05-09 12:04:24.694291 xentropy-0.1.1/PKG-INFO
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      314 2024-05-09 02:41:29.000000 xentropy-0.1.1/README.md
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2290 2024-05-09 02:41:29.000000 xentropy-0.1.1/interface.cpp
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       38 2024-05-09 12:04:24.697738 xentropy-0.1.1/setup.cfg
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5770 2024-05-09 12:02:39.000000 xentropy-0.1.1/setup.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:02:26.321438 xentropy-0.1.1/xentropy.egg-info/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       80 2024-05-09 12:04:23.000000 xentropy-0.1.1/xentropy.egg-info/PKG-INFO
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      179 2024-05-09 12:04:24.000000 xentropy-0.1.1/xentropy.egg-info/SOURCES.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        1 2024-05-09 12:04:23.000000 xentropy-0.1.1/xentropy.egg-info/dependency_links.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       18 2024-05-09 12:04:23.000000 xentropy-0.1.1/xentropy.egg-info/top_level.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    25783 2024-05-09 02:41:29.000000 xentropy-0.1.1/xentropy_kernel.cu
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:45:38.738817 xentropy-0.1.2/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       80 2024-05-13 03:47:38.875879 xentropy-0.1.2/PKG-INFO
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      314 2024-05-11 06:37:47.000000 xentropy-0.1.2/README.md
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2290 2024-05-11 06:37:47.000000 xentropy-0.1.2/interface.cpp
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       38 2024-05-13 03:47:38.881256 xentropy-0.1.2/setup.cfg
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5770 2024-05-13 03:32:16.000000 xentropy-0.1.2/setup.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:45:38.728483 xentropy-0.1.2/xentropy.egg-info/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       80 2024-05-13 03:47:38.000000 xentropy-0.1.2/xentropy.egg-info/PKG-INFO
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      179 2024-05-13 03:47:38.000000 xentropy-0.1.2/xentropy.egg-info/SOURCES.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        1 2024-05-13 03:47:38.000000 xentropy-0.1.2/xentropy.egg-info/dependency_links.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       18 2024-05-13 03:47:38.000000 xentropy-0.1.2/xentropy.egg-info/top_level.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    25783 2024-05-11 06:37:47.000000 xentropy-0.1.2/xentropy_kernel.cu
```

### Comparing `xentropy-0.1.1/interface.cpp` & `xentropy-0.1.2/interface.cpp`

 * *Files identical despite different names*

### Comparing `xentropy-0.1.1/setup.py` & `xentropy-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 class CustomBdistWheel(bdist_wheel):
     def finalize_options(self):
         bdist_wheel.finalize_options(self)
         self.plat_name = 'manylinux2014_x86_64'
 
 setup(
     name="xentropy",
-    version="0.1.1",
+    version="0.1.2",
     description="Cross-entropy loss",
     ext_modules=ext_modules,
     cmdclass={
         "build_ext": BuildExtension,
         "bdist_wheel": CustomBdistWheel
     },
 )
```

### Comparing `xentropy-0.1.1/xentropy_kernel.cu` & `xentropy-0.1.2/xentropy_kernel.cu`

 * *Files identical despite different names*

