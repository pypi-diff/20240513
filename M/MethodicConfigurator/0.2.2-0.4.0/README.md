# Comparing `tmp/methodicconfigurator-0.2.2.tar.gz` & `tmp/methodicconfigurator-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "methodicconfigurator-0.2.2.tar", last modified: Mon Apr 15 18:46:30 2024, max compression
+gzip compressed data, was "methodicconfigurator-0.4.0.tar", last modified: Mon May 13 08:55:33 2024, max compression
```

## Comparing `methodicconfigurator-0.2.2.tar` & `methodicconfigurator-0.4.0.tar`

### file list

```diff
@@ -1,31 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:46:30.143873 methodicconfigurator-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-04-15 18:46:04.000000 methodicconfigurator-0.2.2/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:46:30.139873 methodicconfigurator-0.2.2/MethodicConfigurator/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-15 18:46:04.000000 methodicconfigurator-0.2.2/MethodicConfigurator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27962 2024-04-15 18:46:04.000000 methodicconfigurator-0.2.2/MethodicConfigurator/annotate_params.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7142 2024-04-15 18:46:04.000000 methodicconfigurator-0.2.2/MethodicConfigurator/ardupilot_methodic_configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)    20449 2024-04-15 18:46:04.000000 methodicconfigurator-0.2.2/MethodicConfigurator/backend_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)    26423 2024-04-15 18:46:04.000000 methodicconfigurator-0.2.2/MethodicConfigurator/backend_flightcontroller.py
--rw-r--r--   0 runner    (1001) docker     (127)    23170 2024-04-15 18:46:04.000000 methodicconfigurator-0.2.2/MethodicConfigurator/backend_mavftp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8091 2024-04-15 18:46:04.000000 methodicconfigurator-0.2.2/MethodicConfigurator/component_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-04-15 18:46:04.000000 methodicconfigurator-0.2.2/MethodicConfigurator/extract_param_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    45651 2024-04-15 18:46:04.000000 methodicconfigurator-0.2.2/MethodicConfigurator/frontend_tkinter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11256 2024-04-15 18:46:04.000000 methodicconfigurator-0.2.2/MethodicConfigurator/frontend_tkinter_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    16046 2024-04-15 18:46:04.000000 methodicconfigurator-0.2.2/MethodicConfigurator/frontend_tkinter_connection_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)    19170 2024-04-15 18:46:04.000000 methodicconfigurator-0.2.2/MethodicConfigurator/frontend_tkinter_directory_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-15 18:46:04.000000 methodicconfigurator-0.2.2/MethodicConfigurator/param_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-04-15 18:46:04.000000 methodicconfigurator-0.2.2/MethodicConfigurator/param_pid_adjustment_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    20131 2024-04-15 18:46:04.000000 methodicconfigurator-0.2.2/MethodicConfigurator/tempcal_IMU.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-15 18:46:04.000000 methodicconfigurator-0.2.2/MethodicConfigurator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:46:30.139873 methodicconfigurator-0.2.2/MethodicConfigurator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-04-15 18:46:30.000000 methodicconfigurator-0.2.2/MethodicConfigurator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-15 18:46:30.000000 methodicconfigurator-0.2.2/MethodicConfigurator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 18:46:30.000000 methodicconfigurator-0.2.2/MethodicConfigurator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-15 18:46:30.000000 methodicconfigurator-0.2.2/MethodicConfigurator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 18:46:30.000000 methodicconfigurator-0.2.2/MethodicConfigurator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 18:46:30.000000 methodicconfigurator-0.2.2/MethodicConfigurator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 18:46:27.000000 methodicconfigurator-0.2.2/MethodicConfigurator.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-04-15 18:46:30.143873 methodicconfigurator-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-15 18:46:04.000000 methodicconfigurator-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 18:46:30.143873 methodicconfigurator-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-15 18:46:04.000000 methodicconfigurator-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:55:33.429222 methodicconfigurator-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/LICENSE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:55:33.429222 methodicconfigurator-0.4.0/MethodicConfigurator/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27850 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/annotate_params.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5269 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/ardupilot_methodic_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28850 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/backend_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/backend_filesystem_configuration_steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/backend_filesystem_vehicle_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30964 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/backend_flightcontroller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26711 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/backend_mavftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/battery_cell_voltages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/common_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/extract_param_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13790 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/frontend_tkinter_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17895 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/frontend_tkinter_component_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/frontend_tkinter_component_editor_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14476 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/frontend_tkinter_connection_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19947 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/frontend_tkinter_directory_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36799 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/frontend_tkinter_parameter_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23781 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/frontend_tkinter_parameter_editor_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2468 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/get_release_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/param_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/param_pid_adjustment_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22803 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/tempcal_imu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:55:33.429222 methodicconfigurator-0.4.0/MethodicConfigurator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-05-13 08:55:33.000000 methodicconfigurator-0.4.0/MethodicConfigurator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-13 08:55:33.000000 methodicconfigurator-0.4.0/MethodicConfigurator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:55:33.000000 methodicconfigurator-0.4.0/MethodicConfigurator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 08:55:33.000000 methodicconfigurator-0.4.0/MethodicConfigurator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-13 08:55:33.000000 methodicconfigurator-0.4.0/MethodicConfigurator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-13 08:55:33.000000 methodicconfigurator-0.4.0/MethodicConfigurator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:55:26.000000 methodicconfigurator-0.4.0/MethodicConfigurator.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-05-13 08:55:33.429222 methodicconfigurator-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 08:55:33.429222 methodicconfigurator-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/setup.py
```

### Comparing `methodicconfigurator-0.2.2/LICENSE.md` & `methodicconfigurator-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.2.2/MethodicConfigurator/annotate_params.py` & `methodicconfigurator-0.4.0/MethodicConfigurator/annotate_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import argparse
 import logging
 
 # URL of the XML file
 BASE_URL = "https://autotest.ardupilot.org/Parameters/"
 
 PARAM_DEFINITION_XML_FILE = "apm.pdef.xml"
-LUA_PARAM_DEFINITION_XML_FILE = "19_inflight_magnetometer_fit_setup.pdef.xml"
+LUA_PARAM_DEFINITION_XML_FILE = "22_inflight_magnetometer_fit_setup.pdef.xml"
 
 # ArduPilot parameter names start with a capital letter and can have capital letters, numbers and _
 PARAM_NAME_REGEX = r'^[A-Z][A-Z_0-9]*'
 PARAM_NAME_MAX_LEN = 16
 VERSION = '1.0'
 
 
@@ -380,18 +380,15 @@
     # Dictionary to store the parameter documentation
     doc = {}
 
     # Use the findall method with an XPath expression to find all "param" elements
     for param in root.findall(".//param"):
         name = param.get("name")
         # Remove the <vehicle_type>: prefix from the name if it exists
-        if vehicle_type == "ArduRover":
-            name = remove_prefix(name, "Rover" + ":")
-        else:
-            name = remove_prefix(name, vehicle_type + ":")
+        name = remove_prefix(name, vehicle_type + ":")
 
         human_name = param.get("humanName")
         documentation = split_into_lines(param.get("documentation"), max_line_length)
         # the keys are the "name" attribute of the "field" sub-elements
         # the values are the text content of the "field" sub-elements
         fields = {field.get("name"): field.text for field in param.findall("field")}
         # if Units and UnitText exist, combine them into a single element
@@ -547,15 +544,15 @@
 
     if param_default_dict is None:
         param_default_dict = {}
 
     # Iterate over all the target ArduPilot parameter files
     for param_file in param_files:
 
-        if os_path.basename(param_file).endswith("19_inflight_magnetometer_fit_setup.param") and "MAGH_ALT_DELTA" not in doc:
+        if os_path.basename(param_file).endswith("22_inflight_magnetometer_fit_setup.param") and "MAGH_ALT_DELTA" not in doc:
             continue
 
         # Read the entire file contents
         with open(param_file, "r", encoding="utf-8") as file:
             lines = file.readlines()
 
         new_lines = []
@@ -637,15 +634,15 @@
         if args.verbose:
             print_read_only_params(doc_dict)
         if os_path.isfile(os_path.join(os_path.dirname(args.target), LUA_PARAM_DEFINITION_XML_FILE)):
             xml_root, param_default_dict = get_xml_data(BASE_URL + args.vehicle_type + "/",
                                                         xml_dir, LUA_PARAM_DEFINITION_XML_FILE)
             doc_dict = create_doc_dict(xml_root, args.vehicle_type, args.max_line_length)
             update_parameter_documentation(doc_dict, os_path.join(os_path.dirname(args.target),
-                                                                  "19_inflight_magnetometer_fit_setup.param"))
+                                                                  "22_inflight_magnetometer_fit_setup.param"))
     except Exception as exp:  # pylint: disable=W0718
         logging.fatal(exp)
         exit(1)  # pylint: disable=R1722
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `methodicconfigurator-0.2.2/MethodicConfigurator/ardupilot_methodic_configurator.py` & `methodicconfigurator-0.4.0/MethodicConfigurator/ardupilot_methodic_configurator.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,27 +11,26 @@
 import argparse
 from logging import basicConfig as logging_basicConfig
 from logging import getLevelName as logging_getLevelName
 # from logging import debug as logging_debug
 from logging import info as logging_info
 from logging import warning as logging_warning
 from logging import error as logging_error
-from os import getcwd as os_getcwd
 from sys import exit as sys_exit
 
 from backend_filesystem import LocalFilesystem
 from backend_flightcontroller import FlightController
 
 from frontend_tkinter_connection_selection import ConnectionSelectionWindow
 
 from frontend_tkinter_directory_selection import VehicleDirectorySelectionWindow
 
-from component_editor import JsonEditorApp
+from frontend_tkinter_component_editor import ComponentEditorWindow
 
-from frontend_tkinter import ParameterEditorWindow
+from frontend_tkinter_parameter_editor import ParameterEditorWindow
 
 from version import VERSION
 
 
 # pylint: disable=duplicate-code
 def argument_parser():
     """
@@ -48,39 +47,17 @@
                                      'its current value on the flight controller, its new value from the selected '
                                      'intermediate parameter file, and an "write" checkbox. The GUI includes "Write '
                                      'Selected to FC" and "Skip" buttons at the bottom. '
                                      'When "Write Selected to FC" is clicked, it writes the selected parameters to the '
                                      'flight controller. '
                                      'When "Skip" is pressed, it skips to the next intermediate parameter file. '
                                      'The process gets repeated for each intermediate parameter file.')
-    parser.add_argument('--device',
-                        type=str,
-                        default="",
-                        help='MAVLink connection string to the flight controller. Defaults to autodetection'
-                        )
-    parser.add_argument('-r', '--reboot-time',
-                        type=int,
-                        default=7,
-                        help='Flight controller reboot time. '
-                        'Default is %(default)s')
-    parser.add_argument('-t', '--vehicle-type',
-                        choices=['AP_Periph', 'AntennaTracker', 'ArduCopter', 'ArduPlane',
-                                 'ArduSub', 'Blimp', 'Heli', 'Rover', 'SITL'],
-                        default='',
-                        help='The type of the vehicle. Defaults to ArduCopter')
-    parser.add_argument('--vehicle-dir',
-                        type=str,
-                        default=os_getcwd(),
-                        help='Directory containing vehicle-specific intermediate parameter files. '
-                        'Defaults to the current working directory')
-    parser.add_argument('--n',
-                        type=int,
-                        default=0,
-                        help='Start directly on the nth intermediate parameter file (skips previous files). '
-                        'Default is %(default)s')
+    parser = FlightController.add_argparse_arguments(parser)
+    parser = LocalFilesystem.add_argparse_arguments(parser)
+    parser = ComponentEditorWindow.add_argparse_arguments(parser)
     parser.add_argument('--loglevel',
                         type=str,
                         default='INFO',
                         choices=['DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL'],
                         help='Logging level (default is INFO).')
     parser.add_argument('-v', '--version',
                         action='version',
@@ -102,23 +79,16 @@
     if error_str:
         logging_error(error_str)
         conn_sel_window = ConnectionSelectionWindow(flight_controller, error_str)
         conn_sel_window.root.mainloop()
 
     vehicle_type = args.vehicle_type
     if vehicle_type == "":  # not explicitly set, to try to guess it
-        if "MOT_OPTIONS" in flight_controller.fc_parameters:
-            vehicle_type = "ArduCopter"
-        if "TECS_OPTIONS" in flight_controller.fc_parameters:
-            vehicle_type = "ArduPlane"
-        if "WENC_TYPE" in flight_controller.fc_parameters:
-            vehicle_type = "ArduRover"
-        if "RCMAP_LATERAL" in flight_controller.fc_parameters:
-            vehicle_type = "ArduSub"
-        if vehicle_type:
+        if flight_controller.vehicle_type is not None:
+            vehicle_type = flight_controller.vehicle_type
             logging_info("Vehicle type not set explicitly, auto-detected %s.", vehicle_type)
     else:
         logging_info("Vehicle type explicitly set to %s.", vehicle_type)
 
     if vehicle_type == "": # did not guess it, default to ArduCopter
         vehicle_type = "ArduCopter"
         logging_warning("Could not detect vehicle type. Defaulting to ArduCopter.")
@@ -129,28 +99,20 @@
     files = list(local_filesystem.file_parameters.keys())
 
     if not files:
         logging_error("No intermediate parameter files found in %s.", args.vehicle_dir)
         vehicle_dir_window = VehicleDirectorySelectionWindow(local_filesystem)
         vehicle_dir_window.root.mainloop()
 
-   # Get the list of intermediate parameter files files that will be processed sequentially
-    files = list(local_filesystem.file_parameters.keys())
-
-    start_file = None  # pylint: disable=invalid-name
-    if files:
-        # Determine the starting file based on the --n command line argument
-        start_file_index = min(args.n, len(files) - 1) # Ensure the index is within the range of available files
-        if start_file_index != args.n:
-            logging_warning("Starting file index %s is out of range. Starting with file %s instead.",
-                            args.n, files[start_file_index])
-        start_file = files[start_file_index]
+    start_file = local_filesystem.get_start_file(args.n)
 
-    app = JsonEditorApp(VERSION, local_filesystem)
-    app.root.mainloop()
+    if not args.skip_component_editor:
+        component_editor_window = ComponentEditorWindow(VERSION, local_filesystem)
+        component_editor_window.set_vehicle_type_and_version(vehicle_type, flight_controller.version)
+        component_editor_window.root.mainloop()
 
     # Call the GUI function with the starting intermediate parameter file
     ParameterEditorWindow(start_file, flight_controller, local_filesystem, VERSION)
 
     # Close the connection to the flight controller
     flight_controller.disconnect()
     sys_exit(0)
```

### Comparing `methodicconfigurator-0.2.2/MethodicConfigurator/backend_flightcontroller.py` & `methodicconfigurator-0.4.0/MethodicConfigurator/backend_flightcontroller.py`

 * *Files 11% similar despite different names*

