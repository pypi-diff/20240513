# Comparing `tmp/pywlroots-0.2.8.tar.gz` & `tmp/pywlroots-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pywlroots-0.2.8.tar", last modified: Sat May  8 21:41:15 2021, max compression
+gzip compressed data, was "dist/pywlroots-0.2.9.tar", last modified: Sat May 15 12:20:06 2021, max compression
```

## Comparing `pywlroots-0.2.8.tar` & `pywlroots-0.2.9.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-08 21:41:15.871594 pywlroots-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2021-05-08 21:41:10.000000 pywlroots-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-05-08 21:41:10.000000 pywlroots-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2021-05-08 21:41:15.871594 pywlroots-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-05-08 21:41:10.000000 pywlroots-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-08 21:41:15.867593 pywlroots-0.2.8/include/
--rw-r--r--   0 runner    (1001) docker     (121)    19834 2021-05-08 21:41:10.000000 pywlroots-0.2.8/include/wlr-layer-shell-unstable-v1-protocol.h
--rw-r--r--   0 runner    (1001) docker     (121)    57885 2021-05-08 21:41:10.000000 pywlroots-0.2.8/include/xdg-shell-protocol.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-08 21:41:15.867593 pywlroots-0.2.8/pywlroots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2021-05-08 21:41:15.000000 pywlroots-0.2.8/pywlroots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1298 2021-05-08 21:41:15.000000 pywlroots-0.2.8/pywlroots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-08 21:41:15.000000 pywlroots-0.2.8/pywlroots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-08 21:41:15.000000 pywlroots-0.2.8/pywlroots.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       99 2021-05-08 21:41:15.000000 pywlroots-0.2.8/pywlroots.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-05-08 21:41:15.000000 pywlroots-0.2.8/pywlroots.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1663 2021-05-08 21:41:15.871594 pywlroots-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      126 2021-05-08 21:41:10.000000 pywlroots-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-08 21:41:15.867593 pywlroots-0.2.8/wlroots/
--rw-r--r--   0 runner    (1001) docker     (121)      830 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3810 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/backend.py
--rw-r--r--   0 runner    (1001) docker     (121)    42231 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/ffi_build.py
--rw-r--r--   0 runner    (1001) docker     (121)      842 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     3130 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-08 21:41:15.867593 pywlroots-0.2.8/wlroots/util/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/util/clock.py
--rw-r--r--   0 runner    (1001) docker     (121)      259 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/util/edges.py
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/util/log.py
--rw-r--r--   0 runner    (1001) docker     (121)     1650 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/util/region.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-08 21:41:15.871594 pywlroots-0.2.8/wlroots/wlr_types/
--rw-r--r--   0 runner    (1001) docker     (121)     1272 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/wlr_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      823 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/wlr_types/box.py
--rw-r--r--   0 runner    (1001) docker     (121)      638 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/wlr_types/compositor.py
--rw-r--r--   0 runner    (1001) docker     (121)     8006 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/wlr_types/cursor.py
--rw-r--r--   0 runner    (1001) docker     (121)      386 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/wlr_types/data_device_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)      411 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/wlr_types/gamma_control_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1594 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/wlr_types/input_device.py
--rw-r--r--   0 runner    (1001) docker     (121)     4472 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/wlr_types/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (121)     6042 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/wlr_types/layer_shell_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     2705 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/wlr_types/matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     7975 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/wlr_types/output.py
--rw-r--r--   0 runner    (1001) docker     (121)     2775 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/wlr_types/output_damage.py
--rw-r--r--   0 runner    (1001) docker     (121)     2475 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/wlr_types/output_layout.py
--rw-r--r--   0 runner    (1001) docker     (121)     4592 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/wlr_types/pointer.py
--rw-r--r--   0 runner    (1001) docker     (121)      404 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/wlr_types/screencopy_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)    13154 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/wlr_types/seat.py
--rw-r--r--   0 runner    (1001) docker     (121)     3219 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/wlr_types/surface.py
--rw-r--r--   0 runner    (1001) docker     (121)      868 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/wlr_types/texture.py
--rw-r--r--   0 runner    (1001) docker     (121)     1339 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/wlr_types/virtual_keyboard_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1355 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/wlr_types/xcursor_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     2850 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/wlr_types/xdg_decoration_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)      481 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/wlr_types/xdg_output_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     9650 2021-05-08 21:41:10.000000 pywlroots-0.2.8/wlroots/wlr_types/xdg_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-15 12:20:06.032292 pywlroots-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1486 2021-05-15 12:20:00.000000 pywlroots-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2021-05-15 12:20:00.000000 pywlroots-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2021-05-15 12:20:06.032292 pywlroots-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2021-05-15 12:20:00.000000 pywlroots-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-15 12:20:06.024292 pywlroots-0.2.9/include/
+-rw-r--r--   0 runner    (1001) docker     (121)    19834 2021-05-15 12:20:00.000000 pywlroots-0.2.9/include/wlr-layer-shell-unstable-v1-protocol.h
+-rw-r--r--   0 runner    (1001) docker     (121)    57885 2021-05-15 12:20:00.000000 pywlroots-0.2.9/include/xdg-shell-protocol.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-15 12:20:06.024292 pywlroots-0.2.9/pywlroots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2021-05-15 12:20:05.000000 pywlroots-0.2.9/pywlroots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1340 2021-05-15 12:20:06.000000 pywlroots-0.2.9/pywlroots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-15 12:20:05.000000 pywlroots-0.2.9/pywlroots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-15 12:20:05.000000 pywlroots-0.2.9/pywlroots.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2021-05-15 12:20:05.000000 pywlroots-0.2.9/pywlroots.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2021-05-15 12:20:05.000000 pywlroots-0.2.9/pywlroots.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1663 2021-05-15 12:20:06.032292 pywlroots-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2021-05-15 12:20:00.000000 pywlroots-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-15 12:20:06.028292 pywlroots-0.2.9/wlroots/
+-rw-r--r--   0 runner    (1001) docker     (121)     1257 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3810 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46816 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/ffi_build.py
+-rw-r--r--   0 runner    (1001) docker     (121)      842 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     3130 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-15 12:20:06.028292 pywlroots-0.2.9/wlroots/util/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1030 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/util/clock.py
+-rw-r--r--   0 runner    (1001) docker     (121)      259 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/util/edges.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1109 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/util/log.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1763 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/util/region.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-15 12:20:06.032292 pywlroots-0.2.9/wlroots/wlr_types/
+-rw-r--r--   0 runner    (1001) docker     (121)     1272 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/wlr_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1220 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/wlr_types/box.py
+-rw-r--r--   0 runner    (1001) docker     (121)      638 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/wlr_types/compositor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8020 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/wlr_types/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      386 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/wlr_types/data_device_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)      425 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/wlr_types/gamma_control_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1608 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/wlr_types/input_device.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4491 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/wlr_types/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6068 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/wlr_types/layer_shell_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2705 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/wlr_types/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9345 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/wlr_types/output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2917 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/wlr_types/output_damage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4431 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/wlr_types/output_layout.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5312 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/wlr_types/output_management_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4592 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/wlr_types/pointer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      418 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/wlr_types/screencopy_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13173 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/wlr_types/seat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3238 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/wlr_types/surface.py
+-rw-r--r--   0 runner    (1001) docker     (121)      868 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/wlr_types/texture.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1339 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/wlr_types/virtual_keyboard_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1355 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/wlr_types/xcursor_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2894 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/wlr_types/xdg_decoration_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)      481 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/wlr_types/xdg_output_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10517 2021-05-15 12:20:00.000000 pywlroots-0.2.9/wlroots/wlr_types/xdg_shell.py
```

### Comparing `pywlroots-0.2.8/LICENSE` & `pywlroots-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pywlroots-0.2.8/PKG-INFO` & `pywlroots-0.2.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywlroots
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python binding to the wlroots library using cffi
 Home-page: https://github.com/flacjacket/pywlroots
 Author: Sean Vig
 Author-email: sean.v.775@gmail.com
 License: MIT
 Project-URL: Code, https://github.com/flacjacket/pywlroots/
 Project-URL: Issue tracker, https://github.com/flacjacket/pywlroots/issues
