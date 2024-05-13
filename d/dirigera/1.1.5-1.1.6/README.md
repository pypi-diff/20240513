# Comparing `tmp/dirigera-1.1.5.tar.gz` & `tmp/dirigera-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dirigera-1.1.5.tar", last modified: Sat Apr 20 08:49:56 2024, max compression
+gzip compressed data, was "dirigera-1.1.6.tar", last modified: Fri Apr 26 06:15:03 2024, max compression
```

## Comparing `dirigera-1.1.5.tar` & `dirigera-1.1.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:49:56.037443 dirigera-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-20 08:49:52.000000 dirigera-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-04-20 08:49:56.037443 dirigera-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13383 2024-04-20 08:49:52.000000 dirigera-1.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-20 08:49:52.000000 dirigera-1.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 08:49:56.037443 dirigera-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-20 08:49:52.000000 dirigera-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:49:56.029443 dirigera-1.1.5/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:49:56.029443 dirigera-1.1.5/src/dirigera/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:49:56.033443 dirigera-1.1.5/src/dirigera/devices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/devices/air_purifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/devices/base_ikea_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/devices/blinds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/devices/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/devices/environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/devices/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/devices/motion_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/devices/open_close_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/devices/outlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/devices/scene.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/devices/water_sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:49:56.033443 dirigera-1.1.5/src/dirigera/hub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/hub/abstract_smart_home_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    15813 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/hub/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/hub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:49:56.033443 dirigera-1.1.5/src/dirigera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-04-20 08:49:56.000000 dirigera-1.1.5/src/dirigera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-20 08:49:56.000000 dirigera-1.1.5/src/dirigera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 08:49:56.000000 dirigera-1.1.5/src/dirigera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-20 08:49:56.000000 dirigera-1.1.5/src/dirigera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-20 08:49:56.000000 dirigera-1.1.5/src/dirigera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-20 08:49:56.000000 dirigera-1.1.5/src/dirigera.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:49:56.033443 dirigera-1.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-20 08:49:52.000000 dirigera-1.1.5/tests/test_air_purifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-20 08:49:52.000000 dirigera-1.1.5/tests/test_blinds.py
--rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-20 08:49:52.000000 dirigera-1.1.5/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-20 08:49:52.000000 dirigera-1.1.5/tests/test_environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12981 2024-04-20 08:49:52.000000 dirigera-1.1.5/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-20 08:49:52.000000 dirigera-1.1.5/tests/test_motion_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-20 08:49:52.000000 dirigera-1.1.5/tests/test_open_close_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-04-20 08:49:52.000000 dirigera-1.1.5/tests/test_outlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-20 08:49:52.000000 dirigera-1.1.5/tests/test_scenes.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-20 08:49:52.000000 dirigera-1.1.5/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-20 08:49:52.000000 dirigera-1.1.5/tests/test_water_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:15:03.405449 dirigera-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-26 06:14:54.000000 dirigera-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16363 2024-04-26 06:15:03.405449 dirigera-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14132 2024-04-26 06:14:54.000000 dirigera-1.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-26 06:14:54.000000 dirigera-1.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 06:15:03.405449 dirigera-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-26 06:14:54.000000 dirigera-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:15:03.397449 dirigera-1.1.6/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 06:14:54.000000 dirigera-1.1.6/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:15:03.397449 dirigera-1.1.6/src/dirigera/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-26 06:14:54.000000 dirigera-1.1.6/src/dirigera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:15:03.401449 dirigera-1.1.6/src/dirigera/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 06:14:54.000000 dirigera-1.1.6/src/dirigera/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-26 06:14:54.000000 dirigera-1.1.6/src/dirigera/devices/air_purifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-26 06:14:54.000000 dirigera-1.1.6/src/dirigera/devices/base_ikea_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-26 06:14:54.000000 dirigera-1.1.6/src/dirigera/devices/blinds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-26 06:14:54.000000 dirigera-1.1.6/src/dirigera/devices/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-26 06:14:54.000000 dirigera-1.1.6/src/dirigera/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-26 06:14:54.000000 dirigera-1.1.6/src/dirigera/devices/environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-26 06:14:54.000000 dirigera-1.1.6/src/dirigera/devices/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-26 06:14:54.000000 dirigera-1.1.6/src/dirigera/devices/motion_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-26 06:14:54.000000 dirigera-1.1.6/src/dirigera/devices/open_close_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-26 06:14:54.000000 dirigera-1.1.6/src/dirigera/devices/outlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-26 06:14:54.000000 dirigera-1.1.6/src/dirigera/devices/scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-26 06:14:54.000000 dirigera-1.1.6/src/dirigera/devices/water_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:15:03.401449 dirigera-1.1.6/src/dirigera/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 06:14:54.000000 dirigera-1.1.6/src/dirigera/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-26 06:14:54.000000 dirigera-1.1.6/src/dirigera/hub/abstract_smart_home_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-26 06:14:54.000000 dirigera-1.1.6/src/dirigera/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15813 2024-04-26 06:14:54.000000 dirigera-1.1.6/src/dirigera/hub/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-26 06:14:54.000000 dirigera-1.1.6/src/dirigera/hub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:15:03.405449 dirigera-1.1.6/src/dirigera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16363 2024-04-26 06:15:03.000000 dirigera-1.1.6/src/dirigera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-26 06:15:03.000000 dirigera-1.1.6/src/dirigera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 06:15:03.000000 dirigera-1.1.6/src/dirigera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-26 06:15:03.000000 dirigera-1.1.6/src/dirigera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-26 06:15:03.000000 dirigera-1.1.6/src/dirigera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 06:15:03.000000 dirigera-1.1.6/src/dirigera.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:15:03.405449 dirigera-1.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-26 06:14:54.000000 dirigera-1.1.6/tests/test_air_purifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-26 06:14:54.000000 dirigera-1.1.6/tests/test_blinds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-26 06:14:54.000000 dirigera-1.1.6/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-26 06:14:54.000000 dirigera-1.1.6/tests/test_environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12981 2024-04-26 06:14:54.000000 dirigera-1.1.6/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-26 06:14:54.000000 dirigera-1.1.6/tests/test_motion_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-26 06:14:54.000000 dirigera-1.1.6/tests/test_open_close_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-04-26 06:14:54.000000 dirigera-1.1.6/tests/test_outlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-04-26 06:14:54.000000 dirigera-1.1.6/tests/test_scenes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-26 06:14:54.000000 dirigera-1.1.6/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-26 06:14:54.000000 dirigera-1.1.6/tests/test_water_sensor.py
```

### Comparing `dirigera-1.1.5/LICENSE` & `dirigera-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.5/PKG-INFO` & `dirigera-1.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 1.1.5
+Version: 1.1.6
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -414,19 +414,34 @@
 )
 ```
 
 Triggers look like this:
 
 ```python
 class Trigger(BaseIkeaModel):
