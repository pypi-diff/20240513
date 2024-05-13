# Comparing `tmp/mostlyai-0.3.4.tar.gz` & `tmp/mostlyai-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mostlyai-0.3.4.tar", max compression
+gzip compressed data, was "mostlyai-0.3.5.tar", max compression
```

## Comparing `mostlyai-0.3.4.tar` & `mostlyai-0.3.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-12-22 12:47:38.462094 mostlyai-0.3.4/LICENSE
--rw-r--r--   0        0        0     2303 2024-04-02 17:48:15.885881 mostlyai-0.3.4/README.md
--rw-r--r--   0        0        0       26 2024-03-20 14:08:04.920127 mostlyai-0.3.4/mostlyai/__init__.py
--rw-r--r--   0        0        0    13512 2024-04-26 12:02:34.891812 mostlyai-0.3.4/mostlyai/api.py
--rw-r--r--   0        0        0     9150 2024-04-19 16:58:34.132208 mostlyai-0.3.4/mostlyai/base.py
--rw-r--r--   0        0        0     2859 2024-04-19 16:58:25.136301 mostlyai-0.3.4/mostlyai/connectors.py
--rw-r--r--   0        0        0      574 2024-04-19 16:58:25.136734 mostlyai-0.3.4/mostlyai/exceptions.py
--rw-r--r--   0        0        0     4193 2024-04-19 16:58:25.138102 mostlyai-0.3.4/mostlyai/generators.py
--rw-r--r--   0        0        0    39914 2024-04-26 12:49:57.880422 mostlyai-0.3.4/mostlyai/model.py
--rw-r--r--   0        0        0     1694 2024-04-22 07:20:07.509641 mostlyai-0.3.4/mostlyai/shares.py
--rw-r--r--   0        0        0     7215 2024-04-26 12:02:34.893929 mostlyai-0.3.4/mostlyai/synthetic_datasets.py
--rw-r--r--   0        0        0     5217 2024-04-19 16:58:25.140847 mostlyai-0.3.4/mostlyai/utils.py
--rw-r--r--   0        0        0     1370 2024-04-26 12:54:09.403685 mostlyai-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     3094 1970-01-01 00:00:00.000000 mostlyai-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-08 15:08:04.881678 mostlyai-0.3.5/LICENSE
+-rw-r--r--   0        0        0     2303 2024-05-13 12:51:10.053542 mostlyai-0.3.5/README.md
+-rw-r--r--   0        0        0       26 2024-03-19 14:08:19.064057 mostlyai-0.3.5/mostlyai/__init__.py
+-rw-r--r--   0        0        0    14643 2024-05-13 12:51:10.056448 mostlyai-0.3.5/mostlyai/api.py
+-rw-r--r--   0        0        0     9150 2024-05-13 12:51:10.057253 mostlyai-0.3.5/mostlyai/base.py
+-rw-r--r--   0        0        0     3103 2024-05-13 12:51:10.058056 mostlyai-0.3.5/mostlyai/connectors.py
+-rw-r--r--   0        0        0      574 2024-03-19 14:08:19.083253 mostlyai-0.3.5/mostlyai/exceptions.py
+-rw-r--r--   0        0        0     4193 2024-05-13 12:51:10.058284 mostlyai-0.3.5/mostlyai/generators.py
+-rw-r--r--   0        0        0    42470 2024-05-13 12:51:10.058814 mostlyai-0.3.5/mostlyai/model.py
+-rw-r--r--   0        0        0     1694 2024-05-13 12:51:10.058978 mostlyai-0.3.5/mostlyai/shares.py
+-rw-r--r--   0        0        0     7215 2024-05-13 12:51:10.059430 mostlyai-0.3.5/mostlyai/synthetic_datasets.py
+-rw-r--r--   0        0        0     5217 2024-03-19 14:08:19.082058 mostlyai-0.3.5/mostlyai/utils.py
+-rw-r--r--   0        0        0     1370 2024-05-13 14:28:07.566943 mostlyai-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     3094 1970-01-01 00:00:00.000000 mostlyai-0.3.5/PKG-INFO
```

### Comparing `mostlyai-0.3.4/LICENSE` & `mostlyai-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.4/README.md` & `mostlyai-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.4/mostlyai/api.py` & `mostlyai-0.3.5/mostlyai/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -56,116 +56,148 @@
 
     def connect(self, config: dict[str, Any]) -> Connector:
         """
         Create a connector, and optionally validate the connection before saving.
 
         If validation fails, a 400 status with an error message will be returned.
 
-        The structures of the config, secrets and ssl parameters depend on the connector type.
-        Cloud storage:
-        - AZURE_STORAGE
-            - config
-                - accountName: string
-            - secrets
-                - accountKey: string
-            - location: container/path
-        - GOOGLE_CLOUD_STORAGE
-            - config
-            - secrets
-                - keyFile: string
-            - location: bucket/path
-        - S3_STORAGE
-            - config
-                - accessKey: string
-            - secrets
-                - secretKey: string
-            - location: bucket/path
-        Database:
-        - BIGQUERY
-            - config
-            - secrets
-                - keyFile: string
-            - location: dataset.table
-        - DATABRICKS
-            - config
-                - host: string
-                - httpPath: string
-                - catalog: string
-            - secrets
-                - accessToken: keyFile
-            - location: schema.table
-        - HIVE
-            - config
-                - host: string
-                - port: integer, default: 10000
-                - username: string, optional
-                - kerberos_enabled: boolean, default: false
-                - kerberos_principal: string, optional
-                - kerberos_krb5_conf: string, optional
-            - secrets
-                - password: string, optional
-                - kerberos_keytab: base64-encoded string, optional
-            - location: database.table
-        - MARIADB
-            - config
-                - host: string
-                - port: integer, default: 3306
-                - username: string
-            - secrets
-                - password: string
-            - location: database.table
-        - MSSQL
-            - config
-                - host: string
-                - port: integer, default: 1433
-                - username: string
-                - database: string
-            - secrets
-                - password: string
-            - location: schema.table
-        - MYSQL
-            - config
-                - host: string
-                - port: integer, default: 3306
-                - username: string
-            - secrets
-                - password: string
-            - location: database.table
-        - ORACLE
-            - config
-                - host: string
-                - port: integer, default: 1521
-                - username: string
-                - connectionType: enum {SID, SERVICE_NAME}, default: SID
-                - database: string, default: ORCL
-            - secrets
-                - password: string
-            - location: schema.table
-        - POSTGRES
-            - config
-                - host: string
-                - port: integer, default: 5432
-                - username: string
-                - database: string
-            - secrets
-                - password: string
-            - ssl
-                - rootCertificate: string
-                - sslCertificate: string
-                - sslCertificateKey: string
-            - location: schema.table
-        - SNOWFLAKE
-            - config
-                - account: string
-                - username: string
-                - warehouse: string, default: COMPUTE_WH
-                - database: string
-            - secrets
-                - password: string
-            - location: schema.table
+        `config` is a dictionary with the keys `type`, `config`, `secrets`, and `ssl`.
+        The structures of the `config`, `secrets` and `ssl` parameters depend on the connector `type`:
+
+        - Cloud storage:
+            - \t
+            ```yaml
+            type: AZURE_STORAGE
+            config:
+              accountName: string
+              clientId: string (required for auth via service principal)
+              tenantId: string (required for auth via service principal)
+            secrets:
+              accountKey: string (required for regular auth)
+              clientSecret: string (required for auth via service principal)
+            ```
+            - \t
+            ```yaml
+            type: GOOGLE_CLOUD_STORAGE
+            config:
+            secrets:
+              keyFile: string
+            ```
+            - \t
+            ```yaml
+            type: S3_STORAGE
+            config:
+              accessKey: string
+            secrets:
+              secretKey: string
+            ```
+        - Database:
+            - \t
+                ```yaml
+                type: BIGQUERY
+                config:
+                secrets:
+                  keyFile: string
+                ```
+            - \t
+                ```yaml
+                type: DATABRICKS
+                config:
+                  host: string
+                  httpPath: string
+                  catalog: string
+                  clientId: string (required for auth via service principal)
+                  tenantId: string (required for auth via service principal)
+                secrets:
+                  accessToken: string (required for regular auth)
+                  clientSecret: string (required for auth via service principal)
+                ```
+            - \t
+                ```yaml
+                type: HIVE
+                config:
+                  host: string
+                  port: integer, default: 10000
+                  username: string (required for regular auth)
+                  kerberos_enabled: boolean, default: false
+                  kerberos_principal: string (required if kerberos_enabled)
+                  kerberos_krb5_conf: string (required if kerberos_enabled)
+                secrets:
+                  password: string (required for regular auth)
+                  kerberos_keytab: base64-encoded string (required if kerberos_enabled)
+                ```
+            - \t
+                ```yaml
+                type: MARIADB
+                config:
+                  host: string
+                  port: integer, default: 3306
+                  username: string
+                secrets:
+                  password: string
+                ```
+            - \t
+                ```yaml
+                type: MSSQL
+                config:
+                  host: string
+                  port: integer, default: 1433
+                  username: string
+                  database: string
+                secrets:
+                 password: string
+                ```
+            - \t
+                ```yaml
+                type: MYSQL
+                config:
+                  host: string
+                  port: integer, default: 3306
+                  username: string
+                secrets:
+                  password: string
+                ```
+            - \t
+                ```yaml
+                type: ORACLE
+                config:
+                  host: string
+                  port: integer, default: 1521
+                  username: string
+                  connectionType: enum {SID, SERVICE_NAME}, default: SID
+                  database: string, default: ORCL
+                secrets:
+                  password: string
+                ```
+            - \t
+                ```yaml
+                type: POSTGRES
+                config:
+                  host: string
+                  port: integer, default: 5432
+                  username: string
+                  database: string
+                secrets:
+                  password: string
+                ssl:
+                  rootCertificate: string
+                  sslCertificate: string
+                  sslCertificateKey: string
+                ```
+            - \t
+                ```yaml
+                type: SNOWFLAKE
+                config:
+                  account: string
+                  username: string
+                  warehouse: string, default: COMPUTE_WH
+                  database: string
+                secrets:
+                  password: string
+                ```
 
         :return: The created connector.
         """
         c = self.connectors.create(config)
         rich.print(
             f"Created connector [link={self.base_url}/d/connectors/{c.id} blue underline]{c.id}[/]"
         )
