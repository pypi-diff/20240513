# Comparing `tmp/pybelt-1.2.2.tar.gz` & `tmp/pybelt-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybelt-1.2.2.tar", last modified: Tue Sep  5 11:41:24 2023, max compression
+gzip compressed data, was "pybelt-1.2.3.tar", last modified: Mon May 13 18:27:59 2024, max compression
```

## Comparing `pybelt-1.2.2.tar` & `pybelt-1.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-09-05 11:41:24.236062 pybelt-1.2.2/
--rw-rw-rw-   0        0        0    11558 2020-11-23 09:55:46.000000 pybelt-1.2.2/LICENSE
--rw-rw-rw-   0        0        0     2133 2023-09-05 11:41:24.232067 pybelt-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1636 2021-01-11 09:49:47.000000 pybelt-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-09-05 11:41:24.211123 pybelt-1.2.2/pybelt/
--rw-rw-rw-   0        0        0      112 2020-06-22 14:06:02.000000 pybelt-1.2.2/pybelt/__init__.py
--rw-rw-rw-   0        0        0    37722 2023-09-05 10:28:58.000000 pybelt-1.2.2/pybelt/_communication_interface.py
--rw-rw-rw-   0        0        0     8833 2023-01-05 13:18:44.000000 pybelt-1.2.2/pybelt/_gatt_profile.py
--rw-rw-rw-   0        0        0    66878 2023-09-05 09:06:36.000000 pybelt-1.2.2/pybelt/belt_controller.py
--rw-rw-rw-   0        0        0     3993 2023-09-04 14:43:56.000000 pybelt-1.2.2/pybelt/belt_scanner.py
--rw-rw-rw-   0        0        0     5529 2023-08-28 08:25:13.000000 pybelt-1.2.2/pybelt/examples_utility.py
--rw-rw-rw-   0        0        0     1033 2023-08-28 08:25:13.000000 pybelt-1.2.2/pybelt/examples_utility_getch.py
-drwxrwxrwx   0        0        0        0 2023-09-05 11:41:24.230072 pybelt-1.2.2/pybelt.egg-info/
--rw-rw-rw-   0        0        0     2133 2023-09-05 11:41:23.000000 pybelt-1.2.2/pybelt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-09-05 11:41:23.000000 pybelt-1.2.2/pybelt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-05 11:41:23.000000 pybelt-1.2.2/pybelt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-09-05 11:41:23.000000 pybelt-1.2.2/pybelt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-09-05 11:41:23.000000 pybelt-1.2.2/pybelt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-09-05 11:41:24.236062 pybelt-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      759 2023-09-05 11:41:04.000000 pybelt-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:27:59.152864 pybelt-1.2.3/
+-rw-rw-rw-   0        0        0    11558 2020-11-23 09:55:46.000000 pybelt-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0     2133 2024-05-13 18:27:59.151866 pybelt-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1636 2021-01-11 09:49:47.000000 pybelt-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 18:27:59.142358 pybelt-1.2.3/pybelt/
+-rw-rw-rw-   0        0        0      112 2020-06-22 14:06:02.000000 pybelt-1.2.3/pybelt/__init__.py
+-rw-rw-rw-   0        0        0    38508 2024-04-15 13:51:12.000000 pybelt-1.2.3/pybelt/_communication_interface.py
+-rw-rw-rw-   0        0        0     8833 2023-01-05 13:18:44.000000 pybelt-1.2.3/pybelt/_gatt_profile.py
+-rw-rw-rw-   0        0        0    67139 2024-04-18 13:10:56.000000 pybelt-1.2.3/pybelt/belt_controller.py
+-rw-rw-rw-   0        0        0     3993 2023-09-04 14:43:56.000000 pybelt-1.2.3/pybelt/belt_scanner.py
+-rw-rw-rw-   0        0        0     5542 2024-04-22 10:24:14.000000 pybelt-1.2.3/pybelt/examples_utility.py
+-rw-rw-rw-   0        0        0     1033 2023-08-28 08:25:13.000000 pybelt-1.2.3/pybelt/examples_utility_getch.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:27:59.150864 pybelt-1.2.3/pybelt.egg-info/
+-rw-rw-rw-   0        0        0     2133 2024-05-13 18:27:59.000000 pybelt-1.2.3/pybelt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2024-05-13 18:27:59.000000 pybelt-1.2.3/pybelt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 18:27:59.000000 pybelt-1.2.3/pybelt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-13 18:27:59.000000 pybelt-1.2.3/pybelt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-13 18:27:59.000000 pybelt-1.2.3/pybelt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 18:27:59.152864 pybelt-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      759 2024-05-13 18:27:45.000000 pybelt-1.2.3/setup.py
```

### Comparing `pybelt-1.2.2/LICENSE` & `pybelt-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pybelt-1.2.2/PKG-INFO` & `pybelt-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybelt
-Version: 1.2.2
+Version: 1.2.3
 Summary: An Python library to control the feelSpace naviBelt from your application
 Home-page: https://github.com/feelSpace/pybelt
 Author: feelSpace GmbH
 Author-email: dev@feelspace.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pybelt-1.2.2/README.md` & `pybelt-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pybelt-1.2.2/pybelt/_communication_interface.py` & `pybelt-1.2.3/pybelt/_communication_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,20 +125,21 @@
         """
         Returns the connection state.
 
         :return: 'True' if the belt is connected.
         """
         pass
 
