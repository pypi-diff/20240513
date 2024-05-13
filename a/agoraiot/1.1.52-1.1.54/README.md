# Comparing `tmp/agoraiot-1.1.52-py2.py3-none-any.whl.zip` & `tmp/agoraiot-1.1.54-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2045 bytes, number of entries: 6
--rw-r--r--  2.0 fat      349 b- defN 24-Feb-12 16:40 agoraiot/__init__.py
--rw-r--r--  2.0 fat       25 b- defN 24-Feb-29 22:54 agoraiot/version.py
--rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agoraiot-1.1.52.dist-info/LICENSE
--rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agoraiot-1.1.52.dist-info/WHEEL
--rw-r--r--  2.0 fat      974 b- defN 16-Jan-01 00:00 agoraiot-1.1.52.dist-info/METADATA
--rw-r--r--  2.0 fat      450 b- defN 16-Jan-01 00:00 agoraiot-1.1.52.dist-info/RECORD
-6 files, 2031 bytes uncompressed, 1229 bytes compressed:  39.5%
+Zip file size: 2095 bytes, number of entries: 6
+-rw-r--r--  2.0 fat      395 b- defN 24-May-13 16:50 agoraiot/__init__.py
+-rw-r--r--  2.0 fat       25 b- defN 24-May-13 17:00 agoraiot/version.py
+-rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agoraiot-1.1.54.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agoraiot-1.1.54.dist-info/WHEEL
+-rw-r--r--  2.0 fat     1061 b- defN 16-Jan-01 00:00 agoraiot-1.1.54.dist-info/METADATA
+-rw-r--r--  2.0 fat      451 b- defN 16-Jan-01 00:00 agoraiot-1.1.54.dist-info/RECORD
+6 files, 2165 bytes uncompressed, 1279 bytes compressed:  40.9%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: agoraiot/__init__.py
 Comment: 
 
 Filename: agoraiot/version.py
 Comment: 
 
-Filename: agoraiot-1.1.52.dist-info/LICENSE
+Filename: agoraiot-1.1.54.dist-info/LICENSE
 Comment: 
 
-Filename: agoraiot-1.1.52.dist-info/WHEEL
+Filename: agoraiot-1.1.54.dist-info/WHEEL
 Comment: 
 
-Filename: agoraiot-1.1.52.dist-info/METADATA
+Filename: agoraiot-1.1.54.dist-info/METADATA
 Comment: 
 
-Filename: agoraiot-1.1.52.dist-info/RECORD
+Filename: agoraiot-1.1.54.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agoraiot/__init__.py

```diff
@@ -1,6 +1,7 @@
 from agora_busclient import IoDataReportMsg, IoPoint, RequestMsg, \
       bus_client, IoPoint, IoDeviceData, IoTagDataDict, MessageHeader, EventMsg, MediaData, WorkFlow
 from agora_utils import AgoraTimeStamp, UTCDateTime
 from agora_config import config, DictOfDict
 from agora_logging import logger, LogLevel
-from agora_redis_client import redis
+from agora_redis_client import redis
+from agora_twin_property import TwinProperty
```

## agoraiot/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.52'
+__version__ = '1.1.54'
```

## Comparing `agoraiot-1.1.52.dist-info/METADATA` & `agoraiot-1.1.54.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: agoraiot
-Version: 1.1.52
+Version: 1.1.54
 Summary: AgoraIoT Python Libraries
 Author-email: AgoraIoT <agoraiot@slb.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: agora_logging == 1.1.52
-Requires-Dist: agora_busclient == 1.1.52
-Requires-Dist: agora_config == 1.1.52
-Requires-Dist: agora_redis_client == 1.1.52
-Requires-Dist: agora_utils == 1.1.52
+Requires-Dist: agora_logging == 1.1.54
+Requires-Dist: agora_busclient == 1.1.54
+Requires-Dist: agora_config == 1.1.54
+Requires-Dist: agora_redis_client == 1.1.54
+Requires-Dist: agora_twin_property == 1.1.54
+Requires-Dist: agora_utils == 1.1.54
 Project-URL: Documentation, https://agoraiot.github.io
 Project-URL: Home, https://www.agoraiot.com
 
 # agoraiot
 
 This primary package for the entire Agora Edge Apps SDK (Python) developed by SLB.
 
 Use this SDK to construct an edge application, and then containerize it for the running on the edge with AgoraIoT.  Documentation on using the entire SDK can be found at: [AgoraIoT SDK Documentation](https://slb-edge.github.io).
 
 ## Release Notes
 
+### v1.1.53
+- Added Twin Property Module
+
 ### v1.0.18
 
 - Make versions of all modules the same
 
 ### v1.0.7 - Beta
 
 - Initial test release.
```