```

### Comparing `mostlyai-0.3.4/mostlyai/base.py` & `mostlyai-0.3.5/mostlyai/base.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.4/mostlyai/connectors.py` & `mostlyai-0.3.5/mostlyai/connectors.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Iterator, Optional
+from typing import Any, Iterator, Optional, List, Dict
 
 from mostlyai.base import DELETE, GET, PATCH, POST, Paginator, _MostlyBaseClient
 from mostlyai.model import Connector
 from mostlyai.shares import _MostlySharesMixin
 
 
 class _MostlyConnectorsClient(_MostlyBaseClient, _MostlySharesMixin):
@@ -87,7 +87,13 @@
         return response
 
     def _locations(self, connector_id: str, prefix: str = "") -> list:
         response = self.request(
             verb=GET, path=[connector_id, "locations"], params={"prefix": prefix}
         )
         return response
+
+    def _schema(self, connector_id: str, location: str) -> List[Dict[str, Any]]:
+        response = self.request(
+            verb=GET, path=[connector_id, "schema"], params={"location": location}
+        )
+        return response
```

### Comparing `mostlyai-0.3.4/mostlyai/exceptions.py` & `mostlyai-0.3.5/mostlyai/exceptions.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.4/mostlyai/generators.py` & `mostlyai-0.3.5/mostlyai/generators.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.4/mostlyai/model.py` & `mostlyai-0.3.5/mostlyai/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # generated by datamodel-codegen:
-#   timestamp: 2024-04-26T12:18:03+00:00
+#   timestamp: 2024-05-13T11:50:56+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from pathlib import Path
 from typing import Annotated, Any, ClassVar, Dict, List, Literal, Optional, Union