-    def write_gatt_char(self, gatt_char, data) -> bool:
+    def write_gatt_char(self, gatt_char, data, with_response=True) -> bool:
         """
         Writes a GATT attribute.
 
         :param GattCharacteristic gatt_char:  The characteristic to write.
         :param bytes data: The data to write.
+        :param bool with_response: 'True' for write with response, 'False' for write without response.
         :return: 'True' if successful, 'False' if not connected or a problem occurs.
         """
         pass
 
     def set_gatt_notifications(self, gatt_char, enabled) -> bool:
         """
         Enables or disables the notifications for a characteristic.
@@ -161,14 +162,20 @@
     def get_gatt_profile(self) -> NaviBeltGattProfile:
         """
         Returns the GATT profile with characteristics.
         :return: the GATT profile with characteristics.
         """
         pass
 
+    def get_max_packet_size(self) -> int:
+        """
+        Returns the maximum size for data packets.
+        :return: the maximum size for packets.
+        """
+
 
 class SerialPortInterface(threading.Thread, BeltCommunicationInterface):
     """Serial port interface.
     """
 
     # --------------------------------------------------------------- #
     # Public methods
@@ -304,21 +311,23 @@
         self.join(timeout)
         self._expect_disconnection = False
         return self.is_connected()
 
     def is_connected(self) -> bool:
         return self._serial_port is not None
 
-    def write_gatt_char(self, gatt_char, data) -> bool:
+    def write_gatt_char(self, gatt_char, data, with_response=True) -> bool:
         self._wait_empty_buffer()
         with self._serial_port_lock:
             try:
-                # TODO TBR
-                # print("Serial: in buff. {}, out buff. {}".format(self._serial_port.in_waiting, self._serial_port.out_waiting))
-                packet = bytes([gatt_char.value_attr.handle]) + bytes([len(data)]) + data
+                if len(data) >= 255:
+                    # Allow packets larger than 255 bytes (only for supported characteristics)
+                    packet = bytes([gatt_char.value_attr.handle]) + b'\xff' + data
+                else:
+                    packet = bytes([gatt_char.value_attr.handle]) + bytes([len(data)]) + data
                 self._serial_port.write(packet)
             except:
                 return False
         return True
 
     def set_gatt_notifications(self, gatt_char, enabled) -> bool:
         self._wait_empty_buffer()
@@ -351,14 +360,17 @@
             except:
                 return False
         return True
 
     def get_gatt_profile(self) -> NaviBeltGattProfile:
         return self._gatt_profile
 
+    def get_max_packet_size(self) -> int:
+        return 1024
+
     # --------------------------------------------------------------- #
     # Implementation of Thread methods
 
     def run(self):
         self.stop_flag = False
         self._expect_disconnection = False
         self.logger.debug("SerialPortListener: Start listening belt.")
@@ -603,29 +615,30 @@
                 else:
                     self.logger.debug("BleInterface: Client already disconnected.")
         except:
             self.logger.exception("BleInterface: Error when disconnecting!")
             success = False
         return success
 
-    async def _write_gatt_char(self, gatt_char, data) -> bool:
+    async def _write_gatt_char(self, gatt_char, data, with_response=True) -> bool:
         """
         Writes a GATT characteristic.
         :param GattCharacteristic gatt_char: The characteristic to write.
         :param bytes data: The data to write.
