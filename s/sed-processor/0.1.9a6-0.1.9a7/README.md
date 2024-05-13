# Comparing `tmp/sed_processor-0.1.9a6.tar.gz` & `tmp/sed_processor-0.1.9a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sed_processor-0.1.9a6.tar", max compression
+gzip compressed data, was "sed_processor-0.1.9a7.tar", max compression
```

## Comparing `sed_processor-0.1.9a6.tar` & `sed_processor-0.1.9a7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1072 2024-04-04 07:13:45.495365 sed_processor-0.1.9a6/LICENSE
--rw-r--r--   0        0        0     2881 2024-04-04 07:13:45.495365 sed_processor-0.1.9a6/README.md
--rw-r--r--   0        0        0     2840 2024-04-04 07:14:27.231338 sed_processor-0.1.9a6/pyproject.toml
--rw-r--r--   0        0        0      127 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/__init__.py
--rw-r--r--   0        0        0      160 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/binning/__init__.py
--rw-r--r--   0        0        0    21273 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/binning/binning.py
--rw-r--r--   0        0        0     8570 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/binning/numba_bin.py
--rw-r--r--   0        0        0     6073 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/binning/utils.py
--rw-r--r--   0        0        0      231 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/calibrator/__init__.py
--rw-r--r--   0        0        0    17235 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/calibrator/delay.py
--rw-r--r--   0        0        0    88866 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/calibrator/energy.py
--rw-r--r--   0        0        0    83020 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/calibrator/momentum.py
--rwxr-xr-x   0        0        0    17175 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/config/NXmpes_config.json
--rw-r--r--   0        0        0     4692 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/config/default.yaml
--rw-r--r--   0        0        0     6359 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/config/flash_example_config.yaml
--rw-r--r--   0        0        0    11357 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/config/mpes_example_config.yaml
--rw-r--r--   0        0        0      105 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/core/__init__.py
--rw-r--r--   0        0        0     9017 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/core/config.py
--rw-r--r--   0        0        0    17134 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/core/dfops.py
--rw-r--r--   0        0        0     4182 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/core/metadata.py
--rw-r--r--   0        0        0   101134 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/core/processor.py
--rw-r--r--   0        0        0     4903 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/diagnostics.py
--rw-r--r--   0        0        0      262 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/io/__init__.py
--rw-r--r--   0        0        0     5939 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/io/hdf5.py
--rw-r--r--   0        0        0     1381 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/io/nexus.py
--rw-r--r--   0        0        0     7865 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/io/tiff.py
--rw-r--r--   0        0        0      166 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/loader/__init__.py
--rw-r--r--   0        0        0       14 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/loader/base/README.md
--rw-r--r--   0        0        0        0 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/loader/base/__init__.py
--rw-r--r--   0        0        0     6110 2024-04-04 07:13:45.503365 sed_processor-0.1.9a6/sed/loader/base/loader.py
--rw-r--r--   0        0        0        0 2024-04-04 07:13:45.503365 sed_processor-0.1.9a6/sed/loader/flash/__init__.py
--rw-r--r--   0        0        0    35851 2024-04-04 07:13:45.503365 sed_processor-0.1.9a6/sed/loader/flash/loader.py
--rw-r--r--   0        0        0     4300 2024-04-04 07:13:45.503365 sed_processor-0.1.9a6/sed/loader/flash/metadata.py
--rw-r--r--   0        0        0        0 2024-04-04 07:13:45.503365 sed_processor-0.1.9a6/sed/loader/generic/__init__.py
--rw-r--r--   0        0        0     5749 2024-04-04 07:13:45.503365 sed_processor-0.1.9a6/sed/loader/generic/loader.py
--rw-r--r--   0        0        0     2015 2024-04-04 07:13:45.503365 sed_processor-0.1.9a6/sed/loader/loader_interface.py
--rw-r--r--   0        0        0    11180 2024-04-04 07:13:45.503365 sed_processor-0.1.9a6/sed/loader/mirrorutil.py
--rw-r--r--   0        0        0        0 2024-04-04 07:13:45.503365 sed_processor-0.1.9a6/sed/loader/mpes/__init__.py
--rw-r--r--   0        0        0    35421 2024-04-04 07:13:45.503365 sed_processor-0.1.9a6/sed/loader/mpes/loader.py
--rw-r--r--   0        0        0        0 2024-04-04 07:13:45.503365 sed_processor-0.1.9a6/sed/loader/sxp/__init__.py
--rw-r--r--   0        0        0    38089 2024-04-04 07:13:45.503365 sed_processor-0.1.9a6/sed/loader/sxp/loader.py
--rw-r--r--   0        0        0     7507 2024-04-04 07:13:45.503365 sed_processor-0.1.9a6/sed/loader/utils.py
--rw-r--r--   0        0        0     4816 1970-01-01 00:00:00.000000 sed_processor-0.1.9a6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-04 09:34:13.511217 sed_processor-0.1.9a7/LICENSE
+-rw-r--r--   0        0        0     2881 2024-04-04 09:34:13.511217 sed_processor-0.1.9a7/README.md
+-rw-r--r--   0        0        0     2840 2024-04-04 09:34:25.339274 sed_processor-0.1.9a7/pyproject.toml
+-rw-r--r--   0        0        0      127 2024-04-04 09:34:13.515217 sed_processor-0.1.9a7/sed/__init__.py
+-rw-r--r--   0        0        0      160 2024-04-04 09:34:13.515217 sed_processor-0.1.9a7/sed/binning/__init__.py
+-rw-r--r--   0        0        0    21273 2024-04-04 09:34:13.515217 sed_processor-0.1.9a7/sed/binning/binning.py
+-rw-r--r--   0        0        0     8570 2024-04-04 09:34:13.515217 sed_processor-0.1.9a7/sed/binning/numba_bin.py
+-rw-r--r--   0        0        0     6073 2024-04-04 09:34:13.515217 sed_processor-0.1.9a7/sed/binning/utils.py
+-rw-r--r--   0        0        0      231 2024-04-04 09:34:13.515217 sed_processor-0.1.9a7/sed/calibrator/__init__.py
+-rw-r--r--   0        0        0    17235 2024-04-04 09:34:13.515217 sed_processor-0.1.9a7/sed/calibrator/delay.py
+-rw-r--r--   0        0        0    88868 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/calibrator/energy.py
+-rw-r--r--   0        0        0    83190 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/calibrator/momentum.py
+-rwxr-xr-x   0        0        0    17175 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/config/NXmpes_config.json
+-rw-r--r--   0        0        0     4692 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/config/default.yaml
+-rw-r--r--   0        0        0     6359 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/config/flash_example_config.yaml
+-rw-r--r--   0        0        0    11357 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/config/mpes_example_config.yaml
+-rw-r--r--   0        0        0      105 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/core/__init__.py
+-rw-r--r--   0        0        0     9017 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/core/config.py
+-rw-r--r--   0        0        0    17134 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/core/dfops.py
+-rw-r--r--   0        0        0     4182 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/core/metadata.py
+-rw-r--r--   0        0        0   101146 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/core/processor.py
+-rw-r--r--   0        0        0     4903 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/diagnostics.py
+-rw-r--r--   0        0        0      262 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/io/__init__.py
+-rw-r--r--   0        0        0     5939 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/io/hdf5.py
+-rw-r--r--   0        0        0     1381 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/io/nexus.py
+-rw-r--r--   0        0        0     7865 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/io/tiff.py
+-rw-r--r--   0        0        0      166 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/loader/__init__.py
+-rw-r--r--   0        0        0       14 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/loader/base/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/loader/base/__init__.py
+-rw-r--r--   0        0        0     6110 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/loader/base/loader.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/loader/flash/__init__.py
+-rw-r--r--   0        0        0    35851 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/loader/flash/loader.py
+-rw-r--r--   0        0        0     4300 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/loader/flash/metadata.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/loader/generic/__init__.py
+-rw-r--r--   0        0        0     5749 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/loader/generic/loader.py
+-rw-r--r--   0        0        0     2015 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/loader/loader_interface.py
+-rw-r--r--   0        0        0    11180 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/loader/mirrorutil.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/loader/mpes/__init__.py
+-rw-r--r--   0        0        0    35421 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/loader/mpes/loader.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/loader/sxp/__init__.py
+-rw-r--r--   0        0        0    38089 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/loader/sxp/loader.py
+-rw-r--r--   0        0        0     7507 2024-04-04 09:34:13.519217 sed_processor-0.1.9a7/sed/loader/utils.py
+-rw-r--r--   0        0        0     4816 1970-01-01 00:00:00.000000 sed_processor-0.1.9a7/PKG-INFO
```

### Comparing `sed_processor-0.1.9a6/LICENSE` & `sed_processor-0.1.9a7/LICENSE`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a6/README.md` & `sed_processor-0.1.9a7/README.md`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a6/pyproject.toml` & `sed_processor-0.1.9a7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "sed-processor"
 packages = [
     {include = "sed"}
 ]