@@ -123,27 +123,29 @@
     ]
 
 
 class ModelEncodingType(str, Enum):
     """
     The encoding type used for model training and data generation.
     This property is only relevant if generation method is AI_MODEL.
+    - AUTO: Model chooses among available encoding types based on the column's data type.
     - CATEGORICAL: Model samples from existing (non-rare) categories.
     - NUMERIC_AUTO: Model chooses among 3 numeric encoding types based on the values.
     - NUMERIC_DISCRETE: Model samples from existing discrete numerical values.
     - NUMERIC_BINNED: Model samples from binned buckets, to then sample randomly within a bucket.
     - NUMERIC_DIGIT: Model samples each digit of a numerical value.
     - CHARACTER: Model samples each character of a string value.
     - DATETIME: Model samples each part of a datetime value.
     - DATETIME_RELATIVE: Model samples the relative difference between datetimes within a sequence.
     - LAT_LONG: Model samples a latitude-longitude column. The format is "latitude,longitude".
     - TEXT_MODEL: Model will train a distinct TEXT model for this column.
 
     """
 
+    auto = "AUTO"
     categorical = "CATEGORICAL"
     numeric_auto = "NUMERIC_AUTO"
     numeric_discrete = "NUMERIC_DISCRETE"
     numeric_binned = "NUMERIC_BINNED"
     numeric_digit = "NUMERIC_DIGIT"
     character = "CHARACTER"
     datetime = "DATETIME"
