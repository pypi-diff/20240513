# Comparing `tmp/kafka-broker-0.4.3.tar.gz` & `tmp/kafka-broker-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafka-broker-0.4.3.tar", last modified: Fri Apr 26 08:43:26 2024, max compression
+gzip compressed data, was "kafka-broker-0.4.4.tar", last modified: Mon May 13 11:20:53 2024, max compression
```

## Comparing `kafka-broker-0.4.3.tar` & `kafka-broker-0.4.4.tar`

### file list

```diff
@@ -1,38 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 08:43:26.599851 kafka-broker-0.4.3/
--rw-rw-rw-   0        0        0     1090 2023-11-07 12:59:41.000000 kafka-broker-0.4.3/LICENSE
--rw-rw-rw-   0        0        0     4159 2024-04-26 08:43:26.598851 kafka-broker-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     3507 2023-11-17 10:11:05.000000 kafka-broker-0.4.3/README.md
--rw-rw-rw-   0        0        0      851 2024-04-26 08:43:08.000000 kafka-broker-0.4.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-26 08:43:26.599851 kafka-broker-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0      365 2024-04-08 10:30:04.000000 kafka-broker-0.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 08:43:26.560764 kafka-broker-0.4.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-26 08:43:26.577304 kafka-broker-0.4.3/src/kafka_broker/
--rw-rw-rw-   0        0        0      385 2024-04-08 10:30:04.000000 kafka-broker-0.4.3/src/kafka_broker/__init__.py
--rw-rw-rw-   0        0        0      281 2023-11-20 13:43:40.000000 kafka-broker-0.4.3/src/kafka_broker/base_config.ini
--rw-rw-rw-   0        0        0     6006 2024-04-08 10:30:04.000000 kafka-broker-0.4.3/src/kafka_broker/broker_manager.py
-drwxrwxrwx   0        0        0        0 2024-04-26 08:43:26.592825 kafka-broker-0.4.3/src/kafka_broker/classes/
--rw-rw-rw-   0        0        0        0 2024-04-08 10:30:04.000000 kafka-broker-0.4.3/src/kafka_broker/classes/__init__.py
--rw-rw-rw-   0        0        0     2003 2024-04-08 10:30:04.000000 kafka-broker-0.4.3/src/kafka_broker/classes/cache.py
--rw-rw-rw-   0        0        0     2190 2023-11-17 10:11:05.000000 kafka-broker-0.4.3/src/kafka_broker/classes/consumer_storage.py
--rw-rw-rw-   0        0        0     2888 2024-04-08 10:30:04.000000 kafka-broker-0.4.3/src/kafka_broker/classes/event_object.py
--rw-rw-rw-   0        0        0     3198 2024-04-26 08:39:25.000000 kafka-broker-0.4.3/src/kafka_broker/classes/event_router.py
--rw-rw-rw-   0        0        0     1167 2023-11-17 10:11:05.000000 kafka-broker-0.4.3/src/kafka_broker/config.py
--rw-rw-rw-   0        0        0     3234 2024-04-08 10:30:04.000000 kafka-broker-0.4.3/src/kafka_broker/consumer.py
--rw-rw-rw-   0        0        0      184 2024-04-08 10:30:04.000000 kafka-broker-0.4.3/src/kafka_broker/enums.py
-drwxrwxrwx   0        0        0        0 2024-04-26 08:43:26.595823 kafka-broker-0.4.3/src/kafka_broker/exceptions/
--rw-rw-rw-   0        0        0        0 2023-11-20 10:24:31.000000 kafka-broker-0.4.3/src/kafka_broker/exceptions/__init__.py
--rw-rw-rw-   0        0        0      462 2024-04-08 12:44:45.000000 kafka-broker-0.4.3/src/kafka_broker/exceptions/base.py
--rw-rw-rw-   0        0        0      605 2024-04-08 10:30:04.000000 kafka-broker-0.4.3/src/kafka_broker/exceptions/cache.py
--rw-rw-rw-   0        0        0     1368 2024-04-08 10:30:04.000000 kafka-broker-0.4.3/src/kafka_broker/producer.py
--rw-rw-rw-   0        0        0        0 2024-04-08 10:30:04.000000 kafka-broker-0.4.3/src/kafka_broker/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-26 08:43:26.596823 kafka-broker-0.4.3/src/kafka_broker/schemas/
--rw-rw-rw-   0        0        0        0 2024-04-08 11:56:29.000000 kafka-broker-0.4.3/src/kafka_broker/schemas/__init__.py
--rw-rw-rw-   0        0        0      341 2024-04-26 08:42:50.000000 kafka-broker-0.4.3/src/kafka_broker/schemas/log.py
-drwxrwxrwx   0        0        0        0 2024-04-26 08:43:26.583300 kafka-broker-0.4.3/src/kafka_broker.egg-info/
--rw-rw-rw-   0        0        0     4159 2024-04-26 08:43:26.000000 kafka-broker-0.4.3/src/kafka_broker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      881 2024-04-26 08:43:26.000000 kafka-broker-0.4.3/src/kafka_broker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 08:43:26.000000 kafka-broker-0.4.3/src/kafka_broker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-26 08:43:26.000000 kafka-broker-0.4.3/src/kafka_broker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-26 08:43:26.000000 kafka-broker-0.4.3/src/kafka_broker.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-26 08:43:26.597823 kafka-broker-0.4.3/tests/
--rw-rw-rw-   0        0        0      356 2023-11-17 10:11:05.000000 kafka-broker-0.4.3/tests/test_event_object.py
+drwxrwxrwx   0        0        0        0 2024-05-13 11:20:53.855554 kafka-broker-0.4.4/
+-rw-rw-rw-   0        0        0     1090 2024-05-13 11:08:25.000000 kafka-broker-0.4.4/LICENSE
+-rw-rw-rw-   0        0        0     4159 2024-05-13 11:20:53.854555 kafka-broker-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3507 2024-05-13 11:08:25.000000 kafka-broker-0.4.4/README.md
+-rw-rw-rw-   0        0        0      851 2024-05-13 11:19:36.000000 kafka-broker-0.4.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 11:20:53.855554 kafka-broker-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      365 2024-05-13 11:08:25.000000 kafka-broker-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 11:20:53.830553 kafka-broker-0.4.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-13 11:20:53.841554 kafka-broker-0.4.4/src/kafka_broker/
+-rw-rw-rw-   0        0        0      385 2024-05-13 11:08:25.000000 kafka-broker-0.4.4/src/kafka_broker/__init__.py
+-rw-rw-rw-   0        0        0      281 2024-05-13 11:08:25.000000 kafka-broker-0.4.4/src/kafka_broker/base_config.ini
+-rw-rw-rw-   0        0        0     6006 2024-05-13 11:08:25.000000 kafka-broker-0.4.4/src/kafka_broker/broker_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-13 11:20:53.849554 kafka-broker-0.4.4/src/kafka_broker/classes/
+-rw-rw-rw-   0        0        0        0 2024-05-13 11:08:25.000000 kafka-broker-0.4.4/src/kafka_broker/classes/__init__.py
+-rw-rw-rw-   0        0        0     2003 2024-05-13 11:08:25.000000 kafka-broker-0.4.4/src/kafka_broker/classes/cache.py
+-rw-rw-rw-   0        0        0     2190 2024-05-13 11:08:25.000000 kafka-broker-0.4.4/src/kafka_broker/classes/consumer_storage.py
+-rw-rw-rw-   0        0        0     2899 2024-05-13 11:09:26.000000 kafka-broker-0.4.4/src/kafka_broker/classes/event_object.py
+-rw-rw-rw-   0        0        0     3198 2024-05-13 11:08:25.000000 kafka-broker-0.4.4/src/kafka_broker/classes/event_router.py
+-rw-rw-rw-   0        0        0     1167 2024-05-13 11:08:25.000000 kafka-broker-0.4.4/src/kafka_broker/config.py
+-rw-rw-rw-   0        0        0     3234 2024-05-13 11:08:25.000000 kafka-broker-0.4.4/src/kafka_broker/consumer.py
+-rw-rw-rw-   0        0        0      184 2024-05-13 11:08:25.000000 kafka-broker-0.4.4/src/kafka_broker/enums.py
+drwxrwxrwx   0        0        0        0 2024-05-13 11:20:53.852554 kafka-broker-0.4.4/src/kafka_broker/exceptions/
+-rw-rw-rw-   0        0        0        0 2024-05-13 11:08:25.000000 kafka-broker-0.4.4/src/kafka_broker/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      462 2024-05-13 11:08:25.000000 kafka-broker-0.4.4/src/kafka_broker/exceptions/base.py
+-rw-rw-rw-   0        0        0      605 2024-05-13 11:08:25.000000 kafka-broker-0.4.4/src/kafka_broker/exceptions/cache.py
+-rw-rw-rw-   0        0        0     1368 2024-05-13 11:08:25.000000 kafka-broker-0.4.4/src/kafka_broker/producer.py
+drwxrwxrwx   0        0        0        0 2024-05-13 11:20:53.853553 kafka-broker-0.4.4/src/kafka_broker/schemas/
+-rw-rw-rw-   0        0        0        0 2024-05-13 11:08:25.000000 kafka-broker-0.4.4/src/kafka_broker/schemas/__init__.py
+-rw-rw-rw-   0        0        0      341 2024-05-13 11:08:25.000000 kafka-broker-0.4.4/src/kafka_broker/schemas/log.py
+drwxrwxrwx   0        0        0        0 2024-05-13 11:20:53.845554 kafka-broker-0.4.4/src/kafka_broker.egg-info/
+-rw-rw-rw-   0        0        0     4159 2024-05-13 11:20:53.000000 kafka-broker-0.4.4/src/kafka_broker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      828 2024-05-13 11:20:53.000000 kafka-broker-0.4.4/src/kafka_broker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 11:20:53.000000 kafka-broker-0.4.4/src/kafka_broker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-13 11:20:53.000000 kafka-broker-0.4.4/src/kafka_broker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-13 11:20:53.000000 kafka-broker-0.4.4/src/kafka_broker.egg-info/top_level.txt
```

### Comparing `kafka-broker-0.4.3/LICENSE` & `kafka-broker-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.4.3/PKG-INFO` & `kafka-broker-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-broker
-Version: 0.4.3
+Version: 0.4.4
 Summary: A python package implementation for the confluent kafka package. Managing producing and consuming.
 Author-email: Tijmen Simons <tijmen.simons@student.hu.nl>, Ivar Stek <ivar.stek@student.hu.nl>
 Project-URL: Homepage, https://github.com/TijmenSimons/kafka-broker
 Project-URL: Bug Tracker, https://github.com/TijmenSimons/kafka-broker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kafka-broker-0.4.3/README.md` & `kafka-broker-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.4.3/pyproject.toml` & `kafka-broker-0.4.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kafka-broker"