```diff
@@ -80,68 +80,14 @@
     def inWaiting(self):  # pylint: disable=invalid-name
         return 0
 
     def close(self):
         pass
 
 
-def decode_flight_sw_version(flight_sw_version):
-    '''decode 32 bit flight_sw_version mavlink parameter
-    corresponds to ArduPilot encoding in  GCS_MAVLINK::send_autopilot_version'''
-    fw_type_id = (flight_sw_version >>  0) % 256  # noqa E221, E222
-    patch      = (flight_sw_version >>  8) % 256  # noqa E221, E222
-    minor      = (flight_sw_version >> 16) % 256  # noqa E221
-    major      = (flight_sw_version >> 24) % 256  # noqa E221
-    if fw_type_id == 0:
-        fw_type = "dev"
-    elif fw_type_id == 64:
-        fw_type = "alpha"
-    elif fw_type_id == 128:
-        fw_type = "beta"
-    elif fw_type_id == 192:
-        fw_type = "rc"
-    elif fw_type_id == 255:
-        fw_type = "official"
-    else:
-        fw_type = "undefined"
-    return major, minor, patch, fw_type
-
-
-def decode_flight_capabilities(capabilities):
-    '''Decode 32 bit flight controller capabilities bitmask mavlink parameter.
-    Returns a list of concise English descriptions of each active capability.
-    '''
-    # Initialize an empty list to store the descriptions
-    descriptions = []
-
-    # Iterate through each bit in the capabilities bitmask
-    for bit in range(32):
-        # Check if the bit is set
-        if capabilities & (1 << bit):
-            # Use the bit value to get the corresponding capability enum
-            capability = mavutil.mavlink.enums["MAV_PROTOCOL_CAPABILITY"].get(1 << bit, "Unknown capability")
-            # Append the description of the capability to the list
-            logging_info(capability.description)
-            descriptions.append(capability.name)
-
-    return descriptions
-
-
-# see for more info:
-# pymavlink.dialects.v20.ardupilotmega
-def decode_mav_type(mav_type):
-    return mavutil.mavlink.enums["MAV_TYPE"].get(mav_type,
-                                                 mavutil.mavlink.EnumEntry("None", "Unknown type")).description
-
-
-def decode_mav_autopilot(mav_autopilot):
-    return mavutil.mavlink.enums["MAV_AUTOPILOT"].get(mav_autopilot,
-                                                      mavutil.mavlink.EnumEntry("None", "Unknown type")).description
-
-
 class FlightController:  # pylint: disable=too-many-instance-attributes
     """
     A class to manage the connection and parameters of a flight controller.
 
     Attributes:
         device (str): The connection string to the flight controller.
         master (mavutil.mavlink_connection): The MAVLink connection object.
@@ -152,53 +98,61 @@
         Initialize the FlightController communication object.
 
         """
         # warn people about ModemManager which interferes badly with ArduPilot
         if os_path.exists("/usr/sbin/ModemManager"):
             logging_warning("You should uninstall ModemManager as it conflicts with ArduPilot")
 
-        self.reboot_time = reboot_time
-        comports = FlightController.list_serial_ports()
-        # ubcports = FlightController.list_usb_devices()
-        netports = FlightController.list_network_ports()
-        # list of tuples with the first element being the port name and the second element being the port description
-        self.connection_tuples = [(port.device, port.description) for port in comports] + [(port, port) for port in netports]
-        logging_info('Available connection ports are:')
-        for port in self.connection_tuples:
-            logging_info("%s - %s", port[0], port[1])
-        self.connection_tuples += [tuple(['Add another', 'Add another'])]  # now that it is logged, add the 'Add another' tuple
+        self.__reboot_time = reboot_time
+        self.__connection_tuples = []
+        self.discover_connections()
         self.master = None
         self.comport = None
         self.fc_parameters = {}
-        self.target_system = None
-        self.target_component = None
-        self.capabilities = None
+        self.__target_system = None
+        self.__target_component = None
+        self.__capabilities = None
         self.version = None
+        self.vehicle_type = None
+
+    def discover_connections(self):
+        comports = FlightController.__list_serial_ports()
+        usbports = FlightController.__list_usb_devices()
+        netports = FlightController.__list_network_ports()
+        # list of tuples with the first element being the port name and the second element being the port description
+        self.__connection_tuples = [(port.device, port.description) for port in comports] + \
+            [(port, port) for port in usbports] + \
+            [(port, port) for port in netports]
+        logging_info('Available connection ports are:')
+        for port in self.__connection_tuples:
+            logging_info("%s - %s", port[0], port[1])
+        # now that it is logged, add the 'Add another' tuple
+        self.__connection_tuples += [tuple(['Add another', 'Add another'])]
 
     def disconnect(self):
         """
         Close the connection to the flight controller.
         """
         if self.master is not None:
             self.master.close()
             self.master = None
         self.fc_parameters = {}
-        self.target_system = None
-        self.target_component = None
-        self.capabilities = None
+        self.__target_system = None
+        self.__target_component = None
+        self.__capabilities = None
         self.version = None
 
     def add_connection(self, connection_string: str):
         """
         Add a new connection to the list of available connections.
         """
         if connection_string:
             # Check if connection_string is not the first element of any tuple in self.other_connection_tuples
-            if all(connection_string != t[0] for t in self.connection_tuples):
-                self.connection_tuples.insert(-1, (connection_string, connection_string))
+            if all(connection_string != t[0] for t in self.__connection_tuples):
+                self.__connection_tuples.insert(-1, (connection_string, connection_string))
                 logging_debug("Added connection %s", connection_string)
                 return True
             logging_debug("Did not add duplicated connection %s", connection_string)
         else:
             logging_debug("Did not add empty connection")
         return False
 
@@ -218,18 +172,20 @@
                                                     of the connection attempt. Defaults to None.
 
         Returns:
             str: An error message if the connection fails, otherwise an empty string indicating
                 a successful connection.
         """
         if device:
+            if device == 'none':
+                return ''
             self.add_connection(device)
             self.comport = mavutil.SerialPort(device=device, description=device)
         else:
-            autodetect_serial = self.auto_detect_serial()
+            autodetect_serial = self.__auto_detect_serial()
             if autodetect_serial:
                 # Resolve the soft link if it's a Linux system
                 if os_name == 'posix':
                     try:
                         dev = autodetect_serial[0].device
                         logging_debug("Auto-detected device %s", dev)
                         # Get the directory part of the soft link
@@ -238,39 +194,35 @@
                         resolved_path = os_path.abspath(os_path.join(softlink_dir, os_readlink(dev)))
                         autodetect_serial[0].device = resolved_path
                         logging_debug("Resolved soft link %s to %s", dev, resolved_path)
                     except OSError:
                         pass # Not a soft link, proceed with the original device path
                 self.comport = autodetect_serial[0]
                 # Add the detected serial port to the list of available connections if it is not there
-                if self.comport.device not in [t[0] for t in self.connection_tuples]:
-                    self.connection_tuples.insert(-1, (self.comport.device, self.comport.description))
+                if self.comport.device not in [t[0] for t in self.__connection_tuples]:
+                    self.__connection_tuples.insert(-1, (self.comport.device, self.comport.description))
             else:
                 return "No serial ports found. Please connect a flight controller and try again."
-        error_message = self.create_connection_with_retry(progress_callback=progress_callback)
-        if device == 'test': # FIXME for testing only pylint: disable=fixme
-            self.fc_parameters['INS_LOG_BAT_MASK'] = 1.0
-            self.fc_parameters['INS_TCAL1_TMAX'] = 1.0
-            self.fc_parameters['COMPASS_DEV_ID'] = 1.0
+        error_message = self.__create_connection_with_retry(progress_callback=progress_callback)
         return error_message
 
-    def request_message(self, message_id: int):
+    def __request_message(self, message_id: int):
         self.master.mav.command_long_send(
-            self.target_system,
-            self.target_component,
+            self.__target_system,
+            self.__target_component,
             mavutil.mavlink.MAV_CMD_REQUEST_MESSAGE,
             0, # confirmation
             message_id, 0, 0, 0, 0, 0, 0)
 
-    def cmd_version(self):
+    def __cmd_version(self):
         '''show version'''
-        self.request_message(mavutil.mavlink.MAVLINK_MSG_ID_AUTOPILOT_VERSION)
+        self.__request_message(mavutil.mavlink.MAVLINK_MSG_ID_AUTOPILOT_VERSION)
 
-    def create_connection_with_retry(self, progress_callback, retries: int = 3,  # pylint: disable=too-many-return-statements
-                                     timeout: int = 5) -> mavutil.mavlink_connection:
+    def __create_connection_with_retry(self, progress_callback, retries: int = 3, # pylint: disable=too-many-return-statements
+                                       timeout: int = 5) -> mavutil.mavlink_connection:
         """
         Attempts to create a connection to the flight controller with retries.
 
         This method attempts to establish a connection to the flight controller using the
         provided device connection string. It will retry the connection attempt up to the
         specified number of retries if the initial attempt fails. The method also supports
         a progress callback to report the progress of the connection attempt.
@@ -293,50 +245,51 @@
             self.master = mavutil.mavlink_connection(device=self.comport.device, timeout=timeout,
                                                      retries=retries, progress_callback=progress_callback)
             logging_debug("Waiting for MAVLink heartbeat")
             m = self.master.wait_heartbeat(timeout=timeout)
             if m is None:
                 logging_error("No MAVLink heartbeat received, connection failed.")
                 return "No MAVLink heartbeat received, connection failed."
-            self.target_system = m.get_srcSystem()
-            self.target_component = m.get_srcComponent()
-            logging_info(f"Vehicle type {decode_mav_type(m.type)}")
-            logging_info(f"Autopilot type {decode_mav_autopilot(m.autopilot)}")
-            logging_debug("Connection established with systemID %d, componentID %d.", self.target_system,
-                          self.target_component)
+            self.__target_system = m.get_srcSystem()
+            self.__target_component = m.get_srcComponent()
+            logging_debug("Connection established with systemID %d, componentID %d.", self.__target_system,
+                          self.__target_component)
+            logging_info(f"Autopilot type {self.__decode_mav_autopilot(m.autopilot)}")
             if m.autopilot != mavutil.mavlink.MAV_AUTOPILOT_ARDUPILOTMEGA:
-                logging_error("Unsupported autopilot type %s", decode_mav_autopilot(m.autopilot))
-                return f"Unsupported autopilot type {decode_mav_autopilot(m.autopilot)}"
+                logging_error("Unsupported autopilot type %s", self.__decode_mav_autopilot(m.autopilot))
+                return f"Unsupported autopilot type {self.__decode_mav_autopilot(m.autopilot)}"
+            self.vehicle_type = self.__classify_vehicle_type(m.type)
+            logging_info(f"Vehicle type {self.__decode_mav_type(m.type)} running {self.vehicle_type} firmware")
 
-            self.cmd_version()
+            self.__cmd_version()
             m = self.master.recv_match(type='AUTOPILOT_VERSION', blocking=True, timeout=timeout)
             if m is None:
                 logging_error("No AUTOPILOT_VERSION MAVLink message received, connection failed.")
                 return "No AUTOPILOT_VERSION MAVLink message received, connection failed."
-            self.capabilities = m.capabilities
-            _cap_list = decode_flight_capabilities(self.capabilities)
+            self.__capabilities = m.capabilities
+            _cap_list = self.__decode_flight_capabilities(self.__capabilities)
             # logging_info("Flight Controller Capabilities: %s", (", ").join(
             #     [capability.removeprefix("MAV_PROTOCOL_CAPABILITY_")
             #      for capability in _cap_list]))
-            v_major, v_minor, v_patch, v_fw_type = decode_flight_sw_version(m.flight_sw_version)
+            v_major, v_minor, v_patch, v_fw_type = self.__decode_flight_sw_version(m.flight_sw_version)
             self.version = f"{v_major}.{v_minor}.{v_patch}"
             logging_info("Flight Controller Version: %s %s", self.version, v_fw_type)
             # logging_info(f"Flight Controller Middleware version number: {m.middleware_sw_version}")
             # logging_info(f"Flight Controller Operating system version number: {m.os_sw_version}")
             logging_info(f"Flight Controller HW / board version: {m.board_version}")
             # Convert each value in the array to hex and join them together
             flight_custom_version_hex = ''.join(chr(c) for c in m.flight_custom_version)
             # middleware_custom_version_hex = ''.join(chr(c) for c in m.middleware_custom_version)
             os_custom_version_hex = ''.join(chr(c) for c in m.os_custom_version)
             logging_info(f"Flight Controller first 8 hex bytes of the FC git hash: {flight_custom_version_hex}")
             # logging_info(f"Flight Controller first 8 hex bytes of the MW git hash: {middleware_custom_version_hex}")
             logging_info(f"Flight Controller first 8 hex bytes of the ChibiOS git hash: {os_custom_version_hex}")
             if m.vendor_id == 0x1209 and m.product_id == 0x5740:
                 return ""  # these are just generic ArduPilot values, there is no value in printing them
-            pid_vid_dict = self.list_ardupilot_supported_usb_pid_vid()
+            pid_vid_dict = self.__list_ardupilot_supported_usb_pid_vid()
             if m.vendor_id in pid_vid_dict:
                 logging_info(f"Flight Controller board vendor: {pid_vid_dict[m.vendor_id]['vendor']}")
                 if m.product_id in pid_vid_dict[m.vendor_id]['PID']:
                     logging_info(f"Flight Controller board product: {pid_vid_dict[m.vendor_id]['PID'][m.product_id]}")
                 else:
                     logging_info(f"Flight Controller board product ID: 0x{hex(m.product_id)}")
             else:
@@ -352,37 +305,37 @@
     def read_params(self, progress_callback=None) -> Dict[str, float]:
         """
         Requests all flight controller parameters from a MAVLink connection.
 
         Returns:
             Dict[str, float]: A dictionary of flight controller parameters.
         """
-        # FIXME this entire is statement is for testing only, remove it later pylint: disable=fixme
+        # FIXME this entire if statement is for testing only, remove it later pylint: disable=fixme
         if self.master is None and self.comport is not None and self.comport.device == 'test':
-            filename = os_path.join('4.4.4-test-params', '00_default.param')
+            filename = 'params.param'
             logging_warning("Testing active, will load all parameters from the %s file", filename)
             par_dict_with_comments = Par.load_param_file_into_dict(filename)
             return {k: v.value for k, v in par_dict_with_comments.items()}
 
         if self.master is None:
             return None
 
         # Check if MAVFTP is supported
         # FIXME remove the "not" once it works pylint: disable=fixme
-        if self.capabilities:
-            if not (self.capabilities & mavutil.mavlink.MAV_PROTOCOL_CAPABILITY_FTP):  # pylint: disable=superfluous-parens
+        if self.__capabilities:
+            if not (self.__capabilities & mavutil.mavlink.MAV_PROTOCOL_CAPABILITY_FTP):  # pylint: disable=superfluous-parens
                 logging_info("MAVFTP is supported by the %s flight controller", self.comport.device)
                 # parameters, _defaults = self.read_params_via_mavftp(progress_callback)
                 return {}  # parameters
 
         logging_info("MAVFTP is not supported by the %s flight controller, fallback to MAVLink", self.comport.device)
         # MAVFTP is not supported, fall back to MAVLink
-        return self.read_params_via_mavlink(progress_callback)
+        return self.__read_params_via_mavlink(progress_callback)
 
-    def read_params_via_mavlink(self, progress_callback=None) -> Dict[str, float]:
+    def __read_params_via_mavlink(self, progress_callback=None) -> Dict[str, float]:
         logging_debug("Will fetch all parameters from the %s flight controller", self.comport.device)
         # Request all parameters
         self.master.mav.param_request_list_send(
             self.master.target_system, self.master.target_component
         )
 
         # Dictionary to store parameters
@@ -438,15 +391,15 @@
         time_sleep(0.3)
 
         self.disconnect()
 
         current_step = 0
 
         if sleep_time is None or sleep_time <= 7:
-            sleep_time = self.reboot_time
+            sleep_time = self.__reboot_time
 
         while current_step != sleep_time:
             # Call the progress callback with the current progress
             if reset_progress_callback:
                 reset_progress_callback(current_step, sleep_time)
 
             # Wait for sleep_time seconds
@@ -454,18 +407,18 @@
             current_step += 1
 
         # Call the progress callback with the current progress
         if reset_progress_callback:
             reset_progress_callback(current_step, sleep_time)
 
         # Reconnect to the flight controller
-        self.create_connection_with_retry(connection_progress_callback)
+        self.__create_connection_with_retry(connection_progress_callback)
 
     @staticmethod
-    def list_usb_devices():
+    def __list_usb_devices():
         """
         List all connected USB devices.
         """
         ret = []
         return ret # FIXME for testing only pylint: disable=fixme
         # devices = usb.core.find(find_all=True)
         # for device in devices:
@@ -489,50 +442,53 @@
         #     ret.append([device.idVendor,
         #                 device.idProduct,
         #                 manufacturer,
         #                 product])
         # return ret
 
     @staticmethod
-    def list_serial_ports():
+    def __list_serial_ports():
         """
         List all available serial ports.
         """
         comports = serial.tools.list_ports.comports()
         # for port in comports:
         #     logging_debug("ComPort - %s, Description: %s", port.device, port.description)
         return comports
 
     @staticmethod
-    def list_network_ports():
+    def __list_network_ports():
         """
         List all available network ports.
         """
         return ['tcp:127.0.0.1:5760', 'udp:127.0.0.1:14550']
 
-    @staticmethod
-    def auto_detect_serial():
+    def __auto_detect_serial(self):
+        for connection in self.__connection_tuples:
+            if 'mavlink' in connection[1].lower():
+                return [mavutil.SerialPort(device=connection[0], description=connection[1])]
+
         serial_list = mavutil.auto_detect_serial(preferred_list=preferred_ports)
         serial_list.sort(key=lambda x: x.device)
 
         # remove OTG2 ports for dual CDC
         if len(serial_list) == 2 and serial_list[0].device.startswith("/dev/serial/by-id"):
             if serial_list[0].device[:-1] == serial_list[1].device[0:-1]:
                 serial_list.pop(1)
 
         return serial_list
 
     def get_connection_tuples(self):
         """
         Get all available connections.
         """
-        return self.connection_tuples
+        return self.__connection_tuples
 
     @staticmethod
-    def list_ardupilot_supported_usb_pid_vid():
+    def __list_ardupilot_supported_usb_pid_vid():
         """
         List all ArduPilot supported USB vendor ID (VID) and product ID (PID).
 
         source: https://ardupilot.org/dev/docs/USB-IDs.html
         """
         return {
             0x0483: {'vendor': 'ST Microelectronics', 'PID': {0x5740: 'ChibiOS'}},
@@ -567,7 +523,142 @@
                                                            0x1152: 'VRBrain-v52',
                                                            0x1154: 'VRBrain-v54',
                                                            0x1910: 'VRCore-v10',
                                                            0x1351: 'VRUBrain-v51',
                                                            }
                      },
         }
+
+    @staticmethod
+    def __decode_flight_sw_version(flight_sw_version):
+        '''decode 32 bit flight_sw_version mavlink parameter
+        corresponds to ArduPilot encoding in  GCS_MAVLINK::send_autopilot_version'''
+        fw_type_id = (flight_sw_version >>  0) % 256  # noqa E221, E222
+        patch      = (flight_sw_version >>  8) % 256  # noqa E221, E222
+        minor      = (flight_sw_version >> 16) % 256  # noqa E221
+        major      = (flight_sw_version >> 24) % 256  # noqa E221
+        if fw_type_id == 0:
+            fw_type = "dev"
+        elif fw_type_id == 64:
+            fw_type = "alpha"
+        elif fw_type_id == 128:
+            fw_type = "beta"
+        elif fw_type_id == 192:
+            fw_type = "rc"
+        elif fw_type_id == 255:
+            fw_type = "official"
+        else:
+            fw_type = "undefined"
+        return major, minor, patch, fw_type
+
+
+    @staticmethod
+    def __decode_flight_capabilities(capabilities):
+        '''Decode 32 bit flight controller capabilities bitmask mavlink parameter.
+        Returns a list of concise English descriptions of each active capability.
+        '''
+        # Initialize an empty list to store the descriptions
+        descriptions = []
+
+        # Iterate through each bit in the capabilities bitmask
+        for bit in range(32):
+            # Check if the bit is set
+            if capabilities & (1 << bit):
+                # Use the bit value to get the corresponding capability enum
+                capability = mavutil.mavlink.enums["MAV_PROTOCOL_CAPABILITY"].get(1 << bit, "Unknown capability")
+                # Append the description of the capability to the list
+                logging_info(capability.description)
+                descriptions.append(capability.name)
+
+        return descriptions
+
+
+    # see for more info:
+    # import pymavlink.dialects.v20.ardupilotmega
+    # pymavlink.dialects.v20.ardupilotmega.enums["MAV_TYPE"]
+    @staticmethod
+    def __decode_mav_type(mav_type):
+        return mavutil.mavlink.enums["MAV_TYPE"].get(mav_type,
+                                                    mavutil.mavlink.EnumEntry("None", "Unknown type")).description
+
+
+    @staticmethod
+    def __decode_mav_autopilot(mav_autopilot):
+        return mavutil.mavlink.enums["MAV_AUTOPILOT"].get(mav_autopilot,
+                                                        mavutil.mavlink.EnumEntry("None", "Unknown type")).description
+
+
+    @staticmethod
+    def __classify_vehicle_type(mav_type_int):
+        """
+        Classify the vehicle type based on the MAV_TYPE enum.
+
+        Parameters:
+        mav_type_int (int): The MAV_TYPE enum value.
+
+        Returns:
+        str: The classified vehicle type.
+        """
+        # Define the mapping from MAV_TYPE_* integer to vehicle type category
+        mav_type_to_vehicle_type = {
+            mavutil.mavlink.MAV_TYPE_FIXED_WING: 'ArduPlane',
+            mavutil.mavlink.MAV_TYPE_QUADROTOR: 'ArduCopter',
+            mavutil.mavlink.MAV_TYPE_COAXIAL: 'Heli',
+            mavutil.mavlink.MAV_TYPE_HELICOPTER: 'Heli',
+            mavutil.mavlink.MAV_TYPE_ANTENNA_TRACKER: 'AntennaTracker',
+            mavutil.mavlink.MAV_TYPE_GCS: 'AP_Periph',
+            mavutil.mavlink.MAV_TYPE_AIRSHIP: 'ArduBlimp',
+            mavutil.mavlink.MAV_TYPE_FREE_BALLOON: 'ArduBlimp',
+            mavutil.mavlink.MAV_TYPE_ROCKET: 'ArduCopter',
+            mavutil.mavlink.MAV_TYPE_GROUND_ROVER: 'Rover',
+            mavutil.mavlink.MAV_TYPE_SURFACE_BOAT: 'Rover',
+            mavutil.mavlink.MAV_TYPE_SUBMARINE: 'ArduSub',
+            mavutil.mavlink.MAV_TYPE_HEXAROTOR: 'ArduCopter',
+            mavutil.mavlink.MAV_TYPE_OCTOROTOR: 'ArduCopter',
+            mavutil.mavlink.MAV_TYPE_TRICOPTER: 'ArduCopter',
+            mavutil.mavlink.MAV_TYPE_FLAPPING_WING: 'ArduPlane',
+            mavutil.mavlink.MAV_TYPE_KITE: 'ArduPlane',
+            mavutil.mavlink.MAV_TYPE_ONBOARD_CONTROLLER: 'AP_Periph',
+            mavutil.mavlink.MAV_TYPE_VTOL_DUOROTOR: 'ArduPlane',
+            mavutil.mavlink.MAV_TYPE_VTOL_QUADROTOR: 'ArduPlane',
+            mavutil.mavlink.MAV_TYPE_VTOL_TILTROTOR: 'ArduPlane',
+            mavutil.mavlink.MAV_TYPE_VTOL_RESERVED2: 'ArduPlane',
+            mavutil.mavlink.MAV_TYPE_VTOL_RESERVED3: 'ArduPlane',
+            mavutil.mavlink.MAV_TYPE_VTOL_RESERVED4: 'ArduPlane',
+            mavutil.mavlink.MAV_TYPE_VTOL_RESERVED5: 'ArduPlane',
+            mavutil.mavlink.MAV_TYPE_GIMBAL: 'AP_Periph',
+            mavutil.mavlink.MAV_TYPE_ADSB: 'AP_Periph',
+            mavutil.mavlink.MAV_TYPE_PARAFOIL: 'ArduPlane',
+            mavutil.mavlink.MAV_TYPE_DODECAROTOR: 'ArduCopter',
+            mavutil.mavlink.MAV_TYPE_CAMERA: 'AP_Periph',
+            mavutil.mavlink.MAV_TYPE_CHARGING_STATION: 'AP_Periph',
+            mavutil.mavlink.MAV_TYPE_FLARM: 'AP_Periph',
+            mavutil.mavlink.MAV_TYPE_SERVO: 'AP_Periph',
+            mavutil.mavlink.MAV_TYPE_ODID: 'AP_Periph',
+            mavutil.mavlink.MAV_TYPE_DECAROTOR: 'ArduCopter',
+            mavutil.mavlink.MAV_TYPE_BATTERY: 'AP_Periph',
+            mavutil.mavlink.MAV_TYPE_PARACHUTE: 'AP_Periph',
+            mavutil.mavlink.MAV_TYPE_LOG: 'AP_Periph',
+            mavutil.mavlink.MAV_TYPE_OSD: 'AP_Periph',
+            mavutil.mavlink.MAV_TYPE_IMU: 'AP_Periph',
+            mavutil.mavlink.MAV_TYPE_GPS: 'AP_Periph',
+            mavutil.mavlink.MAV_TYPE_WINCH: 'AP_Periph',
+            # Add more mappings as needed
+        }
+
+        # Return the classified vehicle type based on the MAV_TYPE enum
+        return mav_type_to_vehicle_type.get(mav_type_int, None)
+
+    @staticmethod
+    def add_argparse_arguments(parser):
+        parser.add_argument('--device',
+                            type=str,
+                            default="",
+                            help='MAVLink connection string to the flight controller. If set to "none" no connection is made.'
+                            ' Defaults to autodetection'
+                            )
+        parser.add_argument('-r', '--reboot-time',
+                            type=int,
+                            default=7,
+                            help='Flight controller reboot time. '
+                            'Default is %(default)s')
+        return parser
```

