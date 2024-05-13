# Comparing `tmp/aotpy-1.0.0.tar.gz` & `tmp/aotpy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aotpy-1.0.0.tar", last modified: Tue Aug  1 16:38:04 2023, max compression
+gzip compressed data, was "aotpy-2.0.0.tar", last modified: Mon May 13 15:41:27 2024, max compression
```

## Comparing `aotpy-1.0.0.tar` & `aotpy-2.0.0.tar`

### file list

```diff
@@ -1,56 +1,58 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 16:38:04.935191 aotpy-1.0.0/
--rw-rw-rw-   0        0        0     1592 2022-07-17 01:57:35.000000 aotpy-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3108 2023-08-01 16:38:04.935191 aotpy-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2309 2023-07-26 16:33:12.000000 aotpy-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 16:38:04.845614 aotpy-1.0.0/aotpy/
--rw-rw-rw-   0        0        0      521 2023-05-03 10:25:00.000000 aotpy-1.0.0/aotpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 16:38:04.886179 aotpy-1.0.0/aotpy/core/
--rw-rw-rw-   0        0        0      555 2023-05-08 11:52:45.000000 aotpy-1.0.0/aotpy/core/__init__.py
--rw-rw-rw-   0        0        0     1073 2023-05-02 09:36:00.000000 aotpy-1.0.0/aotpy/core/aberration.py
--rw-rw-rw-   0        0        0     5304 2023-07-17 15:33:42.000000 aotpy-1.0.0/aotpy/core/ao_system.py
--rw-rw-rw-   0        0        0     3050 2023-07-17 15:15:05.000000 aotpy-1.0.0/aotpy/core/atmosphere.py
--rw-rw-rw-   0        0        0     1162 2023-08-01 14:14:59.000000 aotpy-1.0.0/aotpy/core/base.py
--rw-rw-rw-   0        0        0     1338 2023-07-31 08:42:20.000000 aotpy-1.0.0/aotpy/core/image.py
--rw-rw-rw-   0        0        0     5293 2023-07-17 15:13:26.000000 aotpy-1.0.0/aotpy/core/loop.py
--rw-rw-rw-   0        0        0    11452 2023-05-08 11:39:26.000000 aotpy-1.0.0/aotpy/core/optical_sensor.py
--rw-rw-rw-   0        0        0     2863 2023-05-22 10:44:57.000000 aotpy-1.0.0/aotpy/core/source.py
--rw-rw-rw-   0        0        0     4887 2023-06-19 16:50:55.000000 aotpy-1.0.0/aotpy/core/telescope.py
--rw-rw-rw-   0        0        0      706 2023-06-19 16:50:55.000000 aotpy-1.0.0/aotpy/core/time.py
--rw-rw-rw-   0        0        0     3552 2023-07-17 10:39:59.000000 aotpy-1.0.0/aotpy/core/wavefront_corrector.py
-drwxrwxrwx   0        0        0        0 2023-08-01 16:38:04.889161 aotpy-1.0.0/aotpy/data/
-drwxrwxrwx   0        0        0        0 2023-08-01 16:38:04.891156 aotpy-1.0.0/aotpy/data/ERIS/
--rw-rw-rw-   0        0        0    11520 2023-04-03 16:42:38.000000 aotpy-1.0.0/aotpy/data/ERIS/ho_subap.fits
--rw-rw-rw-   0        0        0     5760 2023-06-19 12:38:42.000000 aotpy-1.0.0/aotpy/data/ERIS/lo_subap.fits
-drwxrwxrwx   0        0        0        0 2023-08-01 16:38:04.894158 aotpy-1.0.0/aotpy/data/GALACSI/
--rw-rw-rw-   0        0        0    11520 2023-04-03 16:42:38.000000 aotpy-1.0.0/aotpy/data/GALACSI/subap.fits
-drwxrwxrwx   0        0        0        0 2023-08-01 16:38:04.895157 aotpy-1.0.0/aotpy/data/NAOMI/
--rw-rw-rw-   0        0        0  7344000 2023-05-03 14:12:48.000000 aotpy-1.0.0/aotpy/data/NAOMI/zernike_control_modes.fits
-drwxrwxrwx   0        0        0        0 2023-08-01 16:38:04.908618 aotpy-1.0.0/aotpy/data/PAPYRUS/
--rw-rw-rw-   0        0        0  1013760 2023-06-19 15:05:10.000000 aotpy-1.0.0/aotpy/data/PAPYRUS/T152_pupil.fits
--rw-rw-rw-   0        0        0      105 2023-05-02 18:50:46.000000 aotpy-1.0.0/aotpy/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 16:38:04.912624 aotpy-1.0.0/aotpy/io/
--rw-rw-rw-   0        0        0      436 2023-06-19 16:50:12.000000 aotpy-1.0.0/aotpy/io/__init__.py
--rw-rw-rw-   0        0        0     2789 2023-06-19 16:50:12.000000 aotpy-1.0.0/aotpy/io/base.py
-drwxrwxrwx   0        0        0        0 2023-08-01 16:38:04.918642 aotpy-1.0.0/aotpy/io/fits/
--rw-rw-rw-   0        0        0      200 2023-05-02 13:23:11.000000 aotpy-1.0.0/aotpy/io/fits/__init__.py
--rw-rw-rw-   0        0        0    26722 2023-07-25 11:24:17.000000 aotpy-1.0.0/aotpy/io/fits/_keywords.py
--rw-rw-rw-   0        0        0    40530 2023-07-28 15:36:51.000000 aotpy-1.0.0/aotpy/io/fits/reader.py
--rw-rw-rw-   0        0        0     9760 2023-08-01 15:07:29.000000 aotpy-1.0.0/aotpy/io/fits/utils.py
--rw-rw-rw-   0        0        0    31140 2023-08-01 14:05:38.000000 aotpy-1.0.0/aotpy/io/fits/writer.py
-drwxrwxrwx   0        0        0        0 2023-08-01 16:38:04.930647 aotpy-1.0.0/aotpy/translators/
--rw-rw-rw-   0        0        0      440 2023-06-28 16:02:08.000000 aotpy-1.0.0/aotpy/translators/__init__.py
--rw-rw-rw-   0        0        0      981 2023-06-19 16:46:11.000000 aotpy-1.0.0/aotpy/translators/base.py
--rw-rw-rw-   0        0        0     7166 2023-07-25 17:10:27.000000 aotpy-1.0.0/aotpy/translators/ciao.py
--rw-rw-rw-   0        0        0    18590 2023-08-01 16:25:41.000000 aotpy-1.0.0/aotpy/translators/eris.py
--rw-rw-rw-   0        0        0    11377 2023-08-01 15:46:15.000000 aotpy-1.0.0/aotpy/translators/eso.py
--rw-rw-rw-   0        0        0    11574 2023-08-01 16:28:10.000000 aotpy-1.0.0/aotpy/translators/galacsi.py
--rw-rw-rw-   0        0        0     7616 2023-08-01 15:46:15.000000 aotpy-1.0.0/aotpy/translators/naomi.py
--rw-rw-rw-   0        0        0    12598 2023-08-01 16:31:56.000000 aotpy-1.0.0/aotpy/translators/papyrus.py
-drwxrwxrwx   0        0        0        0 2023-08-01 16:38:04.860354 aotpy-1.0.0/aotpy.egg-info/
--rw-rw-rw-   0        0        0     3108 2023-08-01 16:38:04.000000 aotpy-1.0.0/aotpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1058 2023-08-01 16:38:04.000000 aotpy-1.0.0/aotpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 16:38:04.000000 aotpy-1.0.0/aotpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      138 2023-08-01 16:38:04.000000 aotpy-1.0.0/aotpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-08-01 16:38:04.000000 aotpy-1.0.0/aotpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-11-05 13:42:41.000000 aotpy-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0     1029 2023-08-01 16:38:04.938203 aotpy-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 15:41:27.939886 aotpy-2.0.0/
+-rw-rw-rw-   0        0        0     1563 2024-05-13 10:57:01.000000 aotpy-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     7372 2024-05-13 15:41:27.937883 aotpy-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4106 2024-05-13 14:31:30.000000 aotpy-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 15:41:27.867266 aotpy-2.0.0/aotpy/
+-rw-rw-rw-   0        0        0      521 2024-04-30 10:49:48.000000 aotpy-2.0.0/aotpy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:41:27.893607 aotpy-2.0.0/aotpy/core/
+-rw-rw-rw-   0        0        0      555 2023-05-08 11:52:45.000000 aotpy-2.0.0/aotpy/core/__init__.py
+-rw-rw-rw-   0        0        0     1073 2023-05-02 09:36:00.000000 aotpy-2.0.0/aotpy/core/aberration.py
+-rw-rw-rw-   0        0        0     6896 2024-05-13 12:20:49.000000 aotpy-2.0.0/aotpy/core/ao_system.py
+-rw-rw-rw-   0        0        0     3061 2024-02-28 19:38:37.000000 aotpy-2.0.0/aotpy/core/atmosphere.py
+-rw-rw-rw-   0        0        0     1331 2024-02-28 18:31:48.000000 aotpy-2.0.0/aotpy/core/base.py
+-rw-rw-rw-   0        0        0     1338 2024-05-13 09:19:17.000000 aotpy-2.0.0/aotpy/core/image.py
+-rw-rw-rw-   0        0        0     5291 2024-05-08 17:35:27.000000 aotpy-2.0.0/aotpy/core/loop.py
+-rw-rw-rw-   0        0        0    12181 2024-05-13 09:27:11.000000 aotpy-2.0.0/aotpy/core/optical_sensor.py
+-rw-rw-rw-   0        0        0     2912 2024-05-13 09:29:32.000000 aotpy-2.0.0/aotpy/core/source.py
+-rw-rw-rw-   0        0        0     4887 2023-06-19 16:50:55.000000 aotpy-2.0.0/aotpy/core/telescope.py
+-rw-rw-rw-   0        0        0      706 2023-06-19 16:50:55.000000 aotpy-2.0.0/aotpy/core/time.py
+-rw-rw-rw-   0        0        0     3552 2023-07-17 10:39:59.000000 aotpy-2.0.0/aotpy/core/wavefront_corrector.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:41:27.894607 aotpy-2.0.0/aotpy/data/
+drwxrwxrwx   0        0        0        0 2024-05-13 15:41:27.896609 aotpy-2.0.0/aotpy/data/ERIS/
+-rw-rw-rw-   0        0        0    11520 2023-04-03 16:42:38.000000 aotpy-2.0.0/aotpy/data/ERIS/ho_subap.fits
+-rw-rw-rw-   0        0        0     5760 2023-06-19 12:38:42.000000 aotpy-2.0.0/aotpy/data/ERIS/lo_subap.fits
+drwxrwxrwx   0        0        0        0 2024-05-13 15:41:27.898609 aotpy-2.0.0/aotpy/data/GALACSI/
+-rw-rw-rw-   0        0        0    11520 2023-04-03 16:42:38.000000 aotpy-2.0.0/aotpy/data/GALACSI/subap.fits
+drwxrwxrwx   0        0        0        0 2024-05-13 15:41:27.899610 aotpy-2.0.0/aotpy/data/NAOMI/
+-rw-rw-rw-   0        0        0  7344000 2023-05-03 14:12:48.000000 aotpy-2.0.0/aotpy/data/NAOMI/zernike_control_modes.fits
+drwxrwxrwx   0        0        0        0 2024-05-13 15:41:27.907413 aotpy-2.0.0/aotpy/data/PAPYRUS/
+-rw-rw-rw-   0        0        0  1013760 2023-06-19 15:05:10.000000 aotpy-2.0.0/aotpy/data/PAPYRUS/T152_pupil.fits
+-rw-rw-rw-   0        0        0      105 2023-05-02 18:50:46.000000 aotpy-2.0.0/aotpy/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:41:27.907413 aotpy-2.0.0/aotpy/io/
+-rw-rw-rw-   0        0        0      511 2024-04-30 11:06:29.000000 aotpy-2.0.0/aotpy/io/__init__.py
+-rw-rw-rw-   0        0        0     1544 2024-04-29 16:39:22.000000 aotpy-2.0.0/aotpy/io/base.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:41:27.920940 aotpy-2.0.0/aotpy/io/fits/
+-rw-rw-rw-   0        0        0      293 2024-04-30 11:06:54.000000 aotpy-2.0.0/aotpy/io/fits/__init__.py
+-rw-rw-rw-   0        0        0    76805 2024-05-13 14:47:57.000000 aotpy-2.0.0/aotpy/io/fits/_file.py
+-rw-rw-rw-   0        0        0     9603 2024-05-07 09:26:42.000000 aotpy-2.0.0/aotpy/io/fits/_strings.py
+-rw-rw-rw-   0        0        0     1028 2024-05-07 09:53:29.000000 aotpy-2.0.0/aotpy/io/fits/compat.py
+-rw-rw-rw-   0        0        0    19460 2024-05-13 09:51:15.000000 aotpy-2.0.0/aotpy/io/fits/reader.py
+-rw-rw-rw-   0        0        0     9945 2024-05-13 10:01:57.000000 aotpy-2.0.0/aotpy/io/fits/utils.py
+-rw-rw-rw-   0        0        0    23015 2024-05-13 12:59:46.000000 aotpy-2.0.0/aotpy/io/fits/writer.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:41:27.927469 aotpy-2.0.0/aotpy/translators/
+-rw-rw-rw-   0        0        0      440 2024-04-30 11:08:00.000000 aotpy-2.0.0/aotpy/translators/__init__.py
+-rw-rw-rw-   0        0        0      981 2023-06-19 16:46:11.000000 aotpy-2.0.0/aotpy/translators/base.py
+-rw-rw-rw-   0        0        0     7195 2024-02-28 19:38:37.000000 aotpy-2.0.0/aotpy/translators/ciao.py
+-rw-rw-rw-   0        0        0    18595 2024-04-30 11:05:28.000000 aotpy-2.0.0/aotpy/translators/eris.py
+-rw-rw-rw-   0        0        0    11420 2024-04-30 10:52:42.000000 aotpy-2.0.0/aotpy/translators/eso.py
+-rw-rw-rw-   0        0        0    11579 2024-04-30 11:05:28.000000 aotpy-2.0.0/aotpy/translators/galacsi.py
+-rw-rw-rw-   0        0        0     7618 2024-02-28 19:38:37.000000 aotpy-2.0.0/aotpy/translators/naomi.py
+-rw-rw-rw-   0        0        0    12608 2024-04-30 11:04:34.000000 aotpy-2.0.0/aotpy/translators/papyrus.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:41:27.935884 aotpy-2.0.0/aotpy.egg-info/
+-rw-rw-rw-   0        0        0     7372 2024-05-13 15:41:27.000000 aotpy-2.0.0/aotpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1094 2024-05-13 15:41:27.000000 aotpy-2.0.0/aotpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 15:41:27.000000 aotpy-2.0.0/aotpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      138 2024-05-13 15:41:27.000000 aotpy-2.0.0/aotpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-13 15:41:27.000000 aotpy-2.0.0/aotpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1437 2024-05-13 12:21:25.000000 aotpy-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 15:41:27.939886 aotpy-2.0.0/setup.cfg
```

### Comparing `aotpy-1.0.0/LICENSE` & `aotpy-2.0.0/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-BSD 3-Clause License
-
-Copyright (c) 2022, Faculdade de Engenharia da Universidade do Porto (FEUP)
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2022, Faculdade de Engenharia da Universidade do Porto (FEUP)
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `aotpy-1.0.0/aotpy/__init__.py` & `aotpy-2.0.0/aotpy/__init__.py`

 * *Files identical despite different names*