-version = "0.4.3"
+version = "0.4.4"
 authors = [
   { name="Tijmen Simons", email="tijmen.simons@student.hu.nl" },
   { name="Ivar Stek", email="ivar.stek@student.hu.nl" },
 ]
 description = "A python package implementation for the confluent kafka package. Managing producing and consuming."
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `kafka-broker-0.4.3/src/kafka_broker/broker_manager.py` & `kafka-broker-0.4.4/src/kafka_broker/broker_manager.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.4.3/src/kafka_broker/classes/cache.py` & `kafka-broker-0.4.4/src/kafka_broker/classes/cache.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.4.3/src/kafka_broker/classes/consumer_storage.py` & `kafka-broker-0.4.4/src/kafka_broker/classes/consumer_storage.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.4.3/src/kafka_broker/classes/event_object.py` & `kafka-broker-0.4.4/src/kafka_broker/classes/event_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 from pydantic import BaseModel
 
 
 class EventObject:
     def __init__(
         self,
         *,
-        correlation_id: int = None,
+        correlation_id: uuid.UUID = None,
         event: str = None,
         data: dict[any] = None,
         status: str = None,
         audit_log: list[dict[str, int, int]] = None,
     ) -> None:
         """Initialize the EventObject:
 
         Parameters
         ----------
-        correlation_id : int
-            Event intentifier
+        correlation_id : uuid.UUID
+            Event identifier
 
         event : str
             Event action
 
         data : any
             payload
```

