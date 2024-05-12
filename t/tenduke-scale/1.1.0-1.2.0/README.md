# Comparing `tmp/tenduke_scale-1.1.0.tar.gz` & `tmp/tenduke_scale-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenduke_scale-1.1.0.tar", max compression
+gzip compressed data, was "tenduke_scale-1.2.0.tar", max compression
```

## Comparing `tenduke_scale-1.1.0.tar` & `tenduke_scale-1.2.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1108 2024-04-09 03:52:51.018162 tenduke_scale-1.1.0/LICENSE
--rw-r--r--   0        0        0     3348 2024-04-09 03:52:51.018162 tenduke_scale-1.1.0/README.md
--rw-r--r--   0        0        0     3656 2024-04-09 03:53:03.123146 tenduke_scale-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      352 2024-04-09 03:52:51.020162 tenduke_scale-1.1.0/tenduke_scale/__init__.py
--rw-r--r--   0        0        0      169 2024-04-09 03:52:51.020162 tenduke_scale-1.1.0/tenduke_scale/auth/__init__.py
--rw-r--r--   0        0        0     4385 2024-04-09 03:52:51.020162 tenduke_scale-1.1.0/tenduke_scale/auth/scale_jwt_auth_provider.py
--rw-r--r--   0        0        0     1787 2024-04-09 03:52:51.020162 tenduke_scale-1.1.0/tenduke_scale/describe_license_options.py
--rw-r--r--   0        0        0       43 2024-04-09 03:52:51.020162 tenduke_scale-1.1.0/tenduke_scale/exceptions/__init__.py
--rw-r--r--   0        0        0     1515 2024-04-09 03:52:51.020162 tenduke_scale-1.1.0/tenduke_scale/exceptions/validation.py
--rw-r--r--   0        0        0     1440 2024-04-09 03:52:51.020162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/__init__.py
--rw-r--r--   0        0        0     3011 2024-04-09 03:52:51.020162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/client_details.py
--rw-r--r--   0        0        0     7689 2024-04-09 03:52:51.020162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/enforced_license_checkout_client.py
--rw-r--r--   0        0        0      469 2024-04-09 03:52:51.020162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/feature_flags_response.py
--rw-r--r--   0        0        0     2464 2024-04-09 03:52:51.020162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/feature_flags_token.py
--rw-r--r--   0        0        0     2220 2024-04-09 03:52:51.020162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_checkout_arguments.py
--rw-r--r--   0        0        0    23993 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_checkout_client.py
--rw-r--r--   0        0        0     2034 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_consumer_client_binding_status.py
--rw-r--r--   0        0        0      899 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_consumer_licenses_status.py
--rw-r--r--   0        0        0     8151 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_consumption_client_binding.py
--rw-r--r--   0        0        0     1349 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_heartbeat_arguments.py
--rw-r--r--   0        0        0      883 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_release_arguments.py
--rw-r--r--   0        0        0     3188 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_release_result.py
--rw-r--r--   0        0        0     4309 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_token.py
--rw-r--r--   0        0        0     8746 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/metered_license_checkout_client.py
--rw-r--r--   0        0        0     3585 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/token_store.py
--rw-r--r--   0        0        0      848 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/licensing/__init__.py
--rw-r--r--   0        0        0      522 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/licensing/consumer_type.py
--rw-r--r--   0        0        0     3455 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/licensing/effective_product_config_info.py
--rw-r--r--   0        0        0     6350 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/licensing/license.py
--rw-r--r--   0        0        0     3588 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/licensing/license_consumer.py
--rw-r--r--   0        0        0     1407 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/licensing/license_container.py
--rw-r--r--   0        0        0      821 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/licensing/license_feature.py
--rw-r--r--   0        0        0     1153 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/licensing/license_key.py
--rw-r--r--   0        0        0     3090 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/licensing/license_metadata.py
--rw-r--r--   0        0        0     2507 2024-04-09 03:52:51.022162 tenduke_scale-1.1.0/tenduke_scale/licensing/license_model.py
--rw-r--r--   0        0        0      359 2024-04-09 03:52:51.022162 tenduke_scale-1.1.0/tenduke_scale/licensing/quantity_dimension.py
--rw-r--r--   0        0        0      302 2024-04-09 03:52:51.022162 tenduke_scale-1.1.0/tenduke_scale/licensing/quantity_enforcement_type.py
--rw-r--r--   0        0        0     1421 2024-04-09 03:52:51.022162 tenduke_scale-1.1.0/tenduke_scale/paging.py
--rw-r--r--   0        0        0        0 2024-04-09 03:52:51.054162 tenduke_scale-1.1.0/tenduke_scale/py.typed
--rw-r--r--   0        0        0     4466 1970-01-01 00:00:00.000000 tenduke_scale-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1108 2024-04-15 21:31:47.027469 tenduke_scale-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3348 2024-04-15 21:31:47.027469 tenduke_scale-1.2.0/README.md
+-rw-r--r--   0        0        0     3656 2024-04-15 21:31:58.801768 tenduke_scale-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      352 2024-04-15 21:31:47.029469 tenduke_scale-1.2.0/tenduke_scale/__init__.py
+-rw-r--r--   0        0        0      169 2024-04-15 21:31:47.029469 tenduke_scale-1.2.0/tenduke_scale/auth/__init__.py
+-rw-r--r--   0        0        0     4385 2024-04-15 21:31:47.029469 tenduke_scale-1.2.0/tenduke_scale/auth/scale_jwt_auth_provider.py
+-rw-r--r--   0        0        0     1787 2024-04-15 21:31:47.029469 tenduke_scale-1.2.0/tenduke_scale/describe_license_options.py
+-rw-r--r--   0        0        0       43 2024-04-15 21:31:47.029469 tenduke_scale-1.2.0/tenduke_scale/exceptions/__init__.py
+-rw-r--r--   0        0        0     1515 2024-04-15 21:31:47.029469 tenduke_scale-1.2.0/tenduke_scale/exceptions/validation.py
+-rw-r--r--   0        0        0     1440 2024-04-15 21:31:47.029469 tenduke_scale-1.2.0/tenduke_scale/license_checkout/__init__.py
+-rw-r--r--   0        0        0     3011 2024-04-15 21:31:47.029469 tenduke_scale-1.2.0/tenduke_scale/license_checkout/client_details.py
+-rw-r--r--   0        0        0     7689 2024-04-15 21:31:47.029469 tenduke_scale-1.2.0/tenduke_scale/license_checkout/enforced_license_checkout_client.py
+-rw-r--r--   0        0        0      469 2024-04-15 21:31:47.029469 tenduke_scale-1.2.0/tenduke_scale/license_checkout/feature_flags_response.py
+-rw-r--r--   0        0        0     2464 2024-04-15 21:31:47.029469 tenduke_scale-1.2.0/tenduke_scale/license_checkout/feature_flags_token.py
+-rw-r--r--   0        0        0     2220 2024-04-15 21:31:47.029469 tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_checkout_arguments.py
+-rw-r--r--   0        0        0    23998 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_checkout_client.py
+-rw-r--r--   0        0        0     2034 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_consumer_client_binding_status.py
+-rw-r--r--   0        0        0      899 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_consumer_licenses_status.py
+-rw-r--r--   0        0        0     8151 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_consumption_client_binding.py
+-rw-r--r--   0        0        0     1349 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_heartbeat_arguments.py
+-rw-r--r--   0        0        0      883 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_release_arguments.py
+-rw-r--r--   0        0        0     3188 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_release_result.py
+-rw-r--r--   0        0        0     4309 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_token.py
+-rw-r--r--   0        0        0     8746 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/license_checkout/metered_license_checkout_client.py
+-rw-r--r--   0        0        0     3585 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/license_checkout/token_store.py
+-rw-r--r--   0        0        0      848 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/licensing/__init__.py
+-rw-r--r--   0        0        0      522 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/licensing/consumer_type.py
+-rw-r--r--   0        0        0     3455 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/licensing/effective_product_config_info.py
+-rw-r--r--   0        0        0     6350 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/licensing/license.py
+-rw-r--r--   0        0        0     3588 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/licensing/license_consumer.py
+-rw-r--r--   0        0        0     1407 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/licensing/license_container.py
+-rw-r--r--   0        0        0      821 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/licensing/license_feature.py
+-rw-r--r--   0        0        0     1153 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/licensing/license_key.py
+-rw-r--r--   0        0        0     3090 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/licensing/license_metadata.py
+-rw-r--r--   0        0        0     2507 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/licensing/license_model.py
+-rw-r--r--   0        0        0      359 2024-04-15 21:31:47.030470 tenduke_scale-1.2.0/tenduke_scale/licensing/quantity_dimension.py
+-rw-r--r--   0        0        0      302 2024-04-15 21:31:47.031469 tenduke_scale-1.2.0/tenduke_scale/licensing/quantity_enforcement_type.py
+-rw-r--r--   0        0        0     1421 2024-04-15 21:31:47.031469 tenduke_scale-1.2.0/tenduke_scale/paging.py
+-rw-r--r--   0        0        0        0 2024-04-15 21:31:47.062469 tenduke_scale-1.2.0/tenduke_scale/py.typed
+-rw-r--r--   0        0        0     4466 1970-01-01 00:00:00.000000 tenduke_scale-1.2.0/PKG-INFO
```

### Comparing `tenduke_scale-1.1.0/LICENSE` & `tenduke_scale-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/README.md` & `tenduke_scale-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/pyproject.toml` & `tenduke_scale-1.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tenduke_scale"
-version = "1.1.0"
+version = "1.2.0"
 description = "API client for 10Duke Scale."
 authors = []
 repository = "https://gitlab.com/10Duke/scale/python/python-scale-sdk"
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "tenduke_scale"},
@@ -30,36 +30,36 @@
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 requests = {extras = ["security"], version = "^2.31.0"}
 pyjwt = "^2.8.0"
