# Comparing `tmp/omegi_python_instrumentation-0.0.6.tar.gz` & `tmp/omegi_python_instrumentation-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omegi_python_instrumentation-0.0.6.tar", last modified: Tue May  7 07:37:33 2024, max compression
+gzip compressed data, was "omegi_python_instrumentation-0.0.7.tar", last modified: Mon May 13 04:24:35 2024, max compression
```

## Comparing `omegi_python_instrumentation-0.0.6.tar` & `omegi_python_instrumentation-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-07 07:37:33.659923 omegi_python_instrumentation-0.0.6/
--rw-r--r--   0 whisenlantern   (501) staff       (20)       13 2024-05-07 06:22:05.000000 omegi_python_instrumentation-0.0.6/LICENSE.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2065 2024-05-07 07:37:33.659713 omegi_python_instrumentation-0.0.6/PKG-INFO
--rw-r--r--   0 whisenlantern   (501) staff       (20)       44 2024-05-07 06:21:19.000000 omegi_python_instrumentation-0.0.6/README.md
--rw-r--r--   0 whisenlantern   (501) staff       (20)      103 2024-05-07 06:17:54.000000 omegi_python_instrumentation-0.0.6/pyproject.toml
--rw-r--r--   0 whisenlantern   (501) staff       (20)       38 2024-05-07 07:37:33.659966 omegi_python_instrumentation-0.0.6/setup.cfg
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2167 2024-05-07 07:37:09.000000 omegi_python_instrumentation-0.0.6/setup.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-07 07:37:33.657138 omegi_python_instrumentation-0.0.6/src/
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-07 07:37:33.658587 omegi_python_instrumentation-0.0.6/src/omegi/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2809 2024-05-06 19:38:23.000000 omegi_python_instrumentation-0.0.6/src/omegi/KafkaSpanExporter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1350 2024-05-07 07:10:24.000000 omegi_python_instrumentation-0.0.6/src/omegi/OmegHandler.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2242 2024-05-07 07:36:46.000000 omegi_python_instrumentation-0.0.6/src/omegi/OmegiTracer.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-07 06:14:19.000000 omegi_python_instrumentation-0.0.6/src/omegi/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-07 07:37:33.659415 omegi_python_instrumentation-0.0.6/src/omegi_python_instrumentation.egg-info/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2065 2024-05-07 07:37:33.000000 omegi_python_instrumentation-0.0.6/src/omegi_python_instrumentation.egg-info/PKG-INFO
--rw-r--r--   0 whisenlantern   (501) staff       (20)      427 2024-05-07 07:37:33.000000 omegi_python_instrumentation-0.0.6/src/omegi_python_instrumentation.egg-info/SOURCES.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)        1 2024-05-07 07:37:33.000000 omegi_python_instrumentation-0.0.6/src/omegi_python_instrumentation.egg-info/dependency_links.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)      840 2024-05-07 07:37:33.000000 omegi_python_instrumentation-0.0.6/src/omegi_python_instrumentation.egg-info/requires.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)        6 2024-05-07 07:37:33.000000 omegi_python_instrumentation-0.0.6/src/omegi_python_instrumentation.egg-info/top_level.txt
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-13 04:24:35.441855 omegi_python_instrumentation-0.0.7/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       13 2024-05-07 06:22:05.000000 omegi_python_instrumentation-0.0.7/LICENSE.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2065 2024-05-13 04:24:35.441666 omegi_python_instrumentation-0.0.7/PKG-INFO
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       44 2024-05-07 06:21:19.000000 omegi_python_instrumentation-0.0.7/README.md
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      103 2024-05-07 06:17:54.000000 omegi_python_instrumentation-0.0.7/pyproject.toml
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       38 2024-05-13 04:24:35.441904 omegi_python_instrumentation-0.0.7/setup.cfg
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2318 2024-05-13 04:22:13.000000 omegi_python_instrumentation-0.0.7/setup.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-13 04:24:35.438914 omegi_python_instrumentation-0.0.7/src/
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-13 04:24:35.440402 omegi_python_instrumentation-0.0.7/src/omegi/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1861 2024-05-12 16:36:10.000000 omegi_python_instrumentation-0.0.7/src/omegi/OmegiDecorator.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     3085 2024-05-13 04:12:52.000000 omegi_python_instrumentation-0.0.7/src/omegi/OmegiSpanExporter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2104 2024-05-13 03:46:40.000000 omegi_python_instrumentation-0.0.7/src/omegi/OmegiUtil.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      592 2024-05-13 04:18:09.000000 omegi_python_instrumentation-0.0.7/src/omegi/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-13 04:24:35.441383 omegi_python_instrumentation-0.0.7/src/omegi_python_instrumentation.egg-info/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2065 2024-05-13 04:24:35.000000 omegi_python_instrumentation-0.0.7/src/omegi_python_instrumentation.egg-info/PKG-INFO
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      487 2024-05-13 04:24:35.000000 omegi_python_instrumentation-0.0.7/src/omegi_python_instrumentation.egg-info/SOURCES.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        1 2024-05-13 04:24:35.000000 omegi_python_instrumentation-0.0.7/src/omegi_python_instrumentation.egg-info/dependency_links.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       90 2024-05-13 04:24:35.000000 omegi_python_instrumentation-0.0.7/src/omegi_python_instrumentation.egg-info/entry_points.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      840 2024-05-13 04:24:35.000000 omegi_python_instrumentation-0.0.7/src/omegi_python_instrumentation.egg-info/requires.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        6 2024-05-13 04:24:35.000000 omegi_python_instrumentation-0.0.7/src/omegi_python_instrumentation.egg-info/top_level.txt
```

### Comparing `omegi_python_instrumentation-0.0.6/PKG-INFO` & `omegi_python_instrumentation-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegi-python-instrumentation
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python Instrumentation for Automatic Error Logging
 Home-page: https://github.com/TeamOmegi/Instrumentation-Python
 Author: Omegi
 Author-email: canon1107@naver.com
 Project-URL: Source Code, https://github.com/TeamOmegi/Instrumentation-Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `omegi_python_instrumentation-0.0.6/setup.py` & `omegi_python_instrumentation-0.0.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="omegi-python-instrumentation",
