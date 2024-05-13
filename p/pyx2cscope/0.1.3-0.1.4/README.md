# Comparing `tmp/pyx2cscope-0.1.3.tar.gz` & `tmp/pyx2cscope-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyx2cscope-0.1.3.tar", max compression
+gzip compressed data, was "pyx2cscope-0.1.4.tar", max compression
```

## Comparing `pyx2cscope-0.1.3.tar` & `pyx2cscope-0.1.4.tar`

### file list

```diff
@@ -1,37 +1,40 @@
--rw-r--r--   0        0        0     1086 2024-03-31 11:44:06.260050 pyx2cscope-0.1.3/LICENSE
--rw-r--r--   0        0        0     5218 2024-03-31 11:44:06.260050 pyx2cscope-0.1.3/README.md
--rw-r--r--   0        0        0      748 2024-03-31 11:44:06.292051 pyx2cscope-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       91 2024-03-31 11:44:06.292051 pyx2cscope-0.1.3/pyx2cscope/__init__.py
--rw-r--r--   0        0        0     1602 2024-03-31 11:44:06.292051 pyx2cscope-0.1.3/pyx2cscope/__main__.py
--rw-r--r--   0        0        0     1669 2024-03-31 11:44:06.292051 pyx2cscope-0.1.3/pyx2cscope/examples/auto_tuner.py
--rw-r--r--   0        0        0      646 2024-03-31 11:44:06.292051 pyx2cscope-0.1.3/pyx2cscope/examples/check_date.py
--rw-r--r--   0        0        0     1180 2024-03-31 11:44:06.292051 pyx2cscope-0.1.3/pyx2cscope/examples/exampleMCFG.py
--rw-r--r--   0        0        0      603 2024-03-31 11:44:06.292051 pyx2cscope-0.1.3/pyx2cscope/examples/example_new.py
--rw-r--r--   0        0        0     2723 2024-03-31 11:44:06.292051 pyx2cscope-0.1.3/pyx2cscope/examples/get_data_raw_blinkyTest.py
--rw-r--r--   0        0        0     3418 2024-03-31 11:44:06.292051 pyx2cscope-0.1.3/pyx2cscope/examples/live_scope.py
--rw-r--r--   0        0        0      312 2024-03-31 11:44:06.292051 pyx2cscope-0.1.3/pyx2cscope/examples/minimal_gui.py
--rw-r--r--   0        0        0     3298 2024-03-31 11:44:06.292051 pyx2cscope-0.1.3/pyx2cscope/examples/plotting_and_saving.py
--rw-r--r--   0        0        0     3713 2024-03-31 11:44:06.292051 pyx2cscope-0.1.3/pyx2cscope/examples/pyX2CScope_demo.py
--rw-r--r--   0        0        0      605 2024-03-31 11:44:06.292051 pyx2cscope-0.1.3/pyx2cscope/examples/simplest.py
--rw-r--r--   0        0        0        0 2024-03-31 11:44:06.292051 pyx2cscope-0.1.3/pyx2cscope/gui/__init__.py
--rw-r--r--   0        0        0     7188 2024-03-31 11:44:06.292051 pyx2cscope-0.1.3/pyx2cscope/gui/img/COM-Port.jpg
--rw-r--r--   0        0        0    72887 2024-03-31 11:44:06.292051 pyx2cscope-0.1.3/pyx2cscope/gui/img/MCHP.png
--rw-r--r--   0        0        0    63551 2024-03-31 11:44:06.292051 pyx2cscope-0.1.3/pyx2cscope/gui/img/Setting.jpg
--rw-r--r--   0        0        0        0 2024-03-31 11:44:06.292051 pyx2cscope-0.1.3/pyx2cscope/gui/img/__init__.py
--rw-r--r--   0        0        0    17008 2024-03-31 11:44:06.292051 pyx2cscope-0.1.3/pyx2cscope/gui/img/afterconnect.jpg
--rw-r--r--   0        0        0     4750 2024-03-31 11:44:06.292051 pyx2cscope-0.1.3/pyx2cscope/gui/img/microchip-technology-logo.png
--rw-r--r--   0        0        0    29732 2024-03-31 11:44:06.292051 pyx2cscope-0.1.3/pyx2cscope/gui/img/pyx2cscope.jpg
--rw-r--r--   0        0        0     7642 2024-03-31 11:44:06.292051 pyx2cscope-0.1.3/pyx2cscope/gui/img/refresh.png
--rw-r--r--   0        0        0        0 2024-03-31 11:44:06.292051 pyx2cscope-0.1.3/pyx2cscope/gui/scopeView/__init__.py
--rw-r--r--   0        0        0        0 2024-03-31 11:44:06.292051 pyx2cscope-0.1.3/pyx2cscope/gui/watchView/__init__.py
--rw-r--r--   0        0        0    33497 2024-03-31 11:44:06.292051 pyx2cscope-0.1.3/pyx2cscope/gui/watchView/minimal_gui.py
--rw-r--r--   0        0        0    16590 2024-03-31 11:44:06.292051 pyx2cscope-0.1.3/pyx2cscope/parser/Elf16Parser.py
--rw-r--r--   0        0        0    12555 2024-03-31 11:44:06.292051 pyx2cscope-0.1.3/pyx2cscope/parser/Elf32Parser.py
--rw-r--r--   0        0        0     3689 2024-03-31 11:44:06.296051 pyx2cscope-0.1.3/pyx2cscope/parser/Elf_Parser.py
--rw-r--r--   0        0        0        0 2024-03-31 11:44:06.296051 pyx2cscope-0.1.3/pyx2cscope/parser/__init__.py
--rw-r--r--   0        0        0     2185 2024-03-31 11:44:06.296051 pyx2cscope-0.1.3/pyx2cscope/parser/arraySupport.py
--rw-r--r--   0        0        0        0 2024-03-31 11:44:06.296051 pyx2cscope-0.1.3/pyx2cscope/variable/__init__.py
--rw-r--r--   0        0        0    12568 2024-03-31 11:44:06.296051 pyx2cscope-0.1.3/pyx2cscope/variable/variable.py
--rw-r--r--   0        0        0     4481 2024-03-31 11:44:06.296051 pyx2cscope-0.1.3/pyx2cscope/variable/variable_factory.py
--rw-r--r--   0        0        0    11832 2024-03-31 11:44:06.296051 pyx2cscope-0.1.3/pyx2cscope/xc2scope.py
--rw-r--r--   0        0        0     6480 1970-01-01 00:00:00.000000 pyx2cscope-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-05-13 10:59:21.125205 pyx2cscope-0.1.4/LICENSE
+-rw-r--r--   0        0        0     5218 2024-05-13 10:59:21.125205 pyx2cscope-0.1.4/README.md
+-rw-r--r--   0        0        0      780 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       91 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyx2cscope/__init__.py
+-rw-r--r--   0        0        0     1602 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyx2cscope/__main__.py
+-rw-r--r--   0        0        0     1669 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyx2cscope/examples/auto_tuner.py
+-rw-r--r--   0        0        0      646 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyx2cscope/examples/check_date.py
+-rw-r--r--   0        0        0     1180 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyx2cscope/examples/exampleMCFG.py
+-rw-r--r--   0        0        0      603 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyx2cscope/examples/example_new.py
+-rw-r--r--   0        0        0     2701 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyx2cscope/examples/get_data_raw_blinkyTest.py
+-rw-r--r--   0        0        0     2743 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyx2cscope/examples/live_scope.py
+-rw-r--r--   0        0        0      312 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyx2cscope/examples/minimal_gui.py
+-rw-r--r--   0        0        0     3298 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyx2cscope/examples/plotting_and_saving.py
+-rw-r--r--   0        0        0     3647 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyx2cscope/examples/pyX2CScope_demo.py
+-rw-r--r--   0        0        0      605 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyx2cscope/examples/simplest.py
+-rw-r--r--   0        0        0      759 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyx2cscope/examples/testingArray.py
+-rw-r--r--   0        0        0        0 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyx2cscope/gui/__init__.py
+-rw-r--r--   0        0        0     7188 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyx2cscope/gui/img/COM-Port.jpg
+-rw-r--r--   0        0        0    72887 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyx2cscope/gui/img/MCHP.png
+-rw-r--r--   0        0        0    63551 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyx2cscope/gui/img/Setting.jpg
+-rw-r--r--   0        0        0        0 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyx2cscope/gui/img/__init__.py
+-rw-r--r--   0        0        0    17008 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyx2cscope/gui/img/afterconnect.jpg
+-rw-r--r--   0        0        0     4750 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyx2cscope/gui/img/microchip-technology-logo.png
+-rw-r--r--   0        0        0    29732 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyx2cscope/gui/img/pyx2cscope.jpg
+-rw-r--r--   0        0        0     7642 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyx2cscope/gui/img/refresh.png
+-rw-r--r--   0        0        0        0 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyx2cscope/gui/scopeView/__init__.py
+-rw-r--r--   0        0        0     2045 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyx2cscope/gui/scopeView/scopeView_GUI.py
+-rw-r--r--   0        0        0        0 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyx2cscope/gui/watchView/__init__.py
+-rw-r--r--   0        0        0    32919 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyx2cscope/gui/watchView/minimal_gui.py
+-rw-r--r--   0        0        0    18062 2024-05-13 10:59:21.157204 pyx2cscope-0.1.4/pyx2cscope/parser/Elf16Parser.py
+-rw-r--r--   0        0        0    12138 2024-05-13 10:59:21.161204 pyx2cscope-0.1.4/pyx2cscope/parser/Elf32Parser.py
+-rw-r--r--   0        0        0     3741 2024-05-13 10:59:21.161204 pyx2cscope-0.1.4/pyx2cscope/parser/Elf_Parser.py
+-rw-r--r--   0        0        0     3358 2024-05-13 10:59:21.161204 pyx2cscope-0.1.4/pyx2cscope/parser/TestarraySupport.py
+-rw-r--r--   0        0        0        0 2024-05-13 10:59:21.161204 pyx2cscope-0.1.4/pyx2cscope/parser/__init__.py
+-rw-r--r--   0        0        0     1933 2024-05-13 10:59:21.161204 pyx2cscope-0.1.4/pyx2cscope/parser/arraySupport.py
+-rw-r--r--   0        0        0        0 2024-05-13 10:59:21.161204 pyx2cscope-0.1.4/pyx2cscope/variable/__init__.py
+-rw-r--r--   0        0        0    15453 2024-05-13 10:59:21.161204 pyx2cscope-0.1.4/pyx2cscope/variable/variable.py
+-rw-r--r--   0        0        0     4564 2024-05-13 10:59:21.161204 pyx2cscope-0.1.4/pyx2cscope/variable/variable_factory.py
+-rw-r--r--   0        0        0    12377 2024-05-13 10:59:21.161204 pyx2cscope-0.1.4/pyx2cscope/xc2scope.py
+-rw-r--r--   0        0        0     6480 1970-01-01 00:00:00.000000 pyx2cscope-0.1.4/PKG-INFO
```

### Comparing `pyx2cscope-0.1.3/LICENSE` & `pyx2cscope-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyx2cscope-0.1.3/README.md` & `pyx2cscope-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyx2cscope-0.1.3/pyproject.toml` & `pyx2cscope-0.1.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
+[tool.black]
+line-length = 120
+
 [tool.poetry]
 name = "pyx2cscope"