```

### Comparing `pywlroots-0.2.8/include/wlr-layer-shell-unstable-v1-protocol.h` & `pywlroots-0.2.9/include/wlr-layer-shell-unstable-v1-protocol.h`

 * *Files identical despite different names*

### Comparing `pywlroots-0.2.8/include/xdg-shell-protocol.h` & `pywlroots-0.2.9/include/xdg-shell-protocol.h`

 * *Files identical despite different names*

### Comparing `pywlroots-0.2.8/pywlroots.egg-info/PKG-INFO` & `pywlroots-0.2.9/pywlroots.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywlroots
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python binding to the wlroots library using cffi
 Home-page: https://github.com/flacjacket/pywlroots
 Author: Sean Vig
 Author-email: sean.v.775@gmail.com
 License: MIT
 Project-URL: Code, https://github.com/flacjacket/pywlroots/
 Project-URL: Issue tracker, https://github.com/flacjacket/pywlroots/issues
```

### Comparing `pywlroots-0.2.8/pywlroots.egg-info/SOURCES.txt` & `pywlroots-0.2.9/pywlroots.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 wlroots/wlr_types/input_device.py
 wlroots/wlr_types/keyboard.py
 wlroots/wlr_types/layer_shell_v1.py
 wlroots/wlr_types/matrix.py
 wlroots/wlr_types/output.py
 wlroots/wlr_types/output_damage.py
 wlroots/wlr_types/output_layout.py
+wlroots/wlr_types/output_management_v1.py
 wlroots/wlr_types/pointer.py
 wlroots/wlr_types/screencopy_v1.py
 wlroots/wlr_types/seat.py
 wlroots/wlr_types/surface.py
 wlroots/wlr_types/texture.py
 wlroots/wlr_types/virtual_keyboard_v1.py
 wlroots/wlr_types/xcursor_manager.py
```

### Comparing `pywlroots-0.2.8/setup.cfg` & `pywlroots-0.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `pywlroots-0.2.8/wlroots/__init__.py` & `pywlroots-0.2.9/wlroots/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # Copyright (c) Sean Vig 2018
 
+from typing import Any
+
 from ._ffi import ffi, lib  # noqa: F401
 
 __wlroots_version__ = "{}.{}.{}".format(
     lib.WLR_VERSION_MAJOR,
     lib.WLR_VERSION_MICRO,
     lib.WLR_VERSION_MINOR,
 )
 
-__version__ = "0.2.8"
+__version__ = "0.2.9"
 
 
 class Ptr:
     """Add equality checks for objects holding the same cdata
 
     Objects that reference the same cdata objects will be treated as equal.
     Note that these objects will still have a different hash such that they
@@ -24,7 +26,23 @@
     def __eq__(self, other) -> bool:
         """Return true if the other object holds the same cdata"""
         return hasattr(other, "_ptr") and self._ptr == other._ptr
 
     def __hash__(self) -> int:
         """Use the hash from `object`, which is unique per object"""
         return super().__hash__()
+
+
+class PtrHasData(Ptr):
+    """
+    Add methods to get and set the void *data member on the wrapped struct. The value
+    stored can be of any Python type.
+    """
+
+    @property
+    def data(self) -> Any:
+        return ffi.from_handle(self._ptr.data)
+
+    @data.setter
+    def data(self, data: Any) -> None:
+        self._data_handle = ffi.new_handle(data)
+        self._ptr.data = self._data_handle
```

