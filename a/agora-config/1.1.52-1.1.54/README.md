# Comparing `tmp/agora_config-1.1.52-py2.py3-none-any.whl.zip` & `tmp/agora_config-1.1.54-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 9217 bytes, number of entries: 13
+Zip file size: 9227 bytes, number of entries: 13
 -rw-r--r--  2.0 fat       70 b- defN 23-Sep-06 12:54 agora_config/__init__.py
--rw-r--r--  2.0 fat     7203 b- defN 24-Feb-12 16:40 agora_config/agora_config.py
+-rw-r--r--  2.0 fat     7203 b- defN 24-Apr-23 15:18 agora_config/agora_config.py
 -rw-r--r--  2.0 fat      745 b- defN 23-Sep-06 12:54 agora_config/command_line_provider.py
 -rw-r--r--  2.0 fat     2600 b- defN 23-Sep-06 12:54 agora_config/dict_of_dict.py
 -rw-r--r--  2.0 fat      646 b- defN 23-Sep-06 12:54 agora_config/environment_variable_provider.py
 -rw-r--r--  2.0 fat     3644 b- defN 23-Sep-06 12:54 agora_config/file_key_provider.py
 -rw-r--r--  2.0 fat     2418 b- defN 23-Sep-06 12:54 agora_config/file_provider.py
 -rw-r--r--  2.0 fat     1099 b- defN 23-Sep-06 12:54 agora_config/last_value_callbacks.py
--rw-r--r--  2.0 fat       25 b- defN 24-Feb-29 22:54 agora_config/version.py
--rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_config-1.1.52.dist-info/LICENSE
--rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_config-1.1.52.dist-info/WHEEL
--rw-r--r--  2.0 fat     1847 b- defN 16-Jan-01 00:00 agora_config-1.1.52.dist-info/METADATA
--rw-r--r--  2.0 fat     1107 b- defN 16-Jan-01 00:00 agora_config-1.1.52.dist-info/RECORD
-13 files, 21637 bytes uncompressed, 7349 bytes compressed:  66.0%
+-rw-r--r--  2.0 fat       25 b- defN 24-May-13 17:00 agora_config/version.py
+-rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_config-1.1.54.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_config-1.1.54.dist-info/WHEEL
+-rw-r--r--  2.0 fat     1900 b- defN 16-Jan-01 00:00 agora_config-1.1.54.dist-info/METADATA
+-rw-r--r--  2.0 fat     1107 b- defN 16-Jan-01 00:00 agora_config-1.1.54.dist-info/RECORD
+13 files, 21690 bytes uncompressed, 7359 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: agora_config/last_value_callbacks.py
 Comment: 
 
 Filename: agora_config/version.py
 Comment: 
 
-Filename: agora_config-1.1.52.dist-info/LICENSE
+Filename: agora_config-1.1.54.dist-info/LICENSE
 Comment: 
 
-Filename: agora_config-1.1.52.dist-info/WHEEL
+Filename: agora_config-1.1.54.dist-info/WHEEL
 Comment: 
 
-Filename: agora_config-1.1.52.dist-info/METADATA
+Filename: agora_config-1.1.54.dist-info/METADATA
 Comment: 
 
-Filename: agora_config-1.1.52.dist-info/RECORD
+Filename: agora_config-1.1.54.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agora_config/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.52'
+__version__ = '1.1.54'
```

## Comparing `agora_config-1.1.52.dist-info/METADATA` & `agora_config-1.1.54.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: agora_config
-Version: 1.1.52
+Version: 1.1.54
 Summary: Configuration libraries for the Agora Edge Apps SDK 2.0 (Python)
 Author-email: AgoraIoT <agoraiot@slb.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: agora_logging == 1.1.52
+Requires-Dist: agora_logging == 1.1.54
 Project-URL: Home, https://agoraiot.github.io
 
 # agora_config
 
 This package is the Configuration library for the Agora Edge Apps SDK (Python) developed by SLB.
 
 Use this SDK to construct an edge application, and then containerize it for the running on the edge with AgoraIoT.  Documentation on using the entire SDK can be found at: [AgoraIoT SDK Documentation](https://slb-edge.github.io).
 
 ## Release Notes
 
+### v1.1.53
+- Make versions of all modules the same
+
 ### v1.0.26
 - Deprecate config_overrides and config_defaults in favor or config.overrides and config.defaults to make more parallel to .NET SDK.  Update all associated documentation.
 
 
 ### v1.0.23
 - Remove config default value "DEVICE_ID"
 - Set default config value "GATEWAY_ID" to be "IOTEDGE_DEVICEID" env var if it is available.
```

## Comparing `agora_config-1.1.52.dist-info/RECORD` & `agora_config-1.1.54.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 agora_config/agora_config.py,sha256=RoVr0AlxIGOCpwD7HAPB_d2SRLakeSFjZVyU7dg5kpU,7203
 agora_config/command_line_provider.py,sha256=ufrsQ-227QaO4oyjnxOR1HZWbYc9J78iu_OClhPBQ0A,745
 agora_config/dict_of_dict.py,sha256=2TDOYcb6bYn2wGkeRDENwNf8ylEJPbltQNuQCPg7m_o,2600
 agora_config/environment_variable_provider.py,sha256=V86CVODvwLKqetl6V7qwSLrnAGtYe7H__6v59lU3Lfk,646
 agora_config/file_key_provider.py,sha256=_FcCcc_nVnQlpHeORofOYVidPWHvkL_j_O6eyiv5d2Q,3644
 agora_config/file_provider.py,sha256=C859Nok0wLO3lH33xADH-1n7XYAu0VTcp1dEt3TZufs,2418
 agora_config/last_value_callbacks.py,sha256=IvCr6BVNMu8q9rqfmfeOy4I4hiZ73LC4epORXYzS3R0,1099
-agora_config/version.py,sha256=DJOzku5VtxZPW8oVz4bIbxGE4aoRSn3D3hyoQKwWpUc,25
-agora_config-1.1.52.dist-info/LICENSE,sha256=R-TdODMyhPUhIFgVHS3Y973VNriIq35ZLKQ6iTN2ySo,134
-agora_config-1.1.52.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
-agora_config-1.1.52.dist-info/METADATA,sha256=vfwzNvpm0G829x32oLA3xFC1KfHHR3DS4SO_jgQyi9Q,1847
-agora_config-1.1.52.dist-info/RECORD,,
+agora_config/version.py,sha256=4WdBeM0yBfBzaTQBed8t9GEwEa64wGAS3T9tdCg7Q-g,25
+agora_config-1.1.54.dist-info/LICENSE,sha256=R-TdODMyhPUhIFgVHS3Y973VNriIq35ZLKQ6iTN2ySo,134
+agora_config-1.1.54.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
+agora_config-1.1.54.dist-info/METADATA,sha256=DDRwhevXCdoLuSLprCrhjDhGGG5VOS74UYLh_O6TwHU,1900
+agora_config-1.1.54.dist-info/RECORD,,
```

