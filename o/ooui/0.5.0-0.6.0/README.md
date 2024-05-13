# Comparing `tmp/ooui-0.5.0.tar.gz` & `tmp/ooui-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ooui-0.5.0.tar", last modified: Mon May 13 14:33:44 2024, max compression
+gzip compressed data, was "dist/ooui-0.6.0.tar", last modified: Mon May 13 15:06:54 2024, max compression
```

## Comparing `ooui-0.5.0.tar` & `ooui-0.6.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 14:33:44.000000 ooui-0.5.0/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      562 2024-05-13 14:32:56.000000 ooui-0.5.0/setup.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       38 2024-05-13 14:33:44.000000 ooui-0.5.0/setup.cfg
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 14:33:44.000000 ooui-0.5.0/ooui.egg-info/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        5 2024-05-13 14:33:44.000000 ooui-0.5.0/ooui.egg-info/top_level.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       43 2024-05-13 14:33:44.000000 ooui-0.5.0/ooui.egg-info/requires.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      408 2024-05-13 14:33:44.000000 ooui-0.5.0/ooui.egg-info/SOURCES.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        1 2024-05-13 14:33:44.000000 ooui-0.5.0/ooui.egg-info/dependency_links.txt
--rw-r--r--   0 ecarreras  (1000) ecarreras  (1000)      276 2024-05-13 14:33:44.000000 ooui-0.5.0/ooui.egg-info/PKG-INFO
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 14:33:44.000000 ooui-0.5.0/ooui/
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 14:33:44.000000 ooui-0.5.0/ooui/helpers/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1407 2024-05-13 14:13:20.000000 ooui-0.5.0/ooui/helpers/conditions.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      526 2024-05-06 17:19:46.000000 ooui-0.5.0/ooui/helpers/__init__.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-06 16:22:58.000000 ooui-0.5.0/ooui/__init__.py
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 14:33:44.000000 ooui-0.5.0/ooui/graph/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      783 2024-05-10 12:49:23.000000 ooui-0.5.0/ooui/graph/base.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2900 2024-05-10 12:48:29.000000 ooui-0.5.0/ooui/graph/processor.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     3305 2024-05-10 12:09:54.000000 ooui-0.5.0/ooui/graph/fields.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     9439 2024-05-08 12:28:50.000000 ooui-0.5.0/ooui/graph/timerange.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      779 2024-05-10 12:16:14.000000 ooui-0.5.0/ooui/graph/__init__.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2611 2024-05-13 14:32:17.000000 ooui-0.5.0/ooui/graph/indicator.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2599 2024-05-08 10:59:34.000000 ooui-0.5.0/ooui/graph/axis.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     5632 2024-05-10 12:48:45.000000 ooui-0.5.0/ooui/graph/chart.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       40 2024-05-06 16:18:58.000000 ooui-0.5.0/README.md
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1065 2024-05-06 16:18:58.000000 ooui-0.5.0/LICENSE
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      276 2024-05-13 14:33:44.000000 ooui-0.5.0/PKG-INFO
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:06:54.000000 ooui-0.6.0/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      562 2024-05-13 15:06:21.000000 ooui-0.6.0/setup.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       38 2024-05-13 15:06:54.000000 ooui-0.6.0/setup.cfg
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:06:54.000000 ooui-0.6.0/ooui.egg-info/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        5 2024-05-13 15:06:54.000000 ooui-0.6.0/ooui.egg-info/top_level.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       43 2024-05-13 15:06:54.000000 ooui-0.6.0/ooui.egg-info/requires.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      431 2024-05-13 15:06:54.000000 ooui-0.6.0/ooui.egg-info/SOURCES.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        1 2024-05-13 15:06:54.000000 ooui-0.6.0/ooui.egg-info/dependency_links.txt
+-rw-r--r--   0 ecarreras  (1000) ecarreras  (1000)      276 2024-05-13 15:06:54.000000 ooui-0.6.0/ooui.egg-info/PKG-INFO
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:06:54.000000 ooui-0.6.0/ooui/
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:06:54.000000 ooui-0.6.0/ooui/helpers/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      971 2024-05-13 14:52:41.000000 ooui-0.6.0/ooui/helpers/domain.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1407 2024-05-13 14:13:20.000000 ooui-0.6.0/ooui/helpers/conditions.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      526 2024-05-06 17:19:46.000000 ooui-0.6.0/ooui/helpers/__init__.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-06 16:22:58.000000 ooui-0.6.0/ooui/__init__.py
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:06:54.000000 ooui-0.6.0/ooui/graph/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      783 2024-05-10 12:49:23.000000 ooui-0.6.0/ooui/graph/base.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2996 2024-05-13 15:00:24.000000 ooui-0.6.0/ooui/graph/processor.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     3305 2024-05-10 12:09:54.000000 ooui-0.6.0/ooui/graph/fields.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     9439 2024-05-08 12:28:50.000000 ooui-0.6.0/ooui/graph/timerange.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      779 2024-05-10 12:16:14.000000 ooui-0.6.0/ooui/graph/__init__.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2728 2024-05-13 15:02:17.000000 ooui-0.6.0/ooui/graph/indicator.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2599 2024-05-08 10:59:34.000000 ooui-0.6.0/ooui/graph/axis.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     5632 2024-05-10 12:48:45.000000 ooui-0.6.0/ooui/graph/chart.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       40 2024-05-06 16:18:58.000000 ooui-0.6.0/README.md
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1065 2024-05-06 16:18:58.000000 ooui-0.6.0/LICENSE
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      276 2024-05-13 15:06:54.000000 ooui-0.6.0/PKG-INFO
```

### Comparing `ooui-0.5.0/setup.py` & `ooui-0.6.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 setup(
     name='ooui',
     description='Open Object User Interface',
     author='GISCE',
     author_email='devel@gisce.net',
     url='https://github.com/gisce/python-ooui',
-    version='0.5.0',
+    version='0.6.0',
     license='MIT',
     long_description='''Open Object User Interface for GISCE-ERP''',
     provides=['ooui'],
     install_requires=[
         'lxml',
         'python-dateutil',
         'six',
```

### Comparing `ooui-0.5.0/ooui/helpers/conditions.py` & `ooui-0.6.0/ooui/helpers/conditions.py`

 * *Files identical despite different names*

### Comparing `ooui-0.5.0/ooui/helpers/__init__.py` & `ooui-0.6.0/ooui/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ooui-0.5.0/ooui/graph/base.py` & `ooui-0.6.0/ooui/graph/base.py`

 * *Files identical despite different names*

### Comparing `ooui-0.5.0/ooui/graph/processor.py` & `ooui-0.6.0/ooui/graph/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,18 @@
     :param dict fields: A dictionary of field definitions.
     :param dict options: Optional additional options for processing graph data.
 
     :rtype: dict
     :returns: A dictionary containing the final processed data and flags like
         isGroup and isStack.
     """
-    return ooui.process(values, fields, options=options)
+    if ooui.type == "indicatorField":
+        return ooui.process(values, fields)
+    else:
+        return ooui.process(values, fields, options=options)
 
 
 def get_values_for_y_field(entries, field_name, fields):
     """
     Retrieve labels for a specified field across multiple entries.
 
     :param list entries: A list of dictionaries representing the entries.
```

### Comparing `ooui-0.5.0/ooui/graph/fields.py` & `ooui-0.6.0/ooui/graph/fields.py`

 * *Files identical despite different names*

### Comparing `ooui-0.5.0/ooui/graph/timerange.py` & `ooui-0.6.0/ooui/graph/timerange.py`

 * *Files identical despite different names*

### Comparing `ooui-0.5.0/ooui/graph/__init__.py` & `ooui-0.6.0/ooui/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `ooui-0.5.0/ooui/graph/indicator.py` & `ooui-0.6.0/ooui/graph/indicator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 from __future__ import division
 from ooui.graph.base import Graph
 from ooui.helpers import parse_bool_attribute, replace_entities
 from ooui.helpers.conditions import ConditionParser
+from ooui.helpers.domain import Domain
 from ooui.graph.fields import get_value_for_operator, round_number
 
 
 class GraphIndicator(Graph):
     def __init__(self, graph_type, element):
         # Inicia la classe base Graph
         super(GraphIndicator, self).__init__(element)
 
         self._type = graph_type
         self._color = ConditionParser(replace_entities(element.get('color'))) if element.get(
             'color') else None
         self._icon = ConditionParser(replace_entities(element.get('icon'))) if element.get(
             'icon') else None
         self._suffix = element.get('suffix') if element.get('suffix') else None
-        self._total_domain = replace_entities(
-            element.get('totalDomain')) if element.get('totalDomain') else None
+        self._total_domain = Domain(replace_entities(
+            element.get('totalDomain')) if element.get('totalDomain') else None)
         self._show_percent = parse_bool_attribute(
             element.get('showPercent')) if element.get('showPercent') else False
+        self.domain_parse_values = {}
 
     @property
     def color(self):
         return self._color
 
     @property
     def icon(self):
         return self._icon
 
     @property
     def total_domain(self):
-        return self._total_domain
+        return self._total_domain.parse(self.domain_parse_values)
 
     @property
     def show_percent(self):
         return self._show_percent
 
     @property
     def suffix(self):
```

### Comparing `ooui-0.5.0/ooui/graph/axis.py` & `ooui-0.6.0/ooui/graph/axis.py`

 * *Files identical despite different names*

### Comparing `ooui-0.5.0/ooui/graph/chart.py` & `ooui-0.6.0/ooui/graph/chart.py`

 * *Files identical despite different names*

### Comparing `ooui-0.5.0/LICENSE` & `ooui-0.6.0/LICENSE`

 * *Files identical despite different names*

