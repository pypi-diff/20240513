# Comparing `tmp/clear_skies_stripe-0.9.5.tar.gz` & `tmp/clear_skies_stripe-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clear_skies_stripe-0.9.5.tar", max compression
+gzip compressed data, was "clear_skies_stripe-0.9.7.tar", max compression
```

## Comparing `clear_skies_stripe-0.9.5.tar` & `clear_skies_stripe-0.9.7.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1065 2024-04-12 11:44:22.990759 clear_skies_stripe-0.9.5/LICENSE
--rw-r--r--   0        0        0     8999 2024-04-19 18:20:25.160175 clear_skies_stripe-0.9.5/README.md
--rw-r--r--   0        0        0      728 2024-05-11 23:45:08.264729 clear_skies_stripe-0.9.5/pyproject.toml
--rw-r--r--   0        0        0       45 2024-04-19 18:15:31.887302 clear_skies_stripe-0.9.5/src/clearskies_stripe/__init__.py
--rw-r--r--   0        0        0       88 2024-04-19 11:45:03.248687 clear_skies_stripe-0.9.5/src/clearskies_stripe/backends/__init__.py
--rw-r--r--   0        0        0     2848 2024-04-19 18:17:49.367726 clear_skies_stripe-0.9.5/src/clearskies_stripe/backends/stripe_sdk_backend.py
--rw-r--r--   0        0        0      267 2024-04-19 06:51:54.068916 clear_skies_stripe-0.9.5/src/clearskies_stripe/di/__init__.py
--rw-r--r--   0        0        0     3410 2024-04-21 18:00:23.248867 clear_skies_stripe-0.9.5/src/clearskies_stripe/di/stripe.py
--rw-r--r--   0        0        0       91 2024-04-14 19:53:52.183390 clear_skies_stripe-0.9.5/src/clearskies_stripe/handlers/__init__.py
--rw-r--r--   0        0        0     3948 2024-04-22 20:41:16.037215 clear_skies_stripe-0.9.5/src/clearskies_stripe/handlers/create_setup_intent.py
--rw-r--r--   0        0        0     3569 2024-04-22 20:43:04.981495 clear_skies_stripe-0.9.5/src/clearskies_stripe/handlers/create_setup_intent_test.py
--rw-r--r--   0        0        0      223 2024-05-11 23:44:40.209139 clear_skies_stripe-0.9.5/src/clearskies_stripe/models/__init__.py
--rw-r--r--   0        0        0     2187 2024-05-11 23:44:40.209139 clear_skies_stripe-0.9.5/src/clearskies_stripe/models/stripe_charge.py
--rw-r--r--   0        0        0     1279 2024-05-11 23:44:40.209139 clear_skies_stripe-0.9.5/src/clearskies_stripe/models/stripe_customer.py
--rw-r--r--   0        0        0        0 2024-05-11 23:44:40.209139 clear_skies_stripe-0.9.5/src/clearskies_stripe/models/stripe_payment.py
--rw-r--r--   0        0        0      615 2024-05-11 23:44:40.209139 clear_skies_stripe-0.9.5/src/clearskies_stripe/models/stripe_payment_method.py
--rw-r--r--   0        0        0     9668 1970-01-01 00:00:00.000000 clear_skies_stripe-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-12 11:44:22.990759 clear_skies_stripe-0.9.7/LICENSE
+-rw-r--r--   0        0        0     8999 2024-04-19 18:20:25.160175 clear_skies_stripe-0.9.7/README.md
+-rw-r--r--   0        0        0      728 2024-05-12 17:41:27.733077 clear_skies_stripe-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-04-19 18:15:31.887302 clear_skies_stripe-0.9.7/src/clearskies_stripe/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-19 11:45:03.248687 clear_skies_stripe-0.9.7/src/clearskies_stripe/backends/__init__.py
+-rw-r--r--   0        0        0     3082 2024-05-12 17:41:08.620060 clear_skies_stripe-0.9.7/src/clearskies_stripe/backends/stripe_sdk_backend.py
+-rw-r--r--   0        0        0      267 2024-04-19 06:51:54.068916 clear_skies_stripe-0.9.7/src/clearskies_stripe/di/__init__.py
+-rw-r--r--   0        0        0     3410 2024-04-21 18:00:23.248867 clear_skies_stripe-0.9.7/src/clearskies_stripe/di/stripe.py
+-rw-r--r--   0        0        0       91 2024-04-14 19:53:52.183390 clear_skies_stripe-0.9.7/src/clearskies_stripe/handlers/__init__.py
+-rw-r--r--   0        0        0     3948 2024-04-22 20:41:16.037215 clear_skies_stripe-0.9.7/src/clearskies_stripe/handlers/create_setup_intent.py
+-rw-r--r--   0        0        0     3569 2024-04-22 20:43:04.981495 clear_skies_stripe-0.9.7/src/clearskies_stripe/handlers/create_setup_intent_test.py
+-rw-r--r--   0        0        0      223 2024-05-12 17:44:47.700270 clear_skies_stripe-0.9.7/src/clearskies_stripe/models/__init__.py
+-rw-r--r--   0        0        0     2223 2024-05-12 16:24:18.957847 clear_skies_stripe-0.9.7/src/clearskies_stripe/models/stripe_charge.py
+-rw-r--r--   0        0        0     1279 2024-05-11 23:44:40.209139 clear_skies_stripe-0.9.7/src/clearskies_stripe/models/stripe_customer.py
+-rw-r--r--   0        0        0      651 2024-05-12 16:21:32.157006 clear_skies_stripe-0.9.7/src/clearskies_stripe/models/stripe_payment_method.py
+-rw-r--r--   0        0        0     9668 1970-01-01 00:00:00.000000 clear_skies_stripe-0.9.7/PKG-INFO
```

### Comparing `clear_skies_stripe-0.9.5/LICENSE` & `clear_skies_stripe-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `clear_skies_stripe-0.9.5/README.md` & `clear_skies_stripe-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `clear_skies_stripe-0.9.5/pyproject.toml` & `clear_skies_stripe-0.9.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 [tool.poetry]
 name = "clear-skies-stripe"