-tenduke-core = ">=1.0.0,<2.0.0"
+tenduke-core = ">=1.1.0,<2.0.0"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.1.13"
 mypy = "^1.9.0"
-mutmut = "^2.4.4"
+mutmut = "^2.4.5"
 pydocstyle = "^6.3.0"
-pyright = "^1.1.356"
+pyright = "^1.1.358"
 pytest = "^7.4.4"
 pytest-asyncio = "^0.23.3"
 pytest-cov = "^4.1.0"
 pytest-freezer = "^0.4.8"
 pytest-mock = "^3.14.0"
 requests-mock = "^1.12.1"
 tox = "^4.14.2"
 types-python-dateutil = "^2.9.0.20240316"
-types-requests = "^2.31.0.20240402"
+types-requests = "^2.31.0.20240406"
 
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.5.3"
-mkdocs-material = "^9.5.16"
+mkdocs-material = "^9.5.17"
 mkdocstrings = {extras = ["python"], version = "^0.24.0"}
 mdx-include = "^1.4.2"
 
 [[tool.poetry.source]]
 name = "gitlab-tenduke-core"
 url = "https://gitlab.com/api/v4/projects/53247933/packages/pypi/simple"
 priority = "supplemental"
```

### Comparing `tenduke_scale-1.1.0/tenduke_scale/auth/scale_jwt_auth_provider.py` & `tenduke_scale-1.2.0/tenduke_scale/auth/scale_jwt_auth_provider.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/tenduke_scale/describe_license_options.py` & `tenduke_scale-1.2.0/tenduke_scale/describe_license_options.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/tenduke_scale/exceptions/validation.py` & `tenduke_scale-1.2.0/tenduke_scale/exceptions/validation.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/tenduke_scale/license_checkout/__init__.py` & `tenduke_scale-1.2.0/tenduke_scale/license_checkout/__init__.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/tenduke_scale/license_checkout/client_details.py` & `tenduke_scale-1.2.0/tenduke_scale/license_checkout/client_details.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/tenduke_scale/license_checkout/enforced_license_checkout_client.py` & `tenduke_scale-1.2.0/tenduke_scale/license_checkout/enforced_license_checkout_client.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/tenduke_scale/license_checkout/feature_flags_token.py` & `tenduke_scale-1.2.0/tenduke_scale/license_checkout/feature_flags_token.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_checkout_arguments.py` & `tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_checkout_arguments.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_checkout_client.py` & `tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_checkout_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from .license_heartbeat_arguments import LicenseHeartbeatArguments
 from .license_release_arguments import LicenseReleaseArguments
 from .license_release_result import LicenseReleaseResult
 from .license_token import LicenseToken
 from .token_store import DefaultTokenStore, TokenStoreABC
 
 