### Comparing `aotpy-1.0.0/aotpy/core/__init__.py` & `aotpy-2.0.0/aotpy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `aotpy-1.0.0/aotpy/core/aberration.py` & `aotpy-2.0.0/aotpy/core/aberration.py`

 * *Files identical despite different names*

### Comparing `aotpy-1.0.0/aotpy/core/atmosphere.py` & `aotpy-2.0.0/aotpy/core/atmosphere.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,24 +19,24 @@
     'Reference wavelength. (in m units)'
 
     time: Time = None
 
     r0: list[float] = field(default_factory=list)
     'List of Fried parameters at reference wavelength at zenith, over time. (in m units)'
 
-    fwhm: list[float] = field(default_factory=list)
+    seeing: list[float] = field(default_factory=list)
     'List of full width at half maximum measures of the seeing disc at zenith, over time. (in arcsec units)'
 
     tau0: list[float] = field(default_factory=list)
     'List of atmospheric coherence times, over time. (in s units)'
 
     theta0: list[float] = field(default_factory=list)
     'List of isoplanatic angles, over time. (in rad units)'
 
-    layers_weight: Image = None
+    layers_relative_weight: Image = None
     """Fractional weight of each :math:`l` turbulence layer (sums to 1), for each time instant.
     (Dimensions :math:`t \\times l`, dimensionless quantity, using data type flt)"""
 
     layers_height: Image = None
     """Height above observatory at zenith of each :math:`l` turbulence layer, for each time instant.
     (Dimensions :math:`t \\times l`, in m units, using data type flt)"""