-    version="0.0.6",
+    version="0.0.7",
     author="Omegi",
     author_email="canon1107@naver.com",
     description="Python Instrumentation for Automatic Error Logging",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TeamOmegi/Instrumentation-Python",
     project_urls={
@@ -65,8 +65,13 @@
         "uvicorn==0.29.0",
         "uvloop==0.19.0",
         "watchfiles==0.21.0",
         "websockets==12.0",
         "wrapt==1.16.0",
         "zipp==3.18.1",
     ],
+    entry_points={
+        "opentelemetry_traces_exporter": [
+            "omegi_kafka = omegi_kafka_exporter:OmegiKafkaSpanExporter"
+        ],
+    }
 )
```

### Comparing `omegi_python_instrumentation-0.0.6/src/omegi/KafkaSpanExporter.py` & `omegi_python_instrumentation-0.0.7/src/omegi/OmegiSpanExporter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 import json
+import os
 import re
 from typing import Sequence
 
 from kafka import KafkaProducer
 from opentelemetry.sdk.trace.export import SpanExporter
 from opentelemetry.trace import Span
 
 
-class KafkaSpanExporter(SpanExporter):
-    def __init__(self, kafka_config, topic, token):
-        self.producer = KafkaProducer(bootstrap_servers=kafka_config)
+class OmegiKafkaSpanExporter(SpanExporter):
+    def __init__(self):
+        kafka_config = os.environ.get('KAFKA_CONFIG', "localhost:9092").split()
+        topic = os.environ.get('KAFKA_TOPIC', "error")
+        token = os.environ.get('OMEGI_TOKEN', "ddddd")
+
+        # self.producer = KafkaProducer(bootstrap_servers=kafka_config)
         self.topic = topic
         self.token = token
 
     def export(self, spans: Sequence[Span]):
         is_error = False
         for span in spans:
+            print(span.get_span_context(), flush=True)
             if(span.name == 'exception'):
                 is_error = True
                 break
         if is_error:
             message = json.dumps(self.__format_spans__(spans)).encode('utf-8')
-            self.producer.send(self.topic, message)
+            print(message, flush=True)
+            # self.producer.send(self.topic, message)
 
     def __format_spans__(self, origin_spans: Sequence[Span]):
         data = {}
         error = {}
         spans = []
         trace_id = None
         for origin_span in origin_spans:
```

### Comparing `omegi_python_instrumentation-0.0.6/src/omegi_python_instrumentation.egg-info/PKG-INFO` & `omegi_python_instrumentation-0.0.7/src/omegi_python_instrumentation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegi-python-instrumentation
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python Instrumentation for Automatic Error Logging
 Home-page: https://github.com/TeamOmegi/Instrumentation-Python
 Author: Omegi
 Author-email: canon1107@naver.com
 Project-URL: Source Code, https://github.com/TeamOmegi/Instrumentation-Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `omegi_python_instrumentation-0.0.6/src/omegi_python_instrumentation.egg-info/requires.txt` & `omegi_python_instrumentation-0.0.7/src/omegi_python_instrumentation.egg-info/requires.txt`

 * *Files identical despite different names*

