# Comparing `tmp/midas-goa-1.0.0rc5.tar.gz` & `tmp/midas-goa-1.0.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midas-goa-1.0.0rc5.tar", last modified: Mon May  9 08:13:05 2022, max compression
+gzip compressed data, was "midas-goa-1.0.0rc6.tar", last modified: Wed Jun 15 11:03:58 2022, max compression
```

## Comparing `midas-goa-1.0.0rc5.tar` & `midas-goa-1.0.0rc6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-05-09 08:13:05.990148 midas-goa-1.0.0rc5/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     7648 2022-04-06 13:16:46.000000 midas-goa-1.0.0rc5/LICENSE
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1016 2022-05-09 08:13:05.990148 midas-goa-1.0.0rc5/PKG-INFO
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)       27 2022-04-06 13:17:03.000000 midas-goa-1.0.0rc5/README.md
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-05-09 08:13:05.986815 midas-goa-1.0.0rc5/midas/
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-05-09 08:13:05.986815 midas-goa-1.0.0rc5/midas/modules/
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-05-09 08:13:05.986815 midas-goa-1.0.0rc5/midas/modules/goa/
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-05-09 06:28:20.000000 midas-goa-1.0.0rc5/midas/modules/goa/__init__.py
--rwxrwxrwx   0 sbalduin  (1000) wheel      (998)      648 2022-04-06 13:21:05.000000 midas-goa-1.0.0rc5/midas/modules/goa/meta.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-05-09 08:13:05.990148 midas-goa-1.0.0rc5/midas/modules/goa/model/
--rwxrwxrwx   0 sbalduin  (1000) wheel      (998)        0 2022-04-06 13:21:05.000000 midas-goa-1.0.0rc5/midas/modules/goa/model/__init__.py
--rwxrwxrwx   0 sbalduin  (1000) wheel      (998)     3367 2022-04-25 08:26:41.000000 midas-goa-1.0.0rc5/midas/modules/goa/model/coordinator.py
--rwxrwxrwx   0 sbalduin  (1000) wheel      (998)     4233 2022-04-06 13:21:05.000000 midas-goa-1.0.0rc5/midas/modules/goa/model/grid_analyzer.py
--rwxrwxrwx   0 sbalduin  (1000) wheel      (998)     6338 2022-04-06 13:23:31.000000 midas-goa-1.0.0rc5/midas/modules/goa/model/grid_forecaster.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      833 2022-05-04 08:01:27.000000 midas-goa-1.0.0rc5/midas/modules/goa/model/grid_observer.py
--rwxrwxrwx   0 sbalduin  (1000) wheel      (998)     2375 2022-05-09 08:07:20.000000 midas-goa-1.0.0rc5/midas/modules/goa/model/load_estimator.py
--rwxrwxrwx   0 sbalduin  (1000) wheel      (998)     5807 2022-04-06 13:21:05.000000 midas-goa-1.0.0rc5/midas/modules/goa/model/messenger.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     8359 2022-05-09 06:28:20.000000 midas-goa-1.0.0rc5/midas/modules/goa/module.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     5078 2022-05-09 08:07:20.000000 midas-goa-1.0.0rc5/midas/modules/goa/simulator.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-05-09 08:13:05.990148 midas-goa-1.0.0rc5/midas_goa.egg-info/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1016 2022-05-09 08:13:05.000000 midas-goa-1.0.0rc5/midas_goa.egg-info/PKG-INFO
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      584 2022-05-09 08:13:05.000000 midas-goa-1.0.0rc5/midas_goa.egg-info/SOURCES.txt
--rw-r--r--   0 sbalduin  (1000) wheel      (998)        1 2022-05-09 08:13:05.000000 midas-goa-1.0.0rc5/midas_goa.egg-info/dependency_links.txt
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      133 2022-05-09 08:13:05.000000 midas-goa-1.0.0rc5/midas_goa.egg-info/requires.txt
--rw-r--r--   0 sbalduin  (1000) wheel      (998)        6 2022-05-09 08:13:05.000000 midas-goa-1.0.0rc5/midas_goa.egg-info/top_level.txt
--rw-r--r--   0 sbalduin  (1000) wheel      (998)       38 2022-05-09 08:13:05.990148 midas-goa-1.0.0rc5/setup.cfg
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     1718 2022-04-06 13:28:50.000000 midas-goa-1.0.0rc5/setup.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-06-15 11:03:58.513725 midas-goa-1.0.0rc6/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     7648 2022-04-06 13:16:46.000000 midas-goa-1.0.0rc6/LICENSE
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1016 2022-06-15 11:03:58.513725 midas-goa-1.0.0rc6/PKG-INFO
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)       27 2022-04-06 13:17:03.000000 midas-goa-1.0.0rc6/README.md
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-06-15 11:03:58.513725 midas-goa-1.0.0rc6/midas/
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-06-15 11:03:58.513725 midas-goa-1.0.0rc6/midas/modules/
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-06-15 11:03:58.513725 midas-goa-1.0.0rc6/midas/modules/goa/
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-05-09 06:28:20.000000 midas-goa-1.0.0rc6/midas/modules/goa/__init__.py
+-rwxrwxrwx   0 sbalduin  (1000) wheel      (998)      648 2022-04-06 13:21:05.000000 midas-goa-1.0.0rc6/midas/modules/goa/meta.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-06-15 11:03:58.513725 midas-goa-1.0.0rc6/midas/modules/goa/model/
+-rwxrwxrwx   0 sbalduin  (1000) wheel      (998)        0 2022-04-06 13:21:05.000000 midas-goa-1.0.0rc6/midas/modules/goa/model/__init__.py
+-rwxrwxrwx   0 sbalduin  (1000) wheel      (998)     3367 2022-04-25 08:26:41.000000 midas-goa-1.0.0rc6/midas/modules/goa/model/coordinator.py
+-rwxrwxrwx   0 sbalduin  (1000) wheel      (998)     4233 2022-04-06 13:21:05.000000 midas-goa-1.0.0rc6/midas/modules/goa/model/grid_analyzer.py
+-rwxrwxrwx   0 sbalduin  (1000) wheel      (998)     6338 2022-04-06 13:23:31.000000 midas-goa-1.0.0rc6/midas/modules/goa/model/grid_forecaster.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      833 2022-05-04 08:01:27.000000 midas-goa-1.0.0rc6/midas/modules/goa/model/grid_observer.py
+-rwxrwxrwx   0 sbalduin  (1000) wheel      (998)     2375 2022-05-09 08:07:20.000000 midas-goa-1.0.0rc6/midas/modules/goa/model/load_estimator.py
+-rwxrwxrwx   0 sbalduin  (1000) wheel      (998)     5807 2022-04-06 13:21:05.000000 midas-goa-1.0.0rc6/midas/modules/goa/model/messenger.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     8391 2022-06-15 10:59:54.000000 midas-goa-1.0.0rc6/midas/modules/goa/module.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     5078 2022-05-09 08:07:20.000000 midas-goa-1.0.0rc6/midas/modules/goa/simulator.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-06-15 11:03:58.513725 midas-goa-1.0.0rc6/midas_goa.egg-info/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1016 2022-06-15 11:03:58.000000 midas-goa-1.0.0rc6/midas_goa.egg-info/PKG-INFO
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      584 2022-06-15 11:03:58.000000 midas-goa-1.0.0rc6/midas_goa.egg-info/SOURCES.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)        1 2022-06-15 11:03:58.000000 midas-goa-1.0.0rc6/midas_goa.egg-info/dependency_links.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      133 2022-06-15 11:03:58.000000 midas-goa-1.0.0rc6/midas_goa.egg-info/requires.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)        6 2022-06-15 11:03:58.000000 midas-goa-1.0.0rc6/midas_goa.egg-info/top_level.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)       38 2022-06-15 11:03:58.513725 midas-goa-1.0.0rc6/setup.cfg
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     1718 2022-04-06 13:28:50.000000 midas-goa-1.0.0rc6/setup.py
```

### Comparing `midas-goa-1.0.0rc5/LICENSE` & `midas-goa-1.0.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `midas-goa-1.0.0rc5/PKG-INFO` & `midas-goa-1.0.0rc6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas-goa
-Version: 1.0.0rc5
+Version: 1.0.0rc6
 Summary: A MIDAS module for the grid operator agent.
 Home-page: https://gitlab.com/midas-mosaik/midas-goa
 Author: Stephan Balduin
 Author-email: stephan.balduin@offis.de
 License: LGPL
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `midas-goa-1.0.0rc5/midas/modules/goa/meta.py` & `midas-goa-1.0.0rc6/midas/modules/goa/meta.py`

 * *Files identical despite different names*

### Comparing `midas-goa-1.0.0rc5/midas/modules/goa/model/coordinator.py` & `midas-goa-1.0.0rc6/midas/modules/goa/model/coordinator.py`

 * *Files identical despite different names*

### Comparing `midas-goa-1.0.0rc5/midas/modules/goa/model/grid_analyzer.py` & `midas-goa-1.0.0rc6/midas/modules/goa/model/grid_analyzer.py`

 * *Files identical despite different names*

### Comparing `midas-goa-1.0.0rc5/midas/modules/goa/model/grid_forecaster.py` & `midas-goa-1.0.0rc6/midas/modules/goa/model/grid_forecaster.py`

 * *Files identical despite different names*

### Comparing `midas-goa-1.0.0rc5/midas/modules/goa/model/grid_observer.py` & `midas-goa-1.0.0rc6/midas/modules/goa/model/grid_observer.py`

 * *Files identical despite different names*

### Comparing `midas-goa-1.0.0rc5/midas/modules/goa/model/load_estimator.py` & `midas-goa-1.0.0rc6/midas/modules/goa/model/load_estimator.py`

 * *Files identical despite different names*

### Comparing `midas-goa-1.0.0rc5/midas/modules/goa/model/messenger.py` & `midas-goa-1.0.0rc6/midas/modules/goa/model/messenger.py`

 * *Files identical despite different names*

### Comparing `midas-goa-1.0.0rc5/midas/modules/goa/module.py` & `midas-goa-1.0.0rc6/midas/modules/goa/module.py`

 * *Files 7% similar despite different names*

```diff
@@ -150,15 +150,15 @@
             attrs = sensors["goa_output"]
             goa = self.scenario.generate_model_key(self, model)
             self.connect_entities(goa, db_key, attrs)
 
     def get_sensors(self):
         for model, sensors in self.models.items():
             # attrs = sensors["goa_output"]
