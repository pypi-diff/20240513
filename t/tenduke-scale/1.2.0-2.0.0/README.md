# Comparing `tmp/tenduke_scale-1.2.0.tar.gz` & `tmp/tenduke_scale-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenduke_scale-1.2.0.tar", max compression
+gzip compressed data, was "tenduke_scale-2.0.0.tar", max compression
```

## Comparing `tenduke_scale-1.2.0.tar` & `tenduke_scale-2.0.0.tar`

### file list

```diff
@@ -1,40 +1,42 @@
--rw-r--r--   0        0        0     1108 2024-04-15 21:31:47.027469 tenduke_scale-1.2.0/LICENSE
--rw-r--r--   0        0        0     3348 2024-04-15 21:31:47.027469 tenduke_scale-1.2.0/README.md
--rw-r--r--   0        0        0     3656 2024-04-15 21:31:58.801768 tenduke_scale-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      352 2024-04-15 21:31:47.029469 tenduke_scale-1.2.0/tenduke_scale/__init__.py
--rw-r--r--   0        0        0      169 2024-04-15 21:31:47.029469 tenduke_scale-1.2.0/tenduke_scale/auth/__init__.py
--rw-r--r--   0        0        0     4385 2024-04-15 21:31:47.029469 tenduke_scale-1.2.0/tenduke_scale/auth/scale_jwt_auth_provider.py
--rw-r--r--   0        0        0     1787 2024-04-15 21:31:47.029469 tenduke_scale-1.2.0/tenduke_scale/describe_license_options.py
--rw-r--r--   0        0        0       43 2024-04-15 21:31:47.029469 tenduke_scale-1.2.0/tenduke_scale/exceptions/__init__.py
--rw-r--r--   0        0        0     1515 2024-04-15 21:31:47.029469 tenduke_scale-1.2.0/tenduke_scale/exceptions/validation.py
--rw-r--r--   0        0        0     1440 2024-04-15 21:31:47.029469 tenduke_scale-1.2.0/tenduke_scale/license_checkout/__init__.py
--rw-r--r--   0        0        0     3011 2024-04-15 21:31:47.029469 tenduke_scale-1.2.0/tenduke_scale/license_checkout/client_details.py
--rw-r--r--   0        0        0     7689 2024-04-15 21:31:47.029469 tenduke_scale-1.2.0/tenduke_scale/license_checkout/enforced_license_checkout_client.py
--rw-r--r--   0        0        0      469 2024-04-15 21:31:47.029469 tenduke_scale-1.2.0/tenduke_scale/license_checkout/feature_flags_response.py
--rw-r--r--   0        0        0     2464 2024-04-15 21:31:47.029469 tenduke_scale-1.2.0/tenduke_scale/license_checkout/feature_flags_token.py
--rw-r--r--   0        0        0     2220 2024-04-15 21:31:47.029469 tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_checkout_arguments.py
--rw-r--r--   0        0        0    23998 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_checkout_client.py
--rw-r--r--   0        0        0     2034 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_consumer_client_binding_status.py
--rw-r--r--   0        0        0      899 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_consumer_licenses_status.py
--rw-r--r--   0        0        0     8151 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_consumption_client_binding.py
--rw-r--r--   0        0        0     1349 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_heartbeat_arguments.py
--rw-r--r--   0        0        0      883 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_release_arguments.py
--rw-r--r--   0        0        0     3188 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_release_result.py
--rw-r--r--   0        0        0     4309 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_token.py
--rw-r--r--   0        0        0     8746 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/license_checkout/metered_license_checkout_client.py
--rw-r--r--   0        0        0     3585 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/license_checkout/token_store.py
--rw-r--r--   0        0        0      848 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/licensing/__init__.py
--rw-r--r--   0        0        0      522 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/licensing/consumer_type.py
--rw-r--r--   0        0        0     3455 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/licensing/effective_product_config_info.py
--rw-r--r--   0        0        0     6350 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/licensing/license.py
--rw-r--r--   0        0        0     3588 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/licensing/license_consumer.py
--rw-r--r--   0        0        0     1407 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/licensing/license_container.py
--rw-r--r--   0        0        0      821 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/licensing/license_feature.py
--rw-r--r--   0        0        0     1153 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/licensing/license_key.py
--rw-r--r--   0        0        0     3090 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/licensing/license_metadata.py
--rw-r--r--   0        0        0     2507 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/licensing/license_model.py
--rw-r--r--   0        0        0      359 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/licensing/quantity_dimension.py
--rw-r--r--   0        0        0      302 2024-04-15 21:31:47.031469 tenduke_scale-1.2.0/tenduke_scale/licensing/quantity_enforcement_type.py
--rw-r--r--   0        0        0     1421 2024-04-15 21:31:47.031469 tenduke_scale-1.2.0/tenduke_scale/paging.py
--rw-r--r--   0        0        0        0 2024-04-15 21:31:47.062469 tenduke_scale-1.2.0/tenduke_scale/py.typed
--rw-r--r--   0        0        0     4466 1970-01-01 00:00:00.000000 tenduke_scale-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1108 2024-05-12 22:18:00.629210 tenduke_scale-2.0.0/LICENSE
+-rw-r--r--   0        0        0     3348 2024-05-12 22:18:00.629210 tenduke_scale-2.0.0/README.md
+-rw-r--r--   0        0        0     3656 2024-05-12 22:18:14.270175 tenduke_scale-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      352 2024-05-12 22:18:00.632210 tenduke_scale-2.0.0/tenduke_scale/__init__.py
+-rw-r--r--   0        0        0      169 2024-05-12 22:18:00.632210 tenduke_scale-2.0.0/tenduke_scale/auth/__init__.py
+-rw-r--r--   0        0        0     4385 2024-05-12 22:18:00.633210 tenduke_scale-2.0.0/tenduke_scale/auth/scale_jwt_auth_provider.py
+-rw-r--r--   0        0        0     1787 2024-05-12 22:18:00.633210 tenduke_scale-2.0.0/tenduke_scale/describe_license_options.py
+-rw-r--r--   0        0        0       43 2024-05-12 22:18:00.633210 tenduke_scale-2.0.0/tenduke_scale/exceptions/__init__.py
+-rw-r--r--   0        0        0     1515 2024-05-12 22:18:00.633210 tenduke_scale-2.0.0/tenduke_scale/exceptions/validation.py
+-rw-r--r--   0        0        0      118 2024-05-12 22:18:00.633210 tenduke_scale-2.0.0/tenduke_scale/http/__init__.py
+-rw-r--r--   0        0        0      666 2024-05-12 22:18:00.633210 tenduke_scale-2.0.0/tenduke_scale/http/scale_session_factory.py
+-rw-r--r--   0        0        0     1440 2024-05-12 22:18:00.633210 tenduke_scale-2.0.0/tenduke_scale/license_checkout/__init__.py
+-rw-r--r--   0        0        0     3011 2024-05-12 22:18:00.633210 tenduke_scale-2.0.0/tenduke_scale/license_checkout/client_details.py
+-rw-r--r--   0        0        0     7689 2024-05-12 22:18:00.633210 tenduke_scale-2.0.0/tenduke_scale/license_checkout/enforced_license_checkout_client.py
+-rw-r--r--   0        0        0      469 2024-05-12 22:18:00.633210 tenduke_scale-2.0.0/tenduke_scale/license_checkout/feature_flags_response.py
+-rw-r--r--   0        0        0     2464 2024-05-12 22:18:00.633210 tenduke_scale-2.0.0/tenduke_scale/license_checkout/feature_flags_token.py
+-rw-r--r--   0        0        0     2220 2024-05-12 22:18:00.634210 tenduke_scale-2.0.0/tenduke_scale/license_checkout/license_checkout_arguments.py
+-rw-r--r--   0        0        0    23998 2024-05-12 22:18:00.634210 tenduke_scale-2.0.0/tenduke_scale/license_checkout/license_checkout_client.py
+-rw-r--r--   0        0        0     2034 2024-05-12 22:18:00.634210 tenduke_scale-2.0.0/tenduke_scale/license_checkout/license_consumer_client_binding_status.py
+-rw-r--r--   0        0        0      899 2024-05-12 22:18:00.634210 tenduke_scale-2.0.0/tenduke_scale/license_checkout/license_consumer_licenses_status.py
+-rw-r--r--   0        0        0     8151 2024-05-12 22:18:00.634210 tenduke_scale-2.0.0/tenduke_scale/license_checkout/license_consumption_client_binding.py
+-rw-r--r--   0        0        0     1349 2024-05-12 22:18:00.634210 tenduke_scale-2.0.0/tenduke_scale/license_checkout/license_heartbeat_arguments.py
+-rw-r--r--   0        0        0      883 2024-05-12 22:18:00.634210 tenduke_scale-2.0.0/tenduke_scale/license_checkout/license_release_arguments.py
+-rw-r--r--   0        0        0     3188 2024-05-12 22:18:00.634210 tenduke_scale-2.0.0/tenduke_scale/license_checkout/license_release_result.py
+-rw-r--r--   0        0        0     4309 2024-05-12 22:18:00.634210 tenduke_scale-2.0.0/tenduke_scale/license_checkout/license_token.py
+-rw-r--r--   0        0        0     8746 2024-05-12 22:18:00.635210 tenduke_scale-2.0.0/tenduke_scale/license_checkout/metered_license_checkout_client.py
+-rw-r--r--   0        0        0     3585 2024-05-12 22:18:00.635210 tenduke_scale-2.0.0/tenduke_scale/license_checkout/token_store.py
+-rw-r--r--   0        0        0      848 2024-05-12 22:18:00.635210 tenduke_scale-2.0.0/tenduke_scale/licensing/__init__.py
+-rw-r--r--   0        0        0      522 2024-05-12 22:18:00.635210 tenduke_scale-2.0.0/tenduke_scale/licensing/consumer_type.py
+-rw-r--r--   0        0        0     3455 2024-05-12 22:18:00.635210 tenduke_scale-2.0.0/tenduke_scale/licensing/effective_product_config_info.py
+-rw-r--r--   0        0        0     6350 2024-05-12 22:18:00.635210 tenduke_scale-2.0.0/tenduke_scale/licensing/license.py
+-rw-r--r--   0        0        0     3588 2024-05-12 22:18:00.635210 tenduke_scale-2.0.0/tenduke_scale/licensing/license_consumer.py
+-rw-r--r--   0        0        0     1407 2024-05-12 22:18:00.635210 tenduke_scale-2.0.0/tenduke_scale/licensing/license_container.py
+-rw-r--r--   0        0        0      821 2024-05-12 22:18:00.635210 tenduke_scale-2.0.0/tenduke_scale/licensing/license_feature.py
+-rw-r--r--   0        0        0     1153 2024-05-12 22:18:00.635210 tenduke_scale-2.0.0/tenduke_scale/licensing/license_key.py
+-rw-r--r--   0        0        0     3090 2024-05-12 22:18:00.635210 tenduke_scale-2.0.0/tenduke_scale/licensing/license_metadata.py
+-rw-r--r--   0        0        0     2507 2024-05-12 22:18:00.635210 tenduke_scale-2.0.0/tenduke_scale/licensing/license_model.py
+-rw-r--r--   0        0        0      359 2024-05-12 22:18:00.635210 tenduke_scale-2.0.0/tenduke_scale/licensing/quantity_dimension.py
+-rw-r--r--   0        0        0      302 2024-05-12 22:18:00.635210 tenduke_scale-2.0.0/tenduke_scale/licensing/quantity_enforcement_type.py
+-rw-r--r--   0        0        0     1421 2024-05-12 22:18:00.636210 tenduke_scale-2.0.0/tenduke_scale/paging.py
+-rw-r--r--   0        0        0        0 2024-05-12 22:18:00.675210 tenduke_scale-2.0.0/tenduke_scale/py.typed
+-rw-r--r--   0        0        0     4466 1970-01-01 00:00:00.000000 tenduke_scale-2.0.0/PKG-INFO
```

### Comparing `tenduke_scale-1.2.0/LICENSE` & `tenduke_scale-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/README.md` & `tenduke_scale-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/pyproject.toml` & `tenduke_scale-2.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tenduke_scale"
-version = "1.2.0"
+version = "2.0.0"
 description = "API client for 10Duke Scale."
 authors = []
 repository = "https://gitlab.com/10Duke/scale/python/python-scale-sdk"
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "tenduke_scale"},
@@ -30,15 +30,15 @@
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 requests = {extras = ["security"], version = "^2.31.0"}
 pyjwt = "^2.8.0"
