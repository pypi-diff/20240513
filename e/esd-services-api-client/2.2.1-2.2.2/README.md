# Comparing `tmp/esd_services_api_client-2.2.1.tar.gz` & `tmp/esd_services_api_client-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esd_services_api_client-2.2.1.tar", max compression
+gzip compressed data, was "esd_services_api_client-2.2.2.tar", max compression
```

## Comparing `esd_services_api_client-2.2.1.tar` & `esd_services_api_client-2.2.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    10693 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/LICENSE
--rw-r--r--   0        0        0      111 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/README.md
--rw-r--r--   0        0        0      603 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/__init__.py
--rw-r--r--   0        0        0       22 2024-04-12 11:44:04.246022 esd_services_api_client-2.2.1/esd_services_api_client/_version.py
--rw-r--r--   0        0        0      723 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/beast/__init__.py
--rw-r--r--   0        0        0      754 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/beast/v3/__init__.py
--rw-r--r--   0        0        0    11478 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/beast/v3/_connector.py
--rw-r--r--   0        0        0     6766 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/beast/v3/_models.py
--rw-r--r--   0        0        0     3618 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/boxer/README.md
--rw-r--r--   0        0        0      785 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/boxer/__init__.py
--rw-r--r--   0        0        0     7445 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/boxer/_auth.py
--rw-r--r--   0        0        0      981 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/boxer/_base.py
--rw-r--r--   0        0        0     8677 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/boxer/_connector.py
--rw-r--r--   0        0        0     1702 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/boxer/_models.py
--rw-r--r--   0        0        0      603 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/common/__init__.py
--rw-r--r--   0        0        0      792 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/crystal/__init__.py
--rw-r--r--   0        0        0      837 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/crystal/_api_versions.py
--rw-r--r--   0        0        0    12875 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/crystal/_connector.py
--rw-r--r--   0        0        0     4030 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/crystal/_models.py
--rw-r--r--   0        0        0     9393 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/README.md
--rw-r--r--   0        0        0      627 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/__init__.py
--rw-r--r--   0        0        0      627 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/abstractions/__init__.py
--rw-r--r--   0        0        0     3338 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/abstractions/algrorithm_cache.py
--rw-r--r--   0        0        0     1761 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/abstractions/input_object.py
--rw-r--r--   0        0        0     2019 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/abstractions/logger_factory.py
--rw-r--r--   0        0        0     3039 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/abstractions/nexus_object.py
--rw-r--r--   0        0        0     1729 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/abstractions/socket_provider.py
--rw-r--r--   0        0        0      903 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/__init__.py
--rw-r--r--   0        0        0     2925 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/_baseline_algorithm.py
--rw-r--r--   0        0        0     3900 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/_remote_algorithm.py
--rw-r--r--   0        0        0     1702 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/distributed.py
--rw-r--r--   0        0        0     4310 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/forked_algorithm.py
--rw-r--r--   0        0        0     1644 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/minimalistic.py
--rw-r--r--   0        0        0     2007 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/recursive.py
--rw-r--r--   0        0        0        0 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/configurations/__init__.py
--rw-r--r--   0        0        0     1091 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/configurations/algorithm_configuration.py
--rw-r--r--   0        0        0      627 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/core/__init__.py
--rw-r--r--   0        0        0    10037 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/core/app_core.py
--rw-r--r--   0        0        0     6674 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/core/app_dependencies.py
--rw-r--r--   0        0        0      696 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/exceptions/__init__.py
--rw-r--r--   0        0        0      895 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/exceptions/_nexus_error.py
--rw-r--r--   0        0        0     1622 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/exceptions/cache_errors.py
--rw-r--r--   0        0        0     1765 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/exceptions/input_reader_error.py
--rw-r--r--   0        0        0     1991 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/exceptions/startup_error.py
--rw-r--r--   0        0        0      758 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/input/__init__.py
--rw-r--r--   0        0        0     3132 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/input/input_processor.py
--rw-r--r--   0        0        0     3505 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/input/input_reader.py
--rw-r--r--   0        0        0     2516 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/input/payload_reader.py
--rw-r--r--   0        0        0        0 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/telemetry/__init__.py
--rw-r--r--   0        0        0     3220 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/telemetry/recorder.py
--rw-r--r--   0        0        0     1237 2024-04-12 11:44:04.246022 esd_services_api_client-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     1292 1970-01-01 00:00:00.000000 esd_services_api_client-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0    10693 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/LICENSE
+-rw-r--r--   0        0        0      111 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/README.md
+-rw-r--r--   0        0        0      603 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-13 09:38:59.167327 esd_services_api_client-2.2.2/esd_services_api_client/_version.py
+-rw-r--r--   0        0        0      723 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/beast/__init__.py
+-rw-r--r--   0        0        0      754 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/beast/v3/__init__.py
+-rw-r--r--   0        0        0    11478 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/beast/v3/_connector.py
+-rw-r--r--   0        0        0     6766 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/beast/v3/_models.py
+-rw-r--r--   0        0        0     3618 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/boxer/README.md
+-rw-r--r--   0        0        0      785 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/boxer/__init__.py
+-rw-r--r--   0        0        0     7445 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/boxer/_auth.py
+-rw-r--r--   0        0        0      981 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/boxer/_base.py
+-rw-r--r--   0        0        0     8677 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/boxer/_connector.py
+-rw-r--r--   0        0        0     1702 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/boxer/_models.py
+-rw-r--r--   0        0        0      603 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/common/__init__.py
+-rw-r--r--   0        0        0      792 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/crystal/__init__.py
+-rw-r--r--   0        0        0      837 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/crystal/_api_versions.py
+-rw-r--r--   0        0        0    13053 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/crystal/_connector.py
+-rw-r--r--   0        0        0     4338 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/crystal/_models.py
+-rw-r--r--   0        0        0     9393 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/README.md
+-rw-r--r--   0        0        0      627 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/__init__.py
+-rw-r--r--   0        0        0      627 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/abstractions/__init__.py
+-rw-r--r--   0        0        0     3338 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/abstractions/algrorithm_cache.py
+-rw-r--r--   0        0        0     1761 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/abstractions/input_object.py
+-rw-r--r--   0        0        0     2019 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/abstractions/logger_factory.py
+-rw-r--r--   0        0        0     3039 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/abstractions/nexus_object.py
+-rw-r--r--   0        0        0     1729 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/abstractions/socket_provider.py
+-rw-r--r--   0        0        0      903 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/algorithms/__init__.py
+-rw-r--r--   0        0        0     2925 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/algorithms/_baseline_algorithm.py
+-rw-r--r--   0        0        0     3900 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/algorithms/_remote_algorithm.py
+-rw-r--r--   0        0        0     1702 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/algorithms/distributed.py
+-rw-r--r--   0        0        0     4310 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/algorithms/forked_algorithm.py
+-rw-r--r--   0        0        0     1644 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/algorithms/minimalistic.py
+-rw-r--r--   0        0        0     2007 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/algorithms/recursive.py
+-rw-r--r--   0        0        0        0 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/configurations/__init__.py
+-rw-r--r--   0        0        0     1091 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/configurations/algorithm_configuration.py
+-rw-r--r--   0        0        0      627 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/core/__init__.py
+-rw-r--r--   0        0        0    10037 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/core/app_core.py
+-rw-r--r--   0        0        0     6674 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/core/app_dependencies.py
+-rw-r--r--   0        0        0      696 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/exceptions/__init__.py
+-rw-r--r--   0        0        0      895 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/exceptions/_nexus_error.py
+-rw-r--r--   0        0        0     1622 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/exceptions/cache_errors.py
+-rw-r--r--   0        0        0     1765 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/exceptions/input_reader_error.py
+-rw-r--r--   0        0        0     1991 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/exceptions/startup_error.py
+-rw-r--r--   0        0        0      758 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/input/__init__.py
+-rw-r--r--   0        0        0     3132 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/input/input_processor.py
+-rw-r--r--   0        0        0     3505 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/input/input_reader.py
+-rw-r--r--   0        0        0     2516 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/input/payload_reader.py
+-rw-r--r--   0        0        0        0 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/telemetry/__init__.py
+-rw-r--r--   0        0        0     3644 2024-05-13 09:38:48.679232 esd_services_api_client-2.2.2/esd_services_api_client/nexus/telemetry/recorder.py
+-rw-r--r--   0        0        0     1237 2024-05-13 09:38:59.167327 esd_services_api_client-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1292 1970-01-01 00:00:00.000000 esd_services_api_client-2.2.2/PKG-INFO
```

### Comparing `esd_services_api_client-2.2.1/LICENSE` & `esd_services_api_client-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/__init__.py` & `esd_services_api_client-2.2.2/esd_services_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/beast/__init__.py` & `esd_services_api_client-2.2.2/esd_services_api_client/beast/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/beast/v3/__init__.py` & `esd_services_api_client-2.2.2/esd_services_api_client/beast/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/beast/v3/_connector.py` & `esd_services_api_client-2.2.2/esd_services_api_client/beast/v3/_connector.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/beast/v3/_models.py` & `esd_services_api_client-2.2.2/esd_services_api_client/beast/v3/_models.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/boxer/README.md` & `esd_services_api_client-2.2.2/esd_services_api_client/boxer/README.md`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/boxer/__init__.py` & `esd_services_api_client-2.2.2/esd_services_api_client/boxer/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/boxer/_auth.py` & `esd_services_api_client-2.2.2/esd_services_api_client/boxer/_auth.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/boxer/_base.py` & `esd_services_api_client-2.2.2/esd_services_api_client/boxer/_base.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/boxer/_connector.py` & `esd_services_api_client-2.2.2/esd_services_api_client/boxer/_connector.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/boxer/_models.py` & `esd_services_api_client-2.2.2/esd_services_api_client/boxer/_models.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/common/__init__.py` & `esd_services_api_client-2.2.2/esd_services_api_client/common/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/crystal/__init__.py` & `esd_services_api_client-2.2.2/esd_services_api_client/crystal/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/crystal/_api_versions.py` & `esd_services_api_client-2.2.2/esd_services_api_client/crystal/_api_versions.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/crystal/_connector.py` & `esd_services_api_client-2.2.2/esd_services_api_client/crystal/_connector.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from esd_services_api_client.crystal._models import (
     RequestResult,
     AlgorithmRunResult,
     CrystalEntrypointArguments,
     AlgorithmRequest,
     AlgorithmConfiguration,
     RequestLifeCycleStage,
+    ParentRequest,
 )
 
 T = TypeVar("T")  # pylint: disable=C0103
 
 
 def add_crystal_args(parser: Optional[ArgumentParser] = None) -> ArgumentParser:
     """
@@ -150,36 +151,39 @@
         self.dispose()
 
     def create_run(
         self,
         algorithm: str,
         payload: Dict,
         custom_config: Optional[AlgorithmConfiguration] = None,
+        parent_request: Optional[ParentRequest] = None,
         tag: Optional[str] = None,
     ) -> str:
         """
           Creates a Crystal job run against the latest API version.
 
         :param algorithm: Name of a connected algorithm.
         :param payload: Algorithm payload.
         :param custom_config: Customized config for this run.
+        :param parent_request: Parent request for this run.
         :param tag: Client-side submission identifier.
         :return: Request identifier assigned to the job by Crystal.
         """
 
         def get_api_path() -> str:
             if self._api_version == ApiVersion.V1_2:
                 return f"{self._scheduler_base_url}/algorithm/{self._api_version.value}/run/{algorithm}"
 
             raise ValueError(f"Unsupported API version {self._api_version}")
 
         run_body = AlgorithmRequest(
             algorithm_name=algorithm,
             algorithm_parameters=payload,
             custom_configuration=custom_config,
+            parent_request=parent_request,
             tag=tag,
         ).to_dict()
 
         run_response = self._http.post(get_api_path(), json=run_body)
 
         # raise if not successful
         run_response.raise_for_status()
```

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/crystal/_models.py` & `esd_services_api_client-2.2.2/esd_services_api_client/crystal/_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -131,16 +131,28 @@
     monitoring_parameters: Optional[List[str]] = None
     custom_resources: Optional[Dict[str, str]] = None
     speculative_attempts: Optional[int] = None
 
 
 @dataclass_json(letter_case=LetterCase.CAMEL)
 @dataclass
