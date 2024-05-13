# Comparing `tmp/easyland-0.7.2.tar.gz` & `tmp/easyland-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyland-0.7.2.tar", last modified: Fri May  3 09:08:32 2024, max compression
+gzip compressed data, was "easyland-0.7.4.tar", last modified: Mon May 13 09:05:51 2024, max compression
```

## Comparing `easyland-0.7.2.tar` & `easyland-0.7.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-03 09:08:32.276980 easyland-0.7.2/
--rw-r--r--   0 ju        (1000) ju        (1000)     1066 2024-04-25 19:16:43.000000 easyland-0.7.2/LICENSE.txt
--rw-r--r--   0 ju        (1000) ju        (1000)    14346 2024-05-03 09:08:32.276980 easyland-0.7.2/PKG-INFO
--rw-r--r--   0 ju        (1000) ju        (1000)    13475 2024-05-03 08:13:49.000000 easyland-0.7.2/README.md
--rw-r--r--   0 ju        (1000) ju        (1000)      968 2024-05-02 15:06:34.000000 easyland-0.7.2/pyproject.toml
--rw-r--r--   0 ju        (1000) ju        (1000)       38 2024-05-03 09:08:32.276980 easyland-0.7.2/setup.cfg
-drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-03 09:08:32.273646 easyland-0.7.2/src/
-drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-03 09:08:32.276980 easyland-0.7.2/src/easyland/
--rw-r--r--   0 ju        (1000) ju        (1000)      142 2024-05-01 07:14:10.000000 easyland-0.7.2/src/easyland/__init__.py
--rw-r--r--   0 ju        (1000) ju        (1000)     2405 2024-05-01 17:31:04.000000 easyland-0.7.2/src/easyland/command.py
--rw-r--r--   0 ju        (1000) ju        (1000)     4904 2024-05-03 07:32:12.000000 easyland-0.7.2/src/easyland/daemon.py
--rw-r--r--   0 ju        (1000) ju        (1000)     2229 2024-05-01 20:26:14.000000 easyland-0.7.2/src/easyland/idle.py
--rw-r--r--   0 ju        (1000) ju        (1000)      236 2024-05-01 11:08:03.000000 easyland-0.7.2/src/easyland/log.py
--rwxr-xr-x   0 ju        (1000) ju        (1000)     1245 2024-05-02 15:06:52.000000 easyland-0.7.2/src/easyland/main.py
-drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-03 09:08:32.276980 easyland-0.7.2/src/easyland.egg-info/
--rw-r--r--   0 ju        (1000) ju        (1000)    14346 2024-05-03 09:08:32.000000 easyland-0.7.2/src/easyland.egg-info/PKG-INFO
--rw-r--r--   0 ju        (1000) ju        (1000)      388 2024-05-03 09:08:32.000000 easyland-0.7.2/src/easyland.egg-info/SOURCES.txt
--rw-r--r--   0 ju        (1000) ju        (1000)        1 2024-05-03 09:08:32.000000 easyland-0.7.2/src/easyland.egg-info/dependency_links.txt
--rw-r--r--   0 ju        (1000) ju        (1000)       48 2024-05-03 09:08:32.000000 easyland-0.7.2/src/easyland.egg-info/entry_points.txt
--rw-r--r--   0 ju        (1000) ju        (1000)       18 2024-05-03 09:08:32.000000 easyland-0.7.2/src/easyland.egg-info/requires.txt
--rw-r--r--   0 ju        (1000) ju        (1000)        9 2024-05-03 09:08:32.000000 easyland-0.7.2/src/easyland.egg-info/top_level.txt
+drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-13 09:05:51.120082 easyland-0.7.4/
+-rw-r--r--   0 ju        (1000) ju        (1000)     1066 2024-04-25 19:16:43.000000 easyland-0.7.4/LICENSE.txt
+-rw-r--r--   0 ju        (1000) ju        (1000)    14346 2024-05-13 09:05:51.120082 easyland-0.7.4/PKG-INFO
+-rw-r--r--   0 ju        (1000) ju        (1000)    13475 2024-05-03 08:13:49.000000 easyland-0.7.4/README.md
+-rw-r--r--   0 ju        (1000) ju        (1000)      968 2024-05-13 09:01:43.000000 easyland-0.7.4/pyproject.toml
+-rw-r--r--   0 ju        (1000) ju        (1000)       38 2024-05-13 09:05:51.120082 easyland-0.7.4/setup.cfg
+drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-13 09:05:51.120082 easyland-0.7.4/src/
+drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-13 09:05:51.120082 easyland-0.7.4/src/easyland/
+-rw-r--r--   0 ju        (1000) ju        (1000)      142 2024-05-01 07:14:10.000000 easyland-0.7.4/src/easyland/__init__.py
+-rw-r--r--   0 ju        (1000) ju        (1000)     2405 2024-05-01 17:31:04.000000 easyland-0.7.4/src/easyland/command.py
+-rw-r--r--   0 ju        (1000) ju        (1000)     4904 2024-05-03 07:32:12.000000 easyland-0.7.4/src/easyland/daemon.py
+-rw-r--r--   0 ju        (1000) ju        (1000)     2440 2024-05-13 09:00:58.000000 easyland-0.7.4/src/easyland/idle.py
+-rw-r--r--   0 ju        (1000) ju        (1000)      236 2024-05-01 11:08:03.000000 easyland-0.7.4/src/easyland/log.py
+-rwxr-xr-x   0 ju        (1000) ju        (1000)     1245 2024-05-13 09:02:01.000000 easyland-0.7.4/src/easyland/main.py
+drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-13 09:05:51.120082 easyland-0.7.4/src/easyland.egg-info/
+-rw-r--r--   0 ju        (1000) ju        (1000)    14346 2024-05-13 09:05:51.000000 easyland-0.7.4/src/easyland.egg-info/PKG-INFO
+-rw-r--r--   0 ju        (1000) ju        (1000)      388 2024-05-13 09:05:51.000000 easyland-0.7.4/src/easyland.egg-info/SOURCES.txt
+-rw-r--r--   0 ju        (1000) ju        (1000)        1 2024-05-13 09:05:51.000000 easyland-0.7.4/src/easyland.egg-info/dependency_links.txt
+-rw-r--r--   0 ju        (1000) ju        (1000)       48 2024-05-13 09:05:51.000000 easyland-0.7.4/src/easyland.egg-info/entry_points.txt
+-rw-r--r--   0 ju        (1000) ju        (1000)       18 2024-05-13 09:05:51.000000 easyland-0.7.4/src/easyland.egg-info/requires.txt
+-rw-r--r--   0 ju        (1000) ju        (1000)        9 2024-05-13 09:05:51.000000 easyland-0.7.4/src/easyland.egg-info/top_level.txt
```

### Comparing `easyland-0.7.2/LICENSE.txt` & `easyland-0.7.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easyland-0.7.2/PKG-INFO` & `easyland-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyland
-Version: 0.7.2
+Version: 0.7.4
 Summary: A python swiss-knife to manage wayand compositors like Hyprland and Sway
 Author-email: Julien Pro <contact@julienpro.com>
 Project-URL: Homepage, https://github.com/juienpro/easyland
 Project-URL: Issues, https://github.com/juienpro/easyland/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easyland-0.7.2/README.md` & `easyland-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `easyland-0.7.2/pyproject.toml` & `easyland-0.7.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "easyland"