```

### Comparing `aotpy-1.0.0/aotpy/core/image.py` & `aotpy-2.0.0/aotpy/core/image.py`

 * *Files identical despite different names*

### Comparing `aotpy-1.0.0/aotpy/core/loop.py` & `aotpy-2.0.0/aotpy/core/loop.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
     time: Time = None
 
     closed: bool = True
     "Indicates whether the loop was opened or closed for the duration of the data collection."
 
     commands: Image = None
-
     """Sequence of commands sent to the associated wavefront corrector. Each of the :math:`t` frames contains the values
     sent to each of the :math:`a_v` valid actuators of a certain wavefront corrector.
     (Dimensions :math:`t \\times a_v`, in m units, using data type flt)"""
 
     ref_commands: Image = None
     """Reference offset commands for each of :math:`a_v` actuators.
     (Dimensions :math:`a_v`, in m units, using data type flt)"""
```

### Comparing `aotpy-1.0.0/aotpy/core/optical_sensor.py` & `aotpy-2.0.0/aotpy/core/optical_sensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,56 +37,62 @@
     r'Readout noise. (in e\ :math:`^-` s\ :math:`^{-1}` pix\ :math:`^{-1}` units)'
 
     pixel_intensities: Image = None
     """Intensity detected in each pixel, for each data frame. This is a sequence of :math:`t` images, each spanning 
     :math:`x` pixels horizontally and :math:`y` pixels vertically.
     (Dimensions :math:`t \\times h \\times w`, in ADU units, using data type flt)"""
 
