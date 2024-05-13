# Comparing `tmp/openmeter-1.0.0b73.tar.gz` & `tmp/openmeter-1.0.0b74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmeter-1.0.0b73.tar", max compression
+gzip compressed data, was "openmeter-1.0.0b74.tar", max compression
```

## Comparing `openmeter-1.0.0b73.tar` & `openmeter-1.0.0b74.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1260 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/README.md
--rw-r--r--   0        0        0      837 2024-05-11 09:10:09.645854 openmeter-1.0.0b73/pyproject.toml
--rw-r--r--   0        0        0      702 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/__init__.py
--rw-r--r--   0        0        0     3982 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/_client.py
--rw-r--r--   0        0        0     1807 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/_configuration.py
--rw-r--r--   0        0        0      682 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/_operations/__init__.py
--rw-r--r--   0        0        0   177834 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/_operations/_operations.py
--rw-r--r--   0        0        0     4874 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/_operations/_patch.py
--rw-r--r--   0        0        0      674 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/_patch.py
--rw-r--r--   0        0        0    78873 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/_serialization.py
--rw-r--r--   0        0        0      851 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/_vendor.py
--rw-r--r--   0        0        0      702 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/aio/__init__.py
--rw-r--r--   0        0        0     4100 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/aio/_client.py
--rw-r--r--   0        0        0     1817 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/aio/_configuration.py
--rw-r--r--   0        0        0      682 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/aio/_operations/__init__.py
--rw-r--r--   0        0        0   156104 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/aio/_operations/_operations.py
--rw-r--r--   0        0        0      674 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/aio/_operations/_patch.py
--rw-r--r--   0        0        0      674 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/aio/_patch.py
--rw-r--r--   0        0        0      862 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/aio/_vendor.py
--rw-r--r--   0        0        0       26 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/py.typed
--rw-r--r--   0        0        0     2257 1970-01-01 00:00:00.000000 openmeter-1.0.0b73/PKG-INFO
+-rw-r--r--   0        0        0     1260 2024-05-13 16:24:07.508440 openmeter-1.0.0b74/README.md
+-rw-r--r--   0        0        0      837 2024-05-13 16:25:03.537116 openmeter-1.0.0b74/pyproject.toml
+-rw-r--r--   0        0        0      702 2024-05-13 16:24:07.508440 openmeter-1.0.0b74/src/openmeter/__init__.py
+-rw-r--r--   0        0        0     3982 2024-05-13 16:24:07.508440 openmeter-1.0.0b74/src/openmeter/_client.py
+-rw-r--r--   0        0        0     1807 2024-05-13 16:24:07.508440 openmeter-1.0.0b74/src/openmeter/_configuration.py
+-rw-r--r--   0        0        0      682 2024-05-13 16:24:07.508440 openmeter-1.0.0b74/src/openmeter/_operations/__init__.py
+-rw-r--r--   0        0        0   177834 2024-05-13 16:24:07.508440 openmeter-1.0.0b74/src/openmeter/_operations/_operations.py
+-rw-r--r--   0        0        0     4874 2024-05-13 16:24:07.508440 openmeter-1.0.0b74/src/openmeter/_operations/_patch.py
+-rw-r--r--   0        0        0      674 2024-05-13 16:24:07.508440 openmeter-1.0.0b74/src/openmeter/_patch.py
+-rw-r--r--   0        0        0    78873 2024-05-13 16:24:07.512440 openmeter-1.0.0b74/src/openmeter/_serialization.py
+-rw-r--r--   0        0        0      851 2024-05-13 16:24:07.512440 openmeter-1.0.0b74/src/openmeter/_vendor.py
+-rw-r--r--   0        0        0      702 2024-05-13 16:24:07.512440 openmeter-1.0.0b74/src/openmeter/aio/__init__.py
+-rw-r--r--   0        0        0     4100 2024-05-13 16:24:07.512440 openmeter-1.0.0b74/src/openmeter/aio/_client.py
+-rw-r--r--   0        0        0     1817 2024-05-13 16:24:07.512440 openmeter-1.0.0b74/src/openmeter/aio/_configuration.py
+-rw-r--r--   0        0        0      682 2024-05-13 16:24:07.512440 openmeter-1.0.0b74/src/openmeter/aio/_operations/__init__.py
+-rw-r--r--   0        0        0   156104 2024-05-13 16:24:07.512440 openmeter-1.0.0b74/src/openmeter/aio/_operations/_operations.py
+-rw-r--r--   0        0        0      674 2024-05-13 16:24:07.512440 openmeter-1.0.0b74/src/openmeter/aio/_operations/_patch.py
+-rw-r--r--   0        0        0      674 2024-05-13 16:24:07.512440 openmeter-1.0.0b74/src/openmeter/aio/_patch.py
+-rw-r--r--   0        0        0      862 2024-05-13 16:24:07.512440 openmeter-1.0.0b74/src/openmeter/aio/_vendor.py
+-rw-r--r--   0        0        0       26 2024-05-13 16:24:07.512440 openmeter-1.0.0b74/src/openmeter/py.typed
+-rw-r--r--   0        0        0     2257 1970-01-01 00:00:00.000000 openmeter-1.0.0b74/PKG-INFO
```

### Comparing `openmeter-1.0.0b73/README.md` & `openmeter-1.0.0b74/README.md`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b73/pyproject.toml` & `openmeter-1.0.0b74/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openmeter"
-version = "v1.0.0-beta.73"
+version = "v1.0.0-beta.74"
 description = "Client for OpenMeter: Real-Time and Scalable Usage Metering"
 authors = ["Andras Toth <4157749+tothandras@users.noreply.github.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/openmeter/openmeter"
 homepage = "https://openmeter.io"
 keywords = [
```

