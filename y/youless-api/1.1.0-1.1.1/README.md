# Comparing `tmp/youless_api-1.1.0.tar.gz` & `tmp/youless_api-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youless_api-1.1.0.tar", last modified: Tue Mar 12 13:30:30 2024, max compression
+gzip compressed data, was "youless_api-1.1.1.tar", last modified: Mon May 13 07:13:24 2024, max compression
```

## Comparing `youless_api-1.1.0.tar` & `youless_api-1.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-03-12 13:30:30.233663 youless_api-1.1.0/
--rw-rw-rw-   0        0        0     1899 2024-03-12 13:30:30.232663 youless_api-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1630 2024-03-12 13:15:11.000000 youless_api-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-03-12 13:30:30.234663 youless_api-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      541 2024-03-12 13:15:23.000000 youless_api-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-12 13:30:30.213127 youless_api-1.1.0/youless_api/
--rw-rw-rw-   0        0        0     4140 2024-03-12 13:15:11.000000 youless_api-1.1.0/youless_api/__init__.py
--rw-rw-rw-   0        0        0       42 2021-01-29 14:31:49.000000 youless_api-1.1.0/youless_api/const.py
-drwxrwxrwx   0        0        0        0 2024-03-12 13:30:30.223127 youless_api-1.1.0/youless_api/device/
--rw-rw-rw-   0        0        0     2645 2024-03-12 13:15:11.000000 youless_api-1.1.0/youless_api/device/LS110.py
--rw-rw-rw-   0        0        0     5705 2024-03-12 13:15:11.000000 youless_api-1.1.0/youless_api/device/LS120.py
--rw-rw-rw-   0        0        0      541 2024-03-12 13:15:11.000000 youless_api-1.1.0/youless_api/device/LS120_pv.py
--rw-rw-rw-   0        0        0     2100 2024-03-12 13:15:11.000000 youless_api-1.1.0/youless_api/device/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-12 13:30:30.230665 youless_api-1.1.0/youless_api/test/
--rw-rw-rw-   0        0        0      594 2024-03-12 13:15:11.000000 youless_api-1.1.0/youless_api/test/__init__.py
--rw-rw-rw-   0        0        0     1146 2024-03-12 13:15:11.000000 youless_api-1.1.0/youless_api/test/test_LS110.py
--rw-rw-rw-   0        0        0     5697 2024-03-12 13:15:11.000000 youless_api-1.1.0/youless_api/test/test_LS120.py
--rw-rw-rw-   0        0        0     1642 2024-03-12 13:15:11.000000 youless_api-1.1.0/youless_api/test/test_LS120_pv.py
--rw-rw-rw-   0        0        0     3907 2024-03-12 13:15:11.000000 youless_api-1.1.0/youless_api/test/test_api.py
--rw-rw-rw-   0        0        0      298 2024-03-12 13:15:11.000000 youless_api-1.1.0/youless_api/test/test_youless_sensor.py
--rw-rw-rw-   0        0        0     2079 2024-03-12 13:15:11.000000 youless_api-1.1.0/youless_api/youless_sensor.py
-drwxrwxrwx   0        0        0        0 2024-03-12 13:30:30.231663 youless_api-1.1.0/youless_api.egg-info/
--rw-rw-rw-   0        0        0     1899 2024-03-12 13:30:30.000000 youless_api-1.1.0/youless_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      579 2024-03-12 13:30:30.000000 youless_api-1.1.0/youless_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-12 13:30:30.000000 youless_api-1.1.0/youless_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2021-01-28 14:04:36.000000 youless_api-1.1.0/youless_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-03-12 13:30:30.000000 youless_api-1.1.0/youless_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:13:24.811150 youless_api-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-13 07:13:24.811150 youless_api-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-13 07:13:20.000000 youless_api-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 07:13:24.811150 youless_api-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-13 07:13:20.000000 youless_api-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:13:24.811150 youless_api-1.1.1/youless_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-13 07:13:20.000000 youless_api-1.1.1/youless_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-13 07:13:20.000000 youless_api-1.1.1/youless_api/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:13:24.811150 youless_api-1.1.1/youless_api/device/
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-13 07:13:20.000000 youless_api-1.1.1/youless_api/device/LS110.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-13 07:13:20.000000 youless_api-1.1.1/youless_api/device/LS120.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-13 07:13:20.000000 youless_api-1.1.1/youless_api/device/LS120_pv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-13 07:13:20.000000 youless_api-1.1.1/youless_api/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:13:24.811150 youless_api-1.1.1/youless_api/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-13 07:13:20.000000 youless_api-1.1.1/youless_api/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-13 07:13:20.000000 youless_api-1.1.1/youless_api/test/test_LS110.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-13 07:13:20.000000 youless_api-1.1.1/youless_api/test/test_LS120.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-13 07:13:20.000000 youless_api-1.1.1/youless_api/test/test_LS120_pv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-05-13 07:13:20.000000 youless_api-1.1.1/youless_api/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-13 07:13:20.000000 youless_api-1.1.1/youless_api/test/test_youless_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-13 07:13:20.000000 youless_api-1.1.1/youless_api/youless_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:13:24.811150 youless_api-1.1.1/youless_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-13 07:13:24.000000 youless_api-1.1.1/youless_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-13 07:13:24.000000 youless_api-1.1.1/youless_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 07:13:24.000000 youless_api-1.1.1/youless_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 07:13:24.000000 youless_api-1.1.1/youless_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 07:13:24.000000 youless_api-1.1.1/youless_api.egg-info/top_level.txt
```

### Comparing `youless_api-1.1.0/PKG-INFO` & `youless_api-1.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-Metadata-Version: 2.1
-Name: youless_api
-Version: 1.1.0
-Summary: A bridge for python to the YouLess sensor
-Home-page: https://bitbucket.org/jongsoftdev/youless-python-bridge/src/master/
-Author: G. Jongerius
-License: MIT
-Description-Content-Type: text/markdown
-
-# YouLess Python Data Bridge
-[![PyPI version](https://badge.fury.io/py/youless-api.svg)](https://badge.fury.io/py/youless-api)
-
-This package contains support classes to fetch data from the YouLess sensors. The current implementation
-supports the following YouLess devices:
-
-* LS120, both the Enologic and the PVOutput firmware
-* LS110
-
-Experimental support for authentication was added in v0.15 of the youless-python-bridge.
-
-## Contributing
-
-To request new features or report bugs please use:
-
-    https://jongsoftdev.atlassian.net/jira/software/c/projects/YA/issues/
-
-If you want to contribute by creating code yourself then create a fork of the repository and offer the changes in a PR back into this repository.
-
-## Using the python integration
-
-To use the API use the following code:
-
-```python
-from youless_api.youless_api import YoulessAPI
-
-if __name__ == '__main__':
-    api = YoulessAPI("192.168.1.2")  # use the ip address of the YouLess device
-    api.initialize()
-    api.update()
-
-    # from this point on on you should be able to access the sensors through the YouLess bridge
-    gasUsage = api.gas_meter.value
-```
-
-To use authentication please use the snippet below (this is still experimental):
-
-```python
-from youless_api.youless_api import YoulessAPI
-
-if __name__ == '__main__':
-    api = YoulessAPI("192.168.1.2", "my-user-name", "my-password")  # use the ip address of the YouLess device
-    api.initialize()
-    api.update()
-
-    # from this point on on you should be able to access the sensors through the YouLess bridge
-    gasUsage = api.gas_meter.value
-```
+Metadata-Version: 2.1
+Name: youless_api
+Version: 1.1.1
+Summary: A bridge for python to the YouLess sensor
+Home-page: https://github.com/gjong/youless-python-bridge
+Author: G. Jongerius
+License: MIT
+Description-Content-Type: text/markdown
+
+# YouLess Python Data Bridge
+[![PyPI version](https://badge.fury.io/py/youless-api.svg)](https://badge.fury.io/py/youless-api)
+
+This package contains support classes to fetch data from the YouLess sensors. The current implementation
+supports the following YouLess devices:
+
+* LS120, both the Enologic and the PVOutput firmware
+* LS110
+
+Experimental support for authentication was added in v0.15 of the youless-python-bridge.
+
+## Contributing
+
+To request new features or report bugs please use:
+
+    https://github.com/gjong/youless-python-bridge/issues/new
+
+If you want to contribute by creating code yourself then create a fork of the repository and offer the changes in a PR back into this repository.
+
+## Using the python integration
+
+To use the API use the following code:
+
+```python
+from youless_api.youless_api import YoulessAPI
+
+if __name__ == '__main__':
+    api = YoulessAPI("192.168.1.2")  # use the ip address of the YouLess device
+    api.initialize()
+    api.update()
+
+    # from this point on on you should be able to access the sensors through the YouLess bridge
+    gasUsage = api.gas_meter.value
+```
+
+To use authentication please use the snippet below (this is still experimental):
+
+```python
+from youless_api.youless_api import YoulessAPI
+
+if __name__ == '__main__':
+    api = YoulessAPI("192.168.1.2", "my-user-name", "my-password")  # use the ip address of the YouLess device
+    api.initialize()
+    api.update()
+
+    # from this point on on you should be able to access the sensors through the YouLess bridge
+    gasUsage = api.gas_meter.value
+```
```

### Comparing `youless_api-1.1.0/README.md` & `youless_api-1.1.1/youless_api.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,57 @@
-# YouLess Python Data Bridge
-[![PyPI version](https://badge.fury.io/py/youless-api.svg)](https://badge.fury.io/py/youless-api)
-
-This package contains support classes to fetch data from the YouLess sensors. The current implementation
-supports the following YouLess devices:
-
-* LS120, both the Enologic and the PVOutput firmware
-* LS110
-
-Experimental support for authentication was added in v0.15 of the youless-python-bridge.
-
-## Contributing
-
-To request new features or report bugs please use:
-
-    https://jongsoftdev.atlassian.net/jira/software/c/projects/YA/issues/
-
-If you want to contribute by creating code yourself then create a fork of the repository and offer the changes in a PR back into this repository.
-
-## Using the python integration
-
-To use the API use the following code:
-
-```python
-from youless_api.youless_api import YoulessAPI
-
-if __name__ == '__main__':
-    api = YoulessAPI("192.168.1.2")  # use the ip address of the YouLess device
-    api.initialize()
-    api.update()
-
-    # from this point on on you should be able to access the sensors through the YouLess bridge
-    gasUsage = api.gas_meter.value
-```
-
-To use authentication please use the snippet below (this is still experimental):
-
-```python
-from youless_api.youless_api import YoulessAPI
-
-if __name__ == '__main__':
-    api = YoulessAPI("192.168.1.2", "my-user-name", "my-password")  # use the ip address of the YouLess device
-    api.initialize()
-    api.update()
-
-    # from this point on on you should be able to access the sensors through the YouLess bridge
-    gasUsage = api.gas_meter.value
-```
+Metadata-Version: 2.1
+Name: youless_api
+Version: 1.1.1
+Summary: A bridge for python to the YouLess sensor
+Home-page: https://github.com/gjong/youless-python-bridge
+Author: G. Jongerius
+License: MIT
+Description-Content-Type: text/markdown
+
+# YouLess Python Data Bridge
+[![PyPI version](https://badge.fury.io/py/youless-api.svg)](https://badge.fury.io/py/youless-api)
+
+This package contains support classes to fetch data from the YouLess sensors. The current implementation
+supports the following YouLess devices:
+
+* LS120, both the Enologic and the PVOutput firmware
+* LS110
+
+Experimental support for authentication was added in v0.15 of the youless-python-bridge.
+
+## Contributing
+
+To request new features or report bugs please use:
+
+    https://github.com/gjong/youless-python-bridge/issues/new
+
+If you want to contribute by creating code yourself then create a fork of the repository and offer the changes in a PR back into this repository.
+
+## Using the python integration
+
+To use the API use the following code:
+
+```python
+from youless_api.youless_api import YoulessAPI
+
+if __name__ == '__main__':
+    api = YoulessAPI("192.168.1.2")  # use the ip address of the YouLess device
+    api.initialize()
+    api.update()
+
+    # from this point on on you should be able to access the sensors through the YouLess bridge
+    gasUsage = api.gas_meter.value
+```
+
+To use authentication please use the snippet below (this is still experimental):
+
+```python
+from youless_api.youless_api import YoulessAPI
+
+if __name__ == '__main__':
+    api = YoulessAPI("192.168.1.2", "my-user-name", "my-password")  # use the ip address of the YouLess device
+    api.initialize()
+    api.update()
+
+    # from this point on on you should be able to access the sensors through the YouLess bridge
+    gasUsage = api.gas_meter.value
+```
```

### Comparing `youless_api-1.1.0/youless_api/__init__.py` & `youless_api-1.1.1/youless_api/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,133 +1,141 @@
-"""
-This file contains a helper class to easily obtain data from the YouLess sensor.
-"""
-from typing import Optional
-
-import requests
-
-from youless_api.device import YouLessDevice
-from youless_api.device.LS110 import LS110
-from youless_api.device.LS120 import LS120
-from youless_api.device.LS120_pv import LS120PVOutput
-from youless_api.youless_sensor import YoulessSensor, PowerMeter, ExtraMeter, DeliveryMeter, Phase
-
-name = "youless_api"
-
-
-class YoulessAPI:
-    """A helper class to obtain data from the YouLess Sensor."""
-
-    _device: Optional[YouLessDevice]
-
-    def __init__(self, host, username=None, password=None):
-        """Initialize the data bridge."""
-        self._url = 'http://' + host
-        if username is None:
-            self._authentication = None
-        else:
-            self._authentication = (username, password)
-        self._device = None
-
-    def initialize(self):
-        """Establish a connection to the remote device"""
-        response = requests.get(f"{self._url}/d", auth=self._authentication, timeout=2)
-        if response.ok:
-            firmware_check = requests.get(f"{self._url}/e", auth=self._authentication, timeout=2)
-            if firmware_check.ok and firmware_check.headers['Content-Type'] == 'application/json':
-                self._device = LS120(self._url, response.json())
-            else:
-                self._device = LS120PVOutput(self._url, response.json())
-        else:
-            alive = requests.get(self._url, auth=self._authentication, timeout=2)
-            if alive.ok:
-                self._device = LS110(self._url)
-
-    def update(self):
-        """Fetch the latest settings from the Youless Sensor."""
-        if self._device:
-            self._device.update()
-
-    @property
-    def mac_address(self) -> Optional[str]:
-        """Get the MAC address of the connected device."""
-        if self._device is not None:
-            return self._device.mac_address
-
-        return None
-
-    @property
-    def model(self) -> Optional[str]:
-        """Return the model of the connected device."""
-        if self._device is not None:
-            return self._device.model
-
-        return None
-
-    @property
-    def gas_meter(self) -> Optional[YoulessSensor]:
-        """"Get the gas data available."""
-        if self._device is not None:
-            return self._device.gas_meter
-
-        return None
-
-    @property
-    def current_power_usage(self) -> Optional[YoulessSensor]:
-        """Get the current power usage."""
-        if self._device is not None:
-            return self._device.current_power_usage
-
-        return None
-
-    @property
-    def power_meter(self) -> Optional[PowerMeter]:
-        """Get the power meter values."""
-        if self._device is not None:
-            return self._device.power_meter
-
-        return None
-
-    @property
-    def delivery_meter(self) -> Optional[DeliveryMeter]:
-        """Get the power delivered values."""
-        if self._device is not None:
-            return self._device.delivery_meter
-
-        return None
-
-    @property
-    def extra_meter(self) -> Optional[ExtraMeter]:
-        """Get the meter values of an attached meter."""
-        if self._device is not None:
-            return self._device.extra_meter
-
-        return None
-
-    @property
-    def phase1(self) -> Optional[Phase]:
-        """Get the phase 1 information"""
-        if self._device is not None:
-            return self._device.phase1
-
-        return None
-
-    @property
-    def phase2(self) -> Optional[Phase]:
-        """Get the phase 1 information"""
-        if self._device is not None:
-            return self._device.phase2
-
-        return None
-
-    @property
-    def phase3(self) -> Optional[Phase]:
-        """Get the phase 1 information"""
-        if self._device is not None:
-            return self._device.phase3
-
-        return None
-
-    @property
-    def secured(self) -> bool:
-        """Flag indicating if the API has authentication or not."""
-        return self._authentication is not None
+"""
+This file contains a helper class to easily obtain data from the YouLess sensor.
+"""
+from typing import Optional
+
+import requests
+
+from youless_api.device import YouLessDevice
+from youless_api.device.LS110 import LS110
+from youless_api.device.LS120 import LS120
+from youless_api.device.LS120_pv import LS120PVOutput
+from youless_api.youless_sensor import YoulessSensor, PowerMeter, ExtraMeter, DeliveryMeter, Phase
+
+name = "youless_api"
+
+
+class YoulessAPI:
+    """A helper class to obtain data from the YouLess Sensor."""
+
+    _device: Optional[YouLessDevice]
+
+    def __init__(self, host, username=None, password=None):
+        """Initialize the data bridge."""
+        self._url = 'http://' + host
+        if username is None:
+            self._authentication = None
+        else:
+            self._authentication = (username, password)
+        self._device = None
+
+    def initialize(self):
+        """Establish a connection to the remote device"""
+        response = requests.get(f"{self._url}/d", auth=self._authentication, timeout=2)
+        if response.ok:
+            firmware_check = requests.get(f"{self._url}/e", auth=self._authentication, timeout=2)
+            if firmware_check.ok and firmware_check.headers['Content-Type'] == 'application/json':
+                self._device = LS120(self._url, response.json())
+            else:
+                self._device = LS120PVOutput(self._url, response.json())
+        else:
+            alive = requests.get(self._url, auth=self._authentication, timeout=2)
+            if alive.ok:
+                self._device = LS110(self._url)
+
+    def update(self):
+        """Fetch the latest settings from the Youless Sensor."""
+        if self._device:
+            self._device.update()
+
+    @property
+    def mac_address(self) -> Optional[str]:
+        """Get the MAC address of the connected device."""
+        if self._device is not None:
+            return self._device.mac_address
+
+        return None
+
+    @property
+    def model(self) -> Optional[str]:
+        """Return the model of the connected device."""
+        if self._device is not None:
+            return self._device.model
+
+        return None
+
+    @property
+    def water_meter(self) -> Optional[YoulessSensor]:
+        """"Get the water data available."""
+        if self._device is not None:
+            return self._device.water_meter
+
+        return None
+
+    @property
+    def gas_meter(self) -> Optional[YoulessSensor]:
+        """"Get the gas data available."""
+        if self._device is not None:
+            return self._device.gas_meter
+
+        return None
+
+    @property
+    def current_power_usage(self) -> Optional[YoulessSensor]:
+        """Get the current power usage."""
+        if self._device is not None:
+            return self._device.current_power_usage
+
+        return None
+
+    @property
+    def power_meter(self) -> Optional[PowerMeter]:
+        """Get the power meter values."""
+        if self._device is not None:
+            return self._device.power_meter
+
+        return None
+
+    @property
+    def delivery_meter(self) -> Optional[DeliveryMeter]:
+        """Get the power delivered values."""
+        if self._device is not None:
+            return self._device.delivery_meter
+
+        return None
+
+    @property
+    def extra_meter(self) -> Optional[ExtraMeter]:
+        """Get the meter values of an attached meter."""
+        if self._device is not None:
+            return self._device.extra_meter
+
+        return None
+
+    @property
+    def phase1(self) -> Optional[Phase]:
+        """Get the phase 1 information"""
+        if self._device is not None:
+            return self._device.phase1
+
+        return None
+
+    @property
+    def phase2(self) -> Optional[Phase]:
+        """Get the phase 1 information"""
+        if self._device is not None:
+            return self._device.phase2
+
+        return None
+
+    @property
+    def phase3(self) -> Optional[Phase]:
+        """Get the phase 1 information"""
+        if self._device is not None:
+            return self._device.phase3
+
+        return None
+
+    @property
+    def secured(self) -> bool:
+        """Flag indicating if the API has authentication or not."""
+        return self._authentication is not None
```

### Comparing `youless_api-1.1.0/youless_api/device/LS110.py` & `youless_api-1.1.1/youless_api/device/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,82 +1,83 @@
-import requests
-from typing import Optional
-
-from youless_api.device import YouLessDevice
-from youless_api.const import STATE_OK, STATE_FAILED
-from youless_api.youless_sensor import YoulessSensor, PowerMeter, ExtraMeter
-
-
-def validate_basic_response(raw_data: dict) -> dict:
-    """Validate the response from the old /a interface and adjust the dict if needed."""
-
-    corrected = {**{'cs0': None, 'ps0': None}, **raw_data}
-    parse_float_values_for = ['cnt', 'cs0']
-
-    for correct_value in parse_float_values_for:
-        if correct_value in corrected and corrected[correct_value] is not None:
-            corrected[correct_value] = float(corrected[correct_value].replace(",", "."))
-
-    return corrected
-
-
-class LS110(YouLessDevice):
-    """The device integration for the Youless LS110"""
-
-    def __init__(self, host):
-        """Initialize the integration"""
-        super().__init__()
-        self._host = host
-        self._cache = None
-        self._state = STATE_OK
-
-
-    @property
-    def state(self) -> Optional[str]:
-        """Get the current device connectivity state"""
-        return self._state
-
-    @property
-    def model(self) -> Optional[str]:
-        """Return the device model"""
-        return "LS110"
-
-    @property
-    def power_meter(self) -> Optional[PowerMeter]:
-        """Fetch the power meter values from the internal cache"""
-        if self._cache is not None:
-            return PowerMeter(
-                YoulessSensor(None, None),
-                YoulessSensor(None, None),
-                YoulessSensor(self._cache['cnt'], 'kWh')
-            )
-
-        return None
-
-    @property
-    def current_power_usage(self) -> Optional[YoulessSensor]:
-        """Fetch the current power usage from the internal cache"""
-        if self._cache is not None:
-            return YoulessSensor(self._cache['pwr'], 'W')
-
-        return None
-
-    @property
-    def extra_meter(self):
-        """Get the meter values of an attached meter."""
-        if self._cache is not None:
-            return ExtraMeter(
-                YoulessSensor(self._cache['cs0'], 'kWh'),
-                YoulessSensor(self._cache['ps0'], 'W')
-            )
-
-        return None
-
-    def update(self) -> None:
-        """Update the sensor values from the device"""
-        response = requests.get(f"{self._host}/a?f=j", timeout=2)
-        if response.ok:
-            validated_response = validate_basic_response(response.json())
-            self._state = STATE_OK
-            self._cache = validated_response
-        else:
-            self._state = STATE_FAILED
+from typing import Optional
+
+from youless_api.youless_sensor import YoulessSensor, PowerMeter, DeliveryMeter, ExtraMeter, Phase
+
+
+class YouLessDevice:
+    """The base class for the Youless devices"""
+
+    def __init__(self):
+        """Initialize the state"""
+
+    @property
+    def state(self) -> Optional[str]:
+        """The current state of the connection"""
+        return None
+
+    @property
+    def error(self) -> Optional[str]:
+        """Returns the last known error, only if state == 'FAILED'"""
+        return None
+
+    @property
+    def mac_address(self) -> Optional[str]:
+        """Returns the MAC address"""
+        return None
+
+    @property
+    def firmware(self) -> Optional[str]:
+        """Returns the current firmware on the device."""
+        return None
+
+    @property
+    def model(self) -> Optional[str]:
+        """Returns the model number of the device"""
+        return None
+
+    @property
+    def water_meter(self) -> Optional[YoulessSensor]:
+        """"Get the water data available."""
+        return None
+
+    @property
+    def gas_meter(self) -> Optional[YoulessSensor]:
+        """"Get the gas data available."""
+        return None
+
+    @property
+    def current_power_usage(self) -> Optional[YoulessSensor]:
+        """Get the current power usage."""
+        return None
+
+    @property
+    def power_meter(self) -> Optional[PowerMeter]:
+        """Get the power meter values."""
+        return None
+
+    @property
+    def delivery_meter(self) -> Optional[DeliveryMeter]:
+        """Get the power delivered values."""
+        return None
+
+    @property
+    def extra_meter(self) -> Optional[ExtraMeter]:
+        """Get the meter values of an attached meter."""
+        return None
+
+    @property
+    def phase1(self) -> Optional[Phase]:
+        """Get the phase 1 information"""
+        return None
+
+    @property
+    def phase2(self) -> Optional[Phase]:
+        """Get the phase 1 information"""
+        return None
+
+    @property
+    def phase3(self) -> Optional[Phase]:
+        """Get the phase 1 information"""
+        return None
+
+    def update(self) -> None:
+        """Placeholder to update values from device"""
```

### Comparing `youless_api-1.1.0/youless_api/device/LS120.py` & `youless_api-1.1.1/youless_api/device/LS120.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,179 +1,179 @@
-import datetime
-from typing import Optional
-
-import requests
-
-from youless_api.const import STATE_OK, STATE_FAILED
-from youless_api.device import YouLessDevice
-from youless_api.youless_sensor import YoulessSensor, PowerMeter, ExtraMeter, DeliveryMeter, Phase
-
-
-def validate_enologic_response(raw_data: dict) -> dict:
-    """Validate the response to verify that it makes sense and no junk data is returned"""
-
-    corrected = {**{'p1': None, 'p2': None, 'n1': None, 'n2': None, 'gas': None, 'wtr': None}, **raw_data}
-    if 'gts' in corrected:
-        formatted_date = datetime.datetime.now().strftime("%y%m%d") + "0000"
-        if corrected["gts"] != 0 and int(formatted_date) >= corrected["gts"]:
-            corrected["gas"] = None
-
-    if 'wts' in corrected:
-        formatted_date = datetime.datetime.now().strftime("%y%m%d") + "0000"
-        if corrected["wts"] != 0 and int(formatted_date) >= corrected["wts"]:
-            corrected["wtr"] = None
-
-    return corrected
-
-def supports_phases(firmware: Optional[str]) -> bool:
-    """Determine if the provided firmware supports phase information."""
-    if firmware is not None:
-        major_ver = float(firmware[0:3])
-        return major_ver >= 1.5
-
-    return False
-
-
-class LS120(YouLessDevice):
-    """The device integration for the Youless LS120"""
-
-    def __init__(self, host, device_information):
-        """Initialize the integration"""
-        super().__init__()
-        self._host = host
-        self._cache = None
-        self._phases = None
-        self._state = STATE_OK
-        self._info = device_information
-        self._phase_support = supports_phases(device_information.get('fw', None))
-
-    @property
-    def gas_meter(self):
-        """"Get the gas meter from the internal cache"""
-        if self._cache is not None:
-            return YoulessSensor(self._cache['gas'], 'm3')
-
-        return None
-
-    @property
-    def water_meter(self):
-        """"Get the water meter from the internal cache"""
-        if self._cache is not None:
-            return YoulessSensor(self._cache['wtr'], 'm3')
-
-        return None
-
-    @property
-    def current_power_usage(self):
-        """Get the current power usage from the internal cache"""
-        if self._cache is not None:
-            return YoulessSensor(self._cache['pwr'], 'W')
-
-        return None
-
-    @property
-    def power_meter(self):
-        """Get the power meter values."""
-        if self._cache is not None:
-            return PowerMeter(
-                YoulessSensor(self._cache['p1'], 'kWh'),
-                YoulessSensor(self._cache['p2'], 'kWh'),
-                YoulessSensor(self._cache['net'], 'kWh')
-            )
-
-        return None
-
-    @property
-    def delivery_meter(self):
-        """Get the power delivered values."""
-        if self._cache is not None:
-            return DeliveryMeter(
-                YoulessSensor(self._cache['n1'], 'kWh'),
-                YoulessSensor(self._cache['n2'], 'kWh')
-            )
-
-        return None
-
-    @property
-    def extra_meter(self):
-        """Get the meter values of an attached meter."""
-        if self._cache is not None:
-            return ExtraMeter(
-                YoulessSensor(self._cache['cs0'], 'kWh'),
-                YoulessSensor(self._cache['ps0'], 'W')
-            )
-
-        return None
-
-    @property
-    def state(self) -> Optional[str]:
-        """Returns the current connectivity state"""
-        return self._state
-
-    @property
-    def mac_address(self) -> Optional[str]:
-        """Return the MAC address"""
-        if self._info is not None:
-            return self._info['mac']
-
-        return None
-
-    @property
-    def model(self) -> Optional[str]:
-        """Return the device model"""
-        return "LS120"
-
-    @property
-    def firmware(self) -> Optional[str]:
-        """Returns the actual firmware on the device."""
-        if self._info is not None and 'fw' in self._info:
-            return self._info['fw']
-
-        return None
-
-    @property
-    def phase1(self) -> Optional[Phase]:
-        if self._phases is not None:
-            return Phase(
-                YoulessSensor(self._phases['i1'], ''),
-                YoulessSensor(self._phases['v1'], ''),
-                YoulessSensor(self._phases['l1'], ''))
-
-        return None
-
-    @property
-    def phase2(self) -> Optional[Phase]:
-        if self._phases is not None:
-            return Phase(
-                YoulessSensor(self._phases['i2'], ''),
-                YoulessSensor(self._phases['v2'], ''),
-                YoulessSensor(self._phases['l2'], ''))
-
-        return None
-
-    @property
-    def phase3(self) -> Optional[Phase]:
-        if self._phases is not None:
-            return Phase(
-                YoulessSensor(self._phases['i3'], ''),
-                YoulessSensor(self._phases['v3'], ''),
-                YoulessSensor(self._phases['l3'], ''))
-
-        return None
-
-    def update(self) -> None:
-        """Update the sensor values from the device"""
-        response = requests.get(f"{self._host}/e", timeout=2)
-        if response.ok:
-            response = validate_enologic_response(response.json()[0])
-            if response is not None:
-                self._state = STATE_OK
-                self._cache = response
-            else:
-                self._state = STATE_FAILED
-        else:
-            self._state = STATE_FAILED
-
-        if self._phase_support:
-            response = requests.get(f"{self._host}/f", timeout=2)
-            if response.ok:
-                self._phases = response.json()
+import datetime
+from typing import Optional
+
+import requests
+
+from youless_api.const import STATE_OK, STATE_FAILED
+from youless_api.device import YouLessDevice
+from youless_api.youless_sensor import YoulessSensor, PowerMeter, ExtraMeter, DeliveryMeter, Phase
+
+
+def validate_enologic_response(raw_data: dict) -> dict:
+    """Validate the response to verify that it makes sense and no junk data is returned"""
+
+    corrected = {**{'p1': None, 'p2': None, 'n1': None, 'n2': None, 'gas': None, 'wtr': None}, **raw_data}
+    if 'gts' in corrected:
+        formatted_date = datetime.datetime.now().strftime("%y%m%d") + "0000"
+        if corrected["gts"] != 0 and int(formatted_date) >= corrected["gts"]:
+            corrected["gas"] = None
+
+    if 'wts' in corrected:
+        formatted_date = datetime.datetime.now().strftime("%y%m%d") + "0000"
+        if corrected["wts"] != 0 and int(formatted_date) >= corrected["wts"]:
+            corrected["wtr"] = None
+
+    return corrected
+
+def supports_phases(firmware: Optional[str]) -> bool:
+    """Determine if the provided firmware supports phase information."""
+    if firmware is not None:
+        major_ver = float(firmware[0:3])
+        return major_ver >= 1.5
+
+    return False
+
+
+class LS120(YouLessDevice):
+    """The device integration for the Youless LS120"""
+
+    def __init__(self, host, device_information):
+        """Initialize the integration"""
+        super().__init__()
+        self._host = host
+        self._cache = None
+        self._phases = None
+        self._state = STATE_OK
+        self._info = device_information
+        self._phase_support = supports_phases(device_information.get('fw', None))
+
+    @property
+    def gas_meter(self):
+        """"Get the gas meter from the internal cache"""
+        if self._cache is not None:
+            return YoulessSensor(self._cache['gas'], 'm3')
+
+        return None
+
+    @property
+    def water_meter(self):
+        """"Get the water meter from the internal cache"""
+        if self._cache is not None:
+            return YoulessSensor(self._cache['wtr'], 'm3')
+
+        return None
+
+    @property
+    def current_power_usage(self):
+        """Get the current power usage from the internal cache"""
+        if self._cache is not None:
+            return YoulessSensor(self._cache['pwr'], 'W')
+
+        return None
+
+    @property
+    def power_meter(self):
+        """Get the power meter values."""
+        if self._cache is not None:
+            return PowerMeter(
+                YoulessSensor(self._cache['p1'], 'kWh'),
+                YoulessSensor(self._cache['p2'], 'kWh'),
+                YoulessSensor(self._cache['net'], 'kWh')
+            )
+
+        return None
+
+    @property
+    def delivery_meter(self):
+        """Get the power delivered values."""
+        if self._cache is not None:
+            return DeliveryMeter(
+                YoulessSensor(self._cache['n1'], 'kWh'),
+                YoulessSensor(self._cache['n2'], 'kWh')
+            )
+
+        return None
+
+    @property
+    def extra_meter(self):
+        """Get the meter values of an attached meter."""
+        if self._cache is not None:
+            return ExtraMeter(
+                YoulessSensor(self._cache['cs0'], 'kWh'),
+                YoulessSensor(self._cache['ps0'], 'W')
+            )
+
+        return None
+
+    @property
+    def state(self) -> Optional[str]:
+        """Returns the current connectivity state"""
+        return self._state
+
+    @property
+    def mac_address(self) -> Optional[str]:
+        """Return the MAC address"""
+        if self._info is not None:
+            return self._info['mac']
+
+        return None
+
+    @property
+    def model(self) -> Optional[str]:
+        """Return the device model"""
+        return "LS120"
+
+    @property
+    def firmware(self) -> Optional[str]:
+        """Returns the actual firmware on the device."""
+        if self._info is not None and 'fw' in self._info:
+            return self._info['fw']
+
+        return None
+
+    @property
+    def phase1(self) -> Optional[Phase]:
+        if self._phases is not None:
+            return Phase(
+                YoulessSensor(self._phases['i1'], ''),
+                YoulessSensor(self._phases['v1'], ''),
+                YoulessSensor(self._phases['l1'], ''))
+
+        return None
+
+    @property
+    def phase2(self) -> Optional[Phase]:
+        if self._phases is not None:
+            return Phase(
+                YoulessSensor(self._phases['i2'], ''),
+                YoulessSensor(self._phases['v2'], ''),
+                YoulessSensor(self._phases['l2'], ''))
+
+        return None
+
+    @property
+    def phase3(self) -> Optional[Phase]:
+        if self._phases is not None:
+            return Phase(
+                YoulessSensor(self._phases['i3'], ''),
+                YoulessSensor(self._phases['v3'], ''),
+                YoulessSensor(self._phases['l3'], ''))
+
+        return None
+
+    def update(self) -> None:
+        """Update the sensor values from the device"""
+        response = requests.get(f"{self._host}/e", timeout=2)
+        if response.ok:
+            response = validate_enologic_response(response.json()[0])
+            if response is not None:
+                self._state = STATE_OK
+                self._cache = response
+            else:
+                self._state = STATE_FAILED
+        else:
+            self._state = STATE_FAILED
+
+        if self._phase_support:
+            response = requests.get(f"{self._host}/f", timeout=2)
+            if response.ok:
+                self._phases = response.json()
```

### Comparing `youless_api-1.1.0/youless_api/test/__init__.py` & `youless_api-1.1.1/youless_api/test/__init__.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-
-URI_ELOGIC = '/e'
-URI_DEVICE_INFO = '/d'
-URI_GENERIC = '/a?f=j'
-URI_PHASES = '/f'
-
-
-class MockResponse:
-
-    def __init__(self):
-        self._ok = False
-        self._json = lambda: 0
-        self._headers = {}
-        self._text = ''
-
-    def setup(self, ok, json, text, headers):
-        self._ok = ok
-        self._json = json
-        self._text = text
-        self._headers = headers
-
-    @property
-    def ok(self):
-        return self._ok
-
-    def json(self):
-        return self._json()
-
-    @property
-    def headers(self):
-        return self._headers
+
+URI_ELOGIC = '/e'
+URI_DEVICE_INFO = '/d'
+URI_GENERIC = '/a?f=j'
+URI_PHASES = '/f'
+
+
+class MockResponse:
+
+    def __init__(self):
+        self._ok = False
+        self._json = lambda: 0
+        self._headers = {}
+        self._text = ''
+
+    def setup(self, ok, json, text, headers):
+        self._ok = ok
+        self._json = json
+        self._text = text
+        self._headers = headers
+
+    @property
+    def ok(self):
+        return self._ok
+
+    def json(self):
+        return self._json()
+
+    @property
+    def headers(self):
+        return self._headers
```

### Comparing `youless_api-1.1.0/youless_api/test/test_LS110.py` & `youless_api-1.1.1/youless_api/test/test_LS110.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from unittest import TestCase
-from unittest.mock import patch, Mock
-
-from youless_api.const import STATE_OK
-from youless_api.device.LS110 import LS110
-
-
-class LS110Test(TestCase):
-
-    def test_ls110_ok(self):
-        with patch('youless_api.device.LS110.requests.get') as mock_get:
-            mock_get.return_value = Mock(ok=True)
-            mock_get.return_value.json.return_value = {
-                "cnt": "141950,625",
-                "pwr": 750,
-                "lvl": 90,
-                "dev": "(&plusmn;3%)",
-                "det": "",
-                "con": "OK",
-                "sts": "(33)",
-                "raw": 743
-            }
-
-            api = LS110('')
-            api.update()
-
-        self.assertEqual(api.state, STATE_OK)
-        self.assertEqual(api.power_meter.high.value, None)
-        self.assertEqual(api.power_meter.low.value, None)
-        self.assertEqual(api.power_meter.total.unit_of_measurement, "kWh")
-        self.assertEqual(api.power_meter.total.value, 141950.625)
-        self.assertEqual(api.current_power_usage.value, 750)
-        self.assertEqual(api.firmware, None)
+from unittest import TestCase
+from unittest.mock import patch, Mock
+
+from youless_api.const import STATE_OK
+from youless_api.device.LS110 import LS110
+
+
+class LS110Test(TestCase):
+
+    def test_ls110_ok(self):
+        with patch('youless_api.device.LS110.requests.get') as mock_get:
+            mock_get.return_value = Mock(ok=True)
+            mock_get.return_value.json.return_value = {
+                "cnt": "141950,625",
+                "pwr": 750,
+                "lvl": 90,
+                "dev": "(&plusmn;3%)",
+                "det": "",
+                "con": "OK",
+                "sts": "(33)",
+                "raw": 743
+            }
+
+            api = LS110('')
+            api.update()
+
+        self.assertEqual(api.state, STATE_OK)
+        self.assertEqual(api.power_meter.high.value, None)
+        self.assertEqual(api.power_meter.low.value, None)
+        self.assertEqual(api.power_meter.total.unit_of_measurement, "kWh")
+        self.assertEqual(api.power_meter.total.value, 141950.625)
+        self.assertEqual(api.current_power_usage.value, 750)
+        self.assertEqual(api.firmware, None)
```

### Comparing `youless_api-1.1.0/youless_api/test/test_LS120.py` & `youless_api-1.1.1/youless_api/test/test_LS120.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,171 +1,171 @@
-import datetime
-from unittest import TestCase
-from unittest.mock import patch, Mock
-
-from youless_api.const import STATE_FAILED, STATE_OK
-from youless_api.device.LS120 import LS120
-from youless_api.test import MockResponse, URI_ELOGIC, URI_PHASES
-
-default_ok_response = [{
-    "tm": 1611929119,
-    "net": 9194.164,
-    "pwr": 2382,
-    "ts0": 1608654000,
-    "cs0": 0.000,
-    "ps0": 0,
-    "p1": 4703.562,
-    "p2": 4490.631,
-    "n1": 0.029,
-    "n2": 0.000,
-    "gas": 1624.264,
-    "gts": int(datetime.datetime.now().strftime("%y%m%d%H00")),
-    "wtr": 1234.564,
-    "wts": int(datetime.datetime.now().strftime("%y%m%d%H00"))
-}]
-default_phases_response = {
-    "ver": 50,
-    "tr": 2,
-    "i1": 0.000,
-    "i2": 0.000,
-    "i3": 2.000,
-    "v1": 231.600,
-    "v2": 230.400,
-    "v3": 233.100,
-    "l1": 64,
-    "l2": 103,
-    "l3": 312
-}
-
-
-def mock_ls120_ok(*args, **kwargs) -> MockResponse:
-    response = MockResponse()
-    if args[0] == URI_ELOGIC:
-        response.setup(
-            True,
-            lambda: default_ok_response,
-            '',
-            {'Content-Type': 'application/json'}
-        )
-
-    return response
-
-
-def mock_ls120_phase_output(*args, **kwargs) -> MockResponse:
-    response = mock_ls120_ok(*args, *kwargs)
-
-    if args[0] == URI_PHASES:
-        response.setup(
-            True,
-            lambda: default_phases_response,
-            '',
-            {'Content-Type': 'application/json'}
-        )
-
-    return response
-
-
-class LS120Tests(TestCase):
-
-    def test_ls120_failed(self):
-        """Check what happens if the remote device is not ok"""
-        with patch('youless_api.device.LS120.requests.get') as mock_get:
-            mock_get.return_value = Mock(ok=False)
-
-            api = LS120('', {})
-            api.update()
-
-        self.assertEqual(api.state, STATE_FAILED)
-
-    @patch('youless_api.device.LS120.requests.get', side_effect=mock_ls120_ok)
-    def test_ls120_ok(self, mock_get):
-        """Test the update functionality."""
-        api = LS120('', {})
-        api.update()
-
-        self.assertEqual(api.state, STATE_OK)
-        self.assertEqual(api.firmware, None)
-
-        self.assertEqual(api.power_meter.total.value, 9194.164)
-        self.assertEqual(api.power_meter.high.value, 4490.631)
-        self.assertEqual(api.power_meter.low.value, 4703.562)
-        self.assertEqual(api.current_power_usage.value, 2382)
-        self.assertEqual(api.gas_meter.value, 1624.264)
-        self.assertEqual(api.water_meter.value, 1234.564)
-        self.assertEqual(api.delivery_meter.high.value, 0.000)
-        self.assertEqual(api.delivery_meter.low.value, 0.029)
-        self.assertEqual(api.phase1, None)
-        self.assertEqual(api.phase2, None)
-        self.assertEqual(api.phase3, None)
-
-    def test_ls120_gas_stale(self):
-        """Test case for incident with stale data from the API"""
-        with patch('youless_api.device.LS120.requests.get') as mock_get:
-            mock_get.return_value = Mock(ok=True)
-            mock_get.return_value.json.return_value = [{
-                "tm": 1611929119,
-                "net": 9194.164,
-                "pwr": 2382,
-                "ts0": 1608654000,
-                "cs0": 0.000,
-                "ps0": 0,
-                "p1": 4703.562,
-                "p2": 4490.631,
-                "n1": 0.029,
-                "n2": 0.000,
-                "gas": 1624.264,
-                "gts": 3894900,
-                "wtr": 1234.564,
-                "wts": 3894900
-            }]
-
-            api = LS120('', {})
-            api.update()
-
-        self.assertEqual(api.state, STATE_OK)
-        self.assertIsNone(api.gas_meter.value)
-
-    def test_ls120_missing_p_and_n(self):
-        """Test case for incident with missing sensors from the API"""
-        with patch('youless_api.device.LS120.requests.get') as mock_get:
-            mock_get.return_value = Mock(ok=True)
-            mock_get.return_value.json.return_value = [{
-                "tm": 1611929119,
-                "net": 9194.164,
-                "pwr": 2382,
-                "ts0": 1608654000,
-                "cs0": 0.000,
-                "ps0": 0,
-                "gas": 1624.264,
-                "gts": int(datetime.datetime.now().strftime("%y%m%d%H00")),
-                "wtr": 1234.564,
-                "wts": int(datetime.datetime.now().strftime("%y%m%d%H00"))
-            }]
-
-            api = LS120('', {})
-            api.update()
-
-        self.assertEqual(api.state, STATE_OK)
-        self.assertEqual(api.power_meter.high.value, None)
-        self.assertEqual(api.power_meter.low.value, None)
-
-    @patch('youless_api.device.LS120.requests.get', side_effect=mock_ls120_phase_output)
-    def test_ls120_with_phases(self, mock_get):
-        """Test case for the new 1.5.x firmware with phases"""
-        api = LS120('', {
-            "model": "LS120",
-            "mac": "xxxx",
-            "fw": "1.5.3-EL"
-        })
-        api.update()
-
-        self.assertEqual(api.state, STATE_OK)
-        self.assertEqual(api.firmware, '1.5.3-EL')
-        self.assertEqual(api.phase1.current.value, 0.000)
-        self.assertEqual(api.phase1.voltage.value, 231.600)
-        self.assertEqual(api.phase1.power.value, 64)
-        self.assertEqual(api.phase2.current.value, 0.000)
-        self.assertEqual(api.phase2.voltage.value, 230.400)
-        self.assertEqual(api.phase2.power.value, 103)
-        self.assertEqual(api.phase3.current.value, 2.000)
-        self.assertEqual(api.phase3.voltage.value, 233.100)
-        self.assertEqual(api.phase3.power.value, 312)
+import datetime
+from unittest import TestCase
+from unittest.mock import patch, Mock
+
+from youless_api.const import STATE_FAILED, STATE_OK
+from youless_api.device.LS120 import LS120
+from youless_api.test import MockResponse, URI_ELOGIC, URI_PHASES
+
+default_ok_response = [{
+    "tm": 1611929119,
+    "net": 9194.164,
+    "pwr": 2382,
+    "ts0": 1608654000,
+    "cs0": 0.000,
+    "ps0": 0,
+    "p1": 4703.562,
+    "p2": 4490.631,
+    "n1": 0.029,
+    "n2": 0.000,
+    "gas": 1624.264,
+    "gts": int(datetime.datetime.now().strftime("%y%m%d%H00")),
+    "wtr": 1234.564,
+    "wts": int(datetime.datetime.now().strftime("%y%m%d%H00"))
+}]
+default_phases_response = {
+    "ver": 50,
+    "tr": 2,
+    "i1": 0.000,
+    "i2": 0.000,
+    "i3": 2.000,
+    "v1": 231.600,
+    "v2": 230.400,
+    "v3": 233.100,
+    "l1": 64,
+    "l2": 103,
+    "l3": 312
+}
+
+
+def mock_ls120_ok(*args, **kwargs) -> MockResponse:
+    response = MockResponse()
+    if args[0] == URI_ELOGIC:
+        response.setup(
+            True,
+            lambda: default_ok_response,
+            '',
+            {'Content-Type': 'application/json'}
+        )
+
+    return response
+
+
+def mock_ls120_phase_output(*args, **kwargs) -> MockResponse:
+    response = mock_ls120_ok(*args, *kwargs)
+
+    if args[0] == URI_PHASES:
+        response.setup(
+            True,
+            lambda: default_phases_response,
+            '',
+            {'Content-Type': 'application/json'}
+        )
+
+    return response
+
+
+class LS120Tests(TestCase):
+
+    def test_ls120_failed(self):
+        """Check what happens if the remote device is not ok"""
+        with patch('youless_api.device.LS120.requests.get') as mock_get:
+            mock_get.return_value = Mock(ok=False)
+
+            api = LS120('', {})
+            api.update()
+
+        self.assertEqual(api.state, STATE_FAILED)
+
+    @patch('youless_api.device.LS120.requests.get', side_effect=mock_ls120_ok)
+    def test_ls120_ok(self, mock_get):
+        """Test the update functionality."""
+        api = LS120('', {})
+        api.update()
+
+        self.assertEqual(api.state, STATE_OK)
+        self.assertEqual(api.firmware, None)
+
+        self.assertEqual(api.power_meter.total.value, 9194.164)
+        self.assertEqual(api.power_meter.high.value, 4490.631)
+        self.assertEqual(api.power_meter.low.value, 4703.562)
+        self.assertEqual(api.current_power_usage.value, 2382)
+        self.assertEqual(api.gas_meter.value, 1624.264)
+        self.assertEqual(api.water_meter.value, 1234.564)
+        self.assertEqual(api.delivery_meter.high.value, 0.000)
+        self.assertEqual(api.delivery_meter.low.value, 0.029)
+        self.assertEqual(api.phase1, None)
+        self.assertEqual(api.phase2, None)
+        self.assertEqual(api.phase3, None)
+
+    def test_ls120_gas_stale(self):
+        """Test case for incident with stale data from the API"""
+        with patch('youless_api.device.LS120.requests.get') as mock_get:
+            mock_get.return_value = Mock(ok=True)
+            mock_get.return_value.json.return_value = [{
+                "tm": 1611929119,
+                "net": 9194.164,
+                "pwr": 2382,
+                "ts0": 1608654000,
+                "cs0": 0.000,
+                "ps0": 0,
+                "p1": 4703.562,
+                "p2": 4490.631,
+                "n1": 0.029,
+                "n2": 0.000,
+                "gas": 1624.264,
+                "gts": 3894900,
+                "wtr": 1234.564,
+                "wts": 3894900
+            }]
+
+            api = LS120('', {})
+            api.update()
+
+        self.assertEqual(api.state, STATE_OK)
+        self.assertIsNone(api.gas_meter.value)
+
+    def test_ls120_missing_p_and_n(self):
+        """Test case for incident with missing sensors from the API"""
+        with patch('youless_api.device.LS120.requests.get') as mock_get:
+            mock_get.return_value = Mock(ok=True)
+            mock_get.return_value.json.return_value = [{
+                "tm": 1611929119,
+                "net": 9194.164,
+                "pwr": 2382,
+                "ts0": 1608654000,
+                "cs0": 0.000,
+                "ps0": 0,
+                "gas": 1624.264,
+                "gts": int(datetime.datetime.now().strftime("%y%m%d%H00")),
+                "wtr": 1234.564,
+                "wts": int(datetime.datetime.now().strftime("%y%m%d%H00"))
+            }]
+
+            api = LS120('', {})
+            api.update()
+
+        self.assertEqual(api.state, STATE_OK)
+        self.assertEqual(api.power_meter.high.value, None)
+        self.assertEqual(api.power_meter.low.value, None)
+
+    @patch('youless_api.device.LS120.requests.get', side_effect=mock_ls120_phase_output)
+    def test_ls120_with_phases(self, mock_get):
+        """Test case for the new 1.5.x firmware with phases"""
+        api = LS120('', {
+            "model": "LS120",
+            "mac": "xxxx",
+            "fw": "1.5.3-EL"
+        })
+        api.update()
+
+        self.assertEqual(api.state, STATE_OK)
+        self.assertEqual(api.firmware, '1.5.3-EL')
+        self.assertEqual(api.phase1.current.value, 0.000)
+        self.assertEqual(api.phase1.voltage.value, 231.600)
+        self.assertEqual(api.phase1.power.value, 64)
+        self.assertEqual(api.phase2.current.value, 0.000)
+        self.assertEqual(api.phase2.voltage.value, 230.400)
+        self.assertEqual(api.phase2.power.value, 103)
+        self.assertEqual(api.phase3.current.value, 2.000)
+        self.assertEqual(api.phase3.voltage.value, 233.100)
+        self.assertEqual(api.phase3.power.value, 312)
```

### Comparing `youless_api-1.1.0/youless_api/test/test_LS120_pv.py` & `youless_api-1.1.1/youless_api/test/test_LS120_pv.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-import unittest
-
-from unittest.mock import patch
-
-from youless_api.device.LS120_pv import LS120PVOutput
-from youless_api.test import MockResponse, URI_ELOGIC, URI_GENERIC
-
-
-def mock_ls120_pvoutput(*args, **kwargs) -> MockResponse:
-    response = MockResponse()
-
-    def raise_ex(e):
-        raise Exception(e)
-
-    if args[0] == URI_ELOGIC:
-        response.setup(
-            True,
-            lambda: raise_ex("Unsupported operation"),
-            'd=20210903&t=14:58&v1=3024759&v2=370&c1=1&v3=19623222&v4=300',
-            {'Content-Type': 'text/html'})
-
-    if args[0] == URI_GENERIC:
-        response.setup(
-            True,
-            lambda: {
-                "cnt": " 16600,536",
-                "pwr": -930,
-                "lvl": 0,
-                "dev": "",
-                "det": "",
-                "con": "OK",
-                "sts": "(245)",
-                "cs0": " 3021,525",
-                "ps0": 1288,
-                "raw": 0},
-            '',
-            {'Content-Type': 'application/json'})
-
-    return response
-
-
-class LS120Tests(unittest.TestCase):
-
-    @patch('youless_api.device.LS110.requests.get', side_effect=mock_ls120_pvoutput)
-    def test_ls120_pvoutput_firmware(self, mock_get):
-        api = LS120PVOutput('', {})
-        api.update()
-
-        self.assertEqual(api.current_power_usage.value, -930)
-        self.assertEqual(api.power_meter.total.value, 16600.536)
-        self.assertEqual(api.extra_meter.usage.value, 1288)
-        self.assertEqual(api.extra_meter.total.value, 3021.525)
-        self.assertEqual(api.extra_meter.usage.value, 1288)
-
+import unittest
+
+from unittest.mock import patch
+
+from youless_api.device.LS120_pv import LS120PVOutput
+from youless_api.test import MockResponse, URI_ELOGIC, URI_GENERIC
+
+
+def mock_ls120_pvoutput(*args, **kwargs) -> MockResponse:
+    response = MockResponse()
+
+    def raise_ex(e):
+        raise Exception(e)
+
+    if args[0] == URI_ELOGIC:
+        response.setup(
+            True,
+            lambda: raise_ex("Unsupported operation"),
+            'd=20210903&t=14:58&v1=3024759&v2=370&c1=1&v3=19623222&v4=300',
+            {'Content-Type': 'text/html'})
+
+    if args[0] == URI_GENERIC:
+        response.setup(
+            True,
+            lambda: {
+                "cnt": " 16600,536",
+                "pwr": -930,
+                "lvl": 0,
+                "dev": "",
+                "det": "",
+                "con": "OK",
+                "sts": "(245)",
+                "cs0": " 3021,525",
+                "ps0": 1288,
+                "raw": 0},
+            '',
+            {'Content-Type': 'application/json'})
+
+    return response
+
+
+class LS120Tests(unittest.TestCase):
+
+    @patch('youless_api.device.LS110.requests.get', side_effect=mock_ls120_pvoutput)
+    def test_ls120_pvoutput_firmware(self, mock_get):
+        api = LS120PVOutput('', {})
+        api.update()
+
+        self.assertEqual(api.current_power_usage.value, -930)
+        self.assertEqual(api.power_meter.total.value, 16600.536)
+        self.assertEqual(api.extra_meter.usage.value, 1288)
+        self.assertEqual(api.extra_meter.total.value, 3021.525)
+        self.assertEqual(api.extra_meter.usage.value, 1288)
+
```

### Comparing `youless_api-1.1.0/youless_api.egg-info/PKG-INFO` & `youless_api-1.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,48 @@
-Metadata-Version: 2.1
-Name: youless_api
-Version: 1.1.0
-Summary: A bridge for python to the YouLess sensor
-Home-page: https://bitbucket.org/jongsoftdev/youless-python-bridge/src/master/
-Author: G. Jongerius
-License: MIT
-Description-Content-Type: text/markdown
-
-# YouLess Python Data Bridge
-[![PyPI version](https://badge.fury.io/py/youless-api.svg)](https://badge.fury.io/py/youless-api)
-
-This package contains support classes to fetch data from the YouLess sensors. The current implementation
-supports the following YouLess devices:
-
-* LS120, both the Enologic and the PVOutput firmware
-* LS110
-
-Experimental support for authentication was added in v0.15 of the youless-python-bridge.
-
-## Contributing
-
-To request new features or report bugs please use:
-
-    https://jongsoftdev.atlassian.net/jira/software/c/projects/YA/issues/
-
-If you want to contribute by creating code yourself then create a fork of the repository and offer the changes in a PR back into this repository.
-
-## Using the python integration
-
-To use the API use the following code:
-
-```python
-from youless_api.youless_api import YoulessAPI
-
-if __name__ == '__main__':
-    api = YoulessAPI("192.168.1.2")  # use the ip address of the YouLess device
-    api.initialize()
-    api.update()
-
-    # from this point on on you should be able to access the sensors through the YouLess bridge
-    gasUsage = api.gas_meter.value
-```
-
-To use authentication please use the snippet below (this is still experimental):
-
-```python
-from youless_api.youless_api import YoulessAPI
-
-if __name__ == '__main__':
-    api = YoulessAPI("192.168.1.2", "my-user-name", "my-password")  # use the ip address of the YouLess device
-    api.initialize()
-    api.update()
-
-    # from this point on on you should be able to access the sensors through the YouLess bridge
-    gasUsage = api.gas_meter.value
-```
+# YouLess Python Data Bridge
+[![PyPI version](https://badge.fury.io/py/youless-api.svg)](https://badge.fury.io/py/youless-api)
+
+This package contains support classes to fetch data from the YouLess sensors. The current implementation
+supports the following YouLess devices:
+
+* LS120, both the Enologic and the PVOutput firmware
+* LS110
+
+Experimental support for authentication was added in v0.15 of the youless-python-bridge.
+
+## Contributing
+
+To request new features or report bugs please use:
+
+    https://github.com/gjong/youless-python-bridge/issues/new
+
+If you want to contribute by creating code yourself then create a fork of the repository and offer the changes in a PR back into this repository.
+
+## Using the python integration
+
+To use the API use the following code:
+
+```python
+from youless_api.youless_api import YoulessAPI
+
+if __name__ == '__main__':
+    api = YoulessAPI("192.168.1.2")  # use the ip address of the YouLess device
+    api.initialize()
+    api.update()
+
+    # from this point on on you should be able to access the sensors through the YouLess bridge
+    gasUsage = api.gas_meter.value
+```
+
+To use authentication please use the snippet below (this is still experimental):
+
+```python
+from youless_api.youless_api import YoulessAPI
+
+if __name__ == '__main__':
+    api = YoulessAPI("192.168.1.2", "my-user-name", "my-password")  # use the ip address of the YouLess device
+    api.initialize()
+    api.update()
+
+    # from this point on on you should be able to access the sensors through the YouLess bridge
+    gasUsage = api.gas_meter.value
+```
```

### Comparing `youless_api-1.1.0/youless_api.egg-info/SOURCES.txt` & `youless_api-1.1.1/youless_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

