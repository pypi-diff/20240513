# Comparing `tmp/methodicconfigurator-0.4.0.tar.gz` & `tmp/methodicconfigurator-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "methodicconfigurator-0.4.0.tar", last modified: Mon May 13 08:55:33 2024, max compression
+gzip compressed data, was "methodicconfigurator-0.4.2.tar", last modified: Mon May 13 17:13:34 2024, max compression
```

## Comparing `methodicconfigurator-0.4.0.tar` & `methodicconfigurator-0.4.2.tar`

### file list

```diff
@@ -1,38 +1,255 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:55:33.429222 methodicconfigurator-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:55:33.429222 methodicconfigurator-0.4.0/MethodicConfigurator/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27850 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/annotate_params.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5269 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/ardupilot_methodic_configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)    28850 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/backend_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/backend_filesystem_configuration_steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/backend_filesystem_vehicle_components.py
--rw-r--r--   0 runner    (1001) docker     (127)    30964 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/backend_flightcontroller.py
--rw-r--r--   0 runner    (1001) docker     (127)    26711 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/backend_mavftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/battery_cell_voltages.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/common_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/extract_param_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    13790 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/frontend_tkinter_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17895 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/frontend_tkinter_component_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/frontend_tkinter_component_editor_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    14476 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/frontend_tkinter_connection_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)    19947 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/frontend_tkinter_directory_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)    36799 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/frontend_tkinter_parameter_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    23781 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/frontend_tkinter_parameter_editor_table.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2468 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/get_release_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/param_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/param_pid_adjustment_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    22803 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/tempcal_imu.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/MethodicConfigurator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:55:33.429222 methodicconfigurator-0.4.0/MethodicConfigurator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-05-13 08:55:33.000000 methodicconfigurator-0.4.0/MethodicConfigurator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-13 08:55:33.000000 methodicconfigurator-0.4.0/MethodicConfigurator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:55:33.000000 methodicconfigurator-0.4.0/MethodicConfigurator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 08:55:33.000000 methodicconfigurator-0.4.0/MethodicConfigurator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-13 08:55:33.000000 methodicconfigurator-0.4.0/MethodicConfigurator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-13 08:55:33.000000 methodicconfigurator-0.4.0/MethodicConfigurator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:55:26.000000 methodicconfigurator-0.4.0/MethodicConfigurator.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-05-13 08:55:33.429222 methodicconfigurator-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 08:55:33.429222 methodicconfigurator-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-13 08:55:03.000000 methodicconfigurator-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:13:34.064245 methodicconfigurator-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:13:34.008244 methodicconfigurator-0.4.2/MethodicConfigurator/
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/ArduPilot_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26216 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/ArduPilot_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27848 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/annotate_params.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5416 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/ardupilot_methodic_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29018 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/backend_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/backend_filesystem_configuration_steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/backend_filesystem_vehicle_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30985 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/backend_flightcontroller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26774 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/backend_mavftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/battery_cell_voltages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/common_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/extract_param_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13811 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18042 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_component_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_component_editor_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14623 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_connection_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20073 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_directory_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37030 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_parameter_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23945 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_parameter_editor_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2468 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/get_release_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/param_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/param_pid_adjustment_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22803 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/tempcal_imu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:13:34.064245 methodicconfigurator-0.4.2/MethodicConfigurator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-05-13 17:13:33.000000 methodicconfigurator-0.4.2/MethodicConfigurator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20244 2024-05-13 17:13:34.000000 methodicconfigurator-0.4.2/MethodicConfigurator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 17:13:33.000000 methodicconfigurator-0.4.2/MethodicConfigurator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 17:13:33.000000 methodicconfigurator-0.4.2/MethodicConfigurator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-13 17:13:33.000000 methodicconfigurator-0.4.2/MethodicConfigurator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-13 17:13:33.000000 methodicconfigurator-0.4.2/MethodicConfigurator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 17:13:26.000000 methodicconfigurator-0.4.2/MethodicConfigurator.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-05-13 17:13:34.064245 methodicconfigurator-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 17:13:34.064245 methodicconfigurator-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:13:34.004244 methodicconfigurator-0.4.2/vehicle_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:13:34.004244 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:13:34.004244 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:13:34.024244 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/
+-rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/00_default.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/02_imu_temperature_calibration_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/03_imu_temperature_calibration_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/04_board_orientation.param
+-rw-r--r--   0 runner    (1001) docker     (127)    20925 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/05_remote_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/06_telemetry.param
+-rw-r--r--   0 runner    (1001) docker     (127)    15574 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/07_esc.param
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/08_batt1.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/09_batt2.param
+-rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/10_gnss.param
+-rw-r--r--   0 runner    (1001) docker     (127)    34562 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/11_mp_setup_mandatory_hardware.param
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/12_general_configuration.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/13_logging.param
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/14_motor.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/15_pid_adjustment.param
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/16_remote_id.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/17_notch_filter_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/18_notch_filter_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/19_throttle_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/20_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/21_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/23_inflight_magnetometer_fit_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/24_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/25_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/26_evaluate_the_aircraft_tune_ff_disable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/27_evaluate_the_aircraft_tune_ff_enable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/28_autotune_roll_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/29_autotune_roll_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/30_autotune_pitch_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/31_autotune_pitch_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/32_autotune_yaw_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/33_autotune_yaw_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/34_autotune_yawd_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/35_autotune_yawd_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/36_autotune_roll_pitch_retune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/37_autotune_roll_pitch_retune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/38_windspeed_estimation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/39_barometer_compensation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/40_system_id_roll.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/41_system_id_pitch.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/42_system_id_yaw.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/43_system_id_thrust.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/44_analytical_pid_optimization.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/45_everyday_use.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/46_position_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)    13406 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/47_precision_land.param
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/48_guided_operation.param
+-rw-r--r--   0 runner    (1001) docker     (127)  1476098 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/apm.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle_components.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:13:34.036244 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/
+-rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/00_default.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/02_imu_temperature_calibration_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/03_imu_temperature_calibration_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/04_board_orientation.param
+-rw-r--r--   0 runner    (1001) docker     (127)    21593 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/05_remote_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/06_telemetry.param
+-rw-r--r--   0 runner    (1001) docker     (127)    15131 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/07_esc.param
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/08_batt1.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/09_batt2.param
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/10_gnss.param
+-rw-r--r--   0 runner    (1001) docker     (127)    34447 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/11_mp_setup_mandatory_hardware.param
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/12_general_configuration.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/13_logging.param
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/14_motor.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/15_pid_adjustment.param
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/16_remote_id.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/17_notch_filter_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/18_notch_filter_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/19_throttle_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/20_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/21_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/23_inflight_magnetometer_fit_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/24_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/25_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/26_evaluate_the_aircraft_tune_ff_disable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/27_evaluate_the_aircraft_tune_ff_enable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/28_autotune_roll_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/29_autotune_roll_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/30_autotune_pitch_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/31_autotune_pitch_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/32_autotune_yaw_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/33_autotune_yaw_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/34_autotune_yawd_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/35_autotune_yawd_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/36_autotune_roll_pitch_retune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/37_autotune_roll_pitch_retune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/38_windspeed_estimation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/39_barometer_compensation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/40_system_id_roll.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/41_system_id_pitch.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/42_system_id_yaw.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/43_system_id_thrust.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/44_analytical_pid_optimization.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/45_everyday_use.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/46_position_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)    13612 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/47_precision_land.param
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/48_guided_operation.param
+-rw-r--r--   0 runner    (1001) docker     (127)  1599965 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/apm.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle_components.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:13:34.052245 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/
+-rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/00_default.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/02_imu_temperature_calibration_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/03_imu_temperature_calibration_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/04_board_orientation.param
+-rw-r--r--   0 runner    (1001) docker     (127)    21636 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/05_remote_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/06_telemetry.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/07_esc.param
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/08_batt1.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/09_batt2.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/10_gnss.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/11_mp_setup_mandatory_hardware.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/12_general_configuration.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/13_logging.param
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/14_motor.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/15_pid_adjustment.param
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/16_remote_id.param
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/17_notch_filter_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/18_notch_filter_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/19_throttle_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/20_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/21_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/23_inflight_magnetometer_fit_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/24_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/25_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/26_evaluate_the_aircraft_tune_ff_disable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/27_evaluate_the_aircraft_tune_ff_enable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/28_autotune_roll_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/29_autotune_roll_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/30_autotune_pitch_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/31_autotune_pitch_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/32_autotune_yaw_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/33_autotune_yaw_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/34_autotune_yawd_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/35_autotune_yawd_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/36_autotune_roll_pitch_retune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/37_autotune_roll_pitch_retune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/38_windspeed_estimation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/39_barometer_compensation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/40_system_id_roll.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/41_system_id_pitch.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/42_system_id_yaw.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/43_system_id_thrust.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/44_analytical_pid_optimization.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/45_everyday_use.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/46_position_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)    14081 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/47_precision_land.param
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/48_guided_operation.param
+-rw-r--r--   0 runner    (1001) docker     (127)  1966610 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/apm.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle_components.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:13:34.064245 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/
+-rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/00_default.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/02_imu_temperature_calibration_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/03_imu_temperature_calibration_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/04_board_orientation.param
+-rw-r--r--   0 runner    (1001) docker     (127)    22629 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/05_remote_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/06_telemetry.param
+-rw-r--r--   0 runner    (1001) docker     (127)    15514 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/07_esc.param
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/08_batt1.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/09_batt2.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/10_gnss.param
+-rw-r--r--   0 runner    (1001) docker     (127)    34447 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/11_mp_setup_mandatory_hardware.param
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/12_general_configuration.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/13_logging.param
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/14_motor.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/15_pid_adjustment.param
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/16_remote_id.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/17_notch_filter_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/18_notch_filter_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/19_throttle_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/20_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/21_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/23_inflight_magnetometer_fit_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/24_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/25_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/26_evaluate_the_aircraft_tune_ff_disable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/27_evaluate_the_aircraft_tune_ff_enable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/28_autotune_roll_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/29_autotune_roll_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/30_autotune_pitch_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/31_autotune_pitch_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/32_autotune_yaw_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/33_autotune_yaw_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/34_autotune_yawd_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/35_autotune_yawd_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/36_autotune_roll_pitch_retune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/37_autotune_roll_pitch_retune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/38_windspeed_estimation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/39_barometer_compensation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     6244 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/40_system_id_roll.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/41_system_id_pitch.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/42_system_id_yaw.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/43_system_id_thrust.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/44_analytical_pid_optimization.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/45_everyday_use.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/46_position_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)    14119 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/47_precision_land.param
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/48_guided_operation.param
+-rw-r--r--   0 runner    (1001) docker     (127)  1982447 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/apm.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle_components.json
```

### Comparing `methodicconfigurator-0.4.0/LICENSE.md` & `methodicconfigurator-0.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.0/MethodicConfigurator/annotate_params.py` & `methodicconfigurator-0.4.2/MethodicConfigurator/annotate_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -461,15 +461,15 @@
         formatted_strings.append(" ".join(row))
 
     return formatted_strings
 
 
 def extract_parameter_name(item: str) -> str:
     """
-    Extract the parameter name from a line. Very simple to be used in sorting
+    Extract the parameter name from a line. Very simple to use in sorting
     """
     item = item.strip()
     match = re.match(PARAM_NAME_REGEX, item)
     return match.group(0) if match else item
 
 
 def missionplanner_sort(item: str) -> Tuple[str, ...]:
@@ -515,15 +515,15 @@
                                    sort_type: str = 'none', param_default_dict: Optional[Dict] = None) -> None:
     """
     Updates the parameter documentation in the target file or in all *.param,*.parm files of the target directory.
 
     This function iterates over all the ArduPilot parameter files in the target directory or file.
     For each file, it DELETES all comments that start at the beginning of a line, optionally sorts the
     parameter names and checks if the parameter name is in the dictionary of parameter documentation.
-    If it is, it prefixes the line with comment derived from the dictionary element.
+    If it is, it prefixes the line with a comment derived from the dictionary element.
     If it's not, it copies the parameter line 1-to-1.
     After processing all the parameters in a file, it writes the new lines back to the file.
 
     Args:
         doc (Dict[str, Any]): A dictionary of parameter documentation.
         target (str, optional): The target directory or file. Defaults to '.'.
         sort_type (str, optional): The type of sorting to apply to the parameters.
@@ -552,15 +552,15 @@
             continue
 
         # Read the entire file contents
         with open(param_file, "r", encoding="utf-8") as file:
             lines = file.readlines()
 
         new_lines = []
-        if os_path.basename(param_file).endswith("14_pid_adjustment.param"):
+        if os_path.basename(param_file).endswith("15_pid_adjustment.param"):
             new_lines.extend(lines[0:7])  # copy the first 8 lines verbatim
 
         total_params = 0
         documented_params = 0
         undocumented_params = []
         is_first_param_in_file = True  # pylint: disable=C0103
         if sort_type == "missionplanner":
```

### Comparing `methodicconfigurator-0.4.0/MethodicConfigurator/ardupilot_methodic_configurator.py` & `methodicconfigurator-0.4.2/MethodicConfigurator/ardupilot_methodic_configurator.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 from logging import getLevelName as logging_getLevelName
 # from logging import debug as logging_debug
 from logging import info as logging_info
 from logging import warning as logging_warning
 from logging import error as logging_error
 from sys import exit as sys_exit
 
-from backend_filesystem import LocalFilesystem
-from backend_flightcontroller import FlightController
+from MethodicConfigurator.backend_filesystem import LocalFilesystem
+from MethodicConfigurator.backend_flightcontroller import FlightController
 
-from frontend_tkinter_connection_selection import ConnectionSelectionWindow
+from MethodicConfigurator.frontend_tkinter_connection_selection import ConnectionSelectionWindow
 
-from frontend_tkinter_directory_selection import VehicleDirectorySelectionWindow
+from MethodicConfigurator.frontend_tkinter_directory_selection import VehicleDirectorySelectionWindow
 
-from frontend_tkinter_component_editor import ComponentEditorWindow
+from MethodicConfigurator.frontend_tkinter_component_editor import ComponentEditorWindow
 
-from frontend_tkinter_parameter_editor import ParameterEditorWindow
+from MethodicConfigurator.frontend_tkinter_parameter_editor import ParameterEditorWindow
 
-from version import VERSION
+from MethodicConfigurator.version import VERSION
 
 
 # pylint: disable=duplicate-code
 def argument_parser():
     """
     Parses command-line arguments for the script.