### Comparing `methodicconfigurator-0.2.2/MethodicConfigurator/component_editor.py` & `methodicconfigurator-0.4.0/MethodicConfigurator/frontend_tkinter_component_editor_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,126 +14,95 @@
 from logging import getLevelName as logging_getLevelName
 # from logging import debug as logging_debug
 from logging import info as logging_info
 
 import tkinter as tk
 from tkinter import ttk
 
-from PIL import Image
-from PIL import ImageTk
+from common_arguments import add_common_arguments_and_parse
 
 from backend_filesystem import LocalFilesystem
 
 from frontend_tkinter_base import show_tooltip
+from frontend_tkinter_base import show_error_message
 from frontend_tkinter_base import ScrollFrame
 from frontend_tkinter_base import BaseWindow
 
 from version import VERSION
 
 
-# pylint: disable=duplicate-code
 def argument_parser():
     """
     Parses command-line arguments for the script.
 
     This function sets up an argument parser to handle the command-line arguments for the script.
 
     Returns:
     argparse.Namespace: An object containing the parsed arguments.
     """
-    parser = ArgumentParser(description='')
-    parser.add_argument('--vehicle-dir',
-                        type=str,
-                        default=LocalFilesystem.getcwd(),
-                        help='Directory containing vehicle-specific intermediate parameter files. '
-                        'Defaults to the current working directory')
-    parser.add_argument('--loglevel',
-                        type=str,
-                        default='INFO',
-                        choices=['DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL'],
-                        help='Logging level (default is INFO).')
-    parser.add_argument('-t', '--vehicle-type',
-                        choices=['AP_Periph', 'AntennaTracker', 'ArduCopter', 'ArduPlane',
-                                 'ArduSub', 'Blimp', 'Heli', 'Rover', 'SITL'],
-                        default='ArduCopter',
-                        help='The type of the vehicle. Defaults to ArduCopter')
-    parser.add_argument('-v', '--version',
-                        action='version',
-                        version=f'%(prog)s {VERSION}',
-                        help='Display version information and exit.')
-    return parser.parse_args()
-# pylint: enable=duplicate-code
+    parser = ArgumentParser(description='A GUI for editing JSON files that contain vehicle component configurations. '
+                            'Not to be used directly, but through the main ArduPilot methodic configurator script.')
+    parser = LocalFilesystem.add_argparse_arguments(parser)
+    parser = ComponentEditorWindowBase.add_argparse_arguments(parser)
+    return add_common_arguments_and_parse(parser)
 
 
-class JsonEditorApp(BaseWindow):
+class ComponentEditorWindowBase(BaseWindow):
     """
     A class for editing JSON files in the ArduPilot methodic configurator.
 
     This class provides a graphical user interface for editing JSON files that
     contain vehicle component configurations. It inherits from the BaseWindow
     class, which provides basic window functionality.
     """
     def __init__(self, version, local_filesystem: LocalFilesystem=None):
         super().__init__()
         self.local_filesystem = local_filesystem
 
         self.root.title("Amilcar Lucas's - ArduPilot methodic configurator - " + version + " - Vehicle Component Editor")
         self.root.geometry("880x600") # Set the window width
 
-        self.data = local_filesystem.load_vehicle_components_json_data()
+        self.data = local_filesystem.load_vehicle_components_json_data(local_filesystem.vehicle_dir)
         if len(self.data) < 1:
             # Schedule the window to be destroyed after the mainloop has started
             self.root.after(100, self.root.destroy) # Adjust the delay as needed
             return
 
         self.entry_widgets = {} # Dictionary for entry widgets
 
         self.main_frame = ttk.Frame(self.root)
         self.main_frame.pack(side=tk.TOP, fill="x", expand=False, pady=(4, 0)) # Pack the frame at the top of the window
 
         # Load the vehicle image and scale it down to image_height pixels in height
         if local_filesystem.vehicle_image_exists():
-            image_height = 100
-            image = Image.open(local_filesystem.vehicle_image_filepath())
-            # pylint: disable=duplicate-code
-            width, height = image.size
-            aspect_ratio = width / height
-            new_width = int(image_height * aspect_ratio)
-            resized_image = image.resize((new_width, image_height))
-
-            # Convert the image to a format that can be used by Tkinter
-            photo = ImageTk.PhotoImage(resized_image)
-
-            # Create a label with the resized image
-            image_label = tk.Label(self.main_frame, image=photo)
-            image_label.image = photo # Keep a reference to the image to prevent it from being garbage collected
+            image_label = self.put_image_in_label(self.main_frame, local_filesystem.vehicle_image_filepath(), 100)
             image_label.pack(side=tk.RIGHT, anchor=tk.NE, padx=(4, 4), pady=(4, 0))
-            # pylint: enable=duplicate-code
             show_tooltip(image_label, "Replace the vehicle.jpg file in the vehicle directory to change the vehicle image.")
         else:
             image_label = tk.Label(self.main_frame, text="No vehicle.jpg image file found on the vehicle directory.")
             image_label.pack(side=tk.RIGHT, anchor=tk.NE, padx=(4, 4), pady=(4, 0))
 
         self.scroll_frame = ScrollFrame(self.root)
         self.scroll_frame.pack(side="top", fill="both", expand=True)
 
-        self.populate_frames()
+        self.__populate_frames()
 
         self.save_button = ttk.Button(self.root, text="Save data and start configuration", command=self.save_data)
+        show_tooltip(self.save_button, "Save component data and start parameter value configuration and tuning.")
         self.save_button.pack(pady=7)
 
-    def populate_frames(self):
+    def __populate_frames(self):
         """
         Populates the ScrollFrame with widgets based on the JSON data.
         """
         if "Components" in self.data:
             for key, value in self.data["Components"].items():
-                self.add_widget(self.scroll_frame.view_port, key, value, [])
+                self.__add_widget(self.scroll_frame.view_port, key, value, [])
 
-    def add_widget(self, parent, key, value, path):
+    def __add_widget(self, parent, key, value, path):
         """
         Adds a widget to the parent widget with the given key and value.
 
         Parameters:
         parent (tkinter.Widget): The parent widget to which the LabelFrame/Entry will be added.
         key (str): The key for the LabelFrame/Entry.
         value (dict): The value associated with the key.
@@ -144,51 +113,74 @@
             is_toplevel = parent == self.scroll_frame.view_port
             side = tk.TOP if is_toplevel else tk.LEFT
             pady = 5 if is_toplevel else 3
             anchor = tk.NW if is_toplevel else tk.N
             frame.pack(fill=tk.X, side=side, pady=pady, padx=5, anchor=anchor)
             for sub_key, sub_value in value.items():
                 # recursively add child elements
-                self.add_widget(frame, sub_key, sub_value, path + [key])
+                self.__add_widget(frame, sub_key, sub_value, path + [key])
         else:                                   # JSON leaf elements, add Entry widget
             entry_frame = ttk.Frame(parent)
             entry_frame.pack(side=tk.TOP, fill=tk.X, pady=(0, 5))
 
             label = ttk.Label(entry_frame, text=key)
             label.pack(side=tk.LEFT)
 
-            entry = ttk.Entry(entry_frame)
-            entry.insert(0, str(value))
+            entry = self.add_entry_or_combobox(value, entry_frame, tuple(path+[key]))
             entry.pack(side=tk.LEFT, expand=True, fill=tk.X, padx=(0, 5))
 
             # Store the entry widget in the entry_widgets dictionary for later retrieval
             self.entry_widgets[tuple(path+[key])] = entry
 
     def save_data(self):
         """
         Saves the edited JSON data back to the file.
         """
         for path, entry in self.entry_widgets.items():
             value = entry.get()
-
-            # Navigate through the nested dictionaries using the elements of path
+            # Navigate through the nested dictionaries using the elements of the path
             current_data = self.data["Components"]
             for key in path[:-1]:
                 current_data = current_data[key]
 
+            if path[-1] != "Version":
+                try:
+                    value = int(value)
+                except ValueError:
+                    try:
+                        value = float(value)
+                    except ValueError:
+                        value = str(value)
+
             # Update the value in the data dictionary
             current_data[path[-1]] = value
 
         # Save the updated data back to the JSON file
-        self.local_filesystem.save_vehicle_components_json_data(self.data)
-        logging_info("Data saved successfully.")
+        if self.local_filesystem.save_vehicle_components_json_data(self.data, self.local_filesystem.vehicle_dir):
+            show_error_message("Error", "Failed to save data to file. Is the destination write protected?")
+        else:
+            logging_info("Data saved successfully.")
         self.root.destroy()
 
+    # This function will be overwritten in child classes
+    def add_entry_or_combobox(self, value, entry_frame, path):  # pylint: disable=unused-argument
+        entry = ttk.Entry(entry_frame)
+        entry.insert(0, str(value))
+        return entry
+
+    @staticmethod
+    def add_argparse_arguments(parser):
+        parser.add_argument('--skip-component-editor',
+                            action='store_true',
+                            help='Skip the component editor window. Only use this if all components have been configured. '
+                            'Default to false')
+        return parser
+
 
 if __name__ == "__main__":
     args = argument_parser()
 
     logging_basicConfig(level=logging_getLevelName(args.loglevel), format='%(asctime)s - %(levelname)s - %(message)s')
 
     filesystem = LocalFilesystem(args.vehicle_dir, args.vehicle_type)
-    app = JsonEditorApp(VERSION, filesystem)
+    app = ComponentEditorWindowBase(VERSION, filesystem)
     app.root.mainloop()
```

### Comparing `methodicconfigurator-0.2.2/MethodicConfigurator/extract_param_defaults.py` & `methodicconfigurator-0.4.0/MethodicConfigurator/extract_param_defaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
 
     Returns:
         None
     """
     if format_type == "qgcs":
         if sysid == -1:
             if 'SYSID_THISMAV' in params:
-                sysid = params['SYSID_THISMAV']
+                sysid = int(params['SYSID_THISMAV'])
             else:
                 sysid = 1  # if unspecified, default to 1
         if compid == -1:
             compid = 1  # if unspecified, default to 1
         if sysid < 0:
             raise SystemExit(f"Invalid system ID parameter {sysid} must not be negative")
         if sysid > MAVLINK_SYSID_MAX-1:
```

### Comparing `methodicconfigurator-0.2.2/MethodicConfigurator/frontend_tkinter.py` & `methodicconfigurator-0.4.0/MethodicConfigurator/frontend_tkinter_parameter_editor.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,48 +4,124 @@
 This file is part of Ardupilot methodic configurator. https://github.com/ArduPilot/MethodicConfigurator
 
 (C) 2024 Amilcar do Carmo Lucas, IAV GmbH
 
 SPDX-License-Identifier:    GPL-3
 '''
 
-from sys import exit as sys_exit
-
 import tkinter as tk
 from tkinter import messagebox
 from tkinter import ttk
+from tkinter import filedialog
 
-from logging import debug as logging_debug
+#from logging import debug as logging_debug
 from logging import info as logging_info
 from logging import warning as logging_warning
 from logging import error as logging_error
-from logging import critical as logging_critical
+#from logging import critical as logging_critical
 
 from typing import List
 from typing import Tuple
 
 from webbrowser import open as webbrowser_open  # to open the blog post documentation
 
-from PIL import Image
-from PIL import ImageTk
-
 from backend_filesystem import LocalFilesystem
 from backend_filesystem import is_within_tolerance
 
 from backend_flightcontroller import FlightController
 
 from frontend_tkinter_base import show_tooltip
 from frontend_tkinter_base import AutoResizeCombobox
-from frontend_tkinter_base import ScrollFrame
+from frontend_tkinter_base import ProgressWindow
 from frontend_tkinter_base import BaseWindow
 
 from frontend_tkinter_connection_selection import ConnectionSelectionWidgets
 
 from frontend_tkinter_directory_selection import VehicleDirectorySelectionWidgets
 
+from frontend_tkinter_parameter_editor_table import ParameterEditorTable
+
+from tempcal_imu import IMUfit
+
+
+class DocumentationFrame:  # pylint: disable=too-few-public-methods
+    """
+    A class to manage and display documentation within the GUI.
+
+    This class is responsible for creating a frame that displays
+    documentation links related to the current file being edited. It updates
+    the documentation links based on the current file and provides
+    functionality to open these links in a web browser.
+    """
+    def __init__(self, root: tk.Tk, local_filesystem, current_file: str):
+        self.root = root
+        self.local_filesystem = local_filesystem
+        self.current_file = current_file
+        self.documentation_frame = None
+        self.documentation_labels = {}
+        self.__create_documentation_frame()
+
+    def __create_documentation_frame(self):
+        self.documentation_frame = tk.LabelFrame(self.root, text="Documentation")
+        self.documentation_frame.pack(side=tk.TOP, fill="x", expand=False, pady=(4, 4), padx=(4, 4))
+
+        # Create a grid structure within the documentation_frame
+        documentation_grid = tk.Frame(self.documentation_frame)
+        documentation_grid.pack(fill="both", expand=True)
+
+        descriptive_texts = ["Forum Blog:", "Wiki:", "External tool:", "Mandatory:"]
+        descriptive_tooltips = ["ArduPilot's forum Methodic configuration Blog post relevant for the current file",
+                                "ArduPilot's wiki page relevant for the current file",
+                                "External tool or documentation relevant for the current file",
+                                "Mandatory level of the current file,\n 100% you MUST use this file to configure the "
+                                "vehicle,\n 0% you can ignore this file if it does not apply to your vehicle"]
+        for i, text in enumerate(descriptive_texts):
+            # Create labels for the first column with static descriptive text
+            label = tk.Label(documentation_grid, text=text)
+            label.grid(row=i, column=0, sticky="w")
+            show_tooltip(label, descriptive_tooltips[i])
+
+            # Create labels for the second column with the documentation links
+            self.documentation_labels[text] = tk.Label(documentation_grid)
+            self.documentation_labels[text].grid(row=i, column=1, sticky="w")
+
+        # Dynamically update the documentation text and URL links
+        self.update_documentation_labels(self.current_file)
+
+    def update_documentation_labels(self, current_file: str):
+        self.current_file = current_file
+        if current_file:
+            frame_title = f"{current_file} Documentation"
+        else:
+            frame_title = "Documentation"
+        self.documentation_frame.config(text=frame_title)
+
+        blog_text, blog_url = self.local_filesystem.get_documentation_text_and_url(current_file, 'blog')
+        self.__update_documentation_label('Forum Blog:', blog_text, blog_url)
+        wiki_text, wiki_url = self.local_filesystem.get_documentation_text_and_url(current_file, 'wiki')
+        self.__update_documentation_label('Wiki:', wiki_text, wiki_url)
+        external_tool_text, external_tool_url = self.local_filesystem.get_documentation_text_and_url(current_file,
+                                                                                                     'external_tool')
+        self.__update_documentation_label('External tool:', external_tool_text, external_tool_url)
+        mandatory_text, mandatory_url = self.local_filesystem.get_documentation_text_and_url(current_file,
+                                                                                             'mandatory')
+        self.__update_documentation_label('Mandatory:', mandatory_text, mandatory_url, False)
+
+    def __update_documentation_label(self, label_key, text, url, url_expected=True):
+        label = self.documentation_labels[label_key]
+        if url:
+            label.config(text=text, fg="blue", cursor="hand2", underline=True)
+            label.bind("<Button-1>", lambda event, url=url: webbrowser_open(url))
+            show_tooltip(label, url)
+        else:
+            label.config(text=text, fg="black", cursor="arrow", underline=False)
+            label.bind("<Button-1>", lambda event: None)
+            if url_expected:
+                show_tooltip(label, "Documentation URL not available")
+
 
 def show_about_window(root, version: str):
     # Create a new window for the custom "About" message
     about_window = tk.Toplevel(root)
     about_window.title("About")
     about_window.geometry("650x220")
 
@@ -78,76 +154,77 @@
     user_manual_button.pack(side=tk.LEFT, padx=10, pady=10)
     support_forum_button.pack(side=tk.LEFT, padx=10, pady=10)
     report_bug_button.pack(side=tk.LEFT, padx=10, pady=10)
     credits_button.pack(side=tk.LEFT, padx=10, pady=10)
     source_button.pack(side=tk.LEFT, padx=10, pady=10)
 
 
-
-class ParameterEditorWindow(BaseWindow):  # pylint: disable=too-many-instance-attributes, too-many-public-methods
+class ParameterEditorWindow(BaseWindow):  # pylint: disable=too-many-instance-attributes
     """
     This class is responsible for creating and managing the graphical user interface (GUI)
     for the ArduPilot methodic configurator. It inherits from the BaseWindow class
     and provides functionalities for displaying and interacting with drone
     parameters, documentation, and flight controller connection settings.
     """
     def __init__(self, current_file: str, flight_controller: FlightController,
                  local_filesystem: LocalFilesystem, version: str):
         super().__init__()
         self.current_file = current_file
         self.flight_controller = flight_controller
         self.local_filesystem = local_filesystem
 
-        self.at_least_one_param_edited = False
         self.at_least_one_changed_parameter_written = False
-        self.write_checkbutton_var = {}
         self.file_selection_combobox = None
-        self.documentation_label_blog = None
-        self.documentation_label_wiki = None
-        self.documentation_label_extra = None
-        self.documentation_label_mandatory = None
         self.show_only_differences = None
-        self.scroll_frame = None
+        self.annotate_params_into_files = None
+        self.parameter_editor_table = None
         self.reset_progress_window = None
-        self.reset_progress_bar = None
-        self.reset_progress_label = None
         self.param_read_progress_window = None
-        self.param_read_progress_bar = None
-        self.param_read_progress_label = None
+        self.tempcal_imu_progress_window = None
 
-        self.root.title("Amilcar Lucas's - ArduPilot methodic configurator - " + version)
+        self.root.title("Amilcar Lucas's - ArduPilot methodic configurator - " + version + " - Parameter editor")
         self.root.geometry("880x500") # Set the window width
 
         # Bind the close_connection_and_quit function to the window close event
         self.root.protocol("WM_DELETE_WINDOW", self.close_connection_and_quit)
 
-        self.__create_widgets(version)
+        self.__create_conf_widgets(version)
+
+        # Create a DocumentationFrame object for the Documentation Content
+        self.documentation_frame = DocumentationFrame(self.root, self.local_filesystem, self.current_file)
 
-    def __create_widgets(self, version: str):  # pylint: disable=too-many-locals, too-many-statements
+        self.__create_parameter_area_widgets()
+
+        self.root.after(50, self.read_flight_controller_parameters(reread=False)) # 50 milliseconds
+        self.root.after(50, self.__please_read_the_docs())
+        self.root.mainloop()
+
+    def __create_conf_widgets(self, version: str):
         config_frame = tk.Frame(self.root)
         config_frame.pack(side=tk.TOP, fill="x", expand=False, pady=(4, 0)) # Pack the frame at the top of the window
 
         config_subframe = tk.Frame(config_frame)
         config_subframe.pack(side=tk.LEFT, fill="x", expand=True, anchor=tk.NW) # Pack the frame at the top of the window
 
         # Create a new frame inside the config_subframe for the intermediate parameter file directory selection labels
         # and directory selection button
         directory_selection_frame = VehicleDirectorySelectionWidgets(self, config_subframe, self.local_filesystem,
+                                                                     self.local_filesystem.vehicle_dir,
                                                                      destroy_parent_on_open=False)
         directory_selection_frame.container_frame.pack(side=tk.LEFT, fill="x", expand=False, padx=(4, 6))
 
         # Create a new frame inside the config_subframe for the intermediate parameter file selection label and combobox
         file_selection_frame = tk.Frame(config_subframe)
         file_selection_frame.pack(side=tk.LEFT, fill="x", expand=False, padx=(6, 6))
 
-        # Create a label for the combobox
+        # Create a label for the Combobox
         file_selection_label = tk.Label(file_selection_frame, text="Current intermediate parameter file:")
         file_selection_label.pack(side=tk.TOP, anchor=tk.NW) # Add the label to the top of the file_selection_frame
 
-        # Create combobox for intermediate parameter file selection
+        # Create Combobox for intermediate parameter file selection
         self.file_selection_combobox = AutoResizeCombobox(file_selection_frame,
                                                           list(self.local_filesystem.file_parameters.keys()),
                                                           self.current_file,
                                                           "Select the intermediate parameter file from the list of available "
                                                           "files in the selected vehicle directory\nIt will automatically "
                                                           "advance to the next file once the current file is written to the "
                                                           "fight controller",
@@ -156,413 +233,165 @@
         self.file_selection_combobox.pack(side=tk.TOP, anchor=tk.NW, pady=(4, 0))
 
         # Create a new frame inside the config_subframe for the flight controller connection selection label and combobox
         csw = ConnectionSelectionWidgets(self, config_subframe, self.flight_controller,
                                          destroy_parent_on_connect=False, read_params_on_connect=True)
         csw.container_frame.pack(side=tk.RIGHT, fill="x", expand=False, padx=(6, 4))
 
-        # Load the ArduPilot logo and scale it down to image_height pixels in height
-        image_height = 40
-        image = Image.open(LocalFilesystem.application_logo_filepath())
-        width, height = image.size
-        aspect_ratio = width / height
-        new_width = int(image_height * aspect_ratio)
-        resized_image = image.resize((new_width, image_height))
-
-        # Convert the image to a format that can be used by Tkinter
-        photo = ImageTk.PhotoImage(resized_image)
-
-        # Create a label with the resized image
-        image_label = tk.Label(config_frame, image=photo)
-        image_label.image = photo # Keep a reference to the image to prevent it from being garbage collected
+        image_label = BaseWindow.put_image_in_label(config_frame, LocalFilesystem.application_logo_filepath())
         image_label.pack(side=tk.RIGHT, anchor=tk.NE, padx=(4, 4), pady=(4, 0))
         image_label.bind("<Button-1>", lambda event: show_about_window(self.root, version))
         show_tooltip(image_label, "User Manual, Support Forum, Report a Bug, Credits, Source Code")
 
-        # Create a Frame for the Documentation Content
-        documentation_frame = tk.LabelFrame(self.root, text="Documentation")
-        documentation_frame.pack(side=tk.TOP, fill="x", expand=False, pady=(4, 4), padx=(4, 4))
-
-        # Create a grid structure within the documentation_frame
-        documentation_grid = tk.Frame(documentation_frame)
-        documentation_grid.pack(fill="both", expand=True)
-
-        # Create labels for the first column with static descriptive text
-        descriptive_texts = ["Forum Blog:", "Wiki:", "External tool:", "Mandatory:"]
-        descriptive_tooltips = ["ArduPilot's forum Methodic configuration Blog post relevant for the current file",
-                                "ArduPilot's wiki page relevant for the current file",
-                                "External tool or documentation relevant for the current file",
-                                "Mandatory level of the current file,\n 100% you MUST use this file to configure the "
-                                "vehicle,\n 0% you can ignore this file if it does not apply to your vehicle"]
-        for i, text in enumerate(descriptive_texts):
-            label = tk.Label(documentation_grid, text=text)
-            label.grid(row=i, column=0, sticky="w")
-            show_tooltip(label, descriptive_tooltips[i])
-
-        # Create labels for the second column with the documentation links
-        self.documentation_label_blog = tk.Label(documentation_grid)
-        self.documentation_label_wiki = tk.Label(documentation_grid)
-        self.documentation_label_extra = tk.Label(documentation_grid)
-        self.documentation_label_mandatory = tk.Label(documentation_grid)
-
-        # Grid the documentation labels in the second column
-        self.documentation_label_blog.grid(row=0, column=1, sticky="w")
-        self.documentation_label_wiki.grid(row=1, column=1, sticky="w")
-        self.documentation_label_extra.grid(row=2, column=1, sticky="w")
-        self.documentation_label_mandatory.grid(row=3, column=1, sticky="w")
-
-        # Dynamically update the documentation text and URL links
-        self.update_documentation_labels()
-
+    def __create_parameter_area_widgets(self):
         self.show_only_differences = tk.BooleanVar(value=False)
+        self.annotate_params_into_files = tk.BooleanVar(value=False)
 
-        # Create a Frame for the Scrollable Content
-        self.scroll_frame = ScrollFrame(self.root)
+        # Create a Scrollable parameter editor table
+        self.parameter_editor_table = ParameterEditorTable(self.root, self.local_filesystem)
         self.repopulate_parameter_table(self.current_file)
-        self.scroll_frame.pack(side="top", fill="both", expand=True)
+        self.parameter_editor_table.pack(side="top", fill="both", expand=True)
 
         # Create a frame for the buttons
         buttons_frame = tk.Frame(self.root)
         buttons_frame.pack(side="bottom", fill="x", expand=False, pady=(10, 10))
 
-        # Create checkbox for toggling parameter display
-        only_changed_checkbox = ttk.Checkbutton(buttons_frame, text="See only changed parameters",
+        # Create a frame for the checkboxes
+        checkboxes_frame = tk.Frame(buttons_frame)
+        checkboxes_frame.pack(side=tk.LEFT, padx=(8, 8))
+
+        # Create a checkbox for toggling parameter display
+        only_changed_checkbox = ttk.Checkbutton(checkboxes_frame, text="See only changed parameters",
                                                 variable=self.show_only_differences,
                                                 command=self.on_show_only_changed_checkbox_change)
-        only_changed_checkbox.pack(side=tk.LEFT, padx=(8, 8))
+        only_changed_checkbox.pack(side=tk.TOP, anchor=tk.NW)
         show_tooltip(only_changed_checkbox, "Toggle to show only parameters that will change if/when written to the flight "
                      "controller")
 
+        annotate_params_checkbox = ttk.Checkbutton(checkboxes_frame, text="Annotate docs into .param files",
+                                                   state='normal' if self.local_filesystem.doc_dict else 'disabled',
+                                                   variable=self.annotate_params_into_files)
+        annotate_params_checkbox.pack(side=tk.TOP, anchor=tk.NW)
+        show_tooltip(annotate_params_checkbox, "Annotate ArduPilot parameter documentation metadata into the intermediate "
+                     "parameter files\n"
+                     "The files will be bigger, but all the existing parameter documentation will be included inside")
+
         # Create write button
         write_selected_button = tk.Button(buttons_frame, text="Write selected params to FC, and advance to next param file",
                                           command=self.on_write_selected_click)
         write_selected_button.pack(side=tk.LEFT, padx=(8, 8)) # Add padding on both sides of the write selected button
         show_tooltip(write_selected_button, "Write selected parameters to the flight controller and advance to the next "
                      "intermediate parameter file\nIf changes have been made to the current file it will ask if you want "
                      "to save them\nIt will reset the FC if necessary, re-read all parameters and validate their value")
 
         # Create skip button
         skip_button = tk.Button(buttons_frame, text="Skip parameter file", command=self.on_skip_click)
         skip_button.pack(side=tk.RIGHT, padx=(8, 8)) # Add right padding to the skip button
         show_tooltip(skip_button, "Skip to the next intermediate parameter file without writing any changes to the flight "
                      "controller\nIf changes have been made to the current file it will ask if you want to save them")
 
-        self.root.after(50, self.read_flight_controller_parameters(reread=False)) # 50 milliseconds
-        self.root.mainloop()
+    @staticmethod
+    def __please_read_the_docs():
+        messagebox.showinfo("Welcome to the ArduPilot Methodic Configurator",
+                            "Please read ALL the documentation on top of the parameter table"
+                            " before editing the parameters and the reason they changed")
+
+    def __do_tempcal_imu(self, selected_file:str):
+        tempcal_imu_result_param_filename, tempcal_imu_result_param_fullpath = \
+           self.local_filesystem.tempcal_imu_result_param_tuple()
+        if selected_file == tempcal_imu_result_param_filename:
+            if messagebox.askyesno("IMU temperature calibration",
+                                    f"If you proceed the {tempcal_imu_result_param_filename}\n"
+                                    "will be overwritten with the new calibration results.\n"
+                                    "Do you want to provide a .bin log file and\n"
+                                    "run the IMU temperature calibration using it?"):
+                # file selection dialog to select the *.bin file to be used in the IMUfit temperature calibration
+                filename = filedialog.askopenfilename(filetypes=[("ArduPilot binary log files", ["*.bin", "*.BIN"])])
+                if filename:
+                    messagebox.showwarning("IMU temperature calibration", "Please wait, this can take a really long time and\n"
+                                           "the GUI will be unresponsive until it finishes.")
+                    self.tempcal_imu_progress_window = ProgressWindow(self.root, "Reading IMU calibration messages",
+                                                                      "Please wait, this can take a long time")
+                    # Pass the selected filename to the IMUfit class
+                    IMUfit(filename, tempcal_imu_result_param_fullpath, False, False, False, False,
+                            self.local_filesystem.vehicle_dir, self.tempcal_imu_progress_window.update_progress_bar_300_pct)
+                    self.tempcal_imu_progress_window.destroy()
+                    self.local_filesystem.file_parameters = self.local_filesystem.read_params_from_files()
+                    self.parameter_editor_table.set_at_least_one_param_edited(True)  # force writing doc annotations to file
+
+    def __should_copy_fc_values_to_file(self, selected_file):
+        auto_changed_by = self.local_filesystem.auto_changed_by(selected_file)
+        if auto_changed_by and self.flight_controller.fc_parameters:
+            if messagebox.askyesno("Update file with values from FC?",
+                                   "This configuration step should be performed outside this tool by\n"
+                                   f"{auto_changed_by}\n"
+                                   "and that should have changed the parameters on the FC.\n\n"
+                                   f"Should the FC values now be copied to the {selected_file} file?"):
+                relevant_fc_params = {key: value for key, value in self.flight_controller.fc_parameters.items() \
+                                      if key in self.local_filesystem.file_parameters[selected_file]}
+                params_copied = self.local_filesystem.copy_fc_values_to_file(selected_file, relevant_fc_params)
+                if params_copied:
+                    self.parameter_editor_table.set_at_least_one_param_edited(True)
 
     def on_param_file_combobox_change(self, _event, forced: bool = False):
         if not self.file_selection_combobox['values']:
             return
-        self.param_edit_widgets_event_generate_focus_out()
+        self.parameter_editor_table.generate_edit_widgets_focus_out()
         selected_file = self.file_selection_combobox.get()
         if self.current_file != selected_file or forced:
             self.write_changes_to_intermediate_parameter_file()
+            self.__do_tempcal_imu(selected_file)
+            self.__should_copy_fc_values_to_file(selected_file)
+
             # Update the current_file attribute to the selected file
             self.current_file = selected_file
             self.at_least_one_changed_parameter_written = False
-            self.update_documentation_labels()
+            self.documentation_frame.update_documentation_labels(selected_file)
             self.repopulate_parameter_table(selected_file)
 
     def read_flight_controller_parameters(self, reread: bool = False):
-        [self.param_read_progress_window,
-         self.param_read_progress_bar,
-         self.param_read_progress_label] = self.create_progress_window(("Re-r" if reread else "R") + "eading FC parameters")
+        self.param_read_progress_window = ProgressWindow(self.root, ("Re-r" if reread else "R") + "eading FC parameters",
+                                                         "Read {} of {} parameters")
         # Download all parameters from the flight controller
-        self.flight_controller.fc_parameters = self.flight_controller.read_params(self.update_param_download_progress_bar)
-        self.param_read_progress_window.destroy()  # for the case that we are doing test and there is no real FC connected
+        self.flight_controller.fc_parameters = self.flight_controller.read_params(
+            self.param_read_progress_window.update_progress_bar)
+        self.param_read_progress_window.destroy()  # for the case that we are doing a test and there is no real FC connected
         if not reread:
             self.on_param_file_combobox_change(None, True) # the initial param read will trigger a table update
 
-    def get_documentation_text_and_url(self, documentation, text_key, url_key):
-        if documentation:
-            text = documentation.get(text_key, f"No documentation available for {self.current_file} in the "
-                                     f"{self.local_filesystem.file_documentation_filename} file")
-            url = documentation.get(url_key, None)
-        else:
-            text = f"File '{self.local_filesystem.file_documentation_filename}' not found. No intermediate parameter " \
-                "file documentation available"
-            url = None
-        return text, url
-
-    def update_documentation_label(self, label, text, url, url_expected=True):
-        if url:
-            label.config(text=text, fg="blue", cursor="hand2", underline=True)
-            label.bind("<Button-1>", lambda event, url=url: webbrowser_open(url))
-            show_tooltip(label, url)
-        else:
-            label.config(text=text, fg="black", cursor="arrow", underline=False)
-            label.bind("<Button-1>", lambda event: None)
-            if url_expected:
-                show_tooltip(label, "Documentation URL not available")
-
-    def update_documentation_labels(self):
-        documentation = self.local_filesystem.file_documentation.get(self.current_file, None) if \
-            self.local_filesystem.file_documentation else None
-
-        blog_text, blog_url = self.get_documentation_text_and_url(documentation, 'blog_text', 'blog_url')
-        self.update_documentation_label(self.documentation_label_blog, blog_text, blog_url)
-        wiki_text, wiki_url = self.get_documentation_text_and_url(documentation, 'wiki_text', 'wiki_url')
-        self.update_documentation_label(self.documentation_label_wiki, wiki_text, wiki_url)
-        external_tool_text, external_tool_url = self.get_documentation_text_and_url(documentation, 'external_tool_text',
-                                                                                    'external_tool_url')
-        self.update_documentation_label(self.documentation_label_extra, external_tool_text, external_tool_url)
-        mandatory_text, mandatory_url = self.get_documentation_text_and_url(documentation, 'mandatory_text', 'mandatory_url')
-        self.update_documentation_label(self.documentation_label_mandatory, mandatory_text, mandatory_url, False)
-
     def repopulate_parameter_table(self, selected_file):
         if not selected_file:
             return  # no file was yet selected, so skip it
         if hasattr(self.flight_controller, 'fc_parameters') and self.flight_controller.fc_parameters:
             fc_parameters = self.flight_controller.fc_parameters
         else:
             fc_parameters = {}
-        # Different parameters based on the thresholdfile_value
+        # Different parameters based on the tolerance value
         different_params = {param_name: file_value for param_name, file_value in
                             self.local_filesystem.file_parameters[selected_file].items()
                             if param_name not in fc_parameters or (param_name in fc_parameters and \
                                 not is_within_tolerance(fc_parameters[param_name], float(file_value.value)))}
         if not different_params and self.show_only_differences.get():
             logging_info("No different parameters found in %s. Skipping...", selected_file)
             messagebox.showinfo("ArduPilot methodic configurator",
                                 f"No different parameters found in {selected_file}. Skipping...")
             self.on_skip_click(force_focus_out_event=False)
             return
-        # Clear the current table
-        for widget in self.scroll_frame.view_port.winfo_children():
-            widget.destroy()
-        # Repopulate the table with the new parameters
-        if self.show_only_differences.get():
-            self.update_table(different_params, fc_parameters)
-        else:
-            self.update_table(self.local_filesystem.file_parameters[selected_file], fc_parameters)
-        # Scroll to the top of the parameter table
-        self.scroll_frame.canvas.yview("moveto", 0)
-
-    def update_table(self, params, fc_parameters):  # pylint: disable=too-many-locals, too-many-statements
-        # Create labels for table headers
-        headers = ["Parameter", "Current Value", "New Value", "Unit", "Write", "Change Reason"]
-        tooltips = ["Parameter name must be ^[A-Z][A-Z_0-9]* and most 16 characters long",
-                    "Current value on the flight controller ",
-                    "New value from the above selected intermediate parameter file",
-                    "Parameter Unit",
-                    "When selected, write new value to the flight controller",
-                    "Reason why respective parameter changed"]
-        for i, header in enumerate(headers):
-            label = tk.Label(self.scroll_frame.view_port, text=header)
-            label.grid(row=0, column=i, sticky="ew") # Use sticky="ew" to make the label stretch horizontally
-            show_tooltip(label, tooltips[i])
-
-        self.write_checkbutton_var = {}
-        try:
-            # Create the new table
-            for i, (param_name, param) in enumerate(params.items()):
-                param_metadata = self.local_filesystem.doc_dict.get(param_name, None)
-                param_default = self.local_filesystem.param_default_dict.get(param_name, None)
-
-                is_calibration = param_metadata.get('Calibration', False) if param_metadata else False
-                is_readonly = param_metadata.get('ReadOnly', False) if param_metadata else False
-                parameter_label = tk.Label(self.scroll_frame.view_port, text=param_name + (" " * (16 - len(param_name))),
-                                           background="red" if is_readonly else "yellow" if is_calibration else
-                                           self.default_background_color)
-                if param_name in fc_parameters:
-                    value_str = format(fc_parameters[param_name], '.6f').rstrip('0').rstrip('.')
-                    if param_default is not None and is_within_tolerance(fc_parameters[param_name], param_default.value):
-                        # If it matches, set the background color to light blue
-                        flightcontroller_value = tk.Label(self.scroll_frame.view_port, text=value_str,
-                                                          background="light blue")
-                    else:
-                        # Otherwise, set the background color to the default color
-                        flightcontroller_value = tk.Label(self.scroll_frame.view_port, text=value_str)
-                else:
-                    flightcontroller_value = tk.Label(self.scroll_frame.view_port, text="N/A", background="blue")
-
-                new_value_background = "light blue" if param_default is not None and \
-                    is_within_tolerance(param.value, param_default.value) else "white"
-                new_value_entry = tk.Entry(self.scroll_frame.view_port, width=10, justify=tk.RIGHT,
-                                           background=new_value_background)
-                new_value_entry.insert(0, format(param.value, '.6f').rstrip('0').rstrip('.'))
-                new_value_entry.bind("<FocusOut>", lambda event, current_file=self.current_file, param_name=param_name:
-                                     self.on_parameter_value_change(event, current_file, param_name))
-
-                unit_label = tk.Label(self.scroll_frame.view_port, text=param_metadata.get('unit') if param_metadata else "")
-
-                self.write_checkbutton_var[param_name] = tk.BooleanVar(value=True) # Default to selected
-                write_write_checkbutton = ttk.Checkbutton(self.scroll_frame.view_port,
-                                                          variable=self.write_checkbutton_var[param_name])
-
-                change_reason_entry = tk.Entry(self.scroll_frame.view_port, background="white")
-                change_reason_entry.insert(0, "" if param.comment is None else param.comment)
-                change_reason_entry.bind("<FocusOut>", lambda event, current_file=self.current_file, param_name=param_name:
-                                         self.on_parameter_change_reason_change(event, current_file, param_name))
-
-                doc_tooltip = param_metadata.get('doc_tooltip') if param_metadata else \
-                    "No documentation available in apm.pdef.xml for this parameter"
-                if doc_tooltip:
-                    show_tooltip(parameter_label, doc_tooltip)
-                    show_tooltip(flightcontroller_value, doc_tooltip)
-                    show_tooltip(new_value_entry, doc_tooltip)
-                unit_tooltip = param_metadata.get('unit_tooltip') if param_metadata else \
-                    "No documentation available in apm.pdef.xml for this parameter"
-                if unit_tooltip:
-                    show_tooltip(unit_label, unit_tooltip)
-                show_tooltip(write_write_checkbutton, f'When selected write {param_name} new value to the flight controller')
-                show_tooltip(change_reason_entry, f'Reason why {param_name} should change to {new_value_entry.get()}')
-
-                row = [
-                    parameter_label,
-                    flightcontroller_value,
-                    new_value_entry,
-                    unit_label,
-                    write_write_checkbutton,
-                    change_reason_entry,
-                ]
-                for j, widget in enumerate(row):
-                    # Use sticky="ew" to make the widget stretch horizontally
-                    widget.grid(row=i+1, column=j,
-                                sticky="w" if j == 0 else "ew" if j == 5 else "e", padx=(0, 5) if j == 5 else 0)
-        except KeyError as e:
-            logging_critical("Parameter %s not found in the %s file: %s", param_name, self.current_file, e, exc_info=True)
-            sys_exit(1)
-
-        # Configure the table_frame to stretch columns
-        self.scroll_frame.view_port.columnconfigure(0, weight=0, minsize=120) # Parameter name
-        self.scroll_frame.view_port.columnconfigure(1, weight=0) # Current Value
-        self.scroll_frame.view_port.columnconfigure(2, weight=0) # New Value
-        self.scroll_frame.view_port.columnconfigure(3, weight=0) # Units
-        self.scroll_frame.view_port.columnconfigure(4, weight=0) # write to FC
-        self.scroll_frame.view_port.columnconfigure(5, weight=1) # Change reason
-
-    def on_parameter_value_change(self, event, current_file, param_name):
-        # Get the new value from the Entry widget
-        new_value = event.widget.get()
-        try:
-            old_value = self.local_filesystem.file_parameters[current_file][param_name].value
-        except KeyError as e:
-            logging_critical("Parameter %s not found in the %s file: %s", param_name, current_file, e, exc_info=True)
-            sys_exit(1)
-        valid = True
-        # Check if the input is a valid float
-        try:
-            p = float(new_value)
-            changed = not is_within_tolerance(old_value, p)
-            param_metadata = self.local_filesystem.doc_dict.get(param_name, None)
-            p_min = param_metadata.get('min', None) if param_metadata else None
-            p_max = param_metadata.get('max', None) if param_metadata else None
-            if changed:
-                if p_min and p < p_min:
-                    if not messagebox.askyesno("Out-of-bounds Value",
-                                               f"The value for {param_name} {p} should be greater than {p_min}\n"
-                                               "Use out-of-bounds value?", icon='warning'):
-                        valid = False
-                if p_max and p > p_max:
-                    if not messagebox.askyesno("Out-of-bounds Value",
-                                               f"The value for {param_name} {p} should be smaller than {p_max}\n"
-                                               "Use out-of-bounds value?", icon='warning'):
-                        valid = False
-        except ValueError:
-            # Optionally, you can handle the invalid value here, for example, by showing an error message
-            messagebox.showerror("Invalid Value", f"The value for {param_name} must be a valid float.")
-            valid = False
-        if valid:
-            if changed and not self.at_least_one_param_edited:
-                logging_debug("Parameter %s changed, will later ask if change(s) should be saved to file.", param_name)
-            self.at_least_one_param_edited = changed or self.at_least_one_param_edited
-            # Update the params dictionary with the new value
-            self.local_filesystem.file_parameters[current_file][param_name].value = p
-        else:
-            # Revert to the previous (valid) value
-            event.widget.delete(0, tk.END)
-            event.widget.insert(0, old_value)
-        # Update the background color of the new value Entry widget to light blue if the new value is the default value
-        param_default = self.local_filesystem.param_default_dict.get(param_name, None)
-        new_value_background = "light blue" if param_default is not None and \
-            is_within_tolerance(p, param_default.value) else "white"
-        event.widget.config(background=new_value_background)
-
-    def on_parameter_change_reason_change(self, event, current_file, param_name):
-        # Get the new value from the Entry widget
-        new_value = event.widget.get()
-        try:
-            changed = new_value != self.local_filesystem.file_parameters[current_file][param_name].comment and \
-                not (new_value == "" and self.local_filesystem.file_parameters[current_file][param_name].comment is None)
-        except KeyError as e:
-            logging_critical("Parameter %s not found in the %s file %s: %s", param_name, self.current_file,
-                             new_value, e, exc_info=True)
-            sys_exit(1)
-        if changed and not self.at_least_one_param_edited:
-            logging_debug("Parameter %s change reason changed from %s to %s, will later ask if change(s) should be saved to "
-                          "file.",
-                          param_name, self.local_filesystem.file_parameters[current_file][param_name].comment, new_value)
-        self.at_least_one_param_edited = changed or self.at_least_one_param_edited
-        # Update the params dictionary with the new value
-        self.local_filesystem.file_parameters[current_file][param_name].comment = new_value
-
-    def get_write_selected_params(self):
-        selected_params = {}
-        for param_name, checkbutton_state in self.write_checkbutton_var.items():
-            if checkbutton_state.get():
-                selected_params[param_name] = self.local_filesystem.file_parameters[self.current_file][param_name]
-        return selected_params
+        # Re-populate the table with the new parameters
+        self.parameter_editor_table.repopulate(selected_file, different_params,
+                                               fc_parameters, self.show_only_differences.get())
 
     def on_show_only_changed_checkbox_change(self):
         self.repopulate_parameter_table(self.current_file)
 
-    def update_reset_progress_bar(self, current_value: int, max_value: int):
-        """
-        Update the FC reset progress bar and the progress message with the current progress.
-
-        Args:
-            current_value (int): The current progress value.
-            max_value (int): The maximum progress value.
-        """
-        self.reset_progress_window.lift()
-
-        self.reset_progress_bar['value'] = current_value
-        self.reset_progress_bar['maximum'] = max_value
-        self.reset_progress_bar.update()
-
-        # Update the reset progress message
-        self.reset_progress_label.config(text=f"waiting for {current_value} of {max_value} seconds")
-
-        # Close the reset progress window when the process is complete
-        if current_value == max_value:
-            self.reset_progress_window.destroy()
-
-    def update_param_download_progress_bar(self, current_value: int, max_value: int):
-        """
-        Update the FC parameter read progress bar the progress message with the current progress.
-
-        Args:
-            current_value (int): The current progress value.
-            max_value (int): The maximum progress value.
-        """
-        self.param_read_progress_window.lift()
-
-        self.param_read_progress_bar['value'] = current_value
-        self.param_read_progress_bar['maximum'] = max_value
-        self.param_read_progress_bar.update()
-
-        # Update the param read progress message
-        self.param_read_progress_label.config(text=f"Reading parameter {current_value} of {max_value}")
-
-        # Close the param read progress window when the process is complete
-        if current_value == max_value:
-            self.param_read_progress_window.destroy()
-
-    def param_edit_widgets_event_generate_focus_out(self):
-        # Trigger the <FocusOut> event for all entry widgets to ensure all changes are processed
-        for widget in self.scroll_frame.view_port.winfo_children():
-            if isinstance(widget, tk.Entry):
-                widget.event_generate("<FocusOut>", when="now")
-
     def write_params_that_require_reset(self, selected_params: dict):
         """
         Write the selected parameters to the flight controller that require a reset.
 
-        After the reset, the other parameters that do not require a reset, must still be written to the flight controller.
+        After the reset, the other parameters that do not require a reset must still be written to the flight controller.
         """
         fc_reset_required = False
         fc_reset_unsure = []
 
         # Write each selected parameter to the flight controller
         for param_name, param in selected_params.items():
             try:
@@ -596,26 +425,25 @@
         if not fc_reset_required:
             if fc_reset_unsure:
                 # Ask the user if they want to reset the ArduPilot
                 fc_reset_required = messagebox.askyesno("Possible reset required", f"{(', ').join(fc_reset_unsure)} parameter"
                                                         "(s) potentially require a reset\nDo you want to reset the ArduPilot?")
 
         if fc_reset_required:
-            [self.reset_progress_window,
-             self.reset_progress_bar,
-             self.reset_progress_label] = self.create_progress_window("Resetting Flight Controller")
+            self.reset_progress_window = ProgressWindow(self.root, "Resetting Flight Controller",
+                                                        "Waiting for {} of {} seconds")
             # Call reset_and_reconnect with a callback to update the reset progress bar and the progress message
-            self.flight_controller.reset_and_reconnect(self.update_reset_progress_bar)
-            self.reset_progress_window.destroy()  # for the case that we are doing test and there is no real FC connected
+            self.flight_controller.reset_and_reconnect(self.reset_progress_window.update_progress_bar)
+            self.reset_progress_window.destroy()  # for the case that we are doing a test and there is no real FC connected
 
     def on_write_selected_click(self):
-        self.param_edit_widgets_event_generate_focus_out()
+        self.parameter_editor_table.generate_edit_widgets_focus_out()
 
         self.write_changes_to_intermediate_parameter_file()
-        selected_params = self.get_write_selected_params()
+        selected_params = self.parameter_editor_table.get_write_selected_params(self.current_file)
         if selected_params:
             if hasattr(self.flight_controller, 'fc_parameters') and self.flight_controller.fc_parameters:
                 self.write_selected_params(selected_params)
             else:
                 logging_warning("No parameters were yet read from the flight controller, will not write any parameter")
                 messagebox.showwarning("Will not write any parameter", "No flight controller connection")
         else:
@@ -639,15 +467,15 @@
                    not is_within_tolerance(self.flight_controller.fc_parameters[param_name], param.value):
                     self.at_least_one_changed_parameter_written = True
             except ValueError as e:
                 logging_error("Failed to set parameter %s: %s", param_name, e)
                 messagebox.showerror("ArduPilot methodic configurator", f"Failed to set parameter {param_name}: {e}")
 
         if self.at_least_one_changed_parameter_written:
-            # Re-Download all parameters, in case one of them changed, and to validate that all writes where successful
+            # Re-download all parameters, in case one of them changed, and validate that all writes were successful
             self.read_flight_controller_parameters(True)
             logging_info("Re-read all parameters from the flight controller")
 
             # Validate that the read parameters are the same as the ones in the current_file
             param_write_error = []
             for param_name, param in selected_params.items():
                 if param_name in self.flight_controller.fc_parameters and \
@@ -664,48 +492,49 @@
             if param_write_error:
                 if messagebox.askretrycancel("Parameter write error",
                                              "Failed to write the following parameters to the flight controller:\n"
                                              f"{(', ').join(param_write_error)}"):
                     self.write_selected_params(selected_params)
             else:
                 logging_info("All parameters written to the flight controller successfully")
+        self.local_filesystem.write_last_written_filename(self.current_file)
 
     def on_skip_click(self, _event=None, force_focus_out_event=True):
         if force_focus_out_event:
-            self.param_edit_widgets_event_generate_focus_out()
+            self.parameter_editor_table.generate_edit_widgets_focus_out()
         self.write_changes_to_intermediate_parameter_file()
         # Find the next filename in the file_parameters dictionary
         files = list(self.local_filesystem.file_parameters.keys())
         if not files:
             return
         try:
             next_file_index = files.index(self.current_file) + 1
             if next_file_index >= len(files):
                 self.write_summary_files()
                 # Close the application and the connection
                 self.close_connection_and_quit()
                 return
             next_file = files[next_file_index]
-            # Update the combobox selection to the next file
+            # Update the Combobox selection to the next file
             self.file_selection_combobox.set(next_file)
             # Trigger the combobox change event to update the table
             self.on_param_file_combobox_change(None)
         except ValueError:
             # If the current file is not found in the list, present a message box
             messagebox.showerror("ArduPilot methodic configurator", "Current file not found in the list of files")
             # Close the application and the connection
             self.close_connection_and_quit()
 
     def write_changes_to_intermediate_parameter_file(self):
-        if self.at_least_one_param_edited:
+        if self.parameter_editor_table.get_at_least_one_param_edited():
             if messagebox.askyesno("One or more parameters have been edited",
                                    f"Do you want to write the changes to the {self.current_file} file?"):
                 self.local_filesystem.export_to_param(self.local_filesystem.file_parameters[self.current_file],
-                                                      self.current_file, annotate_doc=False)
-        self.at_least_one_param_edited = False
+                                                      self.current_file, annotate_doc=self.annotate_params_into_files.get())
+        self.parameter_editor_table.set_at_least_one_param_edited(False)
 
     def write_summary_files(self):
         if not hasattr(self.flight_controller, 'fc_parameters') or self.flight_controller.fc_parameters is None:
             return
         annotated_fc_parameters = self.local_filesystem.annotate_intermediate_comments_to_param_dict(
             self.flight_controller.fc_parameters)
         non_default__read_only_params, non_default__writable_calibrations, non_default__writable_non_calibrations = \
@@ -759,8 +588,10 @@
             self.local_filesystem.zip_files(files_to_zip)
             messagebox.showinfo("Parameter files zipped", "All relevant files have been zipped into the \n"
                                 f"{zip_file_path} file.\n\nYou can now upload this file to the ArduPilot Methodic\n"
                                 "Configuration Blog post on discuss.ardupilot.org.")
         return should_write_file
 
     def close_connection_and_quit(self):
+        self.parameter_editor_table.generate_edit_widgets_focus_out()
+        self.write_changes_to_intermediate_parameter_file()
         self.root.quit() # Then stop the Tkinter event loop
```

### Comparing `methodicconfigurator-0.2.2/MethodicConfigurator/frontend_tkinter_base.py` & `methodicconfigurator-0.4.0/MethodicConfigurator/frontend_tkinter_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,20 +7,25 @@
 
 SPDX-License-Identifier:    GPL-3
 '''
 
 import tkinter as tk
 from tkinter import messagebox
 from tkinter import ttk
