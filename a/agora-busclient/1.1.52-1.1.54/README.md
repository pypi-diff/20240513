# Comparing `tmp/agora_busclient-1.1.52-py2.py3-none-any.whl.zip` & `tmp/agora_busclient-1.1.54-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 19044 bytes, number of entries: 22
+Zip file size: 19053 bytes, number of entries: 22
 -rw-r--r--  2.0 fat      261 b- defN 23-Jul-28 12:34 agora_busclient/__init__.py
 -rw-r--r--  2.0 fat     5679 b- defN 24-Jan-17 19:50 agora_busclient/base_mqtt_client.py
 -rw-r--r--  2.0 fat     5008 b- defN 23-Nov-07 10:50 agora_busclient/bus_client.py
 -rw-r--r--  2.0 fat     4771 b- defN 23-Sep-06 12:54 agora_busclient/message_queue.py
--rw-r--r--  2.0 fat     5135 b- defN 24-Feb-20 13:41 agora_busclient/mqtt_client.py
--rw-r--r--  2.0 fat       25 b- defN 24-Feb-29 22:54 agora_busclient/version.py
+-rw-r--r--  2.0 fat     5135 b- defN 24-Apr-23 15:18 agora_busclient/mqtt_client.py
+-rw-r--r--  2.0 fat       25 b- defN 24-May-13 17:00 agora_busclient/version.py
 -rw-r--r--  2.0 fat      432 b- defN 23-Jul-10 22:39 agora_busclient/messages/__init__.py
 -rw-r--r--  2.0 fat     2739 b- defN 23-Nov-07 10:50 agora_busclient/messages/event_msg.py
 -rw-r--r--  2.0 fat      763 b- defN 23-Nov-07 10:50 agora_busclient/messages/io_device_data.py
 -rw-r--r--  2.0 fat     1564 b- defN 23-Nov-07 10:50 agora_busclient/messages/io_point.py
 -rw-r--r--  2.0 fat     1487 b- defN 23-Nov-07 10:50 agora_busclient/messages/io_tag_data_dict.py
 -rw-r--r--  2.0 fat     3183 b- defN 23-Nov-07 10:50 agora_busclient/messages/iodatareport_message.py
 -rw-r--r--  2.0 fat     2367 b- defN 23-Nov-07 10:50 agora_busclient/messages/media_data.py
 -rw-r--r--  2.0 fat     1863 b- defN 23-Nov-07 10:50 agora_busclient/messages/message_header.py
--rw-r--r--  2.0 fat     7634 b- defN 24-Feb-29 22:45 agora_busclient/messages/msg_decoder.py
+-rw-r--r--  2.0 fat     7634 b- defN 24-Apr-23 15:18 agora_busclient/messages/msg_decoder.py
 -rw-r--r--  2.0 fat     3919 b- defN 24-Feb-29 22:36 agora_busclient/messages/msg_encoder.py
 -rw-r--r--  2.0 fat     1560 b- defN 23-Nov-07 10:50 agora_busclient/messages/request_msg.py
 -rw-r--r--  2.0 fat      558 b- defN 23-Nov-07 10:50 agora_busclient/messages/work_flow.py
--rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_busclient-1.1.52.dist-info/LICENSE
--rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_busclient-1.1.52.dist-info/WHEEL
--rw-r--r--  2.0 fat     1536 b- defN 16-Jan-01 00:00 agora_busclient-1.1.52.dist-info/METADATA
--rw-r--r--  2.0 fat     2005 b- defN 16-Jan-01 00:00 agora_busclient-1.1.52.dist-info/RECORD
-22 files, 52722 bytes uncompressed, 15722 bytes compressed:  70.2%
+-rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_busclient-1.1.54.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_busclient-1.1.54.dist-info/WHEEL
+-rw-r--r--  2.0 fat     1589 b- defN 16-Jan-01 00:00 agora_busclient-1.1.54.dist-info/METADATA
+-rw-r--r--  2.0 fat     2005 b- defN 16-Jan-01 00:00 agora_busclient-1.1.54.dist-info/RECORD
+22 files, 52775 bytes uncompressed, 15731 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -48,20 +48,20 @@
 
 Filename: agora_busclient/messages/request_msg.py
 Comment: 
 
 Filename: agora_busclient/messages/work_flow.py
 Comment: 
 
-Filename: agora_busclient-1.1.52.dist-info/LICENSE
+Filename: agora_busclient-1.1.54.dist-info/LICENSE
 Comment: 
 
-Filename: agora_busclient-1.1.52.dist-info/WHEEL
+Filename: agora_busclient-1.1.54.dist-info/WHEEL
 Comment: 
 
-Filename: agora_busclient-1.1.52.dist-info/METADATA
+Filename: agora_busclient-1.1.54.dist-info/METADATA
 Comment: 
 
-Filename: agora_busclient-1.1.52.dist-info/RECORD
+Filename: agora_busclient-1.1.54.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agora_busclient/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.52'
+__version__ = '1.1.54'
```

## Comparing `agora_busclient-1.1.52.dist-info/METADATA` & `agora_busclient-1.1.54.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: agora_busclient
-Version: 1.1.52
+Version: 1.1.54
 Summary: Bus Client libraries for the Agora Edge Apps SDK 2.0 (Python)
 Author-email: AgoraIoT <agoraiot@slb.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: agora_logging == 1.1.52