### Comparing `pywlroots-0.2.8/wlroots/backend.py` & `pywlroots-0.2.9/wlroots/backend.py`

 * *Files identical despite different names*

### Comparing `pywlroots-0.2.8/wlroots/ffi_build.py` & `pywlroots-0.2.9/wlroots/ffi_build.py`

 * *Files 2% similar despite different names*

```diff
@@ -461,14 +461,19 @@
 void wlr_output_create_global(struct wlr_output *output);
 void wlr_output_destroy_global(struct wlr_output *output);
 
 struct wlr_output_mode *wlr_output_preferred_mode(struct wlr_output *output);
 
 void wlr_output_set_mode(struct wlr_output *output,
     struct wlr_output_mode *mode);
+void wlr_output_set_custom_mode(struct wlr_output *output, int32_t width,
+    int32_t height, int32_t refresh);
+void wlr_output_set_transform(struct wlr_output *output,
+    enum wl_output_transform transform);
+void wlr_output_set_scale(struct wlr_output *output, float scale);
 
 bool wlr_output_attach_render(struct wlr_output *output, int *buffer_age);
 void wlr_output_transformed_resolution(struct wlr_output *output,
     int *width, int *height);
 void wlr_output_effective_resolution(struct wlr_output *output,
     int *width, int *height);
 void wlr_output_set_damage(struct wlr_output *output,
@@ -528,27 +533,131 @@
 
 void wlr_output_damage_add_box(struct wlr_output_damage *output_damage,
     struct wlr_box *box);
 """
 
 # types/wlr_output_layout.h
 CDEF += """
+struct wlr_output_layout {
+    struct wl_list outputs;
+    struct wlr_output_layout_state *state;
+
+    struct {
+        struct wl_signal add;
+        struct wl_signal change;
+        struct wl_signal destroy;
+    } events;
+
+    void *data;
+    ...;
+};
 struct wlr_output_layout *wlr_output_layout_create(void);
 void wlr_output_layout_destroy(struct wlr_output_layout *layout);
 
 void wlr_output_layout_output_coords(struct wlr_output_layout *layout,
     struct wlr_output *reference, double *lx, double *ly);
 
+void wlr_output_layout_closest_point(struct wlr_output_layout *layout,
+    struct wlr_output *reference, double lx, double ly, double *dest_lx,
+    double *dest_ly);
+
+void wlr_output_layout_add(struct wlr_output_layout *layout,
+    struct wlr_output *output, int lx, int ly);
+
+void wlr_output_layout_move(struct wlr_output_layout *layout,
+    struct wlr_output *output, int lx, int ly);
+
+void wlr_output_layout_remove(struct wlr_output_layout *layout,
+    struct wlr_output *output);
+
+struct wlr_box *wlr_output_layout_get_box(
+    struct wlr_output_layout *layout, struct wlr_output *reference);
+
 void wlr_output_layout_add_auto(struct wlr_output_layout *layout,
     struct wlr_output *output);
 
 struct wlr_output *wlr_output_layout_output_at(struct wlr_output_layout *layout,
     double lx, double ly);
 """
 
+# types/wlr_output_management_v1.h
+CDEF += """
+struct wlr_output_manager_v1 {
+    struct wl_display *display;
+    struct wl_global *global;
+    struct wl_list resources; // wl_resource_get_link
+    struct wl_list heads; // wlr_output_head_v1::link
+    uint32_t serial;
+    bool current_configuration_dirty;
+
+    struct {
+        struct wl_signal apply; // wlr_output_configuration_v1
+        struct wl_signal test; // wlr_output_configuration_v1
+        struct wl_signal destroy;
+    } events;
+
+    struct wl_listener display_destroy;
+    void *data;
+    ...;
+};
+
+struct wlr_output_configuration_v1 {
+    struct wl_list heads; // wlr_output_configuration_head_v1::link
+
+    // client state
+    struct wlr_output_manager_v1 *manager;
+    uint32_t serial;
+    bool finalized; // client has requested to apply the config
+    bool finished; // feedback has been sent by the compositor
+    struct wl_resource *resource; // can be NULL if destroyed early
+    ...;
+};
+
+struct wlr_output_configuration_head_v1 {
+    struct wlr_output_head_v1_state state;
+    struct wlr_output_configuration_v1 *config;
+    struct wl_list link; // wlr_output_configuration_v1::heads
+    // client state
+    struct wl_resource *resource; // can be NULL if finalized or disabled
+    struct wl_listener output_destroy;
+    ...;
+};
+
+struct wlr_output_head_v1_state {
+    struct wlr_output *output;
+
+    bool enabled;
+    struct wlr_output_mode *mode;
+    struct {
+        int32_t width, height;
+        int32_t refresh;
+    } custom_mode;
+    int32_t x, y;
+    enum wl_output_transform transform;
+    float scale;
+};
+
+struct wlr_output_manager_v1 *wlr_output_manager_v1_create(
+    struct wl_display *display);
+
+void wlr_output_manager_v1_set_configuration(
+    struct wlr_output_manager_v1 *manager,
+    struct wlr_output_configuration_v1 *config);
+struct wlr_output_configuration_v1 *wlr_output_configuration_v1_create(void);
+void wlr_output_configuration_v1_send_succeeded(
+    struct wlr_output_configuration_v1 *config);
+void wlr_output_configuration_v1_send_failed(
+    struct wlr_output_configuration_v1 *config);
+struct wlr_output_configuration_head_v1 *
+    wlr_output_configuration_head_v1_create(
+    struct wlr_output_configuration_v1 *config, struct wlr_output *output);
+void wlr_output_configuration_v1_destroy(
+    struct wlr_output_configuration_v1 *config);
+"""
+
 # types/wlr_pointer.h
 CDEF += """
 struct wlr_pointer {
     const struct wlr_pointer_impl *impl;
 
     struct {
         struct wl_signal motion;
@@ -1176,14 +1285,59 @@
         struct wl_signal destroy;
     } events;
 
     void *data;
     ...;
 };
 
+struct wlr_xdg_client {
+    struct wlr_xdg_shell *shell;
+    struct wl_resource *resource;
+    struct wl_client *client;
+    struct wl_list surfaces;
+
+    struct wl_list link; // wlr_xdg_shell::clients
+
+    uint32_t ping_serial;
+    struct wl_event_source *ping_timer;
+};
+
+struct wlr_xdg_positioner {
+    struct wlr_box anchor_rect;
+    enum xdg_positioner_anchor anchor;
+    enum xdg_positioner_gravity gravity;
+    enum xdg_positioner_constraint_adjustment constraint_adjustment;
+
+    struct {
+        int32_t width, height;
+    } size;
+
+    struct {
+        int32_t x, y;
+    } offset;
+    ...;
+};
+
+struct wlr_xdg_popup {
+    struct wlr_xdg_surface *base;
+    struct wl_list link;
+
+    struct wl_resource *resource;
+    bool committed;
+    struct wlr_surface *parent;
+    struct wlr_seat *seat;
+
+    struct wlr_box geometry;
+
+    struct wlr_xdg_positioner positioner;
+
+    struct wl_list grab_link; // wlr_xdg_popup_grab::popups
+    ...;
+};
+
 struct wlr_xdg_shell *wlr_xdg_shell_create(struct wl_display *display);
 
 struct wlr_xdg_toplevel_state {
     bool maximized, fullscreen, resizing, activated;
     uint32_t tiled;
     uint32_t width, height;
     uint32_t max_width, max_height;
@@ -1298,14 +1452,17 @@
     struct wlr_xdg_surface *surface;
     struct wlr_seat_client *seat;
     uint32_t serial;
     uint32_t x, y;
     ...;
 };
 
+void wlr_xdg_popup_unconstrain_from_box(struct wlr_xdg_popup *popup,
+    const struct wlr_box *toplevel_sx_box);
+
 void wlr_xdg_surface_ping(struct wlr_xdg_surface *surface);
 
 uint32_t wlr_xdg_toplevel_set_size(struct wlr_xdg_surface *surface,
     uint32_t width, uint32_t height);
 uint32_t wlr_xdg_toplevel_set_activated(struct wlr_xdg_surface *surface,
     bool activated);
 uint32_t wlr_xdg_toplevel_set_maximized(struct wlr_xdg_surface *surface,
@@ -1409,14 +1566,15 @@
 #include <wlr/types/wlr_keyboard.h>
 #include <wlr/types/wlr_layer_shell_v1.h>
 #include <wlr/types/wlr_linux_dmabuf_v1.h>
 #include <wlr/types/wlr_matrix.h>
 #include <wlr/types/wlr_output.h>
 #include <wlr/types/wlr_output_damage.h>
 #include <wlr/types/wlr_output_layout.h>
+#include <wlr/types/wlr_output_management_v1.h>
 #include <wlr/types/wlr_screencopy_v1.h>
 #include <wlr/types/wlr_surface.h>
 #include <wlr/types/wlr_seat.h>
 #include <wlr/types/wlr_virtual_keyboard_v1.h>
 #include <wlr/types/wlr_xcursor_manager.h>
 #include <wlr/types/wlr_xdg_decoration_v1.h>
 #include <wlr/types/wlr_xdg_output_v1.h>
```