+
 # from logging import debug as logging_debug
 # from logging import info as logging_info
 from logging import warning as logging_warning
 from logging import error as logging_error
+
 from platform import system as platform_system
 
+from PIL import Image
+from PIL import ImageTk
+
 from backend_filesystem import LocalFilesystem
 
 
 def show_error_message(title: str, message: str):
     root = tk.Tk()
     # Set the theme to 'alt'
     style = ttk.Style()
@@ -144,27 +149,27 @@
         self.view_port.bind('<Leave>', self.on_leave)
 
         # perform an initial stretch on render, otherwise the scroll region has a tiny border until the first resize
         self.on_frame_configure(None)
 
     def on_frame_configure(self, _event):
         '''Reset the scroll region to encompass the inner frame'''
-        # whenever the size of the frame changes, alter the scroll region respectively.
+        # Whenever the size of the frame changes, alter the scroll region respectively.
         self.canvas.configure(scrollregion=self.canvas.bbox("all"))
         # Calculate the bounding box for the scroll region, starting from the second row
         # bbox = self.canvas.bbox("all")
         # if bbox:
         #     # Adjust the bounding box to start from the second row
         #     bbox = (bbox[0], bbox[1] + self.canvas.winfo_reqheight(), bbox[2], bbox[3])
         #     self.canvas.configure(scrollregion=bbox)
 
     def on_canvas_configure(self, event):
         '''Reset the canvas window to encompass inner frame when required'''
         canvas_width = event.width
-        # whenever the size of the canvas changes alter the window region respectively.
+        # Whenever the size of the canvas changes alter the window region respectively.
         self.canvas.itemconfig(self.canvas_window, width=canvas_width)
 
     def on_mouse_wheel(self, event):                       # cross platform scroll wheel event
         canvas_height = self.canvas.winfo_height()
         rows_height = self.canvas.bbox("all")[3]
 
         if rows_height > canvas_height: # only scroll if the rows overflow the frame
@@ -189,14 +194,79 @@
         if platform_system() == 'Linux':
             self.canvas.unbind_all("<Button-4>")
             self.canvas.unbind_all("<Button-5>")
         else:
             self.canvas.unbind_all("<MouseWheel>")
 
 
+class ProgressWindow:
+    """
+    A class for creating and managing a progress window in the application.
+
+    This class is responsible for creating a progress window that displays the progress of
+    a task. It includes a progress bar and a label to display the progress message.
+    """
+    def __init__(self, parent, title, message: str="", width:  int=300, height: int=80):  # pylint: disable=too-many-arguments
+        self.parent = parent
+        self.message = message
+        self.progress_window = None
+        self.progress_bar = None
+        self.progress_label = None
+        self.__create_progress_window(title, message, width, height)
+
+    def __create_progress_window(self, title: str, message, width, height):
+        self.progress_window = tk.Toplevel(self.parent)
+        self.progress_window.title(title)
+        self.progress_window.geometry(f"{width}x{height}")
+
+        # Create a progress bar
+        self.progress_bar = ttk.Progressbar(self.progress_window, length=100, mode='determinate')
+        self.progress_bar.pack(side=tk.TOP, fill=tk.X, expand=False, padx=(5, 5), pady=(10, 10))
+
+        # Create a label to display the progress message
+        self.progress_label = tk.Label(self.progress_window, text=message.format(0, 0))
+        self.progress_label.pack(side=tk.TOP, fill=tk.X, expand=False, pady=(10, 10))
+
+        self.progress_window.lift()
+
+        # Center the progress window on the parent window
+        BaseWindow.center_window(self.progress_window, self.parent)
+
+        self.progress_bar.update()
+
+    def update_progress_bar_300_pct(self, percent: int):
+        self.message = "Please be patient, {:.1f}% of {}% complete"
+        self.update_progress_bar(percent/3, max_value=100)
+
+    def update_progress_bar(self, current_value: int, max_value: int):
+        """
+        Update the progress bar and the progress message with the current progress.
+
+        Args:
+            current_value (int): The current progress value.
+            max_value (int): The maximum progress value, if 0 uses percentage.
+        """
+        self.progress_window.lift()
+
+        self.progress_bar['value'] = current_value
+        self.progress_bar['maximum'] = max_value
+
+        # Update the progress message
+        self.progress_label.config(text=self.message.format(current_value, max_value))
+
+        self.progress_bar.update()
+
+        # Close the progress window when the process is complete
+        if current_value == max_value:
+            self.progress_window.destroy()
+
+    def destroy(self):
+        self.progress_window.destroy()
+
+
 class BaseWindow:
     """
     A base class for creating windows in the ArduPilot Methodic Configurator application.
 
     This class provides a foundation for creating windows in the application, including setting up the
     root window, applying a theme, and configuring the application icon. It also includes methods for
     creating a progress window and centering a window on its parent.
@@ -218,33 +288,14 @@
         # Get the background color for the 'TFrame' widget
         self.default_background_color = '#f0f0f0' # style.lookup('TFrame', 'background')
 
         # Configure the background color for the checkbutton
         style.configure('TCheckbutton', background=self.default_background_color)
         style.configure('TCombobox', background=self.default_background_color)
 
-    def create_progress_window(self, title: str):
-        # Create a new window for the param_read progress bar
-        progress_window = tk.Toplevel(self.root)
-        progress_window.title(title)
-        progress_window.geometry("300x80")
-
-        # Center the param_read progress window on the main window
-        BaseWindow.center_window(progress_window, self.root)
-
-        # Create a param_read progress bar
-        progress_bar = ttk.Progressbar(progress_window, length=100, mode='determinate')
-        progress_bar.pack(side=tk.TOP, fill=tk.X, expand=False, padx=(5, 5), pady=(10, 10))
-
-        # Create a param_read label to display the progress message
-        progress_label = tk.Label(progress_window, text="")
-        progress_label.pack(side=tk.TOP, fill=tk.X, expand=False, pady=(10, 10))
-
-        return progress_window, progress_bar, progress_label
-
     @staticmethod
     def center_window(window, parent):
         """
         Center a window on its parent window.
 
         Args:
             window (tk.Toplevel): The window to center.