### Comparing `openmeter-1.0.0b73/src/openmeter/__init__.py` & `openmeter-1.0.0b74/src/openmeter/__init__.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b73/src/openmeter/_client.py` & `openmeter-1.0.0b74/src/openmeter/_client.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b73/src/openmeter/_configuration.py` & `openmeter-1.0.0b74/src/openmeter/_configuration.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b73/src/openmeter/_operations/__init__.py` & `openmeter-1.0.0b74/src/openmeter/_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b73/src/openmeter/_operations/_operations.py` & `openmeter-1.0.0b74/src/openmeter/_operations/_operations.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b73/src/openmeter/_operations/_patch.py` & `openmeter-1.0.0b74/src/openmeter/_operations/_patch.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b73/src/openmeter/_patch.py` & `openmeter-1.0.0b74/src/openmeter/_patch.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b73/src/openmeter/_serialization.py` & `openmeter-1.0.0b74/src/openmeter/_serialization.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b73/src/openmeter/_vendor.py` & `openmeter-1.0.0b74/src/openmeter/_vendor.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b73/src/openmeter/aio/__init__.py` & `openmeter-1.0.0b74/src/openmeter/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b73/src/openmeter/aio/_client.py` & `openmeter-1.0.0b74/src/openmeter/aio/_client.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b73/src/openmeter/aio/_configuration.py` & `openmeter-1.0.0b74/src/openmeter/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b73/src/openmeter/aio/_operations/__init__.py` & `openmeter-1.0.0b74/src/openmeter/aio/_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b73/src/openmeter/aio/_operations/_operations.py` & `openmeter-1.0.0b74/src/openmeter/aio/_operations/_operations.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b73/src/openmeter/aio/_operations/_patch.py` & `openmeter-1.0.0b74/src/openmeter/aio/_operations/_patch.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b73/src/openmeter/aio/_patch.py` & `openmeter-1.0.0b74/src/openmeter/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b73/src/openmeter/aio/_vendor.py` & `openmeter-1.0.0b74/src/openmeter/aio/_vendor.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b73/PKG-INFO` & `openmeter-1.0.0b74/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmeter
-Version: 1.0.0b73
+Version: 1.0.0b74
 Summary: Client for OpenMeter: Real-Time and Scalable Usage Metering
 Home-page: https://openmeter.io
 License: Apache-2.0
 Keywords: openmeter,api,client,usage,usage-based,metering,ai,aggregation,real-time,billing,cloud
 Author: Andras Toth
 Author-email: 4157749+tothandras@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
```