+    field_centre: Coordinates = field(default_factory=Coordinates)
+    """Defines the horizontal/vertical coordinates of the detector pixel on which the centre of the field is projected. 
+    Fractional `Coordinates` values imply that the centre is located in-between two pixels. (in pix units)"""
+
     integration_time: float = None
-    'TODO: Integration time. (in s units)'
+    'Duration in seconds a pixel integrates flux, independent of the detector reading scheme. (in s units)'
 
     coadds: int = None
     'Number of frame co-additions.  (in count units)'
 
     dark: Image = None
     """Intensity detected in each pixel when there is no light being observed. This is an image spanning 
     :math:`x` pixels horizontally and :math:`y` pixels vertically.
     (Dimensions :math:`h \\times w`, in ADU units, using data type flt)"""
 
     weight_map: Image = None
     """Pixel weight map, where each detector pixel is associated with a number that represents its relative value.
     Summing up to 1. (Dimensions :math:`h \\times w`, dimensionless quantity, using data type flt)"""
 
     quantum_efficiency: float = None
-    'TODO: Quantum efficiency. (dimensionless quantity)'
+    """A 0–1 scalar indicating the ability to convert a photon into a usable electron. Quoted at the central wavelength 
+    as an effective value (dimensionless quantity)"""
 
     pixel_scale: float = None
-    r'TODO: Pixel scale. (in rad pix\ :math:`^{-1}` units)'
+    r'Resolution in radians per detector pixel. (in rad pix\ :math:`^{-1}` units)'
 
     binning: int = None
-    'TODO: Binning. (in count units)'
+    'Integer value indicating the 2D pixel combination by the binning factor. (in count units)'
 
     bandwidth: float = None
-    'TODO: Spectral bandwidth. (in m units)'
+    'Width of the filter/bandpass of the optics+detector. (in m units)'
 
     transmission_wavelength: list[float] = field(default_factory=list)
     'List of wavelengths that describe a transmission profile. (in m units)'
 
     transmission: list[float] = field(default_factory=list)
     'List of transmission percentages that describe a transmission profile. (dimensionless quantity)'
 
     sky_background: Image = None
     """detector pixel intensities from a source-less direction in the sky
     (Dimensions :math:`h \\times w`, in ADU units, using data type flt)"""
 
     gain: float = None