-version = "0.1.3"
+version = "0.1.4"
 description = "python implementation of X2Cscope"
 authors = [
   "Yash Agarwal <yash.agarwal@microchip.com>",
   "Edras Pacola",
   "Christoph Baumgartner",
   "Mark Wendler",
 ]
```

### Comparing `pyx2cscope-0.1.3/pyx2cscope/__main__.py` & `pyx2cscope-0.1.4/pyx2cscope/__main__.py`

 * *Files identical despite different names*

### Comparing `pyx2cscope-0.1.3/pyx2cscope/examples/auto_tuner.py` & `pyx2cscope-0.1.4/pyx2cscope/examples/auto_tuner.py`

 * *Files identical despite different names*

### Comparing `pyx2cscope-0.1.3/pyx2cscope/examples/check_date.py` & `pyx2cscope-0.1.4/pyx2cscope/examples/check_date.py`

 * *Files identical despite different names*

### Comparing `pyx2cscope-0.1.3/pyx2cscope/examples/exampleMCFG.py` & `pyx2cscope-0.1.4/pyx2cscope/examples/exampleMCFG.py`

 * *Files identical despite different names*

### Comparing `pyx2cscope-0.1.3/pyx2cscope/examples/example_new.py` & `pyx2cscope-0.1.4/pyx2cscope/examples/example_new.py`

 * *Files identical despite different names*

### Comparing `pyx2cscope-0.1.3/pyx2cscope/examples/get_data_raw_blinkyTest.py` & `pyx2cscope-0.1.4/pyx2cscope/examples/get_data_raw_blinkyTest.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,15 @@
     return set_led_state(value, variable, False)
 
 
 def example():
     try:
         # Initialize serial communication and other setup code...
 
-        SFR_LED = x2cscope.get_variable_raw(
-            3702, "int", "sfr"
-        )  # LATE address from data sheet 3702
+        SFR_LED = x2cscope.get_variable_raw(3702, "int", "sfr")  # LATE address from data sheet 3702
 
         # Get the initial LED state from SFR_LED or any other source
         initial_led_state = SFR_LED.get_value()
         logging.debug("initial value: %s", initial_led_state)
         while 1:
             #########################
             # SET LED1 and LED2 High
```

### Comparing `pyx2cscope-0.1.3/pyx2cscope/examples/live_scope.py` & `pyx2cscope-0.1.4/pyx2cscope/examples/live_scope.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,100 +1,93 @@
+import csv
 import logging
+import time
 
 import matplotlib.pyplot as plt
-from matplotlib.animation import FuncAnimation
 
 from pyx2cscope.xc2scope import X2CScope
 
-# Set up logging This sets up the logging system to capture information and errors, storing them in a log file with
-# the same name as this script.
+# Set up logging
 logging.basicConfig(
     level=logging.INFO,
     filename=__file__ + ".log",
 )
 
-# X2C Scope Setup Initialize the X2C Scope for real-time data acquisition from a microcontroller. Specify the COM
-# port and path to the ELF file.
-elf_file = (
-    r"C:\_DESKTOP\_Projects\Motorbench_Projects\motorbench_FOC_PLL_PIC33CK256mp508_MCLV2"
-    r"\ZSMT_dsPIC33CK_MCLV_48_300.X\dist\default\production\ZSMT_dsPIC33CK_MCLV_48_300_Future.X.production.elf"
-)
-x2cScope = X2CScope(port="COM16", elf_file=elf_file)
+# X2C Scope Set up
+elf_file = r"C:\_DESKTOP\_Projects\Motorbench_Projects\motorbench_FOC_PLL_PIC33CK256mp508_MCLV2\ZSMT_dsPIC33CK_MCLV_48_300.X\dist\default\production\ZSMT_dsPIC33CK_MCLV_48_300.X.production.elf"
+x2cScope = X2CScope(port="COM14", elf_file=elf_file)
 
