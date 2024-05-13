# Comparing `tmp/pyuptech-0.1.4a0.tar.gz` & `tmp/pyuptech-0.1.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuptech-0.1.4a0.tar", last modified: Sun Apr 21 09:30:44 2024, max compression
+gzip compressed data, was "pyuptech-0.1.4a1.tar", last modified: Sun Apr 21 11:35:46 2024, max compression
```

## Comparing `pyuptech-0.1.4a0.tar` & `pyuptech-0.1.4a1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     8297 2024-04-21 09:30:25.579958 pyuptech-0.1.4a0/README.md
--rw-r--r--   0        0        0      547 2024-04-21 09:30:44.336152 pyuptech-0.1.4a0/pyproject.toml
--rw-r--r--   0        0        0     1280 2024-04-21 09:30:25.579958 pyuptech-0.1.4a0/src/pyuptech/__init__.py
--rw-r--r--   0        0        0   219512 2024-04-21 09:30:25.583958 pyuptech-0.1.4a0/src/pyuptech/lib/libuptech.so
--rw-r--r--   0        0        0      110 2024-04-21 09:30:25.583958 pyuptech-0.1.4a0/src/pyuptech/modules/constant.py
--rw-r--r--   0        0        0     1933 2024-04-21 09:30:25.583958 pyuptech-0.1.4a0/src/pyuptech/modules/emulation.py
--rw-r--r--   0        0        0     1096 2024-04-21 09:30:25.583958 pyuptech-0.1.4a0/src/pyuptech/modules/loader.py
--rw-r--r--   0        0        0      577 2024-04-21 09:30:25.583958 pyuptech-0.1.4a0/src/pyuptech/modules/logger.py
--rw-r--r--   0        0        0     1761 2024-04-21 09:30:25.583958 pyuptech-0.1.4a0/src/pyuptech/modules/pins.py
--rw-r--r--   0        0        0    10454 2024-04-21 09:30:25.583958 pyuptech-0.1.4a0/src/pyuptech/modules/screen.py
--rw-r--r--   0        0        0    10681 2024-04-21 09:30:25.583958 pyuptech-0.1.4a0/src/pyuptech/modules/sensors.py
--rw-r--r--   0        0        0     6040 2024-04-21 09:30:25.583958 pyuptech-0.1.4a0/src/pyuptech/tools/display.py
--rw-r--r--   0        0        0      252 2024-04-21 09:30:25.583958 pyuptech-0.1.4a0/tests/__init__.py
--rw-r--r--   0        0        0      386 2024-04-21 09:30:25.583958 pyuptech-0.1.4a0/tests/display_tests.py
--rw-r--r--   0        0        0     1036 2024-04-21 09:30:25.583958 pyuptech-0.1.4a0/tests/perf_tests.py
--rw-r--r--   0        0        0     8614 1970-01-01 00:00:00.000000 pyuptech-0.1.4a0/PKG-INFO
+-rw-r--r--   0        0        0     8297 2024-04-21 11:35:28.293904 pyuptech-0.1.4a1/README.md
+-rw-r--r--   0        0        0      547 2024-04-21 11:35:46.454119 pyuptech-0.1.4a1/pyproject.toml
+-rw-r--r--   0        0        0     1280 2024-04-21 11:35:28.293904 pyuptech-0.1.4a1/src/pyuptech/__init__.py
+-rw-r--r--   0        0        0   219512 2024-04-21 11:35:28.293904 pyuptech-0.1.4a1/src/pyuptech/lib/libuptech.so
+-rw-r--r--   0        0        0      110 2024-04-21 11:35:28.293904 pyuptech-0.1.4a1/src/pyuptech/modules/constant.py
+-rw-r--r--   0        0        0     2043 2024-04-21 11:35:28.293904 pyuptech-0.1.4a1/src/pyuptech/modules/emulation.py
+-rw-r--r--   0        0        0     1096 2024-04-21 11:35:28.293904 pyuptech-0.1.4a1/src/pyuptech/modules/loader.py
+-rw-r--r--   0        0        0      577 2024-04-21 11:35:28.293904 pyuptech-0.1.4a1/src/pyuptech/modules/logger.py
+-rw-r--r--   0        0        0     1761 2024-04-21 11:35:28.297904 pyuptech-0.1.4a1/src/pyuptech/modules/pins.py
+-rw-r--r--   0        0        0    10454 2024-04-21 11:35:28.297904 pyuptech-0.1.4a1/src/pyuptech/modules/screen.py
+-rw-r--r--   0        0        0    11278 2024-04-21 11:35:28.297904 pyuptech-0.1.4a1/src/pyuptech/modules/sensors.py
+-rw-r--r--   0        0        0     6148 2024-04-21 11:35:28.297904 pyuptech-0.1.4a1/src/pyuptech/tools/display.py
+-rw-r--r--   0        0        0      252 2024-04-21 11:35:28.297904 pyuptech-0.1.4a1/tests/__init__.py
+-rw-r--r--   0        0        0      386 2024-04-21 11:35:28.297904 pyuptech-0.1.4a1/tests/display_tests.py
+-rw-r--r--   0        0        0     1036 2024-04-21 11:35:28.297904 pyuptech-0.1.4a1/tests/perf_tests.py
+-rw-r--r--   0        0        0     8614 1970-01-01 00:00:00.000000 pyuptech-0.1.4a1/PKG-INFO
```

### Comparing `pyuptech-0.1.4a0/README.md` & `pyuptech-0.1.4a1/README.md`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.4a0/pyproject.toml` & `pyuptech-0.1.4a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyuptech"
-version = "0.1.4a0"
+version = "0.1.4a1"
 description = "A Python wrapper for the uptech binary lib"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "coloredlogs>=15.0.1",
     "terminaltables>=3.1.10",
```