### Comparing `kafka-broker-0.4.3/src/kafka_broker/classes/event_router.py` & `kafka-broker-0.4.4/src/kafka_broker/classes/event_router.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.4.3/src/kafka_broker/config.py` & `kafka-broker-0.4.4/src/kafka_broker/config.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.4.3/src/kafka_broker/consumer.py` & `kafka-broker-0.4.4/src/kafka_broker/consumer.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.4.3/src/kafka_broker/exceptions/cache.py` & `kafka-broker-0.4.4/src/kafka_broker/exceptions/cache.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.4.3/src/kafka_broker/producer.py` & `kafka-broker-0.4.4/src/kafka_broker/producer.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.4.3/src/kafka_broker.egg-info/PKG-INFO` & `kafka-broker-0.4.4/src/kafka_broker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-broker
-Version: 0.4.3
+Version: 0.4.4
 Summary: A python package implementation for the confluent kafka package. Managing producing and consuming.
 Author-email: Tijmen Simons <tijmen.simons@student.hu.nl>, Ivar Stek <ivar.stek@student.hu.nl>
 Project-URL: Homepage, https://github.com/TijmenSimons/kafka-broker
 Project-URL: Bug Tracker, https://github.com/TijmenSimons/kafka-broker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kafka-broker-0.4.3/src/kafka_broker.egg-info/SOURCES.txt` & `kafka-broker-0.4.4/src/kafka_broker.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,22 @@
 src/kafka_broker/__init__.py
 src/kafka_broker/base_config.ini
 src/kafka_broker/broker_manager.py
 src/kafka_broker/config.py
 src/kafka_broker/consumer.py
 src/kafka_broker/enums.py
 src/kafka_broker/producer.py
-src/kafka_broker/py.typed
 src/kafka_broker.egg-info/PKG-INFO
 src/kafka_broker.egg-info/SOURCES.txt
 src/kafka_broker.egg-info/dependency_links.txt
 src/kafka_broker.egg-info/requires.txt
 src/kafka_broker.egg-info/top_level.txt
 src/kafka_broker/classes/__init__.py
 src/kafka_broker/classes/cache.py
 src/kafka_broker/classes/consumer_storage.py
 src/kafka_broker/classes/event_object.py
 src/kafka_broker/classes/event_router.py
 src/kafka_broker/exceptions/__init__.py
 src/kafka_broker/exceptions/base.py
 src/kafka_broker/exceptions/cache.py
 src/kafka_broker/schemas/__init__.py
-src/kafka_broker/schemas/log.py
-tests/test_event_object.py
+src/kafka_broker/schemas/log.py
```

