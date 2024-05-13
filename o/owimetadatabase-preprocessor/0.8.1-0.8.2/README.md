# Comparing `tmp/owimetadatabase_preprocessor-0.8.1.tar.gz` & `tmp/owimetadatabase_preprocessor-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owimetadatabase_preprocessor-0.8.1.tar", max compression
+gzip compressed data, was "owimetadatabase_preprocessor-0.8.2.tar", max compression
```

## Comparing `owimetadatabase_preprocessor-0.8.1.tar` & `owimetadatabase_preprocessor-0.8.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35148 2024-04-30 08:33:48.953993 owimetadatabase_preprocessor-0.8.1/LICENSE
--rw-r--r--   0        0        0     1471 2024-04-30 08:33:48.957993 owimetadatabase_preprocessor-0.8.1/README.md
--rw-r--r--   0        0        0     2535 2024-04-30 08:33:48.957993 owimetadatabase_preprocessor-0.8.1/pyproject.toml
--rw-r--r--   0        0        0       84 2024-04-30 08:33:48.957993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/__init__.py
--rw-r--r--   0        0        0       66 2024-04-30 08:33:48.957993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/fatigue/__init__.py
--rw-r--r--   0        0        0    34147 2024-04-30 08:33:48.957993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/fatigue/data_objects.py
--rw-r--r--   0        0        0    24890 2024-04-30 08:33:48.957993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/fatigue/io.py
--rw-r--r--   0        0        0       40 2024-04-30 08:33:48.957993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/geometry/__init__.py
--rw-r--r--   0        0        0    11835 2024-04-30 08:33:48.957993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/geometry/io.py
--rw-r--r--   0        0        0    38484 2024-04-30 08:33:48.957993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/geometry/processing.py
--rw-r--r--   0        0        0    24884 2024-04-30 08:33:48.957993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/geometry/structures.py
--rw-r--r--   0        0        0     7067 2024-04-30 08:33:48.957993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/io.py
--rw-r--r--   0        0        0       41 2024-04-30 08:33:48.961993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/locations/__init__.py
--rw-r--r--   0        0        0     8155 2024-04-30 08:33:48.961993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/locations/io.py
--rw-r--r--   0        0        0        0 2024-04-30 08:33:48.961993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/soil/__init__.py
--rw-r--r--   0        0        0    87680 2024-04-30 08:33:48.961993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/soil/io.py
--rw-r--r--   0        0        0     7268 2024-04-30 08:33:48.961993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/utils.py
--rw-r--r--   0        0        0     3748 1970-01-01 00:00:00.000000 owimetadatabase_preprocessor-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-05-13 09:44:59.506966 owimetadatabase_preprocessor-0.8.2/LICENSE
+-rw-r--r--   0        0        0     1471 2024-05-13 09:44:59.506966 owimetadatabase_preprocessor-0.8.2/README.md
+-rw-r--r--   0        0        0     2535 2024-05-13 09:44:59.510966 owimetadatabase_preprocessor-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0       84 2024-05-13 09:44:59.510966 owimetadatabase_preprocessor-0.8.2/src/owimetadatabase_preprocessor/__init__.py
+-rw-r--r--   0        0        0       66 2024-05-13 09:44:59.510966 owimetadatabase_preprocessor-0.8.2/src/owimetadatabase_preprocessor/fatigue/__init__.py
+-rw-r--r--   0        0        0    34147 2024-05-13 09:44:59.510966 owimetadatabase_preprocessor-0.8.2/src/owimetadatabase_preprocessor/fatigue/data_objects.py
+-rw-r--r--   0        0        0    24938 2024-05-13 09:44:59.510966 owimetadatabase_preprocessor-0.8.2/src/owimetadatabase_preprocessor/fatigue/io.py
+-rw-r--r--   0        0        0       40 2024-05-13 09:44:59.510966 owimetadatabase_preprocessor-0.8.2/src/owimetadatabase_preprocessor/geometry/__init__.py
+-rw-r--r--   0        0        0    12192 2024-05-13 09:44:59.510966 owimetadatabase_preprocessor-0.8.2/src/owimetadatabase_preprocessor/geometry/io.py
+-rw-r--r--   0        0        0    38484 2024-05-13 09:44:59.510966 owimetadatabase_preprocessor-0.8.2/src/owimetadatabase_preprocessor/geometry/processing.py
+-rw-r--r--   0        0        0    24884 2024-05-13 09:44:59.510966 owimetadatabase_preprocessor-0.8.2/src/owimetadatabase_preprocessor/geometry/structures.py
+-rw-r--r--   0        0        0     7067 2024-05-13 09:44:59.510966 owimetadatabase_preprocessor-0.8.2/src/owimetadatabase_preprocessor/io.py
+-rw-r--r--   0        0        0       41 2024-05-13 09:44:59.510966 owimetadatabase_preprocessor-0.8.2/src/owimetadatabase_preprocessor/locations/__init__.py
+-rw-r--r--   0        0        0     8155 2024-05-13 09:44:59.510966 owimetadatabase_preprocessor-0.8.2/src/owimetadatabase_preprocessor/locations/io.py
+-rw-r--r--   0        0        0        0 2024-05-13 09:44:59.510966 owimetadatabase_preprocessor-0.8.2/src/owimetadatabase_preprocessor/soil/__init__.py
+-rw-r--r--   0        0        0    87680 2024-05-13 09:44:59.510966 owimetadatabase_preprocessor-0.8.2/src/owimetadatabase_preprocessor/soil/io.py
+-rw-r--r--   0        0        0     7268 2024-05-13 09:44:59.510966 owimetadatabase_preprocessor-0.8.2/src/owimetadatabase_preprocessor/utils.py
+-rw-r--r--   0        0        0     3748 1970-01-01 00:00:00.000000 owimetadatabase_preprocessor-0.8.2/PKG-INFO
```

### Comparing `owimetadatabase_preprocessor-0.8.1/LICENSE` & `owimetadatabase_preprocessor-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `owimetadatabase_preprocessor-0.8.1/README.md` & `owimetadatabase_preprocessor-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `owimetadatabase_preprocessor-0.8.1/pyproject.toml` & `owimetadatabase_preprocessor-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "owimetadatabase-preprocessor"
-version = "0.8.1"
+version = "0.8.2"
 description = "Package for preprocessing data from owimetadatabase."
 authors = ["arsmlnkv <melnikov.arsene@gmail.com>"]
 readme = "README.md"
 homepage = "https://owi-lab.github.io/owimetadatabase-preprocessor/"
 repository = "https://github.com/OWI-Lab/owimetadatabase-preprocessor"
 license = "GNU General Public License v3.0"
 keywords = ["owimetadatabase"]
