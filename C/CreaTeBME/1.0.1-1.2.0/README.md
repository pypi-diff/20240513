# Comparing `tmp/CreaTeBME-1.0.1.tar.gz` & `tmp/createbme-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CreaTeBME-1.0.1.tar", last modified: Tue May 16 14:24:14 2023, max compression
+gzip compressed data, was "createbme-1.2.0.tar", last modified: Mon May 13 11:45:44 2024, max compression
```

## Comparing `CreaTeBME-1.0.1.tar` & `createbme-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:24:14.192275 CreaTeBME-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-16 14:23:59.000000 CreaTeBME-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-16 14:24:14.192275 CreaTeBME-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-16 14:23:59.000000 CreaTeBME-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 14:23:59.000000 CreaTeBME-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 14:24:14.192275 CreaTeBME-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-16 14:23:59.000000 CreaTeBME-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:24:14.192275 CreaTeBME-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:24:14.192275 CreaTeBME-1.0.1/src/CreaTeBME/
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-05-16 14:23:59.000000 CreaTeBME-1.0.1/src/CreaTeBME/ImuSensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-16 14:23:59.000000 CreaTeBME-1.0.1/src/CreaTeBME/SensorEmulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-05-16 14:23:59.000000 CreaTeBME-1.0.1/src/CreaTeBME/SensorManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-16 14:23:59.000000 CreaTeBME-1.0.1/src/CreaTeBME/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-16 14:23:59.000000 CreaTeBME-1.0.1/src/CreaTeBME/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-16 14:23:59.000000 CreaTeBME-1.0.1/src/CreaTeBME/uuids.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:24:14.192275 CreaTeBME-1.0.1/src/CreaTeBME.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-16 14:24:14.000000 CreaTeBME-1.0.1/src/CreaTeBME.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-16 14:24:14.000000 CreaTeBME-1.0.1/src/CreaTeBME.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 14:24:14.000000 CreaTeBME-1.0.1/src/CreaTeBME.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 14:24:14.000000 CreaTeBME-1.0.1/src/CreaTeBME.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 14:24:14.000000 CreaTeBME-1.0.1/src/CreaTeBME.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:45:44.451104 createbme-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-13 11:45:39.000000 createbme-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-13 11:45:44.451104 createbme-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-13 11:45:39.000000 createbme-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-13 11:45:39.000000 createbme-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 11:45:44.451104 createbme-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-13 11:45:39.000000 createbme-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:45:44.447105 createbme-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:45:44.447105 createbme-1.2.0/src/CreaTeBME/
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-13 11:45:39.000000 createbme-1.2.0/src/CreaTeBME/ImuSensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-13 11:45:39.000000 createbme-1.2.0/src/CreaTeBME/SensorEmulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-13 11:45:39.000000 createbme-1.2.0/src/CreaTeBME/SensorManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-13 11:45:39.000000 createbme-1.2.0/src/CreaTeBME/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-13 11:45:39.000000 createbme-1.2.0/src/CreaTeBME/connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-13 11:45:39.000000 createbme-1.2.0/src/CreaTeBME/uuids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:45:44.451104 createbme-1.2.0/src/CreaTeBME.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-13 11:45:44.000000 createbme-1.2.0/src/CreaTeBME.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-13 11:45:44.000000 createbme-1.2.0/src/CreaTeBME.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 11:45:44.000000 createbme-1.2.0/src/CreaTeBME.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-13 11:45:44.000000 createbme-1.2.0/src/CreaTeBME.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-13 11:45:44.000000 createbme-1.2.0/src/CreaTeBME.egg-info/top_level.txt
```

### Comparing `CreaTeBME-1.0.1/LICENSE` & `createbme-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CreaTeBME-1.0.1/PKG-INFO` & `createbme-1.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,25 @@
-Metadata-Version: 2.1
-Name: CreaTeBME
-Version: 1.0.1
-Summary: Python Package for interfacing the bluetooth IMU module for CreaTe M8 BME.
-Home-page: https://github.com/CreaTe-M8-BME/CreaTeBME
-Author: Jonathan Matarazzi
-Author-email: git@jonathanm.nl
-Project-URL: Bug Tracker, https://github.com/CreaTe-M8-BME/CreaTeBME/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CreaTeBME
 
