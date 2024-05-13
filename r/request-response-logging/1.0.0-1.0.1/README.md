# Comparing `tmp/request_response_logging-1.0.0.tar.gz` & `tmp/request_response_logging-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "request_response_logging-1.0.0.tar", last modified: Tue Apr 30 07:10:43 2024, max compression
+gzip compressed data, was "request_response_logging-1.0.1.tar", last modified: Mon May 13 03:10:05 2024, max compression
```

## Comparing `request_response_logging-1.0.0.tar` & `request_response_logging-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 praveentiwari  (1001) praveentiwari  (1001)        0 2024-04-30 07:10:43.499419 request_response_logging-1.0.0/
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)     5941 2024-04-30 07:10:43.499419 request_response_logging-1.0.0/PKG-INFO
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)     4558 2024-02-07 12:35:50.000000 request_response_logging-1.0.0/README.md
-drwxrwxr-x   0 praveentiwari  (1001) praveentiwari  (1001)        0 2024-04-30 07:10:43.487419 request_response_logging-1.0.0/request_logging/
-drwxrwxr-x   0 praveentiwari  (1001) praveentiwari  (1001)        0 2024-04-30 07:10:43.491419 request_response_logging-1.0.0/request_logging/Filters/
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)     1638 2024-01-21 16:59:31.000000 request_response_logging-1.0.0/request_logging/Filters/LoggingFilters.py
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)       59 2024-01-21 03:11:04.000000 request_response_logging-1.0.0/request_logging/Filters/__init__.py
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)      107 2024-01-21 11:20:31.000000 request_response_logging-1.0.0/request_logging/__init__.py
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)      522 2024-01-21 11:26:55.000000 request_response_logging-1.0.0/request_logging/decorators.py
-drwxrwxr-x   0 praveentiwari  (1001) praveentiwari  (1001)        0 2024-04-30 07:10:43.495419 request_response_logging-1.0.0/request_logging/middleware/
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)     6131 2024-04-30 07:05:46.000000 request_response_logging-1.0.0/request_logging/middleware/RequestResponseLogging.py
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)       53 2024-01-21 03:14:15.000000 request_response_logging-1.0.0/request_logging/middleware/__init__.py
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)      247 2024-02-02 17:51:13.000000 request_response_logging-1.0.0/request_logging/utils.py
-drwxrwxr-x   0 praveentiwari  (1001) praveentiwari  (1001)        0 2024-04-30 07:10:43.499419 request_response_logging-1.0.0/request_response_logging.egg-info/
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)     5941 2024-04-30 07:10:43.000000 request_response_logging-1.0.0/request_response_logging.egg-info/PKG-INFO
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)      510 2024-04-30 07:10:43.000000 request_response_logging-1.0.0/request_response_logging.egg-info/SOURCES.txt
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)        1 2024-04-30 07:10:43.000000 request_response_logging-1.0.0/request_response_logging.egg-info/dependency_links.txt
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)       11 2024-04-30 07:10:43.000000 request_response_logging-1.0.0/request_response_logging.egg-info/requires.txt
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)       16 2024-04-30 07:10:43.000000 request_response_logging-1.0.0/request_response_logging.egg-info/top_level.txt
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)       38 2024-04-30 07:10:43.499419 request_response_logging-1.0.0/setup.cfg
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)      590 2024-04-30 07:10:26.000000 request_response_logging-1.0.0/setup.py
+drwxrwxr-x   0 praveentiwari  (1001) praveentiwari  (1001)        0 2024-05-13 03:10:05.944378 request_response_logging-1.0.1/
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)     6149 2024-05-13 03:10:05.944378 request_response_logging-1.0.1/PKG-INFO
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)     4742 2024-05-13 03:09:08.000000 request_response_logging-1.0.1/README.md
+drwxrwxr-x   0 praveentiwari  (1001) praveentiwari  (1001)        0 2024-05-13 03:10:05.932378 request_response_logging-1.0.1/request_logging/
+drwxrwxr-x   0 praveentiwari  (1001) praveentiwari  (1001)        0 2024-05-13 03:10:05.936378 request_response_logging-1.0.1/request_logging/Filters/
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)     1638 2024-01-21 16:59:31.000000 request_response_logging-1.0.1/request_logging/Filters/LoggingFilters.py
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)       59 2024-01-21 03:11:04.000000 request_response_logging-1.0.1/request_logging/Filters/__init__.py
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)      107 2024-01-21 11:20:31.000000 request_response_logging-1.0.1/request_logging/__init__.py
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)      522 2024-01-21 11:26:55.000000 request_response_logging-1.0.1/request_logging/decorators.py
+drwxrwxr-x   0 praveentiwari  (1001) praveentiwari  (1001)        0 2024-05-13 03:10:05.940378 request_response_logging-1.0.1/request_logging/middleware/
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)     6536 2024-05-13 03:08:08.000000 request_response_logging-1.0.1/request_logging/middleware/RequestResponseLogging.py
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)       53 2024-01-21 03:14:15.000000 request_response_logging-1.0.1/request_logging/middleware/__init__.py
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)      247 2024-02-02 17:51:13.000000 request_response_logging-1.0.1/request_logging/utils.py
+drwxrwxr-x   0 praveentiwari  (1001) praveentiwari  (1001)        0 2024-05-13 03:10:05.944378 request_response_logging-1.0.1/request_response_logging.egg-info/
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)     6149 2024-05-13 03:10:05.000000 request_response_logging-1.0.1/request_response_logging.egg-info/PKG-INFO
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)      510 2024-05-13 03:10:05.000000 request_response_logging-1.0.1/request_response_logging.egg-info/SOURCES.txt
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)        1 2024-05-13 03:10:05.000000 request_response_logging-1.0.1/request_response_logging.egg-info/dependency_links.txt
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)       11 2024-05-13 03:10:05.000000 request_response_logging-1.0.1/request_response_logging.egg-info/requires.txt
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)       16 2024-05-13 03:10:05.000000 request_response_logging-1.0.1/request_response_logging.egg-info/top_level.txt
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)       38 2024-05-13 03:10:05.944378 request_response_logging-1.0.1/setup.cfg
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)      590 2024-05-13 03:09:25.000000 request_response_logging-1.0.1/setup.py
```

### Comparing `request_response_logging-1.0.0/PKG-INFO` & `request_response_logging-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: request_response_logging
-Version: 1.0.0
+Version: 1.0.1
 Summary: Django logger to log request response
 Home-page: UNKNOWN
 Author: Pravin Tiwari
 Author-email: pravint198@gmail.com
 License: UNKNOWN
 Description: # request-response-logging
         