### Comparing `pywlroots-0.2.8/wlroots/helper.py` & `pywlroots-0.2.9/wlroots/helper.py`

 * *Files identical despite different names*

### Comparing `pywlroots-0.2.8/wlroots/renderer.py` & `pywlroots-0.2.9/wlroots/renderer.py`

 * *Files identical despite different names*

### Comparing `pywlroots-0.2.8/wlroots/util/clock.py` & `pywlroots-0.2.9/wlroots/util/clock.py`

 * *Files identical despite different names*

### Comparing `pywlroots-0.2.8/wlroots/util/log.py` & `pywlroots-0.2.9/wlroots/util/log.py`

 * *Files identical despite different names*

### Comparing `pywlroots-0.2.8/wlroots/util/region.py` & `pywlroots-0.2.9/wlroots/util/region.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,21 +4,24 @@
 
 from pywayland.protocol.wayland import WlOutput
 from wlroots import ffi, lib, Ptr
 from wlroots.wlr_types.box import Box
 
 
 class PixmanRegion32(Ptr):
-    def __init__(self) -> None:
+    def __init__(self, ptr=None) -> None:
         """This is a convenience wrapper around pixman_region32_t
 
         :param ptr:
             The pixman_region32_t cdata pointer
         """
-        self._ptr = ffi.new("struct pixman_region32 *")
+        if ptr is None:
+            self._ptr = ffi.new("struct pixman_region32 *")
+        else:
+            self._ptr = ptr
 
     def __enter__(self) -> "PixmanRegion32":
         """Use the pixman_region32 in a context manager"""
         lib.pixman_region32_init(self._ptr)
         return self
 
     def __exit__(self, exc_type, exc_value, exc_tb) -> None:
@@ -35,15 +38,19 @@
             boxes.append(
                 Box(rects.x1, rects.y1, rects.x2 - rects.x1, rects.y2 - rects.y1)
             )
             rects += 1
         return boxes
 
     def transform(
-        self, src: "PixmanRegion32", transform: WlOutput.transform, width: int, height: int
+        self,
+        src: "PixmanRegion32",
+        transform: WlOutput.transform,
+        width: int,
+        height: int,
     ) -> None:
         """
         Applies a transform to a region inside a box of size `width` x `height`.
         """
         lib.wlr_region_transform(self._ptr, src._ptr, transform, width, height)
 
     def not_empty(self) -> bool:
```

### Comparing `pywlroots-0.2.8/wlroots/wlr_types/__init__.py` & `pywlroots-0.2.9/wlroots/wlr_types/__init__.py`

 * *Files identical despite different names*

### Comparing `pywlroots-0.2.8/wlroots/wlr_types/compositor.py` & `pywlroots-0.2.9/wlroots/wlr_types/compositor.py`

 * *Files identical despite different names*

### Comparing `pywlroots-0.2.8/wlroots/wlr_types/cursor.py` & `pywlroots-0.2.9/wlroots/wlr_types/cursor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Sean Vig 2019
 
 import enum
 from typing import Optional, Tuple
 
 from pywayland.server import Signal
 
