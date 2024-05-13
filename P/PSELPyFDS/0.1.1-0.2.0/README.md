# Comparing `tmp/PSELPyFDS-0.1.1-py3-none-any.whl.zip` & `tmp/PSELPyFDS-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 14537 bytes, number of entries: 9
+Zip file size: 14341 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat      388 b- defN 23-Sep-13 15:44 PSELPyFDS/__init__.py
--rw-rw-rw-  2.0 fat      125 b- defN 24-Feb-14 15:16 PSELPyFDS/__version__.py
--rw-rw-rw-  2.0 fat      938 b- defN 23-Sep-13 15:44 PSELPyFDS/_fds_mixin.py
--rw-rw-rw-  2.0 fat    67446 b- defN 24-Feb-14 15:16 PSELPyFDS/fds.py
--rw-rw-rw-  2.0 fat     1115 b- defN 24-Feb-14 15:30 PSELPyFDS-0.1.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1750 b- defN 24-Feb-14 15:30 PSELPyFDS-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Feb-14 15:30 PSELPyFDS-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-Feb-14 15:30 PSELPyFDS-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      710 b- defN 24-Feb-14 15:30 PSELPyFDS-0.1.1.dist-info/RECORD
-9 files, 72574 bytes uncompressed, 13317 bytes compressed:  81.7%
+-rw-rw-rw-  2.0 fat      125 b- defN 24-May-13 16:02 PSELPyFDS/__version__.py
+-rw-rw-rw-  2.0 fat      990 b- defN 24-May-13 16:02 PSELPyFDS/_fds_mixin.py
+-rw-rw-rw-  2.0 fat    64174 b- defN 24-May-13 16:02 PSELPyFDS/fds.py
+-rw-rw-rw-  2.0 fat     1115 b- defN 24-May-13 16:16 PSELPyFDS-0.2.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1746 b- defN 24-May-13 16:16 PSELPyFDS-0.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-13 16:16 PSELPyFDS-0.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 24-May-13 16:16 PSELPyFDS-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      710 b- defN 24-May-13 16:16 PSELPyFDS-0.2.0.dist-info/RECORD
+9 files, 69350 bytes uncompressed, 13121 bytes compressed:  81.1%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: PSELPyFDS/_fds_mixin.py
 Comment: 
 
 Filename: PSELPyFDS/fds.py
 Comment: 
 
-Filename: PSELPyFDS-0.1.1.dist-info/LICENSE.txt
+Filename: PSELPyFDS-0.2.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: PSELPyFDS-0.1.1.dist-info/METADATA
+Filename: PSELPyFDS-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: PSELPyFDS-0.1.1.dist-info/WHEEL
+Filename: PSELPyFDS-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: PSELPyFDS-0.1.1.dist-info/top_level.txt
+Filename: PSELPyFDS-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: PSELPyFDS-0.1.1.dist-info/RECORD
+Filename: PSELPyFDS-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## PSELPyFDS/__version__.py

```diff
@@ -1,5 +1,5 @@
 from __future__ import annotations
 
 #  Copyright (c) 2023. Photonic Science and Engineering Ltd.
 
-__version__ = "0.1.1"
+__version__ = "0.2.0"
```

## PSELPyFDS/_fds_mixin.py

```diff
@@ -14,14 +14,16 @@
     CameraOptionsMixin,
     CameraTypeMixin,
     ClockSpeedABC,
     ConnectionABC,
     DLLABC,
     ExposureABC,
     FlatFieldCorrectionABC,
+    FusionABC,
+    FusionNoiseReductionFactorABC,
     HardwareBinningABC,
     HighPrecisionRemapping,
     ImageModeABC,
     IntensifierGainABC,
     IPortABC,
     Is14BitCameraABC,
     IsCyclopsCameraABC,
```

## PSELPyFDS/fds.py

