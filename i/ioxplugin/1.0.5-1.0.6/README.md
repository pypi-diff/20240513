# Comparing `tmp/ioxplugin-1.0.5.tar.gz` & `tmp/ioxplugin-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ioxplugin-1.0.5.tar", last modified: Mon May 13 07:05:12 2024, max compression
+gzip compressed data, was "ioxplugin-1.0.6.tar", last modified: Mon May 13 08:17:21 2024, max compression
```

## Comparing `ioxplugin-1.0.5.tar` & `ioxplugin-1.0.6.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:05:12.886504 ioxplugin-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-13 07:05:12.886504 ioxplugin-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:05:12.882504 ioxplugin-1.0.5/ioxplugin/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    56393 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/ast_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/iox_controller_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/iox_node_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)    11192 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/iox_node_impl_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/iox_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/iox_to_modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/iox_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/main_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/new_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/node_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/nodedef.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3014 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/oauth_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/plugin_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/uom.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:05:12.886504 ioxplugin-1.0.5/ioxplugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-13 07:05:12.000000 ioxplugin-1.0.5/ioxplugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-13 07:05:12.000000 ioxplugin-1.0.5/ioxplugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 07:05:12.000000 ioxplugin-1.0.5/ioxplugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-13 07:05:12.000000 ioxplugin-1.0.5/ioxplugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 07:05:12.000000 ioxplugin-1.0.5/ioxplugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 07:05:12.886504 ioxplugin-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:05:12.886504 ioxplugin-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/tests/test_ioxplugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:17:21.195151 ioxplugin-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-13 08:17:21.195151 ioxplugin-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:17:21.195151 ioxplugin-1.0.6/ioxplugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56393 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/ast_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/iox_controller_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/iox_main_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/iox_node_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11192 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/iox_node_impl_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/iox_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/iox_to_modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/iox_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/main_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/new_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/node_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/nodedef.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3014 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/oauth_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/plugin_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/uom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:17:21.195151 ioxplugin-1.0.6/ioxplugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-13 08:17:21.000000 ioxplugin-1.0.6/ioxplugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-13 08:17:21.000000 ioxplugin-1.0.6/ioxplugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:17:21.000000 ioxplugin-1.0.6/ioxplugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-13 08:17:21.000000 ioxplugin-1.0.6/ioxplugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 08:17:21.000000 ioxplugin-1.0.6/ioxplugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 08:17:21.195151 ioxplugin-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:17:21.195151 ioxplugin-1.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/tests/test_ioxplugin.py
```

### Comparing `ioxplugin-1.0.5/PKG-INFO` & `ioxplugin-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ioxplugin
-Version: 1.0.5
+Version: 1.0.6
 Summary: IoX Plugin Helper Package
 Home-page: https://github.com/universaldevices/ioxplugin.git
 Author: Michel Kohanim
 Author-email: support@universal-devices.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ioxplugin-1.0.5/ioxplugin/__init__.py` & `ioxplugin-1.0.6/ioxplugin/__init__.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.5/ioxplugin/ast_util.py` & `ioxplugin-1.0.6/ioxplugin/ast_util.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.5/ioxplugin/commands.py` & `ioxplugin-1.0.6/ioxplugin/commands.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.5/ioxplugin/editor.py` & `ioxplugin-1.0.6/ioxplugin/editor.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.5/ioxplugin/iox_controller_template.py` & `ioxplugin-1.0.6/ioxplugin/iox_controller_template.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.5/ioxplugin/iox_node_gen.py` & `ioxplugin-1.0.6/ioxplugin/iox_node_gen.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.5/ioxplugin/iox_node_impl_gen.py` & `ioxplugin-1.0.6/ioxplugin/iox_node_impl_gen.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.5/ioxplugin/iox_profile.py` & `ioxplugin-1.0.6/ioxplugin/iox_profile.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.5/ioxplugin/iox_to_modbus.py` & `ioxplugin-1.0.6/ioxplugin/iox_to_modbus.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.5/ioxplugin/iox_transport.py` & `ioxplugin-1.0.6/ioxplugin/iox_transport.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.5/ioxplugin/log.py` & `ioxplugin-1.0.6/ioxplugin/log.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.5/ioxplugin/new_project.py` & `ioxplugin-1.0.6/ioxplugin/new_project.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.5/ioxplugin/node_properties.py` & `ioxplugin-1.0.6/ioxplugin/node_properties.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.5/ioxplugin/nodedef.py` & `ioxplugin-1.0.6/ioxplugin/nodedef.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.5/ioxplugin/oauth_service.py` & `ioxplugin-1.0.6/ioxplugin/oauth_service.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.5/ioxplugin/plugin.py` & `ioxplugin-1.0.6/ioxplugin/plugin.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.5/ioxplugin/plugin_meta.py` & `ioxplugin-1.0.6/ioxplugin/plugin_meta.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.5/ioxplugin/properties.py` & `ioxplugin-1.0.6/ioxplugin/properties.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.5/ioxplugin/protocol.py` & `ioxplugin-1.0.6/ioxplugin/protocol.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.5/ioxplugin/uom.py` & `ioxplugin-1.0.6/ioxplugin/uom.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.5/ioxplugin/validator.py` & `ioxplugin-1.0.6/ioxplugin/validator.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.5/ioxplugin.egg-info/PKG-INFO` & `ioxplugin-1.0.6/ioxplugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ioxplugin
-Version: 1.0.5
+Version: 1.0.6
 Summary: IoX Plugin Helper Package
 Home-page: https://github.com/universaldevices/ioxplugin.git
 Author: Michel Kohanim
 Author-email: support@universal-devices.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ioxplugin-1.0.5/ioxplugin.egg-info/SOURCES.txt` & `ioxplugin-1.0.6/ioxplugin.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.py
 ioxplugin/__init__.py
 ioxplugin/ast_util.py
 ioxplugin/commands.py
 ioxplugin/editor.py
 ioxplugin/iox_controller_template.py
+ioxplugin/iox_main_template.py
 ioxplugin/iox_node_gen.py
 ioxplugin/iox_node_impl_gen.py
 ioxplugin/iox_profile.py
 ioxplugin/iox_to_modbus.py
 ioxplugin/iox_transport.py
 ioxplugin/log.py
 ioxplugin/main_gen.py
```

### Comparing `ioxplugin-1.0.5/setup.py` & `ioxplugin-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ioxplugin',
-    version='1.0.5',
+    version='1.0.6',
     packages=find_packages(),
     description='IoX Plugin Helper Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Michel Kohanim',
     author_email='support@universal-devices.com',
     url='https://github.com/universaldevices/ioxplugin.git',
```

