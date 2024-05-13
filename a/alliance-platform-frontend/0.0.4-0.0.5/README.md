# Comparing `tmp/alliance_platform_frontend-0.0.4.tar.gz` & `tmp/alliance_platform_frontend-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alliance_platform_frontend-0.0.4.tar", last modified: Tue Apr 23 21:40:21 2024, max compression
+gzip compressed data, was "alliance_platform_frontend-0.0.5.tar", last modified: Mon May 13 01:21:01 2024, max compression
```

## Comparing `alliance_platform_frontend-0.0.4.tar` & `alliance_platform_frontend-0.0.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     2946 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/README.md
--rw-r--r--   0        0        0       22 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/__init__.py
--rw-r--r--   0        0        0      784 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/button.py
--rw-r--r--   0        0        0     1839 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/date_picker.py
--rw-r--r--   0        0        0     2524 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/icon.py
--rw-r--r--   0        0        0     1421 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/inline_alert.py
--rw-r--r--   0        0        0     1464 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/menubar.py
--rw-r--r--   0        0        0     2075 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/misc.py
--rw-r--r--   0        0        0     1622 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/pagination.py
--rw-r--r--   0        0        0     2270 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/table.py
--rw-r--r--   0        0        0     1127 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/time_input.py
--rw-r--r--   0        0        0     1243 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/utils.py
--rw-r--r--   0        0        0      358 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/apps.py
--rw-r--r--   0        0        0      633 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/__init__.py
--rw-r--r--   0        0        0     2402 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/asset_registry.py
--rw-r--r--   0        0        0    15999 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/base.py
--rw-r--r--   0        0        0    17116 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/context.py
--rw-r--r--   0        0        0     2507 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/middleware.py
--rw-r--r--   0        0        0    13537 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/ssr.py
--rw-r--r--   0        0        0     7051 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/vanilla_extract.py
--rw-r--r--   0        0        0    33895 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/vite.py
--rw-r--r--   0        0        0      175 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/vitePreload.ts
--rw-r--r--   0        0        0    11144 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/dom_possible_standard_names.py
--rw-r--r--   0        0        0        0 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/forms/__init__.py
--rw-r--r--   0        0        0     1620 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/forms/renderers.py
--rw-r--r--   0        0        0     5340 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/management/commands/extract_frontend_assets.py
--rw-r--r--   0        0        0    10434 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/prop_handlers.py
--rw-r--r--   0        0        0        0 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/py.typed
--rw-r--r--   0        0        0     7344 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/settings.py
--rw-r--r--   0        0        0     2684 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/templates/bundler_dev_check.html
--rw-r--r--   0        0        0        0 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/templatetags/__init__.py
--rw-r--r--   0        0        0     5451 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/templatetags/alliance_ui.py
--rw-r--r--   0        0        0    12922 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/templatetags/bundler.py
--rw-r--r--   0        0        0     9664 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/templatetags/form.py
--rw-r--r--   0        0        0    56265 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/templatetags/react.py
--rw-r--r--   0        0        0     4316 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/templatetags/vanilla_extract.py
--rw-r--r--   0        0        0     3283 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/util.py
--rw-r--r--   0        0        0     2120 2024-04-23 21:40:21.584088 alliance_platform_frontend-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     2503 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/tests/fixtures/build_test/manifest.json
--rw-r--r--   0        0        0       39 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/tests/fixtures/development-css-mappings/login_css_ts.json
--rw-r--r--   0        0        0       30 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/tests/fixtures/production-css-mappings/login_css_ts.json
--rw-r--r--   0        0        0      648 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/tests/fixtures/server_build_test/manifest.json
--rw-r--r--   0        0        0     7955 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/tests/test_alliance_ui_templatetags.py
--rw-r--r--   0        0        0    11182 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/tests/test_bundler.py
--rw-r--r--   0        0        0    33736 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/tests/test_bundler_templatetags.py
--rw-r--r--   0        0        0     5837 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/tests/test_context.py
--rw-r--r--   0        0        0      721 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/tests/test_utils/__init__.py
--rw-r--r--   0        0        0     2370 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/tests/test_utils/bundler.py
--rw-r--r--   0        0        0     4424 1970-01-01 00:00:00.000000 alliance_platform_frontend-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2946 2024-05-13 01:20:27.951018 alliance_platform_frontend-0.0.5/README.md
+-rw-r--r--   0        0        0       22 2024-05-13 01:20:27.951018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 01:20:27.951018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/__init__.py
+-rw-r--r--   0        0        0      784 2024-05-13 01:20:27.951018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/button.py
+-rw-r--r--   0        0        0     1839 2024-05-13 01:20:27.951018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/date_picker.py
+-rw-r--r--   0        0        0     2524 2024-05-13 01:20:27.951018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/icon.py
+-rw-r--r--   0        0        0     1421 2024-05-13 01:20:27.951018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/inline_alert.py
+-rw-r--r--   0        0        0     1464 2024-05-13 01:20:27.951018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/menubar.py
+-rw-r--r--   0        0        0     2075 2024-05-13 01:20:27.951018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/misc.py
+-rw-r--r--   0        0        0     1622 2024-05-13 01:20:27.951018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/pagination.py
+-rw-r--r--   0        0        0     2270 2024-05-13 01:20:27.951018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/table.py
+-rw-r--r--   0        0        0     1127 2024-05-13 01:20:27.951018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/time_input.py
+-rw-r--r--   0        0        0     1243 2024-05-13 01:20:27.951018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/utils.py
+-rw-r--r--   0        0        0      358 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/apps.py
+-rw-r--r--   0        0        0      633 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/__init__.py
+-rw-r--r--   0        0        0     2402 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/asset_registry.py
+-rw-r--r--   0        0        0    16050 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/base.py
+-rw-r--r--   0        0        0    17210 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/context.py
+-rw-r--r--   0        0        0     2507 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/middleware.py
+-rw-r--r--   0        0        0    13537 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/ssr.py
+-rw-r--r--   0        0        0     7051 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/vanilla_extract.py
+-rw-r--r--   0        0        0    34218 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/vite.py
+-rw-r--r--   0        0        0      175 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/vitePreload.ts
+-rw-r--r--   0        0        0    11144 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/dom_possible_standard_names.py
+-rw-r--r--   0        0        0        0 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/forms/__init__.py
+-rw-r--r--   0        0        0     1620 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/forms/renderers.py
+-rw-r--r--   0        0        0     5340 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/management/commands/extract_frontend_assets.py
+-rw-r--r--   0        0        0     9471 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/prop_handlers.py
+-rw-r--r--   0        0        0        0 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/py.typed
+-rw-r--r--   0        0        0     8806 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/settings.py
+-rw-r--r--   0        0        0     2684 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/templates/bundler_dev_check.html
+-rw-r--r--   0        0        0        0 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/templatetags/__init__.py
+-rw-r--r--   0        0        0     5451 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/templatetags/alliance_ui.py
+-rw-r--r--   0        0        0    13141 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/templatetags/bundler.py
+-rw-r--r--   0        0        0     9664 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/templatetags/form.py
+-rw-r--r--   0        0        0    64472 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/templatetags/react.py
+-rw-r--r--   0        0        0     4316 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/templatetags/vanilla_extract.py
+-rw-r--r--   0        0        0     3283 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/alliance_platform/frontend/util.py
+-rw-r--r--   0        0        0     2120 2024-05-13 01:21:01.663164 alliance_platform_frontend-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     2503 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/tests/fixtures/build_test/manifest.json
+-rw-r--r--   0        0        0       39 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/tests/fixtures/development-css-mappings/login_css_ts.json
+-rw-r--r--   0        0        0       30 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/tests/fixtures/production-css-mappings/login_css_ts.json
+-rw-r--r--   0        0        0      648 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/tests/fixtures/server_build_test/manifest.json
+-rw-r--r--   0        0        0     7955 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/tests/test_alliance_ui_templatetags.py
+-rw-r--r--   0        0        0    12764 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/tests/test_bundler.py
+-rw-r--r--   0        0        0    41503 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/tests/test_bundler_templatetags.py
+-rw-r--r--   0        0        0     5837 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/tests/test_context.py
+-rw-r--r--   0        0        0      721 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0     2384 2024-05-13 01:20:27.955018 alliance_platform_frontend-0.0.5/tests/test_utils/bundler.py
+-rw-r--r--   0        0        0     4424 1970-01-01 00:00:00.000000 alliance_platform_frontend-0.0.5/PKG-INFO
```

### Comparing `alliance_platform_frontend-0.0.4/README.md` & `alliance_platform_frontend-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/button.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/button.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/date_picker.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/date_picker.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/icon.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/icon.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/inline_alert.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/inline_alert.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/menubar.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/menubar.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/misc.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/misc.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/pagination.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/pagination.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/table.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/table.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/time_input.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/time_input.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/utils.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/alliance_ui/utils.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/__init__.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/__init__.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/asset_registry.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/asset_registry.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/base.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,16 @@
 
 @dataclass
 class DevServerCheck:
     """Describes status of dev server"""
 
     #: True if dev server is running at the expected location (depends on the bundler)
     is_running: bool