-version = "0.1.9a6"
+version = "0.1.9a7"
 description = "Single Event Data Frame Processor: Backend to handle photoelectron resolved datastreams"
 authors = ["OpenCOMPES team <sed-processor@mpes.science>"]
 readme = "README.md"
 repository = "https://github.com/OpenCOMPES/sed"
 documentation = "https://opencompes.github.io/sed/"
 keywords = ["sed", "mpes", "flash", "arpes"]
 license = "MIT"
```

### Comparing `sed_processor-0.1.9a6/sed/binning/binning.py` & `sed_processor-0.1.9a7/sed/binning/binning.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a6/sed/binning/numba_bin.py` & `sed_processor-0.1.9a7/sed/binning/numba_bin.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a6/sed/binning/utils.py` & `sed_processor-0.1.9a7/sed/binning/utils.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a6/sed/calibrator/delay.py` & `sed_processor-0.1.9a7/sed/calibrator/delay.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a6/sed/calibrator/energy.py` & `sed_processor-0.1.9a7/sed/calibrator/energy.py`

 * *Files 0% similar despite different names*

```diff
@@ -574,15 +574,15 @@
                 f", got {energy_scale}.",
             )
 
         binwidth = kwds.pop("binwidth", self.binwidth)
         binning = kwds.pop("binning", self.binning)
 
         if method == "lmfit":
