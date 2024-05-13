# Comparing `tmp/adb_tool_py-0.0.1.tar.gz` & `tmp/adb_tool_py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adb_tool_py-0.0.1.tar", last modified: Sun May 12 13:54:41 2024, max compression
+gzip compressed data, was "adb_tool_py-0.0.2.tar", last modified: Mon May 13 12:22:31 2024, max compression
```

## Comparing `adb_tool_py-0.0.1.tar` & `adb_tool_py-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-12 13:54:41.550840 adb_tool_py-0.0.1/
--rw-r--r--   0 iuchi      (501) staff       (20)     1059 2024-05-12 12:33:16.000000 adb_tool_py-0.0.1/LICENSE
--rw-r--r--   0 iuchi      (501) staff       (20)       34 2024-05-12 13:08:55.000000 adb_tool_py-0.0.1/MANIFEST.in
--rw-r--r--   0 iuchi      (501) staff       (20)      292 2024-05-12 13:54:41.550715 adb_tool_py-0.0.1/PKG-INFO
--rw-r--r--   0 iuchi      (501) staff       (20)       14 2024-05-12 13:37:06.000000 adb_tool_py-0.0.1/README.md
-drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-12 13:54:41.549819 adb_tool_py-0.0.1/adb_tool_py/
--rw-r--r--   0 iuchi      (501) staff       (20)        0 2024-05-12 12:33:36.000000 adb_tool_py-0.0.1/adb_tool_py/__init__.py
--rw-r--r--   0 iuchi      (501) staff       (20)     1820 2024-05-12 13:37:06.000000 adb_tool_py-0.0.1/adb_tool_py/adb_command.py
--rw-r--r--   0 iuchi      (501) staff       (20)       84 2024-05-12 12:33:36.000000 adb_tool_py-0.0.1/adb_tool_py/adb_device.py
--rw-r--r--   0 iuchi      (501) staff       (20)     2605 2024-05-12 13:46:35.000000 adb_tool_py-0.0.1/adb_tool_py/adb_tool.py
--rw-r--r--   0 iuchi      (501) staff       (20)     4360 2024-05-12 13:37:06.000000 adb_tool_py-0.0.1/adb_tool_py/adb_view_tree.py
--rw-r--r--   0 iuchi      (501) staff       (20)      468 2024-05-12 12:33:36.000000 adb_tool_py-0.0.1/adb_tool_py/command.py
--rw-r--r--   0 iuchi      (501) staff       (20)     2436 2024-05-12 12:33:36.000000 adb_tool_py-0.0.1/adb_tool_py/ui_node.py
-drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-12 13:54:41.550546 adb_tool_py-0.0.1/adb_tool_py.egg-info/
--rw-r--r--   0 iuchi      (501) staff       (20)      292 2024-05-12 13:54:41.000000 adb_tool_py-0.0.1/adb_tool_py.egg-info/PKG-INFO
--rw-r--r--   0 iuchi      (501) staff       (20)      388 2024-05-12 13:54:41.000000 adb_tool_py-0.0.1/adb_tool_py.egg-info/SOURCES.txt
--rw-r--r--   0 iuchi      (501) staff       (20)        1 2024-05-12 13:54:41.000000 adb_tool_py-0.0.1/adb_tool_py.egg-info/dependency_links.txt
--rw-r--r--   0 iuchi      (501) staff       (20)        8 2024-05-12 13:54:41.000000 adb_tool_py-0.0.1/adb_tool_py.egg-info/requires.txt
--rw-r--r--   0 iuchi      (501) staff       (20)       12 2024-05-12 13:54:41.000000 adb_tool_py-0.0.1/adb_tool_py.egg-info/top_level.txt
--rw-r--r--   0 iuchi      (501) staff       (20)       38 2024-05-12 13:54:41.550885 adb_tool_py-0.0.1/setup.cfg
--rw-r--r--   0 iuchi      (501) staff       (20)      457 2024-05-12 13:54:15.000000 adb_tool_py-0.0.1/setup.py
+drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-13 12:22:31.054522 adb_tool_py-0.0.2/
+-rw-r--r--   0 iuchi      (501) staff       (20)     1059 2024-05-12 12:33:16.000000 adb_tool_py-0.0.2/LICENSE
+-rw-r--r--   0 iuchi      (501) staff       (20)       34 2024-05-12 13:08:55.000000 adb_tool_py-0.0.2/MANIFEST.in
+-rw-r--r--   0 iuchi      (501) staff       (20)      446 2024-05-13 12:22:31.054397 adb_tool_py-0.0.2/PKG-INFO
+-rw-r--r--   0 iuchi      (501) staff       (20)       14 2024-05-12 13:37:06.000000 adb_tool_py-0.0.2/README.md
+drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-13 12:22:31.053732 adb_tool_py-0.0.2/adb_tool_py/
+-rw-r--r--   0 iuchi      (501) staff       (20)        0 2024-05-12 12:33:36.000000 adb_tool_py-0.0.2/adb_tool_py/__init__.py
+-rw-r--r--   0 iuchi      (501) staff       (20)     1820 2024-05-12 13:37:06.000000 adb_tool_py-0.0.2/adb_tool_py/adb_command.py
+-rw-r--r--   0 iuchi      (501) staff       (20)       84 2024-05-12 12:33:36.000000 adb_tool_py-0.0.2/adb_tool_py/adb_device.py
+-rw-r--r--   0 iuchi      (501) staff       (20)     2605 2024-05-12 13:46:35.000000 adb_tool_py-0.0.2/adb_tool_py/adb_tool.py
+-rw-r--r--   0 iuchi      (501) staff       (20)     4360 2024-05-12 13:37:06.000000 adb_tool_py-0.0.2/adb_tool_py/adb_view_tree.py
+-rw-r--r--   0 iuchi      (501) staff       (20)      468 2024-05-12 12:33:36.000000 adb_tool_py-0.0.2/adb_tool_py/command.py
+-rw-r--r--   0 iuchi      (501) staff       (20)     2436 2024-05-12 12:33:36.000000 adb_tool_py-0.0.2/adb_tool_py/ui_node.py
+drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-13 12:22:31.054249 adb_tool_py-0.0.2/adb_tool_py.egg-info/
+-rw-r--r--   0 iuchi      (501) staff       (20)      446 2024-05-13 12:22:31.000000 adb_tool_py-0.0.2/adb_tool_py.egg-info/PKG-INFO
+-rw-r--r--   0 iuchi      (501) staff       (20)      388 2024-05-13 12:22:31.000000 adb_tool_py-0.0.2/adb_tool_py.egg-info/SOURCES.txt
+-rw-r--r--   0 iuchi      (501) staff       (20)        1 2024-05-13 12:22:31.000000 adb_tool_py-0.0.2/adb_tool_py.egg-info/dependency_links.txt
+-rw-r--r--   0 iuchi      (501) staff       (20)        8 2024-05-13 12:22:31.000000 adb_tool_py-0.0.2/adb_tool_py.egg-info/requires.txt
+-rw-r--r--   0 iuchi      (501) staff       (20)       12 2024-05-13 12:22:31.000000 adb_tool_py-0.0.2/adb_tool_py.egg-info/top_level.txt
+-rw-r--r--   0 iuchi      (501) staff       (20)       38 2024-05-13 12:22:31.054562 adb_tool_py-0.0.2/setup.cfg
+-rw-r--r--   0 iuchi      (501) staff       (20)      756 2024-05-13 12:20:55.000000 adb_tool_py-0.0.2/setup.py
```

### Comparing `adb_tool_py-0.0.1/LICENSE` & `adb_tool_py-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adb_tool_py-0.0.1/adb_tool_py/adb_command.py` & `adb_tool_py-0.0.2/adb_tool_py/adb_command.py`

 * *Files identical despite different names*

### Comparing `adb_tool_py-0.0.1/adb_tool_py/adb_tool.py` & `adb_tool_py-0.0.2/adb_tool_py/adb_tool.py`

 * *Files identical despite different names*

### Comparing `adb_tool_py-0.0.1/adb_tool_py/adb_view_tree.py` & `adb_tool_py-0.0.2/adb_tool_py/adb_view_tree.py`

 * *Files identical despite different names*

### Comparing `adb_tool_py-0.0.1/adb_tool_py/ui_node.py` & `adb_tool_py-0.0.2/adb_tool_py/ui_node.py`

 * *Files identical despite different names*