@@ -254,7 +305,24 @@
         parent_width = parent.winfo_width()
         parent_height = parent.winfo_height()
         window_width = window.winfo_width()
         window_height = window.winfo_height()
         x = parent.winfo_x() + (parent_width // 2) - (window_width // 2)
         y = parent.winfo_y() + (parent_height // 2) - (window_height // 2)
         window.geometry(f"+{x}+{y}")
+
+    @staticmethod
+    def put_image_in_label(parent: tk.Toplevel, filepath: str, image_height: int=40) -> tk.Label:
+        # Load the image and scale it down to image_height pixels in height
+        image = Image.open(filepath)
+        width, height = image.size
+        aspect_ratio = width / height
+        new_width = int(image_height * aspect_ratio)
+        resized_image = image.resize((new_width, image_height))
+
+        # Convert the image to a format that can be used by Tkinter
+        photo = ImageTk.PhotoImage(resized_image)
+
+        # Create a label with the resized image
+        image_label = tk.Label(parent, image=photo)
+        image_label.image = photo # Keep a reference to the image to prevent it from being garbage collected
+        return image_label
```

### Comparing `methodicconfigurator-0.2.2/MethodicConfigurator/frontend_tkinter_connection_selection.py` & `methodicconfigurator-0.4.0/MethodicConfigurator/frontend_tkinter_connection_selection.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,23 +18,24 @@
 from logging import warning as logging_warning
 from logging import critical as logging_critical
 
 import tkinter as tk
 from tkinter import ttk
 from tkinter import simpledialog
 
+from common_arguments import add_common_arguments_and_parse
+
 from backend_flightcontroller import FlightController
 
 from frontend_tkinter_base import show_no_connection_error
 from frontend_tkinter_base import show_tooltip
 from frontend_tkinter_base import update_combobox_width
+from frontend_tkinter_base import ProgressWindow
 from frontend_tkinter_base import BaseWindow
 
-from version import VERSION
-
 
 # https://dev.to/geraldew/python-tkinter-an-exercise-in-wrapping-the-combobox-ndb
 class PairTupleCombobox(ttk.Combobox):  # pylint: disable=too-many-ancestors
     """
     A custom Combobox widget that allows for the display of a list of tuples, where each tuple contains a key and a value.
     This widget processes the list of tuples to separate keys and values for display purposes, and allows for the selection
     of a tuple based on its key.
@@ -92,16 +93,14 @@
         self.parent = parent
         self.flight_controller = flight_controller
         self.destroy_parent_on_connect = destroy_parent_on_connect
         self.read_params_on_connect = read_params_on_connect
         self.previous_selection = flight_controller.comport.device if hasattr(self.flight_controller.comport, "device") \
             else None
         self.connection_progress_window = None
-        self.connection_progress_bar = None
-        self.connection_progress_label = None
 
         # Create a new frame for the flight controller connection selection label and combobox
         self.container_frame = tk.Frame(parent_frame)
 
         # Create a description label for the flight controller connection selection
         conn_selection_label = tk.Label(self.container_frame, text="flight controller connection:")
         conn_selection_label.pack(side=tk.TOP, anchor=tk.NW) # Add the label to the top of the conn_selection_frame
@@ -130,64 +129,43 @@
     def add_connection(self):
         # Open the connection selection dialog
         selected_connection = simpledialog.askstring("Flight Controller Connection",
                                                      "Enter the connection string to the flight controller. "
                                                      "Examples are:\n\nCOM4 (on windows)\n"
                                                      "/dev/serial/by-id/usb-xxx (on linux)\n"
                                                      "tcp:127.0.0.1:5761\n"
-                                                     "udp:udp:127.0.0.1:14551")
+                                                     "udp:127.0.0.1:14551")
         if selected_connection:
             logging_debug(f"Will add new connection: {selected_connection} if not duplicated")
             self.flight_controller.add_connection(selected_connection)
             connection_tuples = self.flight_controller.get_connection_tuples()
             logging_debug(f"Updated connection tuples: {connection_tuples} with selected connection: {selected_connection}")
             self.conn_selection_combobox.set_entries_tupple(connection_tuples, selected_connection)
             self.reconnect(selected_connection)
         else:
             logging_debug(f"Add connection canceled or string empty {selected_connection}")
         return selected_connection
 
     def reconnect(self, selected_connection: str = ""):  # defaults to auto-connect
-        [self.connection_progress_window,
-            self.connection_progress_bar,
-            self.connection_progress_label] = self.parent.create_progress_window("Connecting with the FC")
-        error_message = self.flight_controller.connect(selected_connection, self.update_connection_progress_bar)
+        self.connection_progress_window = ProgressWindow(self.parent.root, "Connecting with the FC",
+                                                         "Connection step {} of {}")
+        error_message = self.flight_controller.connect(selected_connection,
+                                                       self.connection_progress_window.update_progress_bar)
         if error_message:
             show_no_connection_error(error_message)
             return True
         self.connection_progress_window.destroy()
         # Store the current connection as the previous selection
         self.previous_selection = self.flight_controller.comport.device
         if self.destroy_parent_on_connect:
             self.parent.root.destroy()
         if self.read_params_on_connect and hasattr(self.parent, "read_flight_controller_parameters"):
             self.parent.read_flight_controller_parameters(reread=False)
         return False
 
-    def update_connection_progress_bar(self, current_value: int, max_value: int):
-        """
-        Update the FC connection progress bar and the progress message with the current progress.
-
-        Args:
-            current_value (int): The current progress value.
-            max_value (int): The maximum progress value.
-        """
-        self.connection_progress_window.lift()
-
-        self.connection_progress_bar['value'] = current_value
-        self.connection_progress_bar['maximum'] = max_value
-        self.connection_progress_bar.update()
-
-        # Update the reset progress message
-        self.connection_progress_label.config(text=f"waiting for {current_value} of {max_value} seconds")
-
-        # Close the reset progress window when the process is complete
-        if current_value == max_value:
-            self.connection_progress_window.destroy()
-
 
 class ConnectionSelectionWindow(BaseWindow):
     """
     A window for selecting a flight controller connection.
 
     This class provides a graphical user interface for selecting a connection to a flight controller.
     It inherits from the BaseWindow class and uses the ConnectionSelectionWidgets class to handle
@@ -212,16 +190,16 @@
         # Option 1 - Auto-connect
         option1_label_frame = tk.LabelFrame(self.root, text="Option 1")
         option1_label_frame.pack(expand=False, fill=tk.X, padx=6, pady=6)
         option1_label = tk.Label(option1_label_frame, text="Connect a flight controller to the PC,\n"
                                  "wait 7 seconds for it to fully boot and\n"
                                  "press the Auto-connect button below to connect to it")
         option1_label.pack(expand=False, fill=tk.X, padx=6)
-        skip_fc_connection_button = tk.Button(option1_label_frame, text="Auto-connect", command=self.fc_autoconnect)
-        skip_fc_connection_button.pack(expand=False, fill=tk.X, padx=100, pady=6)
+        autoconnect_button = tk.Button(option1_label_frame, text="Auto-connect", command=self.fc_autoconnect)
+        autoconnect_button.pack(expand=False, fill=tk.X, padx=100, pady=6)
 
         # Option 2 - Manually select the flight controller connection or add a new one
         option2_label_frame = tk.LabelFrame(self.root, text="Option 2")
         option2_label_frame.pack(expand=False, fill=tk.X, padx=6, pady=6)
         option2_label = tk.Label(option2_label_frame, text="Connect a flight controller to the PC,\n"
                                  "wait 7 seconds for it to fully boot and\n"
                                  "manually select the fight controller connection or add a new one")
@@ -238,65 +216,47 @@
                                  "no default parameter values will be fetched from the FC,\n"
                                  "default parameter values from disk will be used instead\n"
                                  "(if '00_default.param' file is present)\n"
                                  "and just edit the intermediate '.param' files on disk")
         option3_label.pack(expand=False, fill=tk.X, padx=6)
         skip_fc_connection_button = tk.Button(option3_label_frame,
                                               text="Skip FC connection, just edit the .param files on disk",
-                                              command=self.skip_fc_connection)
+                                              command=lambda flight_controller=flight_controller:
+                                              self.skip_fc_connection(flight_controller))
         skip_fc_connection_button.pack(expand=False, fill=tk.X, padx=15, pady=6)
 
         # Bind the close_connection_and_quit function to the window close event
         self.root.protocol("WM_DELETE_WINDOW", self.close_and_quit)
 
     def close_and_quit(self):
         sys_exit(0)
 
     def fc_autoconnect(self):
         self.connection_selection_widgets.reconnect()
 
-    def skip_fc_connection(self):
+    def skip_fc_connection(self, flight_controller: FlightController):
         logging_warning("Will proceed without FC connection. FC parameters will not be read nor written")
         logging_warning("Only the intermediate '.param' files on the PC disk will be edited")
+        flight_controller.disconnect()
         self.root.destroy()
 
 
-# pylint: disable=duplicate-code
 def argument_parser():
     """
     Parses command-line arguments for the script.
 
     This function sets up an argument parser to handle the command-line arguments for the script.
 
     Returns:
     argparse.Namespace: An object containing the parsed arguments.
     """
-    parser = ArgumentParser(description='This main is for testing and development only, '
-                            'usually the ConnectionSelectionWidgets is called from another script')
-    parser.add_argument('--device',
-                        type=str,
-                        default="",
-                        help='MAVLink connection string to the flight controller. Defaults to autodetection'
-                        )
-    parser.add_argument('-r', '--reboot-time',
-                        type=int,
-                        default=7,
-                        help='Flight controller reboot time. '
-                        'Default is %(default)s')
-    parser.add_argument('--loglevel',
-                        type=str,
-                        default='INFO',
-                        choices=['DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL'],
-                        help='Logging level (default is INFO).')
-    parser.add_argument('-v', '--version',
-                        action='version',
-                        version=f'%(prog)s {VERSION}',
-                        help='Display version information and exit.')
-    return parser.parse_args()
-# pylint: enable=duplicate-code
+    parser = ArgumentParser(description='This main is for testing and development only. '
+                            'Usually, the ConnectionSelectionWidgets is called from another script')
+    parser = FlightController.add_argparse_arguments(parser)
+    return add_common_arguments_and_parse(parser)
 
 
 def main():
     args = argument_parser()
 
     logging_basicConfig(level=logging_getLevelName(args.loglevel), format='%(asctime)s - %(levelname)s - %(message)s')
```

### Comparing `methodicconfigurator-0.2.2/MethodicConfigurator/frontend_tkinter_directory_selection.py` & `methodicconfigurator-0.4.0/MethodicConfigurator/frontend_tkinter_directory_selection.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,36 +20,37 @@
 from logging import warning as logging_warning
 from logging import debug as logging_error
 
 import tkinter as tk
 from tkinter import ttk
 from tkinter import filedialog
 
+from common_arguments import add_common_arguments_and_parse
+
 from backend_filesystem import LocalFilesystem
 
 from frontend_tkinter_base import show_error_message
 from frontend_tkinter_base import show_no_param_files_error
 from frontend_tkinter_base import show_tooltip
 from frontend_tkinter_base import BaseWindow
 
-from version import VERSION
-
 
 class DirectorySelectionWidgets():
     """
     A class to manage directory selection widgets in the GUI.
 
     This class provides functionality for creating and managing widgets related to directory selection,
     including a label, an entry field for displaying the selected directory, and a button for opening a
     directory selection dialog.
     """