```

### Comparing `owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/fatigue/data_objects.py` & `owimetadatabase_preprocessor-0.8.2/src/owimetadatabase_preprocessor/fatigue/data_objects.py`

 * *Files identical despite different names*

### Comparing `owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/fatigue/io.py` & `owimetadatabase_preprocessor-0.8.2/src/owimetadatabase_preprocessor/fatigue/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,16 +52,16 @@
             credentials = {"token": token}
         elif uname and password:
             credentials = {"uname": uname, "password": password}
         elif kwargs is not None:
             credentials = {}
         else:
             raise ValueError("No credentials provided.")
-        self.geo_api = GeometryAPI(**credentials, **kwargs)
-        self.loc_api = LocationsAPI(**credentials, **kwargs)
+        self.geo_api = GeometryAPI(api_root=self.api_root, **credentials, **kwargs)
+        self.loc_api = LocationsAPI(api_root=self.api_root, **credentials, **kwargs)
         self.api_root = self.api_root + api_subdir
 
     def get_sncurves(self, **kwargs) -> List[SNCurve]:
         """Get all available SN curves requested by the user.
 
         :param kwargs: Any API filter, e.g. 'title__icontains=NRTA1'
         :return: List of SNCurve objects representing SN curves
```

### Comparing `owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/geometry/io.py` & `owimetadatabase_preprocessor-0.8.2/src/owimetadatabase_preprocessor/geometry/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,23 @@
         :param token: Optional: token to access the API.
         :param uname: Optional: username to access the API.
         :param password: Optional: password to access the API.
         :param kwargs: Additional parameters to pass to the API.
         :return: None
         """
         super().__init__(api_root, token, uname, password, **kwargs)
+        if token:
+            credentials = {"token": token}
+        elif uname and password:
+            credentials = {"uname": uname, "password": password}
+        elif kwargs is not None:
+            credentials = {}
+        else:
+            raise ValueError("No credentials provided.")
+        self.loc_api = LocationsAPI(api_root=self.api_root, **credentials, **kwargs)
         self.api_root = self.api_root + api_subdir
 
     def get_subassemblies(
         self,
         projectsite: Union[str, None] = None,
         assetlocation: Union[str, None] = None,
         subassembly_type: Union[str, None] = None,
@@ -166,15 +175,15 @@
         owts = []
         turbines = [turbines] if isinstance(turbines, str) else turbines
         if not isinstance(tower_base, List) and not isinstance(monopile_head, List):
             tower_base = [tower_base] * len(turbines)  # type: ignore
             monopile_head = [monopile_head] * len(turbines)  # type: ignore
         for i in range(len(turbines)):
             subassemblies_data = self.get_subassemblies(assetlocation=turbines[i])
-            location_data = LocationsAPI(header=self.header).get_assetlocation_detail(
+            location_data = self.loc_api.get_assetlocation_detail(
                 assetlocation=turbines[i]
             )
             if subassemblies_data["exists"] and location_data["exists"]:
                 subassemblies = subassemblies_data["data"]
                 location = location_data["data"]
             elif not subassemblies_data["exists"] and not location_data["exists"]:
                 raise ValueError(
```

### Comparing `owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/geometry/processing.py` & `owimetadatabase_preprocessor-0.8.2/src/owimetadatabase_preprocessor/geometry/processing.py`

 * *Files identical despite different names*

### Comparing `owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/geometry/structures.py` & `owimetadatabase_preprocessor-0.8.2/src/owimetadatabase_preprocessor/geometry/structures.py`

 * *Files identical despite different names*

### Comparing `owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/io.py` & `owimetadatabase_preprocessor-0.8.2/src/owimetadatabase_preprocessor/io.py`

 * *Files identical despite different names*

### Comparing `owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/locations/io.py` & `owimetadatabase_preprocessor-0.8.2/src/owimetadatabase_preprocessor/locations/io.py`

 * *Files identical despite different names*

### Comparing `owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/soil/io.py` & `owimetadatabase_preprocessor-0.8.2/src/owimetadatabase_preprocessor/soil/io.py`

 * *Files identical despite different names*

### Comparing `owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/utils.py` & `owimetadatabase_preprocessor-0.8.2/src/owimetadatabase_preprocessor/utils.py`

 * *Files identical despite different names*

### Comparing `owimetadatabase_preprocessor-0.8.1/PKG-INFO` & `owimetadatabase_preprocessor-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owimetadatabase-preprocessor
-Version: 0.8.1
+Version: 0.8.2
 Summary: Package for preprocessing data from owimetadatabase.
 Home-page: https://owi-lab.github.io/owimetadatabase-preprocessor/
 License: GNU General Public License v3.0
 Keywords: owimetadatabase
 Author: arsmlnkv
 Author-email: melnikov.arsene@gmail.com
 Requires-Python: >=3.9,<3.13
```