+[![Build](https://github.com/CreaTe-M8-BME/CreaTeBME/actions/workflows/build_publish.yml/badge.svg)](https://github.com/CreaTe-M8-BME/CreaTeBME/actions/workflows/build_publish.yml)
 [![PyPI](https://img.shields.io/pypi/v/CreaTeBME)](https://pypi.org/project/CreaTeBME/)
 
 Python Package for interfacing the bluetooth IMU module for CreaTe M8 BME.
 
 # Installation
-To install the latest stable version simply run
+To install the latest stable version simply run this in your terminal.
+If you are using PyCharm then you can open the terminal on the bottom left of the screen.
 ```shell
 pip install CreaTeBME
 ```
 
 # Example
 A simple example to connect to a sensor and read and print the data for 10 seconds.
+The package automatically connects to the device, so you do not have to connect to it manually.
 ```python
-import time
 from CreaTeBME import SensorManager
 
 # Create a sensor manager for the given sensor names using the given callback
 manager = SensorManager(['0BE6'])
 
 # Start the sensor manager
 manager.start()
@@ -57,33 +44,32 @@
 
 To connect to the sensors, simply initialize a `SensorManager` object with the sensor names.
 ```python
 from CreaTeBME import SensorManager
 
 manager = SensorManager(['A1B2', 'C3D4'])
 ```
+Then start reading data from the sensors by calling the `start` method of the `SensorManager`.
+```python
+manager.start()
+```
 
 To get the IMU measurements the `get_measurements()' method can be used.
 This returns the measurements received since the last time this method was called.
 ```python
 measurements = manager.get_measurements()
 ```
 
 The data returned by this method is a dictionary containing a list for each sensor with the received measurements.
 A single measurement is a list of 6 floats.
 The measurements are structured like this
 - **[0:2]** = x,y,z of accelerometer in (g).
 - **[3:5]** = x,y,z of gyroscope in (deg/s).
 
-To start reading data from the sensors call the `start` method of the `SensorManager`.
-```python
-manager.start()
-```
-
-Make sure to also call the `stop` method when exiting your program.
+Finally, make sure to also call the `stop` method when exiting your program.
 ```python
 manager.stop()
 ```
 ## Manual Connection
 ⚠️**Understanding of** asyncio **required**⚠️
 
 Another way of connecting IMU sensors is to manually create `ImuSensor` objects.
```

### Comparing `CreaTeBME-1.0.1/setup.py` & `createbme-1.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text('utf-8')
 
 setup(
     name='CreaTeBME',
-    version='1.0.1',
+    version='1.2.0',
     author='Jonathan Matarazzi',
     author_email='git@jonathanm.nl',
     description='Python Package for interfacing the bluetooth IMU module for CreaTe M8 BME.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/CreaTe-M8-BME/CreaTeBME',
     project_urls={
@@ -22,10 +22,10 @@
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent'
     ],
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     python_requires='>=3.7',
     install_requires=[
-        'bleak >= 0.19.5',
+        'bleak >= 0.22.1',
     ]
 )
```

### Comparing `CreaTeBME-1.0.1/src/CreaTeBME/ImuSensor.py` & `createbme-1.2.0/src/CreaTeBME/ImuSensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,17 @@
         await self.__bt_client.start_notify(self.__imu_char, self.__receive_reading)
 
         # Set sample rate if reserve exists
         if self.__sample_rate_reserve:
             await self.set_sample_rate(self.__sample_rate_reserve)
 
     async def disconnect(self) -> None:
+        """
+        Disconnect the BLE device.
+        """
         if self.__bt_client.is_connected:
             await self.__bt_client.stop_notify(self.__imu_char)
             await self.__bt_client.disconnect()
 
     async def set_sample_rate(self, sample_rate: int) -> bool:
         """
         Set the sample frequency of the sensor.
```

### Comparing `CreaTeBME-1.0.1/src/CreaTeBME/SensorEmulator.py` & `createbme-1.2.0/src/CreaTeBME/SensorEmulator.py`

 * *Files identical despite different names*

### Comparing `CreaTeBME-1.0.1/src/CreaTeBME/SensorManager.py` & `createbme-1.2.0/src/CreaTeBME/SensorManager.py`

 * *Files identical despite different names*

### Comparing `CreaTeBME-1.0.1/src/CreaTeBME/connect.py` & `createbme-1.2.0/src/CreaTeBME/connect.py`

 * *Files identical despite different names*

### Comparing `CreaTeBME-1.0.1/src/CreaTeBME.egg-info/PKG-INFO` & `createbme-1.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 Metadata-Version: 2.1
 Name: CreaTeBME
-Version: 1.0.1
+Version: 1.2.0
 Summary: Python Package for interfacing the bluetooth IMU module for CreaTe M8 BME.
 Home-page: https://github.com/CreaTe-M8-BME/CreaTeBME
 Author: Jonathan Matarazzi
 Author-email: git@jonathanm.nl
 Project-URL: Bug Tracker, https://github.com/CreaTe-M8-BME/CreaTeBME/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: bleak>=0.22.1
 
 # CreaTeBME
 
+[![Build](https://github.com/CreaTe-M8-BME/CreaTeBME/actions/workflows/build_publish.yml/badge.svg)](https://github.com/CreaTe-M8-BME/CreaTeBME/actions/workflows/build_publish.yml)
 [![PyPI](https://img.shields.io/pypi/v/CreaTeBME)](https://pypi.org/project/CreaTeBME/)
 
 Python Package for interfacing the bluetooth IMU module for CreaTe M8 BME.
 
 # Installation
-To install the latest stable version simply run
+To install the latest stable version simply run this in your terminal.
+If you are using PyCharm then you can open the terminal on the bottom left of the screen.
 ```shell
 pip install CreaTeBME
 ```
 
 # Example
 A simple example to connect to a sensor and read and print the data for 10 seconds.
+The package automatically connects to the device, so you do not have to connect to it manually.
 ```python
-import time
 from CreaTeBME import SensorManager
 
 # Create a sensor manager for the given sensor names using the given callback
 manager = SensorManager(['0BE6'])
 
 # Start the sensor manager
 manager.start()
@@ -57,33 +60,32 @@
 
 To connect to the sensors, simply initialize a `SensorManager` object with the sensor names.
 ```python
 from CreaTeBME import SensorManager
 
 manager = SensorManager(['A1B2', 'C3D4'])
 ```
+Then start reading data from the sensors by calling the `start` method of the `SensorManager`.
+```python
+manager.start()
+```
 
 To get the IMU measurements the `get_measurements()' method can be used.
 This returns the measurements received since the last time this method was called.
 ```python
 measurements = manager.get_measurements()
 ```
 
 The data returned by this method is a dictionary containing a list for each sensor with the received measurements.
 A single measurement is a list of 6 floats.
 The measurements are structured like this
 - **[0:2]** = x,y,z of accelerometer in (g).
 - **[3:5]** = x,y,z of gyroscope in (deg/s).
 
-To start reading data from the sensors call the `start` method of the `SensorManager`.
-```python
-manager.start()
-```
-
-Make sure to also call the `stop` method when exiting your program.
+Finally, make sure to also call the `stop` method when exiting your program.
 ```python
 manager.stop()
 ```
 ## Manual Connection
 ⚠️**Understanding of** asyncio **required**⚠️
 
 Another way of connecting IMU sensors is to manually create `ImuSensor` objects.
```