```

### Comparing `methodicconfigurator-0.4.0/MethodicConfigurator/backend_filesystem.py` & `methodicconfigurator-0.4.2/MethodicConfigurator/backend_filesystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,23 +38,23 @@
 from typing import Tuple
 
 from zipfile import ZipFile
 
 from platformdirs import site_config_dir
 from platformdirs import user_config_dir
 
-from annotate_params import BASE_URL, PARAM_DEFINITION_XML_FILE, Par
-from annotate_params import get_xml_data
-from annotate_params import create_doc_dict
-from annotate_params import format_columns
-from annotate_params import split_into_lines
-from annotate_params import update_parameter_documentation
+from MethodicConfigurator.annotate_params import BASE_URL, PARAM_DEFINITION_XML_FILE, Par
+from MethodicConfigurator.annotate_params import get_xml_data
+from MethodicConfigurator.annotate_params import create_doc_dict
+from MethodicConfigurator.annotate_params import format_columns
+from MethodicConfigurator.annotate_params import split_into_lines
+from MethodicConfigurator.annotate_params import update_parameter_documentation
 
-from backend_filesystem_vehicle_components import VehicleComponents
-from backend_filesystem_configuration_steps import ConfigurationSteps
+from MethodicConfigurator.backend_filesystem_vehicle_components import VehicleComponents
+from MethodicConfigurator.backend_filesystem_configuration_steps import ConfigurationSteps
 
 
 TOOLTIP_MAX_LENGTH = 105
 
 
 def is_within_tolerance(x: float, y: float, atol: float = 1e-08, rtol: float = 1e-03) -> bool:
     """
```

### Comparing `methodicconfigurator-0.4.0/MethodicConfigurator/backend_filesystem_configuration_steps.py` & `methodicconfigurator-0.4.2/MethodicConfigurator/backend_filesystem_configuration_steps.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from logging import error as logging_error
 
 from json import load as json_load
 from json import JSONDecodeError
 
 from typing import Tuple
 
-from annotate_params import Par
+from MethodicConfigurator.annotate_params import Par
 
 
 class ConfigurationSteps:
     """
     A class to manage configuration steps for the ArduPilot methodic configurator.
 
     This class provides methods for reading and validating configuration steps, including forced and derived parameters.
