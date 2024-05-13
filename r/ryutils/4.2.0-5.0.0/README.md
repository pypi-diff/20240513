# Comparing `tmp/ryutils-4.2.0.tar.gz` & `tmp/ryutils-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryutils-4.2.0.tar", last modified: Mon May 13 05:52:21 2024, max compression
+gzip compressed data, was "ryutils-5.0.0.tar", last modified: Sun May  5 18:21:39 2024, max compression
```

## Comparing `ryutils-4.2.0.tar` & `ryutils-5.0.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:52:21.562121 ryutils-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-13 05:52:16.000000 ryutils-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 05:52:16.000000 ryutils-4.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-13 05:52:21.562121 ryutils-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-13 05:52:16.000000 ryutils-4.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 05:52:16.000000 ryutils-4.2.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-13 05:52:16.000000 ryutils-4.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-13 05:52:16.000000 ryutils-4.2.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:52:21.562121 ryutils-4.2.0/ryutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 05:52:16.000000 ryutils-4.2.0/ryutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-13 05:52:16.000000 ryutils-4.2.0/ryutils/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-13 05:52:16.000000 ryutils-4.2.0/ryutils/csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-13 05:52:16.000000 ryutils-4.2.0/ryutils/dict_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-13 05:52:16.000000 ryutils-4.2.0/ryutils/email_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-13 05:52:16.000000 ryutils-4.2.0/ryutils/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-13 05:52:16.000000 ryutils-4.2.0/ryutils/fmt_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    12364 2024-05-13 05:52:16.000000 ryutils-4.2.0/ryutils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-13 05:52:16.000000 ryutils-4.2.0/ryutils/proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 05:52:16.000000 ryutils-4.2.0/ryutils/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-13 05:52:16.000000 ryutils-4.2.0/ryutils/short_url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:52:21.562121 ryutils-4.2.0/ryutils/sms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 05:52:16.000000 ryutils-4.2.0/ryutils/sms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-13 05:52:16.000000 ryutils-4.2.0/ryutils/sms/pytextbelt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-13 05:52:16.000000 ryutils-4.2.0/ryutils/sms/telegram_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-13 05:52:16.000000 ryutils-4.2.0/ryutils/sms/twilio_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-13 05:52:16.000000 ryutils-4.2.0/ryutils/wait.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-13 05:52:16.000000 ryutils-4.2.0/ryutils/web2_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:52:21.562121 ryutils-4.2.0/ryutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-13 05:52:21.000000 ryutils-4.2.0/ryutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-13 05:52:21.000000 ryutils-4.2.0/ryutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 05:52:21.000000 ryutils-4.2.0/ryutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 05:52:21.000000 ryutils-4.2.0/ryutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-13 05:52:21.000000 ryutils-4.2.0/ryutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 05:52:21.562121 ryutils-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-13 05:52:16.000000 ryutils-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:21:39.019526 ryutils-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-05 18:21:34.000000 ryutils-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-05 18:21:34.000000 ryutils-5.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-05 18:21:39.019526 ryutils-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-05 18:21:34.000000 ryutils-5.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-05 18:21:34.000000 ryutils-5.0.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-05 18:21:34.000000 ryutils-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-05 18:21:34.000000 ryutils-5.0.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:21:39.019526 ryutils-5.0.0/ryutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:21:34.000000 ryutils-5.0.0/ryutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-05 18:21:34.000000 ryutils-5.0.0/ryutils/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-05 18:21:34.000000 ryutils-5.0.0/ryutils/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-05 18:21:34.000000 ryutils-5.0.0/ryutils/dict_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-05 18:21:34.000000 ryutils-5.0.0/ryutils/email_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-05 18:21:34.000000 ryutils-5.0.0/ryutils/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-05 18:21:34.000000 ryutils-5.0.0/ryutils/fmt_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12364 2024-05-05 18:21:34.000000 ryutils-5.0.0/ryutils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-05 18:21:34.000000 ryutils-5.0.0/ryutils/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:21:34.000000 ryutils-5.0.0/ryutils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-05 18:21:34.000000 ryutils-5.0.0/ryutils/short_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:21:39.019526 ryutils-5.0.0/ryutils/sms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:21:34.000000 ryutils-5.0.0/ryutils/sms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-05 18:21:34.000000 ryutils-5.0.0/ryutils/sms/pytextbelt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-05 18:21:34.000000 ryutils-5.0.0/ryutils/sms/telegram_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-05 18:21:34.000000 ryutils-5.0.0/ryutils/sms/twilio_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-05 18:21:34.000000 ryutils-5.0.0/ryutils/wait.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-05 18:21:34.000000 ryutils-5.0.0/ryutils/web2_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:21:39.019526 ryutils-5.0.0/ryutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-05 18:21:39.000000 ryutils-5.0.0/ryutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-05 18:21:39.000000 ryutils-5.0.0/ryutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 18:21:39.000000 ryutils-5.0.0/ryutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-05 18:21:39.000000 ryutils-5.0.0/ryutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-05 18:21:39.000000 ryutils-5.0.0/ryutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 18:21:39.019526 ryutils-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-05 18:21:34.000000 ryutils-5.0.0/setup.py
```

### Comparing `ryutils-4.2.0/LICENSE` & `ryutils-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ryutils-4.2.0/PKG-INFO` & `ryutils-5.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryutils
-Version: 4.2.0
+Version: 5.0.0
 Summary: A collection of utilities for Python
 Author: Ross Yeager
 Author-email: ryeager12@email.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ryutils-4.2.0/pyproject.toml` & `ryutils-5.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ryutils-4.2.0/requirements.txt` & `ryutils-5.0.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `ryutils-4.2.0/ryutils/async_utils.py` & `ryutils-5.0.0/ryutils/async_utils.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.2.0/ryutils/csv_logger.py` & `ryutils-5.0.0/ryutils/csv_logger.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.2.0/ryutils/dict_util.py` & `ryutils-5.0.0/ryutils/dict_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.2.0/ryutils/email_util.py` & `ryutils-5.0.0/ryutils/email_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.2.0/ryutils/fmt_util.py` & `ryutils-5.0.0/ryutils/fmt_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.2.0/ryutils/log.py` & `ryutils-5.0.0/ryutils/log.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.2.0/ryutils/sms/pytextbelt.py` & `ryutils-5.0.0/ryutils/sms/pytextbelt.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.2.0/ryutils/sms/telegram_util.py` & `ryutils-5.0.0/ryutils/sms/telegram_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.2.0/ryutils/sms/twilio_util.py` & `ryutils-5.0.0/ryutils/sms/twilio_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.2.0/ryutils/web2_client.py` & `ryutils-5.0.0/ryutils/web2_client.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.2.0/ryutils.egg-info/PKG-INFO` & `ryutils-5.0.0/ryutils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryutils
-Version: 4.2.0
+Version: 5.0.0
 Summary: A collection of utilities for Python
 Author: Ross Yeager
 Author-email: ryeager12@email.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ryutils-4.2.0/ryutils.egg-info/SOURCES.txt` & `ryutils-5.0.0/ryutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ryutils-4.2.0/setup.py` & `ryutils-5.0.0/setup.py`

 * *Files identical despite different names*