### Comparing `pyuptech-0.1.4a0/src/pyuptech/__init__.py` & `pyuptech-0.1.4a1/src/pyuptech/__init__.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.4a0/src/pyuptech/lib/libuptech.so` & `pyuptech-0.1.4a1/src/pyuptech/lib/libuptech.so`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.4a0/src/pyuptech/modules/emulation.py` & `pyuptech-0.1.4a1/src/pyuptech/modules/emulation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import ctypes
 from random import randint
 from typing import Self, Literal, Any
 
-from .sensors import OnBoardSensors
+from .sensors import OnBoardSensors, MPUDataPack, ADCDataPack
 
 
 class SensorEmulator(OnBoardSensors):
     mpu_rand_range = (0, 2**32 - 1)
     adc_rand_range = (0, 2**16 - 1)
     io_rand_range = (0, 2**8 - 1)
 
@@ -25,46 +25,46 @@
     def set_all_io_mode(self, mode: Literal[0, 1]) -> Self:
         return self
 
     def set_all_io_level(self, level: Literal[0, 1]) -> Self:
         return self
 
     @staticmethod
-    def io_all_channels() -> ctypes.c_uint8:
-        return ctypes.c_uint8(randint(*SensorEmulator.io_rand_range))
+    def io_all_channels() -> int:
+        return ctypes.c_uint8(randint(*SensorEmulator.io_rand_range)).value
 
-    def adc_all_channels(self) -> ctypes.Array:
+    def adc_all_channels(self) -> ADCDataPack:
 
         for i in range(10):
             self._adc_all[i] = randint(*self.adc_rand_range)
 
-        return self._adc_all
+        return tuple(self._adc_all)  # type: ignore
 
     def MPU6500_Open(self) -> Self:
         return self
 
-    def acc_all(self) -> ctypes.Array:
+    def acc_all(self) -> MPUDataPack:
         for i in range(3):
             self._accel_all[i] = randint(*self.mpu_rand_range)
-        return self._accel_all
+        return tuple(self._accel_all)  # type: ignore
 
-    def gyro_all(self) -> ctypes.Array:
+    def gyro_all(self) -> MPUDataPack:
         for i in range(3):
             self._gyro_all[i] = randint(*self.mpu_rand_range)