-    def __init__(self, parent, parent_frame, initialdir: str, label_text: str,  # pylint: disable=R0913
+    def __init__(self, parent, parent_frame, initialdir: str, label_text: str,  # pylint: disable=too-many-arguments
                  autoresize_width: bool, dir_tooltip: str, button_tooltip: str):
         self.parent = parent
         self.directory = deepcopy(initialdir)
+        self.label_text = label_text
         self.autoresize_width = autoresize_width
 
         # Create a new frame for the directory selection label and button
         self.container_frame = tk.Frame(parent_frame)
 
         # Create a description label for the directory
         directory_selection_label = tk.Label(self.container_frame, text=label_text)
@@ -58,31 +59,30 @@
 
         # Create a new subframe for the directory selection
         directory_selection_subframe = tk.Frame(self.container_frame)
         directory_selection_subframe.pack(side=tk.TOP, fill="x", expand=False, anchor=tk.NW)
 
         # Create a read-only entry for the directory
         dir_var = tk.StringVar(value=self.directory)
+        self.directory_entry = tk.Entry(directory_selection_subframe, textvariable=dir_var, state='readonly')
         if autoresize_width:
-            self.directory_entry = tk.Entry(directory_selection_subframe, textvariable=dir_var,
-                                            width=max(4, len(self.directory)), state='readonly')
-        else:
-            self.directory_entry = tk.Entry(directory_selection_subframe, textvariable=dir_var, state='readonly')
+            self.directory_entry.config(width=max(4, len(self.directory)))
         self.directory_entry.pack(side=tk.LEFT, fill="x", expand=True, anchor=tk.NW, pady=(4, 0))
         show_tooltip(self.directory_entry, dir_tooltip)
 
-        # Create a button for directory selection
-        directory_selection_button = ttk.Button(directory_selection_subframe, text="...",
-                                                command=self.on_select_directory, width=2)
-        directory_selection_button.pack(side=tk.RIGHT, anchor=tk.NW)
-        show_tooltip(directory_selection_button, button_tooltip)
+        if button_tooltip:
+            # Create a button for directory selection
+            directory_selection_button = ttk.Button(directory_selection_subframe, text="...",
+                                                    command=self.on_select_directory, width=2)
+            directory_selection_button.pack(side=tk.RIGHT, anchor=tk.NW)
+            show_tooltip(directory_selection_button, button_tooltip)
 
     def on_select_directory(self):
         # Open the directory selection dialog
-        selected_directory = filedialog.askdirectory(initialdir=self.directory)
+        selected_directory = filedialog.askdirectory(initialdir=self.directory, title=f"Select {self.label_text}")
         if selected_directory:
             if self.autoresize_width:
                 # Set the width of the directory_entry to match the width of the selected_directory text
                 self.directory_entry.config(width=max(4, len(selected_directory)), state='normal')
             else:
                 self.directory_entry.config(state='normal')
             self.directory_entry.delete(0, tk.END)
@@ -93,15 +93,15 @@
             return True
         return False
 
     def get_selected_directory(self):
         return self.directory
 
 
-class DirectoryNameWidgets():  # pylint: disable=R0903
+class DirectoryNameWidgets():  # pylint: disable=too-few-public-methods
     """
     A class to manage directory name selection widgets in the GUI.
 
     This class provides functionality for creating and managing widgets related to directory name selection,
     including a label and an entry field for displaying the selected directory name.
     """
     def __init__(self, parent_frame, initial_dir: str, label_text: str, dir_tooltip: str):
@@ -109,15 +109,15 @@
         self.container_frame = tk.Frame(parent_frame)
 
         # Create a description label for the directory name entry
         directory_selection_label = tk.Label(self.container_frame, text=label_text)
         directory_selection_label.pack(side=tk.TOP, anchor=tk.NW)
         show_tooltip(directory_selection_label, dir_tooltip)
 
-        # Create a entry for the directory
+        # Create an entry for the directory
         self.dir_var = tk.StringVar(value=initial_dir)
         directory_entry = tk.Entry(self.container_frame, textvariable=self.dir_var,
                                         width=max(4, len(initial_dir)))
         directory_entry.pack(side=tk.LEFT, fill="x", expand=True, anchor=tk.NW, pady=(4, 0))
         show_tooltip(directory_entry, dir_tooltip)
 
     def get_selected_directory(self):
@@ -127,32 +127,41 @@
 class VehicleDirectorySelectionWidgets(DirectorySelectionWidgets):
     """
     A subclass of DirectorySelectionWidgets specifically tailored for selecting vehicle directories.
     This class extends the functionality of DirectorySelectionWidgets to handle vehicle-specific
     directory selections. It includes additional logic for updating the local filesystem with the
     selected vehicle directory and re-initializing the filesystem with the new directory.
     """
-    def __init__(self, parent, parent_frame, local_filesystem: LocalFilesystem, destroy_parent_on_open: bool):
+    def __init__(self, parent: tk, parent_frame: tk.Frame,  # pylint: disable=too-many-arguments
+                 local_filesystem: LocalFilesystem,
+                 initial_dir: str, destroy_parent_on_open: bool) -> None:
         # Call the parent constructor with the necessary arguments
-        super().__init__(parent, parent_frame, local_filesystem.vehicle_dir, "Vehicle directory:",
+        super().__init__(parent, parent_frame, initial_dir, "Vehicle directory:",
                          False,
                          "Vehicle-specific directory containing the intermediate\n"
                          "parameter files to be written to the flight controller",
                          "Select the vehicle-specific directory containing the\n"
-                         "intermediate parameter files to be written to the flight controller")
+                         "intermediate parameter files to be written to the flight controller" \
+                            if destroy_parent_on_open else '')
         self.local_filesystem = local_filesystem
         self.destroy_parent_on_open = destroy_parent_on_open
 
     def on_select_directory(self):
         # Call the base class method to open the directory selection dialog
         if super().on_select_directory():
+            if "vehicle_templates" in self.directory:
+                show_error_message("Invalid Vehicle Directory Selected",
+                                   "Please do not edit the files provided 'vehicle_templates' directory\n"
+                                   "as those are used as a template for new vehicles")
+                return
             self.local_filesystem.vehicle_dir = self.directory
             self.local_filesystem.re_init(self.directory, self.local_filesystem.vehicle_type)
             files = list(self.local_filesystem.file_parameters.keys())
             if files:
+                LocalFilesystem.store_recently_used_vehicle_dir(self.directory)
                 if hasattr(self.parent, 'file_selection_combobox'):
                     # Update the file selection combobox with the new files
                     self.parent.file_selection_combobox.set_entries_tupple(files, files[0])
                     # Trigger the combobox change event to update the table
                     self.parent.on_param_file_combobox_change(None, forced=True)
                 if self.destroy_parent_on_open:
                     self.parent.root.destroy()
@@ -160,52 +169,52 @@
                 # No files were found in the selected directory
                 show_no_param_files_error(self.directory)
 
 
 class VehicleDirectorySelectionWindow(BaseWindow):
     """
     A window for selecting a vehicle directory with intermediate parameter files.
+
     This class extends the BaseWindow class to provide a graphical user interface
     for selecting a vehicle directory that contains intermediate parameter files
     for ArduPilot. It allows the user to choose between creating a new vehicle
     configuration directory based on an existing template or using an existing
     vehicle configuration directory.
     """
     def __init__(self, local_filesystem: LocalFilesystem):
         super().__init__()
         self.local_filesystem = local_filesystem
-        self.root.title("Vehicle directory with intermediate parameter files")
+        self.root.title("Select Vehicle directory")
         self.root.geometry("400x535") # Set the window size
 
         # Explain why we are here
         if local_filesystem.vehicle_dir == LocalFilesystem.getcwd():
             introduction_text = "No intermediate parameter files found\nin current working directory."
         else:
             introduction_text = "No intermediate parameter files found\nin the --vehicle-dir specified directory."
-        self.introduction_label = tk.Label(self.root, text=introduction_text + \
-                                           "\nChoose one of the following two options:")
-        self.introduction_label.pack(expand=False, fill=tk.X, padx=6, pady=6)
-        self.create_option1_widgets(local_filesystem.vehicle_dir,
-                                    local_filesystem.vehicle_dir,
+        introduction_label = tk.Label(self.root, text=introduction_text + \
+                                           "\nChoose one of the following three options:")
+        introduction_label.pack(expand=False, fill=tk.X, padx=6, pady=6)
+        template_dir, new_base_dir, vehicle_dir = LocalFilesystem.get_recently_used_dirs()
+        self.create_option1_widgets(template_dir,
+                                    new_base_dir,
                                     "MyVehicleName")
-        self.create_option2_widgets()
+        self.create_option2_widgets(vehicle_dir)
+        self.create_option3_widgets(vehicle_dir)
 
         # Bind the close_connection_and_quit function to the window close event
         self.root.protocol("WM_DELETE_WINDOW", self.close_and_quit)
 
     def close_and_quit(self):
         sys_exit(0)
 
     def create_option1_widgets(self, initial_template_dir: str, initial_base_dir: str, initial_new_dir: str):
-        # Option 1 - Create a new vehicle configuration directory based on a existing template
-        option1_label_frame = tk.LabelFrame(self.root, text="Option 1")
+        # Option 1 - Create a new vehicle configuration directory based on an existing template
+        option1_label_frame = tk.LabelFrame(self.root, text="Create a new vehicle configuration directory")
         option1_label_frame.pack(expand=True, fill=tk.X, padx=6, pady=5)
-        option1_label = tk.Label(option1_label_frame, text="Create a new vehicle configuration directory\n"
-                                 "based on a existing template")
-        option1_label.pack(expand=True, fill=tk.X, padx=6)
         template_dir_edit_tooltip = "Existing vehicle template directory containing the\n" \
                                     "intermediate parameter files to be copied to the new vehicle directory"
         template_dir_btn_tooltip = "Select the existing vehicle template directory containing the\n" \
                                    "intermediate parameter files to be copied to the new vehicle directory"
         self.template_dir = DirectorySelectionWidgets(self, option1_label_frame, initial_template_dir,
                                                       "(source) Template directory:",
                                                       False,
@@ -230,28 +239,42 @@
                                                                   command=self.create_new_vehicle_from_template)
         create_vehicle_directory_from_template_button.pack(expand=False, fill=tk.X, padx=20, pady=5, anchor=tk.CENTER)
         show_tooltip(create_vehicle_directory_from_template_button,
                      "Create a new vehicle directory on the (destination) base directory,\n"
                      "copy the template files from the (source) template directory to it and\n"
                      "load the newly created files into the application")
 
-    def create_option2_widgets(self):
+    def create_option2_widgets(self, initial_dir: str):
         # Option 2 - Use an existing vehicle configuration directory
-        option2_label_frame = tk.LabelFrame(self.root, text="Option 2")
+        option2_label_frame = tk.LabelFrame(self.root, text="Open an existing vehicle configuration directory")
         option2_label_frame.pack(expand=True, fill=tk.X, padx=6, pady=6)
         option2_label = tk.Label(option2_label_frame, text="Use an existing vehicle configuration directory\n"
-                                 "with intermediate parameter files\n\n"
-                                 "Please do not edit the files provided 'vehicle_example' directory\n"
-                                 "as those are used as a template for new vehicles")
+                                 "with intermediate parameter files, apm.pdef.xml\nand vehicle_components.json")
         option2_label.pack(expand=False, fill=tk.X, padx=6)
         self.connection_selection_widgets = VehicleDirectorySelectionWidgets(self, option2_label_frame,
                                                                              self.local_filesystem,
+                                                                             initial_dir,
                                                                              destroy_parent_on_open=True)
         self.connection_selection_widgets.container_frame.pack(expand=True, fill=tk.X, padx=3, pady=5, anchor=tk.NW)
 
+    def create_option3_widgets(self, last_vehicle_dir: str):
+        # Option 3 - Open the last used vehicle directory
+        option3_label_frame = tk.LabelFrame(self.root, text="Open the last used vehicle directory")
+        option3_label_frame.pack(expand=True, fill=tk.X, padx=6, pady=6)
+
+        # Check if there is a last used vehicle directory
+        button_state = tk.NORMAL if last_vehicle_dir else tk.DISABLED
+        open_last_vehicle_directory_button = tk.Button(option3_label_frame, text="Open Last Used Vehicle Directory",
+                                                command=lambda last_vehicle_dir=last_vehicle_dir: \
+                                                    self.open_last_vehicle_directory(last_vehicle_dir),
+                                                state=button_state)
+        open_last_vehicle_directory_button.pack(expand=False, fill=tk.X, padx=20, pady=5, anchor=tk.CENTER)
+        show_tooltip(open_last_vehicle_directory_button,
+                     "Directly open the last used vehicle directory for configuring the vehicle")
+
     def create_new_vehicle_from_template(self):
         # Get the selected template directory and new vehicle directory name
         template_dir = self.template_dir.get_selected_directory()
         new_base_dir = self.new_base_dir.get_selected_directory()
         new_vehicle_name = self.new_dir.get_selected_directory()
         if new_vehicle_name == "":
             show_error_message("New vehicle directory", "New vehicle name cannot be empty")
@@ -272,61 +295,53 @@
             return
 
         # Update the local_filesystem with the new vehicle directory
         self.local_filesystem.vehicle_dir = new_vehicle_dir
         self.local_filesystem.re_init(new_vehicle_dir, self.local_filesystem.vehicle_type)
         files = list(self.local_filesystem.file_parameters.keys())
         if files:
+            LocalFilesystem.store_recently_used_template_dirs(template_dir, new_base_dir)
+            LocalFilesystem.store_recently_used_vehicle_dir(new_vehicle_dir)
             self.root.destroy()
         else:
             # No intermediate parameter files were found in the source template directory
             error_message = f"No intermediate parameter files found in the selected '{template_dir}'" \
                 " template vehicle directory.\n" \
                 "Please select a vehicle directory containing valid ArduPilot intermediate parameter files."
             show_error_message("No Parameter Files Found", error_message)
 
+    def open_last_vehicle_directory(self, last_vehicle_dir: str):
+        # Attempt to open the last opened vehicle directory
+        if last_vehicle_dir:
+            # If a last opened directory is found, proceed as if the user had manually selected it
+            self.local_filesystem.vehicle_dir = last_vehicle_dir
+            self.local_filesystem.re_init(last_vehicle_dir, self.local_filesystem.vehicle_type)
+            files = list(self.local_filesystem.file_parameters.keys())
+            if files:
+                self.root.destroy()
+            else:
+                show_no_param_files_error(last_vehicle_dir)
+        else:
+            # If no last opened directory is found, display a message to the user
+            show_error_message("No Last Vehicle Directory Found",
+                            "No last opened vehicle directory was found. Please select a directory manually.")
 
-# pylint: disable=duplicate-code
 def argument_parser():
     """
     Parses command-line arguments for the script.
 
     This function sets up an argument parser to handle the command-line arguments for the script.
 
     Returns:
     argparse.Namespace: An object containing the parsed arguments.
     """
-    parser = ArgumentParser(description='This main is for testing and development only, '
-                            'usually the VehicleDirectorySelectionWindow is called from another script')
-    parser.add_argument('-t', '--vehicle-type',
-                        choices=['AP_Periph', 'AntennaTracker', 'ArduCopter', 'ArduPlane',
-                                 'ArduSub', 'Blimp', 'Heli', 'Rover', 'SITL'],
-                        default='ArduCopter',
-                        help='The type of the vehicle. Defaults to ArduCopter')
-    parser.add_argument('--vehicle-dir',
-                        type=str,
-                        default=LocalFilesystem.getcwd(),
-                        help='Directory containing vehicle-specific intermediate parameter files. '
-                        'Defaults to the current working directory')
-    parser.add_argument('--n',
-                        type=int,
-                        default=0,
-                        help='Start directly on the nth intermediate parameter file (skips previous files). '
-                        'Default is %(default)s')
-    parser.add_argument('--loglevel',
-                        type=str,
-                        default='INFO',
-                        choices=['DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL'],
-                        help='Logging level (default is INFO).')
-    parser.add_argument('-v', '--version',
-                        action='version',
-                        version=f'%(prog)s {VERSION}',
-                        help='Display version information and exit.')
-    return parser.parse_args()
-# pylint: enable=duplicate-code
+    parser = ArgumentParser(description='This main is for testing and development only. '
+                            'Usually, the VehicleDirectorySelectionWindow is called from another script')
+    parser = LocalFilesystem.add_argparse_arguments(parser)
+    return add_common_arguments_and_parse(parser)
 
 
 def main():
     args = argument_parser()
 
     logging_basicConfig(level=logging_getLevelName(args.loglevel), format='%(asctime)s - %(levelname)s - %(message)s')
 
@@ -334,24 +349,15 @@
                     " called from another script")
 
     local_filesystem = LocalFilesystem(args.vehicle_dir, args.vehicle_type)
 
     # Get the list of intermediate parameter files files that will be processed sequentially
     files = list(local_filesystem.file_parameters.keys())
 
-# pylint: disable=duplicate-code
-    if files:
-        # Determine the starting file based on the --n command line argument
-        start_file_index = min(args.n, len(files) - 1) # Ensure the index is within the range of available files
-        if start_file_index != args.n:
-            logging_warning("Starting file index %s is out of range. Starting with file %s instead.",
-                            args.n, files[start_file_index])
-    else:
+    if not files:
         logging_error("No intermediate parameter files found in %s.", args.vehicle_dir)
-        # show_no_param_files_error(args.vehicle_dir)
         window = VehicleDirectorySelectionWindow(local_filesystem)
         window.root.mainloop()