```

### Comparing `methodicconfigurator-0.4.0/MethodicConfigurator/backend_filesystem_vehicle_components.py` & `methodicconfigurator-0.4.2/MethodicConfigurator/backend_filesystem_vehicle_components.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.0/MethodicConfigurator/backend_flightcontroller.py` & `methodicconfigurator-0.4.2/MethodicConfigurator/backend_flightcontroller.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from typing import Dict
 # import usb.core
 # import usb.util
 import serial.tools.list_ports
 import serial.tools.list_ports_common
 
 from serial.serialutil import SerialException
-from annotate_params import Par
+from MethodicConfigurator.annotate_params import Par
 
 # adding all this allows pyinstaller to build a working windows executable
 # note that using --hidden-import does not work for these modules
 try:
     from pymavlink import mavutil
     # import pymavlink.dialects.v20.ardupilotmega
 except Exception: # pylint: disable=broad-exception-caught
```

### Comparing `methodicconfigurator-0.4.0/MethodicConfigurator/backend_mavftp.py` & `methodicconfigurator-0.4.2/MethodicConfigurator/backend_mavftp.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 from random import uniform as random_uniform
 from os import path as os_path
 from typing import Dict
 
 from io import BytesIO as SIO
 
 # from param_ftp import ParamData
-from param_ftp import ftp_param_decode
+from MethodicConfigurator.param_ftp import ftp_param_decode
 