-    r'TODO: Gain. (in e\ :math:`^-` units)'
+    r'Scalar magnitude of detector signal amplification. (in e\ :math:`^-` units)'
 
     excess_noise: float = None
-    r'TODO: Excess noise. (in e\ :math:`^-` units)'
+    r"""Photon-noise gain factor (scalar) as a result of the electron-multiplied gain amplification in EMCCDs. 
+    (in e\ :math:`^-` units)"""
 
     filter: str = None
     'Name of filter in use. (dimensionless quantity)'
 
     bad_pixel_map: Image = None
     """Binary image which identifies the bad pixels. Pixels identified with 1 are considered bad, while 0 is considered
     normal.  (Dimensions :math:`h \\times w`, dimensionless quantity, using data type int)"""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aotpy-1.0.0/aotpy/core/source.py` & `aotpy-2.0.0/aotpy/core/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     elevation_offset: float = None
     "Offset from the Main Telescope's `elevation`. (in deg units)"
 
     azimuth_offset: float = None
     "Offset from the Main Telescope's `azimuth`. (in deg units)"
 
-    width: float = None
+    fwhm: float = None
     'Effective width at zenith. (in rad units)'
 
     def __post_init__(self):
         if self.__class__ == Source:
             raise TypeError("Cannot instantiate abstract class.")
 
 
@@ -78,8 +78,8 @@
 class RayleighLaserGuideStar(LaserGuideStar):
     """Contains data regarding a Rayleigh laser guide star being observed by the system."""
 
     distance: float = None
     'Fixed distance of the LGS from the telescope. (in m units)'
 
     depth: float = None
-    'TODO: Depth (in m units)'
+    'Range covered by the laser light while the shutter is opened. (in m units)'
```

### Comparing `aotpy-1.0.0/aotpy/core/telescope.py` & `aotpy-2.0.0/aotpy/core/telescope.py`

 * *Files identical despite different names*

### Comparing `aotpy-1.0.0/aotpy/core/time.py` & `aotpy-2.0.0/aotpy/core/time.py`

 * *Files identical despite different names*

### Comparing `aotpy-1.0.0/aotpy/core/wavefront_corrector.py` & `aotpy-2.0.0/aotpy/core/wavefront_corrector.py`

 * *Files identical despite different names*

### Comparing `aotpy-1.0.0/aotpy/data/ERIS/ho_subap.fits` & `aotpy-2.0.0/aotpy/data/ERIS/ho_subap.fits`

 * *Files identical despite different names*

### Comparing `aotpy-1.0.0/aotpy/data/ERIS/lo_subap.fits` & `aotpy-2.0.0/aotpy/data/ERIS/lo_subap.fits`

 * *Files identical despite different names*

### Comparing `aotpy-1.0.0/aotpy/data/GALACSI/subap.fits` & `aotpy-2.0.0/aotpy/data/GALACSI/subap.fits`

 * *Files identical despite different names*

### Comparing `aotpy-1.0.0/aotpy/data/NAOMI/zernike_control_modes.fits` & `aotpy-2.0.0/aotpy/data/NAOMI/zernike_control_modes.fits`

 * *Files identical despite different names*

### Comparing `aotpy-1.0.0/aotpy/data/PAPYRUS/T152_pupil.fits` & `aotpy-2.0.0/aotpy/data/PAPYRUS/T152_pupil.fits`

 * *Files identical despite different names*

### Comparing `aotpy-1.0.0/aotpy/io/fits/utils.py` & `aotpy-2.0.0/aotpy/io/fits/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,27 +6,25 @@
 import os
 import re
 
 import numpy as np
 from astropy.io import fits
 
 import aotpy
-from . import _keywords as kw
+from ._strings import IMAGE_UNIT, TIME_REFERENCE
 
-__all__ = ['FITSFileImage', 'FITSURLImage', 'image_from_fits_file', 'image_from_hdus', 'image_from_hdu',
-           'card_from_metadatum', 'metadatum_from_card', 'metadata_from_hdu', 'datetime_to_iso', 'keyword_is_relevant']
+_valid_filename = re.compile(r'[a-zA-Z0-9_\-.]+')
+_standard_patterns = re.compile(r'NAXIS\d*')
+_standard_keywords = {'SIMPLE', 'EXTEND', 'BSCALE', 'BZERO', 'XTENSION', 'BITPIX',
+                      'PCOUNT', 'GCOUNT', 'EXTNAME', 'CHECKSUM', 'DATASUM'}
 
 
-def keyword_is_relevant(keyword):
+def _keyword_is_relevant(keyword):
     """Check if keyword is relevant. Keywords are considered "irrelevant" if they are already reflected elsewhere in the
      object produced by Astropy."""
-    _standard_keywords = {'SIMPLE', 'EXTEND', 'BSCALE', 'BZERO', 'XTENSION', 'BITPIX',
-                          'PCOUNT', 'GCOUNT', 'EXTNAME', 'CHECKSUM', 'DATASUM'}
-    _standard_patterns = re.compile(r'NAXIS\d*')
-
     return keyword not in _standard_keywords and not _standard_patterns.fullmatch(keyword)
 
 
 class _FITSExternalImage(aotpy.Image):
     """Describes an external FITS file containing multidimensional data and metadata related to it."""
 
     def to_internal(self) -> aotpy.Image:
@@ -51,18 +49,20 @@
         Path to FITS file that contains multidimensional data.
     index: int, optional
         Index of the HDU that contains the image data. If omitted, the first HDU containing image data is assumed.
     **kwargs
         Keyword arguments passed on as options to the file handling function.
     """
 
-    def __init__(self, path: str | os.PathLike, index: int = None, **kwargs):
+    def __init__(self, path: str | os.PathLike, index: int = None, *, read_data=True, **kwargs):
         self.filename = os.path.basename(path)
         self.index = index
-        self.name, self.data, self.unit, self._time, self.metadata = _get_image_fields_from_file(path, index, **kwargs)
+        if read_data:
+            self.name, self.data, self.unit, self._time_ref, self.metadata = _get_image_fields_from_file(path, index,
+                                                                                                         **kwargs)
 
     def __eq__(self, other):
         return self.filename == other.filename and self.index == other.index and self.time == other.time
 
 
 class FITSURLImage(_FITSExternalImage):
     """Describes an external FITS file available via URL, containing multidimensional data and metadata related to it.
@@ -75,18 +75,20 @@
         URL to FITS file that contains multidimensional data.
     index: int, optional
         Index of the HDU that contains the image data. If omitted, the first HDU containing image data is assumed.
     **kwargs
         Keyword arguments passed on as options to the file handling function.
     """
 
-    def __init__(self, url: str, index: int = None, **kwargs):
+    def __init__(self, url: str, index: int = None, *, read_data=True, **kwargs):
         self.url = url
         self.index = index
-        self.name, self.data, self.unit, self._time, self.metadata = _get_image_fields_from_file(url, index, **kwargs)
+        if read_data:
+            self.name, self.data, self.unit, self._time_ref, self.metadata = _get_image_fields_from_file(url, index,
+                                                                                                         **kwargs)
 
     def __eq__(self, other):
         return self.url == other.url and self.index == other.index and self.time == other.time
 
 
 def image_from_fits_file(path: str | os.PathLike, index: int = None, *, name: str = None, **kwargs) -> aotpy.Image:
     """
@@ -99,19 +101,19 @@
     index: int, optional
         Index of the HDU that contains the image data. If omitted, the first HDU containing image data is assumed.
     name: str, optional
         Name of the Image. If None, the name is the same as in the file.
     **kwargs
         Keyword arguments passed on as options to the file handling function.
     """
-    _name, data, unit, _time, metadata = _get_image_fields_from_file(path, index, **kwargs)
+    _name, data, unit, _time_ref, metadata = _get_image_fields_from_file(path, index, **kwargs)
     if name is None:
         name = _name
     image = aotpy.Image(name=name, data=data, unit=unit, metadata=metadata)
-    image._time = _time
+    image._time_ref = _time_ref
     return image
 
 
 def image_from_hdus(hdus: fits.HDUList, index: int = None, *, name: str = None) -> aotpy.Image:
     """
     Get `Image` from specified path or URL.
 
@@ -120,38 +122,38 @@
     hdus
         List of HDUs from which `Image` is to be extracted.
     index: int, optional
         Index of the HDU that contains the image data. If omitted, the first HDU containing image data is assumed.
     name: str, optional
         Name of the Image. If None, the name is the same as in the HDU.
     """
-    _name, data, unit, _time, metadata = _get_image_fields_from_hdus(hdus, index)
+    _name, data, unit, _time_ref, metadata = _get_image_fields_from_hdus(hdus, index)
     if name is None:
         name = _name
     image = aotpy.Image(name=name, data=data, unit=unit, metadata=metadata)
-    image._time = _time
+    image._time_ref = _time_ref
     return image
 
 
 def image_from_hdu(hdu: fits.ImageHDU, *, name: str = None) -> aotpy.Image:
     """
     Get `Image` from specified HDU.
 
     Parameters
     ----------
     hdu
         HDU from which `Image` is to be extracted.
     name: str, optional
         Name of the Image. If None, the name is the same as in the HDU.
     """
-    _name, data, unit, _time, metadata = _get_image_fields_from_hdu(hdu)
+    _name, data, unit, _time_ref, metadata = _get_image_fields_from_hdu(hdu)
     if name is None:
         name = _name
     image = aotpy.Image(name=name, data=data, unit=unit, metadata=metadata)
-    image._time = _time
+    image._time_ref = _time_ref
     return image
 
 
 def _get_image_fields_from_file(path: str | os.PathLike, index: int = None, **kwargs) -> \
         tuple[str, np.ndarray, str, str, list[aotpy.Metadatum]]:
     try:
         with fits.open(path, **kwargs) as hdus:
@@ -184,23 +186,23 @@
 
     return _get_image_fields_from_hdu(hdu)
 
 
 def _get_image_fields_from_hdu(hdu) -> tuple[str, np.ndarray, str, str, list[aotpy.Metadatum]]:
     metadata = metadata_from_hdu(hdu)
     unit = None
-    if (md := next((x for x in metadata if x.key == kw.IMAGE_UNIT), None)) is not None:
+    if (md := next((x for x in metadata if x.key == IMAGE_UNIT), None)) is not None:
         unit = md.value
         metadata.remove(md)
 
-    _time = None
-    if (md := next((x for x in metadata if x.key == kw.TIME_REFERENCE), None)) is not None:
-        _time = md.value
+    time_ref = None
+    if (md := next((x for x in metadata if x.key == TIME_REFERENCE), None)) is not None:
+        time_ref = md.value
         metadata.remove(md)
-    return hdu.name, hdu.data, unit, _time, metadata
+    return hdu.name, hdu.data, unit, time_ref, metadata
 
 
 def card_from_metadatum(md: aotpy.Metadatum) -> fits.Card:
     """
     Get `Card` from `Metadatum`.
 
     Parameters