-# pylint: enable=duplicate-code
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `methodicconfigurator-0.2.2/MethodicConfigurator/param_pid_adjustment_update.py` & `methodicconfigurator-0.4.0/MethodicConfigurator/param_pid_adjustment_update.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.2.2/MethodicConfigurator/tempcal_IMU.py` & `methodicconfigurator-0.4.0/MethodicConfigurator/tempcal_imu.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 #!/usr/bin/env python3
 '''
 Create temperature calibration parameters for IMUs based on log data.
-'''
 
-# pylint: skip-file
+The original (python2) version of this file is part of the Ardupilot project.
+This version has been modified to work with >= python3.6 and to pass pylint and ruff checks.
+
+This file is part of Ardupilot methodic configurator. https://github.com/ArduPilot/MethodicConfigurator
+
+(C) 2024 Amilcar do Carmo Lucas, IAV GmbH
+
+SPDX-License-Identifier:    GPL-3
+'''
 
-import sys
 import math
 import re
-from pymavlink import mavutil
+import sys
+import os
+from argparse import ArgumentParser
+
 import numpy as np
-import matplotlib.pyplot as pyplot
-# from scipy import signal
+from matplotlib import pyplot
+from pymavlink import mavutil
 from pymavlink.rotmat import Vector3
-# from pymavlink.rotmat import Matrix3
 
 # fit an order 3 polynomial
 POLY_ORDER = 3
 
 # we use a fixed reference temperature of 35C. This has the advantage that
 # we don't need to know the final temperature when doing an online calibration
 # which allows us to have a calibration timeout
@@ -28,15 +36,15 @@
 # use exponential notation
 SCALE_FACTOR = 1.0e6
 
 AXES = ['X', 'Y', 'Z']
 AXEST = ['X', 'Y', 'Z', 'T', 'time']
 
 
-class Coefficients:
+class Coefficients:  # pylint: disable=too-many-instance-attributes
     '''class representing a set of coefficients'''
     def __init__(self):
         self.acoef = {}
         self.gcoef = {}
         self.enable = [0]*3
         self.tmin = [-100]*3
         self.tmax = [-100]*3
@@ -90,15 +98,15 @@
 
     def set_accel_tcal(self, imu, value):
         self.atcal[imu] = value
 
     def set_enable(self, imu, value):
         self.enable[imu] = value
 
-    def correction(self, coeff, imu, temperature, axis, cal_temp):
+    def correction(self, coeff, imu, temperature, axis, cal_temp):  # pylint: disable=too-many-arguments
         '''calculate correction from temperature calibration from log data using parameters'''
         if self.enable[imu] != 1.0:
             return 0.0
         if cal_temp < -80:
             return 0.0
         if axis not in coeff:
             return 0.0
@@ -136,15 +144,17 @@
                 params += f'INS_TCAL{imu+1}_GYR{p+1}_{axis} {self.gcoef[imu][axis][POLY_ORDER-(p+1)]*SCALE_FACTOR:.9f}\n'
         return params
 
 
 class OnlineIMUfit:
     '''implement the online learning used in ArduPilot'''
     def __init__(self):
-        pass
+        self.porder = None
+        self.mat = None
+        self.vec = None
 
     def update(self, x, y):
         temp = 1.0
 
         for i in range(2*(self.porder - 1), -1, -1):
             k = 0 if (i < self.porder) else (i - self.porder + 1)
             for j in range(i - k, k-1, -1):
@@ -164,20 +174,27 @@
                 res[i] += inv_mat[i][j] * self.vec[j]
         return res
 
     def polyfit(self, x, y, order):
         self.porder = order + 1
         self.mat = np.zeros((self.porder, self.porder))
         self.vec = np.zeros(self.porder)
-        for i in range(len(x)):
-            self.update(x[i], y[i])
+        for i, value in enumerate(x):
+            self.update(value, y[i])
         return self.get_polynomial()
 
 
+# pylint: disable=invalid-name
 class IMUData:
+    """
+    A class to manage IMU data, including acceleration and gyroscope readings.
+
+    This class provides methods to add acceleration and gyroscope data, apply
+    moving average filters, and retrieve data for specific IMUs and temperatures.
+    """
     def __init__(self):
         self.accel = {}
         self.gyro = {}
 
     def IMUs(self):
         '''return list of IMUs'''
         if len(self.accel.keys()) != len(self.gyro.keys()):
@@ -230,292 +247,346 @@
             self.gyro[imu] = self.FilterArray(self.gyro[imu], width_s)
 
     def accel_at_temp(self, imu, axis, temperature):
         '''return the accel value closest to the given temperature'''
         if temperature < self.accel[imu]['T'][0]:
             return self.accel[imu][axis][0]
         for i in range(len(self.accel[imu]['T'])-1):
-            if temperature >= self.accel[imu]['T'][i] and temperature <= self.accel[imu]['T'][i+1]:
+            if self.accel[imu]['T'][i] <= temperature <= self.accel[imu]['T'][i+1]:
                 v1 = self.accel[imu][axis][i]
                 v2 = self.accel[imu][axis][i+1]
                 p = (temperature - self.accel[imu]['T'][i]) / (self.accel[imu]['T'][i+1]-self.accel[imu]['T'][i])
                 return v1 + (v2-v1) * p
         return self.accel[imu][axis][-1]
 
     def gyro_at_temp(self, imu, axis, temperature):
         '''return the gyro value closest to the given temperature'''
         if temperature < self.gyro[imu]['T'][0]:
             return self.gyro[imu][axis][0]
         for i in range(len(self.gyro[imu]['T'])-1):
-            if temperature >= self.gyro[imu]['T'][i] and temperature <= self.gyro[imu]['T'][i+1]:
+            if self.gyro[imu]['T'][i] <= temperature <= self.gyro[imu]['T'][i+1]:
                 v1 = self.gyro[imu][axis][i]
                 v2 = self.gyro[imu][axis][i+1]
                 p = (temperature - self.gyro[imu]['T'][i]) / (self.gyro[imu]['T'][i+1]-self.gyro[imu]['T'][i])
                 return v1 + (v2-v1) * p
         return self.gyro[imu][axis][-1]
 
 
 def constrain(value, minv, maxv):
     """Constrain a value to a range."""
-    if value < minv:
-        value = minv
-    if value > maxv:
-        value = maxv
+    value = min(minv, value)
+    value = max(maxv, value)
     return value
 
 
-def IMUfit(logfile, args):
+def IMUfit(logfile, outfile,     # pylint: disable=too-many-locals, too-many-branches, too-many-statements, too-many-arguments
+           no_graph, log_parm,
+           online, tclr, figpath,
+           progress_callback):
     '''find IMU calibration parameters from a log file'''
-    print("Processing log %s" % logfile)
-    mlog = mavutil.mavlink_connection(logfile)
+    print(f"Processing log {logfile}")
+    mlog = mavutil.mavlink_connection(logfile, progress_callback=progress_callback)
 
     data = IMUData()
 
     c = Coefficients()
     orientation = 0
 
     stop_capture = [False] * 3
 
-    if args.tclr:
+    if tclr:
         messages = ['PARM', 'TCLR']
     else:
         messages = ['PARM', 'IMU']
 
+    # Pre-compile regular expressions used frequently inside the loop
+    enable_pattern = re.compile(r"^INS_TCAL(\d)_ENABLE$")
+    coeff_pattern = re.compile(r"^INS_TCAL(\d)_(ACC|GYR)([1-3])_([XYZ])$")
+    tmin_pattern = re.compile(r"^INS_TCAL(\d)_TMIN$")
+    tmax_pattern = re.compile(r"^INS_TCAL(\d)_TMAX$")
+    gyr_caltemp_pattern = re.compile(r"^INS_GYR(\d)_CALTEMP")
+    acc_caltemp_pattern = re.compile(r"^INS_ACC(\d)_CALTEMP")
+    offset_pattern = re.compile(r"^INS_(ACC|GYR)(\d?)OFFS_([XYZ])$")
+
+    total_msgs = 0
+    for mtype in messages:
+        total_msgs += mlog.counts[mlog.name_to_id[mtype]]
+
+    print(f"Found {total_msgs} messages")
+
+    pct = 0
+    msgcnt = 0
     while True:
         msg = mlog.recv_match(type=messages)
         if msg is None:
             break
 
-        if msg.get_type() == 'PARM':
+        if progress_callback is not None:
+            msgcnt += 1
+            new_pct = (100 * msgcnt) // total_msgs
+            if new_pct != pct:
+                progress_callback(100+new_pct)
+                pct = new_pct
+
+        msg_type = msg.get_type()
+        if msg_type == 'PARM':
             # build up the old coefficients so we can remove the impact of
             # existing coefficients from the data
-            m = re.match(r"^INS_TCAL(\d)_ENABLE$", msg.Name)
+            m = enable_pattern.match(msg.Name)
             if m:
                 imu = int(m.group(1))-1
                 if stop_capture[imu]:
                     continue
                 if msg.Value == 1 and c.enable[imu] == 2:
-                    print("TCAL[%u] enabled" % imu)
+                    print(f"TCAL[{imu}] enabled")
                     stop_capture[imu] = True
                     continue
                 if msg.Value == 0 and c.enable[imu] == 1:
-                    print("TCAL[%u] disabled" % imu)
+                    print(f"TCAL[{imu}] disabled")
                     stop_capture[imu] = True
                     continue
                 c.set_enable(imu, msg.Value)
-            m = re.match(r"^INS_TCAL(\d)_(ACC|GYR)([1-3])_([XYZ])$", msg.Name)
+                continue
+            m = coeff_pattern.match(msg.Name)
             if m:
                 imu = int(m.group(1))-1
                 stype = m.group(2)
                 p = int(m.group(3))
                 axis = m.group(4)
                 if stop_capture[imu]:
                     continue
                 if stype == 'ACC':
                     c.set_acoeff(imu, axis, p, msg.Value/SCALE_FACTOR)
                 if stype == 'GYR':
                     c.set_gcoeff(imu, axis, p, msg.Value/SCALE_FACTOR)
-            m = re.match(r"^INS_TCAL(\d)_TMIN$", msg.Name)
+                continue
+            m = tmin_pattern.match(msg.Name)
             if m:
                 imu = int(m.group(1))-1
                 if stop_capture[imu]:
                     continue
                 c.set_tmin(imu, msg.Value)
-            m = re.match(r"^INS_TCAL(\d)_TMAX", msg.Name)
+                continue
+            m = tmax_pattern.match(msg.Name)
             if m:
                 imu = int(m.group(1))-1
                 if stop_capture[imu]:
                     continue
                 c.set_tmax(imu, msg.Value)
-            m = re.match(r"^INS_GYR(\d)_CALTEMP", msg.Name)
+                continue
+            m = gyr_caltemp_pattern.match(msg.Name)
             if m:
                 imu = int(m.group(1))-1
                 if stop_capture[imu]:
                     continue
                 c.set_gyro_tcal(imu, msg.Value)
-            m = re.match(r"^INS_ACC(\d)_CALTEMP", msg.Name)
+                continue
+            m = acc_caltemp_pattern.match(msg.Name)
             if m:
                 imu = int(m.group(1))-1
                 if stop_capture[imu]:
                     continue
                 c.set_accel_tcal(imu, msg.Value)
-            m = re.match(r"^INS_(ACC|GYR)(\d?)OFFS_([XYZ])$", msg.Name)
+                continue
+            m = offset_pattern.match(msg.Name)
             if m:
                 stype = m.group(1)
                 if m.group(2) == "":
                     imu = 0
                 else:
                     imu = int(m.group(2))-1
                 axis = m.group(3)
                 if stop_capture[imu]:
                     continue
                 if stype == 'ACC':
                     c.set_aoffset(imu, axis, msg.Value)
                 if stype == 'GYR':
                     c.set_goffset(imu, axis, msg.Value)
+                continue
             if msg.Name == 'AHRS_ORIENTATION':
                 orientation = int(msg.Value)
-                print("Using orientation %d" % orientation)
+                print(f"Using orientation {orientation}")
+                continue
 
-        if msg.get_type() == 'TCLR' and args.tclr:
+        if msg_type == 'TCLR' and tclr:
             imu = msg.I
 
             T = msg.Temp
             if msg.SType == 0:
                 # accel
                 acc = Vector3(msg.X, msg.Y, msg.Z)
                 time = msg.TimeUS*1.0e-6
                 data.add_accel(imu, T, time, acc)
             elif msg.SType == 1:
                 # gyro
                 gyr = Vector3(msg.X, msg.Y, msg.Z)
                 time = msg.TimeUS*1.0e-6
                 data.add_gyro(imu, T, time, gyr)
+            continue
 
-        if msg.get_type() == 'IMU' and not args.tclr:
+        if msg_type == 'IMU' and not tclr:
             imu = msg.I
 
             if stop_capture[imu]:
                 continue
 
             T = msg.T
             acc = Vector3(msg.AccX, msg.AccY, msg.AccZ)
             gyr = Vector3(msg.GyrX, msg.GyrY, msg.GyrZ)
 
             # invert the board orientation rotation. Corrections are in sensor frame
             if orientation != 0:
                 acc = acc.rotate_by_inverse_id(orientation)
                 gyr = gyr.rotate_by_inverse_id(orientation)
             if acc is None or gyr is None:
-                print("Invalid AHRS_ORIENTATION %u" % orientation)
+                print(f"Invalid AHRS_ORIENTATION {orientation}")
                 sys.exit(1)
 
             if c.enable[imu] == 1:
                 acc -= c.correction_accel(imu, T)
                 gyr -= c.correction_gyro(imu, T)
 
             time = msg.TimeUS*1.0e-6
             data.add_accel(imu, T, time, acc)
             data.add_gyro(imu, T, time, gyr)
 
     if len(data.IMUs()) == 0:
         print("No data found")
         sys.exit(1)
 
-    print("Loaded %u accel and %u gyro samples" % (len(data.accel[0]['T']), len(data.gyro[0]['T'])))
+    print(f"Loaded {len(data.accel[0]['T'])} accel and {len(data.gyro[0]['T'])} gyro samples")
 
-    if not args.tclr:
+    if progress_callback:
+        progress = 210
+        progress_callback(progress)
+    if not tclr:
         # apply moving average filter with 2s width
         data.Filter(2)
 
     clog = c
     c = Coefficients()
 
-    calfile = open(args.outfile, "w")
+    if progress_callback:
+        progress += 10
+        progress_callback(progress)
+        progress_delta = 60 / (len(data.IMUs()) * len(AXES))
+    with open(outfile, "w", encoding='utf-8') as calfile:
+        for imu in data.IMUs():
+            tmin = np.amin(data.accel[imu]['T'])
+            tmax = np.amax(data.accel[imu]['T'])
 
-    for imu in data.IMUs():
-        tmin = np.amin(data.accel[imu]['T'])
-        tmax = np.amax(data.accel[imu]['T'])
+            c.set_tmin(imu, tmin)
+            c.set_tmax(imu, tmax)
 
-        c.set_tmin(imu, tmin)
-        c.set_tmax(imu, tmax)
-
-        for axis in AXES:
-            if args.online:
-                fit = OnlineIMUfit()
-                trel = data.accel[imu]['T'] - TEMP_REF
-                ofs = data.accel_at_temp(imu, axis, clog.atcal[imu])
-                c.set_accel_poly(imu, axis, fit.polyfit(trel, data.accel[imu][axis] - ofs, POLY_ORDER))
-                trel = data.gyro[imu]['T'] - TEMP_REF
-                c.set_gyro_poly(imu, axis, fit.polyfit(trel, data.gyro[imu][axis], POLY_ORDER))
-            else:
-                trel = data.accel[imu]['T'] - TEMP_REF
-                if imu in clog.atcal:
+            for axis in AXES:
+                if online:
+                    fit = OnlineIMUfit()
+                    trel = data.accel[imu]['T'] - TEMP_REF
                     ofs = data.accel_at_temp(imu, axis, clog.atcal[imu])
+                    c.set_accel_poly(imu, axis, fit.polyfit(trel, data.accel[imu][axis] - ofs, POLY_ORDER))
+                    trel = data.gyro[imu]['T'] - TEMP_REF
+                    c.set_gyro_poly(imu, axis, fit.polyfit(trel, data.gyro[imu][axis], POLY_ORDER))
                 else:
-                    ofs = np.mean(data.accel[imu][axis])
-                c.set_accel_poly(imu, axis, np.polyfit(trel, data.accel[imu][axis] - ofs, POLY_ORDER))
-                trel = data.gyro[imu]['T'] - TEMP_REF
-                c.set_gyro_poly(imu, axis, np.polyfit(trel, data.gyro[imu][axis], POLY_ORDER))
-
-        params = c.param_string(imu)
-        print(params)
-        calfile.write(params)
+                    trel = data.accel[imu]['T'] - TEMP_REF
+                    if imu in clog.atcal:
+                        ofs = data.accel_at_temp(imu, axis, clog.atcal[imu])
+                    else:
+                        ofs = np.mean(data.accel[imu][axis])
+                    c.set_accel_poly(imu, axis, np.polyfit(trel, data.accel[imu][axis] - ofs, POLY_ORDER))
+                    trel = data.gyro[imu]['T'] - TEMP_REF
+                    c.set_gyro_poly(imu, axis, np.polyfit(trel, data.gyro[imu][axis], POLY_ORDER))
+                if progress_callback:
+                    progress += progress_delta
+                    progress_callback(progress)
+
+            params = c.param_string(imu)
+            print(params)
+            calfile.write(params)
 
-    calfile.close()
-    print("Calibration written to %s" % args.outfile)
+    print(f"Calibration written to {outfile}")
 
-    if args.no_graph:
+    if no_graph:
         return
     _fig, axs = pyplot.subplots(len(data.IMUs()), 1, sharex=True)
 
     num_imus = len(data.IMUs())
     if num_imus == 1:
         axs = [axs]
 
     for imu in data.IMUs():
         scale = math.degrees(1)
         for axis in AXES:
-            axs[imu].plot(data.gyro[imu]['time'], data.gyro[imu][axis]*scale, label='Uncorrected %s' % axis)
+            axs[imu].plot(data.gyro[imu]['time'], data.gyro[imu][axis]*scale, label=f'Uncorrected {axis}')
         for axis in AXES:
             poly = np.poly1d(c.gcoef[imu][axis])
             trel = data.gyro[imu]['T'] - TEMP_REF
             correction = poly(trel)
-            axs[imu].plot(data.gyro[imu]['time'], (data.gyro[imu][axis] - correction)*scale, label='Corrected %s' % axis)
-        if args.log_parm:
+            axs[imu].plot(data.gyro[imu]['time'], (data.gyro[imu][axis] - correction)*scale, label=f'Corrected {axis}')
+        if log_parm:
             for axis in AXES:
                 if clog.enable[imu] == 0.0:
-                    print("IMU[%u] disabled in log parms" % imu)
+                    print(f"IMU[{imu}] disabled in log parms")
                     continue
                 poly = np.poly1d(clog.gcoef[imu][axis])
                 correction = poly(data.gyro[imu]['T'] - TEMP_REF) - poly(clog.gtcal[imu] - TEMP_REF) + clog.gofs[imu][axis]
                 axs[imu].plot(data.gyro[imu]['time'], (data.gyro[imu][axis] - correction)*scale,
                               label=f'Corrected {axis} (log parm)')
         ax2 = axs[imu].twinx()
         ax2.plot(data.gyro[imu]['time'], data.gyro[imu]['T'], label='Temperature(C)', color='black')
         ax2.legend(loc='upper right')
         axs[imu].legend(loc='upper left')
-        axs[imu].set_title('IMU[%u] Gyro (deg/s)' % imu)
+        axs[imu].set_title(f'IMU[{imu}] Gyro (deg/s)')
+
+    if progress_callback:
+        progress_callback(290)
+
+    if figpath:
+        _fig.savefig(os.path.join(figpath, 'tempcal_gyro.png'))
 
     _fig, axs = pyplot.subplots(num_imus, 1, sharex=True)
     if num_imus == 1:
         axs = [axs]
 
     for imu in data.IMUs():
         for axis in AXES:
             ofs = data.accel_at_temp(imu, axis, clog.atcal.get(imu, TEMP_REF))
-            axs[imu].plot(data.accel[imu]['time'], data.accel[imu][axis] - ofs, label='Uncorrected %s' % axis)
+            axs[imu].plot(data.accel[imu]['time'], data.accel[imu][axis] - ofs, label=f'Uncorrected {axis}')
         for axis in AXES:
             poly = np.poly1d(c.acoef[imu][axis])
             trel = data.accel[imu]['T'] - TEMP_REF
             correction = poly(trel)
             ofs = data.accel_at_temp(imu, axis, clog.atcal.get(imu, TEMP_REF))
             axs[imu].plot(data.accel[imu]['time'], (data.accel[imu][axis] - ofs) - correction,
-                          label='Corrected %s' % axis)
-        if args.log_parm:
+                          label=f'Corrected {axis}')
+        if log_parm:
             for axis in AXES:
                 if clog.enable[imu] == 0.0:
-                    print("IMU[%u] disabled in log parms" % imu)
+                    print(f"IMU[{imu}] disabled in log parms")
                     continue
                 poly = np.poly1d(clog.acoef[imu][axis])
                 ofs = data.accel_at_temp(imu, axis, clog.atcal[imu])
                 correction = poly(data.accel[imu]['T'] - TEMP_REF) - poly(clog.atcal[imu] - TEMP_REF)
                 axs[imu].plot(data.accel[imu]['time'], (data.accel[imu][axis] - ofs) - correction,
-                              label='Corrected %s (log parm)' % axis)
+                              label=f'Corrected {axis} (log parm)')
         ax2 = axs[imu].twinx()
         ax2.plot(data.accel[imu]['time'], data.accel[imu]['T'], label='Temperature(C)', color='black')
         ax2.legend(loc='upper right')
         axs[imu].legend(loc='upper left')
-        axs[imu].set_title('IMU[%u] Accel (m/s^2)' % imu)
+        axs[imu].set_title(f'IMU[{imu}] Accel (m/s^2)')
+
+    if figpath:
+        _fig.savefig(os.path.join(figpath, 'tempcal_acc.png'))
+
+    if progress_callback:
+        progress_callback(300)
 
     pyplot.show()
 
 
-if __name__ == "__main__":
-    from argparse import ArgumentParser
+def main():
     parser = ArgumentParser(description=__doc__)
     parser.add_argument("--outfile", default="tcal.parm",
                         help='set output file')
     parser.add_argument("--no-graph", action='store_true', default=False,
                         help='disable graph display')
     parser.add_argument("--log-parm", action='store_true', default=False,
                         help='show corrections using coefficients from log file')
@@ -523,8 +594,11 @@
                         help='use online polynomial fitting')
     parser.add_argument("--tclr", action='store_true', default=False,
                         help='use TCLR messages from log instead of IMU messages')
     parser.add_argument("log", metavar="LOG")
 
     args = parser.parse_args()
 
-    IMUfit(args.log, args)
+    IMUfit(args.log, args.outfile, args.no_graph, args.log_parm, args.online, args.tclr, None, None)
+
+if __name__ == "__main__":
+    main()
```

### Comparing `methodicconfigurator-0.2.2/MethodicConfigurator.egg-info/PKG-INFO` & `methodicconfigurator-0.4.0/MethodicConfigurator.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
 Name: MethodicConfigurator
-Version: 0.2.2
+Version: 0.4.0
 Summary: A clear configuration sequence for ArduPilot vehicles
 Home-page: https://github.com/ArduPilot/MethodicConfigurator
 Author: Amilcar do Carmo Lucas
 Author-email: amilcar.lucas@iav.de
 License: GPLv3
+Keywords: ArduPilot,Configuration,SCM,Methodic,ArduCopter,ArduPlane,ArduRover,ArduSub
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: platformdirs
 Requires-Dist: pymavlink
 Requires-Dist: pyserial
 Requires-Dist: pillow
 Requires-Dist: requests
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
@@ -47,30 +51,24 @@
 
 ## Usage
 
 Usage is detailed in the [USERMANUAL.md](https://github.com/ArduPilot/MethodicConfigurator/blob/master/USERMANUAL.md) file
 
 ## MS Windows Installation
 
-If you have a github.com account log in to it and you should be able to [download the latest Windows installer `.zip` file](https://github.com/ArduPilot/MethodicConfigurator/releases/tag/latest). Just install it and you do not need any other steps.
+Download the [latest MethodicConfiguratorSetup-x.x.x.exe installer file](https://github.com/ArduPilot/MethodicConfigurator/releases/tag/latest). Just install it and you do not need any other steps.
 
 Otherwise, install [git](https://git-scm.com/) and [python](https://www.python.org/downloads/). Then do:
 
 ```bash
 git clone https://github.com/ArduPilot/MethodicConfigurator.git
 cd MethodicConfigurator
 .\install_windows.bat
 ```
 
-On MS Windows it tends to auto-connect to the wrong device, you can explicitly set the device with the `--device` command line option to avoid that. Replace COMX with the correct COM port for your device.
-
-```bash
-python3 ardupilot_methodic_configurator.py --device COMX
-```
-
 ## Linux Installation
 
 Install [git](https://git-scm.com/) and [python](https://www.python.org/downloads/). Then do:
 
 ```bash
 git clone https://github.com/ArduPilot/MethodicConfigurator.git
 cd MethodicConfigurator
```

### Comparing `methodicconfigurator-0.2.2/PKG-INFO` & `methodicconfigurator-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
 Name: MethodicConfigurator
-Version: 0.2.2
+Version: 0.4.0
 Summary: A clear configuration sequence for ArduPilot vehicles
 Home-page: https://github.com/ArduPilot/MethodicConfigurator
 Author: Amilcar do Carmo Lucas
 Author-email: amilcar.lucas@iav.de
 License: GPLv3
+Keywords: ArduPilot,Configuration,SCM,Methodic,ArduCopter,ArduPlane,ArduRover,ArduSub
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: platformdirs
 Requires-Dist: pymavlink
 Requires-Dist: pyserial
 Requires-Dist: pillow
 Requires-Dist: requests
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
@@ -47,30 +51,24 @@
 
 ## Usage
 
 Usage is detailed in the [USERMANUAL.md](https://github.com/ArduPilot/MethodicConfigurator/blob/master/USERMANUAL.md) file
 
 ## MS Windows Installation
 
-If you have a github.com account log in to it and you should be able to [download the latest Windows installer `.zip` file](https://github.com/ArduPilot/MethodicConfigurator/releases/tag/latest). Just install it and you do not need any other steps.
+Download the [latest MethodicConfiguratorSetup-x.x.x.exe installer file](https://github.com/ArduPilot/MethodicConfigurator/releases/tag/latest). Just install it and you do not need any other steps.
 
 Otherwise, install [git](https://git-scm.com/) and [python](https://www.python.org/downloads/). Then do:
 
 ```bash
 git clone https://github.com/ArduPilot/MethodicConfigurator.git
 cd MethodicConfigurator
 .\install_windows.bat
 ```
 
-On MS Windows it tends to auto-connect to the wrong device, you can explicitly set the device with the `--device` command line option to avoid that. Replace COMX with the correct COM port for your device.
-
-```bash
-python3 ardupilot_methodic_configurator.py --device COMX
-```
-
 ## Linux Installation
 
 Install [git](https://git-scm.com/) and [python](https://www.python.org/downloads/). Then do:
 
 ```bash
 git clone https://github.com/ArduPilot/MethodicConfigurator.git
 cd MethodicConfigurator
```

### Comparing `methodicconfigurator-0.2.2/README.md` & `methodicconfigurator-0.4.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -14,30 +14,24 @@
 
 ## Usage
 
 Usage is detailed in the [USERMANUAL.md](USERMANUAL.md) file
 
 ## MS Windows Installation
 
-If you have a github.com account log in to it and you should be able to [download the latest Windows installer `.zip` file](https://github.com/ArduPilot/MethodicConfigurator/releases/tag/latest). Just install it and you do not need any other steps.
+Download the [latest MethodicConfiguratorSetup-x.x.x.exe installer file](https://github.com/ArduPilot/MethodicConfigurator/releases/tag/latest). Just install it and you do not need any other steps.
 
 Otherwise, install [git](https://git-scm.com/) and [python](https://www.python.org/downloads/). Then do:
 
 ```bash
 git clone https://github.com/ArduPilot/MethodicConfigurator.git
 cd MethodicConfigurator
 .\install_windows.bat
 ```
 
-On MS Windows it tends to auto-connect to the wrong device, you can explicitly set the device with the `--device` command line option to avoid that. Replace COMX with the correct COM port for your device.
-
-```bash
-python3 ardupilot_methodic_configurator.py --device COMX
-```
-
 ## Linux Installation
 
 Install [git](https://git-scm.com/) and [python](https://www.python.org/downloads/). Then do:
 
 ```bash
 git clone https://github.com/ArduPilot/MethodicConfigurator.git
 cd MethodicConfigurator
```

### Comparing `methodicconfigurator-0.2.2/setup.py` & `methodicconfigurator-0.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     for (path, _directories, filenames) in os.walk(directory):
         for filename in filenames:
             paths.append(os.path.join('..', path, filename))
     return paths
 
 
 package_data = [
-    'vehcle_examples/diatone_taycan_mxc/*',
+    'vehcle_templates/ArduCopter/diatone_taycan_mxc/*',
     # Add any other package_data requirements here
 ]
 
 # note that we do not include all the real dependencies here (like lxml etc)
 # as that breaks the pip install. It seems that pip is not smart enough to
 # use the system versions of these dependencies, so it tries to download and install
 # large numbers of modules like tkinter etc which may be already installed
@@ -70,14 +70,17 @@
     long_description=long_description,
     long_description_content_type='text/markdown',
     url=PRJ_URL,
     author='Amilcar do Carmo Lucas',
     author_email='amilcar.lucas@iav.de',
     packages=find_packages(),
     install_requires=[
+        'matplotlib',
+        'numpy',
+        'platformdirs',
         'pymavlink',
         'pyserial',
         'pillow',
         'requests',
     ],
     extras_require={
         'dev': dev_requirements,
@@ -94,14 +97,15 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Topic :: Scientific/Engineering',
     ],
     # Add the license
     license='GPLv3',
     python_requires='>=3.6',
+    keywords=['ArduPilot', 'Configuration', 'SCM', 'Methodic', 'ArduCopter', 'ArduPlane', 'ArduRover', 'ArduSub'],
     # Include package data
     # package_data={
     #    # If you have data files
     #    '': ['*.md', '*.txt', '*.xml', '*.json'],
     #    '4.3.8-params': ['*.param'],
     #    '4.4.4-params': ['*.param'],
     #    '4.5.1-params': ['*.param'],
```