-        return self._gyro_all
+        return tuple(self._gyro_all)  # type: ignore
 
-    def atti_all(self) -> ctypes.Array:
+    def atti_all(self) -> MPUDataPack:
         for i in range(3):
             self._atti_all[i] = randint(*self.mpu_rand_range)
-        return self._atti_all
+        return tuple(self._atti_all)  # type: ignore
 
     @staticmethod
     def get_io_level(index: Literal[0, 1, 2, 3, 4, 5, 6, 7]) -> int:
         return randint(0, 1)
 
     @staticmethod
-    def get_all_io_mode() -> bytes:
-        return ctypes.c_char(randint(*SensorEmulator.io_rand_range)).value
+    def get_all_io_mode() -> int:
+        return ctypes.c_char(randint(*SensorEmulator.io_rand_range)).value[0]
 
     @staticmethod
     def get_handle(attr_name: str) -> Any:
         raise NotImplementedError("Emulation is not supported")
```

### Comparing `pyuptech-0.1.4a0/src/pyuptech/modules/loader.py` & `pyuptech-0.1.4a1/src/pyuptech/modules/loader.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.4a0/src/pyuptech/modules/logger.py` & `pyuptech-0.1.4a1/src/pyuptech/modules/logger.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.4a0/src/pyuptech/modules/pins.py` & `pyuptech-0.1.4a1/src/pyuptech/modules/pins.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.4a0/src/pyuptech/modules/screen.py` & `pyuptech-0.1.4a1/src/pyuptech/modules/screen.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.4a0/src/pyuptech/modules/sensors.py` & `pyuptech-0.1.4a1/src/pyuptech/modules/sensors.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import ctypes
 from time import perf_counter_ns
-from typing import Self, Literal, Any, Callable
+from typing import Self, Literal, Any, Callable, Tuple, TypeAlias
 
 from .loader import TECHSTAR_LIB
 from .logger import _logger
 
 E6 = 1000000
 
 """
@@ -15,14 +15,17 @@
 LOW = 0
 """
 # this will create a function that returns a C array, but it can't be recognized correctly by the pycharm
 ADCArrayType: Callable = ctypes.c_uint16 * 10  # type: ignore
 # on 32bit machine, this will create a C array of 3 floats with bit-width of 4 bytes
 MPUArrayType: Callable = ctypes.c_float * 3  # type: ignore
 
+ADCDataPack: TypeAlias = Tuple[int, int, int, int, int, int, int, int, int, int]
+MPUDataPack: TypeAlias = Tuple[float, float, float]
+
 
 class OnBoardSensors:
     """
     provides sealed methods accessing to the IOs and builtin sensors
 
     Owns 10 ADC channels and 3 MPU channels  and 8 IO channels
 
@@ -43,14 +46,15 @@
         Parameters:
             adc_min_sample_interval_ms (int): The minimum sample interval in milliseconds for the ADC channels. Defaults to 5.
 
         Examples:
             >>> on_board = OnBoardSensors().adc_io_open().set_all_io_mode(0).set_all_io_level(1).MPU6500_Open()
         """
 
+        self._adc_cache: ADCDataPack = (0,) * 10
         self._adc_all: ctypes.Array = ADCArrayType()
         self._accel_all: ctypes.Array = MPUArrayType()
         self._gyro_all: ctypes.Array = MPUArrayType()
         self._atti_all: ctypes.Array = MPUArrayType()
 
         self.__adc_last_sample_timestamp: int = perf_counter_ns()
 
@@ -92,32 +96,33 @@
         close the adc-io plug
         """
         _logger.info("Closing ADC-IO")
         if TECHSTAR_LIB.adc_io_close() == -1:
             _logger.error("Failed to close ADC-IO")
         return self
 
-    def adc_all_channels(self) -> ctypes.Array:
+    def adc_all_channels(self) -> ADCDataPack:
         """
         Get all the ADC channels. Length = 10
 
         Returns:
-            ctypes.Array: An array containing the values of all the ADC channels.
+            ADCDataPack: An array containing the values of all the ADC channels.
         """
 
         can_update_time = (
             self.__adc_last_sample_timestamp + self.__adc_min_sample_interval_ns
         )
         if can_update_time > (current := perf_counter_ns()):
 
-            return self._adc_all
+            return self._adc_cache
         self.__adc_last_sample_timestamp = current
         if TECHSTAR_LIB.ADC_GetAll(self._adc_all):
             _logger.error("Failed to get all ADC channels")
-        return self._adc_all
+        self._adc_cache = tuple(self._adc_all)
+        return self._adc_cache  # type: ignore
 
     def set_io_level(self, index: int, level: Literal[0, 1]) -> Self:
         """
         Set the level of the specified IO index.
 
         Args:
             index (int): The index of the IO.
@@ -157,25 +162,28 @@
             The function returns the instance of the class.
         """
         if TECHSTAR_LIB.adc_io_SetAll(level):
             _logger.error("Failed to set all IO level")
         return self
 
     @staticmethod
-    def get_all_io_mode() -> bytes:
+    def get_all_io_mode() -> int:
         """
         Get all IO modes. length = 8,store as bit0,bit1,bit2,bit3,bit4,bit5,bit6,bit7
 
         Returns:
-            bytes: A buffer containing all IO modes.
+            int: A buffer containing all IO modes.
+        Examples:
+            0b10000000 => 第io7为输出模式，可用于驱动舵机
+            0b00000001 => 第io0为输入模式，可用于外接传感器
         """
         buffer = ctypes.c_char()
         if TECHSTAR_LIB.adc_io_ModeGetAll(buffer):
             _logger.error("Failed to get all IO mode")
-        return buffer.value
+        return buffer.value[0]
 
     @staticmethod
     def get_io_level(index: Literal[0, 1, 2, 3, 4, 5, 6, 7]) -> int:
         """
         Get the level of the specified IO index.
 
         Args:
@@ -231,90 +239,94 @@
             The function returns the instance of the class.
         """
         if TECHSTAR_LIB.adc_io_ModeSet(index, mode):
             _logger.error(f"Failed to set IO mode, index: {index}, mode: {mode}")
         return self
 
     @staticmethod
-    def io_all_channels() -> ctypes.c_uint8:
+    def io_all_channels() -> int:
         """
         get all io plug input levels
 
         uint8, each bit represents a channel, 1 for high, 0 for low
+
+        Examples:
+            0b10000000 => 第io7为高电平
+            0b00000001 => 第io0为高电平
         """
-        return TECHSTAR_LIB.adc_io_InputGetAll()
+        return TECHSTAR_LIB.adc_io_InputGetAll().value
 
     def MPU6500_Open(self) -> Self:
         """
         initialize the 6-axis enhancer MPU6500
         default settings:
             acceleration: -+8G
             gyro: -+2000 degree/s
             sampling rate: 1kHz
         """
         _logger.info("Initializing MPU6500...")
         if TECHSTAR_LIB.mpu6500_dmp_init():
             _logger.warning("Failed to initialize MPU6500")
         return self
 
-    def acc_all(self) -> ctypes.Array:
+    def acc_all(self) -> MPUDataPack:
         """
         Retrieves the acceleration data from the MPU6500 sensor.
 
         Returns:
-            ctypes.Array: An array containing the acceleration data.
+            MPUDataPack: An array containing the acceleration data.
         Notes:
             length = 3
             [0] ==> axis X
             [1] ==> axis Y
             [2] ==> axis Z
         """
         TECHSTAR_LIB.mpu6500_Get_Accel(
             self._accel_all
         )  # this function return a C pointer to the self._accel_all
-        return self._accel_all
+        return tuple(self._accel_all)  # type: ignore
 
-    def gyro_all(self) -> ctypes.Array:
+    def gyro_all(self) -> MPUDataPack:
         """
         Retrieves the gyroscope data from the MPU6500 sensor.
 
         Returns:
