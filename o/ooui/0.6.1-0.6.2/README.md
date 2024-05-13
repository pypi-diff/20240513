# Comparing `tmp/ooui-0.6.1.tar.gz` & `tmp/ooui-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ooui-0.6.1.tar", last modified: Mon May 13 15:30:15 2024, max compression
+gzip compressed data, was "ooui-0.6.2.tar", last modified: Mon May 13 15:38:30 2024, max compression
```

## Comparing `ooui-0.6.1.tar` & `ooui-0.6.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:30:15.000000 ooui-0.6.1/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      562 2024-05-13 15:29:49.000000 ooui-0.6.1/setup.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       38 2024-05-13 15:30:15.000000 ooui-0.6.1/setup.cfg
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:30:15.000000 ooui-0.6.1/ooui.egg-info/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        5 2024-05-13 15:30:15.000000 ooui-0.6.1/ooui.egg-info/top_level.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       43 2024-05-13 15:30:15.000000 ooui-0.6.1/ooui.egg-info/requires.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      431 2024-05-13 15:30:15.000000 ooui-0.6.1/ooui.egg-info/SOURCES.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        1 2024-05-13 15:30:15.000000 ooui-0.6.1/ooui.egg-info/dependency_links.txt
--rw-r--r--   0 ecarreras  (1000) ecarreras  (1000)      276 2024-05-13 15:30:15.000000 ooui-0.6.1/ooui.egg-info/PKG-INFO
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:30:15.000000 ooui-0.6.1/ooui/
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:30:15.000000 ooui-0.6.1/ooui/helpers/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      971 2024-05-13 14:52:41.000000 ooui-0.6.1/ooui/helpers/domain.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1407 2024-05-13 14:13:20.000000 ooui-0.6.1/ooui/helpers/conditions.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      526 2024-05-06 17:19:46.000000 ooui-0.6.1/ooui/helpers/__init__.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-06 16:22:58.000000 ooui-0.6.1/ooui/__init__.py
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:30:15.000000 ooui-0.6.1/ooui/graph/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      783 2024-05-10 12:49:23.000000 ooui-0.6.1/ooui/graph/base.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2996 2024-05-13 15:00:24.000000 ooui-0.6.1/ooui/graph/processor.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     3305 2024-05-10 12:09:54.000000 ooui-0.6.1/ooui/graph/fields.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     9439 2024-05-08 12:28:50.000000 ooui-0.6.1/ooui/graph/timerange.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      779 2024-05-10 12:16:14.000000 ooui-0.6.1/ooui/graph/__init__.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2696 2024-05-13 15:27:59.000000 ooui-0.6.1/ooui/graph/indicator.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2599 2024-05-08 10:59:34.000000 ooui-0.6.1/ooui/graph/axis.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     5632 2024-05-10 12:48:45.000000 ooui-0.6.1/ooui/graph/chart.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       40 2024-05-06 16:18:58.000000 ooui-0.6.1/README.md
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1065 2024-05-06 16:18:58.000000 ooui-0.6.1/LICENSE
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      276 2024-05-13 15:30:15.000000 ooui-0.6.1/PKG-INFO
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:38:30.162073 ooui-0.6.2/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1065 2024-05-06 16:18:58.000000 ooui-0.6.2/LICENSE
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      268 2024-05-13 15:38:30.162073 ooui-0.6.2/PKG-INFO
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       40 2024-05-06 16:18:58.000000 ooui-0.6.2/README.md
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:38:30.158073 ooui-0.6.2/ooui/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-06 16:22:58.000000 ooui-0.6.2/ooui/__init__.py
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:38:30.162073 ooui-0.6.2/ooui/graph/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      779 2024-05-10 12:16:14.000000 ooui-0.6.2/ooui/graph/__init__.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2599 2024-05-08 10:59:34.000000 ooui-0.6.2/ooui/graph/axis.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      783 2024-05-10 12:49:23.000000 ooui-0.6.2/ooui/graph/base.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     5632 2024-05-10 12:48:45.000000 ooui-0.6.2/ooui/graph/chart.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     3305 2024-05-10 12:09:54.000000 ooui-0.6.2/ooui/graph/fields.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2696 2024-05-13 15:27:59.000000 ooui-0.6.2/ooui/graph/indicator.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2996 2024-05-13 15:00:24.000000 ooui-0.6.2/ooui/graph/processor.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     9439 2024-05-08 12:28:50.000000 ooui-0.6.2/ooui/graph/timerange.py
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:38:30.162073 ooui-0.6.2/ooui/helpers/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      526 2024-05-06 17:19:46.000000 ooui-0.6.2/ooui/helpers/__init__.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1407 2024-05-13 14:13:20.000000 ooui-0.6.2/ooui/helpers/conditions.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1088 2024-05-13 15:37:47.000000 ooui-0.6.2/ooui/helpers/domain.py
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:38:30.162073 ooui-0.6.2/ooui.egg-info/
+-rw-r--r--   0 ecarreras  (1000) ecarreras  (1000)      268 2024-05-13 15:38:30.000000 ooui-0.6.2/ooui.egg-info/PKG-INFO
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      431 2024-05-13 15:38:30.000000 ooui-0.6.2/ooui.egg-info/SOURCES.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        1 2024-05-13 15:38:30.000000 ooui-0.6.2/ooui.egg-info/dependency_links.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       43 2024-05-13 15:38:30.000000 ooui-0.6.2/ooui.egg-info/requires.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        5 2024-05-13 15:38:30.000000 ooui-0.6.2/ooui.egg-info/top_level.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       38 2024-05-13 15:38:30.162073 ooui-0.6.2/setup.cfg
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      562 2024-05-13 15:38:02.000000 ooui-0.6.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ooui-0.6.1/setup.py` & `ooui-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 setup(
     name='ooui',
     description='Open Object User Interface',
     author='GISCE',
     author_email='devel@gisce.net',
     url='https://github.com/gisce/python-ooui',
-    version='0.6.1',
+    version='0.6.2',
     license='MIT',
     long_description='''Open Object User Interface for GISCE-ERP''',
     provides=['ooui'],
     install_requires=[
         'lxml',
         'python-dateutil',
         'six',
```

### Comparing `ooui-0.6.1/ooui/helpers/domain.py` & `ooui-0.6.2/ooui/helpers/domain.py`

 * *Files 22% similar despite different names*

```diff
@@ -32,7 +32,13 @@
         s = EvalWithCompoundTypes(
             names=values, functions=EVAL_FUNCTIONS, operators=operators
         )
         return s.eval(self.domain)
 
     def __str__(self):
         return self.domain
+
+    def __bool__(self):
+        return bool(self.domain)
+
+    def __nonzero__(self):
+        return self.__bool__()
```

### Comparing `ooui-0.6.1/ooui/helpers/conditions.py` & `ooui-0.6.2/ooui/helpers/conditions.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.1/ooui/helpers/__init__.py` & `ooui-0.6.2/ooui/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.1/ooui/graph/base.py` & `ooui-0.6.2/ooui/graph/base.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.1/ooui/graph/processor.py` & `ooui-0.6.2/ooui/graph/processor.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.1/ooui/graph/fields.py` & `ooui-0.6.2/ooui/graph/fields.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.1/ooui/graph/timerange.py` & `ooui-0.6.2/ooui/graph/timerange.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.1/ooui/graph/__init__.py` & `ooui-0.6.2/ooui/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.1/ooui/graph/indicator.py` & `ooui-0.6.2/ooui/graph/indicator.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.1/ooui/graph/axis.py` & `ooui-0.6.2/ooui/graph/axis.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.1/ooui/graph/chart.py` & `ooui-0.6.2/ooui/graph/chart.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.1/LICENSE` & `ooui-0.6.2/LICENSE`

 * *Files identical despite different names*