```diff
@@ -71,22 +71,14 @@
         self.sub_area = (0, 1367, 0, 1039)
         self.software_binning = (1, 1)
         self.hardware_binning = (1, 1)
 
         self._mode = ImageMode.I16
         self._byte_depth = 2
 
-        # Manage Calibration Files
-        # Flat Field
-        self._calibration_files_flat_field_use_user_file = False
-        self._calibration_files_flat_field_user_file_image_file = None
-        self._calibration_files_flat_field_user_file_pedestal = 100
-        self._calibration_files_flat_field_user_file_scale_factor = 1
-        self._calibration_files_flat_field_save_flat_average = 10
-
         # Remapping
         self.remapping = False
         self._smooth = False
         self._clip = True
         self._remap_x = 0
         self._remap_y = 0
         self._remap_rotation = 0
@@ -157,74 +149,14 @@
                                     "value": False,
                                 },
                             ],
                             key=lambda x: str(x["name"]),
                         ),
                     },
                     {
-                        "name": "Manage Calibration Files",
-                        "type": "group",
-                        "children": [
-                            {
-                                "name": "Flat Field",
-                                "type": "group",
-                                "children": [
-                                    {
-                                        "name": (
-                                            "calibration_files_flat_field_use_user_file"
-                                        ),
-                                        "title": "User file",
-                                        "type": "bool",
-                                        "value": self._calibration_files_flat_field_use_user_file,
-                                        "children": [
-                                            {
-                                                "name": "calibration_files_flat_field_user_file_image_file",
-                                                "title": "Image File",
-                                                "type": "file",
-                                                "fileMode": "ExistingFile",
-                                                "directory": str(
-                                                    self._camera_directory
-                                                ),
-                                                "value": self._calibration_files_flat_field_user_file_image_file,
-                                            },
-                                            {
-                                                "name": "calibration_files_flat_field_user_file_pedestal",
-                                                "title": "Pedestal",
-                                                "type": "int",
-                                                "value": self._calibration_files_flat_field_user_file_pedestal,
-                                                "limits": (0, 100_000),
-                                            },
-                                            {
-                                                "name": "calibration_files_flat_field_user_file_scale_factor",
-                                                "title": "Scale Factor",
-                                                "type": "int",
-                                                "value": self._calibration_files_flat_field_user_file_scale_factor,
-                                                "limits": (1, 1_000_000),
-                                            },
-                                        ],
-                                    },
-                                    {
-                                        "name": "calibration_files_flat_field_save",
-                                        "title": "save",
-                                        "type": "action",
-                                        "children": [
-                                            {
-                                                "name": "calibration_files_flat_field_save_flat_average",
-                                                "title": "Flat Average",
-                                                "type": "int",
-                                                "value": self._calibration_files_flat_field_save_flat_average,
-                                                "limits": (1, 256),
-                                            }
-                                        ],
-                                    },
-                                ],
-                            },
-                        ],
-                    },
-                    {
                         "name": "Camera Mode",
                         "type": "group",
                         "children": [
                             {
                                 "name": "clock_speed_mode",
                                 "title": "Clock Speed Mode",
                                 "type": "list",
@@ -371,58 +303,58 @@
                                         "type": "bool",
                                         "value": False,
                                     },
                                 ],
                             },
                         ],
                     },
-                    {
-                        "name": "Flouresence",
-                        "type": "group",
-                        "children": [
-                            {
-                                "name": "flouresence_exposure_start_delay",
-                                "title": "ExposureStartDelay",
-                                "type": "int",
-                                "value": 0,
-                                "limits": (0, 1_000_000_000),
-                            },
-                            {
-                                "name": "flouresence_trigger_out_high_time",
-                                "title": "TriggerOutHighTime",
-                                "type": "int",
-                                "value": 0,
-                                "limits": (0, 1_000_000_000),
-                            },
-                        ],
-                    },
+                    # {
+                    #     "name": "Flouresence",
+                    #     "type": "group",
+                    #     "children": [
+                    #         {
+                    #             "name": "flouresence_exposure_start_delay",
+                    #             "title": "ExposureStartDelay",
+                    #             "type": "int",
+                    #             "value": 0,
+                    #             "limits": (0, 1_000_000_000),
+                    #         },
+                    #         {
+                    #             "name": "flouresence_trigger_out_high_time",
+                    #             "title": "TriggerOutHighTime",
+                    #             "type": "int",
+                    #             "value": 0,
+                    #             "limits": (0, 1_000_000_000),
+                    #         },
+                    #     ],
+                    # },
                     {
                         "name": "Sub Area",
                         "type": "group",
                         "children": [
                             {
                                 "name": "sub_area",
                                 "title": "(L, R, T, B)",
                                 "type": "subarea",
                                 "value": (0, 1367, 0, 1039),
                             },
                         ],
                     },
-                    {
-                        "name": "Auto Level",
-                        "type": "group",
-                        "children": [
-                            {
-                                "name": "auto_level",
-                                "title": "Auto Level",
-                                "type": "bool",
-                                "value": self._auto_level,
-                            }
-                        ],
-                    },
+                    # {
+                    #     "name": "Auto Level",
+                    #     "type": "group",
+                    #     "children": [
+                    #         {
+                    #             "name": "auto_level",
+                    #             "title": "Auto Level",
+                    #             "type": "bool",
+                    #             "value": self._auto_level,
+                    #         }
+                    #     ],
+                    # },
                     {
                         "name": "Miscellaneous",
                         "type": "group",
                         "children": [
                             {
                                 "name": "reset_camera",
                                 "title": "Reset Camera",
@@ -432,21 +364,24 @@
                     },
                     # {"name": "", "type": "", "value": ""},  # Template
                 ],  # children
             }
         ]
 
         self._set_camera_option_routing_dict = {
+            "bin2mode": self.enable_bin2_mode,
             "bright_corner": self.enable_bright_corner_correction,
             "bright_pixel": self.enable_bright_pixel_correction,
             "bright_spot": self.enable_bright_spot_correction,
             "clock_speed_mode": self.set_clock_speed,
+            "enable_fusion": self.enable_fusion,
             "enable_remapping": self.enable_remapping,
             "exposure": self.set_exposure,
             "flat_field": self.enable_flat_field_correction,
+            "fusion_noise_average": self.set_fusion_noise_reduction_factor,
             "hardware_binning": self.set_hardware_binning,
             "HPM_angular": self.set_HPM_angular,
             "HPM_rotation": self.set_HPM_rotation,
             "HPM_sub_height": self.set_HPM_sub_height,
             "HPM_sub_width": self.set_HPM_sub_width,
             "HPM_x": self.set_HPM_x,
             "HPM_y": self.set_HPM_y,
@@ -491,14 +426,16 @@
         self.dll.PSL_VHR_Close.restype = ct.c_bool
         self.dll.PSL_VHR_enable_auto_gain_control.argtypes = [ct.c_bool]
         self.dll.PSL_VHR_enable_auto_gain_control.restype = ct.c_bool
         self.dll.PSL_VHR_enable_bright_corner_subtraction.argtypes = [ct.c_bool]
         self.dll.PSL_VHR_enable_bright_corner_subtraction.restype = ct.c_bool
         self.dll.PSL_VHR_enable_bright_pixel_correction.argtypes = [ct.c_bool]
         self.dll.PSL_VHR_enable_bright_pixel_correction.restype = ct.c_bool
+        self.dll.PSL_VHR_enable_cyclops_bin2_mode.argtypes = [ct.c_bool]
+        self.dll.PSL_VHR_enable_cyclops_bin2_mode.restype = None
         self.dll.PSL_VHR_enable_flat_field_correction.argtypes = [ct.c_bool]
         self.dll.PSL_VHR_enable_flat_field_correction.restype = ct.c_bool
         self.dll.PSL_VHR_enable_image_streaming.argtypes = [ct.c_bool]
         self.dll.PSL_VHR_enable_image_streaming.restype = None
         self.dll.PSL_VHR_enable_offset_subtraction.argtypes = [ct.c_bool]
         self.dll.PSL_VHR_enable_offset_subtraction.restype = ct.c_bool
         self.dll.PSL_VHR_enable_sharpening.argtypes = [ct.c_bool]
@@ -1110,14 +1047,26 @@
         if mode == "12.5MHz":
             return _map_result_to_enum(self.dll.PSL_VHR_set_speed(0))
         elif mode == "25MHz":
             return _map_result_to_enum(self.dll.PSL_VHR_set_speed(1))
         else:
             return OptionSetterResult.FAILED
 
+    def enable_fusion(self, enable: bool) -> OptionSetterResult:
+        self.fusion = enable
+        return OptionSetterResult.COMPLETED
+
+    def set_fusion_noise_reduction_factor(self, value: int) -> OptionSetterResult:
+        self._noise_reduction_factor = value
+        return OptionSetterResult.COMPLETED
+
+    def enable_bin2_mode(self, enable: bool) -> OptionSetterResult:
+        self.dll.PSL_VHR_enable_cyclops_bin2_mode(enable)
+        return OptionSetterResult.COMPLETED
+
     """Image Acquisition"""
 
     def snap(self) -> bool:
         """Acquire an image. This function will block for the duration of the exposure
         time.
 
         Type of acquisition performed depends on if the camera is
```

## Comparing `PSELPyFDS-0.1.1.dist-info/LICENSE.txt` & `PSELPyFDS-0.2.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `PSELPyFDS-0.1.1.dist-info/METADATA` & `PSELPyFDS-0.2.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PSELPyFDS
-Version: 0.1.1
+Version: 0.2.0
 Summary: Package for FDS camera
 Home-page: https://photonicscience.com
 Author: Photonic Science and Engineering Ltd.
 Author-email: support@photonicscience.com
 License: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -19,16 +19,16 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: numpy (>=1.18.0)
-Requires-Dist: PSELPyBaseCamera (>=0.1.0)
+Requires-Dist: numpy >=1.18.0
+Requires-Dist: PSELPyBaseCamera >=0.2.0
 
 # README #
 
 PSELPyFDS is the Photonic Science Python integration for the FDS camera.
 
 ### It provides ###
```