-            ctypes.Array: An array containing the gyroscope data.
+            MPUDataPack: An array containing the gyroscope data.
 
         Notes:
             length = 3
             [0] ==> axis X
             [1] ==> axis Y
             [2] ==> axis Z
         """
 
         TECHSTAR_LIB.mpu6500_Get_Gyro(
             self._gyro_all
         )  # this function return a C pointer to the self._gyro_all
 
-        return self._gyro_all
+        return tuple(self._gyro_all)  # type: ignore
 
-    def atti_all(self) -> ctypes.Array:
+    def atti_all(self) -> MPUDataPack:
         """
         Retrieves the attitude data from the MPU6500 sensor.
 
         Returns:
-            ctypes.Array: An array containing the attitude data.
+            MPUDataPack: An array containing the attitude data.
 
         Notes:
             length = 3
             [0] ==> Pitch|axis X
             [1] ==> Roll |axis Y
             [2] ==> Yaw  |axis Z
         """
         TECHSTAR_LIB.mpu6500_Get_Attitude(
             self._atti_all
         )  # this function return a C pointer to the self._atti_all
 
-        return self._atti_all
+        return tuple(self._atti_all)  # type: ignore
 
     @staticmethod
     def get_handle(attr_name: str) -> Any:
         """
         Returns the attribute value of the TECHSTAR_LIB object corresponding to the given attribute name.
         Reserved to the user to harness other attributes of the TECHSTAR_LIB object.
         Args:
```

### Comparing `pyuptech-0.1.4a0/src/pyuptech/tools/display.py` & `pyuptech-0.1.4a1/src/pyuptech/tools/display.py`

 * *Files 6% similar despite different names*

```diff
@@ -130,19 +130,22 @@
     """
     from terminaltables import DoubleTable
 
     adc_labels = adc_labels or {}
     io_labels = io_labels or {}
     adc = sensors.adc_all_channels()
     io = sensors.io_all_channels()
+    io_modes = sensors.get_all_io_mode()
+
     rows = [
-        ["Names"] + ([adc_labels.get(i, f"ADC{i}") for i in range(10)]),
-        ["ADC"] + [f"{x}" for x in adc],
-        ["Names"] + ([io_labels.get(i, f"IO{i}") for i in range(8)]),
-        ["IO"] + [int(bit) for bit in f"{io.value:08b}"],
+        ["ADC Name"] + ([adc_labels.get(i, f"ADC{i}") for i in range(10)]),
+        ["ADC Data"] + [f"{x}" for x in adc],
+        ["IO Name"] + ([io_labels.get(i, f"IO{i}") for i in range(8)]),
+        ["IO Data"] + [int(bit) for bit in f"{io:08b}"],
+        ["IO Mode"] + [int(bit) for bit in f"{io_modes:08b}"],
     ]
     table = DoubleTable(rows)
     table.inner_row_border = True
     print(table.table)
 
 
 def adc_io_display_on_lcd(
@@ -171,15 +174,15 @@
     adc = sensors.adc_all_channels()
     # 打印 ADC 通道值表格
     for i in range(9):
         label = adc_labels.get(i, f"[{i}]")
         value = adc[i]
         screen.put_string(0, i * 8, f"{label}:{value}")
 
-    io = [int(bit) for bit in f"{sensors.io_all_channels().value:08b}"]
+    io = [int(bit) for bit in f"{sensors.io_all_channels():08b}"]
     # 打印 IO 通道值表格
     for i in range(8):
         label = io_labels.get(i, f"[{i}]")
         value = io[i]
         screen.put_string(90, i * 8, f"{label}:{value}")
     screen.fill_screen(Color.BLACK).refresh()
     time.sleep(interval)
```

### Comparing `pyuptech-0.1.4a0/tests/perf_tests.py` & `pyuptech-0.1.4a1/tests/perf_tests.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.4a0/PKG-INFO` & `pyuptech-0.1.4a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuptech
-Version: 0.1.4a0
+Version: 0.1.4a1
 Summary: A Python wrapper for the uptech binary lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: terminaltables>=3.1.10
 Description-Content-Type: text/markdown
```

