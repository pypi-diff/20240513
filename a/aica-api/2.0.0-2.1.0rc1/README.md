# Comparing `tmp/aica_api-2.0.0.tar.gz` & `tmp/aica_api-2.1.0rc1.tar.gz`

## Comparing `aica_api-2.0.0.tar` & `aica_api-2.1.0rc1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 aica_api-2.0.0/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aica_api-2.0.0/src/aica_api/__init__.py
--rw-r--r--   0        0        0    12831 2020-02-02 00:00:00.000000 aica_api-2.0.0/src/aica_api/client.py
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 aica_api-2.0.0/src/aica_api/sio_client.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 aica_api-2.0.0/.gitignore
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 aica_api-2.0.0/LICENSE
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 aica_api-2.0.0/README.md
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 aica_api-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 aica_api-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 aica_api-2.1.0rc1/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aica_api-2.1.0rc1/src/aica_api/__init__.py
+-rw-r--r--   0        0        0    19092 2020-02-02 00:00:00.000000 aica_api-2.1.0rc1/src/aica_api/client.py
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 aica_api-2.1.0rc1/src/aica_api/sio_client.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 aica_api-2.1.0rc1/.gitignore
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 aica_api-2.1.0rc1/LICENSE
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 aica_api-2.1.0rc1/README.md
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 aica_api-2.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 aica_api-2.1.0rc1/PKG-INFO
```

### Comparing `aica_api-2.0.0/CHANGELOG.md` & `aica_api-2.1.0rc1/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 - [1.2.1](#121)
 - [1.2.0](#120)
 - [1.1.0](#102)
 - [1.0.2](#102)
 - [1.0.1](#101)
 - [1.0.0](#100)
 
+## Upcoming changes
+
+- feat: support hardware and controller states and predicates in `wait_for` functions (#156)
+- feat: define more detailed feature and function compatibility between versions (#158)
+
 ## 2.0.0
 
 This version of the AICA API client is compatible with the new AICA API server version 3.0 by using Socket.IO instead of
 raw websockets for run-time data. This change breaks backwards compatibility for API server versions v2.x and below.
 It uses Socket.IO instead of raw websockets for run-time data required by the new AICA framework API version 3.0.
 
 ### Breaking changes
```

### Comparing `aica_api-2.0.0/src/aica_api/client.py` & `aica_api-2.1.0rc1/src/aica_api/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,25 @@
+from deprecation import deprecated
+from functools import wraps
+from logging import getLogger
 from typing import Union, List
 
 import os
 import requests
+import semver
 import yaml
 
 import importlib.metadata
 
 from aica_api.sio_client import read_until
 
 
+CLIENT_VERSION = importlib.metadata.version('aica_api')
+
+
 class AICA:
     """
     API client for AICA applications.
     """
 
     # noinspection HttpUrlsUsage
     def __init__(self, url: str = 'localhost', port: Union[str, int] = '5000'):
@@ -28,53 +35,104 @@
         if url.startswith('http://'):
             self._address = f'{url}:{port}'
         elif '//' in url or ':' in url:
             raise ValueError(f'Invalid URL format {url}')
         else:
             self._address = f'http://{url}:{port}'
 
+        self._logger = getLogger(__name__)
+        self._api_version = None
+
     def _endpoint(self, endpoint=''):
         """
         Build the request address for a given endpoint.
 
         :param endpoint: The API endpoint
         :return: The constructed request address
         """
         return f'{self._address}/v2/{endpoint}'
 
     @staticmethod
+    def _requires_api_version(version):
+        """
+        Decorator to mark a function with a specific API server version constraint.
+        Elides the function call and returns None with a warning if the version constraint is violated.
+
+        Example usage:
+        @_requires_api_version('>=3.2.1')
+        def my_new_endpoint()
+          ...
+
+        :param version: The version constraint specifier (i.e. >=3.2.1)
+        """
+        def decorator(func):
+            @wraps(func)
+            def wrapper(self, *args, **kwargs):
+                if self._api_version is None and self.api_version() is None:
+                    return None
+                if not semver.match(self._api_version, version):
+                    self._logger.warning(f'The function {func.__name__} requires API server version {version}, '
+                                         f'but the current API server version is {self._api_version}')
+                    return None
+                return func(self, *args, **kwargs)
+
+            return wrapper
+
+        return decorator
+
+    def api_version(self) -> Union[str, None]:
+        """
+        Get the version of the AICA API server
+
+        :return: The version of the API server or None in case of
+        """
+        try:
+            self._api_version = requests.get(f'{self._address}/version').json()
+            self._logger.debug(f'API server version identified as {self._api_version}')
+        except requests.exceptions.RequestException:
+            self._logger.error(f'Error connecting to the API server at {self._address}! '
+                               f'Check that the AICA container is running and configured with the right address.')
+            self._api_version = None
+        return self._api_version
+
+    @staticmethod
     def client_version() -> str:
         """
         Get the version of this API client utility
 
         :return: The version of the API client
         """
-        return importlib.metadata.version('aica_api')
+        return CLIENT_VERSION
 
     def check(self) -> bool:
         """
         Check if this API client is compatible with the detected API server version
 
         :return: True if the client is compatible with the API server version, False otherwise
         """
-        try:
-            api_version = requests.get(f'{self._address}/version').json()
-        except requests.exceptions.RequestException as e:
-            print(f'Error connecting to the API! {e}')
+        if self._api_version is None and self.api_version() is None:
             return False
 
-        if api_version.startswith('3'):
+        version_info = semver.parse_version_info(self._api_version)
+
+        if version_info.major == 3:
             return True
-        elif api_version.startswith('2'):
-            print(f'The detected API version v{api_version} is older than the minimum API version v3.0.0 supported by '
-                  f'this client (v{self.client_version()}). Please install Python API client version v1.2.0 '
-                  f'for API server versions v2.X.')
+        elif version_info.major > 3:
+            self._logger.error(f'The detected API version v{self._api_version} is newer than the maximum API version '
+                               f'supported by this client (v{self.client_version()}). Please upgrade the Python API '
+                               f'client version for newer API server versions.')
+            return False
+        elif version_info.major == 2:
+            self._logger.error(f'The detected API version v{self._api_version} is older than the minimum API version '
+                               f'supported by this client (v{self.client_version()}). Please downgrade the Python API '
+                               f'client to version v1.2.0 for API server versions v2.X.')
             return False
         else:
-            print(f'The detected API version v{api_version} is deprecated and not supported by this API client!')
+            self._logger.error(f'The detected API version v{self._api_version} is deprecated and not supported by '
+                               f'this API client!')
             return False
 
     def component_descriptions(self) -> requests.Response:
         """
         Retrieve the JSON descriptions of all available components.
         """
         return requests.get(self._endpoint('components'))
@@ -262,42 +320,104 @@
     def get_application(self):
         """
         Get the application
         """
         endpoint = "application"
         return requests.get(self._endpoint(endpoint))
 
-    def wait_for_component(self, component: str, state: str, timeout: Union[None, int, float] = None):
+    def wait_for_component(self, component: str, state: str, timeout: Union[None, int, float] = None) -> bool:
         """
         Wait for a component to be in a particular state. Components can be in any of the following states:
             ['unloaded', 'loaded', 'unconfigured', 'inactive', 'active', 'finalized']
 
         :param component: The name of the component
-        :param state: The state of the component
+        :param state: The state of the component to wait for
         :param timeout: Timeout duration in seconds. If set to None, block indefinitely
-        :return: False if the connection times out before the component is in the intended state
+        :return: True if the component is in the intended state before the timeout duration, False otherwise
         """
         return read_until(lambda data: data[component]['state'] == state, url=self._address, namespace='/v2/components',
-                          event='component_data', timeout=timeout)
+                          event='component_data', timeout=timeout) is not None
+
+    @_requires_api_version('>=3.1.0')
+    def wait_for_hardware(self, hardware: str, state: str, timeout: Union[None, int, float] = None) -> bool:
+        """
+        Wait for a hardware interface to be in a particular state. Hardware can be in any of the following states:
+            ['unloaded', 'loaded']
 
-    def wait_for_predicate(self, component: str, predicate: str, timeout: Union[None, int, float] = None):
+        :param hardware: The name of the hardware interface
+        :param state: The state of the hardware to wait for
+        :param timeout: Timeout duration in seconds. If set to None, block indefinitely
+        :return: True if the hardware is in the intended state before the timeout duration, False otherwise
+        """
+        return read_until(lambda data: data[hardware]['state'] == state, url=self._address, namespace='/v2/hardware',
+                          event='hardware_data', timeout=timeout) is not None
+
+    @_requires_api_version('>=3.1.0')
+    def wait_for_controller(self, hardware: str, controller: str, state: str,
+                            timeout: Union[None, int, float] = None) -> bool:
+        """
+        Wait for a controller to be in a particular state. Controllers can be in any of the following states:
+            ['unloaded', 'loaded', 'unconfigured', 'inactive', 'active', 'finalized']
+
+        :param hardware: The name of the hardware interface responsible for the controller
+        :param controller: The name of the controller
+        :param state: The state of the controller to wait for
+        :param timeout: Timeout duration in seconds. If set to None, block indefinitely
+        :return: True if the controller is in the intended state before the timeout duration, False otherwise
+        """
+        return read_until(lambda data: data[hardware]['controllers'][controller]['state'] == state, url=self._address,
+                          namespace='/v2/hardware', event='hardware_data', timeout=timeout) is not None
+
+    @deprecated(deprecated_in='2.1.0', removed_in='3.0.0', current_version=CLIENT_VERSION,
+                details='Use the wait_for_component_predicate function instead')
+    def wait_for_predicate(self, component: str, predicate: str, timeout: Union[None, int, float] = None) -> bool:
         """
         Wait until a component predicate is true.
 
         :param component: The name of the component
         :param predicate: The name of the predicate
         :param timeout: Timeout duration in seconds. If set to None, block indefinitely
-        :return: False if the connection times out before the predicate is true
+        :return: True if the predicate is true before the timeout duration, False otherwise
+        """
+        return read_until(lambda data: data[component]['predicates'][predicate], url=self._address,
+                          namespace='/v2/components', event='component_data', timeout=timeout) is not None
+
+    @_requires_api_version('>=3.1.0')
+    def wait_for_component_predicate(self, component: str, predicate: str,
+                                     timeout: Union[None, int, float] = None) -> bool:
+        """
+        Wait until a component predicate is true.
+
+        :param component: The name of the component
+        :param predicate: The name of the predicate
+        :param timeout: Timeout duration in seconds. If set to None, block indefinitely
+        :return: True if the predicate is true before the timeout duration, False otherwise
+        """
+        return read_until(lambda data: data[component]['predicates'][predicate], url=self._address,
+                          namespace='/v2/components', event='component_data', timeout=timeout) is not None
+
+    @_requires_api_version('>=3.1.0')
+    def wait_for_controller_predicate(self, hardware: str, controller: str, predicate: str,
+                                      timeout: Union[None, int, float] = None) -> bool:
+        """
+        Wait until a controller predicate is true.
+
+        :param hardware: The name of the hardware interface responsible for the controller
+        :param controller: The name of the controller
+        :param predicate: The name of the predicate
+        :param timeout: Timeout duration in seconds. If set to None, block indefinitely
+        :return: True if the predicate is true before the timeout duration, False otherwise
         """
-        return read_until(lambda data: data[component]["predicates"][predicate], url=self._address,
-                          namespace='/v2/components', event='component_data', timeout=timeout)
+        return read_until(lambda data: data[hardware]['controllers'][controller]['predicates'][predicate],
+                          url=self._address, namespace='/v2/hardware', event='hardware_data',
+                          timeout=timeout) is not None
 
-    def wait_for_condition(self, condition, timeout=None):
+    def wait_for_condition(self, condition, timeout=None) -> bool:
         """
         Wait until a condition is true.
 
         :param condition: The name of the condition
         :param timeout: Timeout duration in seconds. If set to None, block indefinitely
-        :return: False if the connection times out before the condition is true
+        :return: True if the condition is true before the timeout duration, False otherwise
         """
         return read_until(lambda data: data[condition], url=self._address, namespace='/v2/conditions',
-                          event='conditions', timeout=timeout)
+                          event='conditions', timeout=timeout) is not None
```

### Comparing `aica_api-2.0.0/src/aica_api/sio_client.py` & `aica_api-2.1.0rc1/src/aica_api/sio_client.py`

 * *Files identical despite different names*

### Comparing `aica_api-2.0.0/LICENSE` & `aica_api-2.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `aica_api-2.0.0/pyproject.toml` & `aica_api-2.1.0rc1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aica_api"
-version = "2.0.0"
+version = "2.1.0-rc.1"
 authors = [
   { name="Enrico Eberhard", email="enrico@aica.tech" },
 ]
 description = "A client utility for the AICA API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
-    "requests >= 2.28.1",
-    "python-socketio[client] >= 5.11.0"
+    "deprecation ~= 2.1.0",
+    "python-socketio[client] ~= 5.11.0",
+    "pyyaml ~= 6.0.1",
+    "requests ~= 2.28.1",
+    "semver ~= 3.0.2"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `aica_api-2.0.0/PKG-INFO` & `aica_api-2.1.0rc1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: aica_api
-Version: 2.0.0
-Summary: A client utility for the AICA API
-Project-URL: Homepage, https://github.com/aica-technology/api
-Project-URL: Bug Tracker, https://github.com/aica-technology/api/issues
-Author-email: Enrico Eberhard <enrico@aica.tech>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Requires-Dist: python-socketio[client]>=5.11.0
-Requires-Dist: requests>=2.28.1
-Description-Content-Type: text/markdown
-
 # Python AICA API Client
 
 The AICA API client module provides simple functions for interacting with the AICA API.
 
 ```shell
 pip install aica-api
 ```
@@ -54,30 +38,41 @@
     print('Predicate is true!')
 else:
     print('Timed out before predicate was true')
 ```
 
 ## Compatability table
 
-The latest version of the AICA API client will generally support the latest API version in the AICA framework. For
-older versions of the AICA framework, it may be necessary to install older versions of the client. Use the following
-compatability table to determine which client version to use.
-
-| API server version | Matching Python client version |
-|--------------------|--------------------------------|
-| `v3.x`             | `>= v2.0.0`                    |
-| `v2.x`             | `v1.2.0`                       |
-| `<= v1.x`          | Unsupported                    |
+The latest version of the AICA API client will generally support the latest API server version in the AICA framework.
+Major changes to the API client or server versions indicate breaking changes and are not backwards compatible. To
+interact with older versions of the AICA framework, it may be necessary to install older versions of the client.
+Use the following compatability table to determine which client version to use.
+
+| API server version | Matching Python client version  |
+|--------------------|---------------------------------|
+| `3.x`              | `>= 2.0.0`                      |
+| `2.x`              | `1.2.0`                         |
+| `<= 1.x`           | Unsupported                     |
+
+Between major version changes, minor updates to the API server version and Python client versions may introduce new
+endpoints and functions respectively. If a function requires a feature that the detected API server version does not yet
+support (as is the case when the Python client version is more up-to-date than the targeted API server), then calling
+that function will return None with a warning.
 
 Recent client versions also support the following functions to check the client version and API compatability.
 
 ```python
 from aica_api.client import AICA
 
 aica = AICA()
 
+# get the current API server version
+print(aica.api_version())
 # get the current client version
-aica.client_version()
+print(aica.client_version())
 
 # check compatability between the client version and API version
-aica.check()
-```
+if aica.check():
+    print('Versions are compatible')
+else:
+    print('Versions are incompatible')
+```
```

