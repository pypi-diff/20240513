# Comparing `tmp/cfn_kafka_admin-0.6.1.tar.gz` & `tmp/cfn_kafka_admin-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfn_kafka_admin-0.6.1.tar", max compression
+gzip compressed data, was "cfn_kafka_admin-0.6.2.tar", max compression
```

## Comparing `cfn_kafka_admin-0.6.1.tar` & `cfn_kafka_admin-0.6.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       95 2022-03-22 06:17:38.518532 cfn_kafka_admin-0.6.1/AUTHORS.rst
--rw-r--r--   0        0        0    16725 2022-03-22 06:17:38.518532 cfn_kafka_admin-0.6.1/LICENSE
--rw-r--r--   0        0        0     2314 2022-05-11 06:55:41.690789 cfn_kafka_admin-0.6.1/README.rst
--rw-r--r--   0        0        0      221 2024-04-25 15:47:12.315533 cfn_kafka_admin-0.6.1/cfn_kafka_admin/__init__.py
--rw-r--r--   0        0        0    22743 2024-04-23 12:35:25.975168 cfn_kafka_admin-0.6.1/cfn_kafka_admin/cfn_kafka_admin.py
--rw-r--r--   0        0        0      652 2023-04-24 12:49:19.847982 cfn_kafka_admin-0.6.1/cfn_kafka_admin/cfn_resources_definitions/__init__.py
--rw-r--r--   0        0        0     1958 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.1/cfn_kafka_admin/cfn_resources_definitions/custom.py
--rw-r--r--   0        0        0     1793 2023-04-24 12:49:19.847982 cfn_kafka_admin-0.6.1/cfn_kafka_admin/cfn_resources_definitions/resource.py
--rw-r--r--   0        0        0     1852 2023-04-24 12:49:19.848981 cfn_kafka_admin-0.6.1/cfn_kafka_admin/cli.py
--rw-r--r--   0        0        0     2949 2023-05-05 09:04:48.510208 cfn_kafka_admin-0.6.1/cfn_kafka_admin/common.py
--rw-r--r--   0        0        0     1012 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.1/cfn_kafka_admin/kafka_resources/__init__.py
--rw-r--r--   0        0        0     4202 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.1/cfn_kafka_admin/kafka_resources/acls.py
--rw-r--r--   0        0        0     1654 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.1/cfn_kafka_admin/kafka_resources/topics/__init__.py
--rw-r--r--   0        0        0     3082 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.1/cfn_kafka_admin/kafka_resources/topics/create.py
--rw-r--r--   0        0        0     1895 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.1/cfn_kafka_admin/kafka_resources/topics/delete.py
--rw-r--r--   0        0        0     4711 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.1/cfn_kafka_admin/kafka_resources/topics/update.py
--rw-r--r--   0        0        0      136 2024-04-17 21:17:54.966767 cfn_kafka_admin-0.6.1/cfn_kafka_admin/lambda_functions/__init__.py
--rw-r--r--   0        0        0     3764 2024-04-18 22:54:19.306229 cfn_kafka_admin-0.6.1/cfn_kafka_admin/lambda_functions/acls.py
--rw-r--r--   0        0        0     6370 2024-04-25 15:46:06.988747 cfn_kafka_admin-0.6.1/cfn_kafka_admin/lambda_functions/schemas.py
--rw-r--r--   0        0        0     7956 2024-04-18 22:54:19.306229 cfn_kafka_admin-0.6.1/cfn_kafka_admin/lambda_functions/topics.py
--rw-r--r--   0        0        0     2105 2024-04-18 22:54:19.306229 cfn_kafka_admin-0.6.1/cfn_kafka_admin/lambda_functions/utils.py
--rw-r--r--   0        0        0      118 2023-04-24 12:49:19.850982 cfn_kafka_admin-0.6.1/cfn_kafka_admin/models/__init__.py
--rw-r--r--   0        0        0    13210 2024-04-23 12:35:48.032734 cfn_kafka_admin-0.6.1/cfn_kafka_admin/models/admin.py
--rw-r--r--   0        0        0      118 2023-04-24 12:49:19.850982 cfn_kafka_admin-0.6.1/cfn_kafka_admin/specs/__init__.py
--rw-r--r--   0        0        0     2998 2024-04-25 15:47:12.514529 cfn_kafka_admin-0.6.1/cfn_kafka_admin/specs/aws-cfn-kafka-admin-provider-schema.json
--rw-r--r--   0        0        0     2446 2024-04-25 15:47:12.514529 cfn_kafka_admin-0.6.1/cfn_kafka_admin/specs/ews-kafka-acl.json
--rw-r--r--   0        0        0     2560 2024-04-25 15:47:12.514529 cfn_kafka_admin-0.6.1/cfn_kafka_admin/specs/ews-kafka-parameters.json
--rw-r--r--   0        0        0     2150 2024-04-25 15:47:12.514529 cfn_kafka_admin-0.6.1/cfn_kafka_admin/specs/ews-kafka-schema.json
--rw-r--r--   0        0        0     7182 2024-04-25 15:47:12.514529 cfn_kafka_admin-0.6.1/cfn_kafka_admin/specs/ews-kafka-topic.json
--rw-r--r--   0        0        0     2644 2024-04-25 15:47:12.315533 cfn_kafka_admin-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     3679 1970-01-01 00:00:00.000000 cfn_kafka_admin-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0       95 2022-03-22 06:17:38.518532 cfn_kafka_admin-0.6.2/AUTHORS.rst
+-rw-r--r--   0        0        0    16725 2022-03-22 06:17:38.518532 cfn_kafka_admin-0.6.2/LICENSE
+-rw-r--r--   0        0        0     2314 2022-05-11 06:55:41.690789 cfn_kafka_admin-0.6.2/README.rst
+-rw-r--r--   0        0        0      221 2024-05-13 07:33:39.646206 cfn_kafka_admin-0.6.2/cfn_kafka_admin/__init__.py
+-rw-r--r--   0        0        0    22743 2024-04-23 12:35:25.975168 cfn_kafka_admin-0.6.2/cfn_kafka_admin/cfn_kafka_admin.py
+-rw-r--r--   0        0        0      652 2023-04-24 12:49:19.847982 cfn_kafka_admin-0.6.2/cfn_kafka_admin/cfn_resources_definitions/__init__.py
+-rw-r--r--   0        0        0     1958 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.2/cfn_kafka_admin/cfn_resources_definitions/custom.py
+-rw-r--r--   0        0        0     1793 2023-04-24 12:49:19.847982 cfn_kafka_admin-0.6.2/cfn_kafka_admin/cfn_resources_definitions/resource.py
+-rw-r--r--   0        0        0     1852 2023-04-24 12:49:19.848981 cfn_kafka_admin-0.6.2/cfn_kafka_admin/cli.py
+-rw-r--r--   0        0        0     2949 2023-05-05 09:04:48.510208 cfn_kafka_admin-0.6.2/cfn_kafka_admin/common.py
+-rw-r--r--   0        0        0     1012 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.2/cfn_kafka_admin/kafka_resources/__init__.py
+-rw-r--r--   0        0        0     4202 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.2/cfn_kafka_admin/kafka_resources/acls.py
+-rw-r--r--   0        0        0     1654 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.2/cfn_kafka_admin/kafka_resources/topics/__init__.py
+-rw-r--r--   0        0        0     3082 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.2/cfn_kafka_admin/kafka_resources/topics/create.py
+-rw-r--r--   0        0        0     1895 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.2/cfn_kafka_admin/kafka_resources/topics/delete.py
+-rw-r--r--   0        0        0     4711 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.2/cfn_kafka_admin/kafka_resources/topics/update.py
+-rw-r--r--   0        0        0      136 2024-04-17 21:17:54.966767 cfn_kafka_admin-0.6.2/cfn_kafka_admin/lambda_functions/__init__.py
+-rw-r--r--   0        0        0     3764 2024-04-18 22:54:19.306229 cfn_kafka_admin-0.6.2/cfn_kafka_admin/lambda_functions/acls.py
+-rw-r--r--   0        0        0     6370 2024-04-25 15:46:06.988747 cfn_kafka_admin-0.6.2/cfn_kafka_admin/lambda_functions/schemas.py
+-rw-r--r--   0        0        0     7956 2024-04-18 22:54:19.306229 cfn_kafka_admin-0.6.2/cfn_kafka_admin/lambda_functions/topics.py
+-rw-r--r--   0        0        0     2105 2024-04-18 22:54:19.306229 cfn_kafka_admin-0.6.2/cfn_kafka_admin/lambda_functions/utils.py
+-rw-r--r--   0        0        0      118 2023-04-24 12:49:19.850982 cfn_kafka_admin-0.6.2/cfn_kafka_admin/models/__init__.py
+-rw-r--r--   0        0        0    13210 2024-04-23 12:35:48.032734 cfn_kafka_admin-0.6.2/cfn_kafka_admin/models/admin.py
+-rw-r--r--   0        0        0      118 2023-04-24 12:49:19.850982 cfn_kafka_admin-0.6.2/cfn_kafka_admin/specs/__init__.py
+-rw-r--r--   0        0        0     2998 2024-05-13 07:33:39.916203 cfn_kafka_admin-0.6.2/cfn_kafka_admin/specs/aws-cfn-kafka-admin-provider-schema.json
+-rw-r--r--   0        0        0     2446 2024-05-13 07:33:39.916203 cfn_kafka_admin-0.6.2/cfn_kafka_admin/specs/ews-kafka-acl.json
+-rw-r--r--   0        0        0     2560 2024-05-13 07:33:39.915202 cfn_kafka_admin-0.6.2/cfn_kafka_admin/specs/ews-kafka-parameters.json
+-rw-r--r--   0        0        0     2150 2024-05-13 07:33:39.916203 cfn_kafka_admin-0.6.2/cfn_kafka_admin/specs/ews-kafka-schema.json
+-rw-r--r--   0        0        0     7182 2024-05-13 07:33:39.916203 cfn_kafka_admin-0.6.2/cfn_kafka_admin/specs/ews-kafka-topic.json
+-rw-r--r--   0        0        0     2644 2024-05-13 07:33:39.646206 cfn_kafka_admin-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     3679 1970-01-01 00:00:00.000000 cfn_kafka_admin-0.6.2/PKG-INFO
```

### Comparing `cfn_kafka_admin-0.6.1/LICENSE` & `cfn_kafka_admin-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.1/README.rst` & `cfn_kafka_admin-0.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.1/cfn_kafka_admin/cfn_kafka_admin.py` & `cfn_kafka_admin-0.6.2/cfn_kafka_admin/cfn_kafka_admin.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.1/cfn_kafka_admin/cfn_resources_definitions/__init__.py` & `cfn_kafka_admin-0.6.2/cfn_kafka_admin/cfn_resources_definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.1/cfn_kafka_admin/cfn_resources_definitions/custom.py` & `cfn_kafka_admin-0.6.2/cfn_kafka_admin/cfn_resources_definitions/custom.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.1/cfn_kafka_admin/cfn_resources_definitions/resource.py` & `cfn_kafka_admin-0.6.2/cfn_kafka_admin/cfn_resources_definitions/resource.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.1/cfn_kafka_admin/cli.py` & `cfn_kafka_admin-0.6.2/cfn_kafka_admin/cli.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.1/cfn_kafka_admin/common.py` & `cfn_kafka_admin-0.6.2/cfn_kafka_admin/common.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.1/cfn_kafka_admin/kafka_resources/__init__.py` & `cfn_kafka_admin-0.6.2/cfn_kafka_admin/kafka_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.1/cfn_kafka_admin/kafka_resources/acls.py` & `cfn_kafka_admin-0.6.2/cfn_kafka_admin/kafka_resources/acls.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.1/cfn_kafka_admin/kafka_resources/topics/__init__.py` & `cfn_kafka_admin-0.6.2/cfn_kafka_admin/kafka_resources/topics/__init__.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.1/cfn_kafka_admin/kafka_resources/topics/create.py` & `cfn_kafka_admin-0.6.2/cfn_kafka_admin/kafka_resources/topics/create.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.1/cfn_kafka_admin/kafka_resources/topics/delete.py` & `cfn_kafka_admin-0.6.2/cfn_kafka_admin/kafka_resources/topics/delete.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.1/cfn_kafka_admin/kafka_resources/topics/update.py` & `cfn_kafka_admin-0.6.2/cfn_kafka_admin/kafka_resources/topics/update.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.1/cfn_kafka_admin/lambda_functions/acls.py` & `cfn_kafka_admin-0.6.2/cfn_kafka_admin/lambda_functions/acls.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.1/cfn_kafka_admin/lambda_functions/schemas.py` & `cfn_kafka_admin-0.6.2/cfn_kafka_admin/lambda_functions/schemas.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.1/cfn_kafka_admin/lambda_functions/topics.py` & `cfn_kafka_admin-0.6.2/cfn_kafka_admin/lambda_functions/topics.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.1/cfn_kafka_admin/lambda_functions/utils.py` & `cfn_kafka_admin-0.6.2/cfn_kafka_admin/lambda_functions/utils.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.1/cfn_kafka_admin/models/admin.py` & `cfn_kafka_admin-0.6.2/cfn_kafka_admin/models/admin.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.1/cfn_kafka_admin/specs/aws-cfn-kafka-admin-provider-schema.json` & `cfn_kafka_admin-0.6.2/cfn_kafka_admin/specs/aws-cfn-kafka-admin-provider-schema.json`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.1/cfn_kafka_admin/specs/ews-kafka-acl.json` & `cfn_kafka_admin-0.6.2/cfn_kafka_admin/specs/ews-kafka-acl.json`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.1/cfn_kafka_admin/specs/ews-kafka-parameters.json` & `cfn_kafka_admin-0.6.2/cfn_kafka_admin/specs/ews-kafka-parameters.json`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.1/cfn_kafka_admin/specs/ews-kafka-schema.json` & `cfn_kafka_admin-0.6.2/cfn_kafka_admin/specs/ews-kafka-schema.json`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.1/cfn_kafka_admin/specs/ews-kafka-topic.json` & `cfn_kafka_admin-0.6.2/cfn_kafka_admin/specs/ews-kafka-topic.json`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.1/pyproject.toml` & `cfn_kafka_admin-0.6.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cfn_kafka_admin"
-version = "0.6.1"
+version = "0.6.2"
 description = "AWS CloudFormation Resources to manage Kafka"
 authors = ["John Mille <john@compose-x.io>"]
 classifiers = [
   "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
   "Natural Language :: English",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.10",
@@ -63,15 +63,15 @@
 disable-timestamp = "true"
 
 
 [tool.tbump]
 github_url = "https://github.com/compose-x/cfn-kafka-admin"
 
 [tool.tbump.version]
-current = "0.6.1"
+current = "0.6.2"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `cfn_kafka_admin-0.6.1/PKG-INFO` & `cfn_kafka_admin-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfn_kafka_admin
-Version: 0.6.1
+Version: 0.6.2
 Summary: AWS CloudFormation Resources to manage Kafka
 License: MPL-2.0
 Author: John Mille
 Author-email: john@compose-x.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