@@ -232,28 +234,28 @@
     Parameters
     ----------
     hdu
         HDU from which to extract metadata.
     """
     # If the keywords are irrelevant they don't need to be part of the image metadata, as that information is already
     # implied in the numpy data.
-    return [metadatum_from_card(card) for card in hdu.header.cards if keyword_is_relevant(card.keyword)]
+    return [metadatum_from_card(card) for card in hdu.header.cards if _keyword_is_relevant(card.keyword)]
 
 
-def datetime_to_iso(d: datetime.datetime):
+def _datetime_to_iso(d: datetime.datetime):
     """
     Convert datetime to ISO format string. If timezone information is present, convert time to UTC and remove
     information.
 
     Parameters
     ----------
     d
         `datetime` to be converted to an ISO string.
     """
     if d is None:
-        return ''
+        return None
     if d.tzinfo is not None:
         # If datetime has timezone data, convert the datetime to UTC and then remove the timezone data.
         # This is done to ensure dt.isoformat() doesn't print UTC offsets.
         # If datetime doesn't have timezone data, we assume it is already in UTC.
         d = d.astimezone(datetime.timezone.utc).replace(tzinfo=None)
     return d.isoformat()
```

### Comparing `aotpy-1.0.0/aotpy/translators/base.py` & `aotpy-2.0.0/aotpy/translators/base.py`

 * *Files identical despite different names*

### Comparing `aotpy-1.0.0/aotpy/translators/ciao.py` & `aotpy-2.0.0/aotpy/translators/ciao.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             main_hdr = hdus[0].header
             main_loop_frame = hdus['LoopFrame'].data
 
         self.system = aotpy.AOSystem(
             ao_mode='SCAO',
             name='CIAO',
             strehl_ratio=main_hdr['ESO AOS ATM SR'],
-            temporal_error=main_hdr['ESO AOS ATM TERR']
+            metadata=[aotpy.Metadatum('TEMP-ERR', main_hdr['ESO AOS ATM TERR'])]
         )
         self.system.main_telescope = aotpy.MainTelescope(
             uid=f'ESO VLT AT{at_number}',
             elevation=main_hdr['ESO TEL ALT'],
             azimuth=self._azimuth_conversion(main_hdr['ESO TEL AZ']),
             parallactic=main_hdr['ESO TEL PRLTIC']
         )
@@ -127,24 +127,24 @@
             framerate=main_hdr['ESO AOS LOOP RATE'],
             closed=main_hdr['ESO AOS TT LOOP ST']
         )
 
         asm = aotpy.AtmosphericParameters(
             'ESO ASM (Astronomical Site Monitor)',
             wavelength=500e-9,
-            fwhm=[main_hdr['ESO TEL AMBI FWHM']],
+            seeing=[main_hdr['ESO TEL AMBI FWHM']],
             tau0=[main_hdr['ESO TEL AMBI TAU0']],
             theta0=[main_hdr['ESO TEL AMBI THETA0']],
             layers_wind_direction=aotpy.Image('ESO TEL AMBI WINDDIR', np.array([[main_hdr['ESO TEL AMBI WINDDIR']]])),
             layers_wind_speed=aotpy.Image('ESO TEL AMBI WINDSP', np.array([[main_hdr['ESO TEL AMBI WINDSP']]]))
         )
 
         aos = aotpy.AtmosphericParameters(
             'AO System',
-            fwhm=[main_hdr['ESO AOS ATM SEEING']],
+            seeing=[main_hdr['ESO AOS ATM SEEING']],
             tau0=[main_hdr['ESO AOS ATM TAU0']],
         )
 
         self.system.sources = [ngs]
         self.system.wavefront_sensors = [wfs]
         self.system.wavefront_correctors = [ho_dm, ittm]
         self.system.loops = [ho_loop, tt_loop]
```

### Comparing `aotpy-1.0.0/aotpy/translators/eris.py` & `aotpy-2.0.0/aotpy/translators/eris.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from datetime import datetime
 from pathlib import Path
 
 import numpy as np
 from astropy.io import fits
 
 import aotpy
-from aotpy.io import image_from_fits_file
+from aotpy.io.fits import image_from_fits_file
 from .eso import ESOTranslator
 
 
 # TODO set image units
 
 
 class ERISTranslator(ESOTranslator):
```

### Comparing `aotpy-1.0.0/aotpy/translators/eso.py` & `aotpy-2.0.0/aotpy/translators/eso.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 try:
     from pyvo.dal import tap
 except (ImportError, ModuleNotFoundError):
     tap = None
 
 import aotpy
+from aotpy.io.fits import image_from_fits_file
 from .base import BaseTranslator
 
 ESO_TAP_OBS = "https://archive.eso.org/tap_obs"
 
 
 class ESOTranslator(BaseTranslator):
     """Abstract class for translators for ESO systems.