+    #: Read timeout
+    read_timeout: bool = False
     #: The project dir the frontend dev server is running at. This is used to determine if it's for the same project as Django.
     project_dir: Path | None = None
 
     def is_wrong_server(self) -> bool:
         """Returns ``True`` if server is running, but it's for a different project"""
         from alliance_platform.frontend.bundler import get_bundler
```

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/context.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,19 +169,21 @@
 
     #: Will be set if used within ``BundlerAssetContextMiddleware``. In other contexts may be unavailable
     request: HttpRequest | None
 
     def __init__(
         self,
         *,
-        frontend_asset_registry: FrontendAssetRegistry = ap_frontend_settings.FRONTEND_ASSET_REGISTRY,
+        frontend_asset_registry: FrontendAssetRegistry | None = None,
         html_target=html_target_browser,
         skip_checks=False,
         request: HttpRequest | None = None,
     ):
+        if frontend_asset_registry is None:
+            frontend_asset_registry = ap_frontend_settings.FRONTEND_ASSET_REGISTRY
         self.request = request
         self.skip_checks = skip_checks
         self.html_target = html_target
         self.frontend_asset_registry = frontend_asset_registry
         self.assets = []
         self.ssr_queue = {}
         self.current_id = 0
```

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/middleware.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/middleware.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/ssr.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/ssr.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/vanilla_extract.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/vanilla_extract.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/vite.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/bundler/vite.py`

 * *Files 1% similar despite different names*

```diff
@@ -505,32 +505,37 @@
 
     def check_dev_server(self):
         try:
             r = requests.get(urljoin(self.dev_server_url_base, "check"), timeout=1)
             if r.status_code != 200:
                 return DevServerCheck(is_running=False)
             return DevServerCheck(is_running=True, project_dir=Path(r.json()["projectDir"]))
-        except requests.ConnectionError:
+        except (requests.ConnectionError, requests.ConnectTimeout):
             return DevServerCheck(is_running=False)
+        except requests.ReadTimeout:
+            return DevServerCheck(is_running=True, read_timeout=True)
 
     def format_code(self, code: str):
         """In dev format code using /format-code endpoint defined in dev-server.ts
 
         In production this is a no-op for performance reasons.
         """
-        if self.is_development():
+        if self.is_development() and (
+            len(code) < ap_frontend_settings.DEV_CODE_FORMAT_LIMIT
+            or ap_frontend_settings.DEV_CODE_FORMAT_LIMIT == 0
+        ):
             if self.wait_for_server:
                 self.wait_for_server()
             payload = {"code": code}
             try:
                 response = requests.post(
                     urljoin(self.dev_server_url_base, "format-code"),
                     data=json.dumps(payload),
                     headers={"Content-Type": "application/json"},
-                    timeout=1,
+                    timeout=ap_frontend_settings.DEV_CODE_FORMAT_TIMEOUT,
                 )
                 if response.status_code != 200:
                     logger.error(
                         f"Bad response {response.status_code} from dev-server.ts for format-code action: {response.content.decode()}"
                     )
                 else:
                     try:
```

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/dom_possible_standard_names.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/dom_possible_standard_names.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/forms/renderers.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/forms/renderers.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/management/commands/extract_frontend_assets.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/management/commands/extract_frontend_assets.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/prop_handlers.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/prop_handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,21 +56,14 @@
     such that the prop passed to the component is a ``Date`` instance. The ``get_representation`` method will return
     the string representation `"2020-01-01"` and ``get_tag`` returns ``"Date"``. This gets serialized to
     ``["@@CUSTOM", "Date", "2020-01-01"]``. The ``@@CUSTOM`` tag is used to indicate that the prop needs special "reviving"
     on the frontend which is detected by ``processSSRRequest`` in ``ssr.ts``, and will call the appropriate "reviver"
     defined in ``ssrJsonRevivers.tsx``.
     """
 
-    def as_debug_string(self):
-        """Return prop as a string for debugging purposes.
-
-        This is outputted in the template in dev to better illustrate how the component and props are constructed.
-        """
-        raise NotImplementedError(f"as_debug_string not implemented for {self.__class__.__name__}")
-
     @classmethod
     def should_apply(cls, value: Any, node: ComponentNode, context: Context):
         """Return ``True`` if this prop handler should be used for the given value."""
         raise NotImplementedError(f"should_apply not implemented for {cls.__name__}")
 
     def __init__(self, value: Any, node: ComponentNode, context: Context):
         """Intentionally blank; each implementation can handle this differently."""
@@ -95,17 +88,14 @@
 
     def generate_code(self, generator: ComponentSourceCodeGenerator):
         calendar_date = generator.resolve_prop_import(
             "frontend/src/re-exports.tsx", ImportSpecifier("CalendarDate")
         )
         return NewExpression(calendar_date, self.js_args)
 
-    def as_debug_string(self):
-        return f'new CalendarDate({", ".join(map(str, self.js_args))})'
-
     @classmethod
     def should_apply(cls, value: Any, node: ComponentNode, context: Context):
         return isinstance(value, datetime.date) and not isinstance(value, datetime.datetime)
 
 
 class DateTimeProp(ComponentProp):
     """Convert a python datetime"""
@@ -136,17 +126,14 @@
             "frontend/src/re-exports.tsx", ImportSpecifier("CalendarDateTime")
         )
         return NewExpression(
             calendar_date,
             self.js_args,
         )
 
-    def as_debug_string(self):
-        return f'new CalendarDateTime({", ".join(map(str, self.js_args))})'
-
     @classmethod
     def should_apply(cls, value: Any, node: ComponentNode, context: Context):
         return isinstance(value, datetime.datetime) and not is_aware(value)
 
 
 class ZonedDateTimeProp(ComponentProp):
     """Convert a python datetime"""
@@ -184,17 +171,14 @@
             "frontend/src/re-exports.tsx", ImportSpecifier("ZonedDateTime")
         )
         return NewExpression(
             calendar_date,
             self.js_args,
         )
 
-    def as_debug_string(self):
-        return f"new ZonedDateTime({', '.join(map(str, self.js_args))})"
-
     @classmethod
     def should_apply(cls, value: Any, node: ComponentNode, context: Context):
         return isinstance(value, datetime.datetime) and is_aware(value)
 
 
 class TimeProp(ComponentProp):
     """Convert a python time to a @internationalized/date time"""
@@ -212,17 +196,14 @@
     def get_representation(self, context):
         return self.js_args
 
     def generate_code(self, generator: ComponentSourceCodeGenerator):
         calendar_date = generator.resolve_prop_import("frontend/src/re-exports.tsx", ImportSpecifier("Time"))
         return NewExpression(calendar_date, self.js_args)
 
-    def as_debug_string(self):
-        return f'new Time({", ".join(map(str, self.js_args))})'
-
     @classmethod
     def should_apply(cls, value: Any, node: ComponentNode, context: Context):
         return isinstance(value, datetime.time)
 
 
 class SetProp(ComponentProp):
     """Handles passing a python ``set`` to a JS ``Set``"""
@@ -237,17 +218,14 @@
 
     def generate_code(self, generator: ComponentSourceCodeGenerator):
         return NewExpression(
             Identifier("Set"),
             [ArrayLiteralExpression([self.convert_to_node(value, generator) for value in self.value])],
         )
 
-    def as_debug_string(self):
-        return f"new Set({list(self.value)})"
-
     @classmethod
     def should_apply(cls, value: Any, node: ComponentNode, context: Context):
         return isinstance(value, set)
 
     def __init__(self, value: set, node: ComponentNode, context: Context):
         super().__init__(value, node, context)
         self.value = set({node.resolve_prop(element, context) for element in value})
@@ -274,18 +252,13 @@
         return Identifier("NaN")
 
     def get_representation(self, context: SSRSerializerContext) -> dict | str | list:
         if math.isinf(self.value):
             return "Infinity" if self.value > 0 else "-Infinity"
         return "NaN"
 
-    def as_debug_string(self):
-        if math.isinf(self.value):
-            return "Infinity" if self.value > 0 else "-Infinity"
-        return "NaN"
-
     @classmethod
     def should_apply(cls, value: Any, node: ComponentNode, context: Context):
         return isinstance(value, float) and (math.isinf(value) or math.isnan(value))
 
 
 default_prop_handlers = [DateProp, DateTimeProp, ZonedDateTimeProp, TimeProp, SetProp, SpecialNumeric]
```

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/settings.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -59,18 +59,24 @@
     BUNDLER_DISABLE_DEV_CHECK_HTML: bool | None
     #: The path to the node_modules directory. This is used by ViteBundler to resolve optimized deps, and extract_frontend_assets to determine when an import comes from node_modules directly.
     NODE_MODULES_DIR: Path | str
     #: The directory production assets exists in. This directory should include the Vanilla Extract mappings.
     PRODUCTION_DIR: Path
     #: Any custom prop handlers to use for react components. This can be a string import path to a list of prop handlers, or the list directly.
     REACT_PROP_HANDLERS: str | list[type["ComponentProp"]]