-# Initialize Variables for Monitoring
-# Define the variables that will be monitored and visualized in real-time.
+# Define variables
 variables = [
-    x2cScope.get_variable("motor.idq.q"),
-    x2cScope.get_variable("motor.vabc.a"),
-    x2cScope.get_variable("motor.vabc.b"),
-    x2cScope.get_variable("motor.vabc.c"),
-    x2cScope.get_variable("motor.apiData.velocityMeasured"),
+    "motor.idq.q",
+    "motor.vabc.a",
+    "motor.vabc.b",
+    "motor.vabc.c",
+    "motor.apiData.velocityMeasured",
 ]
 
-# Adding variables to scope's monitoring channels
-for variable in variables:
-    x2cScope.add_scope_channel(variable)
-
-# Initialize Data Storage
-# A dictionary to store the incoming data for each variable.
-data_storage = {var: [] for var in variables}
-
-# Window Size for Live Plot
-# Specifies the number of data points to display in the live plot at any given time.
-window_size = 250
-
-
-def update_plot(frame):
-    """
-    Update Plot Function
-    This function is called periodically by the animation framework.
-    It fetches new data from the scope and updates the live plot.
-    """
+for var in variables:
+    x2cScope.add_scope_channel(x2cScope.get_variable(var))
+
+x2cScope.set_sample_time(1)
+
+# Create the plot
+plt.ion()  # Turn on interactive mode
+fig, ax = plt.subplots()
+
+# Main loop
+sample_count = 0
+max_sample = 100  # Increase the number of samples if needed
+
+while sample_count < max_sample:
     try:
-        # Check if new scope data is available
         if x2cScope.is_scope_data_ready():
+            sample_count += 1
             logging.info("Scope data is ready.")
 
-            # Process and store new data
-            scope_data = x2cScope.get_scope_channel_data(valid_data=False)
-            for variable, data in scope_data.items():
-                variable_name = str(variable)  # Convert variable to a string identifier
-                data_storage[variable_name].extend(data)
+            data_storage = {}
+            for channel, data in x2cScope.get_scope_channel_data(valid_data=False).items():
+                data_storage[channel] = data
+
+            ax.clear()
+            for channel, data in data_storage.items():
+                # Assuming data is sampled at 1 kHz, adjust as needed
+                time_values = [i * 0.001 for i in range(len(data))]  # milliseconds
+                # time_values = [i * 0.000001 for i in range(len(data))]  # microseconds
+                ax.plot(time_values, data, label=f"Channel {channel}")
+
+            ax.set_xlabel("Time (ms)")  # Change axis label accordingly
+            ax.set_ylabel("Value")
+            ax.set_title("Live Plot of Byte Data")
+            ax.legend()
+
+            plt.pause(0.001)  # Add a short pause to update the plot
 
-            # Request new data from the scope
+            if sample_count >= max_sample:
+                break
             x2cScope.request_scope_data()
 
     except Exception as e:
-        logging.error(f"Error in update_plot: {str(e)}")
+        logging.error(f"Error in main loop: {str(e)}")
+        break
 
-    # Clear the current plot for fresh drawing
-    plt.clf()
+    time.sleep(0.1)
 
-    # Determine the current maximum index for x-axis
-    current_index = max(len(data) for data in data_storage.values())
+plt.ioff()  # Turn off interactive mode after the loop
+plt.show()
 
-    # Plot data for each channel within the moving window
-    for variable_name, data in data_storage.items():
-        if data:
-            start_index = max(0, current_index - window_size)
-            end_index = current_index
-            plt.plot(
-                range(start_index, end_index), data[-window_size:], label=variable_name
-            )
-
-    # Adjust plot settings for the moving window effect
-    plt.xlim(current_index - window_size, current_index)
-    plt.xlabel("Data Index")
-    plt.ylabel("Value")
-    plt.title("Live Plot of Byte Data")
-    plt.legend(loc="upper right")
-    plt.draw()
-
-
-# Live Plot Setup
-# Initialize interactive mode for live updating and create a figure for the plot.
-plt.ion()
-fig = plt.figure()
-ani = FuncAnimation(fig, update_plot, interval=100, cache_frame_data=False)
+logging.info("Data collection complete.")
+
+# Data Storage
+csv_file_path = "scope_data.csv"
+max_length = max(len(data) for data in data_storage.values())
+
+with open(csv_file_path, mode="w", newline="") as file:
+    writer = csv.DictWriter(file, fieldnames=data_storage.keys())
+    writer.writeheader()
+    for i in range(max_length):
+        row = {
+            channel: (data_storage[channel][i] if i < len(data_storage[channel]) else None) for channel in data_storage
+        }
+        writer.writerow(row)
 
-# Display the live plot
-plt.show(block=True)
+logging.info(f"Data saved in {csv_file_path}")
```

### Comparing `pyx2cscope-0.1.3/pyx2cscope/examples/plotting_and_saving.py` & `pyx2cscope-0.1.4/pyx2cscope/examples/plotting_and_saving.py`

 * *Files identical despite different names*

### Comparing `pyx2cscope-0.1.3/pyx2cscope/examples/pyX2CScope_demo.py` & `pyx2cscope-0.1.4/pyx2cscope/examples/pyX2CScope_demo.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,17 +62,15 @@
 while sample_count < max_sample:
     try:
         if x2cScope.is_scope_data_ready():
             sample_count += 1
             logging.info("Scope data is ready.")
 
             # Process and store data
-            for channel, data in x2cScope.get_scope_channel_data(
-                valid_data=False
-            ).items():
+            for channel, data in x2cScope.get_scope_channel_data(valid_data=False).items():
                 if channel not in data_storage:
                     data_storage[channel] = []
                 data_storage[channel].extend(data)
 
             if sample_count >= max_sample:
                 break
             x2cScope.request_scope_data()
@@ -100,15 +98,12 @@
 max_length = max(len(data) for data in data_storage.values())
 
 with open(csv_file_path, mode="w", newline="") as file:
     writer = csv.DictWriter(file, fieldnames=data_storage.keys())
     writer.writeheader()
     for i in range(max_length):
         row = {
-            channel: data_storage[channel][i]
-            if i < len(data_storage[channel])
-            else None
-            for channel in data_storage
+            channel: data_storage[channel][i] if i < len(data_storage[channel]) else None for channel in data_storage
         }
         writer.writerow(row)
 
 logging.info(f"Data saved in {csv_file_path}")
