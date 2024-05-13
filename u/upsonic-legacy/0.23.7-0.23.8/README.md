# Comparing `tmp/upsonic_legacy-0.23.7.tar.gz` & `tmp/upsonic_legacy-0.23.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upsonic_legacy-0.23.7.tar", last modified: Fri May 10 17:36:37 2024, max compression
+gzip compressed data, was "upsonic_legacy-0.23.8.tar", last modified: Mon May 13 12:05:43 2024, max compression
```

## Comparing `upsonic_legacy-0.23.7.tar` & `upsonic_legacy-0.23.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:36:37.715702 upsonic_legacy-0.23.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-10 17:36:26.000000 upsonic_legacy-0.23.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-10 17:36:26.000000 upsonic_legacy-0.23.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-05-10 17:36:37.715702 upsonic_legacy-0.23.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-10 17:36:26.000000 upsonic_legacy-0.23.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-10 17:36:26.000000 upsonic_legacy-0.23.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 17:36:37.715702 upsonic_legacy-0.23.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-10 17:36:26.000000 upsonic_legacy-0.23.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:36:37.715702 upsonic_legacy-0.23.7/upsonic/
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-10 17:36:26.000000 upsonic_legacy-0.23.7/upsonic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:36:37.715702 upsonic_legacy-0.23.7/upsonic/remote/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-10 17:36:26.000000 upsonic_legacy-0.23.7/upsonic/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25476 2024-05-10 17:36:26.000000 upsonic_legacy-0.23.7/upsonic/remote/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-10 17:36:26.000000 upsonic_legacy-0.23.7/upsonic/remote/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    15387 2024-05-10 17:36:26.000000 upsonic_legacy-0.23.7/upsonic/remote/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:36:37.715702 upsonic_legacy-0.23.7/upsonic/remote/localimport/
--rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-05-10 17:36:26.000000 upsonic_legacy-0.23.7/upsonic/remote/localimport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52236 2024-05-10 17:36:26.000000 upsonic_legacy-0.23.7/upsonic/remote/on_prem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:36:37.715702 upsonic_legacy-0.23.7/upsonic_legacy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-05-10 17:36:37.000000 upsonic_legacy-0.23.7/upsonic_legacy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-10 17:36:37.000000 upsonic_legacy-0.23.7/upsonic_legacy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 17:36:37.000000 upsonic_legacy-0.23.7/upsonic_legacy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-10 17:36:37.000000 upsonic_legacy-0.23.7/upsonic_legacy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 17:36:37.000000 upsonic_legacy-0.23.7/upsonic_legacy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-10 17:36:37.000000 upsonic_legacy-0.23.7/upsonic_legacy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 17:36:37.000000 upsonic_legacy-0.23.7/upsonic_legacy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:43.104644 upsonic_legacy-0.23.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-13 12:05:33.000000 upsonic_legacy-0.23.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-13 12:05:33.000000 upsonic_legacy-0.23.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-05-13 12:05:43.104644 upsonic_legacy-0.23.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-13 12:05:33.000000 upsonic_legacy-0.23.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 12:05:33.000000 upsonic_legacy-0.23.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 12:05:43.104644 upsonic_legacy-0.23.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-13 12:05:33.000000 upsonic_legacy-0.23.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:43.100644 upsonic_legacy-0.23.8/upsonic/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-13 12:05:33.000000 upsonic_legacy-0.23.8/upsonic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:43.100644 upsonic_legacy-0.23.8/upsonic/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-13 12:05:33.000000 upsonic_legacy-0.23.8/upsonic/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25476 2024-05-13 12:05:33.000000 upsonic_legacy-0.23.8/upsonic/remote/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-13 12:05:33.000000 upsonic_legacy-0.23.8/upsonic/remote/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15387 2024-05-13 12:05:33.000000 upsonic_legacy-0.23.8/upsonic/remote/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:43.100644 upsonic_legacy-0.23.8/upsonic/remote/localimport/
+-rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-05-13 12:05:33.000000 upsonic_legacy-0.23.8/upsonic/remote/localimport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52330 2024-05-13 12:05:33.000000 upsonic_legacy-0.23.8/upsonic/remote/on_prem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:43.104644 upsonic_legacy-0.23.8/upsonic_legacy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-05-13 12:05:42.000000 upsonic_legacy-0.23.8/upsonic_legacy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-13 12:05:43.000000 upsonic_legacy-0.23.8/upsonic_legacy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:05:42.000000 upsonic_legacy-0.23.8/upsonic_legacy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 12:05:42.000000 upsonic_legacy-0.23.8/upsonic_legacy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:05:42.000000 upsonic_legacy-0.23.8/upsonic_legacy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 12:05:42.000000 upsonic_legacy-0.23.8/upsonic_legacy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-13 12:05:42.000000 upsonic_legacy-0.23.8/upsonic_legacy.egg-info/top_level.txt
```

### Comparing `upsonic_legacy-0.23.7/LICENSE` & `upsonic_legacy-0.23.8/LICENSE`

 * *Files identical despite different names*

### Comparing `upsonic_legacy-0.23.7/PKG-INFO` & `upsonic_legacy-0.23.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upsonic_legacy
-Version: 0.23.7
+Version: 0.23.8
 Summary: Magic Cloud Layer
 Home-page: https://github.com/Upsonic/Upsonic
 Author: Upsonic
 Author-email: onur.atakan.ulusoy@upsonic.co
 License: MIT
 Description: # Upsonic | Self-Driven Autonomous Python Libraries