-version = "0.9.5"
+version = "0.9.7"
 description = "clearskies bindings for working with Stripe"
 authors = [
     "Conor Mancone <cmancone@gmail.com>",
 ]
 repository = "https://github.com/cmancone/clearskies-stripe"
 license = "MIT"
 readme = "./README.md"
```

### Comparing `clear_skies_stripe-0.9.5/src/clearskies_stripe/backends/stripe_sdk_backend.py` & `clear_skies_stripe-0.9.7/src/clearskies_stripe/backends/stripe_sdk_backend.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,39 +30,46 @@
 
     def count(self, configuration: Dict[str, Any], model: clearskies.Model) -> int:
         raise ValueError("Not Supported")
 
     def records(
         self, configuration: Dict[str, Any], model: clearskies.Model, next_page_data: Dict[str, str] = None
     ) -> List[Dict[str, Any]]:
-        kwargs = {where["column"]: where["values"][0] for where in configuration.get("wheres", [])}
+        params = {where["column"]: where["values"][0] for where in configuration.get("wheres", [])}
+        options = {}
         if configuration.get("limit"):
-            kwargs["limit"] = configuration.get("limit")
-        next_page = configuration.get('pagination', {}).get('next_page')
-        if next_page:
-            kwargs["page"] = next_page
-        return getattr(self.stripe, model.table_name()).list(**kwargs)
+            params["limit"] = configuration.get("limit")
+        starting_after = configuration.get('pagination', {}).get('starting_after')
+        if starting_after:
+            params["starting_after"] = starting_after
 
-    def validate_pagination_kwargs(self, kwargs: Dict[str, Any]) -> str:
+        results = getattr(self.stripe, model.table_name()).list(params=params, options=options)
+
+        if results.get("has_more"):
+            next_page_data["starting_after"] = results["data"][-1]["id"]
+
+        return results["data"]
+
+    def validate_pagination_kwargs(self, kwargs: Dict[str, Any], case_mapping: Callable) -> str:
         extra_keys = set(kwargs.keys()) - set(self.allowed_pagination_keys())
         if len(extra_keys):