-    #: File that is used to render React components using the ``react`` tag. This file should export a function named ``renderComponent`` and a function ``createElementWithProps``.
+    #: File that is used to render React components using the ``react`` tag. This file should export a function named ``renderComponent`` and a function ``createElement`` (this can just be re-exported from React).
     REACT_RENDER_COMPONENT_FILE: Path | str
     #: Set to a dotted path to a function that will be called to resolve the global context for SSR. This function should return a dictionary of values to be passed to the SSR renderer under the `globalContext` key.
     SSR_GLOBAL_CONTEXT_RESOLVER: str | None
+    #: The limit to apply for code format requests in development mode. This is limited to 1mb by default; anything above that will not be formatted. This is only
+    #: applicable to dev mode where code is formatted to make debugging easier when viewing the source.
+    DEV_CODE_FORMAT_LIMIT: int | None
+    #: This is the timeout to apply for code format requests in development mode. This is limited to 1 seconds by default. The only time you should need to
+    #: tweak this is if you are attempting to debug issues with a large piece of code; in which case you likely need to increase ``DEV_CODE_FORMAT_LIMIT`` as well.
+    DEV_CODE_FORMAT_TIMEOUT: int | None
 
 
 def maybe_import_string(val: Any | None):
     """
     If the given setting is a string import notation,
     then perform the necessary import or imports.
     """
@@ -109,16 +115,22 @@
     BUNDLER: "BaseBundler"
     #: Directories to exclude from asset extraction. By default, all directories returned by ``get_app_template_dirs("templates")`` will be inspected.
     EXTRACT_ASSETS_EXCLUDE_DIRS: tuple[Path | str, Pattern[str]]
     #: Disable the HTML outputted by ``bundler_dev_checks``. This can be useful if you want the check on generally in a project, but specific developers may wish to disable it.
     BUNDLER_DISABLE_DEV_CHECK_HTML: bool
     #: Set to a dotted path to a function that will be called to resolve the global context for SSR. This function should return a dictionary of values to be passed to the SSR renderer under the `globalContext` key.
     SSR_GLOBAL_CONTEXT_RESOLVER: str | None
-    #: File that is used to render React components using the ``react`` tag. This file should export a function named ``renderComponent`` and a function ``createElementWithProps``.
+    #: File that is used to render React components using the ``react`` tag. This file should export a function named ``renderComponent`` and a function ``createElement`` (this can just be re-exported from React).
     REACT_RENDER_COMPONENT_FILE: Path
+    #: The limit to apply for code format requests in development mode. This is limited to 1mb by default; anything above that will not be formatted. This is only
+    #: applicable to dev mode where code is formatted to make debugging easier when viewing the source.
+    DEV_CODE_FORMAT_LIMIT: int
+    #: This is the timeout to apply for code format requests in development mode. This is limited to 1 seconds by default. The only time you should need to
+    #: tweak this is if you are attempting to debug issues with a large piece of code; in which case you likely need to increase ``DEV_CODE_FORMAT_LIMIT`` as well.
+    DEV_CODE_FORMAT_TIMEOUT: int
 
     def check_settings(self):
         # TODO: Implement checks on required settings
 
         # lock registry to make sure assets aren't added after startup that would be missed by
         # extract_frontend_assets
         self.FRONTEND_ASSET_REGISTRY.lock()
@@ -133,13 +145,15 @@
 DEFAULTS = {
     "REACT_PROP_HANDLERS": "alliance_platform.frontend.prop_handlers.default_prop_handlers",
     "DEBUG_COMPONENT_OUTPUT": False,
     "EXTRACT_ASSETS_EXCLUDE_DIRS": tuple(),
     "BUNDLER_DISABLE_DEV_CHECK_HTML": True,
     "SSR_GLOBAL_CONTEXT_RESOLVER": None,
     "REACT_RENDER_COMPONENT_FILE": None,
+    "DEV_CODE_FORMAT_LIMIT": 1 * 1024 * 1024,
+    "DEV_CODE_FORMAT_TIMEOUT": 1,
 }
 
 
 ap_frontend_settings = AlliancePlatformFrontendSettings(
     "FRONTEND", import_strings=IMPORT_STRINGS, defaults=DEFAULTS
 )
```

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/templates/bundler_dev_check.html` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/templates/bundler_dev_check.html`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/templatetags/alliance_ui.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/templatetags/alliance_ui.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/templatetags/bundler.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/templatetags/bundler.py`

 * *Files 2% similar despite different names*

```diff
@@ -309,11 +309,15 @@
     if not check.is_ok():
         if not check.is_running:
             warnings.warn("Bundler dev server not running; run `yarn dev` to start")
         elif check.is_wrong_server():
             warnings.warn(
                 f"Bundler dev server was found but it's for project {check.project_dir}. You likely need to run `yarn dev` under {bundler.root_dir}"
             )
+        elif check.read_timeout:
+            warnings.warn(
+                "Received ReadTimeout from dev server check; dev server is likely running but no response was received within timeout to verify"
+            )
         if ap_frontend_settings.BUNDLER_DISABLE_DEV_CHECK_HTML:
             return ""
         return get_template("bundler_dev_check.html").render({"check": check})
     return ""
```

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/templatetags/form.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/templatetags/form.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/templatetags/react.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/templatetags/react.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,55 @@
 from __future__ import annotations
 
 from collections import defaultdict
 from dataclasses import dataclass
+from dataclasses import field
+from html.parser import HTMLParser
 import math
 from pathlib import Path
 from typing import Any
+from typing import Callable
+from typing import Union
 from typing import cast
 import warnings
 
+from alliance_platform.codegen.printer import TypescriptPrinter
 from alliance_platform.codegen.printer import TypescriptSourceFileWriter
 from alliance_platform.codegen.typescript import CallExpression
 from alliance_platform.codegen.typescript import FunctionDeclaration
 from alliance_platform.codegen.typescript import Identifier
 from alliance_platform.codegen.typescript import ImportDefaultSpecifier
 from alliance_platform.codegen.typescript import ImportSpecifier
-from alliance_platform.codegen.typescript import Node
+from alliance_platform.codegen.typescript import JsxAttribute
+from alliance_platform.codegen.typescript import JsxElement
+from alliance_platform.codegen.typescript import MultiLineComment
 from alliance_platform.codegen.typescript import PropertyAccessExpression
 from alliance_platform.codegen.typescript import ReturnStatement
 from alliance_platform.codegen.typescript import StringLiteral
 from alliance_platform.codegen.typescript import UnconvertibleValueException
+from alliance_platform.codegen.typescript import convert_to_node
 from allianceutils.template import build_html_attrs
 from allianceutils.template import is_static_expression
 from allianceutils.template import parse_tag_arguments
 from allianceutils.template import resolve
 from allianceutils.util import underscore_to_camel
 from django import template
 from django.core.exceptions import ImproperlyConfigured
 from django.forms.models import ModelChoiceIteratorValue
 from django.template import Context
+from django.template import Node
 from django.template import NodeList
 from django.template import Origin
 from django.template import TemplateSyntaxError
 from django.template.base import UNKNOWN_SOURCE
 from django.template.base import FilterExpression
+from django.template.base import TextNode
+from django.utils.functional import LazyObject
 from django.utils.html import format_html
+from django.utils.safestring import SafeString
 from django.utils.safestring import mark_safe
 
 from ..bundler import get_bundler
 from ..bundler.base import BaseBundler
 from ..bundler.base import ResolveContext
 from ..bundler.context import BundlerAsset
 from ..bundler.context import BundlerAssetContext
@@ -66,14 +78,17 @@
     """
     if isinstance(value, dict):
         return {k: resolve_prop(v, node, context) for k, v in value.items()}
     if isinstance(value, (list, tuple)):
         return list(resolve_prop(v, node, context) for v in value)
     if isinstance(value, ModelChoiceIteratorValue):
         return resolve_prop(value.value, node, context)  # type: ignore[attr-defined] # It has this value but no type info
+    if isinstance(value, LazyObject):
+        # unwrap lazy objects
+        return value.__reduce__()[1][0]
     for handler in ap_frontend_settings.REACT_PROP_HANDLERS:
         if handler.should_apply(value, node, context):
             return handler(value, node, context)
     return value
 
 
 @register.tag("component")
@@ -184,15 +199,15 @@
 
     - ``ssr:disabled=True`` - if specified, no server side rendering will occur for this component
     - ``component:omit_if_empty=True`` - if specified, the component will not be rendered if it has no children. This is
       useful for when components may not be rendered based on permission checks
     - ``container:tag`` - the HTML tag to use for the container. Defaults to the custom element ``dj-component``.
     - ``container:<any other prop>`` - any other props will be passed to the container element. For example, to add
       an id to the container you can use ``container:id="my-id"``. Note that while you can pass a style string, it's
-      likely to be of little use with the default container style ``display: contents``. Most the the time you can just
+      likely to be of little use with the default container style ``display: contents``. Most of the time you can just
       do the styling on the component itself.
 
     For example::
 
         {% component 'core-ui' 'Button' ssr:disabled=True variant="Outlined"%}
             ...
         {% endcomponent %}
@@ -228,36 +243,22 @@
         return {
             # This value will be resolved by revivers.ComponentImport
             "component": self.component.source,
             "props": self.props,
         }
 
     def generate_code(self, generator: ComponentSourceCodeGenerator):
-        component = generator.resolve_component_import(self.component)
-        create_element = generator.resolve_prop_import(
-            ap_frontend_settings.REACT_RENDER_COMPONENT_FILE,
-            ImportSpecifier("createElementWithProps"),
-            import_order_priority=HIGHEST_PRIORITY_IMPORT,
-        )
-        return CallExpression(create_element, [component, self.props.generate_code(generator)])
-
-    def as_debug_string(self):
-        """Returns a string representation of this prop for debugging purposes
-
-        This is only used if you pass a component as a prop to another component. It's not used when
-        just nesting components - that's handled by `print_debug_tree` itself.
-        """
-        return self.component.print_debug_tree(self.props, suppress_origin=True)
+        return generator.create_jsx_element_node(self.component, self.props)
 
 
 PropType = str | float | int | list["PropType"] | tuple["PropType"] | dict[str, "PropType"] | ComponentProp
 PropsType = dict[str, PropType]
 
 
-class ComponentProps(SSRSerializable, CodeGeneratorNode):
+class ComponentProps(SSRSerializable):
     """Stores the props for a given component and handles serialization"""
 
     props: PropsType
 
     def __init__(self, props: PropsType):
         # Copy as ``add_prop`` modifies
         self.props = props.copy()
@@ -290,43 +291,14 @@
 
         Args:
             options: The options to use when serializing. In particular the options tell serialization how to handle
                 resolving imports when dealing with nested components.
         """
         return self._serialize_prop(self.props, ssr_context)
 