@@ -246,19 +248,46 @@
         """
         List connector locations
 
         List the available databases, schemas, tables or folders for a connector.
         For storage connectors, this returns list of folders and files at root, respectively at `prefix` level.
         For DB connectors, this returns list of schemas (or databases for DBs without schema), respectively list of tables if `prefix` is provided.
 
+        The formats of the locations are:
+
+        - Cloud storage:
+            - `AZURE_STORAGE`: `container/path`
+            - `GOOGLE_CLOUD_STORAGE`: `bucket/path`
+            - `S3_STORAGE`: `bucket/path`
+        - Database:
+            - `BIGQUERY`: `dataset.table`
+            - `DATABRICKS`: `schema.table`
+            - `HIVE`: `database.table`
+            - `MARIADB`: `database.table`
+            - `MSSQL`: `schema.table`
+            - `MYSQL`: `database.table`
+            - `ORACLE`: `schema.table`
+            - `POSTGRES`: `schema.table`
+            - `SNOWFLAKE`: `schema.table`
         :param prefix: The prefix to filter the results by.
         :return: A list of locations (schemas, databases, directories, etc.) on the given level.
         """
         return self.client._locations(connector_id=self.id, prefix=prefix)
 
+    def schema(self, location: str) -> list[dict[str, Any]]:
+        """
+        Retrieve the schema (column names, original data types and default model encoding types) of the table at a connector location.
+
+        Please refer to `locations()` for the format of the location.
+
+        :param location: The location of the table
+        :return: The retrieved schema
+        """
+        return self.client._schema(connector_id=self.id, location=location)
+
     def config(self) -> dict[str, Any]:
         """
         Retrieve writeable generator properties
 
         :return: The generator properties as dictionary
         """
         return self.client._config(connector_id=self.id)
@@ -309,24 +338,61 @@
         bool,
         Field(
             description="If true, all tables that are referenced by foreign keys will\nbe included. If false, only the selected table will be included.\n"
         ),
     ]
 
 
+class SourceColumnValueRange(CustomBaseModel):
+    """
+    The (privacy-safe) range of values detected within a source column. These values can then be used as seed values
+    for conditional generation. For CATEGORICAL and NUMERIC_DISCRETE encoding types, this will be given as a list
+    of unique values, sorted by popularity. For other NUMERIC and for DATETIME encoding types, this will be given
+    as a min and max value. Note, that this property will only be populated, once the analysis step for the training
+    of the generator has been completed.
+
+    """
+
+    min: Annotated[
+        Optional[str],
+        Field(
+            description="The minimum value of the column. For dates, this is represented in ISO format."
+        ),
+    ] = None
+    max: Annotated[
+        Optional[str],
+        Field(
+            description="The maximum value of the column. For dates, this is represented in ISO format."
+        ),
+    ] = None
+    values: Annotated[
+        Optional[List[str]],
+        Field(
+            description="The list of distinct values of the column. Limited to a maximum of 1000 values."
+        ),
+    ] = None
+    has_null: Annotated[
+        Optional[bool],
+        Field(description="If true, null value was detected within the column."),
+    ] = None
+
+
 class SourceColumn(CustomBaseModel):
     id: Annotated[str, Field(description="The unique identifier of a source column")]
     name: Annotated[str, Field(description="The name of a source column")]
     included: Annotated[
         bool,
         Field(
             description="If true, the column will be included in the training.\nIf false, the column will be excluded from the training.\n"
         ),
     ]
     model_encoding_type: Annotated[ModelEncodingType, Field(alias="modelEncodingType")]
+    value_range: Annotated[
+        Optional[SourceColumnValueRange], Field(alias="valueRange")
+    ] = None
 
 
 class SourceForeignKey(CustomBaseModel):
     id: Annotated[str, Field(description="The unique identifier of a foreign key")]
     column: Annotated[
         Optional[str], Field(description="The column name of a foreign key.")
     ] = None
```

### Comparing `mostlyai-0.3.4/mostlyai/shares.py` & `mostlyai-0.3.5/mostlyai/shares.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.4/mostlyai/synthetic_datasets.py` & `mostlyai-0.3.5/mostlyai/synthetic_datasets.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.4/mostlyai/utils.py` & `mostlyai-0.3.5/mostlyai/utils.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.4/pyproject.toml` & `mostlyai-0.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mostlyai"
-version = "0.3.4"
+version = "0.3.5"
 description = "The official Python client for the MOSTLY AI platform."
 homepage = "https://app.mostly.ai/"
 authors = ["MOSTLY AI <office@mostly.ai>"]
 license = "Proprietary"
 readme = "README.md"
 packages = [
     { include = "mostlyai" }
```

### Comparing `mostlyai-0.3.4/PKG-INFO` & `mostlyai-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mostlyai
-Version: 0.3.4
+Version: 0.3.5
 Summary: The official Python client for the MOSTLY AI platform.
 Home-page: https://app.mostly.ai/
 License: Proprietary
 Author: MOSTLY AI
 Author-email: office@mostly.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