-def raise_for_reponse(response, uri):
+def raise_for_response(response, uri):
     """Translate HTTP code to error.
 
     Args:
         response: Potentially failed response object.
         uri: The URI that was requested.
 
     Raises:
@@ -71,15 +71,15 @@
     """Make a describe request and process any error response."""
     paging_args = kwargs.pop("paging_args", None)
     builder = _DescribeQueryStringBuilder()
     query_string = builder.build(**kwargs)
     uri = f"{host}{path}{query_string}"
     headers = paging_args.to_api() if paging_args is not None else {}
     response = session.get(uri, headers=headers)
-    raise_for_reponse(response, uri)
+    raise_for_response(response, uri)
     return response
 
 
 def _describe_request_json(session, host, path, **kwargs):
     """Make a describe request and return body json."""
     response = _make_request(session, host, path, **kwargs)
     return response.json()
@@ -537,15 +537,15 @@
     ):
         self.raise_if_consumer_unknown(license_consumer_id)
         key_fragment = _license_key_fragment(license_key)
         uri = f"{self.api_url}/licensing/actions/{action}{key_fragment}"
         headers = _concat_checkout_headers(client_details, license_consumer_id)
         body = [co.to_api() for co in args]
         response = self.session.post(uri, headers=headers, json=body)
-        raise_for_reponse(response, uri)
+        raise_for_response(response, uri)
         jwt_list = response.json()
         tokens = [self.parse_jwt(jwt) for jwt in jwt_list]
         self.store.save(tokens)
         return tokens
 
     def _end(
         self,
@@ -556,15 +556,15 @@
     ):
         self.raise_if_consumer_unknown(license_consumer_id)
         key_fragment = _license_key_fragment(license_key)
         uri = f"{self.api_url}/licensing/actions/{action}{key_fragment}"
         headers = _concat_checkout_headers(None, license_consumer_id)
         body = [rel.to_api() for rel in args]
         response = self.session.post(uri, headers=headers, json=body)
-        raise_for_reponse(response, uri)
+        raise_for_response(response, uri)
         results = response.json()
         result_models = [LicenseReleaseResult.from_api(res) for res in results]
         to_release = [
             model.released_lease_id
             for model in result_models
             if model.released and model.released_lease_id is not None
         ]
@@ -594,12 +594,12 @@
         self._raise_if_heartbeat_too_early(args)
         key_fragment = _license_key_fragment(license_key)
         uri = f"{self.api_url}/licensing/actions/{action}{key_fragment}"
         headers = {}
         headers["licenseConsumerId"] = str(license_consumer_id)
         body = [args.to_api() for args in args]
         response = self.session.post(uri, json=body, headers=headers)
-        raise_for_reponse(response, uri)
+        raise_for_response(response, uri)
         jwt_list = response.json()
         tokens = [self.parse_jwt(jwt) for jwt in jwt_list]
         self.store.update(tokens)
         return tokens
```

### Comparing `tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_consumer_client_binding_status.py` & `tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_consumer_client_binding_status.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_consumer_licenses_status.py` & `tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_consumer_licenses_status.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_consumption_client_binding.py` & `tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_consumption_client_binding.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_heartbeat_arguments.py` & `tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_heartbeat_arguments.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_release_arguments.py` & `tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_release_arguments.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_release_result.py` & `tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_release_result.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_token.py` & `tenduke_scale-1.2.0/tenduke_scale/license_checkout/license_token.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/tenduke_scale/license_checkout/metered_license_checkout_client.py` & `tenduke_scale-1.2.0/tenduke_scale/license_checkout/metered_license_checkout_client.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/tenduke_scale/license_checkout/token_store.py` & `tenduke_scale-1.2.0/tenduke_scale/license_checkout/token_store.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/tenduke_scale/licensing/__init__.py` & `tenduke_scale-1.2.0/tenduke_scale/licensing/__init__.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/tenduke_scale/licensing/consumer_type.py` & `tenduke_scale-1.2.0/tenduke_scale/licensing/consumer_type.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/tenduke_scale/licensing/effective_product_config_info.py` & `tenduke_scale-1.2.0/tenduke_scale/licensing/effective_product_config_info.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/tenduke_scale/licensing/license.py` & `tenduke_scale-1.2.0/tenduke_scale/licensing/license.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/tenduke_scale/licensing/license_consumer.py` & `tenduke_scale-1.2.0/tenduke_scale/licensing/license_consumer.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/tenduke_scale/licensing/license_container.py` & `tenduke_scale-1.2.0/tenduke_scale/licensing/license_container.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/tenduke_scale/licensing/license_feature.py` & `tenduke_scale-1.2.0/tenduke_scale/licensing/license_feature.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/tenduke_scale/licensing/license_key.py` & `tenduke_scale-1.2.0/tenduke_scale/licensing/license_key.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/tenduke_scale/licensing/license_metadata.py` & `tenduke_scale-1.2.0/tenduke_scale/licensing/license_metadata.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/tenduke_scale/licensing/license_model.py` & `tenduke_scale-1.2.0/tenduke_scale/licensing/license_model.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/tenduke_scale/paging.py` & `tenduke_scale-1.2.0/tenduke_scale/paging.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.1.0/PKG-INFO` & `tenduke_scale-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tenduke_scale
-Version: 1.1.0
+Version: 1.2.0
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
-Requires-Dist: tenduke-core (>=1.0.0,<2.0.0)
+Requires-Dist: tenduke-core (>=1.1.0,<2.0.0)
 Project-URL: Repository, https://gitlab.com/10Duke/scale/python/python-scale-sdk
 Description-Content-Type: text/markdown
 
 # 10Duke Scale SDK for Python
 
 The 10Duke Scale SDK for Python is a library to facilitate building applications licensed using
 [10Duke Scale](https://docs.scale.10duke.com/).
```