-tenduke-core = ">=1.1.0,<2.0.0"
+tenduke-core = ">=2.0.1,<3.0.0"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.1.13"
 mypy = "^1.9.0"
 mutmut = "^2.4.5"
 pydocstyle = "^6.3.0"
 pyright = "^1.1.358"
```

### Comparing `tenduke_scale-1.2.0/tenduke_scale/auth/scale_jwt_auth_provider.py` & `tenduke_scale-2.0.0/tenduke_scale/auth/scale_jwt_auth_provider.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/describe_license_options.py` & `tenduke_scale-2.0.0/tenduke_scale/describe_license_options.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/exceptions/validation.py` & `tenduke_scale-2.0.0/tenduke_scale/exceptions/validation.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/license_checkout/__init__.py` & `tenduke_scale-2.0.0/tenduke_scale/license_checkout/__init__.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/license_checkout/client_details.py` & `tenduke_scale-2.0.0/tenduke_scale/license_checkout/client_details.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/license_checkout/enforced_license_checkout_client.py` & `tenduke_scale-2.0.0/tenduke_scale/license_checkout/enforced_license_checkout_client.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/license_checkout/feature_flags_token.py` & `tenduke_scale-2.0.0/tenduke_scale/license_checkout/feature_flags_token.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_checkout_arguments.py` & `tenduke_scale-2.0.0/tenduke_scale/license_checkout/license_checkout_arguments.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_checkout_client.py` & `tenduke_scale-2.0.0/tenduke_scale/license_checkout/license_checkout_client.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_consumer_client_binding_status.py` & `tenduke_scale-2.0.0/tenduke_scale/license_checkout/license_consumer_client_binding_status.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_consumer_licenses_status.py` & `tenduke_scale-2.0.0/tenduke_scale/license_checkout/license_consumer_licenses_status.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_consumption_client_binding.py` & `tenduke_scale-2.0.0/tenduke_scale/license_checkout/license_consumption_client_binding.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_heartbeat_arguments.py` & `tenduke_scale-2.0.0/tenduke_scale/license_checkout/license_heartbeat_arguments.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_release_arguments.py` & `tenduke_scale-2.0.0/tenduke_scale/license_checkout/license_release_arguments.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_release_result.py` & `tenduke_scale-2.0.0/tenduke_scale/license_checkout/license_release_result.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_token.py` & `tenduke_scale-2.0.0/tenduke_scale/license_checkout/license_token.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/license_checkout/metered_license_checkout_client.py` & `tenduke_scale-2.0.0/tenduke_scale/license_checkout/metered_license_checkout_client.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/license_checkout/token_store.py` & `tenduke_scale-2.0.0/tenduke_scale/license_checkout/token_store.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/licensing/__init__.py` & `tenduke_scale-2.0.0/tenduke_scale/licensing/__init__.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/licensing/consumer_type.py` & `tenduke_scale-2.0.0/tenduke_scale/licensing/consumer_type.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/licensing/effective_product_config_info.py` & `tenduke_scale-2.0.0/tenduke_scale/licensing/effective_product_config_info.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/licensing/license.py` & `tenduke_scale-2.0.0/tenduke_scale/licensing/license.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/licensing/license_consumer.py` & `tenduke_scale-2.0.0/tenduke_scale/licensing/license_consumer.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/licensing/license_container.py` & `tenduke_scale-2.0.0/tenduke_scale/licensing/license_container.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/licensing/license_feature.py` & `tenduke_scale-2.0.0/tenduke_scale/licensing/license_feature.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/licensing/license_key.py` & `tenduke_scale-2.0.0/tenduke_scale/licensing/license_key.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/licensing/license_metadata.py` & `tenduke_scale-2.0.0/tenduke_scale/licensing/license_metadata.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/licensing/license_model.py` & `tenduke_scale-2.0.0/tenduke_scale/licensing/license_model.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/tenduke_scale/paging.py` & `tenduke_scale-2.0.0/tenduke_scale/paging.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.2.0/PKG-INFO` & `tenduke_scale-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tenduke_scale
-Version: 1.2.0
+Version: 2.0.0
 Summary: API client for 10Duke Scale.
 Home-page: https://gitlab.com/10Duke/scale/python/python-scale-sdk
 License: MIT
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Requires-Dist: requests[security] (>=2.31.0,<3.0.0)
-Requires-Dist: tenduke-core (>=1.1.0,<2.0.0)
+Requires-Dist: tenduke-core (>=2.0.1,<3.0.0)
 Project-URL: Repository, https://gitlab.com/10Duke/scale/python/python-scale-sdk
 Description-Content-Type: text/markdown
 
 # 10Duke Scale SDK for Python
 
 The 10Duke Scale SDK for Python is a library to facilitate building applications licensed using
 [10Duke Scale](https://docs.scale.10duke.com/).
```

