# Comparing `tmp/pymeteobridgesql-1.2.3.tar.gz` & `tmp/pymeteobridgesql-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeteobridgesql-1.2.3.tar", last modified: Mon May  6 05:11:22 2024, max compression
+gzip compressed data, was "pymeteobridgesql-1.2.4.tar", last modified: Mon May 13 16:58:09 2024, max compression
```

## Comparing `pymeteobridgesql-1.2.3.tar` & `pymeteobridgesql-1.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:11:22.783855 pymeteobridgesql-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-06 05:11:16.000000 pymeteobridgesql-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-06 05:11:22.783855 pymeteobridgesql-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-06 05:11:16.000000 pymeteobridgesql-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:11:22.783855 pymeteobridgesql-1.2.3/pymeteobridgesql/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-06 05:11:16.000000 pymeteobridgesql-1.2.3/pymeteobridgesql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-05-06 05:11:16.000000 pymeteobridgesql-1.2.3/pymeteobridgesql/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13264 2024-05-06 05:11:16.000000 pymeteobridgesql-1.2.3/pymeteobridgesql/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:11:22.783855 pymeteobridgesql-1.2.3/pymeteobridgesql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-06 05:11:22.000000 pymeteobridgesql-1.2.3/pymeteobridgesql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-06 05:11:22.000000 pymeteobridgesql-1.2.3/pymeteobridgesql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 05:11:22.000000 pymeteobridgesql-1.2.3/pymeteobridgesql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 05:11:22.000000 pymeteobridgesql-1.2.3/pymeteobridgesql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 05:11:22.783855 pymeteobridgesql-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-06 05:11:16.000000 pymeteobridgesql-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:58:09.207349 pymeteobridgesql-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-13 16:57:57.000000 pymeteobridgesql-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-13 16:58:09.207349 pymeteobridgesql-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-13 16:57:57.000000 pymeteobridgesql-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:58:09.207349 pymeteobridgesql-1.2.4/pymeteobridgesql/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-13 16:57:57.000000 pymeteobridgesql-1.2.4/pymeteobridgesql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-05-13 16:57:57.000000 pymeteobridgesql-1.2.4/pymeteobridgesql/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13329 2024-05-13 16:57:57.000000 pymeteobridgesql-1.2.4/pymeteobridgesql/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:58:09.207349 pymeteobridgesql-1.2.4/pymeteobridgesql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-13 16:58:09.000000 pymeteobridgesql-1.2.4/pymeteobridgesql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-13 16:58:09.000000 pymeteobridgesql-1.2.4/pymeteobridgesql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:58:09.000000 pymeteobridgesql-1.2.4/pymeteobridgesql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-13 16:58:09.000000 pymeteobridgesql-1.2.4/pymeteobridgesql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 16:58:09.207349 pymeteobridgesql-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-13 16:57:57.000000 pymeteobridgesql-1.2.4/setup.py
```

### Comparing `pymeteobridgesql-1.2.3/LICENSE` & `pymeteobridgesql-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pymeteobridgesql-1.2.3/PKG-INFO` & `pymeteobridgesql-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeteobridgesql
-Version: 1.2.3
+Version: 1.2.4
 Summary: Gets weather data from a MySQL table
 Home-page: https://github.com/briis/pymeteobridgesql
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymeteobridgesql-1.2.3/pymeteobridgesql/api.py` & `pymeteobridgesql-1.2.4/pymeteobridgesql/api.py`

 * *Files identical despite different names*

### Comparing `pymeteobridgesql-1.2.3/pymeteobridgesql/data.py` & `pymeteobridgesql-1.2.4/pymeteobridgesql/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,14 +328,15 @@
     wind_speed: float
     wind_gust: float
     wind_bearing: int
     pressure: float
     pressure_trend: float
     uv: float
     solar_radiation: float
+    visibility: float
 
     def to_dict(self):
         return {
             "logdate": self.logdate,
             "temperature": self.temperature,
             "wind_chill": self.wind_chill,
             "air_Quality_pm1": self.air_Quality_pm1,
@@ -350,14 +351,15 @@
             "wind_speed": self.wind_speed,
             "wind_gust": self.wind_gust,
             "wind_bearing": self.wind_bearing,
             "pressure": self.pressure,
             "pressure_trend": self.pressure_trend,
             "uv": self.uv,
             "solar_radiation": self.solar_radiation,
+            "visibility": self.visibility,
         }
 
 @dataclass(frozen=True)
 class MonthlyData:
     logdate: datetime.date
     temperature_low: float
     temperature_high: float
```

### Comparing `pymeteobridgesql-1.2.3/pymeteobridgesql.egg-info/PKG-INFO` & `pymeteobridgesql-1.2.4/pymeteobridgesql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeteobridgesql
-Version: 1.2.3
+Version: 1.2.4
 Summary: Gets weather data from a MySQL table
 Home-page: https://github.com/briis/pymeteobridgesql
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymeteobridgesql-1.2.3/setup.py` & `pymeteobridgesql-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pymeteobridgesql",
-    version="1.2.3",
+    version="1.2.4",
     author="briis",
     author_email="bjarne@briis.com",
     description="Gets weather data from a MySQL table",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/briis/pymeteobridgesql",
```

