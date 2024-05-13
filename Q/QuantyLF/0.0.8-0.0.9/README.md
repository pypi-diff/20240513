# Comparing `tmp/quantylf-0.0.8.tar.gz` & `tmp/quantylf-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantylf-0.0.8.tar", last modified: Tue May  7 18:02:27 2024, max compression
+gzip compressed data, was "quantylf-0.0.9.tar", last modified: Tue May  7 19:26:01 2024, max compression
```

## Comparing `quantylf-0.0.8.tar` & `quantylf-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:02:27.754917 quantylf-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-07 18:02:23.000000 quantylf-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-07 18:02:23.000000 quantylf-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-07 18:02:27.754917 quantylf-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-07 18:02:23.000000 quantylf-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-07 18:02:23.000000 quantylf-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-07 18:02:27.754917 quantylf-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:02:27.750917 quantylf-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:02:27.750917 quantylf-0.0.8/src/QuantyLF/
--rw-r--r--   0 runner    (1001) docker     (127)    18703 2024-05-07 18:02:23.000000 quantylf-0.0.8/src/QuantyLF/QuantyLF.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:02:23.000000 quantylf-0.0.8/src/QuantyLF/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:02:27.754917 quantylf-0.0.8/src/QuantyLF/cases/
--rw-r--r--   0 runner    (1001) docker     (127)    20402 2024-05-07 18:02:23.000000 quantylf-0.0.8/src/QuantyLF/cases/D3h_3d.lua
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-07 18:02:23.000000 quantylf-0.0.8/src/QuantyLF/cases/D3h_3d.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18754 2024-05-07 18:02:23.000000 quantylf-0.0.8/src/QuantyLF/cases/Oh_3d.lua
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-07 18:02:23.000000 quantylf-0.0.8/src/QuantyLF/cases/Oh_3d.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18821 2024-05-07 18:02:23.000000 quantylf-0.0.8/src/QuantyLF/cases/Td_3d.lua
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-07 18:02:23.000000 quantylf-0.0.8/src/QuantyLF/cases/Td_3d.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:02:27.754917 quantylf-0.0.8/src/QuantyLF/cases/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-07 18:02:23.000000 quantylf-0.0.8/src/QuantyLF/cases/utils/slater_integrals.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:02:27.754917 quantylf-0.0.8/src/QuantyLF.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-07 18:02:27.000000 quantylf-0.0.8/src/QuantyLF.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-07 18:02:27.000000 quantylf-0.0.8/src/QuantyLF.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 18:02:27.000000 quantylf-0.0.8/src/QuantyLF.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 18:02:27.000000 quantylf-0.0.8/src/QuantyLF.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 18:02:27.000000 quantylf-0.0.8/src/QuantyLF.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:26:01.980629 quantylf-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-07 19:25:57.000000 quantylf-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-07 19:25:57.000000 quantylf-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-07 19:26:01.980629 quantylf-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-07 19:25:57.000000 quantylf-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-07 19:25:57.000000 quantylf-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-07 19:26:01.984629 quantylf-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:26:01.976629 quantylf-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:26:01.980629 quantylf-0.0.9/src/QuantyLF/
+-rw-r--r--   0 runner    (1001) docker     (127)    18703 2024-05-07 19:25:57.000000 quantylf-0.0.9/src/QuantyLF/QuantyLF.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:25:57.000000 quantylf-0.0.9/src/QuantyLF/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:26:01.980629 quantylf-0.0.9/src/QuantyLF/cases/
+-rw-r--r--   0 runner    (1001) docker     (127)    20672 2024-05-07 19:25:57.000000 quantylf-0.0.9/src/QuantyLF/cases/D3h_3d.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-07 19:25:57.000000 quantylf-0.0.9/src/QuantyLF/cases/D3h_3d.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-05-07 19:25:57.000000 quantylf-0.0.9/src/QuantyLF/cases/Oh_3d.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-07 19:25:57.000000 quantylf-0.0.9/src/QuantyLF/cases/Oh_3d.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19083 2024-05-07 19:25:57.000000 quantylf-0.0.9/src/QuantyLF/cases/Td_3d.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-07 19:25:57.000000 quantylf-0.0.9/src/QuantyLF/cases/Td_3d.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:26:01.980629 quantylf-0.0.9/src/QuantyLF/cases/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-07 19:25:57.000000 quantylf-0.0.9/src/QuantyLF/cases/utils/slater_integrals.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:26:01.980629 quantylf-0.0.9/src/QuantyLF.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-07 19:26:01.000000 quantylf-0.0.9/src/QuantyLF.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-07 19:26:01.000000 quantylf-0.0.9/src/QuantyLF.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:26:01.000000 quantylf-0.0.9/src/QuantyLF.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 19:26:01.000000 quantylf-0.0.9/src/QuantyLF.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 19:26:01.000000 quantylf-0.0.9/src/QuantyLF.egg-info/top_level.txt
```

### Comparing `quantylf-0.0.8/LICENSE` & `quantylf-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `quantylf-0.0.8/PKG-INFO` & `quantylf-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantyLF
-Version: 0.0.8
+Version: 0.0.9
 Summary: QuantyLF is a libary to help manage Liegand Field simulations in Quanty.
 Home-page: https://github.com/CMM02/XPlotLib
 Author: Carl Magnus Meier
 Author-email: magnus.meier@outook.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quantylf-0.0.8/setup.cfg` & `quantylf-0.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = QuantyLF
-version = 0.0.8
+version = 0.0.9
 author = Carl Magnus Meier
 author_email = magnus.meier@outook.de
 description = QuantyLF is a libary to help manage Liegand Field simulations in Quanty.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CMM02/XPlotLib
 classifiers =
```