-    id: str
+    id: Optional[str] = None
     type: str
     triggered_at: Optional[datetime.datetime] = None
     disabled: bool
+    trigger: Optional[TriggerDetails] = None
+```
 
+Example how to create scene with trigger:
+```python
+from dirigera.devices.scene import Info, Icon, Trigger, SceneType, TriggerDetails, ControllerType, ClickPattern
+
+scene = dirigera_hub.create_scene(
+   info=Info(name="Scene with trigger", icon=Icon.SCENES_HEART),
+   scene_type=SceneType.USER_SCENE,
+   triggers=[
+       Trigger(type="app", disabled=False),
+       Trigger(type="controller", disabled=False,
+               trigger=TriggerDetails(clickPattern=ClickPattern.SINGLE_PRESS, buttonIndex=0,
+                                      deviceId="0000aaaa-0000-0000-aa00-0a0aa0a000a0_1",
+                                      controllerType=ControllerType.SHORTCUT_CONTROLLER))])
 ```
 
 All available icons can be found here: [Icons](./src/dirigera/devices/scene.py)
 
 ## [Motion Sensor](./src/dirigera/devices/motion_sensor.py)
 
 To get information about the available motion sensors, you can use the `get_motion_sensors()` method:
```

### Comparing `dirigera-1.1.5/README.md` & `dirigera-1.1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -367,19 +367,34 @@
 )
 ```
 
 Triggers look like this:
 
 ```python
 class Trigger(BaseIkeaModel):