-from common_arguments import add_common_arguments_and_parse
+from MethodicConfigurator.common_arguments import add_common_arguments_and_parse
 
-from backend_flightcontroller import FlightController
+from MethodicConfigurator.backend_flightcontroller import FlightController
 
 # adding all this allows pyinstaller to build a working Windows executable
 # note that using --hidden-import does not work for these modules
 try:
     from pymavlink import mavutil
     from pymavlink import mavparm
 except ImportError:
```

### Comparing `methodicconfigurator-0.4.0/MethodicConfigurator/battery_cell_voltages.py` & `methodicconfigurator-0.4.2/MethodicConfigurator/battery_cell_voltages.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.0/MethodicConfigurator/common_arguments.py` & `methodicconfigurator-0.4.2/MethodicConfigurator/common_arguments.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 This file is part of Ardupilot methodic configurator. https://github.com/ArduPilot/MethodicConfigurator
 
 (C) 2024 Amilcar do Carmo Lucas, IAV GmbH
 
 SPDX-License-Identifier:    GPL-3
 '''
 
-from version import VERSION
+from MethodicConfigurator.version import VERSION
 
 
 def add_common_arguments_and_parse(parser):
     parser.add_argument('--loglevel',
                         type=str,
                         default='INFO',
                         choices=['DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL'],
```

### Comparing `methodicconfigurator-0.4.0/MethodicConfigurator/extract_param_defaults.py` & `methodicconfigurator-0.4.2/MethodicConfigurator/extract_param_defaults.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.0/MethodicConfigurator/frontend_tkinter_base.py` & `methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from logging import error as logging_error
 
 from platform import system as platform_system
 
 from PIL import Image
 from PIL import ImageTk
 
-from backend_filesystem import LocalFilesystem
+from MethodicConfigurator.backend_filesystem import LocalFilesystem
 
 
 def show_error_message(title: str, message: str):
     root = tk.Tk()
     # Set the theme to 'alt'
     style = ttk.Style()
     style.theme_use('alt')
```

### Comparing `methodicconfigurator-0.4.0/MethodicConfigurator/frontend_tkinter_component_editor.py` & `methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_component_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 from logging import getLevelName as logging_getLevelName
 # from logging import debug as logging_debug
 #from logging import info as logging_info
 
 import tkinter as tk
 from tkinter import ttk
 
-from common_arguments import add_common_arguments_and_parse
+from MethodicConfigurator.common_arguments import add_common_arguments_and_parse
 
-from backend_filesystem import LocalFilesystem
+from MethodicConfigurator.backend_filesystem import LocalFilesystem
 
-from battery_cell_voltages import BatteryCell
+from MethodicConfigurator.battery_cell_voltages import BatteryCell
 
-from frontend_tkinter_component_editor_base import ComponentEditorWindowBase
+from MethodicConfigurator.frontend_tkinter_component_editor_base import ComponentEditorWindowBase
 
-#from frontend_tkinter_base import show_tooltip
-from frontend_tkinter_base import show_error_message
+#from MethodicConfigurator.frontend_tkinter_base import show_tooltip
+from MethodicConfigurator.frontend_tkinter_base import show_error_message
 
-from version import VERSION
+from MethodicConfigurator.version import VERSION
 
 
 def argument_parser():
     """
     Parses command-line arguments for the script.
 
     This function sets up an argument parser to handle the command-line arguments for the script.
```

### Comparing `methodicconfigurator-0.4.0/MethodicConfigurator/frontend_tkinter_component_editor_base.py` & `methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_component_editor_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 from logging import getLevelName as logging_getLevelName
 # from logging import debug as logging_debug
 from logging import info as logging_info
 
 import tkinter as tk
 from tkinter import ttk
 
-from common_arguments import add_common_arguments_and_parse
+from MethodicConfigurator.common_arguments import add_common_arguments_and_parse
 
-from backend_filesystem import LocalFilesystem
+from MethodicConfigurator.backend_filesystem import LocalFilesystem
 
-from frontend_tkinter_base import show_tooltip
-from frontend_tkinter_base import show_error_message
-from frontend_tkinter_base import ScrollFrame
-from frontend_tkinter_base import BaseWindow
+from MethodicConfigurator.frontend_tkinter_base import show_tooltip
+from MethodicConfigurator.frontend_tkinter_base import show_error_message
+from MethodicConfigurator.frontend_tkinter_base import ScrollFrame
+from MethodicConfigurator.frontend_tkinter_base import BaseWindow
 
-from version import VERSION
+from MethodicConfigurator.version import VERSION
 
 
 def argument_parser():
     """
     Parses command-line arguments for the script.
 
     This function sets up an argument parser to handle the command-line arguments for the script.
```

### Comparing `methodicconfigurator-0.4.0/MethodicConfigurator/frontend_tkinter_connection_selection.py` & `methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_connection_selection.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,23 +18,23 @@
 from logging import warning as logging_warning
 from logging import critical as logging_critical
 
 import tkinter as tk
 from tkinter import ttk
 from tkinter import simpledialog
 
-from common_arguments import add_common_arguments_and_parse
+from MethodicConfigurator.common_arguments import add_common_arguments_and_parse
 
-from backend_flightcontroller import FlightController
+from MethodicConfigurator.backend_flightcontroller import FlightController
 
-from frontend_tkinter_base import show_no_connection_error
-from frontend_tkinter_base import show_tooltip
-from frontend_tkinter_base import update_combobox_width
-from frontend_tkinter_base import ProgressWindow
-from frontend_tkinter_base import BaseWindow
+from MethodicConfigurator.frontend_tkinter_base import show_no_connection_error
+from MethodicConfigurator.frontend_tkinter_base import show_tooltip
+from MethodicConfigurator.frontend_tkinter_base import update_combobox_width
+from MethodicConfigurator.frontend_tkinter_base import ProgressWindow
+from MethodicConfigurator.frontend_tkinter_base import BaseWindow
 
 
 # https://dev.to/geraldew/python-tkinter-an-exercise-in-wrapping-the-combobox-ndb
 class PairTupleCombobox(ttk.Combobox):  # pylint: disable=too-many-ancestors
     """
     A custom Combobox widget that allows for the display of a list of tuples, where each tuple contains a key and a value.
     This widget processes the list of tuples to separate keys and values for display purposes, and allows for the selection
```

### Comparing `methodicconfigurator-0.4.0/MethodicConfigurator/frontend_tkinter_directory_selection.py` & `methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_directory_selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,22 +20,22 @@
 from logging import warning as logging_warning
 from logging import debug as logging_error
 
 import tkinter as tk
 from tkinter import ttk
 from tkinter import filedialog
 
-from common_arguments import add_common_arguments_and_parse
+from MethodicConfigurator.common_arguments import add_common_arguments_and_parse
 
-from backend_filesystem import LocalFilesystem
+from MethodicConfigurator.backend_filesystem import LocalFilesystem
 
-from frontend_tkinter_base import show_error_message
-from frontend_tkinter_base import show_no_param_files_error
-from frontend_tkinter_base import show_tooltip
-from frontend_tkinter_base import BaseWindow
+from MethodicConfigurator.frontend_tkinter_base import show_error_message
+from MethodicConfigurator.frontend_tkinter_base import show_no_param_files_error
+from MethodicConfigurator.frontend_tkinter_base import show_tooltip
+from MethodicConfigurator.frontend_tkinter_base import BaseWindow
 
 
 class DirectorySelectionWidgets():
     """
     A class to manage directory selection widgets in the GUI.
 
     This class provides functionality for creating and managing widgets related to directory selection,
```

### Comparing `methodicconfigurator-0.4.0/MethodicConfigurator/frontend_tkinter_parameter_editor.py` & `methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_parameter_editor.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,31 +20,31 @@
 #from logging import critical as logging_critical
 
 from typing import List
 from typing import Tuple
 
 from webbrowser import open as webbrowser_open  # to open the blog post documentation
 
-from backend_filesystem import LocalFilesystem
-from backend_filesystem import is_within_tolerance
+from MethodicConfigurator.backend_filesystem import LocalFilesystem
+from MethodicConfigurator.backend_filesystem import is_within_tolerance
 
-from backend_flightcontroller import FlightController
+from MethodicConfigurator.backend_flightcontroller import FlightController
 
-from frontend_tkinter_base import show_tooltip
-from frontend_tkinter_base import AutoResizeCombobox
-from frontend_tkinter_base import ProgressWindow
-from frontend_tkinter_base import BaseWindow
+from MethodicConfigurator.frontend_tkinter_base import show_tooltip
+from MethodicConfigurator.frontend_tkinter_base import AutoResizeCombobox
+from MethodicConfigurator.frontend_tkinter_base import ProgressWindow
+from MethodicConfigurator.frontend_tkinter_base import BaseWindow
 
-from frontend_tkinter_connection_selection import ConnectionSelectionWidgets
+from MethodicConfigurator.frontend_tkinter_connection_selection import ConnectionSelectionWidgets
 
-from frontend_tkinter_directory_selection import VehicleDirectorySelectionWidgets
+from MethodicConfigurator.frontend_tkinter_directory_selection import VehicleDirectorySelectionWidgets
 
-from frontend_tkinter_parameter_editor_table import ParameterEditorTable
+from MethodicConfigurator.frontend_tkinter_parameter_editor_table import ParameterEditorTable
 
-from tempcal_imu import IMUfit
+from MethodicConfigurator.tempcal_imu import IMUfit
 
 
 class DocumentationFrame:  # pylint: disable=too-few-public-methods
     """
     A class to manage and display documentation within the GUI.
 
     This class is responsible for creating a frame that displays
```

### Comparing `methodicconfigurator-0.4.0/MethodicConfigurator/frontend_tkinter_parameter_editor_table.py` & `methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_parameter_editor_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,26 +16,26 @@
 
 from logging import debug as logging_debug
 from logging import info as logging_info
 #from logging import warning as logging_warning
 #from logging import error as logging_error
 from logging import critical as logging_critical
 
-#from backend_filesystem import LocalFilesystem
-from backend_filesystem import is_within_tolerance
+#from MethodicConfigurator.backend_filesystem import LocalFilesystem
+from MethodicConfigurator.backend_filesystem import is_within_tolerance
 
-#from backend_flightcontroller import FlightController
+#from MethodicConfigurator.backend_flightcontroller import FlightController
 
-from frontend_tkinter_base import show_tooltip
-#from frontend_tkinter_base import AutoResizeCombobox
-from frontend_tkinter_base import ScrollFrame
+from MethodicConfigurator.frontend_tkinter_base import show_tooltip
+#from MethodicConfigurator.frontend_tkinter_base import AutoResizeCombobox
+from MethodicConfigurator.frontend_tkinter_base import ScrollFrame
 
 
 
-class ParameterEditorTable(ScrollFrame):
+class ParameterEditorTable(ScrollFrame):  # pylint: disable=too-many-ancestors
     """
     A class to manage and display the parameter editor table within the GUI.
 
     This class inherits from ScrollFrame and is responsible for creating,
     managing, and updating the table that displays parameters for editing.
     """
     def __init__(self, root, local_filesystem):
```

### Comparing `methodicconfigurator-0.4.0/MethodicConfigurator/get_release_stats.py` & `methodicconfigurator-0.4.2/MethodicConfigurator/get_release_stats.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.0/MethodicConfigurator/param_ftp.py` & `methodicconfigurator-0.4.2/MethodicConfigurator/param_ftp.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.0/MethodicConfigurator/param_pid_adjustment_update.py` & `methodicconfigurator-0.4.2/MethodicConfigurator/param_pid_adjustment_update.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.0/MethodicConfigurator/tempcal_imu.py` & `methodicconfigurator-0.4.2/MethodicConfigurator/tempcal_imu.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.0/MethodicConfigurator.egg-info/PKG-INFO` & `methodicconfigurator-0.4.2/MethodicConfigurator.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MethodicConfigurator
-Version: 0.4.0
+Version: 0.4.2
 Summary: A clear configuration sequence for ArduPilot vehicles
 Home-page: https://github.com/ArduPilot/MethodicConfigurator
 Author: Amilcar do Carmo Lucas
 Author-email: amilcar.lucas@iav.de
 License: GPLv3
 Keywords: ArduPilot,Configuration,SCM,Methodic,ArduCopter,ArduPlane,ArduRover,ArduSub
 Classifier: Development Status :: 3 - Alpha
@@ -13,14 +13,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: platformdirs
```

### Comparing `methodicconfigurator-0.4.0/PKG-INFO` & `methodicconfigurator-0.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MethodicConfigurator
-Version: 0.4.0
+Version: 0.4.2
 Summary: A clear configuration sequence for ArduPilot vehicles
 Home-page: https://github.com/ArduPilot/MethodicConfigurator
 Author: Amilcar do Carmo Lucas
 Author-email: amilcar.lucas@iav.de
 License: GPLv3
 Keywords: ArduPilot,Configuration,SCM,Methodic,ArduCopter,ArduPlane,ArduRover,ArduSub
 Classifier: Development Status :: 3 - Alpha
@@ -13,14 +13,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: platformdirs
```

### Comparing `methodicconfigurator-0.4.0/README.md` & `methodicconfigurator-0.4.2/README.md`

 * *Files identical despite different names*

