# Comparing `tmp/agora_utils-1.1.52-py2.py3-none-any.whl.zip` & `tmp/agora_utils-1.1.54-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 2562 bytes, number of entries: 8
+Zip file size: 2569 bytes, number of entries: 8
 -rw-r--r--  2.0 fat       75 b- defN 23-May-12 13:38 agora_utils/__init__.py
 -rw-r--r--  2.0 fat       23 b- defN 23-May-12 13:38 agora_utils/_version.py
 -rw-r--r--  2.0 fat      521 b- defN 23-Jul-27 17:24 agora_utils/agora_time.py
--rw-r--r--  2.0 fat       25 b- defN 24-Feb-29 22:54 agora_utils/version.py
--rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_utils-1.1.52.dist-info/LICENSE
--rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_utils-1.1.52.dist-info/WHEEL
--rw-r--r--  2.0 fat      880 b- defN 16-Jan-01 00:00 agora_utils-1.1.52.dist-info/METADATA
--rw-r--r--  2.0 fat      626 b- defN 16-Jan-01 00:00 agora_utils-1.1.52.dist-info/RECORD
-8 files, 2383 bytes uncompressed, 1462 bytes compressed:  38.6%
+-rw-r--r--  2.0 fat       25 b- defN 24-May-13 17:00 agora_utils/version.py
+-rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_utils-1.1.54.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_utils-1.1.54.dist-info/WHEEL
+-rw-r--r--  2.0 fat      933 b- defN 16-Jan-01 00:00 agora_utils-1.1.54.dist-info/METADATA
+-rw-r--r--  2.0 fat      626 b- defN 16-Jan-01 00:00 agora_utils-1.1.54.dist-info/RECORD
+8 files, 2436 bytes uncompressed, 1469 bytes compressed:  39.7%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: agora_utils/agora_time.py
 Comment: 
 
 Filename: agora_utils/version.py
 Comment: 
 
-Filename: agora_utils-1.1.52.dist-info/LICENSE
+Filename: agora_utils-1.1.54.dist-info/LICENSE
 Comment: 
 
-Filename: agora_utils-1.1.52.dist-info/WHEEL
+Filename: agora_utils-1.1.54.dist-info/WHEEL
 Comment: 
 
-Filename: agora_utils-1.1.52.dist-info/METADATA
+Filename: agora_utils-1.1.54.dist-info/METADATA
 Comment: 
 
-Filename: agora_utils-1.1.52.dist-info/RECORD
+Filename: agora_utils-1.1.54.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agora_utils/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.52'
+__version__ = '1.1.54'
```

## Comparing `agora_utils-1.1.52.dist-info/METADATA` & `agora_utils-1.1.54.dist-info/METADATA`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agora_utils
-Version: 1.1.52
+Version: 1.1.54
 Summary: Utilities libraries for the Agora Edge Apps SDK 2.0 (Python)
 Author-email: AgoraIoT <agoraiot@slb.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: Home, https://agoraiot.github.io
 
 
@@ -12,14 +12,17 @@
 
 This package is the Utilities library for the Agora Edge Apps SDK (Python) developed by SLB.
 
 Use this SDK to construct an edge application, and then containerize it for the running on the edge with AgoraIoT.  Documentation on using the entire SDK can be found at: [AgoraIoT SDK Documentation](https://slb-edge.github.io).
 
 ## Release Notes
 
+### v1.1.53
+- Make versions of all modules the same
+
 ### v1.0.18
 
 - Make versions of all modules all the same
 - Add ability to Mock (AEA2:BusClient:Mock (True/False)) the BusClient
 - Fix issue with subscriptions
 
 ### v1.0.7 - Beta
```

## Comparing `agora_utils-1.1.52.dist-info/RECORD` & `agora_utils-1.1.54.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 agora_utils/__init__.py,sha256=bMi6zdciwSmg3ZDZCOfzQCUHMYaxcHk1GvAL_i2zh0s,75
 agora_utils/_version.py,sha256=kwEyWwKLIIqYSnkf5eXgPtRgw9Bz51riSupwtvDpJMA,23
 agora_utils/agora_time.py,sha256=3vMrPf5MGRQdXqqXxLEwcAv-jH1jcctgeEU-Nbo0d4Q,521
-agora_utils/version.py,sha256=DJOzku5VtxZPW8oVz4bIbxGE4aoRSn3D3hyoQKwWpUc,25
-agora_utils-1.1.52.dist-info/LICENSE,sha256=R-TdODMyhPUhIFgVHS3Y973VNriIq35ZLKQ6iTN2ySo,134
-agora_utils-1.1.52.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
-agora_utils-1.1.52.dist-info/METADATA,sha256=X0vW-5AcXN41Cjb_uc090a-i4cggt8utsHpi47SPbBc,880
-agora_utils-1.1.52.dist-info/RECORD,,
+agora_utils/version.py,sha256=4WdBeM0yBfBzaTQBed8t9GEwEa64wGAS3T9tdCg7Q-g,25
+agora_utils-1.1.54.dist-info/LICENSE,sha256=R-TdODMyhPUhIFgVHS3Y973VNriIq35ZLKQ6iTN2ySo,134
+agora_utils-1.1.54.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
+agora_utils-1.1.54.dist-info/METADATA,sha256=LPxTdcoCazTnWE7-KgJyLzeTX2Up1TV7oNNdILQBq5g,933
+agora_utils-1.1.54.dist-info/RECORD,,
```