```

### Comparing `pyx2cscope-0.1.3/pyx2cscope/examples/simplest.py` & `pyx2cscope-0.1.4/pyx2cscope/examples/simplest.py`

 * *Files identical despite different names*

### Comparing `pyx2cscope-0.1.3/pyx2cscope/gui/img/COM-Port.jpg` & `pyx2cscope-0.1.4/pyx2cscope/gui/img/COM-Port.jpg`

 * *Files identical despite different names*

### Comparing `pyx2cscope-0.1.3/pyx2cscope/gui/img/MCHP.png` & `pyx2cscope-0.1.4/pyx2cscope/gui/img/MCHP.png`

 * *Files identical despite different names*

### Comparing `pyx2cscope-0.1.3/pyx2cscope/gui/img/Setting.jpg` & `pyx2cscope-0.1.4/pyx2cscope/gui/img/Setting.jpg`

 * *Files identical despite different names*

### Comparing `pyx2cscope-0.1.3/pyx2cscope/gui/img/afterconnect.jpg` & `pyx2cscope-0.1.4/pyx2cscope/gui/img/afterconnect.jpg`

 * *Files identical despite different names*

### Comparing `pyx2cscope-0.1.3/pyx2cscope/gui/img/microchip-technology-logo.png` & `pyx2cscope-0.1.4/pyx2cscope/gui/img/microchip-technology-logo.png`

 * *Files identical despite different names*

### Comparing `pyx2cscope-0.1.3/pyx2cscope/gui/img/pyx2cscope.jpg` & `pyx2cscope-0.1.4/pyx2cscope/gui/img/pyx2cscope.jpg`

 * *Files identical despite different names*

### Comparing `pyx2cscope-0.1.3/pyx2cscope/gui/img/refresh.png` & `pyx2cscope-0.1.4/pyx2cscope/gui/img/refresh.png`

 * *Files identical despite different names*

### Comparing `pyx2cscope-0.1.3/pyx2cscope/gui/watchView/minimal_gui.py` & `pyx2cscope-0.1.4/pyx2cscope/gui/watchView/minimal_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,28 +324,20 @@
         self.layout.addLayout(baud_layout, 2, 0)
         self.layout.addWidget(self.select_file_button, 3, 0)
         self.layout.addLayout(self.box_layout, 4, 0)
         self.layout.addLayout(self.grid_layout, 5, 0)
         self.layout.addWidget(self.plot_button, 6, 0)
         # self.grid_layout.addWidget(self.slider_var2, 8, 0, 1, 6)
 