@@ -42,17 +42,20 @@
         
         # health check api endpoint. this will return 200 status code with content OK
         REQUEST_RESPONSE_LOGGING_HEALTH_CHECK_API='/api/health'
         
         # default logger name is request_middleware_logger, in case of overwrite this attribute can be set
         REQUEST_RESPONSE_LOGGING_LOGGER_NAME='django'
         
-        # list of request.META fields to be logged. By default request.META REQUEST_METHOD, CONTENT_LENGTH, HTTP_X_FORWARDED_FOR or REMOTE_ADDR, REMOTE_HOST, SERVER_NAME, SERVER_PORT is being logged.
+        # list of request.META fields to be logged. By default request.META REQUEST_METHOD, CONTENT_LENGTH, HTTP_X_FORWARDED_FOR or REMOTE_ADDR, REMOTE_HOST, SERVER_NAME, SERVER_PORT is being logged in request.
         REQUEST_RESPONSE_LOGGING_META_OPTIONS = ['HTTP_HEADER_FIELD1', 'HTTP_HEADER_FIELD2']
         
+        # set this to true if you want to log REQUEST_RESPONSE_LOGGING_META_OPTIONS in response as well. Defaults to False
+        REQUEST_RESPONSE_LOGGING_META_OPTIONS_IN_RESPONSE = True
+        
         ```
         
         **Sample logger in settings file. request_id filter is to add request_id and masking filter is used to mask fields in request and response**
         ```python
         LOGGING = {
             'version': 1,
             'disable_existing_loggers': False,
```

### Comparing `request_response_logging-1.0.0/README.md` & `request_response_logging-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -34,17 +34,20 @@
 
 # health check api endpoint. this will return 200 status code with content OK
 REQUEST_RESPONSE_LOGGING_HEALTH_CHECK_API='/api/health'
 
 # default logger name is request_middleware_logger, in case of overwrite this attribute can be set
 REQUEST_RESPONSE_LOGGING_LOGGER_NAME='django'
 
-# list of request.META fields to be logged. By default request.META REQUEST_METHOD, CONTENT_LENGTH, HTTP_X_FORWARDED_FOR or REMOTE_ADDR, REMOTE_HOST, SERVER_NAME, SERVER_PORT is being logged.
+# list of request.META fields to be logged. By default request.META REQUEST_METHOD, CONTENT_LENGTH, HTTP_X_FORWARDED_FOR or REMOTE_ADDR, REMOTE_HOST, SERVER_NAME, SERVER_PORT is being logged in request.
 REQUEST_RESPONSE_LOGGING_META_OPTIONS = ['HTTP_HEADER_FIELD1', 'HTTP_HEADER_FIELD2']
 
+# set this to true if you want to log REQUEST_RESPONSE_LOGGING_META_OPTIONS in response as well. Defaults to False
+REQUEST_RESPONSE_LOGGING_META_OPTIONS_IN_RESPONSE = True
+
 ```
 
 **Sample logger in settings file. request_id filter is to add request_id and masking filter is used to mask fields in request and response**
 ```python
 LOGGING = {
     'version': 1,
     'disable_existing_loggers': False,
```

### Comparing `request_response_logging-1.0.0/request_logging/Filters/LoggingFilters.py` & `request_response_logging-1.0.1/request_logging/Filters/LoggingFilters.py`

 * *Files identical despite different names*

### Comparing `request_response_logging-1.0.0/request_logging/decorators.py` & `request_response_logging-1.0.1/request_logging/decorators.py`

 * *Files identical despite different names*

### Comparing `request_response_logging-1.0.0/request_logging/middleware/RequestResponseLogging.py` & `request_response_logging-1.0.1/request_logging/middleware/RequestResponseLogging.py`

 * *Files 21% similar despite different names*

```diff
@@ -21,14 +21,16 @@
                               list())
 RESPONSE_KEYS_TO_POP = [field for field in getattr(
         settings, 'REQUEST_RESPONSE_LOGGING_POP_RESPONSE_KEYS', list())]
 HEALTH_CHECK_API = getattr(settings,
                            'REQUEST_RESPONSE_LOGGING_HEALTH_CHECK_API', None)
 LOG_META_OPTIONS = getattr(settings,
                            'REQUEST_RESPONSE_LOGGING_META_OPTIONS', None)
+LOG_META_OPTIONS_IN_RESPONSE = getattr(settings,
+                           'REQUEST_RESPONSE_LOGGING_META_OPTIONS_IN_RESPONSE', False)
 
 ctx_request_id = ContextVar('request_id')
 
 
 class LoggingMiddleware:
     def __init__(self, get_response):
         self.get_response = get_response
@@ -161,8 +163,14 @@
             "descr": "RESPONSE",
             "request_response_contents": response_content,
             "response_code": response.status_code,
             "X-total-time": duration,
             "response_for_request": request.path
         }
 
