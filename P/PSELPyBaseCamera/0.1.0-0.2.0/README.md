# Comparing `tmp/PSELPyBaseCamera-0.1.0-py3-none-any.whl.zip` & `tmp/PSELPyBaseCamera-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 13811 bytes, number of entries: 16
+Zip file size: 14020 bytes, number of entries: 16
 -rw-rw-rw-  2.0 fat      449 b- defN 23-Jun-22 14:12 PSELPyBaseCamera/__init__.py
--rw-rw-rw-  2.0 fat      208 b- defN 23-Jun-22 14:12 PSELPyBaseCamera/__version__.py
+-rw-rw-rw-  2.0 fat      208 b- defN 24-May-13 15:00 PSELPyBaseCamera/__version__.py
 -rw-rw-rw-  2.0 fat     6447 b- defN 23-Jun-22 14:12 PSELPyBaseCamera/helper.py
 -rw-rw-rw-  2.0 fat     2818 b- defN 23-Jun-22 14:12 PSELPyBaseCamera/image_modes.py
 -rw-rw-rw-  2.0 fat     2006 b- defN 23-Jun-22 14:12 PSELPyBaseCamera/logging_tools.py
--rw-rw-rw-  2.0 fat     3117 b- defN 23-Jun-22 14:12 PSELPyBaseCamera/_abcs_mixins/__init__.py
--rw-rw-rw-  2.0 fat    17740 b- defN 23-Jun-22 14:12 PSELPyBaseCamera/_abcs_mixins/_abcs_mixins.py
+-rw-rw-rw-  2.0 fat     3411 b- defN 24-May-13 14:59 PSELPyBaseCamera/_abcs_mixins/__init__.py
+-rw-rw-rw-  2.0 fat    19371 b- defN 24-May-13 14:59 PSELPyBaseCamera/_abcs_mixins/_abcs_mixins.py
 -rw-rw-rw-  2.0 fat      325 b- defN 23-Jun-22 14:12 PSELPyBaseCamera/options/__init__.py
 -rw-rw-rw-  2.0 fat      761 b- defN 23-Jun-22 14:12 PSELPyBaseCamera/options/errors.py
 -rw-rw-rw-  2.0 fat      691 b- defN 23-Jun-22 14:12 PSELPyBaseCamera/options/results.py
 -rw-rw-rw-  2.0 fat      184 b- defN 23-Jun-22 14:12 PSELPyBaseCamera/options/types.py
--rw-rw-rw-  2.0 fat     1115 b- defN 23-Jun-22 14:13 PSELPyBaseCamera-0.1.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1584 b- defN 23-Jun-22 14:13 PSELPyBaseCamera-0.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-22 14:13 PSELPyBaseCamera-0.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-22 14:13 PSELPyBaseCamera-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1430 b- defN 23-Jun-22 14:13 PSELPyBaseCamera-0.1.0.dist-info/RECORD
-16 files, 38984 bytes uncompressed, 11411 bytes compressed:  70.7%
+-rw-rw-rw-  2.0 fat     1115 b- defN 24-May-13 15:04 PSELPyBaseCamera-0.2.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1584 b- defN 24-May-13 15:04 PSELPyBaseCamera-0.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-13 15:04 PSELPyBaseCamera-0.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 24-May-13 15:04 PSELPyBaseCamera-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1430 b- defN 24-May-13 15:04 PSELPyBaseCamera-0.2.0.dist-info/RECORD
+16 files, 40909 bytes uncompressed, 11620 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: PSELPyBaseCamera/options/results.py
 Comment: 
 
 Filename: PSELPyBaseCamera/options/types.py
 Comment: 
 
-Filename: PSELPyBaseCamera-0.1.0.dist-info/LICENSE.txt
+Filename: PSELPyBaseCamera-0.2.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: PSELPyBaseCamera-0.1.0.dist-info/METADATA
+Filename: PSELPyBaseCamera-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: PSELPyBaseCamera-0.1.0.dist-info/WHEEL
+Filename: PSELPyBaseCamera-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: PSELPyBaseCamera-0.1.0.dist-info/top_level.txt
+Filename: PSELPyBaseCamera-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: PSELPyBaseCamera-0.1.0.dist-info/RECORD
+Filename: PSELPyBaseCamera-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## PSELPyBaseCamera/__version__.py

```diff
@@ -1,7 +1,7 @@
 #  Copyright (c) 2023. Photonic Science and Engineering Ltd.
 from __future__ import annotations
 
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 
 # Detail what changed in version if required
-__version_text__ = "Release v0.1.0"
+__version_text__ = "Release v0.2.0"
```

## PSELPyBaseCamera/_abcs_mixins/__init__.py