-from wlroots import ffi, lib, Ptr
+from wlroots import ffi, PtrHasData, lib
 from .input_device import InputDevice, InputDeviceType
 from .output_layout import OutputLayout
 from .pointer import (
     PointerEventAxis,
     PointerEventButton,
     PointerEventMotion,
     PointerEventMotionAbsolute,
@@ -25,15 +25,15 @@
 
 class WarpMode(enum.Enum):
     Layout = enum.auto()
     LayoutClosest = enum.auto()
     AbsoluteClosest = enum.auto()
 
 
-class Cursor(Ptr):
+class Cursor(PtrHasData):
     def __init__(self, output_layout: OutputLayout) -> None:
         """Manage a cursor attached to the given output layout
 
         Uses the given layout to establish the boundaries and movement
         semantics of this cursor. Cursors without an output layout allow
         infinite movement in any direction and do not support absolute input
         events.
```

### Comparing `pywlroots-0.2.8/wlroots/wlr_types/input_device.py` & `pywlroots-0.2.9/wlroots/wlr_types/input_device.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) Sean Vig 2019
 
 import enum
 import weakref
 
 from .keyboard import Keyboard
-from wlroots import ffi, lib, Ptr
+from wlroots import ffi, PtrHasData, lib
 
 _weakkeydict: weakref.WeakKeyDictionary = weakref.WeakKeyDictionary()
 
 
 @enum.unique
 class ButtonState(enum.IntEnum):
     RELEASED = lib.WLR_BUTTON_RELEASED
@@ -21,15 +21,15 @@
     POINTER = lib.WLR_INPUT_DEVICE_POINTER
     TOUCH = lib.WLR_INPUT_DEVICE_TOUCH
     TABLET_TOOL = lib.WLR_INPUT_DEVICE_TABLET_TOOL
     TABLET_PAD = lib.WLR_INPUT_DEVICE_TABLET_PAD
     SWITCH = lib.WLR_INPUT_DEVICE_SWITCH
 
 
-class InputDevice(Ptr):
+class InputDevice(PtrHasData):
     def __init__(self, ptr) -> None:
         """Create the input device from the given cdata
 
         :param ptr:
             The wlr_input_device for the given input device
         """
         self._ptr = ffi.cast("struct wlr_input_device *", ptr)
```

### Comparing `pywlroots-0.2.8/wlroots/wlr_types/keyboard.py` & `pywlroots-0.2.9/wlroots/wlr_types/keyboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import enum
 from weakref import WeakKeyDictionary
 
 from pywayland.server import Signal
 from pywayland.protocol.wayland import WlKeyboard
 
-from wlroots import ffi, lib, Ptr
+from wlroots import ffi, PtrHasData, lib, Ptr
 
 _weakkeydict: WeakKeyDictionary = WeakKeyDictionary()
 
 
 @enum.unique
 class KeyboardLed(enum.IntFlag):
     NUM_LOCK = lib.WLR_LED_NUM_LOCK
@@ -56,15 +56,15 @@
 
     @property
     def state(self) -> WlKeyboard.key_state:
         """The state of the keycode triggering the event"""
         return WlKeyboard.key_state(self._ptr.state)
 
 
-class Keyboard(Ptr):
+class Keyboard(PtrHasData):
     def __init__(self, ptr) -> None:
         """The Keyboard wlroots object
 
         :param ptr:
             The wlr_keyboard cdata pointer for the given keyboard
         """
         self._ptr = ptr
```

### Comparing `pywlroots-0.2.8/wlroots/wlr_types/layer_shell_v1.py` & `pywlroots-0.2.9/wlroots/wlr_types/layer_shell_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import enum
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Optional, Tuple
 from weakref import WeakKeyDictionary
 
 from pywayland.server import Signal
 
-from wlroots import ffi, lib, Ptr
+from wlroots import ffi, PtrHasData, lib, Ptr
 from .output import Output
 from .surface import Surface
 from .xdg_shell import SurfaceCallback, T
 
 if TYPE_CHECKING:
     from pywayland.server import Display
 
@@ -86,15 +86,15 @@
         return self._ptr.actual_height
 
     @property
     def layer(self) -> LayerShellV1Layer:
         return LayerShellV1Layer(self._ptr.layer)
 
 
-class LayerSurfaceV1(Ptr):
+class LayerSurfaceV1(PtrHasData):
     def __init__(self, ptr):
         self._ptr = ffi.cast("struct wlr_layer_surface_v1 *", ptr)
 
         self.destroy_event = Signal(ptr=ffi.addressof(self._ptr.events.destroy))
         self.map_event = Signal(ptr=ffi.addressof(self._ptr.events.map))
         self.unmap_event = Signal(ptr=ffi.addressof(self._ptr.events.unmap))
         self.new_popup_event = Signal(ptr=ffi.addressof(self._ptr.events.new_popup))
@@ -195,15 +195,15 @@
         )
         if surface_ptr == ffi.NULL:
             return None, 0.0, 0.0
 
         return Surface(surface_ptr), sub_x_data[0], sub_y_data[0]
 
 
-class LayerShellV1(Ptr):
+class LayerShellV1(PtrHasData):
     def __init__(self, display: "Display") -> None:
         """Create an wlr_xdg_output_manager_v1"""
         self._ptr = lib.wlr_layer_shell_v1_create(display._ptr)
 
         self.new_surface_event = Signal(
             ptr=ffi.addressof(self._ptr.events.new_surface), data_wrapper=LayerSurfaceV1
         )
```

### Comparing `pywlroots-0.2.8/wlroots/wlr_types/matrix.py` & `pywlroots-0.2.9/wlroots/wlr_types/matrix.py`

 * *Files identical despite different names*

### Comparing `pywlroots-0.2.8/wlroots/wlr_types/output.py` & `pywlroots-0.2.9/wlroots/wlr_types/output.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 # Copyright (c) Matt Colligan 2021
 
 from typing import Tuple, Optional
 
 from pywayland.server import Signal
 from pywayland.protocol.wayland import WlOutput
 
-from wlroots import ffi, lib, Ptr
+from wlroots import ffi, PtrHasData, lib, Ptr
 from wlroots.util.region import PixmanRegion32
 from .matrix import Matrix
 
 
-class Output(Ptr):
+class Output(PtrHasData):
     def __init__(self, ptr) -> None:
         """A compositor output region
 
         This typically corresponds to a monitor that displays part of the
         compositor space.
 
         The `frame` event will be emitted when it is a good time for the
@@ -78,14 +78,18 @@
             return []
 
     @property
     def enabled(self) -> bool:
         return self._ptr.enabled
 
     @property
+    def current_mode(self) -> "OutputMode":
+        return OutputMode(self._ptr.current_mode)
+
+    @property
     def scale(self) -> float:
         return self._ptr.scale
 
     @property
     def transform(self) -> WlOutput.transform:
         return WlOutput.transform(self._ptr.transform)
 
@@ -115,14 +119,24 @@
     def set_mode(self, mode: "OutputMode") -> None:
         """Sets the output mode
 
         The output needs to be enabled.
         """
         lib.wlr_output_set_mode(self._ptr, mode._ptr)
 
+    def set_custom_mode(
+        self, mode: "OutputMode", width: int, height: int, refresh: int
+    ) -> None:
+        """
+        Sets a custom mode on the output. If modes are available, they are preferred.
+        Setting `refresh` to zero lets the backend pick a preferred value. The
+        output needs to be enabled.
+        """
+        lib.wlr_output_set_custom_mode(self._ptr, width, height, refresh)
+
     def create_global(self) -> None:
         """Create the global corresponding to the output"""
         lib.wlr_output_create_global(self._ptr)
 
     def __enter__(self) -> "Output":
         """Start rendering frame"""
         return self
@@ -202,14 +216,40 @@
 
         This region is not to be confused with the renderer's buffer damage, ie. the
         region compositors need to repaint. Compositors usually need to repaint more
         than what changed since last frame since multiple render buffers are used.
         """
         lib.wlr_output_set_damage(self._ptr, damage._ptr)
 
+    def set_transform(self, transform: WlOutput.transform) -> None:
+        """
+        Sets a transform for the output.
+
+        Transform is double-buffered state, see `wlr_output_commit`.
+        """
+        lib.wlr_output_set_transform(self._ptr, transform)
+
+    def set_scale(self, scale: float) -> None:
+        """
+        Sets a scale for the output.
+
+        Scale is double-buffered state, see `wlr_output_commit`.
+        """
+        lib.wlr_output_set_scale(self._ptr, scale)
+
+    def test(self) -> bool:
+        """
+        Test whether the pending output state would be accepted by the backend. If
+        this function returns true, `wlr_output_commit` can only fail due to a
+        runtime error.
+
+        This function doesn't mutate the pending state.
+        """
+        return lib.wlr_output_test(self._ptr)
+
 
 class OutputMode(Ptr):
     def __init__(self, ptr) -> None:
         self._ptr = ptr
 
     @property
     def width(self) -> int:
```

### Comparing `pywlroots-0.2.8/wlroots/wlr_types/output_damage.py` & `pywlroots-0.2.9/wlroots/wlr_types/output_damage.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,18 @@
         self.destroy_event = Signal(ptr=ffi.addressof(self._ptr.events.destroy))
 
     @property
     def output(self) -> Output:
         """The name of the output"""
         return Output(self._ptr.output)
 
+    @property
+    def current(self) -> PixmanRegion32:
+        return PixmanRegion32(ffi.addressof(self._ptr.current))
+
     def destroy(self) -> None:
         """The name of the output"""
         lib.wlr_output_damage_destroy(self._ptr)
         self._ptr = None
 
     def attach_render(self, damage: PixmanRegion32) -> bool:
         """
@@ -49,15 +53,17 @@
         The buffer damage region accumulates all damage since the buffer has last
         been swapped. This is not to be confused with the output surface damage,
         which only contains the changes between two frames.
 
         Returns a bool specifying whether the output needs a new frame rendered.
         """
         needs_frame_ptr = ffi.new("bool *")
-        if not lib.wlr_output_damage_attach_render(self._ptr, needs_frame_ptr, damage._ptr):
+        if not lib.wlr_output_damage_attach_render(
+            self._ptr, needs_frame_ptr, damage._ptr
+        ):
             raise RuntimeError("Rendering on output failed")
 
         return needs_frame_ptr[0]
 
     def add(self, damage: PixmanRegion32) -> None:
         """Accumulates damage and schedules a `frame` event."""
         lib.wlr_output_damage_add(self._ptr, damage._ptr)
```

### Comparing `pywlroots-0.2.8/wlroots/wlr_types/pointer.py` & `pywlroots-0.2.9/wlroots/wlr_types/pointer.py`

 * *Files identical despite different names*

### Comparing `pywlroots-0.2.8/wlroots/wlr_types/seat.py` & `pywlroots-0.2.9/wlroots/wlr_types/seat.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import Optional, Tuple
 from weakref import WeakKeyDictionary
 
 from pywayland.server import Display, Signal
 from pywayland.protocol.wayland import WlSeat
 
-from wlroots import ffi, lib, Ptr
+from wlroots import ffi, PtrHasData, lib, Ptr
 from .input_device import ButtonState, InputDevice
 from .keyboard import Keyboard, KeyboardModifiers, KeyboardKeyEvent
 from .pointer import AxisSource, AxisOrientation
 from .surface import Surface
 
 _weakkeydict: WeakKeyDictionary = WeakKeyDictionary()
 
@@ -27,15 +27,15 @@
         return self
 
     def __exit__(self, exc_type, exc_value, exc_tb) -> None:
         """End the grab of the keyboard of this seat"""
         lib.wlr_seat_keyboard_end_grab(self._seat)
 
 
-class Seat(Ptr):
+class Seat(PtrHasData):
     def __init__(self, display: Display, name: str) -> None:
         """Allocates a new seat and adds a seat global to the display
 
         :param display:
             The Wayland server display to attach the seat to
         :param name:
             The name of the seat to create
```

### Comparing `pywlroots-0.2.8/wlroots/wlr_types/surface.py` & `pywlroots-0.2.9/wlroots/wlr_types/surface.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Copyright Sean Vig (c) 2020
 
 from weakref import WeakKeyDictionary
 
 from pywayland.protocol.wayland import WlOutput
 from pywayland.server import Signal
 
-from wlroots import ffi, lib, Ptr
+from wlroots import ffi, PtrHasData, lib, Ptr
 from wlroots.util.clock import Timespec
 from .texture import Texture
 
 _weakkeydict: WeakKeyDictionary = WeakKeyDictionary()
 
 
-class Surface(Ptr):
+class Surface(PtrHasData):
     def __init__(self, ptr):
         """Create a wlroots Surface
 
         :param ptr:
             The cdata for the given surface
         """
         self._ptr = ptr
```

### Comparing `pywlroots-0.2.8/wlroots/wlr_types/texture.py` & `pywlroots-0.2.9/wlroots/wlr_types/texture.py`

 * *Files identical despite different names*

### Comparing `pywlroots-0.2.8/wlroots/wlr_types/virtual_keyboard_v1.py` & `pywlroots-0.2.9/wlroots/wlr_types/virtual_keyboard_v1.py`

 * *Files identical despite different names*

### Comparing `pywlroots-0.2.8/wlroots/wlr_types/xcursor_manager.py` & `pywlroots-0.2.9/wlroots/wlr_types/xcursor_manager.py`

 * *Files identical despite different names*

### Comparing `pywlroots-0.2.8/wlroots/wlr_types/xdg_decoration_v1.py` & `pywlroots-0.2.9/wlroots/wlr_types/xdg_decoration_v1.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,54 +2,56 @@
 
 import enum
 from typing import TYPE_CHECKING
 from weakref import WeakKeyDictionary
 
 from pywayland.server import Signal
 
-from wlroots import ffi, lib, Ptr
+from wlroots import ffi, PtrHasData, lib
 from .surface import Surface
 
 if TYPE_CHECKING:
     from pywayland.server import Display
 
 _weakkeydict: WeakKeyDictionary = WeakKeyDictionary()
 
 
 class XdgToplevelDecorationV1Mode(enum.IntEnum):
     NONE = lib.WLR_XDG_TOPLEVEL_DECORATION_V1_MODE_NONE
     CLIENT_SIDE = lib.WLR_XDG_TOPLEVEL_DECORATION_V1_MODE_CLIENT_SIDE
     SERVER_SIDE = lib.WLR_XDG_TOPLEVEL_DECORATION_V1_MODE_SERVER_SIDE
 
 
-class XdgDecorationManagerV1(Ptr):
+class XdgDecorationManagerV1(PtrHasData):
     def __init__(self, ptr) -> None:
         """An XDG decoration manager: wlr_xdg_decoration_manager_v1."""
         self._ptr = ffi.cast("struct wlr_xdg_decoration_manager_v1 *", ptr)
 
         self.new_toplevel_decoration_event = Signal(
             ptr=ffi.addressof(self._ptr.events.new_toplevel_decoration),
-            data_wrapper=XdgToplevelDecorationV1
+            data_wrapper=XdgToplevelDecorationV1,
         )
         self.destroy_event = Signal(ptr=ffi.addressof(self._ptr.events.destroy))
 
     @classmethod
     def create(cls, display: "Display"):
         """Create a wlr_xdg_decoration_manager_v1 for the given display."""
         ptr = lib.wlr_xdg_decoration_manager_v1_create(display._ptr)
         return cls(ptr)
 
 
-class XdgToplevelDecorationV1(Ptr):
+class XdgToplevelDecorationV1(PtrHasData):
     def __init__(self, ptr) -> None:
         """struct wlr_xdg_toplevel_decoration_v1"""
         self._ptr = ffi.cast("struct wlr_xdg_toplevel_decoration_v1 *", ptr)
 
         self.destroy_event = Signal(ptr=ffi.addressof(self._ptr.events.destroy))
-        self.request_mode_event = Signal(ptr=ffi.addressof(self._ptr.events.request_mode))
+        self.request_mode_event = Signal(
+            ptr=ffi.addressof(self._ptr.events.request_mode)
+        )
 
     @property
     def surface(self) -> Surface:
         surface_ptr = self._ptr.surface
         _weakkeydict[surface_ptr] = self._ptr
         return Surface(surface_ptr)
```

### Comparing `pywlroots-0.2.8/wlroots/wlr_types/xdg_shell.py` & `pywlroots-0.2.9/wlroots/wlr_types/xdg_shell.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import enum
 import weakref
 from typing import Callable, Optional, Tuple, TypeVar
 
 from pywayland.server import Display, Signal
 
-from wlroots import ffi, lib, Ptr
+from wlroots import ffi, PtrHasData, lib, Ptr
 from wlroots.util.edges import Edges
 from .box import Box
 from .output import Output
 from .surface import Surface
 
 _weakkeydict: weakref.WeakKeyDictionary = weakref.WeakKeyDictionary()
 
@@ -28,30 +28,30 @@
 
 class XdgSurfaceRole(enum.IntEnum):
     NONE = lib.WLR_XDG_SURFACE_ROLE_NONE
     TOPLEVEL = lib.WLR_XDG_SURFACE_ROLE_TOPLEVEL
     POPUP = lib.WLR_XDG_SURFACE_ROLE_POPUP
 
 
-class XdgShell(Ptr):
+class XdgShell(PtrHasData):
     def __init__(self, display: Display) -> None:
         """Create the shell for protocol windows
 
         :param display:
             The Wayland server display to create the shell on.
         """
         self._ptr = lib.wlr_xdg_shell_create(display._ptr)
 
         self.new_surface_event = Signal(
             ptr=ffi.addressof(self._ptr.events.new_surface), data_wrapper=XdgSurface
         )
         self.destroy_event = Signal(ptr=ffi.addressof(self._ptr.events.destroy))
 
 
-class XdgSurface(Ptr):
+class XdgSurface(PtrHasData):
     def __init__(self, ptr) -> None:
         """A user interface element requiring management by the compositor
 
         An xdg-surface is a user interface element requiring management by the
         compositor. An xdg-surface alone isn't useful, a role should be
         assigned to it in order to map it.
 
@@ -61,14 +61,17 @@
         the `destroy` event if the view is destroyed when mapped
         """
         self._ptr = ffi.cast("struct wlr_xdg_surface *", ptr)
 
         self.map_event = Signal(ptr=ffi.addressof(self._ptr.events.map))
         self.unmap_event = Signal(ptr=ffi.addressof(self._ptr.events.unmap))
         self.destroy_event = Signal(ptr=ffi.addressof(self._ptr.events.destroy))
+        self.new_popup_event = Signal(
+            ptr=ffi.addressof(self._ptr.events.new_popup), data_wrapper=XdgPopup
+        )
 
     @classmethod
     def from_surface(cls, surface: Surface) -> "XdgSurface":
         """Get the xdg surface associated with the given surface"""
         if not surface.is_xdg_surface:
             raise RuntimeError("Surface is not XDG surface")
         surface_ptr = lib.wlr_xdg_surface_from_wlr_surface(surface._ptr)
@@ -288,7 +291,30 @@
     @property
     def x(self) -> int:
         return self._ptr.x
 
     @property
     def y(self) -> int:
         return self._ptr.y
+
+
+class XdgPopup(Ptr):
+    def __init__(self, ptr) -> None:
+        """A wlr_xdg_popup
+
+        :param ptr:
+            The wlr_xdg_popup cdata pointer
+        """
+        self._ptr = ffi.cast("struct wlr_xdg_popup *", ptr)
+
+    @property
+    def base(self) -> XdgSurface:
+        """The xdg surface associated with the popup"""
+        return XdgSurface(self._ptr.base)
+
+    def unconstrain_from_box(self, box: Box) -> None:
+        """
+        Set the geometry of this popup to unconstrain it according to its xdg-positioner
+        rules. The box should be in the popup's root toplevel parent surface coordinate
+        system.
+        """
+        lib.wlr_xdg_popup_unconstrain_from_box(self._ptr, box._ptr)
```