+        if LOG_META_OPTIONS_IN_RESPONSE and LOG_META_OPTIONS and \
+                isinstance(LOG_META_OPTIONS, list):
+            for key in LOG_META_OPTIONS:
+                if request.META.get(key):
+                    log_response.update({key: request.META[key]})
+
         logger.info(json.dumps(log_response))
```

### Comparing `request_response_logging-1.0.0/request_response_logging.egg-info/PKG-INFO` & `request_response_logging-1.0.1/request_response_logging.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: request-response-logging
-Version: 1.0.0
+Version: 1.0.1
 Summary: Django logger to log request response
 Home-page: UNKNOWN
 Author: Pravin Tiwari
 Author-email: pravint198@gmail.com
 License: UNKNOWN
 Description: # request-response-logging
         
@@ -42,17 +42,20 @@
         
         # health check api endpoint. this will return 200 status code with content OK
         REQUEST_RESPONSE_LOGGING_HEALTH_CHECK_API='/api/health'
         
         # default logger name is request_middleware_logger, in case of overwrite this attribute can be set
         REQUEST_RESPONSE_LOGGING_LOGGER_NAME='django'
         
-        # list of request.META fields to be logged. By default request.META REQUEST_METHOD, CONTENT_LENGTH, HTTP_X_FORWARDED_FOR or REMOTE_ADDR, REMOTE_HOST, SERVER_NAME, SERVER_PORT is being logged.
+        # list of request.META fields to be logged. By default request.META REQUEST_METHOD, CONTENT_LENGTH, HTTP_X_FORWARDED_FOR or REMOTE_ADDR, REMOTE_HOST, SERVER_NAME, SERVER_PORT is being logged in request.
         REQUEST_RESPONSE_LOGGING_META_OPTIONS = ['HTTP_HEADER_FIELD1', 'HTTP_HEADER_FIELD2']
         
+        # set this to true if you want to log REQUEST_RESPONSE_LOGGING_META_OPTIONS in response as well. Defaults to False
+        REQUEST_RESPONSE_LOGGING_META_OPTIONS_IN_RESPONSE = True
+        
         ```
         
         **Sample logger in settings file. request_id filter is to add request_id and masking filter is used to mask fields in request and response**
         ```python
         LOGGING = {
             'version': 1,
             'disable_existing_loggers': False,
```

### Comparing `request_response_logging-1.0.0/setup.py` & `request_response_logging-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name='request_response_logging',
-    version='1.0.0',
+    version='1.0.1',
     author='Pravin Tiwari',
     author_email='pravint198@gmail.com',
     description='Django logger to log request response',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=['simplejson'],
```

