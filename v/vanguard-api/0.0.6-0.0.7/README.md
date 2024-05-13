# Comparing `tmp/vanguard_api-0.0.6.tar.gz` & `tmp/vanguard_api-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanguard_api-0.0.6.tar", last modified: Sat May 11 23:33:02 2024, max compression
+gzip compressed data, was "vanguard_api-0.0.7.tar", last modified: Mon May 13 11:04:32 2024, max compression
```

## Comparing `vanguard_api-0.0.6.tar` & `vanguard_api-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:33:02.700075 vanguard_api-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-11 23:32:59.000000 vanguard_api-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-11 23:33:02.700075 vanguard_api-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-11 23:32:59.000000 vanguard_api-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 23:33:02.700075 vanguard_api-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-11 23:32:59.000000 vanguard_api-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:33:02.700075 vanguard_api-0.0.6/vanguard/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-11 23:32:59.000000 vanguard_api-0.0.6/vanguard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-05-11 23:32:59.000000 vanguard_api-0.0.6/vanguard/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    13111 2024-05-11 23:32:59.000000 vanguard_api-0.0.6/vanguard/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     9322 2024-05-11 23:32:59.000000 vanguard_api-0.0.6/vanguard/session.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-11 23:32:59.000000 vanguard_api-0.0.6/vanguard/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:33:02.700075 vanguard_api-0.0.6/vanguard_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-11 23:33:02.000000 vanguard_api-0.0.6/vanguard_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-11 23:33:02.000000 vanguard_api-0.0.6/vanguard_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 23:33:02.000000 vanguard_api-0.0.6/vanguard_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-11 23:33:02.000000 vanguard_api-0.0.6/vanguard_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 23:33:02.000000 vanguard_api-0.0.6/vanguard_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:04:32.444222 vanguard_api-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-13 11:04:28.000000 vanguard_api-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-13 11:04:32.444222 vanguard_api-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-13 11:04:28.000000 vanguard_api-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 11:04:32.444222 vanguard_api-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-13 11:04:28.000000 vanguard_api-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:04:32.444222 vanguard_api-0.0.7/vanguard/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-13 11:04:28.000000 vanguard_api-0.0.7/vanguard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-05-13 11:04:28.000000 vanguard_api-0.0.7/vanguard/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13111 2024-05-13 11:04:28.000000 vanguard_api-0.0.7/vanguard/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9403 2024-05-13 11:04:28.000000 vanguard_api-0.0.7/vanguard/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-13 11:04:28.000000 vanguard_api-0.0.7/vanguard/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:04:32.444222 vanguard_api-0.0.7/vanguard_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-13 11:04:32.000000 vanguard_api-0.0.7/vanguard_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-13 11:04:32.000000 vanguard_api-0.0.7/vanguard_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 11:04:32.000000 vanguard_api-0.0.7/vanguard_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:04:32.000000 vanguard_api-0.0.7/vanguard_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-13 11:04:32.000000 vanguard_api-0.0.7/vanguard_api.egg-info/top_level.txt
```

### Comparing `vanguard_api-0.0.6/LICENSE` & `vanguard_api-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vanguard_api-0.0.6/PKG-INFO` & `vanguard_api-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vanguard-api
-Version: 0.0.6
+Version: 0.0.7
 Summary: An unofficial API for Vanguard Invest
 Home-page: https://github.com/MaxxRK/vanguard-api
-Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.6.tar.gz
+Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.7.tar.gz
 Author: MaxxRK
 Author-email: maxxrk@pm.me
 License: MIT
 Keywords: VANGUARD,API
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
```

### Comparing `vanguard_api-0.0.6/README.md` & `vanguard_api-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `vanguard_api-0.0.6/setup.py` & `vanguard_api-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="vanguard-api",
-    version="0.0.6",
+    version="0.0.7",
     author="MaxxRK",
     author_email="maxxrk@pm.me",
     description="An unofficial API for Vanguard Invest",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/MaxxRK/vanguard-api",
-    download_url="https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.6.tar.gz",
+    download_url="https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.7.tar.gz",
     keywords=["VANGUARD", "API"],
     install_requires=["playwright", "playwright-stealth"],
     packages=["vanguard"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Internet :: WWW/HTTP :: Session",
```

### Comparing `vanguard_api-0.0.6/vanguard/account.py` & `vanguard_api-0.0.7/vanguard/account.py`

 * *Files identical despite different names*

### Comparing `vanguard_api-0.0.6/vanguard/order.py` & `vanguard_api-0.0.7/vanguard/order.py`

 * *Files identical despite different names*

### Comparing `vanguard_api-0.0.6/vanguard/session.py` & `vanguard_api-0.0.7/vanguard/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,14 +173,17 @@
                 otp_cards = self.page.query_selector_all(
                     "xpath=//div[contains(text(), '***-***-')]"
                 )
                 for otp_card in otp_cards:
                     if otp_card.inner_text() == f"***-***-{last_four}":
                         otp_card.click()
                         break
+            except PlaywrightTimeoutError:
+                pass
+            try:
                 self.page.wait_for_selector(
                     "xpath=//div[contains(text(), 'Text')]", timeout=10000
                 ).click()
                 return True
             except PlaywrightTimeoutError:
                 if self.title is not None:
                     self.save_storage_state()
```

### Comparing `vanguard_api-0.0.6/vanguard_api.egg-info/PKG-INFO` & `vanguard_api-0.0.7/vanguard_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vanguard-api
-Version: 0.0.6
+Version: 0.0.7
 Summary: An unofficial API for Vanguard Invest
 Home-page: https://github.com/MaxxRK/vanguard-api
-Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.6.tar.gz
+Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.7.tar.gz
 Author: MaxxRK
 Author-email: maxxrk@pm.me
 License: MIT
 Keywords: VANGUARD,API
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
```