```

### Comparing `upsonic_legacy-0.23.7/README.md` & `upsonic_legacy-0.23.8/README.md`

 * *Files identical despite different names*

### Comparing `upsonic_legacy-0.23.7/setup.py` & `upsonic_legacy-0.23.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup
 
 with open('requirements.txt') as fp:
     install_requires = fp.read()
 setup(
     name="upsonic_legacy",
-    version="0.23.7",
+    version="0.23.8",
     description="""Magic Cloud Layer""",
     long_description="".join(open("README.md", encoding="utf-8").readlines()),
     long_description_content_type="text/markdown",
     url="https://github.com/Upsonic/Upsonic",
     author="Upsonic",
     author_email="onur.atakan.ulusoy@upsonic.co",
     license="MIT",
```

### Comparing `upsonic_legacy-0.23.7/upsonic/__init__.py` & `upsonic_legacy-0.23.8/upsonic/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,12 +24,12 @@
 from .remote import decrypt
 from .remote import upsonic_serializer
 from .remote import interface
 
 
 open_databases = {}
 
-__version__ = '0.23.7'
+__version__ = '0.23.8'
```

### Comparing `upsonic_legacy-0.23.7/upsonic/remote/__init__.py` & `upsonic_legacy-0.23.8/upsonic/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `upsonic_legacy-0.23.7/upsonic/remote/controller.py` & `upsonic_legacy-0.23.8/upsonic/remote/controller.py`

 * *Files identical despite different names*

### Comparing `upsonic_legacy-0.23.7/upsonic/remote/helper.py` & `upsonic_legacy-0.23.8/upsonic/remote/helper.py`

 * *Files identical despite different names*

### Comparing `upsonic_legacy-0.23.7/upsonic/remote/interface.py` & `upsonic_legacy-0.23.8/upsonic/remote/interface.py`

 * *Files identical despite different names*

### Comparing `upsonic_legacy-0.23.7/upsonic/remote/localimport/__init__.py` & `upsonic_legacy-0.23.8/upsonic/remote/localimport/__init__.py`

 * *Files identical despite different names*

### Comparing `upsonic_legacy-0.23.7/upsonic/remote/on_prem.py` & `upsonic_legacy-0.23.8/upsonic/remote/on_prem.py`

 * *Files 0% similar despite different names*

```diff
@@ -610,20 +610,22 @@
                 progress.update(task2, advance=1)
                 each.join()
 
     def dump(
             self,
             key,
             value,
+            message=None,
 
     ):
 
         return self.set(
             key,
             value,
+            message=message
         )
 
     def load(
             self,
             key,
             version=None
     ):
@@ -661,14 +663,15 @@
 
 
 
     def set(
             self,
             key,
             value,
+            message=None
     ):
 
         if key.startswith("."):
             self._log("Error: The key can not start with '.'")
             return False
         if ":" in key:
             self._log("Error: The key can not include ':'")
@@ -802,50 +805,48 @@
         try:
             the_engine_reports["extract_source"] = fernet.encrypt(pickle.dumps(extract_source(value, self.tester), protocol=1))
         except:
             if self.tester:
                 self._log(f"Error on extract_source while dumping {key}")
                 traceback.print_exc()
 
-        try:
-            the_engine_reports["extract_source"] = fernet.encrypt(pickle.dumps(extract_source(value, self.tester), protocol=1))
-        except:
-            if self.tester:
-                self._log(f"Error on extract_source while dumping {key}")
-                traceback.print_exc()
-
         if extracted_needed_libraries != None:
             the_engine_reports["extract_needed_libraries"] = fernet.encrypt(pickle.dumps(extracted_needed_libraries, protocol=1))
 
 
         if self.tester:
             self._log(f"the_engine_reports {the_engine_reports}")
         dumped = pickle.dumps(the_engine_reports, protocol=1)
 
 
         data = {
             "scope": key,
-            "data": fernet.encrypt(dumped)
+            "data": fernet.encrypt(dumped),
+            "commit_message": message
         }
 
         response = self._send_request("POST", "/dump", data)
 
         if response != [None]:
             return True
         else:
             return False
 
+    def print_code(self, key, version=None):
+        print(self.get(key, version=version, extract_source=True))
+
     def get(
             self,
             key,
             version=None,
             print_exc=True,
             pass_python_version_control=False,
             pass_usage_analyses=False,
-            try_to_extract_importable=False
+            try_to_extract_importable=False,
+            extract_source=False
 
     ):
         if self.tester:
             self._log(f"Process started for {key}")
         response = None
 
         encryption_key = "u"
@@ -915,14 +916,16 @@
                         if self.tester:
                             self._log(f"Local files are not enabled")
                 except:
                     if self.tester:
                         self._log(f"Error on extracted_local_files while loading {key}")
                         traceback.print_exc()
                 response.pop("extracted_local_files")
+            if extract_source:
+                return pickle.loads(fernet.decrypt(response["extract_source"]))                
             if "extract_source" in response:
                 response.pop("extract_source")
             needed_libraries = None
             if "extract_needed_libraries" in response:
                 needed_libraries = pickle.loads(fernet.decrypt(response["extract_needed_libraries"]))
                 response.pop("extract_needed_libraries")
             for engine, value in response.items():
```

### Comparing `upsonic_legacy-0.23.7/upsonic_legacy.egg-info/PKG-INFO` & `upsonic_legacy-0.23.8/upsonic_legacy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upsonic-legacy
-Version: 0.23.7
+Version: 0.23.8
 Summary: Magic Cloud Layer
 Home-page: https://github.com/Upsonic/Upsonic
 Author: Upsonic
 Author-email: onur.atakan.ulusoy@upsonic.co
 License: MIT
 Description: # Upsonic | Self-Driven Autonomous Python Libraries
```

### Comparing `upsonic_legacy-0.23.7/upsonic_legacy.egg-info/SOURCES.txt` & `upsonic_legacy-0.23.8/upsonic_legacy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