-            goa = self.scenario[self.gen_mod_key(model)]
+            goa = self.scenario.get_model(self.scenario.generate_model_key(self, model))
             self.scenario.sensors.append(
                 {
                     "sensor_id": f"{goa.full_id}.health",
                     "observation_space": (
                         "Box(low=0, high=1.2, shape=(1,), dtype=np.float32)"
                     ),
                 }
```

### Comparing `midas-goa-1.0.0rc5/midas/modules/goa/simulator.py` & `midas-goa-1.0.0rc6/midas/modules/goa/simulator.py`

 * *Files identical despite different names*

### Comparing `midas-goa-1.0.0rc5/midas_goa.egg-info/PKG-INFO` & `midas-goa-1.0.0rc6/midas_goa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas-goa
-Version: 1.0.0rc5
+Version: 1.0.0rc6
 Summary: A MIDAS module for the grid operator agent.
 Home-page: https://gitlab.com/midas-mosaik/midas-goa
 Author: Stephan Balduin
 Author-email: stephan.balduin@offis.de
 License: LGPL
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `midas-goa-1.0.0rc5/midas_goa.egg-info/SOURCES.txt` & `midas-goa-1.0.0rc6/midas_goa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `midas-goa-1.0.0rc5/setup.py` & `midas-goa-1.0.0rc6/setup.py`

 * *Files identical despite different names*