-    id: str
+    id: Optional[str] = None
     type: str
     triggered_at: Optional[datetime.datetime] = None
     disabled: bool
+    trigger: Optional[TriggerDetails] = None
+```
+
+Example how to create scene with trigger:
+```python
+from dirigera.devices.scene import Info, Icon, Trigger, SceneType, TriggerDetails, ControllerType, ClickPattern
 
+scene = dirigera_hub.create_scene(
+   info=Info(name="Scene with trigger", icon=Icon.SCENES_HEART),
+   scene_type=SceneType.USER_SCENE,
+   triggers=[
+       Trigger(type="app", disabled=False),
+       Trigger(type="controller", disabled=False,
+               trigger=TriggerDetails(clickPattern=ClickPattern.SINGLE_PRESS, buttonIndex=0,
+                                      deviceId="0000aaaa-0000-0000-aa00-0a0aa0a000a0_1",
+                                      controllerType=ControllerType.SHORTCUT_CONTROLLER))])
 ```
 
 All available icons can be found here: [Icons](./src/dirigera/devices/scene.py)
 
 ## [Motion Sensor](./src/dirigera/devices/motion_sensor.py)
 
 To get information about the available motion sensors, you can use the `get_motion_sensors()` method:
```

### Comparing `dirigera-1.1.5/pyproject.toml` & `dirigera-1.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dirigera"
-version = "1.1.5"
+version = "1.1.6"
 description = "An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub"
 readme = "README.md"
 authors = [{ name = "Leggin", email = "legginsun@gmail.com" }]
 license = { file = "LICENSE" }
 keywords = [
     "python",
     "iot",
```

### Comparing `dirigera-1.1.5/src/dirigera/devices/air_purifier.py` & `dirigera-1.1.6/src/dirigera/devices/air_purifier.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.5/src/dirigera/devices/blinds.py` & `dirigera-1.1.6/src/dirigera/devices/blinds.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.5/src/dirigera/devices/controller.py` & `dirigera-1.1.6/src/dirigera/devices/controller.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.5/src/dirigera/devices/device.py` & `dirigera-1.1.6/src/dirigera/devices/device.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.5/src/dirigera/devices/environment_sensor.py` & `dirigera-1.1.6/src/dirigera/devices/environment_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.5/src/dirigera/devices/light.py` & `dirigera-1.1.6/src/dirigera/devices/light.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.5/src/dirigera/devices/motion_sensor.py` & `dirigera-1.1.6/src/dirigera/devices/motion_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.5/src/dirigera/devices/open_close_sensor.py` & `dirigera-1.1.6/src/dirigera/devices/open_close_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.5/src/dirigera/devices/outlet.py` & `dirigera-1.1.6/src/dirigera/devices/outlet.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.5/src/dirigera/devices/scene.py` & `dirigera-1.1.6/src/dirigera/devices/scene.py`

 * *Files 12% similar despite different names*

```diff
@@ -56,18 +56,39 @@
 
 class Info(BaseIkeaModel):
     name: str
     icon: Icon
 
 
 class Trigger(BaseIkeaModel):
-    id: str
+    id: Optional[str] = None  # Optional to allow creation of Trigger instances for create_scene()
     type: str
     triggered_at: Optional[datetime.datetime] = None
     disabled: bool
+    trigger: Optional[TriggerDetails] = None
+
+
+class TriggerDetails(BaseIkeaModel):
+    days: Optional[List[str]] = None
+    controllerType: Optional[ControllerType] = None
+    buttonIndex: Optional[int] = None
+    clickPattern: Optional[ClickPattern] = None
+    deviceId: Optional[str] = None
+    offset: Optional[int] = None
+    type: Optional[str] = None
+
+
+class ControllerType(Enum):
+    SHORTCUT_CONTROLLER = "shortcutController"
+
+
+class ClickPattern(Enum):
+    LONG_PRESS = "longPress"
+    DOUBLE_PRESS = "doublePress"
+    SINGLE_PRESS = "singlePress"
 
 
 class ActionAttributes(BaseIkeaModel, extra="allow"):
     is_on: Optional[bool] = None
 
 
 class Action(BaseIkeaModel):
```

### Comparing `dirigera-1.1.5/src/dirigera/devices/water_sensor.py` & `dirigera-1.1.6/src/dirigera/devices/water_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.5/src/dirigera/hub/abstract_smart_home_hub.py` & `dirigera-1.1.6/src/dirigera/hub/abstract_smart_home_hub.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.5/src/dirigera/hub/auth.py` & `dirigera-1.1.6/src/dirigera/hub/auth.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.5/src/dirigera/hub/hub.py` & `dirigera-1.1.6/src/dirigera/hub/hub.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.5/src/dirigera.egg-info/PKG-INFO` & `dirigera-1.1.6/src/dirigera.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 1.1.5
+Version: 1.1.6
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -414,19 +414,34 @@
 )
 ```
 
 Triggers look like this:
 
 ```python
 class Trigger(BaseIkeaModel):
