# Comparing `tmp/pyrippleapi-2024.2.2.tar.gz` & `tmp/pyrippleapi-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrippleapi-2024.2.2.tar", last modified: Thu Feb 29 14:16:58 2024, max compression
+gzip compressed data, was "pyrippleapi-2024.5.1.tar", last modified: Mon May 13 13:47:27 2024, max compression
```

## Comparing `pyrippleapi-2024.2.2.tar` & `pyrippleapi-2024.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-02-29 14:16:58.125759 pyrippleapi-2024.2.2/
--rw-rw-rw-   0        0        0      418 2024-02-29 14:16:58.125759 pyrippleapi-2024.2.2/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-07-11 09:09:37.000000 pyrippleapi-2024.2.2/README.md
--rw-rw-rw-   0        0        0       88 2023-05-02 10:29:46.000000 pyrippleapi-2024.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       85 2024-02-29 14:16:58.131757 pyrippleapi-2024.2.2/setup.cfg
--rw-rw-rw-   0        0        0      817 2024-02-29 14:16:52.000000 pyrippleapi-2024.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-29 14:16:58.082758 pyrippleapi-2024.2.2/src/
-drwxrwxrwx   0        0        0        0 2024-02-29 14:16:58.097758 pyrippleapi-2024.2.2/src/pyrippleapi/
--rw-rw-rw-   0        0        0        0 2023-07-11 09:10:36.000000 pyrippleapi-2024.2.2/src/pyrippleapi/__init__.py
--rw-rw-rw-   0        0        0     3287 2024-02-29 13:52:45.000000 pyrippleapi-2024.2.2/src/pyrippleapi/api.py
--rw-rw-rw-   0        0        0      336 2023-07-11 12:16:29.000000 pyrippleapi-2024.2.2/src/pyrippleapi/exceptions.py
--rw-rw-rw-   0        0        0     5756 2024-02-29 14:15:33.000000 pyrippleapi-2024.2.2/src/pyrippleapi/generation_asset.py
-drwxrwxrwx   0        0        0        0 2024-02-29 14:16:58.123757 pyrippleapi-2024.2.2/src/pyrippleapi.egg-info/
--rw-rw-rw-   0        0        0      418 2024-02-29 14:16:57.000000 pyrippleapi-2024.2.2/src/pyrippleapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-02-29 14:16:58.000000 pyrippleapi-2024.2.2/src/pyrippleapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-29 14:16:57.000000 pyrippleapi-2024.2.2/src/pyrippleapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-02-29 14:16:57.000000 pyrippleapi-2024.2.2/src/pyrippleapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-02-29 14:16:57.000000 pyrippleapi-2024.2.2/src/pyrippleapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 13:47:27.746620 pyrippleapi-2024.5.1/
+-rw-rw-rw-   0        0        0      418 2024-05-13 13:47:27.747619 pyrippleapi-2024.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-07-11 09:09:37.000000 pyrippleapi-2024.5.1/README.md
+-rw-rw-rw-   0        0        0       88 2023-05-02 10:29:46.000000 pyrippleapi-2024.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2024-05-13 13:47:27.756622 pyrippleapi-2024.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      817 2024-05-13 13:47:20.000000 pyrippleapi-2024.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 13:47:27.697619 pyrippleapi-2024.5.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-13 13:47:27.714630 pyrippleapi-2024.5.1/src/pyrippleapi/
+-rw-rw-rw-   0        0        0        0 2023-07-11 09:10:36.000000 pyrippleapi-2024.5.1/src/pyrippleapi/__init__.py
+-rw-rw-rw-   0        0        0     3287 2024-02-29 13:52:45.000000 pyrippleapi-2024.5.1/src/pyrippleapi/api.py
+-rw-rw-rw-   0        0        0      336 2023-07-11 12:16:29.000000 pyrippleapi-2024.5.1/src/pyrippleapi/exceptions.py
+-rw-rw-rw-   0        0        0     5909 2024-05-13 13:46:46.000000 pyrippleapi-2024.5.1/src/pyrippleapi/generation_asset.py
+drwxrwxrwx   0        0        0        0 2024-05-13 13:47:27.744620 pyrippleapi-2024.5.1/src/pyrippleapi.egg-info/
+-rw-rw-rw-   0        0        0      418 2024-05-13 13:47:27.000000 pyrippleapi-2024.5.1/src/pyrippleapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-05-13 13:47:27.000000 pyrippleapi-2024.5.1/src/pyrippleapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 13:47:27.000000 pyrippleapi-2024.5.1/src/pyrippleapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-13 13:47:27.000000 pyrippleapi-2024.5.1/src/pyrippleapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-13 13:47:27.000000 pyrippleapi-2024.5.1/src/pyrippleapi.egg-info/top_level.txt
```

### Comparing `pyrippleapi-2024.2.2/setup.py` & `pyrippleapi-2024.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="pyrippleapi",
-    version="2024.2.2",
+    version="2024.5.1",
     description="Ripple energy api wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ryanbdclark/pyrippleapi",
     author="Ryan Clark",
     classifiers=[
         "License :: OSI Approved :: MIT License",
```

### Comparing `pyrippleapi-2024.2.2/src/pyrippleapi/api.py` & `pyrippleapi-2024.5.1/src/pyrippleapi/api.py`

 * *Files identical despite different names*

### Comparing `pyrippleapi-2024.2.2/src/pyrippleapi/generation_asset.py` & `pyrippleapi-2024.5.1/src/pyrippleapi/generation_asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,19 +113,21 @@
         ]
         self._member_expected_annual_generation_units = data[
             "member_expected_annual_generation_units"
         ]
 
     async def get_telemetry(self, data) -> None:
         self._latest_telemetry = data["latest_telemetry"]
-
-        self._latest_telemetry["timestamp"] = datetime.datetime.strptime(
-            self._latest_telemetry["timestamp"],
-            "%Y-%m-%dT%H:%M:%SZ",
-        ).strftime("%Y/%m/%d %H:%M:%S")
+        if "timestamp" in self._latest_telemetry:
+            self._latest_telemetry["timestamp"] = datetime.datetime.strptime(
+                self._latest_telemetry["timestamp"],
+                "%Y-%m-%dT%H:%M:%SZ",
+            ).strftime("%Y/%m/%d %H:%M:%S")
+        else:
+            self._latest_telemetry["timestamp"] = "0001/01/01 00:00:00"
 
     async def get_generation(self, data) -> None:
         for time_scale in [
             "today",
             "yesterday",
             "this_week",
             "last_week",
```