-        for timer, combo_box, value_var in zip(
-            self.timer_list, self.combo_boxes, self.Value_var_boxes
-        ):
-            timer.timeout.connect(
-                lambda cb=combo_box, v_var=value_var: self.handle_var_update(
-                    cb.currentText(), v_var
-                )
-            )
+        for timer, combo_box, value_var in zip(self.timer_list, self.combo_boxes, self.Value_var_boxes):
+            timer.timeout.connect(lambda cb=combo_box, v_var=value_var: self.handle_var_update(cb.currentText(), v_var))
 
         for combo_box, value_var in zip(self.combo_boxes, self.Value_var_boxes):
             combo_box.currentIndexChanged.connect(
-                lambda cb=combo_box, v_var=value_var: self.handle_variable_getram(
-                    self.VariableList[cb], v_var
-                )
+                lambda cb=combo_box, v_var=value_var: self.handle_variable_getram(self.VariableList[cb], v_var)
             )
 
         for (
             combo_box,
             value_var,
         ) in zip(
             self.combo_boxes,
@@ -413,17 +405,15 @@
                     self.update_scaled_value(sc_edit, v_edit, scd_edit, off_edit)
 
                 return on_editing_finished
 
             scaling.editingFinished.connect(connect_editing_finished())
 
         for timer, live_var in zip(self.timer_list, self.live_checkboxes):
-            live_var.stateChanged.connect(
-                lambda state, lv=live_var, tm=timer: self.var_live(lv, tm)
-            )
+            live_var.stateChanged.connect(lambda state, lv=live_var, tm=timer: self.var_live(lv, tm))
 
         # OffsetSet.
 
         for (
             scaling,
             value_var,
             scaled_value,
@@ -520,17 +510,15 @@
         """
         Updates the data for plotting.
         """
         try:
             timestamp = datetime.now()
             if len(self.plot_data) > 0:
                 last_timestamp = self.plot_data[-1][0]
-                time_diff = (
-                    timestamp - last_timestamp
-                ).total_seconds() * 1000  # to convert time in ms.
+                time_diff = (timestamp - last_timestamp).total_seconds() * 1000  # to convert time in ms.
             else:
                 time_diff = 0
             self.plot_data.append(
                 (
                     timestamp,
                     time_diff,
                     float(self.ScaledValue_var1.text()),
@@ -556,21 +544,17 @@
 
             data = np.array(self.plot_data).T
             time_diffs = data[1]
             values = data[2:7]
             self.ax.clear()
             start = time.time()
 
-            for value, combo_box, plot_var in zip(
-                values, self.combo_boxes, self.plot_checkboxes
-            ):
+            for value, combo_box, plot_var in zip(values, self.combo_boxes, self.plot_checkboxes):
                 if plot_var.isChecked() and combo_box.currentIndex() != 0:
-                    self.ax.plot(
-                        np.cumsum(time_diffs), value, label=combo_box.currentText()
-                    )
+                    self.ax.plot(np.cumsum(time_diffs), value, label=combo_box.currentText())
 
             self.ax.set_xlabel("Time (ms)")
             self.ax.set_ylabel("Value")
             self.ax.set_title("Live Plot")
             self.ax.legend(loc="upper right")
             end = time.time()
             logging.debug(end - start)
@@ -586,31 +570,21 @@
         try:
             if not self.plot_data:
                 return
 
             def initialize_plot():
                 self.fig, self.ax = plt.subplots()
 
-                self.ani = FuncAnimation(
-                    self.fig, self.update_plot, interval=1, cache_frame_data=False
-                )
+                self.ani = FuncAnimation(self.fig, self.update_plot, interval=1, cache_frame_data=False)
                 logging.debug(self.ani)
                 plt.xticks(rotation=45)
-                self.ax.axhline(
-                    0, color="black", linewidth=0.5
-                )  # Reference line at y=0
-                self.ax.axvline(
-                    0, color="black", linewidth=0.5
-                )  # Reference line at x=0
-                plt.subplots_adjust(
-                    bottom=0.15, left=0.15
-                )  # Adjust plot window position
-                plt.show(
-                    block=False
-                )  # Use block=False to prevent the GUI from freezing
+                self.ax.axhline(0, color="black", linewidth=0.5)  # Reference line at y=0
+                self.ax.axvline(0, color="black", linewidth=0.5)  # Reference line at x=0
+                plt.subplots_adjust(bottom=0.15, left=0.15)  # Adjust plot window position
+                plt.show(block=False)  # Use block=False to prevent the GUI from freezing
 
             if self.plot_window_open:
                 if self.fig is not None and plt.fignum_exists(self.fig.number):
                     # If the plot window is still open, update the plot and restart the animation with the new interval
                     self.update_plot(0)
                     self.ani.event_source.stop()
                     self.ani.event_source.start(self.timerValue)
@@ -664,20 +638,16 @@
             value_var (QLineEdit): The input field to display the updated value.
         """
         try:
             if counter is not None:
                 counter = self.x2cscope.get_variable(counter)
                 value = counter.get_value()
                 value_var.setText(str(value))
-                if (
-                    value_var == self.Value_var1
-                ):  # Check if it's Variable 1 being updated
-                    self.slider_var1.setValue(
-                        int(value)
-                    )  # Set slider to the updated value
+                if value_var == self.Value_var1:  # Check if it's Variable 1 being updated
+                    self.slider_var1.setValue(int(value))  # Set slider to the updated value
                 self.plot_data_update()
         except Exception as e:
             error_message = f"Error: {e}"
             logging.error(error_message)
             self.handle_error(error_message)
 
     def slider_var1_changed(self, value):
@@ -887,17 +857,15 @@
             # Disconnect first if already connected
             if self.ser is not None and self.ser.is_open:
                 self.disconnect_serial()
 
             port = self.port_combo.currentText()
             baud_rate = int(self.baud_combo.currentText())
 
-            self.x2cscope = X2CScope(
-                port=port, elf_file=self.file_path, baud_rate=baud_rate
-            )
+            self.x2cscope = X2CScope(port=port, elf_file=self.file_path, baud_rate=baud_rate)
             self.ser = self.x2cscope.interface
             self.VariableList = self.x2cscope.list_variables()
             if self.VariableList:
                 self.VariableList.insert(0, "None")
             else:
                 return
             self.refresh_combo_box()
```

### Comparing `pyx2cscope-0.1.3/pyx2cscope/parser/Elf16Parser.py` & `pyx2cscope-0.1.4/pyx2cscope/parser/Elf16Parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         Args:
         elf_path (str): Path to the input ELF file.
 
         Raises:
         ValueError: If the XC16 compiler is not found on the system path.
         """
         self.xc16_read_elf_path = which("xc16-readelf")
-        if not os.path.exists(self.xc16_read_elf_path):
+        if self.xc16_read_elf_path is None or not os.path.exists(self.xc16_read_elf_path):
             raise ValueError("XC16 compiler not found. Is it listed on PATH?")
         super().__init__(elf_path)
         self.tree_string = None
         self.next_line = None
 
     def _parse_cu_attributes(self):
         """
@@ -74,17 +74,15 @@
         while "DW_AT" in self.next_line:
             values = self.next_line.split(":")
 
             key = values[0].strip()
             value = ":".join(values[1:]).strip()
             if key == "DW_AT_name":
                 # Remove the indirect string part and leading space
-                value = re.sub(
-                    r"\(indirect string, offset: 0x[0-9a-fA-F]+\):", "", value
-                ).strip()
+                value = re.sub(r"\(indirect string, offset: 0x[0-9a-fA-F]+\):", "", value).strip()
             value = int(value[1:-1], 16) if key == "DW_AT_type" else value
 
             members.update({key: value})
             self.next_line = next(self.tree_string)
         return members
 
     def _parse_cu_elements(self):
@@ -130,16 +128,15 @@
         command = [self.xc16_read_elf_path, "-w", self.elf_path]
 
         # Execute the command and capture the output
         try:
             output = subprocess.check_output(command, universal_newlines=True)
             self._parse_tree(output)
         except subprocess.CalledProcessError as e:
-            logging.error(f"Error executing xc16-readelf.exe: {e.output}")
-            return
+            raise Exception("Error loading ELF file: {}".format(self.elf_path))
 
     @staticmethod
     def _get_structure_member_offset(location: str):
         """
         Extract the offset of a structure member from its location string.
 
         Args:
@@ -170,48 +167,43 @@
             tuple: A tuple containing the compilation unit and its sibling
         """
         cu = None
         cu_sibling = None
         for cu_offset, cu in self.dwarf_info.items():
             if not (cu_offset < structure_die["offset"] < (cu_offset + cu["length"])):
                 continue
-            cu_sibling = int(
-                cu["elements"][structure_die["offset"]]["DW_AT_sibling"][1:-1], 16
-            )
+            cu_sibling = int(cu["elements"][structure_die["offset"]]["DW_AT_sibling"][1:-1], 16)
             break
         return cu, cu_sibling
 
-    def _get_member_from_nested_members(
-        self, parent_address, nested_member, cu_structure
-    ):
+    def _get_member_from_nested_members(self, parent_address, nested_member, cu_structure):
         """
         Extract information about a structure member from nested members.
 
         Args:
             parent_address (int): Address of the parent structure.
             nested_member (tuple): Nested structure member information.
             cu_structure (dict): DWARF DIE representing a structure.
 
         Returns:
             dict: Dictionary containing information about the structure member.
         """
         member_info = nested_member[1]
         member_address = cu_structure["DW_AT_data_member_location"]
         member_address_offset = (
-            parent_address
-            + self._get_structure_member_offset(member_address)
-            + member_info["address_offset"]
+            parent_address + self._get_structure_member_offset(member_address) + member_info["address_offset"]
         )
         member = {
             cu_structure["DW_AT_name"]
             + "."
             + nested_member[0]: {
                 "address_offset": member_address_offset,
                 "type": member_info["type"],
                 "byte_size": member_info["byte_size"],
+                "array_size": member_info["array_size"],
             }
         }
         return member
 
     def _get_structure_members(self, structure_die, parent_address=0):
         """
         Recursively get all members of a structure.
@@ -235,36 +227,33 @@
             if cu_offset == cu_sibling:
                 break
 
             end_die = self._get_end_die(cu_structure_member)
             try:
                 if end_die["tag"] == "DW_TAG_structure_type":
                     # Handle nested structures recursively
-                    nested_members = self._get_structure_members(
-                        end_die, parent_address
-                    )
+                    nested_members = self._get_structure_members(end_die, parent_address)
                     for nested_member in nested_members.items():
                         members.update(
-                            self._get_member_from_nested_members(
-                                parent_address, nested_member, cu_structure_member
-                            )
+                            self._get_member_from_nested_members(parent_address, nested_member, cu_structure_member)
                         )
                 else:
                     address = parent_address + self._get_structure_member_offset(
                         cu_structure_member["DW_AT_data_member_location"]
                     )
                     member = {
                         cu_structure_member["DW_AT_name"]: {
                             "address_offset": address,
                             "type": end_die["DW_AT_name"],
                             "byte_size": end_die["DW_AT_byte_size"],
+                            "array_size": self.calculate_array_size(array_die=cu_structure_member),
                         }
                     }
                     members.update(member)
-            except Exception:
+            except Exception as e:
                 # there are some missing values
                 # this will be addressed in future versions
                 continue
         return members
 
     @staticmethod
     def _get_address_check(location: str) -> int:
@@ -382,16 +371,19 @@
                 for member, member_info in members.items():
                     member_name = die["DW_AT_name"] + "." + member
                     variable_data = VariableInfo(
                         name=member_name,
                         byte_size=member_info.get("byte_size"),
                         type=member_info.get("type"),
                         address=address + (member_info.get("address_offset")),
+                        array_size=member_info.get("array_size"),
                     )
                     self.variable_map[member_name] = variable_data
+                    # Reset array attributes for each variable
+                    self.array_size = 0
             return True
         return False
 
     def _get_end_die(self, start_die):
         """
         Get the end die of a given die.
 
@@ -408,17 +400,44 @@
             "DW_TAG_pointer_type",
             "DW_TAG_structure_type",
         ]:
             return start_die
         if "DW_AT_type" in start_die:
             type_offset = start_die["DW_AT_type"]
             type_die = self._get_dwarf_die_by_offset(type_offset)
+            #     if type_die["tag"] == "DW_TAG_array_type":
+            #         print(start_die)
+            #         self.array_size = self.calculate_array_size(type_die)
             return self._get_end_die(type_die)
         return None
 
+    def _get_next_die_by_offset(self, offset):
+        take_next = False
+        for cu_offset, cu in self.dwarf_info.items():
+            for die_offset, die in cu["elements"].items():
+                if take_next:
+                    return die
+                if die_offset == offset:
+                    take_next = True
+
+    def calculate_array_size(self, array_die):
+        type_offset = array_die["DW_AT_type"]
+        type_die = self._get_dwarf_die_by_offset(type_offset)
+        if type_die["tag"] == "DW_TAG_array_type":
+            # Retrieve the array type DIE
+            die = self._get_next_die_by_offset(type_die["offset"])
+            try:
+                upper_bound = int(die.get("DW_AT_upper_bound"))
+
+                return upper_bound + 1  # Assuming 0-based indexing
+            except Exception as e:
+                print(array_die)
+        else:
+            return 0
+
     def _get_dwarf_die_by_offset(self, offset):
         """
         Get a DWARF die by offset.
 
         Args:
             offset: The offset of the die.
 
@@ -435,28 +454,28 @@
         self.variable_map.clear()
         for cu_offset, cu in self.dwarf_info.items():
             for die_offset, die in cu["elements"].items():
                 end_die = self._locate_tag_variable_end_die(die)
                 if end_die is None:
                     continue
                 address = self._get_address_location(die.get("DW_AT_location"))
-                if not self._check_for_pointer_tag(
+                if not self._check_for_pointer_tag(die, end_die, address) and not self._check_for_structure_tag(
                     die, end_die, address
-                ) and not self._check_for_structure_tag(die, end_die, address):
+                ):
                     variable_data = VariableInfo(
                         name=die["DW_AT_name"],
                         byte_size=end_die["DW_AT_byte_size"],
                         type=end_die["DW_AT_name"],
                         address=address,
+                        array_size=self.calculate_array_size(die),
                     )
                     self.variable_map[die["DW_AT_name"]] = variable_data
         return self.variable_map
 
 
 if __name__ == "__main__":
-    elf_file = (
-        r"C:\Users\M71906\MPLABXProjects\MotorControl\dsPIC33-LVMC-MB-FOC-Sensorless.X\dist\default\production"
-        r"\dsPIC33-LVMC-MB-FOC-Sensorless.X.production.elf"
-    )
+    # elf_file = r"C:\_DESKTOP\_Projects\Motorbench_Projects\ZSMT-42BLF02-MCLV2-33ck256mp508.X\dist\default\production\ZSMT-42BLF02-MCLV2-33ck256mp508.X.production.elf"
+    elf_file = r"C:\_DESKTOP\_Projects\Motorbench_Projects\motorbench_FOC_PLL_PIC33CK256mp508_MCLV2\ZSMT_dsPIC33CK_MCLV_48_300.X\dist\default\production\ZSMT_dsPIC33CK_MCLV_48_300.X.production.elf"
     logging.basicConfig(level=logging.DEBUG)  # Set the desired logging level and stream
     elf_reader = Elf16Parser(elf_file)
     variable_map = elf_reader.map_variables()
+    print(variable_map)
```

### Comparing `pyx2cscope-0.1.3/pyx2cscope/parser/Elf32Parser.py` & `pyx2cscope-0.1.4/pyx2cscope/parser/Elf32Parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 class Elf32Parser(ElfParser):
     """
     Class for parsing ELF files compatible with 32-bit architectures.
     """
 
     def _get_structure_members_recursive(
         self,
+        type_die,
         die,
         parent_name: str,
         prev_address_offset=0,
     ):
         """
         Recursively gets structure members from a DWARF DIE.
 
@@ -25,32 +26,27 @@
             prev_address_offset (int): Address offset from the parent.
 
         Returns:
             Tuple[dict, int]: Dictionary of members and their offset.
         """
         members = {}
         for child_die in die.iter_children():
-            if (
-                child_die.tag == "DW_TAG_member"
-                or child_die.tag == "DW_TAG_pointer_type"
-            ):
+            if child_die.tag == "DW_TAG_member" or child_die.tag == "DW_TAG_pointer_type":
                 member = {}
                 member_name = ""
                 name_attr = child_die.attributes.get("DW_AT_name")
                 if name_attr:
                     member_name = parent_name + "." + name_attr.value.decode("utf-8")
                 type_attr = child_die.attributes.get("DW_AT_type")
                 if type_attr:
                     type_offset = type_attr.value + child_die.cu.cu_offset
                     try:
                         member_type = self._get_member_type(type_offset)
                         offset_value_from_member_address = int(
-                            child_die.attributes.get(
-                                "DW_AT_data_member_location"
-                            ).value[1]
+                            child_die.attributes.get("DW_AT_data_member_location").value[1]
                         )
                         nested_die = self._get_end_die(child_die)
                         if nested_die.tag == "DW_TAG_structure_type":
                             (
                                 nested_members,
                                 nested_offset,
                             ) = self._get_structure_members_recursive(
@@ -59,51 +55,47 @@
                                 prev_address_offset + offset_value_from_member_address,
                             )
                             if nested_members:
                                 members.update(nested_members)
                         else:
                             member["type"] = member_type["name"]
                             member["byte_size"] = member_type["byte_size"]
-                            member["address_offset"] = (
-                                prev_address_offset + offset_value_from_member_address
-                            )
+                            member["address_offset"] = prev_address_offset + offset_value_from_member_address
+                            member["array_size"] = self._get_array_length(type_die)
                             members[member_name] = member
                     except Exception as e:
                         logging.error("exception", e)
                         # Handle missing fields
                         # TODO This will be handled in future versions
                         continue
 
                     # If the member type is a structure or class, recurse into it
         return members, prev_address_offset
 
-    def _get_structure_members(self, structure_die, var_name):
+    def _get_structure_members(self, type_die, structure_die, var_name):
         """
         Retrieves structure members from a DWARF DIE.
 
         Args:
             structure_die: The DIE representing the structure.
             var_name (str): Name of the variable.
 
         Returns:
             dict: Dictionary of structure members.
         """
         prev_address_offset = 0
-        return self._get_structure_members_recursive(
-            structure_die, var_name, prev_address_offset
-        )
+        return self._get_structure_members_recursive(type_die, structure_die, var_name, prev_address_offset)
 
-    def _processing_end_die(self, end_die):
+    def _processing_end_die(self, type_die, end_die):
         """
         Processes the end DIE of a tag to extract variable information.
 
         Args:
             end_die: The end DIE of the tag.
         """
-        print(end_die)
         try:
             if self.die_variable.attributes.get("DW_AT_location"):
                 data = list(self.die_variable.attributes["DW_AT_location"].value)[1:]
                 self.address = int.from_bytes(bytes(data), byteorder="little")
             else:
                 address = None
         except Exception as e:
@@ -123,22 +115,24 @@
                 name=self.var_name,
                 byte_size=end_die.attributes["DW_AT_byte_size"].value,
                 type=type_name,
                 address=self.address,
             )
 
         elif end_die.tag == "DW_TAG_structure_type":
-            members = self._get_structure_members(end_die, self.var_name)[0]
+            members = self._get_structure_members(type_die, end_die, self.var_name)[0]
             for member_name, member_data in members.items():
                 self.variable_map[member_name] = VariableInfo(
                     name=member_name,
                     byte_size=member_data["byte_size"],
                     type=member_data["type"],
                     address=self.address + member_data["address_offset"],
+                    array_size=member_data["array_size"],
                 )
+                self.array_size = 0
 
         else:
             self.variable_map[self.var_name] = VariableInfo(
                 name=self.var_name,
                 byte_size=end_die.attributes["DW_AT_byte_size"].value,
                 type=end_die.attributes["DW_AT_name"].value.decode("utf-8"),
                 address=self.address,
@@ -150,21 +144,21 @@
 
         Args:
             type_die: The DIE representing the array type.
 
         Returns:
             int: Length of the array.
         """
+        # print(type_die)
+
         for child in type_die.iter_children():
             if child.tag == "DW_TAG_subrange_type":
                 array_length_attr = child.attributes.get("DW_AT_upper_bound")
                 if array_length_attr:
-                    array_length = (
-                        array_length_attr.value + 1
-                    )  # upper_bound is 0-indexed
+                    array_length = array_length_attr.value + 1  # upper_bound is 0-indexed
                     return array_length
 
     def _load_elf_file(self):
         try:
             with open(self.elf_path, "rb") as stream:
                 self.elf_file = ELFFile(stream)
                 self.dwarf_info = self.elf_file.get_dwarf_info()
@@ -200,17 +194,15 @@
         """
         valid_words = [
             "DW_TAG_base_type",
             "DW_TAG_pointer_type",
             "DW_TAG_structure_type",
         ]
         while not any(current_die.tag == word for word in valid_words):
-            ref_addr = (
-                current_die.attributes["DW_AT_type"].value + current_die.cu.cu_offset
-            )
+            ref_addr = current_die.attributes["DW_AT_type"].value + current_die.cu.cu_offset
             current_die = self.dwarf_info.get_DIE_from_refaddr(ref_addr)
         return current_die
 
     def _get_member_type(self, type_offset):
         """
         Retrieve the type information from DWARF given a type offset.
 
@@ -244,74 +236,61 @@
             root_die = compilation_unit.iter_DIEs()
             tag_variables = filter(lambda die: die.tag == "DW_TAG_variable", root_die)
 
             for self.die_variable in tag_variables:
                 #  the structure which has address in specific DIE.
                 if "DW_AT_specification" in self.die_variable.attributes:
                     spec_ref_addr = (
-                        self.die_variable.attributes["DW_AT_specification"].value
-                        + self.die_variable.cu.cu_offset
+                        self.die_variable.attributes["DW_AT_specification"].value + self.die_variable.cu.cu_offset
                     )
                     spec_die = self.dwarf_info.get_DIE_from_refaddr(spec_ref_addr)
 
                     if self.die_variable.attributes.get("DW_AT_location"):
-                        address_set = list(
-                            self.die_variable.attributes["DW_AT_location"].value
-                        )[1:]
-                        self.address = int.from_bytes(
-                            bytes(address_set), byteorder="little"
-                        )
+                        address_set = list(self.die_variable.attributes["DW_AT_location"].value)[1:]
+                        self.address = int.from_bytes(bytes(address_set), byteorder="little")
 
                     if spec_die.tag == "DW_TAG_variable" and self.address is not None:
                         self.die_variable = spec_die
-                        self.var_name = self.die_variable.attributes.get(
-                            "DW_AT_name"
-                        ).value.decode("utf-8")
+                        self.var_name = self.die_variable.attributes.get("DW_AT_name").value.decode("utf-8")
                     else:
                         continue
 
                 elif (
                     self.die_variable.attributes.get("DW_AT_location")
                     and self.die_variable.attributes.get("DW_AT_name") is not None
                 ):
-                    self.var_name = self.die_variable.attributes.get(
-                        "DW_AT_name"
-                    ).value.decode("utf-8")
+                    self.var_name = self.die_variable.attributes.get("DW_AT_name").value.decode("utf-8")
                 else:
                     continue  # Skip to the next iteration if DW_AT_name is missing
 
                 type_attr = self.die_variable.attributes.get("DW_AT_type")
                 if type_attr is None:
                     continue  # Skip to the next iteration if DW_AT_type is missing
 
                 ref_addr = type_attr.value + self.die_variable.cu.cu_offset
 
                 #
                 type_die = self.dwarf_info.get_DIE_from_refaddr(ref_addr)
-                print(type_die)
-                if type_die.tag == "DW_TAG_array_type":
-                    array_length = self._get_array_length(type_die)
-                    print(self.die_variable.attributes.get("DW_AT_name"))
-                    print(array_length)
-                elif type_die.tag != "DW_TAG_volatile_type":
+                # if type_die.tag == "DW_TAG_array_type":
+                #     self.array_size = self._get_array_length(type_die)
+                #     print(self.die_variable.attributes.get("DW_AT_name"))
+                #     print("array_length", self.array_size)
+                if type_die.tag != "DW_TAG_volatile_type":
                     end_die = self._get_end_die(type_die)
-                    self._processing_end_die(end_die)
+                    self._processing_end_die(type_die, end_die)
 
                 elif type_die.tag == "DW_TAG_volatile_type":
                     end_die = self._get_end_die(type_die)
                     if end_die is None:
                         continue
-                    self._processing_end_die(end_die)
+                    self._processing_end_die(type_die, end_die)
                     continue
 
         return self.variable_map
 
 
 if __name__ == "__main__":
     logging.basicConfig(level=logging.DEBUG)
     elf_file = r"C:\Users\m67250\Downloads\mclv2_sam_e54_pim.X.production.elf"
-    # elf_file = r'C:\Users\m67250\Downloads\E54_github_packsupdated\mclv2_sam_e54_pim.X\dist\mclv2_sam_e54_pim
-    # \production\mclv2_sam_e54_pim.X.production.elf'
-
     elf_reader = Elf32Parser(elf_file)
     variable_map = elf_reader.map_variables()
-    print(variable_map)
+    # print(variable_map)
```

### Comparing `pyx2cscope-0.1.3/pyx2cscope/parser/Elf_Parser.py` & `pyx2cscope-0.1.4/pyx2cscope/parser/Elf_Parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         address (int): The memory address of the variable.
     """
 
     name: str
     type: str
     byte_size: int
     address: int
+    array_size: int = 0
 
 
 class ElfParser(ABC):
     """
     Abstract base class for parsing ELF files.
 
     This class provides a general interface for parsing ELF files and extracting
@@ -50,14 +51,15 @@
             elf_path (str): Path to the ELF file.
         """
         self.elf_path = elf_path
         self.dwarf_info = {}
         self.elf_file = None
         self.variable_map = {}
         self.var_name = None
+        self.array_size = 0
         self._load_elf_file()
 
     def get_var_info(self, name: str) -> Optional[VariableInfo]:
         """
         Return the VariableInfo associated with a given variable name, or None if not found.
 
         Args:
```

### Comparing `pyx2cscope-0.1.3/pyx2cscope/parser/arraySupport.py` & `pyx2cscope-0.1.4/pyx2cscope/parser/arraySupport.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,24 +22,18 @@
                         type_offset = type_attr.value + CU.cu_offset
                         type_DIE = offset_to_die.get(type_offset)
 
                         # Now, look for the array length in the type DIE
                         if type_DIE.tag == "DW_TAG_array_type":
                             for child in type_DIE.iter_children():
                                 if child.tag == "DW_TAG_subrange_type":
-                                    array_length_attr = child.attributes.get(
-                                        "DW_AT_upper_bound"
-                                    )
+                                    array_length_attr = child.attributes.get("DW_AT_upper_bound")
                                     if array_length_attr:
-                                        array_length = (
-                                            array_length_attr.value + 1
-                                        )  # upper_bound is 0-indexed
-                                        print(
-                                            f"Array length of '{array_name}': {array_length}"
-                                        )
+                                        array_length = array_length_attr.value + 1  # upper_bound is 0-indexed
+                                        print(f"Array length of '{array_name}': {array_length}")
                                         return array_length
                         break
 
 
 # get_named_array_length(
 #     r"C:\Users\m67250\Downloads\E54_github_packsupdated\mclv2_sam_e54_pim.X\dist\mclv2_sam_e54_pim\production\mclv2_sam_e54_pim.X.production.elf",
 #     "ScopeArray",
```

### Comparing `pyx2cscope-0.1.3/pyx2cscope/variable/variable_factory.py` & `pyx2cscope-0.1.4/pyx2cscope/variable/variable_factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,21 +54,28 @@
 
         Returns:
             Variable: The Variable object, if found. None otherwise.
         """
         try:
             variable_info = self.parser.get_var_info(name)
             return self._get_variable_instance(
-                variable_info.address, variable_info.type, variable_info.name
+                variable_info.address,
+                variable_info.type,
+                variable_info.array_size,
+                variable_info.name,
             )
         except Exception as e:
             logging.error(f"Error while getting variable '{name}' : {str(e)}")
 
     def _get_variable_instance(
-        self, address: int, var_type: str, name: str
+        self,
+        address: int,
+        var_type: str,
+        array_size: int,
+        name: str,
     ) -> Variable:
         """
         create a variable object based on the provided address, type, and name.
 
         args:
             address (int): Address of the variable in the MCU memory.
             var_type (VarTypes): Type of the variable.
@@ -88,17 +95,15 @@
             "int": Variable_int16,
             "long": Variable_int32,
             "long double": Variable_float,
             "long int": Variable_int32,
             "long long": Variable_int64,
             "long long unsigned int": Variable_uint64,
             "long unsigned int": Variable_uint32,
-            "pointer": Variable_uint16
-            if self.device_info.uc_width == 2
-            else Variable_uint32,  # TODO v 0.2.0
+            "pointer": Variable_uint16 if self.device_info.uc_width == 2 else Variable_uint32,  # TODO v 0.2.0
             "short": Variable_int16,
             "short int": Variable_int16,
             "short unsigned int": Variable_uint16,
             "signed char": Variable_int8,
             "signed int": Variable_int32,
             "signed long": Variable_int32,
             "signed long long": Variable_int64,
@@ -106,12 +111,10 @@
             "unsigned int": Variable_uint16,
             "unsigned long": Variable_uint32,
             "unsigned long long": Variable_uint64,
         }
 
         try:
             var_type = var_type.lower().replace("_", "")
-            return type_factory[var_type](self.l_net, address, name)
+            return type_factory[var_type](self.l_net, address, array_size, name)
         except IndexError:
-            raise Exception(
-                f"Type {var_type} not found. Cannot select the right variable representation."
-            )
+            raise Exception(f"Type {var_type} not found. Cannot select the right variable representation.")
```

### Comparing `pyx2cscope-0.1.3/pyx2cscope/xc2scope.py` & `pyx2cscope-0.1.4/pyx2cscope/xc2scope.py`

 * *Files 6% similar despite different names*

```diff
@@ -221,30 +221,25 @@
         Check if the scope data is ready.
 
         Returns:
             bool: True if the scope data is ready, False otherwise.
         """
         scope_data = self.lnet.load_parameters()
         logging.debug(scope_data)
-        return (
-            scope_data.scope_state == 0
-            or scope_data.data_array_pointer == scope_data.data_array_used_length
-        )
+        return scope_data.scope_state == 0 or scope_data.data_array_pointer == scope_data.data_array_used_length
 
     def get_trigger_position(self) -> int:
         """
         Get the position of the trigger event.
 
         Returns:
             int: The index position of the trigger event.
         """
         scope_data: LoadScopeData = self.lnet.scope_data
-        return int(
-            scope_data.trigger_event_position / self.scope_setup.get_dataset_size()
-        )
+        return int(scope_data.trigger_event_position / self.scope_setup.get_dataset_size())
 
     def get_delay_trigger_position(self) -> int:
         """
         Get the position of the delay trigger.
 
         Returns:
             int: The index position of the delay trigger.
@@ -256,44 +251,55 @@
         """
         Calculate the used length of the Scope Data Array (SDA).
 
         Returns:
             The length of the used portion of the SDA.
         """
         # SDA(Scope Data Array) - SDA % DSS(Data Set Size)
-        bytes_not_used = (
-            self.lnet.scope_data.data_array_size % self.scope_setup.get_dataset_size()
-        )
+        bytes_not_used = self.lnet.scope_data.data_array_size % self.scope_setup.get_dataset_size()
         return self.lnet.scope_data.data_array_size - bytes_not_used
 
     def _read_array_chunks(self):
         """
         Read array chunks from the LNet layer.
 
         Returns:
             A list containing the chunk data.
         """
         chunk_data = []
         data_type = 1  # it will always be 1 for array data
-        chunk_size = (
-            253  # full chunk excluding crc and Service-ID in total bytes 255 0xFF
-        )
+        chunk_size = 253  # full chunk excluding crc and Service-ID in total bytes 255 0xFF
         # Calculate the number of chunks
         num_chunks = self._calc_sda_used_length() // chunk_size
         for i in range(num_chunks):
             # Calculate the starting address for the current chunk
             current_address = self.lnet.scope_data.data_array_address + i * chunk_size
             try:
                 # Read the chunk of data
                 data = self.lnet.get_ram_array(current_address, chunk_size, data_type)
                 chunk_data.extend(data)
             except Exception as e:
                 logging.error(f"Error reading chunk {i}: {str(e)}")
         return chunk_data
 
+    def read_array(self, address, data_type):
+        # TODO
+        chunk_data = []
+        chunk_size = 253  # full chunk excluding crc and Service-ID in total bytes 255 0xFF
+        for i in range(5):
+            # Calculate the starting address for the current chunk
+            current_address = self.lnet.scope_data.data_array_address + i * chunk_size
+            try:
+                # Read the chunk of data
+                data = self.lnet.get_ram_array(current_address, chunk_size, data_type)
+                chunk_data.extend(data)
+            except Exception as e:
+                logging.error(f"Error reading chunk {i}: {str(e)}")
+        return chunk_data
+
     def _sort_channel_data(self, data) -> Dict[str, List[Number]]:
         """
         Sort and convert the dataset byte order into channel byte order.
 
         Args:
             data: The raw data read from the scope.
 
@@ -319,17 +325,15 @@
         Args:
             channels: The dictionary of channels with raw data.
 
         Returns:
             The filtered dictionary of channels with valid data only.
         """
         start = self.get_delay_trigger_position()
-        nr_of_sda = int(
-            self.lnet.scope_data.data_array_size % self.scope_setup.get_dataset_size()
-        )
+        nr_of_sda = int(self.lnet.scope_data.data_array_size % self.scope_setup.get_dataset_size())
         end = nr_of_sda - start
         for channel in channels:
             channels[channel] = channels[channel][start:end]
         return channels
 
     def get_scope_channel_data(self, valid_data=False) -> Dict[str, List[Number]]:
         """
```

### Comparing `pyx2cscope-0.1.3/PKG-INFO` & `pyx2cscope-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyx2cscope
-Version: 0.1.3
+Version: 0.1.4
 Summary: python implementation of X2Cscope
 Home-page: https://x2cscope.github.io/
 License: Proprietary
 Author: Yash Agarwal
 Author-email: yash.agarwal@microchip.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 2
```