-Requires-Dist: agora_config == 1.1.52
-Requires-Dist: agora_utils == 1.1.52
+Requires-Dist: agora_logging == 1.1.54
+Requires-Dist: agora_config == 1.1.54
+Requires-Dist: agora_utils == 1.1.54
 Requires-Dist: paho-mqtt
 Project-URL: Home, https://agoraiot.github.io
 
 # agora_busclient
 
  This package is the Bus Client library for the Agora Edge Apps SDK (Python) developed by SLB.
 
 Use this SDK to construct an edge application, and then containerize it for the running on the edge with AgoraIoT.  Documentation on using the entire SDK can be found at: [AgoraIoT SDK Documentation](https://slb-edge.github.io).
 
 ## Release Notes
 
+### v1.1.53
+- Make versions of all modules the same
+
 ### v 1.1.51
 
 - Fix for BREAKING change for paho.mqtt.pythonv2.0.0 Added callback_api_version=mqtt.CallbackAPIVersion.VERSION1 as the first argument to Client()
 ### v 1.1.50
 
 - Fix Event Message Schema with MediaDataRef & Workflow types naming convention
```

## Comparing `agora_busclient-1.1.52.dist-info/RECORD` & `agora_busclient-1.1.54.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 agora_busclient/__init__.py,sha256=u5C1uUUYJLFPg8rdFdLLUBkNZjPznbShJPz_6k7T8nc,261
 agora_busclient/base_mqtt_client.py,sha256=rPTEcLbUHn4mS_RxYe5ehyTjxMgiIyK2wXACZXw1FEs,5679
 agora_busclient/bus_client.py,sha256=9bsoto9CsoZ-ayUur8pOtf-LjJdliyTX58xFz5N5uTg,5008
 agora_busclient/message_queue.py,sha256=b1h2-IfpFueevBn1JLnvwbgEDFy8j3ZDlh7FnZwzPJs,4771
 agora_busclient/mqtt_client.py,sha256=ljLCGTLzEqXRA7bjYjaO_tyyLzePaJKhaV9Ynam_nhs,5135
-agora_busclient/version.py,sha256=DJOzku5VtxZPW8oVz4bIbxGE4aoRSn3D3hyoQKwWpUc,25
+agora_busclient/version.py,sha256=4WdBeM0yBfBzaTQBed8t9GEwEa64wGAS3T9tdCg7Q-g,25
 agora_busclient/messages/__init__.py,sha256=SXI28GSrnaOZxDpXYqH4emANTRWlGDjvKVsClgtQGqw,432
 agora_busclient/messages/event_msg.py,sha256=Xl04sJn83Ip_o_2ScfhKt3sUKcVADfLYEXJ-KRZx6z4,2739
 agora_busclient/messages/io_device_data.py,sha256=H6eVOV6u2QoOn7vadHMCeZlFtKtDBaxNINvoQlQ7R2g,763
 agora_busclient/messages/io_point.py,sha256=HoQJ8EdKm-WwJbTtFSRPZQfYcKIEDtwIGI_NeAX0TeA,1564
 agora_busclient/messages/io_tag_data_dict.py,sha256=iupajzyYhlEsGZLFvoS-oCkzNR6R51ziZmuMOQGSAKk,1487
 agora_busclient/messages/iodatareport_message.py,sha256=1pAUGwdw25Kz4nSO0Xr6BfW5GpLcKTOIJQSxiynqpi8,3183
 agora_busclient/messages/media_data.py,sha256=311C7O9Ag0bUtpfB6H3g6LcEyzQBEnEHjmYLxMiWWTo,2367
 agora_busclient/messages/message_header.py,sha256=L3pE3nF8LmAnf4KoE97Hbog3pONAbwnfJ009A3n5ul4,1863
 agora_busclient/messages/msg_decoder.py,sha256=LuHNuy7y3G4GZTTlwsQpSbDLhNW5-ZSUjysNDvwDFNk,7634
 agora_busclient/messages/msg_encoder.py,sha256=UYYOjcrVwJP2qJnehqYkfPid-1hHleZbeEKikKrXXOg,3919
 agora_busclient/messages/request_msg.py,sha256=HFfL4p2s4L9EHRFo9e467xLVvbUuwk4qucY4SIWAUHo,1560
 agora_busclient/messages/work_flow.py,sha256=78OkTtkC_vSy_40WYYnz0qe22ay2jG7ppHm6B-4oCjA,558
-agora_busclient-1.1.52.dist-info/LICENSE,sha256=R-TdODMyhPUhIFgVHS3Y973VNriIq35ZLKQ6iTN2ySo,134
-agora_busclient-1.1.52.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
-agora_busclient-1.1.52.dist-info/METADATA,sha256=dE_dd7t4qr0SatmTVEO1wAWT3qJXq__YVGwZFEj6ErE,1536
-agora_busclient-1.1.52.dist-info/RECORD,,
+agora_busclient-1.1.54.dist-info/LICENSE,sha256=R-TdODMyhPUhIFgVHS3Y973VNriIq35ZLKQ6iTN2ySo,134
+agora_busclient-1.1.54.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
+agora_busclient-1.1.54.dist-info/METADATA,sha256=mONEdWtLkJpT0MyqP54q5Ey-7uH0feSEe8DapyBLWYY,1589
+agora_busclient-1.1.54.dist-info/RECORD,,
```