-    def _codegen_prop(self, value: PropType, generator: ComponentSourceCodeGenerator):
-        if isinstance(value, dict):
-            return {underscore_to_camel(k): self._codegen_prop(v, generator) for k, v in value.items()}
-        if isinstance(value, (list, tuple)):
-            return [self._codegen_prop(v, generator) for v in value]
-        if isinstance(value, CodeGeneratorNode):
-            return value.generate_code(generator)
-        if isinstance(value, ImportComponentSource):
-            # This lets us pass through imports as props, for example to pass a component class itself as a prop to
-            # another component
-            return generator.resolve_prop_import(
-                value.path,
-                (
-                    ImportDefaultSpecifier(value.import_name)
-                    if value.is_default_import
-                    else ImportSpecifier(value.import_name)
-                ),
-            )
-        return value
-
-    def generate_code(self, generator: ComponentSourceCodeGenerator):
-        try:
-            return self.convert_to_node(self._codegen_prop(self.props, generator), generator)
-        except UnconvertibleValueException as e:
-            raise ValueError(
-                f"Do not know how to handle prop of type {type(e.value)}: {e.value}\n\n "
-                "Either add a handler to ALLIANCE_PLATEFORM['FRONTEND']['REACT_PROP_HANDLERS'] or check the correct value is being passed in."
-            )
-
     def has_prop(self, prop_name: str):
         return prop_name in self.props
 
     def add_prop(self, prop_name: str, value: PropType):
         """Add a new prop"""
         self.props[prop_name] = value
 
@@ -449,25 +421,28 @@
         ]
     """
 
     #: Used internally to track where the current registry is stored in ``Context``
     context_key = "__NestedComponentPropAccumulator"
     #: The stored props as a mapping from the rendered placeholder string, to the ``NestedComponentProp``.
     props: dict[str, NestedComponentProp]
+    #: The origin component node
+    origin_node: ComponentNode
 
     @classmethod
     def get_current(cls, context: Context) -> NestedComponentPropAccumulator | None:
         """Get the current accumulator, if any
 
         This extracts the current accumulator instance from the template context. Returns ``None``
         if there is no active accumulator.
         """
         return context.get(cls.context_key, None)
 
-    def __init__(self, context: Context):
+    def __init__(self, context: Context, origin_node: ComponentNode):
+        self.origin_node = origin_node
         self.context = context
         self.props = {}
 
     def __enter__(self):
         # push current context; matching pop is in ``__exit__``
         self.context.push()
         # store this instance in context
@@ -523,23 +498,31 @@
                     continue
                 if index > prev_index:
                     part = value[prev_index:index]
                     if part:
                         children.append(part)
                 children.append(prop)
                 prev_index = index + len(placeholder)
-            sub_value = value[prev_index:]
-            if sub_value:
-                children.append(sub_value)
-        elif value:
-            children.append(value)
+            value = value[prev_index:]
+        if value:
+            children += self.transform_string(value)
         self.props = {}
 
         return children
 
+    def transform_string(self, child: str | NestedComponentProp):
+        """Given a string, handle any necessary HTML conversions for React compatibility."""
+        if isinstance(child, SafeString):
+            return convert_html_string(
+                child,
+                self.origin_node.origin,
+                wrap_new_node=lambda node: NestedComponentProp(node, self.origin_node, self.context),
+            )
+        return [child]
+
 
 class ComponentSourceCodeGenerator:
     """Helper class to assist in generating source for a component tag
 
     This uses a ``TypescriptSourceFileWriter`` to generate the source code for a component tag but
     provides some additional helpers to make it easier to generate the source.
 