-            self.calibration = fit_energy_calibation(
+            self.calibration = fit_energy_calibration(
                 landmarks,
                 sign * biases,
                 binwidth,
                 binning,
                 ref_id=ref_id,
                 t=t,
                 energy_scale=energy_scale,
@@ -2081,15 +2081,15 @@
 
     except IndexError:  # When no peaks have been found
         pass
 
     return (np.asarray(max_peaks), np.asarray(min_peaks))
 
 
-def fit_energy_calibation(
+def fit_energy_calibration(
     pos: Union[List[float], np.ndarray],
     vals: Union[List[float], np.ndarray],
     binwidth: float,
     binning: int,
     ref_id: int = 0,
     ref_energy: float = None,
     t: Union[List[float], np.ndarray] = None,
```

### Comparing `sed_processor-0.1.9a6/sed/calibrator/momentum.py` & `sed_processor-0.1.9a7/sed/calibrator/momentum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 """sed.calibrator.momentum module. Code for momentum calibration and distortion
 correction. Mostly ported from https://github.com/mpes-kit/mpes.
 """
 import itertools as it
 from copy import deepcopy
 from datetime import datetime
-from multiprocessing import Pool
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Tuple
 from typing import Union
 
 import bokeh.palettes as bp
 import bokeh.plotting as pbk
 import dask.dataframe
 import ipywidgets as ipw
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-import psutil
 import scipy.ndimage as ndi
 import xarray as xr
 from bokeh.colors import RGB
 from bokeh.io import output_notebook
 from bokeh.palettes import Category10 as ColorCycle
 from IPython.display import display
+from joblib import delayed
+from joblib import Parallel
 from matplotlib import cm
 from numpy.linalg import norm
 from scipy.interpolate import griddata
 from scipy.ndimage import map_coordinates
 from symmetrize import pointops as po
 from symmetrize import sym
 from symmetrize import tps
 
-N_CPU = psutil.cpu_count()
-
 
 class MomentumCorrector:
     """
     Momentum distortion correction and momentum calibration workflow functions.
 
     Args:
         data (Union[xr.DataArray, np.ndarray], optional): Multidimensional hypervolume
@@ -68,18 +66,14 @@
             config (dict, optional): Config dictionary. Defaults to None.
         """
         if config is None:
             config = {}
 
         self._config = config
 
-        self.num_cores = self._config.get("binning", {}).get("num_cores", N_CPU - 1)
-        if self.num_cores >= N_CPU:
-            self.num_cores = N_CPU - 1
-
         self.image: np.ndarray = None
         self.img_ndim: int = None
         self.slice: np.ndarray = None
         self.slice_corrected: np.ndarray = None
         self.slice_transformed: np.ndarray = None
         self.bin_ranges: List[Tuple] = self._config["momentum"].get("bin_ranges", [])
 
@@ -337,19 +331,18 @@
                 Array of landmarks, possibly including a center peak. Its shape should
                 be (n,2), where n is equal to the rotation symmetry, or the rotation
                 symmetry+1, if the center is included.
             direction (str, optional):
                 Direction for ordering the points. Defaults to "ccw".
             symscores (bool, optional):
                 Option to calculate symmetry scores. Defaults to False.
-            rotsym (int, optional): Rotational symmetry of the data. Defaults to 6.
             **kwds: Keyword arguments.
 
                 - **symtype** (str): Type of symmetry scores to calculte
-                  if symscores is True.
+                  if symscores is True. Defaults to "rotation".
 
         Raises:
             ValueError: Raised if the number of points does not match the rotsym.
         """
         self.rotsym = int(rotsym)
         self.rotsym_angle = int(360 / self.rotsym)
         self.arot = np.array([0] + [self.rotsym_angle] * (self.rotsym - 1))
@@ -597,14 +590,15 @@
 
     def spline_warp_estimate(
         self,
         image: np.ndarray = None,
         use_center: bool = None,
         fixed_center: bool = True,
         interp_order: int = 1,
+        ascale: Union[float, list, tuple, np.ndarray] = None,
         verbose: bool = True,
         **kwds,
     ) -> np.ndarray:
         """Estimate the spline deformation field using thin plate spline registration.
 
         Args:
             image (np.ndarray, optional):
@@ -614,14 +608,21 @@
                 process. Defaults to config value, or True.
             fixed_center (bool, optional):
                 Option to have a fixed center during registration-based
                 symmetrization. Defaults to True.
             interp_order (int, optional):
                 Order of interpolation (see ``scipy.ndimage.map_coordinates()``).
                 Defaults to 1.
+            ascale: (Union[float, np.ndarray], optional): Scale parameter determining a realtive
+                scale for each symmetry feature. If provided as single float, rotsym has to be 4.
+                This parameter describes the relative scaling between the two orthogonal symmetry
+                directions (for an orthorhombic system). This requires the correction points to be
+                located along the principal axes (X/Y points of the Brillouin zone). Otherwise, an
+                array with ``rotsym`` elements is expected, containing relative scales for each
+                feature. Defaults to an array of equal scales.
             verbose (bool, optional): Option to report the used landmarks for correction.
                 Defaults to True.
             **kwds: keyword arguments:
 
                 - **landmarks**: (list/array): Landmark positions (row, column) used
                   for registration. Defaults to  self.pouter_ord
                 - **targets**: (list/array): Target positions (row, column) used for
@@ -640,23 +641,27 @@
                 image = np.zeros(self._config["momentum"]["bins"][0:2])
                 self.bin_ranges = self._config["momentum"]["ranges"]
 
         if self.pouter_ord is None:
             if self.pouter is not None:
                 self.pouter_ord = po.pointset_order(self.pouter)
                 self.correction["creation_date"] = datetime.now().timestamp()
+                self.correction["creation_date"] = datetime.now().timestamp()
             else:
                 try:
                     features = np.asarray(
                         self.correction["feature_points"],
                     )
                     rotsym = self.correction["rotation_symmetry"]
                     include_center = self.correction["include_center"]
                     if not include_center and len(features) > rotsym:
                         features = features[:rotsym, :]
+                    ascale = self.correction.get("ascale", None)
+                    if ascale is not None:
+                        ascale = np.asarray(ascale)
 
                     if verbose:
                         if "creation_date" in self.correction:
                             datestring = datetime.fromtimestamp(
                                 self.correction["creation_date"],
                             ).strftime(
                                 "%m/%d/%Y, %H:%M:%S",
@@ -676,14 +681,35 @@
                     ) from exc
 
                 self.add_features(features=features, rotsym=rotsym, include_center=include_center)
 
         else:
             self.correction["creation_date"] = datetime.now().timestamp()
 
+        if ascale is not None:
+            if isinstance(ascale, (int, float, np.floating, np.integer)):
+                if self.rotsym != 4:
+                    raise ValueError(
+                        "Providing ascale as scalar number is only valid for 'rotsym'==4.",
+                    )
+                self.ascale = np.array([1.0, ascale, 1.0, ascale])
+            elif isinstance(ascale, (tuple, list, np.ndarray)):
+                if len(ascale) != len(self.ascale):
+                    raise ValueError(
+                        f"ascale needs to be of length 'rotsym', but has length {len(ascale)}.",
+                    )
+                self.ascale = np.asarray(ascale)
+            else:
+                raise TypeError(
+                    (
+                        "ascale needs to be a single number or a list/tuple/np.ndarray of length ",
+                        f"'rotsym' ({self.rotsym})!",
+                    ),
+                )
+
         if use_center is None:
             try:
                 use_center = self.correction["use_center"]
             except KeyError:
                 use_center = True
         self.use_center = use_center
 
@@ -749,14 +775,15 @@
         self.correction["include_center"] = self.include_center
         if self.include_center:
             self.correction["feature_points"] = np.concatenate(
                 (self.pouter_ord, np.asarray([self.pcent])),
             )
         else:
             self.correction["feature_points"] = self.pouter_ord
+        self.correction["ascale"] = self.ascale
 
         if self.slice is not None:
             self.slice_corrected = corrected_image
 
         if verbose:
             print("Calulated thin spline correction based on the following landmarks:")
             print(f"pouter: {self.pouter}")
@@ -1222,15 +1249,14 @@
     def calc_inverse_dfield(self):
         """Calculate the inverse dfield from the cdeform and rdeform fields"""
         self.inverse_dfield = generate_inverse_dfield(
             self.rdeform_field,
             self.cdeform_field,
             self.bin_ranges,
             self.detector_ranges,
-            self.num_cores,
         )
 
         return self.inverse_dfield
 
     def view(  # pylint: disable=dangerous-default-value
         self,
         image: np.ndarray = None,
@@ -1712,15 +1738,14 @@
                     raise ValueError("No corrections or transformations defined!")
 
             self.inverse_dfield = generate_inverse_dfield(
                 self.rdeform_field,
                 self.cdeform_field,
                 self.bin_ranges,
                 self.detector_ranges,
-                self.num_cores,
             )
             self.dfield_updated = False
 
         out_df = df.map_partitions(
             apply_dfield,
             dfield=self.inverse_dfield,
             x_column=x_column,
@@ -2048,26 +2073,24 @@
 
 
 def generate_inverse_dfield(
     rdeform_field: np.ndarray,
     cdeform_field: np.ndarray,
     bin_ranges: List[Tuple],
     detector_ranges: List[Tuple],
-    num_cores: int,
 ) -> np.ndarray:
     """Generate inverse deformation field using inperpolation with griddata.
     Assuming the binning range of the input ``rdeform_field`` and ``cdeform_field``
     covers the whole detector.
 
     Args:
         rdeform_field (np.ndarray): Row-wise deformation field.
         cdeform_field (np.ndarray): Column-wise deformation field.
         bin_ranges (List[Tuple]): Detector ranges of the binned coordinates.
         detector_ranges (List[Tuple]): Ranges of detector coordinates to interpolate to.
-        num_cores (int): number of cores to use for parallelization.
 
     Returns:
         np.ndarray: The calculated inverse deformation field (row/column)
     """
     print(
         "Calculating inverse deformation field, this might take a moment...",
     )
@@ -2092,57 +2115,15 @@
 
     bin_step = (
         np.asarray(bin_ranges)[0:2][:, 1] - np.asarray(bin_ranges)[0:2][:, 0]
     ) / cdeform_field.shape
     rc_position = []  # row/column position in c/rdeform_field
     r_dest = []  # destination pixel row position
     c_dest = []  # destination pixel column position
-    compute_i0 = [(cdeform_field.shape[0] * i) // num_cores for i in np.arange(0, num_cores)]
-    compute_i1 = [(cdeform_field.shape[0] * i) // num_cores for i in np.arange(1, num_cores + 1)]
-    data = [
-        (rdeform_field, cdeform_field, bin_ranges, bin_step, i0, i1)
-        for (i0, i1) in zip(compute_i0, compute_i1)
-    ]
-    with Pool(num_cores) as p:
-        ret = p.map(generate_lists, data)
-
-    for pos, rd, cd in ret:
-        rc_position += pos
-        r_dest += rd
-        c_dest += cd
-
-    with Pool(2) as p:
-        ret = p.map(
-            griddata_,
-            [
-                (np.asarray(rc_position), np.asarray(r_dest), (r_mesh, c_mesh)),
-                (np.asarray(rc_position), np.asarray(c_dest), (r_mesh, c_mesh)),
-            ],
-        )
-
-    inverse_dfield = np.asarray([ret[0], ret[1]])
-
-    return inverse_dfield
-
-
-def generate_lists(args):
-    """Function for paralellizing code with multiprocessing.Pool.map
-
-    Args:
-        args: argument tuple containing (rdeform_field, cdeform_field, bin_ranges, bin_step, i0, i1)
-
-    Returns:
-        return tuple of lists (rc_position, r_dest, c_dest)
-    """
-    (rdeform_field, cdeform_field, bin_ranges, bin_step, i0, i1) = args
-    rc_position = []  # row/column position in c/rdeform_field
-    r_dest = []  # destination pixel row position
-    c_dest = []  # destination pixel column position
-
-    for i in np.arange(i0, i1):
+    for i in np.arange(cdeform_field.shape[0]):
         for j in np.arange(cdeform_field.shape[1]):
             if not np.isnan(rdeform_field[i, j]) and not np.isnan(
                 cdeform_field[i, j],
             ):
                 rc_position.append(
                     [
                         rdeform_field[i, j] + bin_ranges[0][0] / bin_step[0],
@@ -2151,27 +2132,23 @@
                 )
                 r_dest.append(
                     bin_step[0] * i + bin_ranges[0][0],
                 )
                 c_dest.append(
                     bin_step[1] * j + bin_ranges[1][0],
                 )
-    return (rc_position, r_dest, c_dest)
-
 
-def griddata_(args):
-    """Wrapper for griddata to use with multiprocessing.Pool.map
+    ret = Parallel(n_jobs=2)(
+        delayed(griddata)(np.asarray(rc_position), np.asarray(arg), (r_mesh, c_mesh))
+        for arg in [r_dest, c_dest]
+    )
 
-    Args:
-        args: argument tuple to griddata
+    inverse_dfield = np.asarray([ret[0], ret[1]])
 
-    Returns:
-        return value of griddata
-    """
-    return griddata(*args)
+    return inverse_dfield
 
 
 def load_dfield(file: str) -> Tuple[np.ndarray, np.ndarray]:
     """Load inverse dfield from file
 
     Args:
         file (str): Path to file containing the inverse dfield
```

### Comparing `sed_processor-0.1.9a6/sed/config/NXmpes_config.json` & `sed_processor-0.1.9a7/sed/config/NXmpes_config.json`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a6/sed/config/default.yaml` & `sed_processor-0.1.9a7/sed/config/default.yaml`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a6/sed/config/flash_example_config.yaml` & `sed_processor-0.1.9a7/sed/config/flash_example_config.yaml`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a6/sed/config/mpes_example_config.yaml` & `sed_processor-0.1.9a7/sed/config/mpes_example_config.yaml`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a6/sed/core/config.py` & `sed_processor-0.1.9a7/sed/core/config.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a6/sed/core/dfops.py` & `sed_processor-0.1.9a7/sed/core/dfops.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a6/sed/core/metadata.py` & `sed_processor-0.1.9a7/sed/core/metadata.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a6/sed/core/processor.py` & `sed_processor-0.1.9a7/sed/core/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -621,15 +621,15 @@
             raise ValueError("No momentum correction parameters to save!")
         correction = {}
         for key, value in self.mc.correction.items():
             if key in ["reference_points", "target_points", "cdeform_field", "rdeform_field"]:
                 continue
             if key in ["use_center", "rotation_symmetry"]:
                 correction[key] = value
-            elif key == "center_point":
+            elif key in ["center_point", "ascale"]:
                 correction[key] = [float(i) for i in value]
             elif key in ["outer_points", "feature_points"]:
                 correction[key] = []
                 for point in value:
                     correction[key].append([float(i) for i in point])
             else:
                 correction[key] = float(value)
```

### Comparing `sed_processor-0.1.9a6/sed/diagnostics.py` & `sed_processor-0.1.9a7/sed/diagnostics.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a6/sed/io/hdf5.py` & `sed_processor-0.1.9a7/sed/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a6/sed/io/nexus.py` & `sed_processor-0.1.9a7/sed/io/nexus.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a6/sed/io/tiff.py` & `sed_processor-0.1.9a7/sed/io/tiff.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a6/sed/loader/base/loader.py` & `sed_processor-0.1.9a7/sed/loader/base/loader.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a6/sed/loader/flash/loader.py` & `sed_processor-0.1.9a7/sed/loader/flash/loader.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a6/sed/loader/flash/metadata.py` & `sed_processor-0.1.9a7/sed/loader/flash/metadata.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a6/sed/loader/generic/loader.py` & `sed_processor-0.1.9a7/sed/loader/generic/loader.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a6/sed/loader/loader_interface.py` & `sed_processor-0.1.9a7/sed/loader/loader_interface.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a6/sed/loader/mirrorutil.py` & `sed_processor-0.1.9a7/sed/loader/mirrorutil.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a6/sed/loader/mpes/loader.py` & `sed_processor-0.1.9a7/sed/loader/mpes/loader.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a6/sed/loader/sxp/loader.py` & `sed_processor-0.1.9a7/sed/loader/sxp/loader.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a6/sed/loader/utils.py` & `sed_processor-0.1.9a7/sed/loader/utils.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a6/PKG-INFO` & `sed_processor-0.1.9a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sed-processor
-Version: 0.1.9a6
+Version: 0.1.9a7
 Summary: Single Event Data Frame Processor: Backend to handle photoelectron resolved datastreams
 Home-page: https://github.com/OpenCOMPES/sed
 License: MIT
 Keywords: sed,mpes,flash,arpes
 Author: OpenCOMPES team
 Author-email: sed-processor@mpes.science
 Requires-Python: >=3.8,<3.12
```

