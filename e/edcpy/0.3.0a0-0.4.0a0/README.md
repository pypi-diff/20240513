# Comparing `tmp/edcpy-0.3.0a0.tar.gz` & `tmp/edcpy-0.4.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edcpy-0.3.0a0.tar", max compression
+gzip compressed data, was "edcpy-0.4.0a0.tar", max compression
```

## Comparing `edcpy-0.3.0a0.tar` & `edcpy-0.4.0a0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      113 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/README.md
--rw-r--r--   0        0        0        0 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/__init__.py
--rw-r--r--   0        0        0     6135 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/backend.py
--rw-r--r--   0        0        0     2442 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/config.py
--rw-r--r--   0        0        0    12027 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/edc_api.py
--rw-r--r--   0        0        0    10682 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/keycloak.py
--rw-r--r--   0        0        0     4247 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/messaging.py
--rw-r--r--   0        0        0        0 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/models/__init__.py
--rw-r--r--   0        0        0     1621 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/models/asset.py
--rw-r--r--   0        0        0      708 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/models/contract_definition.py
--rw-r--r--   0        0        0     1035 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/models/contract_negotiation.py
--rw-r--r--   0        0        0      835 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/models/data_plane_instance.py
--rw-r--r--   0        0        0      645 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/models/policy_definition.py
--rw-r--r--   0        0        0     1948 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/models/transfer_process.py
--rw-r--r--   0        0        0      245 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/utils.py
--rw-r--r--   0        0        0      975 2024-05-10 12:05:57.783535 edcpy-0.3.0a0/pyproject.toml
--rw-r--r--   0        0        0     1256 1970-01-01 00:00:00.000000 edcpy-0.3.0a0/PKG-INFO
+-rw-r--r--   0        0        0      113 2024-05-13 10:46:47.152101 edcpy-0.4.0a0/README.md
+-rw-r--r--   0        0        0        0 2024-05-13 10:46:47.152101 edcpy-0.4.0a0/edcpy/__init__.py
+-rw-r--r--   0        0        0     6192 2024-05-13 10:46:47.152101 edcpy-0.4.0a0/edcpy/backend.py
+-rw-r--r--   0        0        0     2442 2024-05-13 10:46:47.152101 edcpy-0.4.0a0/edcpy/config.py
+-rw-r--r--   0        0        0    12027 2024-05-13 10:46:47.152101 edcpy-0.4.0a0/edcpy/edc_api.py
+-rw-r--r--   0        0        0    10682 2024-05-13 10:46:47.152101 edcpy-0.4.0a0/edcpy/keycloak.py
+-rw-r--r--   0        0        0     4324 2024-05-13 10:46:47.152101 edcpy-0.4.0a0/edcpy/messaging.py
+-rw-r--r--   0        0        0        0 2024-05-13 10:46:47.152101 edcpy-0.4.0a0/edcpy/models/__init__.py
+-rw-r--r--   0        0        0     1621 2024-05-13 10:46:47.152101 edcpy-0.4.0a0/edcpy/models/asset.py
+-rw-r--r--   0        0        0      708 2024-05-13 10:46:47.152101 edcpy-0.4.0a0/edcpy/models/contract_definition.py
+-rw-r--r--   0        0        0     1035 2024-05-13 10:46:47.152101 edcpy-0.4.0a0/edcpy/models/contract_negotiation.py
+-rw-r--r--   0        0        0      835 2024-05-13 10:46:47.152101 edcpy-0.4.0a0/edcpy/models/data_plane_instance.py
+-rw-r--r--   0        0        0      645 2024-05-13 10:46:47.152101 edcpy-0.4.0a0/edcpy/models/policy_definition.py
+-rw-r--r--   0        0        0     1948 2024-05-13 10:46:47.152101 edcpy-0.4.0a0/edcpy/models/transfer_process.py
+-rw-r--r--   0        0        0      245 2024-05-13 10:46:47.152101 edcpy-0.4.0a0/edcpy/utils.py
+-rw-r--r--   0        0        0      975 2024-05-13 10:46:47.156101 edcpy-0.4.0a0/pyproject.toml
+-rw-r--r--   0        0        0     1256 1970-01-01 00:00:00.000000 edcpy-0.4.0a0/PKG-INFO
```

### Comparing `edcpy-0.3.0a0/edcpy/backend.py` & `edcpy-0.4.0a0/edcpy/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
 class EndpointDataReference(BaseModel):
     id: str
     endpoint: str
     authKey: str
     authCode: str
     properties: dict