### Comparing `quantylf-0.0.8/src/QuantyLF/QuantyLF.py` & `quantylf-0.0.9/src/QuantyLF/QuantyLF.py`

 * *Files identical despite different names*

### Comparing `quantylf-0.0.8/src/QuantyLF/cases/D3h_3d.lua` & `quantylf-0.0.9/src/QuantyLF/cases/D3h_3d.lua`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 -- import slater integral values
-require "src.QuantyLF.cases.utils.slater_integrals"
+function addRelPath(dir)
+    local spath = debug.getinfo(1, 'S').source:sub(2):gsub("^([^/])", "./%1"):gsub("[^/]*$", "")
+    dir = dir and (dir .. "/") or ""
+    spath = spath .. dir
+    package.path = spath .. "?.lua;" .. spath .. "?/init.lua" .. package.path
+end
+
+addRelPath('utils')
+require "slater_integrals"
 
 TimeStart("LF_RIXS")
 -- this example calculates the resonant inelastic x-ray scattering in Transition Metal 3d we look at the
 -- L-L23M45 edge, i.e. we make an excitation from 2p to 3d (L23) and decay from the
 -- 3d shell back to the 2p shell (final "hole" in the 3d shell M45 edge). These spectra
 -- measure d-d excitations and or magnons.
```

### Comparing `quantylf-0.0.8/src/QuantyLF/cases/Oh_3d.lua` & `quantylf-0.0.9/src/QuantyLF/cases/Oh_3d.lua`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 -- import slater integral values
-require "src.QuantyLF.cases.utils.slater_integrals"
+function addRelPath(dir)
+    local spath = debug.getinfo(1, 'S').source:sub(2):gsub("^([^/])", "./%1"):gsub("[^/]*$", "")
+    dir = dir and (dir .. "/") or ""
+    spath = spath .. dir
+    package.path = spath .. "?.lua;" .. spath .. "?/init.lua" .. package.path
+end
+
+addRelPath('utils')
+require "slater_integrals"
 
 TimeStart("LF_RIXS")
 -- this example calculates the resonant inelastic x-ray scattering in Transition Metal 3d we look at the
 -- L-L23M45 edge, i.e. we make an excitation from 2p to 3d (L23) and decay from the
 -- 3d shell back to the 2p shell (final "hole" in the 3d shell M45 edge). These spectra
 -- measure d-d excitations and or magnons.
```

### Comparing `quantylf-0.0.8/src/QuantyLF/cases/Td_3d.lua` & `quantylf-0.0.9/src/QuantyLF/cases/Td_3d.lua`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 -- import slater integral values
-require "src.QuantyLF.cases.utils.slater_integrals"
+function addRelPath(dir)
+    local spath = debug.getinfo(1, 'S').source:sub(2):gsub("^([^/])", "./%1"):gsub("[^/]*$", "")
+    dir = dir and (dir .. "/") or ""
+    spath = spath .. dir
+    package.path = spath .. "?.lua;" .. spath .. "?/init.lua" .. package.path
+end
+
+addRelPath('utils')
+require "slater_integrals"
 
 TimeStart("LF_RIXS")
 -- this example calculates the resonant inelastic x-ray scattering in Transition Metal 3d we look at the
 -- L-L23M45 edge, i.e. we make an excitation from 2p to 3d (L23) and decay from the
 -- 3d shell back to the 2p shell (final "hole" in the 3d shell M45 edge). These spectra
 -- measure d-d excitations and or magnons.
```

### Comparing `quantylf-0.0.8/src/QuantyLF/cases/utils/slater_integrals.lua` & `quantylf-0.0.9/src/QuantyLF/cases/utils/slater_integrals.lua`

 * *Files identical despite different names*

### Comparing `quantylf-0.0.8/src/QuantyLF.egg-info/PKG-INFO` & `quantylf-0.0.9/src/QuantyLF.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantyLF
-Version: 0.0.8
+Version: 0.0.9
 Summary: QuantyLF is a libary to help manage Liegand Field simulations in Quanty.
 Home-page: https://github.com/CMM02/XPlotLib
 Author: Carl Magnus Meier
 Author-email: magnus.meier@outook.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