+class ParentRequest(DataClassJsonMixin):
+    """
+    Used to specify crystal parent job for a new crystal job.
+    """
+
+    request_id: Optional[str] = None
+    algorithm_name: Optional[str] = None
+
+
+@dataclass_json(letter_case=LetterCase.CAMEL)
+@dataclass
 class AlgorithmRequest(DataClassJsonMixin):
     """
     Crystal algorthm request.
     """
 
     algorithm_parameters: Dict
     algorithm_name: Optional[str] = None
     custom_configuration: Optional[AlgorithmConfiguration] = None
+    parent_request: Optional[ParentRequest] = None
     tag: Optional[str] = None
```

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/README.md` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/README.md`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/__init__.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/abstractions/__init__.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/abstractions/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/abstractions/algrorithm_cache.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/abstractions/algrorithm_cache.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/abstractions/input_object.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/abstractions/input_object.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/abstractions/logger_factory.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/abstractions/logger_factory.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/abstractions/nexus_object.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/abstractions/nexus_object.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/abstractions/socket_provider.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/abstractions/socket_provider.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/__init__.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/_baseline_algorithm.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/algorithms/_baseline_algorithm.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/_remote_algorithm.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/algorithms/_remote_algorithm.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/distributed.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/algorithms/distributed.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/forked_algorithm.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/algorithms/forked_algorithm.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/minimalistic.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/algorithms/minimalistic.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/recursive.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/algorithms/recursive.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/configurations/algorithm_configuration.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/configurations/algorithm_configuration.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/core/__init__.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/core/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/core/app_core.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/core/app_core.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/core/app_dependencies.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/core/app_dependencies.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/exceptions/__init__.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/exceptions/_nexus_error.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/exceptions/_nexus_error.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/exceptions/cache_errors.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/exceptions/cache_errors.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/exceptions/input_reader_error.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/exceptions/input_reader_error.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/exceptions/startup_error.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/exceptions/startup_error.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/input/__init__.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/input/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/input/input_processor.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/input/input_processor.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/input/input_reader.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/input/input_reader.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/input/payload_reader.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/input/payload_reader.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.1/esd_services_api_client/nexus/telemetry/recorder.py` & `esd_services_api_client-2.2.2/esd_services_api_client/nexus/telemetry/recorder.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,26 +55,34 @@
             **_,
         ) -> None:
             self._logger.debug(
                 "Recording telemetry for {entity_name} in the run {run_id}",
                 entity_name=entity_name,
                 run_id=run_id,
             )
-            self._storage_client.save_data_as_blob(
-                data=entity_to_record,
-                blob_path=DataSocket(
-                    alias="telemetry",
-                    data_path=f"{self._telemetry_base_path}/{entity_name}/{run_id}",
-                    data_format="null",
-                ).parse_data_path(),
-                serialization_format=DictJsonSerializationFormat
-                if isinstance(entity_to_record, dict)
-                else DataFrameParquetSerializationFormat,
-                overwrite=True,
-            )
+            if not isinstance(entity_to_record, dict) and not isinstance(
+                entity_to_record, pd.DataFrame
+            ):
+                self._logger.warning(
+                    "Unsupported data type: {telemetry_entity_type}. Telemetry recording skipped.",
+                    telemetry_entity_type=type(entity_to_record),
+                )
+            else:
+                self._storage_client.save_data_as_blob(
+                    data=entity_to_record,
+                    blob_path=DataSocket(
+                        alias="telemetry",
+                        data_path=f"{self._telemetry_base_path}/{entity_name}/{run_id}",
+                        data_format="null",
+                    ).parse_data_path(),
+                    serialization_format=DictJsonSerializationFormat
+                    if isinstance(entity_to_record, dict)
+                    else DataFrameParquetSerializationFormat,
+                    overwrite=True,
+                )
 
         telemetry_tasks = [
             asyncio.create_task(
                 partial(
                     _record,
                     entity_to_record=telemetry_value,
                     entity_name=telemetry_key,
```

### Comparing `esd_services_api_client-2.2.1/pyproject.toml` & `esd_services_api_client-2.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "esd-services-api-client"
-version = "2.2.1"
+version = "2.2.2"
 description = "Python clients for ESD services"
 authors = ["ECCO Sneaks & Data <esdsupport@ecco.com>"]
 maintainers = ['GZU <gzu@ecco.com>', 'JRB <ext-jrb@ecco.com>', 'VISA <visa@ecco.com>']
 readme = "README.md"
 license = 'Apache 2.0'
 repository = 'https://github.com/SneaksAndData/esd-services-api-client'
```

### Comparing `esd_services_api_client-2.2.1/PKG-INFO` & `esd_services_api_client-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esd-services-api-client
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python clients for ESD services
 Home-page: https://github.com/SneaksAndData/esd-services-api-client
 License: Apache 2.0
 Author: ECCO Sneaks & Data
 Author-email: esdsupport@ecco.com
 Maintainer: GZU
 Maintainer-email: gzu@ecco.com
```

