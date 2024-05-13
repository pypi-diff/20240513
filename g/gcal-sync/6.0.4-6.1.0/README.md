# Comparing `tmp/gcal-sync-6.0.4.tar.gz` & `tmp/gcal_sync-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcal-sync-6.0.4.tar", last modified: Sat Mar 23 21:47:39 2024, max compression
+gzip compressed data, was "gcal_sync-6.1.0.tar", last modified: Mon May 13 00:36:56 2024, max compression
```

## Comparing `gcal-sync-6.0.4.tar` & `gcal_sync-6.1.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:47:39.384557 gcal-sync-6.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-23 21:47:35.000000 gcal-sync-6.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-03-23 21:47:39.384557 gcal-sync-6.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-03-23 21:47:35.000000 gcal-sync-6.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:47:39.384557 gcal-sync-6.0.4/gcal_sync/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-23 21:47:35.000000 gcal-sync-6.0.4/gcal_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23048 2024-03-23 21:47:35.000000 gcal-sync-6.0.4/gcal_sync/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-03-23 21:47:35.000000 gcal-sync-6.0.4/gcal_sync/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-23 21:47:35.000000 gcal-sync-6.0.4/gcal_sync/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-23 21:47:35.000000 gcal-sync-6.0.4/gcal_sync/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    27067 2024-03-23 21:47:35.000000 gcal-sync-6.0.4/gcal_sync/model.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 21:47:35.000000 gcal-sync-6.0.4/gcal_sync/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-03-23 21:47:35.000000 gcal-sync-6.0.4/gcal_sync/store.py
--rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-03-23 21:47:35.000000 gcal-sync-6.0.4/gcal_sync/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-03-23 21:47:35.000000 gcal-sync-6.0.4/gcal_sync/timeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:47:39.384557 gcal-sync-6.0.4/gcal_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-03-23 21:47:39.000000 gcal-sync-6.0.4/gcal_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-23 21:47:39.000000 gcal-sync-6.0.4/gcal_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 21:47:39.000000 gcal-sync-6.0.4/gcal_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-23 21:47:39.000000 gcal-sync-6.0.4/gcal_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-23 21:47:39.000000 gcal-sync-6.0.4/gcal_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-23 21:47:39.388558 gcal-sync-6.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-23 21:47:35.000000 gcal-sync-6.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:47:39.384557 gcal-sync-6.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    28453 2024-03-23 21:47:35.000000 gcal-sync-6.0.4/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-03-23 21:47:35.000000 gcal-sync-6.0.4/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    26710 2024-03-23 21:47:35.000000 gcal-sync-6.0.4/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-03-23 21:47:35.000000 gcal-sync-6.0.4/tests/test_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    29841 2024-03-23 21:47:35.000000 gcal-sync-6.0.4/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    36085 2024-03-23 21:47:35.000000 gcal-sync-6.0.4/tests/test_timeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:36:56.654286 gcal_sync-6.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 00:36:52.000000 gcal_sync-6.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-13 00:36:56.654286 gcal_sync-6.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-13 00:36:52.000000 gcal_sync-6.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:36:56.650286 gcal_sync-6.1.0/gcal_sync/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-13 00:36:52.000000 gcal_sync-6.1.0/gcal_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23066 2024-05-13 00:36:52.000000 gcal_sync-6.1.0/gcal_sync/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-05-13 00:36:52.000000 gcal_sync-6.1.0/gcal_sync/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-13 00:36:52.000000 gcal_sync-6.1.0/gcal_sync/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-13 00:36:52.000000 gcal_sync-6.1.0/gcal_sync/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27067 2024-05-13 00:36:52.000000 gcal_sync-6.1.0/gcal_sync/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 00:36:52.000000 gcal_sync-6.1.0/gcal_sync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-13 00:36:52.000000 gcal_sync-6.1.0/gcal_sync/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-05-13 00:36:52.000000 gcal_sync-6.1.0/gcal_sync/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-13 00:36:52.000000 gcal_sync-6.1.0/gcal_sync/timeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:36:56.654286 gcal_sync-6.1.0/gcal_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-13 00:36:56.000000 gcal_sync-6.1.0/gcal_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-13 00:36:56.000000 gcal_sync-6.1.0/gcal_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 00:36:56.000000 gcal_sync-6.1.0/gcal_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-13 00:36:56.000000 gcal_sync-6.1.0/gcal_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-13 00:36:56.000000 gcal_sync-6.1.0/gcal_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-13 00:36:52.000000 gcal_sync-6.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-13 00:36:56.654286 gcal_sync-6.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-13 00:36:52.000000 gcal_sync-6.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:36:56.654286 gcal_sync-6.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    28453 2024-05-13 00:36:52.000000 gcal_sync-6.1.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-05-13 00:36:52.000000 gcal_sync-6.1.0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26710 2024-05-13 00:36:52.000000 gcal_sync-6.1.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-13 00:36:52.000000 gcal_sync-6.1.0/tests/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29841 2024-05-13 00:36:52.000000 gcal_sync-6.1.0/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36085 2024-05-13 00:36:52.000000 gcal_sync-6.1.0/tests/test_timeline.py
```

### Comparing `gcal-sync-6.0.4/LICENSE` & `gcal_sync-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gcal-sync-6.0.4/PKG-INFO` & `gcal_sync-6.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 Metadata-Version: 2.1
-Name: gcal-sync
-Version: 6.0.4
+Name: gcal_sync
+Version: 6.1.0
 Summary: A python library for syncing Google Calendar to local storage
 Home-page: https://github.com/allenporter/gcal_sync
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.8.1
-Requires-Dist: pydantic>=1.9.0
 Requires-Dist: ical>=6.1.0
