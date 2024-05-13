# Comparing `tmp/ooui-0.2.0.tar.gz` & `tmp/ooui-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ooui-0.2.0.tar", last modified: Fri May 10 13:16:14 2024, max compression
+gzip compressed data, was "dist/ooui-0.5.0.tar", last modified: Mon May 13 14:33:44 2024, max compression
```

## Comparing `ooui-0.2.0.tar` & `ooui-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-10 13:16:14.842532 ooui-0.2.0/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1065 2024-05-06 16:18:58.000000 ooui-0.2.0/LICENSE
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      268 2024-05-10 13:16:14.842532 ooui-0.2.0/PKG-INFO
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       40 2024-05-06 16:18:58.000000 ooui-0.2.0/README.md
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-10 13:16:14.838532 ooui-0.2.0/ooui/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-06 16:22:58.000000 ooui-0.2.0/ooui/__init__.py
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-10 13:16:14.838532 ooui-0.2.0/ooui/graph/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      779 2024-05-10 12:16:14.000000 ooui-0.2.0/ooui/graph/__init__.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2599 2024-05-08 10:59:34.000000 ooui-0.2.0/ooui/graph/axis.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      783 2024-05-10 12:49:23.000000 ooui-0.2.0/ooui/graph/base.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     5632 2024-05-10 12:48:45.000000 ooui-0.2.0/ooui/graph/chart.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     3305 2024-05-10 12:09:54.000000 ooui-0.2.0/ooui/graph/fields.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1859 2024-05-10 13:12:52.000000 ooui-0.2.0/ooui/graph/indicator.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2900 2024-05-10 12:48:29.000000 ooui-0.2.0/ooui/graph/processor.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     9439 2024-05-08 12:28:50.000000 ooui-0.2.0/ooui/graph/timerange.py
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-10 13:16:14.842532 ooui-0.2.0/ooui/helpers/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      526 2024-05-06 17:19:46.000000 ooui-0.2.0/ooui/helpers/__init__.py
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-10 13:16:14.838532 ooui-0.2.0/ooui.egg-info/
--rw-r--r--   0 ecarreras  (1000) ecarreras  (1000)      268 2024-05-10 13:16:14.000000 ooui-0.2.0/ooui.egg-info/PKG-INFO
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      381 2024-05-10 13:16:14.000000 ooui-0.2.0/ooui.egg-info/SOURCES.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        1 2024-05-10 13:16:14.000000 ooui-0.2.0/ooui.egg-info/dependency_links.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       25 2024-05-10 13:16:14.000000 ooui-0.2.0/ooui.egg-info/requires.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        5 2024-05-10 13:16:14.000000 ooui-0.2.0/ooui.egg-info/top_level.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       38 2024-05-10 13:16:14.842532 ooui-0.2.0/setup.cfg
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      533 2024-05-10 13:15:09.000000 ooui-0.2.0/setup.py
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 14:33:44.000000 ooui-0.5.0/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      562 2024-05-13 14:32:56.000000 ooui-0.5.0/setup.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       38 2024-05-13 14:33:44.000000 ooui-0.5.0/setup.cfg
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 14:33:44.000000 ooui-0.5.0/ooui.egg-info/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        5 2024-05-13 14:33:44.000000 ooui-0.5.0/ooui.egg-info/top_level.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       43 2024-05-13 14:33:44.000000 ooui-0.5.0/ooui.egg-info/requires.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      408 2024-05-13 14:33:44.000000 ooui-0.5.0/ooui.egg-info/SOURCES.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        1 2024-05-13 14:33:44.000000 ooui-0.5.0/ooui.egg-info/dependency_links.txt
+-rw-r--r--   0 ecarreras  (1000) ecarreras  (1000)      276 2024-05-13 14:33:44.000000 ooui-0.5.0/ooui.egg-info/PKG-INFO
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 14:33:44.000000 ooui-0.5.0/ooui/
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 14:33:44.000000 ooui-0.5.0/ooui/helpers/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1407 2024-05-13 14:13:20.000000 ooui-0.5.0/ooui/helpers/conditions.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      526 2024-05-06 17:19:46.000000 ooui-0.5.0/ooui/helpers/__init__.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-06 16:22:58.000000 ooui-0.5.0/ooui/__init__.py
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 14:33:44.000000 ooui-0.5.0/ooui/graph/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      783 2024-05-10 12:49:23.000000 ooui-0.5.0/ooui/graph/base.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2900 2024-05-10 12:48:29.000000 ooui-0.5.0/ooui/graph/processor.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     3305 2024-05-10 12:09:54.000000 ooui-0.5.0/ooui/graph/fields.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     9439 2024-05-08 12:28:50.000000 ooui-0.5.0/ooui/graph/timerange.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      779 2024-05-10 12:16:14.000000 ooui-0.5.0/ooui/graph/__init__.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2611 2024-05-13 14:32:17.000000 ooui-0.5.0/ooui/graph/indicator.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2599 2024-05-08 10:59:34.000000 ooui-0.5.0/ooui/graph/axis.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     5632 2024-05-10 12:48:45.000000 ooui-0.5.0/ooui/graph/chart.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       40 2024-05-06 16:18:58.000000 ooui-0.5.0/README.md
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1065 2024-05-06 16:18:58.000000 ooui-0.5.0/LICENSE
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      276 2024-05-13 14:33:44.000000 ooui-0.5.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `ooui-0.2.0/LICENSE` & `ooui-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ooui-0.2.0/ooui/graph/__init__.py` & `ooui-0.5.0/ooui/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `ooui-0.2.0/ooui/graph/axis.py` & `ooui-0.5.0/ooui/graph/axis.py`

 * *Files identical despite different names*

### Comparing `ooui-0.2.0/ooui/graph/base.py` & `ooui-0.5.0/ooui/graph/base.py`

 * *Files identical despite different names*

### Comparing `ooui-0.2.0/ooui/graph/chart.py` & `ooui-0.5.0/ooui/graph/chart.py`

 * *Files identical despite different names*

### Comparing `ooui-0.2.0/ooui/graph/fields.py` & `ooui-0.5.0/ooui/graph/fields.py`

 * *Files identical despite different names*

### Comparing `ooui-0.2.0/ooui/graph/processor.py` & `ooui-0.5.0/ooui/graph/processor.py`

 * *Files identical despite different names*

### Comparing `ooui-0.2.0/ooui/graph/timerange.py` & `ooui-0.5.0/ooui/graph/timerange.py`

 * *Files identical despite different names*

### Comparing `ooui-0.2.0/ooui/helpers/__init__.py` & `ooui-0.5.0/ooui/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ooui-0.2.0/setup.py` & `ooui-0.5.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 
 setup(
     name='ooui',
     description='Open Object User Interface',
     author='GISCE',
     author_email='devel@gisce.net',
     url='https://github.com/gisce/python-ooui',
-    version='0.2.0',
+    version='0.5.0',
     license='MIT',
     long_description='''Open Object User Interface for GISCE-ERP''',
     provides=['ooui'],
     install_requires=[
         'lxml',
         'python-dateutil',
         'six',
+        'simpleeval<0.9.12',
     ],
     tests_require=[
         'mamba',
         'expects',
     ],
     packages=find_packages()
 )
```

