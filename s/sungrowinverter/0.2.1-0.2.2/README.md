# Comparing `tmp/sungrowinverter-0.2.1.tar.gz` & `tmp/sungrowinverter-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sungrowinverter-0.2.1.tar", max compression
+gzip compressed data, was "sungrowinverter-0.2.2.tar", max compression
```

## Comparing `sungrowinverter-0.2.1.tar` & `sungrowinverter-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      765 2022-12-12 08:25:28.519078 sungrowinverter-0.2.1/LICENSE
--rw-r--r--   0        0        0     5150 2022-12-12 08:26:00.743067 sungrowinverter-0.2.1/README.md
--rwxr-xr-x   0        0        0      971 2023-03-26 03:04:52.189413 sungrowinverter-0.2.1/pyproject.toml
--rwxr-xr-x   0        0        0    15626 2023-03-26 01:58:44.702828 sungrowinverter-0.2.1/sungrowinverter/SungrowInverter.py
--rw-r--r--   0        0        0     3950 2022-12-12 07:49:36.609548 sungrowinverter-0.2.1/sungrowinverter/SungrowModbusTCPClient.py
--rwxr-xr-x   0        0        0      126 2022-12-12 08:16:15.915983 sungrowinverter-0.2.1/sungrowinverter/__init__.py
--rw-r--r--   0        0        0       44 2022-12-12 08:16:24.896755 sungrowinverter-0.2.1/sungrowinverter/configs/__init.__.py
--rw-r--r--   0        0        0     3026 2022-12-12 08:17:18.584574 sungrowinverter-0.2.1/sungrowinverter/configs/common.py
--rw-r--r--   0        0        0     8015 2023-03-22 08:55:09.765598 sungrowinverter-0.2.1/sungrowinverter/configs/hybrid.py
--rw-r--r--   0        0        0     5496 2023-03-22 08:56:40.657353 sungrowinverter-0.2.1/sungrowinverter/configs/inverter.py
--rw-r--r--   0        0        0    10232 2022-12-12 08:26:34.207482 sungrowinverter-0.2.1/sungrowinverter/configs/string.py
--rw-r--r--   0        0        0     6376 1970-01-01 00:00:00.000000 sungrowinverter-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      765 2022-12-12 08:25:28.519078 sungrowinverter-0.2.2/LICENSE
+-rw-r--r--   0        0        0      971 2024-05-13 15:20:00.102039 sungrowinverter-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6141 2024-05-13 15:11:12.460601 sungrowinverter-0.2.2/README.md
+-rw-r--r--   0        0        0      126 2022-12-12 08:16:15.915983 sungrowinverter-0.2.2/sungrowinverter/__init__.py
+-rw-r--r--   0        0        0       44 2022-12-12 08:16:24.896755 sungrowinverter-0.2.2/sungrowinverter/configs/__init.__.py
+-rw-r--r--   0        0        0     3026 2022-12-12 08:17:18.584574 sungrowinverter-0.2.2/sungrowinverter/configs/common.py
+-rw-r--r--   0        0        0     8230 2024-05-13 15:11:12.460601 sungrowinverter-0.2.2/sungrowinverter/configs/hybrid.py
+-rw-r--r--   0        0        0     5850 2024-05-13 15:11:12.461602 sungrowinverter-0.2.2/sungrowinverter/configs/inverter.py
+-rw-r--r--   0        0        0    10232 2022-12-12 08:26:34.207482 sungrowinverter-0.2.2/sungrowinverter/configs/string.py
+-rw-r--r--   0        0        0    15963 2024-05-13 15:11:12.460601 sungrowinverter-0.2.2/sungrowinverter/SungrowInverter.py
+-rw-r--r--   0        0        0     3950 2022-12-12 07:49:36.609548 sungrowinverter-0.2.2/sungrowinverter/SungrowModbusTCPClient.py
+-rw-r--r--   0        0        0     7228 1970-01-01 00:00:00.000000 sungrowinverter-0.2.2/PKG-INFO
```

### Comparing `sungrowinverter-0.2.1/LICENSE` & `sungrowinverter-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sungrowinverter-0.2.1/README.md` & `sungrowinverter-0.2.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,133 +1,139 @@
-# SungrowInverter
-
-Provides a way to query Sungrow residential hybrid or string inverters for current state and statistics using ModBus TCP client.
-
-Currently does not support any writing to holding registers.
-
-## Supported Residental Inverters
-
-### Hybrid/Storage Inverters - inverter that support a battery
-
-Residential Hybrid Single Phase Inverter for Low Voltage Battery [48V to 70V]
-
-SH3K6 / SH4K6 / SH5K-V13 (SH5K) / SH5K-20 / SH4K6-30 / SH5K-30 / SH3K6-30
-
-Residential Hybrid Single Phase Inverter wide battery voltage range [80V to 460V]
-
-SH3.6RS / SH4.6RS / SH5.0RS / SH6.0RS
-
-Residential Hybrid Three Phase Inverter wide battery voltage range [80V to 460V]
-
-SH5.0RT / SH6.0RT / SH8.0RT / SH10RT
-
-### String Inverters - Solar panel and grid connection only
-
-SG3.0RT, SG4.0RT, SG5.0RT, SG6.0RT, SG7.0RT，SG8.0RT, SG10RT, SG12RT, SG15RT, SG17RT, SG20RT
-SG30KTL-M, SG30KTL-M-V31, SG33KTL-M, SG36KTL-M, SG33K3J, SG49K5J, SG34KJ, LP_P34KSG,
-SG50KTL-M-20, SG60KTL, G80KTL, SG80KTL-20, SG60KU-M
-SG5KTL-MT, SG6KTL-MT, SG8KTL-M, SG10KTL-M, SG10KTL-MT, SG12KTL-M, SG15KTL-M,
-SG17KTL-M, SG20KTL-M,
-SG80KTL-M, SG85BF, SG80HV, SG80BF, SG110HV-M, SG111HV, SG125HV, SG125HV-20
-SG25CX-SA, SG30CX, SG33CX, SG40CX, SG50CX, SG36CX-US, SG60CX-US, SG75CX, SG100CX
-SG100CX-JP, SG110CX, SG136TX, SG225HX, SG250HX
-SG250HX-IN, SG250HX-US
-
-Discontinued (as @ 2021-07-12):
-
-SG30KTL, SG10KTL, SG12KTL, SG15KTL, SG20KTL, SG30KU, SG36KTL, SG36KU, SG40KTL,
-SG40KTL-M, SG50KTL-M, SG60KTL-M, SG60KU
-
-
-## Usage
-
-If not called from within an async method
-
-```python
-from sungrowinverter inport SungrowInverter
-import asyncio
-...
-
-client = SungrowInverter("192.168.1.27")
-
-loop = asyncio.new_event_loop()
-asyncio.set_event_loop(loop)
-result = loop.run_until_complete(client.async_update())
-
-#Get a list data returned from the inverter.
-print(client.data)
-```
-
-If called within an async method in your application
-```
-from sungrowinverter inport SungrowInverter
-
-client = SungrowInverter("192.168.1.27")
-client.async_update()
-
-#Get a list data returned from the inverter.
-print(client.model)
-print(client.data)
-```
-
-** of course change 192.168.1.127 to your inverter's ip address.
-
-## Methods and Variables
-
-### Contructor
-
-`SungrowInverter(ip_address, port=502, slave=0x01, retries3, timeout=60)`
-
-port: modbus TCP port defaults to 502 on sungrow inverters used here
-
-slave: defaulted to 0x01 as per specs your inverter may need to change this.
-
-retries: number of attempts to query the registers on the inverter before failing
-
-timeout: <in seconds> tcp connection is timed out and fails after this long
-
-### Methods
-
-Available methods
-
-`client.inverter_model()` Returns a object of sungrowinverter.common.SungrowInverterModel with details of model, serial, nominal output power (kWh)
-
-`client.async_update()` Calls set of registers for the relevant inverter and updates data parameter
-  
-### Parameters Available
-
-#### All inverters
-  
-  `model:` Provides device model (ie. SH5K - as found in current models supported above)
-
-  `device_code:` Sungrow device code found at register 5000 (refer docs for actual codes if needed)
-
-  `serial_number:` Serial number of the inverter
-
-  `nominal_output_power:` The output power that the inverter supports (ie. SH5K is a 5 kWh inverter and will contain 5.0 in this parameter)
-
-  `inverter_type:` [hybrid | string] - type of sungrow inverter that the client is communicating with, hybrid (battery supported inverter SHxxx series or standard inverter SGxxxx series)
-
-  `mppt_input:` The number of mppt inputs the inverter supports, refer notes below.
-
-  `data:` Provides a dictionary of data of all registers queried (key = register name, value = register value) refer to the https://github.com/mvandersteen/SungrowInverter/tree/main/sungrowinverter/configs for details on what registers are exposed.
-
-#### Hybrid (storage) inverters only
-  
-  `battery_type:` Show the battery type configured for the inverter
-
-  `battery_energy_capacity:` hybrid only, this will show the capacity of the battery configured for the inverter
-  
-  
-## Note
-
-```
-client = SungrowInverter("192.168.1.27")
-await client.async_update()
-```
-  `client.data['export_power']` - for this register it is a signed value if positive then the inverter is exporting to the grid, if negative then it is importing from the grid.
-
-  `client.mppt_inputs` - this value dictates how many client.data['mppt_xx_voltage'] & client.data['mppt_xx_current'] registers are available. These values have been obtained from the modbus specs found in the documents directory on this repository. If an inverter only supports 1 mppt connection then only 1 set of mppt_1_voltage and mppt_1_current will appear. If the inverter supports more then mppt\_\[xx\]\_voltage & mppt\_\[xx\]\_current; where [xx] = the number of mppt inputs the inverter supports; the number available depends on the how many the inverter supports can be 1 to 12 sets of data for current set of support inverters. 
-  
-## Python Version prior to 3.9
-
-Refer to https://github.com/mvandersteen/SungrowInverter/issues/2 if you are having issues, where @hallonstedt explains how to resolve for a prior version of python.
+# SungrowInverter
+
+Provides a way to query Sungrow residential hybrid or string inverters for current state and statistics using ModBus TCP client.
+
+Currently does not support any writing to holding registers.
+
+## Supported Residental Inverters
+
+### Hybrid/Storage Inverters - inverter that support a battery
+
+Residential Hybrid Single Phase Inverter for Low Voltage Battery [48V to 70V]
+
+SH3K6 / SH4K6 / SH5K-V13 (SH5K) / SH5K-20 / SH4K6-30 / SH5K-30 / SH3K6-30
+
+Residential Hybrid Single Phase Inverter wide battery voltage range [80V to 460V]
+
+SH3.6RS / SH4.6RS / SH5.0RS / SH6.0RS
+
+Residential Hybrid Three Phase Inverter wide battery voltage range [80V to 460V]
+
+SH5.0RT / SH6.0RT / SH8.0RT / SH10RT
+
+### String Inverters - Solar panel and grid connection only
+
+SG3.0RT, SG4.0RT, SG5.0RT, SG6.0RT, SG7.0RT，SG8.0RT, SG10RT, SG12RT, SG15RT, SG17RT, SG20RT
+SG30KTL-M, SG30KTL-M-V31, SG33KTL-M, SG36KTL-M, SG33K3J, SG49K5J, SG34KJ, LP_P34KSG,
+SG50KTL-M-20, SG60KTL, G80KTL, SG80KTL-20, SG60KU-M
+SG5KTL-MT, SG6KTL-MT, SG8KTL-M, SG10KTL-M, SG10KTL-MT, SG12KTL-M, SG15KTL-M,
+SG17KTL-M, SG20KTL-M,
+SG80KTL-M, SG85BF, SG80HV, SG80BF, SG110HV-M, SG111HV, SG125HV, SG125HV-20
+SG25CX-SA, SG30CX, SG33CX, SG40CX, SG50CX, SG36CX-US, SG60CX-US, SG75CX, SG100CX
+SG100CX-JP, SG110CX, SG136TX, SG225HX, SG250HX
+SG250HX-IN, SG250HX-US
+
+Discontinued (as @ 2021-07-12):
+
+SG30KTL, SG10KTL, SG12KTL, SG15KTL, SG20KTL, SG30KU, SG36KTL, SG36KU, SG40KTL,
+SG40KTL-M, SG50KTL-M, SG60KTL-M, SG60KU
+
+
+## Usage
+
+If not called from within an async method
+
+```python
+from sungrowinverter inport SungrowInverter
+import asyncio
+...
+
+client = SungrowInverter("192.168.1.27")
+
+loop = asyncio.new_event_loop()
+asyncio.set_event_loop(loop)
+result = loop.run_until_complete(client.async_update())
+
+#Get a list data returned from the inverter.
+print(client.data)
+```
+
+If called within an async method in your application
+```
+from sungrowinverter inport SungrowInverter
+
+client = SungrowInverter("192.168.1.27")
+client.async_update()
+
+#Get a list data returned from the inverter.
+print(client.model)
+print(client.data)
+```
+
+** of course change 192.168.1.127 to your inverter's ip address.
+
+## Methods and Variables
+
+### Contructor
+
+`SungrowInverter(ip_address, port=502, slave=0x01, retries3, timeout=60)`
+
+port: modbus TCP port defaults to 502 on sungrow inverters used here
+
+slave: defaulted to 0x01 as per specs your inverter may need to change this.
+
+retries: number of attempts to query the registers on the inverter before failing
+
+timeout: <in seconds> tcp connection is timed out and fails after this long
+
+### Methods
+
+Available methods
+
+`client.inverter_model()` Returns a object of sungrowinverter.common.SungrowInverterModel with details of model, serial, nominal output power (kWh)
+
+`client.async_update()` Calls set of registers for the relevant inverter and updates data parameter
+  
+### Parameters Available
+
+#### All inverters
+  
+  `model:` Provides device model (ie. SH5K - as found in current models supported above)
+
+  `device_code:` Sungrow device code found at register 5000 (refer docs for actual codes if needed)
+
+  `serial_number:` Serial number of the inverter
+
+  `nominal_output_power:` The output power that the inverter supports (ie. SH5K is a 5 kWh inverter and will contain 5.0 in this parameter)
+
+  `inverter_type:` [hybrid | string] - type of sungrow inverter that the client is communicating with, hybrid (battery supported inverter SHxxx series or standard inverter SGxxxx series)
+
+  `mppt_input:` The number of mppt inputs the inverter supports, refer notes below.
+
+  `data:` Provides a dictionary of data of all registers queried (key = register name, value = register value) refer to the https://github.com/mvandersteen/SungrowInverter/tree/main/sungrowinverter/configs for details on what registers are exposed.
+
+#### Hybrid (storage) inverters only
+  
+  `battery_type:` Show the battery type configured for the inverter
+
+  `battery_energy_capacity:` hybrid only, this will show the capacity of the battery configured for the inverter
+  
+  
+## Note
+
+```
+client = SungrowInverter("192.168.1.27")
+await client.async_update()
+```
+  `client.data['export_power']` - for this register it is a signed value if positive then the inverter is exporting to the grid, if negative then it is importing from the grid.
+
+  `client.mppt_inputs` - this value dictates how many client.data['mppt_xx_voltage'] & client.data['mppt_xx_current'] registers are available. These values have been obtained from the modbus specs found in the documents directory on this repository. If an inverter only supports 1 mppt connection then only 1 set of mppt_1_voltage and mppt_1_current will appear. If the inverter supports more then mppt\_\[xx\]\_voltage & mppt\_\[xx\]\_current; where [xx] = the number of mppt inputs the inverter supports; the number available depends on the how many the inverter supports can be 1 to 12 sets of data for current set of support inverters. 
+  
+## Python Version prior to 3.9
+
+Refer to https://github.com/mvandersteen/SungrowInverter/issues/2 if you are having issues, where @hallonstedt explains how to resolve for a prior version of python.
+
+
+## Note
+2024-05-13: I don't have a sungrow invester to test changes on any longer as house is being rebuilt, will look to update again once new build is complete and solar re-added. For now apologies will not be muc help to anyone other than accepting merge every now and then, i don't get on here much any longer.
+
+If you have an inverter not supported by this module BUT do get a response back from the sungrow inverter with a device ID, then you could follow what was done for this pull request https://github.com/mvandersteen/SungrowInverter/commit/9bef6dfcc4db7672edb1140b98bbdd34c672a987 by @ortogonal that is add an entry for your inverter in the inverter list and also if you have a 3 phase inverter (usually denoted by RT) add your inverter number into the list of support inverter for the relevant parameter data pulled from the inverter.
```

### Comparing `sungrowinverter-0.2.1/pyproject.toml` & `sungrowinverter-0.2.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sungrowinverter"
-version = "0.2.1"
+version = "0.2.2"
 description = "Query Sungrow residential hybrid or string inverters for current state and statistics using ModBus TCP client"
 authors = ["Mark Vandersteen <mark@vandersteen.me>"]
 license = "GNU General Public License"
 readme = "README.md"
 repository = "https://github.com/mvandersteen/SungrowInverter"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `sungrowinverter-0.2.1/sungrowinverter/SungrowInverter.py` & `sungrowinverter-0.2.2/sungrowinverter/SungrowInverter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,347 +1,347 @@
-"""
-
-Sungrow Inverter register reader
-
-Connect to a Sungrow modbus via TCP
-
-Supports Sungrow Hybrid & String inverters
-
-Refer configs/hybrid.py and configs/string.py for inverters that are supported.
-"""
-
-__version__ = "0.2.1"
-
-from sungrowinverter.SungrowModbusTCPClient import SungrowModbusTcpClient
-from sungrowinverter.configs.inverter import (
-    INVERTER_SCAN,
-    INVERTER_READ_REGISTERS,
-    INVERTER_HOLDING_REGISTERS,
-    INVERTER_MODELS,
-)
-
-from sungrowinverter.configs.common import SungrowInverterModel
-
-from sungrowinverter.configs.hybrid import (
-    HYBRID_SCAN,
-    HYBRID_READ_REGISTERS,
-    HYBRID_HOLDING_REGISTERS,
-    HYBRID_CALCULATED_REGISTERS,
-)
-from sungrowinverter.configs.string import (
-    STRING_SCAN,
-    STRING_READ_REGISTERS,
-    STRING_HOLDING_REGISTERS,
-)
-
-import logging
-
-REQUESTS_TIMEOUT = 60
-
-
-class SungrowInverter:
-    """
-    SungrowInverter module for read modbus data from tcp connect to Sungrow inverters (hybrid / string) inverters supported
-    """
-
-    def __init__(self, ip_address, port=502, slave=1, retries=3, timeout=REQUESTS_TIMEOUT):
-        """Initialize a Sungrow Inverter TCP Modbus Client object"""
-        self.manufacturer = "Sungrow"
-
-        # Set when invert_model is run
-        self.model = None
-        self.device_code = None
-        self.mppt_inputs = 0
-        self.serial_number = None
-        self.nominal_output_power = None
-        self.inverter_type = None
-
-        self.battery_type = None
-        self.battery_energy_capacity = None
-
-        self._modbusclient = None
-        self._slave = slave
-        self._timeout = timeout
-
-        self.data = {}
-
-        client_payload = {
-            "host": ip_address,
-            "port": port,
-            "timeout": timeout,
-            "retries": retries,
-            "retry_on_empty": True,
-        }
-
-        self._modbusclient = SungrowModbusTcpClient(**client_payload)
-
-        logging.debug("Sungrow modbus TCP client - [IP:%s Port:%s]", ip_address, port)
-
-    async def _load_registers(self, register_type, start, modbus_registers, count=100):
-        try:
-            if register_type == "read":
-                response = self._modbusclient.read_input_registers(int(start), count=count, slave=self._slave)
-            elif register_type == "holding":
-                response = self._modbusclient.read_holding_registers(int(start), count=count, slave=self._slave)
-            else:
-                logging.error("Unsupported register type: %s", register_type)
-
-        except Exception as err:
-            logging.warning("No data. Try increasing the timeout or scan interval: %s", err, exc_info=1)
-            return False
-
-        if response.isError():
-            logging.warning("Modbus connection failed, connection could not be made or register range failed to be read.")
-            return False
-
-        if not hasattr(response, "registers"):
-            logging.warning("No registers returned")
-            return
-
-        if len(response.registers) != count:
-            logging.warning("Mismatched number of registers read %s != %s", len(response.registers), count)
-            return
-
-        logging.debug("Registers: %s [start_register: %s, register_count: %s] contents: %s", register_type, int(start) + 1, count, response.registers)
-
-        for current_register in modbus_registers:
-
-            if (start + 1) <= current_register.address < (start + 1 + count):
-
-                if not next((x for x in modbus_registers if x.address == current_register.address), None,) is None:
-
-                    try:
-
-                        if not current_register.valid_inverters is None:
-                            if not self.device_code in current_register.valid_inverters:
-                                continue
-
-                        # We want to make sure we only add the neccessary mppt entries we dont need to create data
-                        # if the inverter don't support it (most have 2, others 1, 3 or more)
-                        if current_register.key.startswith("mppt_"):
-                            mppt_key = current_register.key.split("_")
-                            if int(mppt_key[1]) > self.mppt_inputs:
-                                continue
-
-                        register_index = current_register.address - (start + 1)
-
-                        if current_register.data_type == "U16":
-                            value = response.registers[register_index]
-
-                        elif current_register.data_type == "U32":
-                            value = (response.registers[register_index + 1] << 16) + response.registers[register_index]
-
-                        elif current_register.data_type == "S16":
-                            value = int.from_bytes(response.registers[register_index].to_bytes(2, "little"), "little", signed=True)
-
-                        elif current_register.data_type == "S32":
-                            value = int.from_bytes(((response.registers[register_index + 1] << 16) + response.registers[register_index]).to_bytes(4, "little"), "little", signed=True)
-
-                        elif current_register.data_type == "UTF8":
-                            value = await self._get_utf8(response.registers, register_index, current_register.length)
-
-                        else:
-                            logging.debug("Unknown data_type used for register %s [register: %s data_type: %s]",
-                                            current_register.key, current_register.address, current_register.data_type)
-
-                        if current_register.unit_precision is not None:
-                            value = round(value * current_register.unit_precision, 1)
-
-                        if current_register.table is not None:
-
-                            # if we need to decode a returned value into a set of binary information
-                            # table hold binary map
-                            # value here will contain the bits to translate against the binary map
-                            if current_register.transform == "BINARY":
-                                # we will set each bit into a value ie. whether something is on or off usually.
-                                binary_map = current_register.table
-                                bit_val = 1
-                                while bit_val < 2 ** int(current_register.length):
-                                    if bit_val in binary_map:
-                                        if value & bit_val == bit_val:
-                                            self.data[binary_map[bit_val]] = True
-                                        else:
-                                            self.data[binary_map[bit_val]] = False
-                                    bit_val = bit_val << 1
-                            else:
-                                #if value in current_register.table:
-                                self.data[current_register.key] = current_register.table[value]
-
-                        else:
-                            self.data[current_register.key] = value
-                    
-                    except Exception as err:
-                        exp = err
-
-        return True
-
-    async def _get_utf8(self, registers, index, length):
-
-        buff = b""
-        for byte in range(index, length):
-            buff += bytes(int(registers[byte]).to_bytes(2, byteorder="big"))
-
-        if bytes(buff).find(b"\0", 0):
-            end = bytes(buff).find(b"\0")
-            if end != -1:
-                return bytes(buff)[0:end].decode("utf-8")
-
-        return ""
-
-    async def inverter_model(self) -> SungrowInverterModel:
-        """Connect to the inverter and scrape the inverter model and serial data"""
-
-        # if first time run then get the model details and load the relevant modmap for the model for future requests
-        # if we fail to connect then do nothing and exit
-        if self.model is None:
-
-            connection = self._modbusclient.connect()
-
-            if connection:
-                # load the inverter registers to get static data, and determine if model found is supported.
-                for scan_type in INVERTER_SCAN["read"]:
-                    if not await self._load_registers("read", scan_type["scan_start"], INVERTER_READ_REGISTERS, scan_type["scan_range"]):
-                        return False
-
-                self._modbusclient.close()
-
-                if "device_type_code" in self.data:
-                    inverter_model = next((x for x in INVERTER_MODELS if x.device_code == self.data["device_type_code"]), None,)
-
-                    if inverter_model is not None:
-                        self.model = inverter_model.model
-                        self.data["model"] = inverter_model.model
-                        self.inverter_type = inverter_model.inverter_type
-                        self.mppt_inputs = inverter_model.mppt_inputs
-                        self.serial_number = self.data["serial_number"]
-                        self.nominal_output_power = f"{self.data['nominal_output_power']} kW"
-                        inverter_model.nominal_output_power = self.nominal_output_power
-                        inverter_model.serial_number = self.serial_number
-                        self.device_code = self.data['device_type_code']
-
-                        logging.info(
-                            "Sungrow residential inverter found: [Device Code: %s, Model: %s, Nominal Ouput: %s, Serial# %s]",
-                            hex(inverter_model.device_code),
-                            inverter_model.model,
-                            inverter_model.nominal_output_power,
-                            inverter_model.serial_number,
-                        )
-
-                        # see if the inverter supports a battery if so grab that data also
-                        if inverter_model.inverter_type == "hybrid":
-                            
-                            connection = self._modbusclient.connect()
-                            if connection:
-
-                                # load the inverter registers to get static data, and determine if model found is supported.
-                                for scan_type in INVERTER_SCAN["holding"]:
-                                    if not await self._load_registers("holding", scan_type["scan_start"], INVERTER_HOLDING_REGISTERS, scan_type["scan_range"]):
-                                        return False
-
-                                self._modbusclient.close()
-
-                                if "battery_type" in self.data:
-                                    self.battery_type = self.data["battery_type"]
-                                    self.battery_energy_capacity = round((self.data["battery_nominal_voltage"] * self.data["battery_capacity"]) / 1000, 1)
-                                    self.data["battery_energy_capacity"] = self.battery_energy_capacity
-
-                                logging.info("Storage device attached to inverter: [Model: %s, Capacity: %s kWh]", self.battery_type, self.battery_energy_capacity)
-
-                        return inverter_model
-                                       
-                    else:
-                        logging.error("UPSUPPORT INVERTER: Supported inverter device_type_code [%s] is not supported", self.data["device_type_code"])
-                else:
-                    logging.error("DEVICE CODE NOT FOUND: A device code could not be obtained from the inverter")
-            else:
-                logging.error("CONNECTION ERROR: Could not connect to inverter @ Host: %s, Port: %s", self._modbusclient.host, self._modbusclient.port)                                        
-        else:
-            return SungrowInverterModel(self.device_code, self.model, self.inverter_type, self.mppt_inputs, self.nominal_output_power, self.serial_number)
-
-        return None
-
-    # Core monitoring loop
-    async def async_update(self):
-        """Connect to the inverter and scrape the metrics"""
-
-        if self.model is None:
-            await self.inverter_model()
-
-        if self.model is not None:
-            
-            calculation_registers = None
-
-            if self.inverter_type == "hybrid":
-                inverter_scan = HYBRID_SCAN
-                read_registers = HYBRID_READ_REGISTERS
-                holding_registers = HYBRID_HOLDING_REGISTERS
-                calculation_registers = HYBRID_CALCULATED_REGISTERS
-
-            elif self.inverter_type == "string":
-                inverter_scan = STRING_SCAN
-                read_registers = STRING_READ_REGISTERS
-                holding_registers = STRING_HOLDING_REGISTERS
-                
-            else:
-                logging.error("UNSUPPORTED INVERTER: Inverter type is not supported")
-                return False
-
-            connected = self._modbusclient.connect()
-
-            if connected:
-                for scan_type, scan_settings in inverter_scan.items():
-                    for scan in scan_settings:
-                        if not await self._load_registers(scan_type,
-                                                          scan["scan_start"],
-                                                          read_registers if scan_type == "read" else holding_registers,
-                                                          int(scan["scan_range"])):
-                            return False
-
-                self._modbusclient.close()
-
-                if calculation_registers is not None:
-                    for register_calc in calculation_registers:
-                        try:
-                            self.data[register_calc.key] = eval(register_calc.calculation)
-                        finally:
-                            self.data[register_calc.key] = 0
-                            
-                try:
-                    self.data["timestamp"] = '%s/%s/%s %02d:%02d:%02d' % (
-                        self.data["year"], self.data["month"], self.data["day"],
-                        self.data["hour"], self.data["minute"], self.data["second"])
-                except Exception:
-                    pass
-
-                logging.debug("Inverter register data %s", self.data)
-                return True
-            else:
-                logging.error("CONNECTION ERROR: Could not connect to inverter to read modbus registers")
-
-        return False
-
-
-    # Core monitoring loop
-    async def async_scan(self, register_type, start_register, register_count, step_by = 20):
-        """Connect to the inverter and scan for register locations"""
-
-        connected = self._modbusclient.connect()
-
-        if connected:
-            for start in range(start_register, start_register + register_count, step_by):
-                try:
-                    if register_type == "read":
-                        response = self._modbusclient.read_input_registers(int(start - 1), count=step_by, unit=self._slave)
-                    elif register_type == "holding":
-                        response = self._modbusclient.read_holding_registers(int(start - 1), count=step_by, unit=self._slave)
-
-                    if hasattr(response, 'registers'):
-                        logging.info("[start_register: %s, register_count: %s] contents: %s", int(start_register) , register_count, response.registers)
-                    else:
-                        logging.info("[start_register: %s, register_count: %s] nothing returned", int(start_register) , register_count)
-
-                except Exception:
-                    logging.info("Exception thrown")
-
-            self._modbusclient.close()
-            return True
-        return False
+"""
+
+Sungrow Inverter register reader
+
+Connect to a Sungrow modbus via TCP
+
+Supports Sungrow Hybrid & String inverters
+
+Refer configs/hybrid.py and configs/string.py for inverters that are supported.
+"""
+
+__version__ = "0.2.1"
+
+from sungrowinverter.SungrowModbusTCPClient import SungrowModbusTcpClient
+from sungrowinverter.configs.inverter import (
+    INVERTER_SCAN,
+    INVERTER_READ_REGISTERS,
+    INVERTER_HOLDING_REGISTERS,
+    INVERTER_MODELS,
+)
+
+from sungrowinverter.configs.common import SungrowInverterModel
+
+from sungrowinverter.configs.hybrid import (
+    HYBRID_SCAN,
+    HYBRID_READ_REGISTERS,
+    HYBRID_HOLDING_REGISTERS,
+    HYBRID_CALCULATED_REGISTERS,
+)
+from sungrowinverter.configs.string import (
+    STRING_SCAN,
+    STRING_READ_REGISTERS,
+    STRING_HOLDING_REGISTERS,
+)
+
+import logging
+
+REQUESTS_TIMEOUT = 60
+
+
+class SungrowInverter:
+    """
+    SungrowInverter module for read modbus data from tcp connect to Sungrow inverters (hybrid / string) inverters supported
+    """
+
+    def __init__(self, ip_address, port=502, slave=1, retries=3, timeout=REQUESTS_TIMEOUT):
+        """Initialize a Sungrow Inverter TCP Modbus Client object"""
+        self.manufacturer = "Sungrow"
+
+        # Set when invert_model is run
+        self.model = None
+        self.device_code = None
+        self.mppt_inputs = 0
+        self.serial_number = None
+        self.nominal_output_power = None
+        self.inverter_type = None
+
+        self.battery_type = None
+        self.battery_energy_capacity = None
+
+        self._modbusclient = None
+        self._slave = slave
+        self._timeout = timeout
+
+        self.data = {}
+
+        client_payload = {
+            "host": ip_address,
+            "port": port,
+            "timeout": timeout,
+            "retries": retries,
+            "retry_on_empty": True,
+        }
+
+        self._modbusclient = SungrowModbusTcpClient(**client_payload)
+
+        logging.debug("Sungrow modbus TCP client - [IP:%s Port:%s]", ip_address, port)
+
+    async def _load_registers(self, register_type, start, modbus_registers, count=100):
+        try:
+            if register_type == "read":
+                response = self._modbusclient.read_input_registers(int(start), count=count, slave=self._slave)
+            elif register_type == "holding":
+                response = self._modbusclient.read_holding_registers(int(start), count=count, slave=self._slave)
+            else:
+                logging.error("Unsupported register type: %s", register_type)
+
+        except Exception as err:
+            logging.warning("No data. Try increasing the timeout or scan interval: %s", err, exc_info=1)
+            return False
+
+        if response.isError():
+            logging.warning("Modbus connection failed, connection could not be made or register range failed to be read.")
+            return False
+
+        if not hasattr(response, "registers"):
+            logging.warning("No registers returned")
+            return
+
+        if len(response.registers) != count:
+            logging.warning("Mismatched number of registers read %s != %s", len(response.registers), count)
+            return
+
+        logging.debug("Registers: %s [start_register: %s, register_count: %s] contents: %s", register_type, int(start) + 1, count, response.registers)
+
+        for current_register in modbus_registers:
+
+            if (start + 1) <= current_register.address < (start + 1 + count):
+
+                if not next((x for x in modbus_registers if x.address == current_register.address), None,) is None:
+
+                    try:
+
+                        if not current_register.valid_inverters is None:
+                            if not self.device_code in current_register.valid_inverters:
+                                continue
+
+                        # We want to make sure we only add the neccessary mppt entries we dont need to create data
+                        # if the inverter don't support it (most have 2, others 1, 3 or more)
+                        if current_register.key.startswith("mppt_"):
+                            mppt_key = current_register.key.split("_")
+                            if int(mppt_key[1]) > self.mppt_inputs:
+                                continue
+
+                        register_index = current_register.address - (start + 1)
+
+                        if current_register.data_type == "U16":
+                            value = response.registers[register_index]
+
+                        elif current_register.data_type == "U32":
+                            value = (response.registers[register_index + 1] << 16) + response.registers[register_index]
+
+                        elif current_register.data_type == "S16":
+                            value = int.from_bytes(response.registers[register_index].to_bytes(2, "little"), "little", signed=True)
+
+                        elif current_register.data_type == "S32":
+                            value = int.from_bytes(((response.registers[register_index + 1] << 16) + response.registers[register_index]).to_bytes(4, "little"), "little", signed=True)
+
+                        elif current_register.data_type == "UTF8":
+                            value = await self._get_utf8(response.registers, register_index, current_register.length)
+
+                        else:
+                            logging.debug("Unknown data_type used for register %s [register: %s data_type: %s]",
+                                            current_register.key, current_register.address, current_register.data_type)
+
+                        if current_register.unit_precision is not None:
+                            value = round(value * current_register.unit_precision, 1)
+
+                        if current_register.table is not None:
+
+                            # if we need to decode a returned value into a set of binary information
+                            # table hold binary map
+                            # value here will contain the bits to translate against the binary map
+                            if current_register.transform == "BINARY":
+                                # we will set each bit into a value ie. whether something is on or off usually.
+                                binary_map = current_register.table
+                                bit_val = 1
+                                while bit_val < 2 ** int(current_register.length):
+                                    if bit_val in binary_map:
+                                        if value & bit_val == bit_val:
+                                            self.data[binary_map[bit_val]] = True
+                                        else:
+                                            self.data[binary_map[bit_val]] = False
+                                    bit_val = bit_val << 1
+                            else:
+                                #if value in current_register.table:
+                                self.data[current_register.key] = current_register.table[value]
+
+                        else:
+                            self.data[current_register.key] = value
+                    
+                    except Exception as err:
+                        exp = err
+
+        return True
+
+    async def _get_utf8(self, registers, index, length):
+
+        buff = b""
+        for byte in range(index, length):
+            buff += bytes(int(registers[byte]).to_bytes(2, byteorder="big"))
+
+        if bytes(buff).find(b"\0", 0):
+            end = bytes(buff).find(b"\0")
+            if end != -1:
+                return bytes(buff)[0:end].decode("utf-8")
+
+        return ""
+
+    async def inverter_model(self) -> SungrowInverterModel:
+        """Connect to the inverter and scrape the inverter model and serial data"""
+
+        # if first time run then get the model details and load the relevant modmap for the model for future requests
+        # if we fail to connect then do nothing and exit
+        if self.model is None:
+
+            connection = self._modbusclient.connect()
+
+            if connection:
+                # load the inverter registers to get static data, and determine if model found is supported.
+                for scan_type in INVERTER_SCAN["read"]:
+                    if not await self._load_registers("read", scan_type["scan_start"], INVERTER_READ_REGISTERS, scan_type["scan_range"]):
+                        return False
+
+                self._modbusclient.close()
+
+                if "device_type_code" in self.data:
+                    inverter_model = next((x for x in INVERTER_MODELS if x.device_code == self.data["device_type_code"]), None,)
+
+                    if inverter_model is not None:
+                        self.model = inverter_model.model
+                        self.data["model"] = inverter_model.model
+                        self.inverter_type = inverter_model.inverter_type
+                        self.mppt_inputs = inverter_model.mppt_inputs
+                        self.serial_number = self.data["serial_number"]
+                        self.nominal_output_power = f"{self.data['nominal_output_power']} kW"
+                        inverter_model.nominal_output_power = self.nominal_output_power
+                        inverter_model.serial_number = self.serial_number
+                        self.device_code = self.data['device_type_code']
+
+                        logging.info(
+                            "Sungrow residential inverter found: [Device Code: %s, Model: %s, Nominal Ouput: %s, Serial# %s]",
+                            hex(inverter_model.device_code),
+                            inverter_model.model,
+                            inverter_model.nominal_output_power,
+                            inverter_model.serial_number,
+                        )
+
+                        # see if the inverter supports a battery if so grab that data also
+                        if inverter_model.inverter_type == "hybrid":
+                            
+                            connection = self._modbusclient.connect()
+                            if connection:
+
+                                # load the inverter registers to get static data, and determine if model found is supported.
+                                for scan_type in INVERTER_SCAN["holding"]:
+                                    if not await self._load_registers("holding", scan_type["scan_start"], INVERTER_HOLDING_REGISTERS, scan_type["scan_range"]):
+                                        return False
+
+                                self._modbusclient.close()
+
+                                if "battery_type" in self.data:
+                                    self.battery_type = self.data["battery_type"]
+                                    self.battery_energy_capacity = round((self.data["battery_nominal_voltage"] * self.data["battery_capacity"]) / 1000, 1)
+                                    self.data["battery_energy_capacity"] = self.battery_energy_capacity
+
+                                logging.info("Storage device attached to inverter: [Model: %s, Capacity: %s kWh]", self.battery_type, self.battery_energy_capacity)
+
+                        return inverter_model
+                                       
+                    else:
+                        logging.error("UPSUPPORT INVERTER: Supported inverter device_type_code [%s] is not supported", self.data["device_type_code"])
+                else:
+                    logging.error("DEVICE CODE NOT FOUND: A device code could not be obtained from the inverter")
+            else:
+                logging.error("CONNECTION ERROR: Could not connect to inverter @ Host: %s, Port: %s", self._modbusclient.host, self._modbusclient.port)                                        
+        else:
+            return SungrowInverterModel(self.device_code, self.model, self.inverter_type, self.mppt_inputs, self.nominal_output_power, self.serial_number)
+
+        return None
+
+    # Core monitoring loop
+    async def async_update(self):
+        """Connect to the inverter and scrape the metrics"""
+
+        if self.model is None:
+            await self.inverter_model()
+
+        if self.model is not None:
+            
+            calculation_registers = None
+
+            if self.inverter_type == "hybrid":
+                inverter_scan = HYBRID_SCAN
+                read_registers = HYBRID_READ_REGISTERS
+                holding_registers = HYBRID_HOLDING_REGISTERS
+                calculation_registers = HYBRID_CALCULATED_REGISTERS
+
+            elif self.inverter_type == "string":
+                inverter_scan = STRING_SCAN
+                read_registers = STRING_READ_REGISTERS
+                holding_registers = STRING_HOLDING_REGISTERS
+                
+            else:
+                logging.error("UNSUPPORTED INVERTER: Inverter type is not supported")
+                return False
+
+            connected = self._modbusclient.connect()
+
+            if connected:
+                for scan_type, scan_settings in inverter_scan.items():
+                    for scan in scan_settings:
+                        if not await self._load_registers(scan_type,
+                                                          scan["scan_start"],
+                                                          read_registers if scan_type == "read" else holding_registers,
+                                                          int(scan["scan_range"])):
+                            return False
+
+                self._modbusclient.close()
+
+                if calculation_registers is not None:
+                    for register_calc in calculation_registers:
+                        try:
+                            self.data[register_calc.key] = eval(register_calc.calculation)
+                        except ZeroDivisionError:
+                            self.data[register_calc.key] = 0
+
+                try:
+                    self.data["timestamp"] = '%s/%s/%s %02d:%02d:%02d' % (
+                        self.data["year"], self.data["month"], self.data["day"],
+                        self.data["hour"], self.data["minute"], self.data["second"])
+                except Exception:
+                    pass
+
+                logging.debug("Inverter register data %s", self.data)
+                return True
+            else:
+                logging.error("CONNECTION ERROR: Could not connect to inverter to read modbus registers")
+
+        return False
+
+
+    # Core monitoring loop
+    async def async_scan(self, register_type, start_register, register_count, step_by = 20):
+        """Connect to the inverter and scan for register locations"""
+
+        connected = self._modbusclient.connect()
+
+        if connected:
+            for start in range(start_register, start_register + register_count, step_by):
+                try:
+                    if register_type == "read":
+                        response = self._modbusclient.read_input_registers(int(start - 1), count=step_by, unit=self._slave)
+                    elif register_type == "holding":
+                        response = self._modbusclient.read_holding_registers(int(start - 1), count=step_by, unit=self._slave)
+
+                    if hasattr(response, 'registers'):
+                        logging.info("[start_register: %s, register_count: %s] contents: %s", int(start_register) , register_count, response.registers)
+                    else:
+                        logging.info("[start_register: %s, register_count: %s] nothing returned", int(start_register) , register_count)
+
+                except Exception:
+                    logging.info("Exception thrown")
+
+            self._modbusclient.close()
+            return True
+        return False
```