```diff
@@ -8,17 +8,21 @@
 from ._abcs_mixins import BrightSpotCorrectionABC
 from ._abcs_mixins import CameraNameMixin
 from ._abcs_mixins import CameraOptionsMixin
 from ._abcs_mixins import CameraTypeMixin
 from ._abcs_mixins import ClockSpeedABC
 from ._abcs_mixins import ConnectionABC
 from ._abcs_mixins import CoolingModeABC
+from ._abcs_mixins import CyclopsBin2ModeABC
 from ._abcs_mixins import DLLABC
 from ._abcs_mixins import ExposureABC
 from ._abcs_mixins import FlatFieldCorrectionABC
+from ._abcs_mixins import FusionABC
+from ._abcs_mixins import FusionLowNoiseABC
+from ._abcs_mixins import FusionNoiseReductionFactorABC
 from ._abcs_mixins import GainModeABC
 from ._abcs_mixins import HardwareBinningABC
 from ._abcs_mixins import HighPrecisionRemapping
 from ._abcs_mixins import ImageModeABC
 from ._abcs_mixins import IntensifierGainABC
 from ._abcs_mixins import IPortABC
 from ._abcs_mixins import Is14BitCameraABC
@@ -48,17 +52,21 @@
     "CameraNameMixin",
     "CameraOptionsMixin",
     "CameraTypeMixin",
     "ClockSpeedABC",
     "ConnectionABC",
     "CoolingModeABC",
     "CoreCamera",
+    "CyclopsBin2ModeABC",
     "DLLABC",
     "ExposureABC",
     "FlatFieldCorrectionABC",
+    "FusionABC",
+    "FusionLowNoiseABC",
+    "FusionNoiseReductionFactorABC",
     "GainModeABC",
     "HardwareBinningABC",
     "HighPrecisionRemapping",
     "ImageModeABC",
     "IntensifierGainABC",
     "IPortABC",
     "Is14BitCameraABC",
```

## PSELPyBaseCamera/_abcs_mixins/_abcs_mixins.py

```diff
@@ -26,17 +26,21 @@
     "BrightSpotCorrectionABC",
     "CameraNameMixin",
     "CameraOptionsMixin",
     "CameraTypeMixin",
     "ClockSpeedABC",
     "ConnectionABC",
     "CoolingModeABC",
+    "CyclopsBin2ModeABC",
     "DLLABC",
     "ExposureABC",
     "FlatFieldCorrectionABC",
+    "FusionABC",
+    "FusionLowNoiseABC",
+    "FusionNoiseReductionFactorABC",
     "GainModeABC",
     "HardwareBinningABC",
     "HighPrecisionRemapping",
     "ImageModeABC",
     "IntensifierGainABC",
     "IPortABC",
     "Is14BitCameraABC",
@@ -363,14 +367,58 @@
 
 class StreamingABC(ABC):
     @abstractmethod
     def enable_streaming(self, enable: bool):
         raise NotImplementedError
 
 
+class FusionABC(ABC):
+    def __init_subclass__(cls, **kwargs):
+        # This ABC requires AcquisitionABC to be present
+        if not issubclass(cls, AcquisitionABC):
+            raise TypeError(
+                f"{__class__.__name__} requires AcquisitionABC to be inherited."
+            )
+
+        # This ABC requires Is14BitCameraABC to be present
+        if not issubclass(cls, Is14BitCameraABC):
+            raise TypeError(
+                f"{__class__.__name__} requires Is14BitCameraABC to be inherited."
+            )
+        super().__init_subclass__(**kwargs)
+
+    def enable_fusion(self, enable: bool):
+        raise NotImplementedError
+
+
+class FusionNoiseReductionFactorABC(ABC):
+    def __init_subclass__(cls, **kwargs):
+        # This ABC requires FusionABC to be present
+        if not issubclass(cls, FusionABC):
+            raise TypeError(f"{__class__.__name__} requires FusionABC to be inherited.")
+
+    def set_fusion_noise_reduction_factor(self, value: int):
+        raise NotImplementedError
+
+
+class FusionLowNoiseABC(ABC):
+    def __init_subclass__(cls, **kwargs):
+        # This ABC requires FusionABC to be present
+        if not issubclass(cls, FusionABC):
+            raise TypeError(f"{__class__.__name__} requires FusionABC to be inherited.")
+
+    def enable_fusion_low_noise(self, enable: bool):
+        raise NotImplementedError
+
+
+class CyclopsBin2ModeABC(ABC):
+    def enable_bin2_mode(self, enable: bool):
+        raise NotImplementedError
+
+
 # Corrections
 
 
 class OffsetSubtractionABC(ABC):
     @abstractmethod
     def enable_offset_subtraction(self, enable: bool):
         raise NotImplementedError
```