-    id: str
+    id: Optional[str] = None
     type: str
     triggered_at: Optional[datetime.datetime] = None
     disabled: bool
+    trigger: Optional[TriggerDetails] = None
+```
 
+Example how to create scene with trigger:
+```python
+from dirigera.devices.scene import Info, Icon, Trigger, SceneType, TriggerDetails, ControllerType, ClickPattern
+
+scene = dirigera_hub.create_scene(
+   info=Info(name="Scene with trigger", icon=Icon.SCENES_HEART),
+   scene_type=SceneType.USER_SCENE,
+   triggers=[
+       Trigger(type="app", disabled=False),
+       Trigger(type="controller", disabled=False,
+               trigger=TriggerDetails(clickPattern=ClickPattern.SINGLE_PRESS, buttonIndex=0,
+                                      deviceId="0000aaaa-0000-0000-aa00-0a0aa0a000a0_1",
+                                      controllerType=ControllerType.SHORTCUT_CONTROLLER))])
 ```
 
 All available icons can be found here: [Icons](./src/dirigera/devices/scene.py)
 
 ## [Motion Sensor](./src/dirigera/devices/motion_sensor.py)
 
 To get information about the available motion sensors, you can use the `get_motion_sensors()` method:
```

### Comparing `dirigera-1.1.5/src/dirigera.egg-info/SOURCES.txt` & `dirigera-1.1.6/src/dirigera.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.5/tests/test_air_purifier.py` & `dirigera-1.1.6/tests/test_air_purifier.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.5/tests/test_blinds.py` & `dirigera-1.1.6/tests/test_blinds.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.5/tests/test_controller.py` & `dirigera-1.1.6/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.5/tests/test_environment_sensor.py` & `dirigera-1.1.6/tests/test_environment_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.5/tests/test_light.py` & `dirigera-1.1.6/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.5/tests/test_motion_sensor.py` & `dirigera-1.1.6/tests/test_motion_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.5/tests/test_open_close_sensor.py` & `dirigera-1.1.6/tests/test_open_close_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.5/tests/test_outlet.py` & `dirigera-1.1.6/tests/test_outlet.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.5/tests/test_utils.py` & `dirigera-1.1.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.5/tests/test_water_sensor.py` & `dirigera-1.1.6/tests/test_water_sensor.py`

 * *Files identical despite different names*