-            key_name = case_mapping('next_page')
+            key_name = case_mapping('starting_after')
             return "Invalid pagination key(s): '" + "','".join(extra_keys) + f"'.  Only '{key_name}' is allowed"
-        if 'next_page' not in kwargs:
-            key_name = case_mapping('next_page')
+        if 'starting_after' not in kwargs:
+            key_name = case_mapping('starting_after')
             return f"You must specify '{key_name}' when setting pagination"
         return ''
 
     def allowed_pagination_keys(self) -> List[str]:
-        return ["next_page"]
+        return ["starting_after"]
 
     def documentation_pagination_next_page_response(self, case_mapping: Callable) -> List[Any]:
-        return [AutoDocString(case_mapping('next_page'))]
+        return [AutoDocString(case_mapping('starting_after'))]
 
     def documentation_pagination_next_page_example(self, case_mapping: Callable) -> Dict[str, Any]:
-        return {case_mapping('next_page'): 'eyJpZCI6IHsiUyI6ICIzODM0MyJ9fQ=='}
+        return {case_mapping('starting_after'): 'cus_asdfer'}
 
     def documentation_pagination_parameters(self, case_mapping: Callable) -> List[Tuple[Any]]:
         return [(
-            AutoDocString(case_mapping('next_page'),
-                          example='eyJpZCI6IHsiUyI6ICIzODM0MyJ9fQ=='), 'A token to fetch the next page of results'
+            AutoDocString(case_mapping('starting_after'),
+                          example='cus_asdfer'), 'A token to fetch the next page of results'
         )]
```

### Comparing `clear_skies_stripe-0.9.5/src/clearskies_stripe/di/stripe.py` & `clear_skies_stripe-0.9.7/src/clearskies_stripe/di/stripe.py`

 * *Files identical despite different names*

### Comparing `clear_skies_stripe-0.9.5/src/clearskies_stripe/handlers/create_setup_intent.py` & `clear_skies_stripe-0.9.7/src/clearskies_stripe/handlers/create_setup_intent.py`

 * *Files identical despite different names*

### Comparing `clear_skies_stripe-0.9.5/src/clearskies_stripe/handlers/create_setup_intent_test.py` & `clear_skies_stripe-0.9.7/src/clearskies_stripe/handlers/create_setup_intent_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_stripe-0.9.5/src/clearskies_stripe/models/stripe_charge.py` & `clear_skies_stripe-0.9.7/src/clearskies_stripe/models/stripe_charge.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,9 +53,10 @@
                 json("shipping"),
                 string("source_transfer"),
                 string("statement_descriptor"),
                 string("statement_descriptor_suffix"),
                 select("status", values=["succeeded", "pending", "failed"]),
                 json("transfer_data"),
                 string("transfer_group"),
+                string("customer"),
             ]
         )
```

### Comparing `clear_skies_stripe-0.9.5/src/clearskies_stripe/models/stripe_customer.py` & `clear_skies_stripe-0.9.7/src/clearskies_stripe/models/stripe_customer.py`

 * *Files identical despite different names*

### Comparing `clear_skies_stripe-0.9.5/src/clearskies_stripe/models/stripe_payment_method.py` & `clear_skies_stripe-0.9.7/src/clearskies_stripe/models/stripe_payment_method.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,9 +16,10 @@
     def columns_configuration(self):
         return OrderedDict(
             [
                 string("id"),
                 string("object"),
                 json("billing_details"),
                 json("card"),
+                string("customer"),
             ]
         )
```

### Comparing `clear_skies_stripe-0.9.5/PKG-INFO` & `clear_skies_stripe-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clear-skies-stripe
-Version: 0.9.5
+Version: 0.9.7
 Summary: clearskies bindings for working with Stripe
 Home-page: https://github.com/cmancone/clearskies-stripe
 License: MIT
 Author: Conor Mancone
 Author-email: cmancone@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