@@ -557,20 +540,20 @@
           true
         );
 
     With a wrapper component::
 
         import { TestComponent } from "http://localhost:5173/assets/frontend/src/components/TestComponent.tsx";
         import {
-          createElementWithProps,
+          createElement,
           renderComponent,
         } from "http://localhost:5173/assets/frontend/src/renderComponent.tsx";
 
         function Wrapper() {
-          return createElementWithProps(TestComponent, {});
+          return createElement(TestComponent, {});
         }
 
         renderComponent(
           document.querySelector("[data-djid='6144913408__1_3']"),
           Wrapper,
           {},
           "6144913408__1_3",
@@ -579,26 +562,45 @@
 
     The second form is only required if one of the props needs to use a React hook (e.g. ``useViewModelCache``).
     """
 
     bundler: BaseBundler
     node: ComponentNode
 
+    #: If a wrapper component is required. This is set by ``requires_wrapper_component``.
     _requires_wrapper_component: bool
+    #: Tracks the name of all identifiers generated so far. This is used to ensure uniqueness.
     _used_identifiers: list[str]
+    #: Used by ``create_jsx_element`` to detect when the template name changes so it can output a comment.
+    _last_template_origin_name: str | None
+    #: Used by ``create_jsx_element`` to track the specified value for the ``include_template_origin`` kwarg in the root node
+    _last_include_template_origin: bool
+    #: Any nodes that should be added to the start of the generated content. This can be used by ``ComponentProp`` handlers to add code outside the component.
+    #: For example, populating a cache should be done once and not on every render.
     _leading_nodes: list[Node]
 
     def __init__(self, node: ComponentNode):
         self.node = node
         self.bundler = node.bundler
-        self._writer = TypescriptSourceFileWriter(resolve_import_url=self._resolve_import_url)
+        self._writer = TypescriptSourceFileWriter(
+            resolve_import_url=self._resolve_import_url,
+        )
         self._requires_wrapper_component = False
         self._used_identifiers = []
+        self._last_template_origin_name = None
+        self._last_include_template_origin = False
         self._leading_nodes = []
 
+        # Resolve the import for createElement and use the returned Identifier for the jsx_transform
+        self._writer.jsx_transform = self._writer.resolve_import(
+            ap_frontend_settings.REACT_RENDER_COMPONENT_FILE,
+            ImportSpecifier("createElement"),
+            import_order_priority=HIGHEST_PRIORITY_IMPORT,
+        )
+
     def _resolve_import_url(self, path: Path | str):
         path = self.bundler.validate_path(path, resolve_extensions=[".ts", ".tsx"])
         return self.bundler.get_url(path)
 
     def resolve_component_import(self, component: ComponentNode):
         """Resolve import to use for a component."""
         if isinstance(component.source, ImportComponentSource):
@@ -633,47 +635,134 @@
         are tracked separated and added to the dynamic dependencies of the component. This allows the ``BundlerContext``
         to check this assets will be available in production and raise an error if not.
         """
         self.node.add_dynamic_dependency(self.bundler.validate_path(path, resolve_extensions=[".ts", ".tsx"]))
         return self._writer.resolve_import(path, specifier, import_order_priority=import_order_priority)
 
     def requires_wrapper_component(self):
-        """Indicate that a wrapper component is required to render this component. This is required when using hooks."""
+        """Indicate that a wrapper component is required to render this component. This is required when using hooks.
+
+        ``ComponentProp`` instances can call this method to indicate that a wrapper component is required.
+        """
         self._requires_wrapper_component = True
 
+    def _codegen_prop(self, value: PropType):
+        if isinstance(value, dict):
+            return {underscore_to_camel(k): self._codegen_prop(v) for k, v in value.items()}
+        if isinstance(value, (list, tuple)):
+            return [self._codegen_prop(v) for v in value]
+        if isinstance(value, CodeGeneratorNode):
+            return value.generate_code(self)
+        if isinstance(value, ImportComponentSource):
+            # This lets us pass through imports as props, for example to pass a component class itself as a prop to
+            # another component
+            return self.resolve_prop_import(
+                value.path,
+                (
+                    ImportDefaultSpecifier(value.import_name)
+                    if value.is_default_import
+                    else ImportSpecifier(value.import_name)
+                ),
+            )
+        return convert_to_node(value)
+
+    def create_jsx_element_node(
+        self, component: ComponentNode, resolved_props: ComponentProps, include_template_origin=None
+    ):
+        """
+        Create a JSX element node for the specified component and props
+
+        Note that this creates the representation of the component as a JSX element. The TypescriptPrinter will
+        then convert it to code, either as JSX directly for debugging, or as React.createElement calls for code
+        outputted to the browser (JSX can't be interpreted directly in the browser, but is very useful for debugging
+        or test cases).
+
+        Args:
+            component: The component node to create the JSX element for
+            resolved_props: The fully resolved props for the component
+            include_template_origin: Whether to include a comment for each component indicating the template it was
+                created from. Useful for debugging.
+
+        Returns:
+            A ``JsxElement`` that can be printed to code.
+        """
+
+        # If not specified, use the last value. This is useful for nested elements to use the value specified on the
+        # root node.
+        if include_template_origin is None:
+            include_template_origin = self._last_include_template_origin
+        last_include_template_origin = self._last_include_template_origin
+        self._last_include_template_origin = include_template_origin
+
+        # Track the template name so we know when it changes. This way we only output the template name when it changes.
+        last_template_name = self._last_template_origin_name
+        template_name = (
+            component.origin.template_name.decode()
+            if isinstance(component.origin.template_name, bytes)
+            else component.origin.template_name
+        )
+        self._last_template_origin_name = template_name
+
+        try:
+            children = cast(
+                list[NestedComponentProp | str] | str | NestedComponentProp,
+                resolved_props.props.get("children", []),
+            )
+            attributes = [
+                JsxAttribute(
+                    StringLiteral(key.lower()) if "-" in key else Identifier(underscore_to_camel(key)),
+                    self._codegen_prop(prop),
+                )
+                for key, prop in resolved_props.props.items()
+                if key != "children"
+            ]
+            jsx_children = [
+                self._codegen_prop(child)
+                for child in ([children] if not isinstance(children, list) else children)
+            ]
+            leading_comments = None
+            if include_template_origin and template_name and template_name != last_template_name:
+                leading_comments = [MultiLineComment(template_name)]
+            return JsxElement(
+                self.resolve_component_import(component),
+                attributes,
+                jsx_children,
+                leading_comments=leading_comments,
+            )
+        except UnconvertibleValueException as e:
+            raise ValueError(
+                f"Do not know how to handle prop of type {type(e.value)}: {e.value}\n\n "
+                "Either add a handler to ALLIANCE_PLATEFORM['FRONTEND']['REACT_PROP_HANDLERS'] or check the correct value is being passed in."
+            )
+        finally:
+            self._last_template_origin_name = last_template_name
+            self._include_template_origin = last_include_template_origin
+
     def generate_code(self, props: ComponentProps, container_id: str):
-        props_node = props.generate_code(self)
-        component_id = self.resolve_component_import(self.node)
+        jsx_element = self.create_jsx_element_node(self.node, props)
+
+        # This needs to happen after the jsx_element is created, as that is where props are processed that may trigger
+        # leading nodes to be added
         for node in self._leading_nodes:
             self._writer.add_node(node)
+
+        # In some cases a wrapper component is needed, e.g. when using props that require hooks. This just wraps
+        # the element in a wrapper function and returns the element. The props themselves may be a hook call, so we
+        # don't have to specifically check for hooks here.
         if self._requires_wrapper_component:
             wrapper_id = Identifier("Wrapper")
             self._writer.add_node(
                 FunctionDeclaration(
                     wrapper_id,
                     [],
-                    [
-                        ReturnStatement(
-                            CallExpression(
-                                self._writer.resolve_import(
-                                    ap_frontend_settings.REACT_RENDER_COMPONENT_FILE,
-                                    ImportSpecifier("createElementWithProps"),
-                                    import_order_priority=HIGHEST_PRIORITY_IMPORT,
-                                ),
-                                [
-                                    component_id,
-                                    props_node,
-                                ],
-                            )
-                        )
-                    ],
+                    [ReturnStatement(jsx_element)],
                 )
             )
             component_id = wrapper_id
-            props_node = {}
+            jsx_element = JsxElement(component_id, [], [])
         self._writer.add_node(
             CallExpression(
                 self._writer.resolve_import(
                     ap_frontend_settings.REACT_RENDER_COMPONENT_FILE,
                     ImportSpecifier("renderComponent"),
                     import_order_priority=HIGHEST_PRIORITY_IMPORT,
                 ),
@@ -681,16 +770,15 @@
                     CallExpression(
                         PropertyAccessExpression(
                             Identifier("document"),
                             Identifier("querySelector"),
                         ),
                         [f"[data-djid='{container_id}']"],
                     ),
-                    component_id,
-                    props_node,
+                    jsx_element,
                     container_id,
                     not self.node.ssr_disabled,
                 ],
             )
         )
         return self._writer.get_code()
 
@@ -794,14 +882,19 @@
 
             processed_children.append(item)
     if current_str:
         processed_children.append(current_str)
     return processed_children
 
 
+# Used to identify children when processing them in resolve_props
+class ChildrenList(list):
+    pass
+
+
 class ComponentNode(template.Node, BundlerAsset):
     """A template node used by :func:`~alliance_platform.frontend.templatetags.react.component`"""
 
     #: Any extra dependencies for this component. This comes from props used that may require imports, for example
     #: DateProp may require the date library be included.
     dynamic_dependencies: list[Path]
 
@@ -819,14 +912,16 @@
         container_tag: str | FilterExpression = "dj-component",
         container_props: dict[str, Any] | None = None,
     ):
         if not ap_frontend_settings.REACT_RENDER_COMPONENT_FILE:
             raise ImproperlyConfigured(
                 "When using the `react` tag you must have `REACT_RENDER_COMPONENT_FILE` set in ALLIANCE_PLATFORM['FRONTEND'] settings"
             )
+        if "children" in props:
+            props["children"] = ChildrenList(props["children"])
         self.container_tag = container_tag
         self.container_props = container_props or {}
         self.ssr_disabled = ssr_disabled
         self.source = source
         self.props = props
         self.target_var = target_var
         self.omit_if_empty = omit_if_empty
@@ -864,48 +959,47 @@
         """Handles resolving values to a type that can be serialized
 
         If you add new :class:`~alliance_platform.frontend.prop_handlers.ComponentProp` there must a case here
         to convert values to the new type.
         """
         if isinstance(value, DeferredProp):
             value = value.resolve(context)
-        if isinstance(value, NodeList):
-            # If it's a NodeList it must be tag children
+        if isinstance(value, (ChildrenList, NodeList)):
             children: list[str | NestedComponentProp] = []
             for child in value:
                 if isinstance(child, ComponentNode):
                     # We could remove this branch - it's an optimisation of the below. We know the node type here
                     # directly so can avoid the extra work + string replacement that happens below.
                     try:
                         children.append(NestedComponentProp(child, self, context))
                     except OmitComponentFromRendering:
                         pass
                 else:
-                    with NestedComponentPropAccumulator(context) as accumulator:
+                    with NestedComponentPropAccumulator(context, self) as accumulator:
                         # This will be a string but there may have been components that render (e.g. within
                         # other django tags like {% if %}, or from template inheritance and rendering into a
                         # block contained within a component).
-                        child_value: str = child.render(context)
+                        child_value: str = child if isinstance(child, str) else child.render(context)
                         if child_value:
                             children += accumulator.apply(child_value)
 
             children = process_component_children(children)
 
             if self.omit_if_empty and not children:
                 raise OmitComponentFromRendering()
 
             # Many things only expect a single child so handle that as a default. This isn't necessary as we handle
-            # it in createElementWithProps but makes for slightly more readable code so leaving it in.
+            # it in our calls to createElement, but makes for slightly more readable code so leaving it in.
             if len(children) == 1:
                 return children[0]
 
             # NOTE: I removed this as we can handle it on the frontend by passing `children` through as a spread to
-            # `React.createElement` which tells it the children are static. See `createElementWithProps` for where this
-            # occurs. Adding keys here did cause some problems - namely with the `Cell` component in `Table`; navigation
-            # with keyboard across rows broke.
+            # `React.createElement` which tells it the children are static. See ``ComponentSourceCodeGenerator.create_jsx_element_node``
+            # for where this occurs. Adding keys here did cause some problems - namely with the `Cell` component in
+            # `Table`; navigation with keyboard across rows broke.
             # for i, child in enumerate(children):
             #     if isinstance(child, required_imports) and not child.props.has_prop("key"):
             #         child.props.add_prop("key", i)
 
             return children
         # This won't be true for props that come from ``extra_props`` as it's already a dict before passed to the template
         # tag (the ``extra_props`` var itself is resolved in ``resolve_props``)
@@ -982,76 +1076,35 @@
 
     def render(self, context: Context):
         try:
             return self.render_component(context)
         except OmitComponentFromRendering:
             return ""
 