+        :param bool with_response: 'True' to write with response, 'False' to write without response.
         :return: 'True' if successful, 'False' otherwise.
         """
         try:
             if self._gatt_client is None:
                 self.logger.warning("BleInterface: No connection to write char!")
                 return False
             if not self._gatt_client.is_connected:
                 self.logger.warning("BleInterface: No connection to set notifications!")
                 return False
-            await self._gatt_client.write_gatt_char(gatt_char.uuid, bytearray(data), response=True)
+            await self._gatt_client.write_gatt_char(gatt_char.uuid, bytearray(data), response=with_response)
         except:
             self.logger.exception("BleInterface: Error when writing characteristic.")
             return False
         return True
 
     async def _set_gatt_notifications(self, gatt_char, enabled) -> bool:
         """
@@ -787,20 +800,21 @@
         self._event_notifier.join(timeout)
         self._expect_disconnection = False
         return self.is_connected()
 
     def is_connected(self) -> bool:
         return self._gatt_client is not None
 
-    def write_gatt_char(self, gatt_char, data) -> bool:
+    def write_gatt_char(self, gatt_char, data, with_response=True) -> bool:
         if self._gatt_client is None:
             self.logger.error("BleInterface: No connection to write char!")
             return False
         try:
-            future = asyncio.run_coroutine_threadsafe(self._write_gatt_char(gatt_char, data), self._event_loop)
+            future = asyncio.run_coroutine_threadsafe(self._write_gatt_char(gatt_char, data, with_response),
+                                                      self._event_loop)
             success = future.result()
             if not success:
                 self.logger.error("BleInterface: Failed to write char!")
                 return False
         except:
             self.logger.exception("BleInterface: Error when scheduling write char operation!")
             return False
@@ -837,14 +851,17 @@
             self.logger.exception("BleInterface: Error when scheduling read char operation!")
             return False
         return True
 
     def get_gatt_profile(self) -> NaviBeltGattProfile:
         return self._gatt_profile
 
+    def get_max_packet_size(self) -> int:
+        return 244 # 244 bytes using GATT with DLE
+
     # --------------------------------------------------------------- #
     # Implementation of Thread methods
 
     def run(self):
         try:
             # Create loop
             self._event_loop = asyncio.new_event_loop()
```

### Comparing `pybelt-1.2.2/pybelt/_gatt_profile.py` & `pybelt-1.2.3/pybelt/_gatt_profile.py`

 * *Files identical despite different names*

### Comparing `pybelt-1.2.2/pybelt/belt_controller.py` & `pybelt-1.2.3/pybelt/belt_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,23 +212,25 @@
             write_result = self.write_gatt(
                 self._gatt_profile.param_request_char,
                 bytes([0x01, 0x82, intensity, 0x00, (0x01 if vibration_feedback else 0x00)]))
         if write_result == 2:
             raise TimeoutError("Timeout period reached when changing the belt mode.")
         return write_result == 0
 
-    def write_gatt(self, gatt_char, data, ack_char=None, ack_data=None, timeout_sec=WAIT_ACK_TIMEOUT_SEC) -> int:
+    def write_gatt(self, gatt_char, data, ack_char=None, ack_data=None, timeout_sec=WAIT_ACK_TIMEOUT_SEC,
+                   with_response=True) -> int:
         """
         Sends data to a GATT characteristic.
 
         :param GattCharacteristic gatt_char: The characteristic to write.
         :param bytes data: The data to write.
         :param GattCharacteristic ack_char: The characteristic for which an acknowledgment should be waited.
         :param bytes ack_data: The acknowledgment pattern.
         :param float timeout_sec: The timeout period in seconds.
+        :param bool with_response: 'True' to write with response, 'False' to write without response.
         :return: Returns '0' if successful, '1' when no connection is available or a problem occurs, '2' when the
         timeout is reached.
         """
         if (self._connection_state == BeltConnectionState.DISCONNECTED or
                 self._connection_state == BeltConnectionState.DISCONNECTING):
             self.logger.error("BeltController: No connection to send packet.")
             return 1