## Comparing `PSELPyBaseCamera-0.1.0.dist-info/LICENSE.txt` & `PSELPyBaseCamera-0.2.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `PSELPyBaseCamera-0.1.0.dist-info/METADATA` & `PSELPyBaseCamera-0.2.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: PSELPyBaseCamera
-Version: 0.1.0
+Version: 0.2.0
 Summary: Package for base camera
 Home-page: https://photonicscience.com
 Author: Photonic Science and Engineering Ltd.
 Author-email: support@photonicscience.com
-License: LICENSE.txt
+License: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

## Comparing `PSELPyBaseCamera-0.1.0.dist-info/RECORD` & `PSELPyBaseCamera-0.2.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 PSELPyBaseCamera/__init__.py,sha256=MqvDYOfWhwz_pNQck1RhYvgkQDiBRQhxH60iT3kZe60,449
-PSELPyBaseCamera/__version__.py,sha256=1JMR8Lq9lkaYUAJV4NSSflGmOxsuiPqn_5psXAd__KI,208
+PSELPyBaseCamera/__version__.py,sha256=TMD-T0PX2yc9Z4t7h_g0KJOwq-PYCUJoXy34RoTaifc,208
 PSELPyBaseCamera/helper.py,sha256=jOTo2DIyTjRA9RmX1H-XRr2adXCQTRi9Tw6_sikT9vA,6447
 PSELPyBaseCamera/image_modes.py,sha256=ZiK1Uln0g-QcOShMVHMrxtisMK4mUI4F2caZaei7oKE,2818
 PSELPyBaseCamera/logging_tools.py,sha256=hkfuMsoLySIgfmXsFpAZissVl94h6uEssxNYFIOBr1Y,2006
-PSELPyBaseCamera/_abcs_mixins/__init__.py,sha256=mi3doJZ9eTvu58z3T_Db6R9O_Mgc8g2aPCR9M4c1B9E,3117
-PSELPyBaseCamera/_abcs_mixins/_abcs_mixins.py,sha256=3RqshZZu3fLlzQEyfx69KIC9teckmKpqWaM0k-0563w,17740
+PSELPyBaseCamera/_abcs_mixins/__init__.py,sha256=kTm7EptL_4PD4zZ8RkTfREFcM9YnPCaRyUDGeDhQqGg,3411
+PSELPyBaseCamera/_abcs_mixins/_abcs_mixins.py,sha256=pYJ9R-SGaZ08r-Qxp3vYLW46KQ4i5UY2JkNJVGmbKOY,19371
 PSELPyBaseCamera/options/__init__.py,sha256=siKbNqFAFW29R8gQMztntFszkVchPCdsPxC2SMi56WQ,325
 PSELPyBaseCamera/options/errors.py,sha256=khnQAtlAwxDvje2EKhkHpFy0tB5zgRaLtvFnpXgcFn0,761
 PSELPyBaseCamera/options/results.py,sha256=IHb4xYC0YoCFttM5ecYOW9I7FdTeJa1CI7K4M09byTs,691
 PSELPyBaseCamera/options/types.py,sha256=iv8iur_3afnAYMuytXFBnNQa5_mnbhg2QDcmvz35sBo,184
-PSELPyBaseCamera-0.1.0.dist-info/LICENSE.txt,sha256=ff2WH3Rd8FJp2TQwDEeM1WtO6MWV9c85Q-9jRGkmOMM,1115
-PSELPyBaseCamera-0.1.0.dist-info/METADATA,sha256=bEo15kmLMVIgGMtyW4eGMzOgcId1x7qhyvEOiLYgJ7Q,1584
-PSELPyBaseCamera-0.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-PSELPyBaseCamera-0.1.0.dist-info/top_level.txt,sha256=FaCI7WxJSGX2_qpy9V1LRfJTVzlt2W-sbpSWyl8kheE,17
-PSELPyBaseCamera-0.1.0.dist-info/RECORD,,
+PSELPyBaseCamera-0.2.0.dist-info/LICENSE.txt,sha256=ff2WH3Rd8FJp2TQwDEeM1WtO6MWV9c85Q-9jRGkmOMM,1115
+PSELPyBaseCamera-0.2.0.dist-info/METADATA,sha256=g2NSeS9YwcRke5_O2KdotMZJ3Uz3Hz_a3C3gC8IUlQw,1584
+PSELPyBaseCamera-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+PSELPyBaseCamera-0.2.0.dist-info/top_level.txt,sha256=FaCI7WxJSGX2_qpy9V1LRfJTVzlt2W-sbpSWyl8kheE,17
+PSELPyBaseCamera-0.2.0.dist-info/RECORD,,
```