@@ -207,15 +208,15 @@
 
         ESO's azimuth is measured westwards from the south, while in AOT it is defined as being measured from the
         eastward from the north.
 
         Parameters
         ----------
         az
-            ESO azimuth to be converted
+            ESO azimuth to be converted.
         """
         # We need to subtract the angle between north and south and then apply symmetry.
         return -(az - 180) % 360
 
     @staticmethod
     def _get_pixel_data_from_table(pix_frame: fits.FITS_rec) -> np.ndarray:
         """
@@ -255,11 +256,11 @@
         # Old ESO pointing data was stored using a pseudo-float format such that e.g. 100526.90157 -> +10h 05m 26.90157s
         # This function converts from this format into decimal degrees
         t = str(time)
         return int(t[:2]) + int(t[2:4]) / 60 + float(t[4:]) / 3600
 
     @staticmethod
     def _image_from_eso_file(filename: str | os.PathLike) -> aotpy.Image:
-        image = aotpy.image_from_fits_file(filename)
+        image = image_from_fits_file(filename)
         image.metadata = [md for md in image.metadata if not md.key.startswith("ESO DPR") and md.key != 'ORIGIN' and
                           md.key != 'RA' and md.key != 'DEC']
         return image
```

### Comparing `aotpy-1.0.0/aotpy/translators/galacsi.py` & `aotpy-2.0.0/aotpy/translators/galacsi.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from datetime import datetime
 from pathlib import Path
 
 import numpy as np
 from astropy.io import fits
 
 import aotpy
-from aotpy.io import image_from_fits_file
+from aotpy.io.fits import image_from_fits_file
 from .eso import ESOTranslator
 
 
 # TODO set image units
 
 
 class GALACSITranslator(ESOTranslator):
```

### Comparing `aotpy-1.0.0/aotpy/translators/naomi.py` & `aotpy-2.0.0/aotpy/translators/naomi.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             closed=main_hdr['ESO AOS LOOP ST'],
             framerate=main_hdr['ESO AOS LOOP RATE']
         )
 
         asm = aotpy.AtmosphericParameters(
             'ESO ASM (Astronomical Site Monitor)',
             wavelength=500e-9,
-            fwhm=[main_hdr['ESO TEL AMBI FWHM']],
+            seeing=[main_hdr['ESO TEL AMBI FWHM']],
             tau0=[main_hdr['ESO TEL AMBI TAU0']],
             theta0=[main_hdr['ESO TEL AMBI THETA0']],
             layers_wind_direction=aotpy.Image('ESO TEL AMBI WINDDIR', np.array([[main_hdr['ESO TEL AMBI WINDDIR']]])),
             layers_wind_speed=aotpy.Image('ESO TEL AMBI WINDSP', np.array([[main_hdr['ESO TEL AMBI WINDSP']]]))
         )
 
         self.system.sources = [ngs]
```

### Comparing `aotpy-1.0.0/aotpy/translators/papyrus.py` & `aotpy-2.0.0/aotpy/translators/papyrus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 This module contains a class for translating telemetry data produced by the ALPAO RTC, part of the PAPYRUS system. 
 It assumes the MATLAB files produced by ALPAO RTC have been converted to use struct objects instead of classes. 
 The custom MATLAB function makeTelemetryFileReadable is made for this.
-Note that the use of scipy.io.loadmat to read the .mat files in python suppose that these .mat files were 
-saved with the version -v7 of matlab or anterior. scipy.io.loadmat does not work for files saved with matlab -v7.3.
+Note that the usage of scipy.io.loadmat to read the .mat files in Python assumes that these files were saved with the
+version -v7 of matlab or previous. scipy.io.loadmat does not work for files saved with matlab -v7.3 or later.
 """
 
 import datetime
 import importlib.resources
 
 import numpy as np
 
 import aotpy
-from aotpy.io import image_from_fits_file
+from aotpy.io.fits import image_from_fits_file
 from .base import BaseTranslator
 
 try:
     from scipy.io import loadmat
 except (ImportError, ModuleNotFoundError):
     loadmat = None
```

### Comparing `aotpy-1.0.0/aotpy.egg-info/SOURCES.txt` & `aotpy-2.0.0/aotpy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
 aotpy/__init__.py
 aotpy.egg-info/PKG-INFO
 aotpy.egg-info/SOURCES.txt
 aotpy.egg-info/dependency_links.txt
 aotpy.egg-info/requires.txt
 aotpy.egg-info/top_level.txt
 aotpy/core/__init__.py
@@ -25,15 +24,17 @@
 aotpy/data/ERIS/lo_subap.fits
 aotpy/data/GALACSI/subap.fits
 aotpy/data/NAOMI/zernike_control_modes.fits
 aotpy/data/PAPYRUS/T152_pupil.fits
 aotpy/io/__init__.py
 aotpy/io/base.py
 aotpy/io/fits/__init__.py
-aotpy/io/fits/_keywords.py
+aotpy/io/fits/_file.py
+aotpy/io/fits/_strings.py
+aotpy/io/fits/compat.py
 aotpy/io/fits/reader.py
 aotpy/io/fits/utils.py
 aotpy/io/fits/writer.py
 aotpy/translators/__init__.py
 aotpy/translators/base.py
 aotpy/translators/ciao.py
 aotpy/translators/eris.py
```