@@ -239,15 +241,15 @@
             self._ack_event.clear()
         # Send packet
         try:
             self.logger.log(5, "BeltController: " + gatt_char.uuid[4:8] + " -> " + bytes_to_hexstr(data))
         except:
             pass
         try:
-            if not self._communication_interface.write_gatt_char(gatt_char, data):
+            if not self._communication_interface.write_gatt_char(gatt_char, data, with_response=with_response):
                 self.logger.error("BeltController: Error when sending packet.")
                 self._ack_char = None
                 self._ack_data = None
                 self._ack_event.clear()
                 return 1
         except:
             self.logger.exception("BeltController: Error when sending packet.")
@@ -938,15 +940,15 @@
 
         :param int belt_mode:
             The belt mode to set.
         """
         if (self._connection_state == BeltConnectionState.DISCONNECTED or
                 self._connection_state == BeltConnectionState.DISCONNECTING):
             return
-        if belt_mode < 0 or belt_mode > 8:
+        if belt_mode < 0 or belt_mode > 10:
             self.logger.error("BeltController: Illegal belt mode.")
             return
         if belt_mode == self._belt_mode:
             return
         self._belt_mode = belt_mode
         if self._connection_state == BeltConnectionState.CONNECTING:
             # No delegate notification during handshake
@@ -1328,14 +1330,15 @@
         #     eol = self._debug_message_buffer.find('\n')
 
         # TODO Other notifications
 
         # Check for ACK
         if (self._ack_data is not None or self._ack_char is not None) and not self._ack_event.is_set():
             if self._is_ack(gatt_char, data):
+                self.logger.log(5, "BeltController: Ack data received 0x"+data.hex())
                 self._ack_data = None
                 self._ack_char = None
                 self._ack_event.set()
 
         # Inform system handlers
         for handler in self._notifications_handlers:
             try:
@@ -1378,14 +1381,15 @@
     COMPASS = 2
     APP_MODE = 3
     PAUSE = 4
     CALIBRATION = 5
     CROSSING = 6
 
 
+
 class BeltOrientationType:
     """Enumeration of orientation types."""
 
     BINARY_MASK = 0
     MOTOR_INDEX = 1
     ANGLE = 2
     MAGNETIC_BEARING = 3
```

### Comparing `pybelt-1.2.2/pybelt/belt_scanner.py` & `pybelt-1.2.3/pybelt/belt_scanner.py`

 * *Files identical despite different names*

### Comparing `pybelt-1.2.2/pybelt/examples_utility.py` & `pybelt-1.2.3/pybelt/examples_utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 def belt_controller_log_to_stdout():
     """Configures the belt-controller logger to print all debug messages on `stdout`.
     """
     logger = pybelt.logger
     logger.setLevel(logging.DEBUG)
     sh = logging.StreamHandler(sys.stdout)
-    sh_format = logging.Formatter('\033[92m %(levelname)s: %(message)s \033[0m')
+    sh_format = logging.Formatter('\033[92m %(levelname)s, %(asctime)s: %(message)s \033[0m')
     sh.setFormatter(sh_format)
     sh.setLevel(logging.DEBUG)
     logger.addHandler(sh)
 
 
 def interactive_belt_connection(belt_controller):
     """Procedures to connect a belt using the terminal.
```

### Comparing `pybelt-1.2.2/pybelt/examples_utility_getch.py` & `pybelt-1.2.3/pybelt/examples_utility_getch.py`

 * *Files identical despite different names*

### Comparing `pybelt-1.2.2/pybelt.egg-info/PKG-INFO` & `pybelt-1.2.3/pybelt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybelt
-Version: 1.2.2
+Version: 1.2.3
 Summary: An Python library to control the feelSpace naviBelt from your application
 Home-page: https://github.com/feelSpace/pybelt
 Author: feelSpace GmbH
 Author-email: dev@feelspace.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pybelt-1.2.2/setup.py` & `pybelt-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pybelt",
-    version="1.2.2",
+    version="1.2.3",
     author="feelSpace GmbH",
     author_email="dev@feelspace.de",
     description="An Python library to control the feelSpace naviBelt from your application",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/feelSpace/pybelt",
     packages=setuptools.find_packages(),
```