+    contractId: str
 
 
 async def get_messaging_app() -> AsyncGenerator[MessagingApp, None]:
     # The Consumer Backend does not declare any queues, it just publishes messages
     async with with_messaging_app() as msg_app:
         yield msg_app
 
@@ -123,14 +124,15 @@
     message = HttpPullMessage(
         auth_code_decoded=decoded_auth_code,
         auth_code=item.authCode,
         auth_key=item.authKey,
         endpoint=item.endpoint,
         id=item.id,
         properties=item.properties,
+        contract_id=item.contractId,
     )
 
     # The provider hostname is included in the routing key to facilitate
     # the scenario of the consumer communicating with multiple providers in parallel.
     # The provider hostname is included in its slugified form since dots are
     # interpreted as routing key separators by RabbitMQ.
     routing_key = f"{BASE_HTTP_PULL_QUEUE_ROUTING_KEY}.{slugify(message.provider_host)}"
```

### Comparing `edcpy-0.3.0a0/edcpy/config.py` & `edcpy-0.4.0a0/edcpy/config.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.3.0a0/edcpy/edc_api.py` & `edcpy-0.4.0a0/edcpy/edc_api.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.3.0a0/edcpy/keycloak.py` & `edcpy-0.4.0a0/edcpy/keycloak.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.3.0a0/edcpy/messaging.py` & `edcpy-0.4.0a0/edcpy/messaging.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 class HttpPullMessage(BaseModel):
     auth_code_decoded: dict
     auth_code: str
     auth_key: str
     endpoint: str
     id: str
     properties: dict
+    contract_id: str
 
     @property
     def http_method(self) -> str:
         ret = (
             self.auth_code_decoded.get("dad", {})
             .get("properties", {})
             .get("method", None)
@@ -42,14 +43,15 @@
 
     @property
     def request_args(self) -> dict:
         return {
             "method": self.http_method,
             "url": self.endpoint,
             "headers": {self.auth_key: self.auth_code},
+            "params": {"contractId": self.contract_id},
         }
 
     @property
     def transfer_process_id(self) -> str:
         return self.id
 
     @property
```

### Comparing `edcpy-0.3.0a0/edcpy/models/asset.py` & `edcpy-0.4.0a0/edcpy/models/asset.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.3.0a0/edcpy/models/contract_definition.py` & `edcpy-0.4.0a0/edcpy/models/contract_definition.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.3.0a0/edcpy/models/contract_negotiation.py` & `edcpy-0.4.0a0/edcpy/models/contract_negotiation.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.3.0a0/edcpy/models/data_plane_instance.py` & `edcpy-0.4.0a0/edcpy/models/data_plane_instance.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.3.0a0/edcpy/models/policy_definition.py` & `edcpy-0.4.0a0/edcpy/models/policy_definition.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.3.0a0/edcpy/models/transfer_process.py` & `edcpy-0.4.0a0/edcpy/models/transfer_process.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.3.0a0/pyproject.toml` & `edcpy-0.4.0a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edcpy"
-version = "0.3.0a0"
+version = "0.4.0a0"
 description = "Package that provides a series of utilities to facilitate interaction with the Management and Control APIs of an EDC connector"
 authors = ["Andres Garcia Mangas <andres.garcia@fundacionctic.org>"]
 license = "EUPL-1.2"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `edcpy-0.3.0a0/PKG-INFO` & `edcpy-0.4.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edcpy
-Version: 0.3.0a0
+Version: 0.4.0a0
 Summary: Package that provides a series of utilities to facilitate interaction with the Management and Control APIs of an EDC connector
 License: EUPL-1.2
 Author: Andres Garcia Mangas
 Author-email: andres.garcia@fundacionctic.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Programming Language :: Python :: 3
```