-    def print_debug_tree(
-        self, props: ComponentProps, level=0, last_template_name=None, suppress_origin=False
-    ):
+    def print_debug_tree(self, props: ComponentProps, include_template_origin=True):
         """Print a debug tree of the component and its children.
 
         This renders to look like JSX with comments indicating which templates are used to render the component::
 
             { /* django/forms/widgets/select.html */ }
             <DjangoWidgetWrapper name="is_active">
               <Select >
                 {/* django/forms/widgets/select_option.html */ }
                 <Item key="unknown">
                   --------
                 </Item>
               </Select>
             </DjangoWidgetWrapper>
         """
-        attrs = {}
-        children = []
-        for name, value in props.props.items():
-            if name == "children":
-                _raw_prop = value
-                raw_prop: list[PropType]
-                if not isinstance(_raw_prop, (list, tuple)):
-                    raw_prop = [cast(PropType, _raw_prop)]
-                else:
-                    raw_prop = cast(list[PropType], _raw_prop)
-                for i, child in enumerate(raw_prop):
-                    if isinstance(child, NestedComponentProp):
-                        children.append(
-                            child.component.print_debug_tree(
-                                child.props, level + 1, self.origin.template_name, suppress_origin=i > 0
-                            )
-                        )
-                    else:
-                        if isinstance(child, str):
-                            child = child.strip()
-                        if child:
-                            children.append(child)
-            else:
-                if isinstance(value, ComponentProp):
-                    value = f"{{{value.as_debug_string()}}}"
-                elif isinstance(value, str):
-                    value = f'"{value}"'
-                else:
-                    value = f"{{{value}}}"
-                attrs[name] = value
-        indent = "  " * level
-        child_indent = "  " * (level + 1)
-        children_str = child_indent + f"\n{child_indent}".join(children)
-        attr_str = " ".join(f"{name}={value}" for name, value in attrs.items())
-        template_name = self.origin.template_name
-        if isinstance(template_name, bytes):
-            template_name = template_name.decode("utf8")
-        if not suppress_origin and template_name and template_name != last_template_name:
-            origin = f"{{/* {template_name} */ }}\n{indent}"
-        else:
-            origin = ""
-        open_tag = f"{origin}<{self.source.as_tag()} {attr_str}>"
-        if not children:
-            return f"{open_tag[:-1]} />"
-        return f"""{open_tag}\n{children_str}\n{indent}</{self.source.as_tag()}>"""
+        # Disable jsx_transform so raw JSX is outputted rather than React.createElement calls
+        printer = TypescriptPrinter(jsx_transform=None)
+        generator = ComponentSourceCodeGenerator(self)
+        jsx_element = generator.create_jsx_element_node(self, props, include_template_origin)
+
+        return self.bundler.format_code(printer.print(jsx_element))
 
 
 @register.simple_tag()
 def react_refresh_preamble():
     """Add `react-refresh <https://www.npmjs.com/package/react-refresh>`_ support
 
     Currently only works with :class:`~alliance_platform.frontend.bundler.vite.ViteBundler`.
@@ -1325,23 +1378,163 @@
                 namespaced_options[namespace][key] = v
     container_props = {**(container_props or {}), **namespaced_options["container"]}
     ssr_options = namespaced_options["ssr"]
     component_options = namespaced_options["component"]
     container_tag = container_props.pop("tag", container_tag)
     props = props.copy() if props else {}
     props.update({key: value for key, value in kwargs.items() if key not in exclude_keys})
-    if nodelist:
-        props["children"] = nodelist
     origin = parser.origin or Origin(UNKNOWN_SOURCE)
+    if nodelist:
+        # Convert the nodelist to a string with placeholders for the template nodes. This is then processed for HTML
+        # contained within ``TextNode``s, before converting back to a list of nodes with any placeholders replaced with
+        # the original template nodes. This allows us to handle HTML being passed to component children directly without
+        # having to use __dangerouslySetInnerHTML.
+        i = 0
+        html = ""
+        replacements: dict[str, Node] = {}
+        for node in nodelist:
+            if isinstance(node, TextNode):
+                html += node.s
+            else:
+                placeholder = _html_replacement_placeholder_template.format(i)
+                html += placeholder
+                replacements[str(i)] = node
+                i += 1
+        props["children"] = convert_html_string(html, origin, replacements=replacements)
     if asset_source is None:
         asset_source = get_component_source_from_tag_args(args, tag_name, origin)
 
     return node_class(
         origin,
         asset_source,
         props,
         target_var=target_var,
         container_tag=container_tag,
         container_props=container_props,
         ssr_disabled=ssr_options.get("disabled", ssr_disabled),
         omit_if_empty=component_options.get("omit_if_empty", omit_if_empty),
     )
+
+
+# These are used to replace template Nodes in a string with placeholders. The resulting string can them be parsed as HTML,
+# and then the placeholders replaced with the original template nodes.
+_html_replacement_placeholder_prefix = "_______PLACEHOLDER_____$"
+_html_replacement_placeholder_suffix = "$_"
+_html_replacement_placeholder_template = (
+    _html_replacement_placeholder_prefix + "{0}" + _html_replacement_placeholder_suffix
+)
+
+
+@dataclass
+class Element:
+    name: str
+    attrs: dict
+
+
+@dataclass
+class HTMLElement:
+    tag: str
+    attributes: dict[str, str] = field(default_factory=dict)
+    children: list[Union["HTMLElement", str]] = field(default_factory=list)
+
+
+class HtmlTreeParser(HTMLParser):
+    def __init__(self):
+        super().__init__(convert_charrefs=True)
+        # The root of the parsed tree. The tag is nonsense, but not used - it's just to make implementation easier. We
+        # just use it for ``children``
+        self.root = HTMLElement("Root")
+        # Stack to maintain hierarchy of elements
+        self.stack = [self.root]
+
+    def handle_starttag(self, tag, attrs):
+        element = HTMLElement(tag, {attr[0]: attr[1] for attr in attrs})
+        if self.stack:
+            self.stack[-1].children.append(element)
+        else:
+            self.root = element
+        self.stack.append(element)
+
+    def handle_endtag(self, tag):
+        if self.stack and self.stack[-1].tag == tag:
+            self.stack.pop()
+
+    def handle_data(self, data):
+        if data and self.stack:
+            self.stack[-1].children.append(data)
+
+
+def convert_html_string(
+    html: str,
+    origin: Origin,
+    *,
+    replacements: dict[str, Node] | None = None,
+    wrap_new_node: Callable[[ComponentNode], ComponentNode | ComponentProp] = lambda x: x,
+):
+    """
+    Given a string that may contain HTML, convert it to a tree of ``ComponentNode``s
+
+    Args:
+        html: The html string to convert
+        origin: The template origin
+        replacements: Any replacements to make in the HTML after conversion. The way this works is that a template NodeList
+            is processed into a string, with any template nodes replaced with placeholders. The string is converted to
+            a component tree, then any placeholders are replaced with the original template nodes.
+        wrap_new_node:
+            Function to call to wrap any created ``ComponentNode``. This is used to wrap nodes in ``NestedComponentProp``
+            when they are children of another component. This isn't necessary for top-level nodes as they are handled
+            when ``parse_component_tag`` is first called.
+    Returns:
+
+    """
+    # NOTE: I tried lxml initially (with & without BeautifulSoup), and it was slower for our specific use case.
+    # In general, it's considered very fast, but we don't need most of its features and this simple parser was
+    # faster.
+    parser = HtmlTreeParser()
+    # Parse the HTML
+    parser.feed(html)
+
+    tags = parser.root.children
+
+    def handle_placeholders(content: str):
+        if not replacements:
+            return [content]
+        parts = content.split(_html_replacement_placeholder_prefix)
+        first = parts.pop(0)
+        if not parts:
+            return [first]
+        children: list[str | Node] = []
+        if first:
+            children.append(first)
+        for part in parts:
+            placeholder_id, extra = part.split(_html_replacement_placeholder_suffix)
+            children.append(replacements[placeholder_id])
+            if extra:
+                children.append(extra)
+        return children
+
+    def convert_attributes(attrs: dict[str, str | Any]):
+        transformed = {}
+        for key, value in attrs.items():
+            parts = handle_placeholders(value)
+            transformed[key] = parts[0] if len(parts) == 1 else NodeList(parts)
+        return transformed
+
+    def convert_tree(tree):
+        children = []
+        for el in tree:
+            if isinstance(el, str):
+                parts = handle_placeholders(el)
+                children += parts
+            else:
+                children.append(
+                    wrap_new_node(
+                        ComponentNode(
+                            origin,
+                            CommonComponentSource(el.tag),
+                            {**convert_attributes(el.attributes), "children": convert_tree(el.children)},
+                        )
+                    )
+                )
+        return children
+
+    return convert_tree(tags)
```

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/templatetags/vanilla_extract.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/templatetags/vanilla_extract.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/alliance_platform/frontend/util.py` & `alliance_platform_frontend-0.0.5/alliance_platform/frontend/util.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/pyproject.toml` & `alliance_platform_frontend-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Typing :: Typed",
 ]
 include = [
     "alliance_platform/frontend/py.typed",
 ]
-version = "0.0.4"
+version = "0.0.5"
 
 [project.license]
 text = "BSD-2-Clause"
 
 [project.urls]
 issues = "https://github.com/AllianceSoftware/alliance-platform-py/issues"
 homepage = "https://github.com/AllianceSoftware/alliance-platform-py/packages/ap-frontend"
```

### Comparing `alliance_platform_frontend-0.0.4/tests/fixtures/build_test/manifest.json` & `alliance_platform_frontend-0.0.5/tests/fixtures/build_test/manifest.json`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/tests/fixtures/server_build_test/manifest.json` & `alliance_platform_frontend-0.0.5/tests/fixtures/server_build_test/manifest.json`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/tests/test_alliance_ui_templatetags.py` & `alliance_platform_frontend-0.0.5/tests/test_alliance_ui_templatetags.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/tests/test_bundler.py` & `alliance_platform_frontend-0.0.5/tests/test_bundler.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from alliance_platform.frontend.bundler.base import SourceDirResolver
 from alliance_platform.frontend.bundler.base import html_target_browser
 from alliance_platform.frontend.bundler.vite import ViteBundler
 from django.conf import settings
 from django.test import TestCase
 from django.test import override_settings
 
+from tests.test_utils import override_ap_frontend_settings
+
 
 class TestBundler(TestCase):
     def test_relative_path_resolver(self):
         resolver = RelativePathResolver()
         # Can't resolve if no source_path specifier in context
         self.assertEqual(None, resolver.resolve("./test", ResolveContext(Path("/root"))))
 
@@ -54,14 +56,23 @@
         )
         self.assertEqual(
             None,
             resolver.resolve("/project/test.ts", ResolveContext(Path("/root"))),
         )
 
 
+class MockRequestResponse:
+    def __init__(self, json_data, status_code):
+        self.json_data = json_data
+        self.status_code = status_code
+
+    def json(self):
+        return self.json_data
+
+
 class TestViteBundler(ViteBundler):
     def validate_path(
         self,
         filename: str | Path,
         suffix_whitelist: list[str] | None = None,
         suffix_hint: str | None = None,
         resolve_extensions: list[str] | None = None,
@@ -269,7 +280,35 @@
 
     def test_resolve_ssr_import_path(self):
         bundler = self.create_bundler()
         self.assertEqual(
             bundler.server_build_dir / "Button.mjs",
             bundler.resolve_ssr_import_path("components/Button.tsx"),
         )
+
+    def test_format_code_size_limit(self):
+        bundler = self.create_bundler(mode="development")
+
+        def mocked_post(*args, **kwargs):
+            return MockRequestResponse({"code": "formatted"}, 200)
+
+        with mock.patch("requests.post", side_effect=mocked_post):
+            self.assertEqual(bundler.format_code("a short string"), "formatted")
+            long_string = "." * 1024 * 1024
+            self.assertEqual(bundler.format_code(long_string), long_string)
+            with override_ap_frontend_settings(DEV_CODE_FORMAT_LIMIT=0):
+                self.assertEqual(bundler.format_code(long_string), "formatted")
+
+    def test_format_code_timeout(self):
+        bundler = self.create_bundler(mode="development")
+
+        def mocked_post(*args, **kwargs):
+            return MockRequestResponse({"code": "formatted"}, 200)
+
+        with mock.patch("requests.post", side_effect=mocked_post) as mock_send:
+            bundler.format_code("code")
+            self.assertEqual(mock_send.call_args.kwargs.get("timeout"), 1)
+
+        with mock.patch("requests.post", side_effect=mocked_post) as mock_send:
+            with override_ap_frontend_settings(DEV_CODE_FORMAT_TIMEOUT=10):
+                bundler.format_code("code")
+                self.assertEqual(mock_send.call_args.kwargs.get("timeout"), 10)
```

### Comparing `alliance_platform_frontend-0.0.4/tests/test_bundler_templatetags.py` & `alliance_platform_frontend-0.0.5/tests/test_bundler_templatetags.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 import datetime
 import json
 from typing import cast
 from unittest import mock
 
+from alliance_platform.codegen.printer import TypescriptPrinter
 from alliance_platform.frontend.bundler.base import HtmlGenerationTarget
 from alliance_platform.frontend.bundler.context import BundlerAssetContext
 from alliance_platform.frontend.bundler.ssr import SSRJsonEncoder
 from alliance_platform.frontend.bundler.ssr import SSRSerializerContext
 from alliance_platform.frontend.bundler.vanilla_extract import resolve_vanilla_extract_cache_names
 from alliance_platform.frontend.templatetags.react import ComponentNode
+from alliance_platform.frontend.templatetags.react import ComponentProps
+from alliance_platform.frontend.templatetags.react import ComponentSourceCodeGenerator
 from django.conf import settings
 from django.template import Context
 from django.template import Template
 from django.test import SimpleTestCase
 from django.test import override_settings
+from django.utils.functional import SimpleLazyObject
+from django.utils.functional import lazy
+from django.utils.safestring import mark_safe
 from django.utils.timezone import make_aware
 
 from .test_utils import override_ap_frontend_settings
 from .test_utils.bundler import TestViteBundler
 from .test_utils.bundler import bundler_kwargs
 from .test_utils.bundler import bypass_frontend_asset_registry
 from .test_utils.bundler import fixtures_dir
 from .test_utils.bundler import format_code
+from .test_utils.bundler import run_prettier
 
 inline_css_prod = {
     fixtures_dir / "build_test/assets/Button-abc123.css": ".prod_button { color: red; }",
 }
 
 
 def mock_read_text(path):
@@ -332,15 +339,15 @@
                     self.assertEqual(
                         expected,
                         actual,
                     )
 
 
 @override_ap_frontend_settings(DEBUG_COMPONENT_OUTPUT=False)
-class TestComponentTemplateTag(SimpleTestCase):
+class TestComponentTemplateTagCodeGen(SimpleTestCase):
     def setUp(self) -> None:
         self.test_production_bundler = TestViteBundler(
             **bundler_kwargs,  # type: ignore[arg-type]
             mode="production",
         )
 
         self.test_development_bundler = TestViteBundler(
@@ -364,35 +371,39 @@
         for bundler_name, expected in [
             # Resolved from fixtures dir / development-css-mappings
             (
                 "test_development_bundler",
                 f"""
                     <dj-component data-djid="C1"><!-- ___SSR_PLACEHOLDER_0___ --></dj-component>
                     <script type="module">
