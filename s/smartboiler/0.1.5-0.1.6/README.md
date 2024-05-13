# Comparing `tmp/smartboiler-0.1.5.tar.gz` & `tmp/smartboiler-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartboiler-0.1.5.tar", last modified: Mon May 13 16:49:03 2024, max compression
+gzip compressed data, was "smartboiler-0.1.6.tar", last modified: Mon May 13 17:01:19 2024, max compression
```

## Comparing `smartboiler-0.1.5.tar` & `smartboiler-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:49:03.340579 smartboiler-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 16:49:03.340579 smartboiler-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-13 16:49:01.000000 smartboiler-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 16:49:03.340579 smartboiler-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-13 16:49:02.000000 smartboiler-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:49:03.336579 smartboiler-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:49:03.336579 smartboiler-0.1.5/src/smartboiler/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 16:49:01.000000 smartboiler-0.1.5/src/smartboiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13942 2024-05-13 16:49:01.000000 smartboiler-0.1.5/src/smartboiler/boiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10412 2024-05-13 16:49:01.000000 smartboiler-0.1.5/src/smartboiler/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    32013 2024-05-13 16:49:01.000000 smartboiler-0.1.5/src/smartboiler/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-13 16:49:01.000000 smartboiler-0.1.5/src/smartboiler/event_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    15569 2024-05-13 16:49:01.000000 smartboiler-0.1.5/src/smartboiler/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-13 16:49:01.000000 smartboiler-0.1.5/src/smartboiler/fotovoltaics.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 16:49:01.000000 smartboiler-0.1.5/src/smartboiler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-13 16:49:01.000000 smartboiler-0.1.5/src/smartboiler/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-13 16:49:01.000000 smartboiler-0.1.5/src/smartboiler/time_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:49:03.340579 smartboiler-0.1.5/src/smartboiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 16:49:03.000000 smartboiler-0.1.5/src/smartboiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-13 16:49:03.000000 smartboiler-0.1.5/src/smartboiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:49:03.000000 smartboiler-0.1.5/src/smartboiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-13 16:49:03.000000 smartboiler-0.1.5/src/smartboiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 16:49:03.000000 smartboiler-0.1.5/src/smartboiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 16:49:03.000000 smartboiler-0.1.5/src/smartboiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:01:19.977301 smartboiler-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 17:01:19.977301 smartboiler-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-13 17:01:17.000000 smartboiler-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 17:01:19.977301 smartboiler-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-13 17:01:18.000000 smartboiler-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:01:19.973301 smartboiler-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:01:19.977301 smartboiler-0.1.6/src/smartboiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 17:01:17.000000 smartboiler-0.1.6/src/smartboiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13942 2024-05-13 17:01:17.000000 smartboiler-0.1.6/src/smartboiler/boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-05-13 17:01:17.000000 smartboiler-0.1.6/src/smartboiler/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32013 2024-05-13 17:01:17.000000 smartboiler-0.1.6/src/smartboiler/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-13 17:01:17.000000 smartboiler-0.1.6/src/smartboiler/event_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15569 2024-05-13 17:01:17.000000 smartboiler-0.1.6/src/smartboiler/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-13 17:01:17.000000 smartboiler-0.1.6/src/smartboiler/fotovoltaics.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:01:17.000000 smartboiler-0.1.6/src/smartboiler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-13 17:01:17.000000 smartboiler-0.1.6/src/smartboiler/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-13 17:01:17.000000 smartboiler-0.1.6/src/smartboiler/time_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:01:19.977301 smartboiler-0.1.6/src/smartboiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 17:01:19.000000 smartboiler-0.1.6/src/smartboiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-13 17:01:19.000000 smartboiler-0.1.6/src/smartboiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 17:01:19.000000 smartboiler-0.1.6/src/smartboiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-13 17:01:19.000000 smartboiler-0.1.6/src/smartboiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 17:01:19.000000 smartboiler-0.1.6/src/smartboiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 17:01:19.000000 smartboiler-0.1.6/src/smartboiler.egg-info/top_level.txt
```

### Comparing `smartboiler-0.1.5/PKG-INFO` & `smartboiler-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.1.5
+Version: 0.1.6
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.1.5/README.md` & `smartboiler-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.5/setup.py` & `smartboiler-0.1.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name="smartboiler",  # Required
-    version="0.1.5",  # Required
+    version="0.1.6",  # Required
     description="Smart boiling of household",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",  # Optional (see note above)
     url="https://github.com/grinwi/smartboiler",  # Optional
     author="Adam GRUNWALD",  # Optional
     author_email="grunwald.adam24@gmail.com",  # Optional
     classifiers=[  # Optional
```

### Comparing `smartboiler-0.1.5/src/smartboiler/boiler.py` & `smartboiler-0.1.6/src/smartboiler/boiler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.5/src/smartboiler/controller.py` & `smartboiler-0.1.6/src/smartboiler/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         """Inits class of Controller. Loads settings from a settings file
 
         Args:
             settings_file (str, optional): [name of json file with settings]. Defaults to 'settings.json'.
         """
 
         self.tmp_min = 5
+        self.learning = learning
 
         self.start_date = datetime.now()
 
         self.dataHandler = dataHandler
         self.boiler = boiler
         self.forecast = forecast
         self.eventChecker = eventChecker
```

### Comparing `smartboiler-0.1.5/src/smartboiler/data_handler.py` & `smartboiler-0.1.6/src/smartboiler/data_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.5/src/smartboiler/event_checker.py` & `smartboiler-0.1.6/src/smartboiler/event_checker.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.5/src/smartboiler/forecast.py` & `smartboiler-0.1.6/src/smartboiler/forecast.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.5/src/smartboiler/fotovoltaics.py` & `smartboiler-0.1.6/src/smartboiler/fotovoltaics.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.5/src/smartboiler/switch.py` & `smartboiler-0.1.6/src/smartboiler/switch.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.5/src/smartboiler/time_handler.py` & `smartboiler-0.1.6/src/smartboiler/time_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.5/src/smartboiler.egg-info/PKG-INFO` & `smartboiler-0.1.6/src/smartboiler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.1.5
+Version: 0.1.6
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.1.5/src/smartboiler.egg-info/SOURCES.txt` & `smartboiler-0.1.6/src/smartboiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

