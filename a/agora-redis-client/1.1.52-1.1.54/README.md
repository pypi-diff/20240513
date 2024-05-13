# Comparing `tmp/agora_redis_client-1.1.52-py2.py3-none-any.whl.zip` & `tmp/agora_redis_client-1.1.54-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2823 bytes, number of entries: 7
+Zip file size: 2848 bytes, number of entries: 7
 -rw-r--r--  2.0 fat       31 b- defN 23-Jun-14 11:28 agora_redis_client/__init__.py
 -rw-r--r--  2.0 fat     1762 b- defN 23-Sep-06 12:54 agora_redis_client/redis_client.py
--rw-r--r--  2.0 fat       25 b- defN 24-Feb-29 22:54 agora_redis_client/version.py
--rw-r--r--  2.0 fat      131 b- defN 23-Jun-14 11:28 agora_redis_client-1.1.52.dist-info/LICENSE
--rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_redis_client-1.1.52.dist-info/WHEEL
--rw-r--r--  2.0 fat      824 b- defN 16-Jan-01 00:00 agora_redis_client-1.1.52.dist-info/METADATA
--rw-r--r--  2.0 fat      600 b- defN 16-Jan-01 00:00 agora_redis_client-1.1.52.dist-info/RECORD
-7 files, 3472 bytes uncompressed, 1743 bytes compressed:  49.8%
+-rw-r--r--  2.0 fat       25 b- defN 24-May-13 17:00 agora_redis_client/version.py
+-rw-r--r--  2.0 fat      131 b- defN 23-Jun-14 11:28 agora_redis_client-1.1.54.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_redis_client-1.1.54.dist-info/WHEEL
+-rw-r--r--  2.0 fat      877 b- defN 16-Jan-01 00:00 agora_redis_client-1.1.54.dist-info/METADATA
+-rw-r--r--  2.0 fat      600 b- defN 16-Jan-01 00:00 agora_redis_client-1.1.54.dist-info/RECORD
+7 files, 3525 bytes uncompressed, 1768 bytes compressed:  49.8%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: agora_redis_client/redis_client.py
 Comment: 
 
 Filename: agora_redis_client/version.py
 Comment: 
 
-Filename: agora_redis_client-1.1.52.dist-info/LICENSE
+Filename: agora_redis_client-1.1.54.dist-info/LICENSE
 Comment: 
 
-Filename: agora_redis_client-1.1.52.dist-info/WHEEL
+Filename: agora_redis_client-1.1.54.dist-info/WHEEL
 Comment: 
 
-Filename: agora_redis_client-1.1.52.dist-info/METADATA
+Filename: agora_redis_client-1.1.54.dist-info/METADATA
 Comment: 
 
-Filename: agora_redis_client-1.1.52.dist-info/RECORD
+Filename: agora_redis_client-1.1.54.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agora_redis_client/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.52'
+__version__ = '1.1.54'
```

## Comparing `agora_redis_client-1.1.52.dist-info/METADATA` & `agora_redis_client-1.1.54.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: agora_redis_client
-Version: 1.1.52
+Version: 1.1.54
 Summary: Redis Client for the Agora Edge Apps SDK 2.0 (Python)
 Author-email: AgoraIoT <agoraiot@slb.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: agora_logging == 1.1.52
-Requires-Dist: agora_config == 1.1.52
+Requires-Dist: agora_logging == 1.1.54
+Requires-Dist: agora_config == 1.1.54
 Requires-Dist: redis
 Project-URL: Home, https://slb-edge.github.io
 
 
 # agora_redisclient
 
 This package is the Redis Client for the Agora Edge Apps SDK (Python) developed by SLB.
 
 Use this SDK to construct an edge application, and then containerize it for the running on the edge with AgoraIoT.  Documentation on using the entire SDK can be found at: [AgoraIoT SDK Documentation](https://slb-edge.github.io).
 
 ## Release Notes
 
+### v1.1.53
+- Make versions of all modules the same
+
 ### v1.0.26
 
 - Initial Version of Redis Client
```

## Comparing `agora_redis_client-1.1.52.dist-info/RECORD` & `agora_redis_client-1.1.54.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 agora_redis_client/__init__.py,sha256=nIxsBty2jHDz3mqsvyOPRhUZoo6FtNNvfkNph7C4F4U,31
 agora_redis_client/redis_client.py,sha256=S7Zp_dZwL5M3914b0dLflTMTbidb5bYMyfJnkD0UHQ4,1762
-agora_redis_client/version.py,sha256=DJOzku5VtxZPW8oVz4bIbxGE4aoRSn3D3hyoQKwWpUc,25
-agora_redis_client-1.1.52.dist-info/LICENSE,sha256=2RSWN0z_ADMOpyELJ0aJpy2UKIuZOOdYq0PpxyllwlA,131
-agora_redis_client-1.1.52.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
-agora_redis_client-1.1.52.dist-info/METADATA,sha256=h0Ha8iHFDykyd68SzYSYx_FGM7ovr9zS721dTHm_zjs,824
-agora_redis_client-1.1.52.dist-info/RECORD,,
+agora_redis_client/version.py,sha256=4WdBeM0yBfBzaTQBed8t9GEwEa64wGAS3T9tdCg7Q-g,25
+agora_redis_client-1.1.54.dist-info/LICENSE,sha256=2RSWN0z_ADMOpyELJ0aJpy2UKIuZOOdYq0PpxyllwlA,131
+agora_redis_client-1.1.54.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
+agora_redis_client-1.1.54.dist-info/METADATA,sha256=qOLlOwaWBGGn08cZ9MR1Q6GH9mj3vr2cLP698sfA_Bo,877
+agora_redis_client-1.1.54.dist-info/RECORD,,
```