### Comparing `sungrowinverter-0.2.1/sungrowinverter/SungrowModbusTCPClient.py` & `sungrowinverter-0.2.2/sungrowinverter/SungrowModbusTCPClient.py`

 * *Files identical despite different names*

### Comparing `sungrowinverter-0.2.1/sungrowinverter/configs/common.py` & `sungrowinverter-0.2.2/sungrowinverter/configs/common.py`

 * *Files identical despite different names*

### Comparing `sungrowinverter-0.2.1/sungrowinverter/configs/hybrid.py` & `sungrowinverter-0.2.2/sungrowinverter/configs/hybrid.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-"""
-#
-# Sungrow Hybrid Storage Inverter Series
-#
-# Valid device types:
-#    SH3K6 / SH4K6 / SH5K-V13 / SH5K-20     - Residential Hybrid Single Phase Inverter for Low Voltage Battery [48V to 70V]
-#    SH4K6-30 / SH5K-30 / SH3K6-30          - Residential Hybrid Single Phase Inverter for Low Voltage Battery [48V to 70V newer version]
-#    SH3.6RS / SH4.6RS / SH5.0RS / SH6.0RS  - Residential Hybrid Single Phase Inverter wide battery voltage range [80V to 460V]
-#    SH5.0RT / SH6.0RT / SH8.0RT / SH10RT   - Residential Hybrid Three Phase Inverter wide battery voltage range [80V to 460V]
-#
-# Sungrow hybrid inverter register definitions
-"""
-
-from sungrowinverter.configs.common import (
-    ModBusRegister,
-    CalcRegister,
-    OUTPUT_TYPE_CODES,
-    GRID_STATE_CODES,
-    TEMP_CELSIUS,
-    KILO_WATT_HOUR,
-    WATT,
-    KILOGRAMS,
-    PERCENTAGE,
-    VOLTAGE,
-    AMPERE,
-    HERTZ,
-)
-
-SYSTEM_STATE_CODES = {
-    0x2: "Stop",
-    0x8: "Standby",
-    0x10: "Initial Standby",
-    0x20: "Startup",
-    0x40: "Running",
-    0x100: "Falt",
-    0x400: "Running in maintain mode",
-    0x800: "Running in forced mode",
-    0x1000: "Running in off-grid mode",
-    0x2501: "Restarting",
-    0x4000: "Running in external EMS mode",
-}
-
-# a data item will exist for each of these states, 
-# the running_state register translates to each of bits below.
-RUNNING_STATE_BITS = {
-    0b00000001: "status_power_generated_from_pv",
-    0b00000010: "status_charging",
-    0b00000100: "status_discharging",
-    0b00001000: "status_load_is_active",
-    0b00010000: "status_exporting_power_to_grid",
-    0b00100000: "status_importing_power_from_grid",
-    0b10000000: "status_power_generated_from_load",
-}
-
-EMS_MODE_CODES = {
-    0: "Self consumption mode (default)",
-    2: "Forced mode (charge/discharge/stop)",
-    3: "External EMS mode",
-}
-
-COMMAND_CHARGE_CODES = {
-    0xAA: "Charge",
-    0xBB: "Discharge",
-    0xCC: "Stop (default)"
-}
-
-# the scan register start 1 less than the actual register recorded in specs.
-# reason being registers start at 0, document for modbus usually refers to register 1 as the start of registers.
-HYBRID_SCAN = {
-    "read": [
-        {"scan_start": 5000, "scan_range": 50},
-        {"scan_start": 12999, "scan_range": 100},
-    ],
-    "holding": [
-        {"scan_start": 4999, "scan_range": 6},
-        {"scan_start": 12999, "scan_range": 17},
-        {"scan_start": 13049, "scan_range": 51},
-    ],
-}
-
-HYBRID_READ_REGISTERS: tuple[ModBusRegister, ...] = (
-    ModBusRegister(5002, "output_type", "U16", table=OUTPUT_TYPE_CODES),
-    ModBusRegister(5003, "daily_energy_yield", "U16", 0.1, KILO_WATT_HOUR, description="Hybrid active power accumulation (Include PV generation and battery discharge energy)"),
-    ModBusRegister(5004, "total_energy_yield", "U32", 0.1, KILO_WATT_HOUR, description="Hybrid active power accumulation (Include PV generation and battery discharge energy)"),
-    ModBusRegister(5008, "inside_temperature", "U16", 0.1, TEMP_CELSIUS, description="Internal inverter temperature"),
-    ModBusRegister(5011, "mppt_1_voltage", "U16", 0.1, VOLTAGE),
-    ModBusRegister(5012, "mppt_1_current", "U16", 0.1, AMPERE),
-    ModBusRegister(5013, "mppt_2_voltage", "U16", 0.1, VOLTAGE),
-    ModBusRegister(5014, "mppt_2_current", "U16", 0.1, AMPERE),
-    ModBusRegister(5017, "total_dc_power", "U32", unit_of_measure=WATT, description="PV power that is usable (inverter inefficiency)"),
-    ModBusRegister(5019, "grid_voltage", "U16", 0.1, VOLTAGE),
-    ModBusRegister(5019, "phase_a_voltage", "U16", 0.1, VOLTAGE, description="Phase A (1-2) voltage is also the grid voltage on a single phase inverter"),
-    ModBusRegister(5020, "phase_b_voltage", "U16", 0.1, VOLTAGE, valid_inverters=[0xE00,0xE01,0xE02,0xE03,0xE0F]),
-    ModBusRegister(5021, "phase_c_voltage", "U16", 0.1, VOLTAGE, valid_inverters=[0xE00,0xE01,0xE02,0xE03,0xE0F]),
-    ModBusRegister(5033, "reactive_power", "S32", unit_of_measure="var"),
-    ModBusRegister(5035, "power_factor", "U16", 0.001),
-    ModBusRegister(5036, "grid_frequency", "U16", 0.1, HERTZ),
-
-    ModBusRegister(13000, "system_state", "U16", table=SYSTEM_STATE_CODES),
-    ModBusRegister(13001, "running_state", "U16", transform="BINARY", length=8, table=RUNNING_STATE_BITS),
-    ModBusRegister(13002, "daily_pv_generation", "U16", 0.1, KILO_WATT_HOUR),
-    ModBusRegister(13003, "total_pv_generation", "U32", 0.1, KILO_WATT_HOUR),
-    ModBusRegister(13005, "daily_export_from_pv", "U16", 0.1, KILO_WATT_HOUR),
-    ModBusRegister(13006, "total_export_from_pv", "U32", 0.1, KILO_WATT_HOUR),
-    ModBusRegister(13008, "load_power", "S32", unit_of_measure=WATT),
-    ModBusRegister(13010, "export_power", "S32", unit_of_measure=WATT),
-    ModBusRegister(13012, "daily_battery_charge_from_pv", "U16", 0.1, KILO_WATT_HOUR),
-    ModBusRegister(13013, "total_battery_charge_from_pv", "U32", 0.1, KILO_WATT_HOUR),
-    ModBusRegister(13015, "co2_reduction", "U32", 0.1, KILOGRAMS),
-    ModBusRegister(13017, "daily_direct_energy_consumption", "U16", 0.1, KILO_WATT_HOUR),
-    ModBusRegister(13018, "total_direct_energy_consumption", "U32", 0.1, KILO_WATT_HOUR),
-    ModBusRegister(13020, "battery_voltage", "U16", 0.1, VOLTAGE),
-    ModBusRegister(13021, "battery_current", "U16", 0.1, AMPERE),
-    ModBusRegister(13022, "battery_power", "U16", 0.1, WATT),
-    ModBusRegister(13023, "battery_level", "U16", 0.1, PERCENTAGE),
-    ModBusRegister(13024, "battery_state_of_health", "U16", 0.1, PERCENTAGE),
-    ModBusRegister(13025, "battery_temperature", "U16", 0.1, TEMP_CELSIUS),
-    ModBusRegister(13026, "daily_battery_discharge", "U16", 0.1, KILO_WATT_HOUR, description="Daily energy that was discharged into the grid"),
-    ModBusRegister(13027, "total_battery_discharge", "U32", 0.1, KILO_WATT_HOUR, description="Total energy that was discharged into the grid"),
-    ModBusRegister(13029, "self_consumption_today", "U16", 0.1, PERCENTAGE),
-    ModBusRegister(13030, "grid_state", "U16", table=GRID_STATE_CODES),
-    ModBusRegister(13031, "phase_a_current", "U16", 0.1, AMPERE),
-    ModBusRegister(13032, "phase_b_current", "U16", 0.1, AMPERE, valid_inverters=[0xE00,0xE01,0xE02,0xE03,0xE0F]),
-    ModBusRegister(13033, "phase_c_current", "U16", 0.1, AMPERE, valid_inverters=[0xE00,0xE01,0xE02,0xE03,0xE0F]),
-    ModBusRegister(13034, "total_active_power", "U32", 0.1, WATT),
-    ModBusRegister(13036, "daily_import_energy", "U16", 0.1, KILO_WATT_HOUR),
-    ModBusRegister(13037, "total_import_energy", "U32", 0.1, KILO_WATT_HOUR),
-
-    ModBusRegister(13040, "daily_charge_from_grid", "U16", 0.1, KILO_WATT_HOUR),
-    ModBusRegister(13041, "total_charge_from_grid", "U16", 0.1, KILO_WATT_HOUR),
-    ModBusRegister(13045, "daily_export_from_battery", "U16", 0.1, KILO_WATT_HOUR),
-    ModBusRegister(13046, "total_export_from_battery", "U32", 0.1, KILO_WATT_HOUR),
-)
-
-HYBRID_HOLDING_REGISTERS: tuple[ModBusRegister, ...] = (
-    ModBusRegister(5000, "year", "U16"),
-    ModBusRegister(5001, "month", "U16"),
-    ModBusRegister(5002, "day", "U16"),
-    ModBusRegister(5003, "hour", "U16"),
-    ModBusRegister(5004, "minute", "U16"),
-    ModBusRegister(5005, "second", "U16"),
-)
-
-HYBRID_CALCULATED_REGISTERS: tuple[CalcRegister, ...] = (
-    CalcRegister("daily_export_energy", "self.data['daily_export_from_pv'] + self.data['daily_export_from_battery']", unit_of_measure=KILO_WATT_HOUR),
-    CalcRegister("total_export_energy", "self.data['total_export_from_pv'] + self.data['total_export_from_battery']", unit_of_measure=KILO_WATT_HOUR),
-    CalcRegister("daily_batery_charge", "self.data['daily_battery_charge_from_pv'] + self.data['daily_charge_from_grid']", unit_of_measure=KILO_WATT_HOUR),
-    CalcRegister("total_batery_charge", "self.data['total_battery_charge_from_pv'] + self.data['total_charge_from_grid']", unit_of_measure=KILO_WATT_HOUR),
-    CalcRegister("inverter_efficiency", "int((self.data['daily_energy_yield'] / self.data['daily_pv_generation']) * 100)", unit_of_measure=PERCENTAGE, description="Energy yield from the days pv generation")  
-)
+"""
+#
+# Sungrow Hybrid Storage Inverter Series
+#
+# Valid device types:
+#    SH3K6 / SH4K6 / SH5K-V13 / SH5K-20     - Residential Hybrid Single Phase Inverter for Low Voltage Battery [48V to 70V]
+#    SH4K6-30 / SH5K-30 / SH3K6-30          - Residential Hybrid Single Phase Inverter for Low Voltage Battery [48V to 70V newer version]
+#    SH3.6RS / SH4.6RS / SH5.0RS / SH6.0RS  - Residential Hybrid Single Phase Inverter wide battery voltage range [80V to 460V]
+#    SH5.0RT / SH6.0RT / SH8.0RT / SH10RT   - Residential Hybrid Three Phase Inverter wide battery voltage range [80V to 460V]
+#
+# Sungrow hybrid inverter register definitions
+"""
+
+from sungrowinverter.configs.common import (
+    ModBusRegister,
+    CalcRegister,
+    OUTPUT_TYPE_CODES,
+    GRID_STATE_CODES,
+    TEMP_CELSIUS,
+    KILO_WATT_HOUR,
+    WATT,
+    KILOGRAMS,
+    PERCENTAGE,
+    VOLTAGE,
+    AMPERE,
+    HERTZ,
+)
+
+SYSTEM_STATE_CODES = {
+    0x2: "Stop",
+    0x8: "Standby",
+    0x10: "Initial Standby",
+    0x20: "Startup",
+    0x40: "Running",
+    0x100: "Fault",
+    0x400: "Running in maintain mode",
+    0x800: "Running in forced mode",
+    0x1000: "Running in off-grid mode",
+    0x2501: "Restarting",
+    0x4000: "Running in external EMS mode",
+}
+
+# a data item will exist for each of these states, 
+# the running_state register translates to each of bits below.
+RUNNING_STATE_BITS = {
+    0b00000001: "status_power_generated_from_pv",
+    0b00000010: "status_charging",
+    0b00000100: "status_discharging",
+    0b00001000: "status_load_is_active",
+    0b00010000: "status_exporting_power_to_grid",
+    0b00100000: "status_importing_power_from_grid",
+    0b10000000: "status_power_generated_from_load",
+}
+
+EMS_MODE_CODES = {
+    0: "Self consumption mode (default)",
+    2: "Forced mode (charge/discharge/stop)",
+    3: "External EMS mode",
+}
+
+COMMAND_CHARGE_CODES = {
+    0xAA: "Charge",
+    0xBB: "Discharge",
+    0xCC: "Stop (default)"
+}
+
+# the scan register start 1 less than the actual register recorded in specs.
+# reason being registers start at 0, document for modbus usually refers to register 1 as the start of registers.
+HYBRID_SCAN = {
+    "read": [
+        {"scan_start": 5000, "scan_range": 50},
+        {"scan_start": 12999, "scan_range": 100},
+    ],
+    "holding": [
+        {"scan_start": 4999, "scan_range": 6},
+        {"scan_start": 12999, "scan_range": 17},
+        {"scan_start": 13049, "scan_range": 51},
+    ],
+}
+
+HYBRID_READ_REGISTERS: tuple[ModBusRegister, ...] = (
+    ModBusRegister(5002, "output_type", "U16", table=OUTPUT_TYPE_CODES),
+    ModBusRegister(5003, "daily_energy_yield", "U16", 0.1, KILO_WATT_HOUR, description="Hybrid active power accumulation (Include PV generation and battery discharge energy)"),
+    ModBusRegister(5004, "total_energy_yield", "U32", 0.1, KILO_WATT_HOUR, description="Hybrid active power accumulation (Include PV generation and battery discharge energy)"),
+    ModBusRegister(5008, "inside_temperature", "U16", 0.1, TEMP_CELSIUS, description="Internal inverter temperature"),
+    ModBusRegister(5011, "mppt_1_voltage", "U16", 0.1, VOLTAGE),
+    ModBusRegister(5012, "mppt_1_current", "U16", 0.1, AMPERE),
+    ModBusRegister(5013, "mppt_2_voltage", "U16", 0.1, VOLTAGE),
+    ModBusRegister(5014, "mppt_2_current", "U16", 0.1, AMPERE),
+    ModBusRegister(5017, "total_dc_power", "U32", unit_of_measure=WATT, description="PV power that is usable (inverter inefficiency)"),
+    ModBusRegister(5019, "grid_voltage", "U16", 0.1, VOLTAGE),
+    ModBusRegister(5019, "phase_a_voltage", "U16", 0.1, VOLTAGE, description="Phase A (1-2) voltage is also the grid voltage on a single phase inverter"),
+    ModBusRegister(5020, "phase_b_voltage", "U16", 0.1, VOLTAGE, valid_inverters=[0xE00,0xE01,0xE02,0xE03,0xE0D,0xE0E,0xE0F,0xE13]),
+    ModBusRegister(5021, "phase_c_voltage", "U16", 0.1, VOLTAGE, valid_inverters=[0xE00,0xE01,0xE02,0xE03,0xE0D,0xE0E,0xE0F,0xE13]),
+    ModBusRegister(5033, "reactive_power", "S32", unit_of_measure="var"),
+    ModBusRegister(5035, "power_factor", "U16", 0.001),
+    ModBusRegister(5036, "grid_frequency", "U16", 0.1, HERTZ),
+
+    ModBusRegister(13000, "system_state", "U16", table=SYSTEM_STATE_CODES),
+    ModBusRegister(13001, "running_state", "U16", transform="BINARY", length=8, table=RUNNING_STATE_BITS),
+    ModBusRegister(13002, "daily_pv_generation", "U16", 0.1, KILO_WATT_HOUR),
+    ModBusRegister(13003, "total_pv_generation", "U32", 0.1, KILO_WATT_HOUR),
+    ModBusRegister(13005, "daily_export_from_pv", "U16", 0.1, KILO_WATT_HOUR),
+    ModBusRegister(13006, "total_export_from_pv", "U32", 0.1, KILO_WATT_HOUR),
+    ModBusRegister(13008, "load_power", "S32", unit_of_measure=WATT),
+    ModBusRegister(13010, "export_power", "S32", unit_of_measure=WATT),
+    ModBusRegister(13012, "daily_battery_charge_from_pv", "U16", 0.1, KILO_WATT_HOUR),
+    ModBusRegister(13013, "total_battery_charge_from_pv", "U32", 0.1, KILO_WATT_HOUR),
+    ModBusRegister(13015, "co2_reduction", "U32", 0.1, KILOGRAMS),
+    ModBusRegister(13017, "daily_direct_energy_consumption", "U16", 0.1, KILO_WATT_HOUR),
+    ModBusRegister(13018, "total_direct_energy_consumption", "U32", 0.1, KILO_WATT_HOUR),
+    ModBusRegister(13020, "battery_voltage", "U16", 0.1, VOLTAGE),
+    ModBusRegister(13021, "battery_current", "U16", 0.1, AMPERE),
+    ModBusRegister(13022, "battery_power", "U16", WATT),
+    ModBusRegister(13023, "battery_level", "U16", 0.1, PERCENTAGE),
+    ModBusRegister(13024, "battery_state_of_health", "U16", 0.1, PERCENTAGE),
+    ModBusRegister(13025, "battery_temperature", "U16", 0.1, TEMP_CELSIUS),
+    ModBusRegister(13026, "daily_battery_discharge", "U16", 0.1, KILO_WATT_HOUR, description="Daily energy that was discharged into the grid"),
+    ModBusRegister(13027, "total_battery_discharge", "U32", 0.1, KILO_WATT_HOUR, description="Total energy that was discharged into the grid"),
+    ModBusRegister(13029, "self_consumption_today", "U16", 0.1, PERCENTAGE),
+    ModBusRegister(13030, "grid_state", "U16", table=GRID_STATE_CODES),
+    ModBusRegister(13031, "phase_a_current", "U16", 0.1, AMPERE),
+    ModBusRegister(13032, "phase_b_current", "U16", 0.1, AMPERE, valid_inverters=[0xE00,0xE01,0xE02,0xE03,0xE0D,0xE0E,0xE0F,0xE13]),
+    ModBusRegister(13033, "phase_c_current", "U16", 0.1, AMPERE, valid_inverters=[0xE00,0xE01,0xE02,0xE03,0xE0D,0xE0E,0xE0F,0xE13]),
+    ModBusRegister(13034, "total_active_power", "U32", WATT),
+    ModBusRegister(13036, "daily_import_energy", "U16", 0.1, KILO_WATT_HOUR),
+    ModBusRegister(13037, "total_import_energy", "U32", 0.1, KILO_WATT_HOUR),
+
+    ModBusRegister(13040, "daily_charge_from_grid", "U16", 0.1, KILO_WATT_HOUR),
+    ModBusRegister(13041, "total_charge_from_grid", "U16", 0.1, KILO_WATT_HOUR),
+    ModBusRegister(13045, "daily_export_from_battery", "U16", 0.1, KILO_WATT_HOUR),
+    ModBusRegister(13046, "total_export_from_battery", "U32", 0.1, KILO_WATT_HOUR),
+)
+
+HYBRID_HOLDING_REGISTERS: tuple[ModBusRegister, ...] = (
+    ModBusRegister(5000, "year", "U16"),
+    ModBusRegister(5001, "month", "U16"),
+    ModBusRegister(5002, "day", "U16"),
+    ModBusRegister(5003, "hour", "U16"),
+    ModBusRegister(5004, "minute", "U16"),
+    ModBusRegister(5005, "second", "U16"),
+)
+
+HYBRID_CALCULATED_REGISTERS: tuple[CalcRegister, ...] = (
+    CalcRegister("daily_export_energy", "self.data['daily_export_from_pv'] + self.data['daily_export_from_battery']", unit_of_measure=KILO_WATT_HOUR),
+    CalcRegister("total_export_energy", "self.data['total_export_from_pv'] + self.data['total_export_from_battery']", unit_of_measure=KILO_WATT_HOUR),
+    CalcRegister("daily_battery_charge", "self.data['daily_battery_charge_from_pv'] + self.data['daily_charge_from_grid']", unit_of_measure=KILO_WATT_HOUR),
+    CalcRegister("total_battery_charge", "self.data['total_battery_charge_from_pv'] + self.data['total_charge_from_grid']", unit_of_measure=KILO_WATT_HOUR),
+    CalcRegister("inverter_efficiency", "int((self.data['daily_energy_yield'] / self.data['daily_pv_generation']) * 100)", unit_of_measure=PERCENTAGE, description="Energy yield from the days pv generation")  
+)
```

### Comparing `sungrowinverter-0.2.1/sungrowinverter/configs/inverter.py` & `sungrowinverter-0.2.2/sungrowinverter/configs/inverter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,112 +1,116 @@
-"""Sungrow inverter register definitions for the model, serial and nominal power output."""
-
-from sungrowinverter.configs.common import (
-    ModBusRegister,
-    SungrowInverterModel,
-    KILO_WATT,
-    VOLTAGE,
-    AMP_HOUR,
-    BATTERY_TYPES,
-)
-
-INVERTER_SCAN = {
-    "read": [{"scan_start": 4989, "scan_range": 12}],
-    "holding": [{"scan_start": 13054, "scan_range": 3}],
-}
-
-INVERTER_READ_REGISTERS: tuple[ModBusRegister, ...] = (
-    ModBusRegister(4990, "serial_number", "UTF8", length=10),
-    ModBusRegister(5000, "device_type_code", "U16"),
-    ModBusRegister(5001, "nominal_output_power", "U16", 0.1, KILO_WATT),
-)
-
-INVERTER_HOLDING_REGISTERS: tuple[ModBusRegister, ...] = (
-    ModBusRegister(13055, "battery_type", "U16", table=BATTERY_TYPES),
-    ModBusRegister(13056, "battery_nominal_voltage", "U16", 0.1, VOLTAGE),
-    ModBusRegister(13057, "battery_capacity", "U16", 1, AMP_HOUR),
-)
-
-INVERTER_MODELS: list[SungrowInverterModel] = (
-    SungrowInverterModel(0xD03, "SH5K", "hybrid", 2),
-    SungrowInverterModel(0xD06, "SH3K6", "hybrid", 2),
-    SungrowInverterModel(0xD07, "SH4K6", "hybrid", 2),
-    SungrowInverterModel(0xD09, "SH5K-20", "hybrid", 2),
-    SungrowInverterModel(0xD0A, "SH3K6-30", "hybrid", 2),
-    SungrowInverterModel(0xD0B, "SH4K6-30", "hybrid", 2),
-    SungrowInverterModel(0xD0C, "SH5K-30", "hybrid", 2),
-    SungrowInverterModel(0xD0D, "SH3.6RS", "hybrid", 2),
-    SungrowInverterModel(0xD0E, "SH4.6RS", "hybrid", 2),
-    SungrowInverterModel(0xD0F, "SH5.0RS", "hybrid", 2),
-    SungrowInverterModel(0xD10, "SH6.0RS", "hybrid", 2),
-    SungrowInverterModel(0xE00, "SH5.0RT", "hybrid", 2),
-    SungrowInverterModel(0xE01, "SH6.0RT", "hybrid", 2),
-    SungrowInverterModel(0xE02, "SH8.0RT", "hybrid", 2),
-    SungrowInverterModel(0xE03, "SH10RT", "hybrid", 2),
-    SungrowInverterModel(0xE0F, "SH10RT-V112", "hybrid", 2),
-    SungrowInverterModel(0x26,'SG10KTL','string',2),
-    SungrowInverterModel(0x27,'SG30KTL','string',2),
-    SungrowInverterModel(0x28,'SG15KTL','string',2),
-    SungrowInverterModel(0x29,'SG12KTL','string',2),
-    SungrowInverterModel(0x2A,'SG20KTL','string',2),
-    SungrowInverterModel(0x2C,'SG30KU','string',2),
-    SungrowInverterModel(0x2D,'SG36KTL','string',2),
-    SungrowInverterModel(0x2E,'SG36KU','string',2),
-    SungrowInverterModel(0x2F,'SG40KTL','string',2),
-    SungrowInverterModel(0x70,'SG30KTL-M-V31','string',3),
-    SungrowInverterModel(0x72,'SG34KJ','string',2),
-    SungrowInverterModel(0x73,'LP_P34KSG','string',1),
-    SungrowInverterModel(0x74,'SG36KTL-M','string',3),
-    SungrowInverterModel(0x010F,'SG60KTL','string',1),
-    SungrowInverterModel(0x011B,'SG50KTL-M-20','string',4),
-    SungrowInverterModel(0x0131,'SG60KTL-M','string',4),
-    SungrowInverterModel(0x0132,'SG60KU-M','string',4),
-    SungrowInverterModel(0x0134,'SG33KTL-M','string',3),
-    SungrowInverterModel(0x0135,'SG40KTL-M','string',3),
-    SungrowInverterModel(0x0136,'SG60KU','string',1),
-    SungrowInverterModel(0x0137,'SG49K5J','string',4),
-    SungrowInverterModel(0x0138,'SG80KTL','string',1),
-    SungrowInverterModel(0x0139,'SG80KTL-M','string',4),
-    SungrowInverterModel(0x013B,'SG125HV','string',1),
-    SungrowInverterModel(0x013C,'SG12KTL-M','string',2),
-    SungrowInverterModel(0x013D,'SG33K3J','string',3),
-    SungrowInverterModel(0x013E,'SG10KTL-M','string',2),
-    SungrowInverterModel(0x013F,'SG8KTL-M','string',2),
-    SungrowInverterModel(0x0141,'SG30KTL-M','string',3),
-    SungrowInverterModel(0x0142,'SG15KTL-M','string',2),
-    SungrowInverterModel(0x0143,'SG20KTL-M','string',2),
-    SungrowInverterModel(0x0147,'SG5KTL-MT','string',2),
-    SungrowInverterModel(0x0148,'SG6KTL-MT','string',2),
-    SungrowInverterModel(0x0149,'SG17KTL-M','string',2),
-    SungrowInverterModel(0x014C,'SG111HV','string',1),
-    SungrowInverterModel(0x2430,'SG5.0RT','string',2),
-    SungrowInverterModel(0x2431,'SG6.0RT','string',2),
-    SungrowInverterModel(0x2432,'SG8.0RT','string',2),
-    SungrowInverterModel(0x2432,'SG8.0RT','string',2),
-    SungrowInverterModel(0x2433,'SG10RT','string',2),
-    SungrowInverterModel(0x2434,'SG12RT','string',2),
-    SungrowInverterModel(0x2435,'SG15RT','string',2),
-    SungrowInverterModel(0x2436,'SG17RT','string',2),
-    SungrowInverterModel(0x2437,'SG20RT','string',2),
-    SungrowInverterModel(0x243C,'SG7.0RT','string',2),
-    SungrowInverterModel(0x243D,'SG3.0RT','string',2),
-    SungrowInverterModel(0x243E,'SG4.0RT','string',2),
-    SungrowInverterModel(0x2C00,'SG33CX','string',3),
-    SungrowInverterModel(0x2C01,'SG40CX','string',4),
-    SungrowInverterModel(0x2C02,'SG50CX','string',5),
-    SungrowInverterModel(0x2C03,'SG125HV-20','string',1),
-    SungrowInverterModel(0x2C06,'SG110CX','string',9),
-    SungrowInverterModel(0x2C0A,'SG36CX-US','string',3),
-    SungrowInverterModel(0x2C0B,'SG60CX-US','string',5),
-    SungrowInverterModel(0x2C0C,'SG250HX','string',12),
-    SungrowInverterModel(0x2C0F,'SG10KTL-MT','string',2),
-    SungrowInverterModel(0x2C10,'SG30CX','string',3),
-    SungrowInverterModel(0x2C11,'SG250HX-US','string',12),
-    SungrowInverterModel(0x2C12,'SG100CX','string',12),
-    SungrowInverterModel(0x2C13,'SG250HX-IN','string',12),
-    SungrowInverterModel(0x2C15,'SG25CX-SA','string',3),
-    SungrowInverterModel(0x2C22,'SG75CX','string',9),
-    # Maybe a correct inverter setting for unsupported SG5K-D??
-    SungrowInverterModel(0x126,'SG5K-D','string',2),
-    # Supplied in Issue #7
-    SungrowInverterModel(0x2600,'SG2.0RS-S','string',2),
-)
+"""Sungrow inverter register definitions for the model, serial and nominal power output."""
+
+from sungrowinverter.configs.common import (
+    ModBusRegister,
+    SungrowInverterModel,
+    KILO_WATT,
+    VOLTAGE,
+    AMP_HOUR,
+    BATTERY_TYPES,
+)
+
+INVERTER_SCAN = {
+    "read": [{"scan_start": 4989, "scan_range": 12}],
+    "holding": [{"scan_start": 13054, "scan_range": 3}],
+}
+
+INVERTER_READ_REGISTERS: tuple[ModBusRegister, ...] = (
+    ModBusRegister(4990, "serial_number", "UTF8", length=10),
+    ModBusRegister(5000, "device_type_code", "U16"),
+    ModBusRegister(5001, "nominal_output_power", "U16", 0.1, KILO_WATT),
+)
+
+INVERTER_HOLDING_REGISTERS: tuple[ModBusRegister, ...] = (
+    ModBusRegister(13055, "battery_type", "U16", table=BATTERY_TYPES),
+    ModBusRegister(13056, "battery_nominal_voltage", "U16", 0.1, VOLTAGE),
+    ModBusRegister(13057, "battery_capacity", "U16", 1, AMP_HOUR),
+)
+
+INVERTER_MODELS: list[SungrowInverterModel] = (
+    SungrowInverterModel(0xD03, "SH5K", "hybrid", 2),
+    SungrowInverterModel(0xD06, "SH3K6", "hybrid", 2),
+    SungrowInverterModel(0xD07, "SH4K6", "hybrid", 2),
+    SungrowInverterModel(0xD09, "SH5K-20", "hybrid", 2),
+    SungrowInverterModel(0xD0A, "SH3K6-30", "hybrid", 2),
+    SungrowInverterModel(0xD0B, "SH4K6-30", "hybrid", 2),
+    SungrowInverterModel(0xD0C, "SH5K-30", "hybrid", 2),
+    SungrowInverterModel(0xD0D, "SH3.6RS", "hybrid", 2),
+    SungrowInverterModel(0xD0E, "SH4.6RS", "hybrid", 2),
+    SungrowInverterModel(0xD0F, "SH5.0RS", "hybrid", 2),
+    SungrowInverterModel(0xD10, "SH6.0RS", "hybrid", 2),
+    SungrowInverterModel(0xE00, "SH5.0RT", "hybrid", 2),
+    SungrowInverterModel(0xE01, "SH6.0RT", "hybrid", 2),
+    SungrowInverterModel(0xE02, "SH8.0RT", "hybrid", 2),
+    SungrowInverterModel(0xE03, "SH10RT", "hybrid", 2),
+    SungrowInverterModel(0xE0D, "SH6.0RT-V112", "hybrid", 2),
+    SungrowInverterModel(0xE0E, "SH8.0RT-V112", "hybrid", 2),
+    SungrowInverterModel(0xE0F, "SH10RT-V112", "hybrid", 2),
+    SungrowInverterModel(0xE13, "SH10RT-20", "hybrid", 2),
+    SungrowInverterModel(0x26,'SG10KTL','string',2),
+    SungrowInverterModel(0x27,'SG30KTL','string',2),
+    SungrowInverterModel(0x28,'SG15KTL','string',2),
+    SungrowInverterModel(0x29,'SG12KTL','string',2),
+    SungrowInverterModel(0x2A,'SG20KTL','string',2),
+    SungrowInverterModel(0x2C,'SG30KU','string',2),
+    SungrowInverterModel(0x2D,'SG36KTL','string',2),
+    SungrowInverterModel(0x2E,'SG36KU','string',2),
+    SungrowInverterModel(0x2F,'SG40KTL','string',2),
+    SungrowInverterModel(0x70,'SG30KTL-M-V31','string',3),
+    SungrowInverterModel(0x72,'SG34KJ','string',2),
+    SungrowInverterModel(0x73,'LP_P34KSG','string',1),
+    SungrowInverterModel(0x74,'SG36KTL-M','string',3),
+    SungrowInverterModel(0x010F,'SG60KTL','string',1),
+    SungrowInverterModel(0x011B,'SG50KTL-M-20','string',4),
+    SungrowInverterModel(0x0131,'SG60KTL-M','string',4),
+    SungrowInverterModel(0x0132,'SG60KU-M','string',4),
+    SungrowInverterModel(0x0134,'SG33KTL-M','string',3),
+    SungrowInverterModel(0x0135,'SG40KTL-M','string',3),
+    SungrowInverterModel(0x0136,'SG60KU','string',1),
+    SungrowInverterModel(0x0137,'SG49K5J','string',4),
+    SungrowInverterModel(0x0138,'SG80KTL','string',1),
+    SungrowInverterModel(0x0139,'SG80KTL-M','string',4),
+    SungrowInverterModel(0x013B,'SG125HV','string',1),
+    SungrowInverterModel(0x013C,'SG12KTL-M','string',2),
+    SungrowInverterModel(0x013D,'SG33K3J','string',3),
+    SungrowInverterModel(0x013E,'SG10KTL-M','string',2),
+    SungrowInverterModel(0x013F,'SG8KTL-M','string',2),
+    SungrowInverterModel(0x0141,'SG30KTL-M','string',3),
+    SungrowInverterModel(0x0142,'SG15KTL-M','string',2),
+    SungrowInverterModel(0x0143,'SG20KTL-M','string',2),
+    SungrowInverterModel(0x0147,'SG5KTL-MT','string',2),
+    SungrowInverterModel(0x0148,'SG6KTL-MT','string',2),
+    SungrowInverterModel(0x0149,'SG17KTL-M','string',2),
+    SungrowInverterModel(0x014C,'SG111HV','string',1),
+    SungrowInverterModel(0x2430,'SG5.0RT','string',2),
+    SungrowInverterModel(0x2431,'SG6.0RT','string',2),
+    SungrowInverterModel(0x2432,'SG8.0RT','string',2),
+    SungrowInverterModel(0x2432,'SG8.0RT','string',2),
+    SungrowInverterModel(0x2433,'SG10RT','string',2),
+    SungrowInverterModel(0x2434,'SG12RT','string',2),
+    SungrowInverterModel(0x2435,'SG15RT','string',2),
+    SungrowInverterModel(0x2436,'SG17RT','string',2),
+    SungrowInverterModel(0x2437,'SG20RT','string',2),
+    SungrowInverterModel(0x243C,'SG7.0RT','string',2),
+    SungrowInverterModel(0x243D,'SG3.0RT','string',2),
+    SungrowInverterModel(0x243E,'SG4.0RT','string',2),
+    SungrowInverterModel(0x2606,'SG5.0RS','string',2),
+    SungrowInverterModel(0x2C00,'SG33CX','string',3),
+    SungrowInverterModel(0x2C01,'SG40CX','string',4),
+    SungrowInverterModel(0x2C02,'SG50CX','string',5),
+    SungrowInverterModel(0x2C03,'SG125HV-20','string',1),
+    SungrowInverterModel(0x2C06,'SG110CX','string',9),
+    SungrowInverterModel(0x2C0A,'SG36CX-US','string',3),
+    SungrowInverterModel(0x2C0B,'SG60CX-US','string',5),
+    SungrowInverterModel(0x2C0C,'SG250HX','string',12),
+    SungrowInverterModel(0x2C0F,'SG10KTL-MT','string',2),
+    SungrowInverterModel(0x2C10,'SG30CX','string',3),
+    SungrowInverterModel(0x2C11,'SG250HX-US','string',12),
+    SungrowInverterModel(0x2C12,'SG100CX','string',12),
+    SungrowInverterModel(0x2C13,'SG250HX-IN','string',12),
+    SungrowInverterModel(0x2C15,'SG25CX-SA','string',3),
+    SungrowInverterModel(0x2C22,'SG75CX','string',9),
+    # Maybe a correct inverter setting for unsupported SG5K-D??
+    SungrowInverterModel(0x126,'SG5K-D','string',2),
+    # Supplied in Issue #7
+    SungrowInverterModel(0x2600,'SG2.0RS-S','string',2),
+)
```

### Comparing `sungrowinverter-0.2.1/sungrowinverter/configs/string.py` & `sungrowinverter-0.2.2/sungrowinverter/configs/string.py`

 * *Files identical despite different names*

### Comparing `sungrowinverter-0.2.1/PKG-INFO` & `sungrowinverter-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sungrowinverter
-Version: 0.2.1
+Version: 0.2.2
 Summary: Query Sungrow residential hybrid or string inverters for current state and statistics using ModBus TCP client
 Home-page: https://github.com/mvandersteen/SungrowInverter
 License: GNU General Public License
 Author: Mark Vandersteen
 Author-email: mark@vandersteen.me
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -154,7 +154,14 @@
   `client.data['export_power']` - for this register it is a signed value if positive then the inverter is exporting to the grid, if negative then it is importing from the grid.
 
   `client.mppt_inputs` - this value dictates how many client.data['mppt_xx_voltage'] & client.data['mppt_xx_current'] registers are available. These values have been obtained from the modbus specs found in the documents directory on this repository. If an inverter only supports 1 mppt connection then only 1 set of mppt_1_voltage and mppt_1_current will appear. If the inverter supports more then mppt\_\[xx\]\_voltage & mppt\_\[xx\]\_current; where [xx] = the number of mppt inputs the inverter supports; the number available depends on the how many the inverter supports can be 1 to 12 sets of data for current set of support inverters. 
   
 ## Python Version prior to 3.9
 
 Refer to https://github.com/mvandersteen/SungrowInverter/issues/2 if you are having issues, where @hallonstedt explains how to resolve for a prior version of python.
+
+
+## Note
+2024-05-13: I don't have a sungrow invester to test changes on any longer as house is being rebuilt, will look to update again once new build is complete and solar re-added. For now apologies will not be muc help to anyone other than accepting merge every now and then, i don't get on here much any longer.
+
+If you have an inverter not supported by this module BUT do get a response back from the sungrow inverter with a device ID, then you could follow what was done for this pull request https://github.com/mvandersteen/SungrowInverter/commit/9bef6dfcc4db7672edb1140b98bbdd34c672a987 by @ortogonal that is add an entry for your inverter in the inverter list and also if you have a 3 phase inverter (usually denoted by RT) add your inverter number into the list of support inverter for the relevant parameter data pulled from the inverter.
+
```