-version = "0.7.2"
+version = "0.7.4"
 authors = [
     { name="Julien Pro", email="contact@julienpro.com"}
 ]
 description = "A python swiss-knife to manage wayand compositors like Hyprland and Sway"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
```

### Comparing `easyland-0.7.2/src/easyland/command.py` & `easyland-0.7.4/src/easyland/command.py`

 * *Files identical despite different names*

### Comparing `easyland-0.7.2/src/easyland/daemon.py` & `easyland-0.7.4/src/easyland/daemon.py`

 * *Files identical despite different names*

### Comparing `easyland-0.7.2/src/easyland/idle.py` & `easyland-0.7.4/src/easyland/idle.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,21 +18,25 @@
         self._config = config
         self._display =  Display()
         self._display.connect()
         self._idle_notifier = None
         self._seat = None
         self._notifications = []
 
+    # def _global_handler_init(self, reg, id_num, iface_name, version):
+    #     if iface_name == 'wl_seat':
+    #         self._seat = reg.bind(id_num, WlSeat, version)
+
     def _global_handler(self, reg, id_num, iface_name, version):
         if iface_name == 'wl_seat':
             self._seat = reg.bind(id_num, WlSeat, version)
-
-        elif iface_name == "ext_idle_notifier_v1":
+        if iface_name == "ext_idle_notifier_v1":
             self._idle_notifier = reg.bind(id_num, ExtIdleNotifierV1, version)
-    
+
+        if self._idle_notifier and self._seat:
             for idx, c in enumerate(self._config):
                 self._notifications.append(None)
                 self._notifications[idx] = self._idle_notifier.get_idle_notification(c[0] * 1000, self._seat)
                 self._notifications[idx]._index = idx
                 self._notifications[idx].dispatcher['idled'] = self._idle_notifier_handler
                 self._notifications[idx].dispatcher['resumed'] = self._idle_notifier_resume_handler
 
@@ -51,8 +55,7 @@
 
     def setup(self):
         reg = self._display.get_registry()
         reg.dispatcher['global'] = self._global_handler
         while True:
             self._display.dispatch(block=True)
 
-
```

### Comparing `easyland-0.7.2/src/easyland/main.py` & `easyland-0.7.4/src/easyland/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import importlib.util
 import importlib.machinery
 import sys
 import time
 import os
 from easyland.daemon import Daemon
 
-version = '0.7.2'
+version = '0.7.4'
 
 def import_from_path(path):
     module_name = os.path.basename(path).replace('-', '_').replace('.py', '')
     spec = importlib.util.spec_from_loader(module_name, importlib.machinery.SourceFileLoader(module_name, path))
     module = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(module)
     sys.modules[module_name] = module
```

### Comparing `easyland-0.7.2/src/easyland.egg-info/PKG-INFO` & `easyland-0.7.4/src/easyland.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyland
-Version: 0.7.2
+Version: 0.7.4
 Summary: A python swiss-knife to manage wayand compositors like Hyprland and Sway
 Author-email: Julien Pro <contact@julienpro.com>
 Project-URL: Homepage, https://github.com/juienpro/easyland
 Project-URL: Issues, https://github.com/juienpro/easyland/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