-                        import {{ renderComponent }} from '{self.dev_url}frontend/src/renderComponent.tsx';
+                        import {{ createElement, renderComponent }} from '{self.dev_url}frontend/src/renderComponent.tsx';
                         import Button, {{  }} from '{self.dev_url}components/Button.tsx';
                         renderComponent(
                           document.querySelector("[data-djid='C1']"),
-                          Button,
-                          {{ children: "Click Me" }},
+                          createElement(Button, {{}}, "Click Me"),
                           "C1",
                           true
                         );
                     </script>
                 """,
             ),
             # Resolved from fixtures dir / production-css-mappings
             (
                 "test_production_bundler",
                 """
                     <dj-component data-djid="C1"><!-- ___SSR_PLACEHOLDER_0___ --></dj-component>
                     <script type="module">
-                        import { renderComponent } from '/static/assets/renderComponent-e1.js';
+                        import { createElement, renderComponent } from '/static/assets/renderComponent-e1.js';
                         import Button, {  } from '/static/assets/Button-def456.js';
-                        renderComponent(document.querySelector("[data-djid='C1']"), Button, {children: "Click Me"}, "C1", true)
+                        renderComponent(
+                            document.querySelector("[data-djid='C1']"),
+                            createElement(Button, {}, "Click Me"),
+                            "C1",
+                            true
+                        );
                     </script>
                 """,
             ),
         ]:
             with mock.patch(
                 "alliance_platform.frontend.bundler.middleware.BundlerAssetContext.generate_id"
             ) as mock_method:
@@ -433,21 +444,20 @@
                     context = Context()
                     actual = tpl.render(context)
                     self.assertCodeEqual(
                         actual,
                         """
                         <dj-component data-djid="C1"><!-- ___SSR_PLACEHOLDER_0___ --></dj-component>
                         <script type="module">
-                            import { createElementWithProps, renderComponent } from "%sfrontend/src/renderComponent.tsx";
+                            import { createElement, renderComponent } from "%sfrontend/src/renderComponent.tsx";
                             import Button from "%scomponents/Button.tsx";
 
                             renderComponent(
                               document.querySelector("[data-djid='C1']"),
-                              Button,
-                              { children: ["Click ", createElementWithProps("strong", {children: "Me"})] },
+                              createElement(Button, {}, "Click ", createElement("strong", {}, "Me")),
                               "C1",
                               true
                             );
                         </script>
                         """
                         % (
                             self.dev_url,
@@ -536,15 +546,15 @@
                                 "aria-label": "Click Me",
                                 "date": datetime.date(2022, 12, 1),
                             }
                         }
                     )
                     actual = tpl.render(context)
                     self.assertIn(
-                        """renderComponent(document.querySelector("[data-djid='C1']"), "button", {disabled: true, children: "Click", "aria-label": "Click Me", date: new CalendarDate(2022, 12, 1)}, "C1", true)""",
+                        """renderComponent(document.querySelector("[data-djid='C1']"), createElement("button", {disabled: true, "aria-label": "Click Me", date: new CalendarDate(2022, 12, 1)}, "Click"), "C1", true)""",
                         actual,
                     )
 
     def assertSerializedPropsEqual(self, template_contents: str, context: dict, expected_props: dict):
         """Helper to compare props generated for a components
 
         Args:
@@ -710,7 +720,208 @@
                                     "@@CUSTOM",
                                     "Component",
                                     {"component": "b", "props": {"children": "Test True 5   "}},
                                 ],
                             ]
                         },
                     )
+
+
+test_development_bundler = TestViteBundler(
+    **bundler_kwargs,  # type: ignore[arg-type]
+    mode="development",
+)
+
+
+@override_ap_frontend_settings(
+    # We rely on this in _get_debug_tree
+    DEBUG_COMPONENT_OUTPUT=True,
+    BUNDLER=test_development_bundler,
+)
+class TestComponentTemplateTagOutput(SimpleTestCase):
+    """For ease of testing, these tests just use the pretty debug output for comparing code
+
+    For testing the actual codegen itself, see the above tests
+    """
+
+    def setUp(self):
+        self.bundler_context = BundlerAssetContext(
+            frontend_asset_registry=bypass_frontend_asset_registry, skip_checks=True
+        )
+        self.bundler_context.__enter__()
+
+    def tearDown(self):
+        self.bundler_context.__exit__(None, None, None)
+
+    def _get_debug_tree(self, template_contents: str, **kwargs: dict):
+        def patch_debug_tree(self, props: ComponentProps, include_template_origin=True):
+            # Like the default implementation except we never include template origin string
+            printer = TypescriptPrinter(jsx_transform=None)
+            generator = ComponentSourceCodeGenerator(self)
+            jsx_element = generator.create_jsx_element_node(self, props, False)
+            return printer.print(jsx_element)
+
+        with mock.patch(
+            "alliance_platform.frontend.templatetags.react.ComponentNode.print_debug_tree", patch_debug_tree
+        ):
+            template = Template("{% load react %}" + template_contents)
+            context = Context(kwargs)
+            context.template = template
+            contents = template.render(context)
+            code = contents.split("<!--").pop().split("-->").pop(0)
+            return code.strip()
+
+    def assertComponentEqual(self, template_code, expected_output, **kwargs):
+        self.assertEqual(
+            run_prettier(self._get_debug_tree(template_code, **kwargs)),
+            run_prettier(expected_output),
+        )
+
+    def test_django_lazy_object_as_prop(self):
+        def get_token():
+            return "abc123"
+
+        token = lazy(get_token, str)
+        self.assertComponentEqual(
+            """{% component "CustomForm" csrf_token=csrf_token %}{% endcomponent %}""",
+            """
+            <CustomForm csrfToken="abc123" />
+            """,
+            csrf_token=token,
+        )
+
+    def test_django_simple_lazy_object_as_prop(self):
+        def get_token():
+            return "abc123"
+
+        token = SimpleLazyObject(get_token)
+        self.assertComponentEqual(
+            """{% component "CustomForm" csrf_token=csrf_token %}{% endcomponent %}""",
+            """
+            <CustomForm csrfToken="abc123" />
+            """,
+            csrf_token=token,
+        )
+
+    def test_variable_string_concat(self):
+        self.assertComponentEqual(
+            """{% component "Button" %}Hello {{ name }}{% endcomponent %}""",
+            """
+            <Button>
+              Hello Sam
+            </Button>
+            """,
+            name="Sam",
+        )
+
+    def test_boolean_attribute(self):
+        self.assertComponentEqual(
+            """{% component "Button" is_disabled=True %}Disabled{% endcomponent %}""",
+            """<Button isDisabled={true}>Disabled</Button>""",
+        )
+
+    def test_string_attribute(self):
+        self.assertComponentEqual(
+            """{% component "Button" variant="primary" %}Click Me{% endcomponent %}""",
+            """<Button variant="primary">Click Me</Button>""",
+        )
+
+    def test_numeric_attribute(self):
+        self.assertComponentEqual(
+            """{% component "Range" min_value=5  %}{% endcomponent %}""",
+            """<Range minValue={5} />""",
+        )
+
+    def test_variable_attribute(self):
+        self.assertComponentEqual(
+            """{% component "Button" variant=variant %}Click Me{% endcomponent %}""",
+            """<Button variant="secondary">Click Me</Button>""",
+            variant="secondary",
+        )
+
+    def test_variable_attribute_raw_html(self):
+        self.assertComponentEqual(
+            """{% component "Button" %}Click <strong id="test-{{id}}">Me</strong>{% endcomponent %}""",
+            """<Button>Click <strong id="test-secondary">Me</strong></Button>""",
+            id="secondary",
+        )
+
+    def test_special_attribute(self):
+        self.assertComponentEqual(
+            """{% component "Button" aria-label="Disable" %}X{% endcomponent %}""",
+            """<Button aria-label="Disable">X</Button>""",
+        )
+
+    def test_html_entities(self):
+        self.assertComponentEqual(
+            """{% component "Button" %}&ldquo;Testing and Stuff&rdquo;{% endcomponent %}""",
+            """<Button>“Testing and Stuff”</Button>""",
+        )
+
+    def test_nested_component(self):
+        self.assertComponentEqual(
+            """{% component "Button" %}Welcome {% component "strong" %}{{ name }}{% endcomponent %}{% endcomponent %}""",
+            """<Button>Welcome <strong>Sam</strong></Button>""",
+            name="Sam",
+        )
+
+    def test_nested_component_raw_html(self):
+        self.assertComponentEqual(
+            """{% component "Button" %}Welcome <strong>{{ name }}</strong>{% endcomponent %}""",
+            """
+            <Button>Welcome <strong>Sam</strong></Button>
+            """,
+            name="Sam",
+        )
+
+    def test_nested_component_raw_html_from_include(self):
+        self.assertComponentEqual(
+            """{% component "Button" %}Welcome {% include "react_test_templates/nested_raw_tag.html" with name=name %}{% endcomponent %}""",
+            """
+            <Button>Welcome <strong>Sam</strong></Button>
+            """,
+            name="Sam",
+        )
+
+    def test_nested_component_from_include(self):
+        self.assertComponentEqual(
+            """{% component "Button" %}Welcome {% include "react_test_templates/nested_tag.html" with name=name %}{% endcomponent %}""",
+            """
+            <Button>Welcome <strong>Sam</strong></Button>
+            """,
+            name="Sam",
+        )
+
+    def test_template_include(self):
+        self.assertComponentEqual(
+            """{% component "Button" %}Hello {% include "react_test_templates/simple_include.html" %}{% endcomponent %}""",
+            """
+            <Button>
+              Hello Inner Content
+            </Button>
+            """,
+            name="Sam",
+        )
+
+    def test_pass_component_as_prop(self):
+        self.assertComponentEqual(
+            """
+            {% component "Icon" as icon %}{% endcomponent %}
+            {% component "Button" icon=icon %}Click{% endcomponent %}""",
+            """<Button icon={<Icon />}>Click</Button>""",
+            name="Sam",
+        )
+
+    def test_html_in_var(self):
+        self.assertComponentEqual(
+            """
+            {% component "div" %}{{ text }}{% endcomponent %}""",
+            """<div><strong>Should not be escaped</strong></div>""",
+            text=mark_safe("<strong>Should not be escaped</strong>"),
+        )
+
+        self.assertComponentEqual(
+            """
+            {% component "div" %}{{ text }}{% endcomponent %}""",
+            """<div>{'<strong>Should be escaped</strong>'}</div>""",
+            text="<strong>Should be escaped</strong>",
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alliance_platform_frontend-0.0.4/tests/test_context.py` & `alliance_platform_frontend-0.0.5/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/tests/test_utils/__init__.py` & `alliance_platform_frontend-0.0.5/tests/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.4/tests/test_utils/bundler.py` & `alliance_platform_frontend-0.0.5/tests/test_utils/bundler.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 
 
 def run_prettier(code):
     p = subprocess.run(
         [
             str(ap_frontend_settings.NODE_MODULES_DIR / ".bin/prettier"),
             "--stdin-filepath",
-            "test.ts",
+            "test.tsx",
         ],
         input=code,
         capture_output=True,
         text=True,
     )
     if p.returncode != 0:
-        raise ValueError("Failed to format code")
+        raise ValueError(f"Failed to format code: {p.stderr}")
     return p.stdout
 
 
 def format_code(code: str):
     # Format the contents of the script tag using the dev code formatter
     soup = BeautifulSoup(code, "html.parser")
     script_tag = soup.find("script")
```

### Comparing `alliance_platform_frontend-0.0.4/PKG-INFO` & `alliance_platform_frontend-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alliance-platform-frontend
-Version: 0.0.4
+Version: 0.0.5
 Summary: Django integration for Frontend Bundlers & React
 Keywords: django,alliance,alliancesoftware
 Home-page: https://github.com/AllianceSoftware/alliance-platform-py/packages/ap-frontend
 Author-Email: Alliance Software <support@alliancesoftware.com.au>
 License: BSD-2-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