+Requires-Dist: pydantic>=1.9.0
 
 An asyncio python library for the [Google Calendar API](https://developers.google.com/calendar/api). This library provides a simplified
 Google Calendar API that is lighter weight and more streamlined compared to using
 aiogoogle, and increased reliability by supporting efficient sync and reading
 from local storage. See the [API Documentation](https://allenporter.github.io/gcal_sync/).
 
 The focus of this API is on making it simple to access the most relevant parts of Google
 Calendar, for doing useful things. It may not support everything in the API however it
 should be easy to extend to do more as needed.
 
 # Quickstart
 
 In order to use the library, you'll need to do some work yourself to get authentication
-credentails. This depends a lot on the context (e.g. redirecting to use OAuth via web)
+credentials. This depends a lot on the context (e.g. redirecting to use OAuth via web)
 but should be easy to incorporate using Google's python authentication libraries. See
 Google's [Authentication and authorization overview](https://developers.google.com/workspace/guides/auth-overview) for details.
 
 You will implement `gcal_sync.AbstractAuth` to provide an access token. Your implementation
-will handle any necessary refreshes. You can invoke the service with your auth implentation
+will handle any necessary refreshes. You can invoke the service with your auth implementation
 to access the API.
 
 ```python
 from gcal_sync.auth import AbstractAuth
 
 
 class MyAuthImpl(gcal_sync.AbstractAuth):
```

### Comparing `gcal-sync-6.0.4/README.md` & `gcal_sync-6.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 The focus of this API is on making it simple to access the most relevant parts of Google
 Calendar, for doing useful things. It may not support everything in the API however it
 should be easy to extend to do more as needed.
 
 # Quickstart
 
 In order to use the library, you'll need to do some work yourself to get authentication
-credentails. This depends a lot on the context (e.g. redirecting to use OAuth via web)
+credentials. This depends a lot on the context (e.g. redirecting to use OAuth via web)
 but should be easy to incorporate using Google's python authentication libraries. See
 Google's [Authentication and authorization overview](https://developers.google.com/workspace/guides/auth-overview) for details.
 
 You will implement `gcal_sync.AbstractAuth` to provide an access token. Your implementation
-will handle any necessary refreshes. You can invoke the service with your auth implentation
+will handle any necessary refreshes. You can invoke the service with your auth implementation
 to access the API.
 
 ```python
 from gcal_sync.auth import AbstractAuth
 
 
 class MyAuthImpl(gcal_sync.AbstractAuth):
```

### Comparing `gcal-sync-6.0.4/gcal_sync/api.py` & `gcal_sync-6.1.0/gcal_sync/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 This library also contains apis for local storage of calendars an events in
 `CalendarListStoreService` and `CalendarEventStoreService`.  See the `sync`
 library for more details on how to
 async down calendars and events to local storage.
 
 All of the request and response messages here use [pydantic](https://pydantic-docs.helpmanual.io/)
-for parsing and valdation of the constraints of the API. The API fields in the
+for parsing and validation of the constraints of the API. The API fields in the
 request and response methods are mirroring the Google Calendar API methods, so
 see the [reference](https://developers.google.com/calendar/api/v3/reference)
 for details.
 """
 
 from __future__ import annotations
 
@@ -276,16 +276,17 @@
 
 class ListEventsResponse:
     """Api response containing a list of events."""
 
     def __init__(
         self,
         model: _ListEventsResponseModel,
-        get_next_page: Callable[[str | None], Awaitable[_ListEventsResponseModel]]
-        | None = None,
+        get_next_page: (
+            Callable[[str | None], Awaitable[_ListEventsResponseModel]] | None
+        ) = None,
     ) -> None:
         """initialize ListEventsResponse."""
         self._model = model
         self._get_next_page = get_next_page
 
     @property
     def items(self) -> list[Event]:
@@ -569,15 +570,15 @@
         event must be specified without a `event_id`.
 
         To delete individual instances or a range of instances of a recurring event
         both the `ical_uuid` and `event_id` can be specified. The `recurrence_range`
         determines if its just the individual event (`Range.NONE`) or also including
         events going forward (`Range.THIS_AND_FUTURE`)
 
-        The local store may be used in some scenarios to deterine the appropriate
+        The local store may be used in some scenarios to determine the appropriate
         commands to send to the calendar API, so it may be operating on stale data.
         You should sync the event store after performing a delete operation to
         ensure the store reflects the latest information from the server
         """
         event = await self._lookup_ical_uuid(ical_uuid)
         if not event or not event.id:
             raise ValueError(f"Event does not exist: {ical_uuid} or malformed")
```

### Comparing `gcal-sync-6.0.4/gcal_sync/auth.py` & `gcal_sync-6.1.0/gcal_sync/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 In order to use `gcal_sync.api`, you need to implement `gcal_sync.AbstractAuth`
 which provides an OAuth access token. See Google's
 [Authentication and authorization overview][1] for general details on how to
 use OAuth, which involves things like redirecting a user to a web flow, and
 redirecting back with an access token.
 
 An example implementation of `gcal_sync.AbstractAuth` would need to handle things like
-passin in the access token and any other necessary OAuth token refreshes when the
+passing in the access token and any other necessary OAuth token refreshes when the
 access token has expired.
 
 ```python
 from gcal_sync.auth import AbstractAuth
 
 class MyAuthImpl(gcal_sync.AbstractAuth):
 
@@ -151,15 +151,15 @@
             raise ApiException(": ".join(detail)) from err
         except ClientError as err:
             raise ApiException(f"Error from API: {err}") from err
         return resp
 
     @staticmethod
     async def _error_detail(resp: aiohttp.ClientResponse) -> List[str]:
-        """Resturns an error message string from the APi response."""
+        """Returns an error message string from the APi response."""
         if resp.status < 400:
             return []
         try:
             result = await resp.json()
             error = result.get(ERROR, {})
         except ClientError:
             return []
```

### Comparing `gcal-sync-6.0.4/gcal_sync/exceptions.py` & `gcal_sync-6.1.0/gcal_sync/exceptions.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-6.0.4/gcal_sync/model.py` & `gcal_sync-6.1.0/gcal_sync/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Library for data model for local calendar objects.
 
-This librayr contains [pydantic](https://pydantic-docs.helpmanual.io/) models
+This library contains [pydantic](https://pydantic-docs.helpmanual.io/) models
 for the Google Calendar API data model. These objects support all methods for
 parsing and serialization supported by pydnatic.
 """
 
 from __future__ import annotations
 
 import datetime
```

### Comparing `gcal-sync-6.0.4/gcal_sync/store.py` & `gcal_sync-6.1.0/gcal_sync/store.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-6.0.4/gcal_sync/sync.py` & `gcal_sync-6.1.0/gcal_sync/sync.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-6.0.4/gcal_sync/timeline.py` & `gcal_sync-6.1.0/gcal_sync/timeline.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-6.0.4/gcal_sync.egg-info/PKG-INFO` & `gcal_sync-6.1.0/gcal_sync.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 Metadata-Version: 2.1
-Name: gcal-sync
-Version: 6.0.4
+Name: gcal_sync
+Version: 6.1.0
 Summary: A python library for syncing Google Calendar to local storage
 Home-page: https://github.com/allenporter/gcal_sync
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.8.1
-Requires-Dist: pydantic>=1.9.0
 Requires-Dist: ical>=6.1.0
+Requires-Dist: pydantic>=1.9.0
 
 An asyncio python library for the [Google Calendar API](https://developers.google.com/calendar/api). This library provides a simplified
 Google Calendar API that is lighter weight and more streamlined compared to using
 aiogoogle, and increased reliability by supporting efficient sync and reading
 from local storage. See the [API Documentation](https://allenporter.github.io/gcal_sync/).
 
 The focus of this API is on making it simple to access the most relevant parts of Google
 Calendar, for doing useful things. It may not support everything in the API however it
 should be easy to extend to do more as needed.
 
 # Quickstart
 
 In order to use the library, you'll need to do some work yourself to get authentication
-credentails. This depends a lot on the context (e.g. redirecting to use OAuth via web)
+credentials. This depends a lot on the context (e.g. redirecting to use OAuth via web)
 but should be easy to incorporate using Google's python authentication libraries. See
 Google's [Authentication and authorization overview](https://developers.google.com/workspace/guides/auth-overview) for details.
 
 You will implement `gcal_sync.AbstractAuth` to provide an access token. Your implementation
-will handle any necessary refreshes. You can invoke the service with your auth implentation
+will handle any necessary refreshes. You can invoke the service with your auth implementation
 to access the API.
 
 ```python
 from gcal_sync.auth import AbstractAuth
 
 
 class MyAuthImpl(gcal_sync.AbstractAuth):
```

### Comparing `gcal-sync-6.0.4/gcal_sync.egg-info/SOURCES.txt` & `gcal_sync-6.1.0/gcal_sync.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 ./gcal_sync/__init__.py
 ./gcal_sync/api.py
 ./gcal_sync/auth.py
 ./gcal_sync/const.py
 ./gcal_sync/exceptions.py
```

### Comparing `gcal-sync-6.0.4/tests/test_api.py` & `gcal_sync-6.1.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-6.0.4/tests/test_auth.py` & `gcal_sync-6.1.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-6.0.4/tests/test_model.py` & `gcal_sync-6.1.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-6.0.4/tests/test_store.py` & `gcal_sync-6.1.0/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-6.0.4/tests/test_sync.py` & `gcal_sync-6.1.0/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-6.0.4/tests/test_timeline.py` & `gcal_sync-6.1.0/tests/test_timeline.py`

 * *Files identical despite different names*

