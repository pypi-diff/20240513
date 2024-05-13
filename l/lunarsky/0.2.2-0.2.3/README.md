# Comparing `tmp/lunarsky-0.2.2.tar.gz` & `tmp/lunarsky-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lunarsky-0.2.2.tar", last modified: Fri Mar 22 21:06:26 2024, max compression
+gzip compressed data, was "lunarsky-0.2.3.tar", last modified: Mon May 13 19:16:35 2024, max compression
```

## Comparing `lunarsky-0.2.2.tar` & `lunarsky-0.2.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:06:26.736067 lunarsky-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-22 21:06:19.000000 lunarsky-0.2.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:06:26.728067 lunarsky-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:06:26.728067 lunarsky-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-03-22 21:06:19.000000 lunarsky-0.2.2/.github/workflows/pypirelease.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-03-22 21:06:19.000000 lunarsky-0.2.2/.github/workflows/testsuite.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-03-22 21:06:19.000000 lunarsky-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-03-22 21:06:19.000000 lunarsky-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-03-22 21:06:19.000000 lunarsky-0.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-03-22 21:06:19.000000 lunarsky-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-22 21:06:19.000000 lunarsky-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-03-22 21:06:26.736067 lunarsky-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-03-22 21:06:19.000000 lunarsky-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:06:26.728067 lunarsky-0.2.2/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-22 21:06:19.000000 lunarsky-0.2.2/ci/cache_kernels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:06:26.732067 lunarsky-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    21034 2024-03-22 21:06:19.000000 lunarsky-0.2.2/docs/figure.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:06:26.732067 lunarsky-0.2.2/lunarsky/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-22 21:06:19.000000 lunarsky-0.2.2/lunarsky/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:06:26.732067 lunarsky-0.2.2/lunarsky/data/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-22 21:06:19.000000 lunarsky-0.2.2/lunarsky/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:06:26.728067 lunarsky-0.2.2/lunarsky/data/fk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:06:26.732067 lunarsky-0.2.2/lunarsky/data/fk/satellites/
--rw-r--r--   0 runner    (1001) docker     (127)    21437 2024-03-22 21:06:19.000000 lunarsky-0.2.2/lunarsky/data/fk/satellites/moon_080317.tf
--rw-r--r--   0 runner    (1001) docker     (127)     8468 2024-03-22 21:06:19.000000 lunarsky-0.2.2/lunarsky/data/fk/satellites/moon_assoc_me.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:06:26.732067 lunarsky-0.2.2/lunarsky/data/pck/
--rw-r--r--   0 runner    (1001) docker     (127)  1770496 2024-03-22 21:06:19.000000 lunarsky-0.2.2/lunarsky/data/pck/moon_pa_de421_1900-2050.bpc
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-03-22 21:06:19.000000 lunarsky-0.2.2/lunarsky/mcmf.py
--rw-r--r--   0 runner    (1001) docker     (127)    22103 2024-03-22 21:06:19.000000 lunarsky-0.2.2/lunarsky/moon.py
--rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-03-22 21:06:19.000000 lunarsky-0.2.2/lunarsky/sky_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-03-22 21:06:19.000000 lunarsky-0.2.2/lunarsky/spice_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:06:26.736067 lunarsky-0.2.2/lunarsky/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-03-22 21:06:19.000000 lunarsky-0.2.2/lunarsky/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-03-22 21:06:19.000000 lunarsky-0.2.2/lunarsky/tests/test_moon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-03-22 21:06:19.000000 lunarsky-0.2.2/lunarsky/tests/test_sky_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-03-22 21:06:19.000000 lunarsky-0.2.2/lunarsky/tests/test_spice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-22 21:06:19.000000 lunarsky-0.2.2/lunarsky/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (127)    12966 2024-03-22 21:06:19.000000 lunarsky-0.2.2/lunarsky/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-03-22 21:06:19.000000 lunarsky-0.2.2/lunarsky/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     7734 2024-03-22 21:06:19.000000 lunarsky-0.2.2/lunarsky/topo.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-22 21:06:26.000000 lunarsky-0.2.2/lunarsky/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:06:26.736067 lunarsky-0.2.2/lunarsky.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-03-22 21:06:26.000000 lunarsky-0.2.2/lunarsky.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-22 21:06:26.000000 lunarsky-0.2.2/lunarsky.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 21:06:26.000000 lunarsky-0.2.2/lunarsky.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-22 21:06:26.000000 lunarsky-0.2.2/lunarsky.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-22 21:06:26.000000 lunarsky-0.2.2/lunarsky.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-22 21:06:26.736067 lunarsky-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-22 21:06:19.000000 lunarsky-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:16:35.162403 lunarsky-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 19:16:30.000000 lunarsky-0.2.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:16:35.150403 lunarsky-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:16:35.154403 lunarsky-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-13 19:16:30.000000 lunarsky-0.2.3/.github/workflows/pypirelease.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-13 19:16:30.000000 lunarsky-0.2.3/.github/workflows/testsuite.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-13 19:16:30.000000 lunarsky-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-13 19:16:30.000000 lunarsky-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-13 19:16:30.000000 lunarsky-0.2.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-13 19:16:30.000000 lunarsky-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-13 19:16:30.000000 lunarsky-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-05-13 19:16:35.162403 lunarsky-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-13 19:16:30.000000 lunarsky-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:16:35.154403 lunarsky-0.2.3/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-13 19:16:30.000000 lunarsky-0.2.3/ci/cache_kernels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:16:35.154403 lunarsky-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    21034 2024-05-13 19:16:30.000000 lunarsky-0.2.3/docs/figure.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:16:35.158403 lunarsky-0.2.3/lunarsky/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-13 19:16:30.000000 lunarsky-0.2.3/lunarsky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:16:35.158403 lunarsky-0.2.3/lunarsky/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-13 19:16:30.000000 lunarsky-0.2.3/lunarsky/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:16:35.154403 lunarsky-0.2.3/lunarsky/data/fk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:16:35.158403 lunarsky-0.2.3/lunarsky/data/fk/satellites/
+-rw-r--r--   0 runner    (1001) docker     (127)    21437 2024-05-13 19:16:30.000000 lunarsky-0.2.3/lunarsky/data/fk/satellites/moon_080317.tf
+-rw-r--r--   0 runner    (1001) docker     (127)     8468 2024-05-13 19:16:30.000000 lunarsky-0.2.3/lunarsky/data/fk/satellites/moon_assoc_me.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:16:35.158403 lunarsky-0.2.3/lunarsky/data/pck/
+-rw-r--r--   0 runner    (1001) docker     (127)  1770496 2024-05-13 19:16:30.000000 lunarsky-0.2.3/lunarsky/data/pck/moon_pa_de421_1900-2050.bpc
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-05-13 19:16:30.000000 lunarsky-0.2.3/lunarsky/mcmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22103 2024-05-13 19:16:30.000000 lunarsky-0.2.3/lunarsky/moon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-05-13 19:16:30.000000 lunarsky-0.2.3/lunarsky/sky_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-05-13 19:16:30.000000 lunarsky-0.2.3/lunarsky/spice_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:16:35.162403 lunarsky-0.2.3/lunarsky/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-13 19:16:30.000000 lunarsky-0.2.3/lunarsky/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-05-13 19:16:30.000000 lunarsky-0.2.3/lunarsky/tests/test_moon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-13 19:16:30.000000 lunarsky-0.2.3/lunarsky/tests/test_sky_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-13 19:16:30.000000 lunarsky-0.2.3/lunarsky/tests/test_spice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-13 19:16:30.000000 lunarsky-0.2.3/lunarsky/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12966 2024-05-13 19:16:30.000000 lunarsky-0.2.3/lunarsky/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-13 19:16:30.000000 lunarsky-0.2.3/lunarsky/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7734 2024-05-13 19:16:30.000000 lunarsky-0.2.3/lunarsky/topo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-13 19:16:35.000000 lunarsky-0.2.3/lunarsky/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:16:35.162403 lunarsky-0.2.3/lunarsky.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-05-13 19:16:35.000000 lunarsky-0.2.3/lunarsky.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-13 19:16:35.000000 lunarsky-0.2.3/lunarsky.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:16:35.000000 lunarsky-0.2.3/lunarsky.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-13 19:16:35.000000 lunarsky-0.2.3/lunarsky.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-13 19:16:35.000000 lunarsky-0.2.3/lunarsky.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-13 19:16:35.162403 lunarsky-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-13 19:16:30.000000 lunarsky-0.2.3/setup.py
```

### Comparing `lunarsky-0.2.2/.github/workflows/pypirelease.yaml` & `lunarsky-0.2.3/.github/workflows/pypirelease.yaml`

 * *Files identical despite different names*

### Comparing `lunarsky-0.2.2/.github/workflows/testsuite.yaml` & `lunarsky-0.2.3/.github/workflows/testsuite.yaml`

 * *Files identical despite different names*

### Comparing `lunarsky-0.2.2/.gitignore` & `lunarsky-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lunarsky-0.2.2/.pre-commit-config.yaml` & `lunarsky-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lunarsky-0.2.2/CHANGELOG.md` & `lunarsky-0.2.3/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # Changelog
 
-## [0.2.2] -- 2022-03-19
+## [0.2.3] -- 2024-05-13
+
+## Fixed
+- Make lunarsky.time.Time location handling compatible with astropy >= 6.1
+
+## [0.2.2] -- 2024-03-19
 
 ## Added
 - Support for ellipsoid models for selenodetic coordinates (non-spherical)
 
 ## Deprecated
 - Removed support for Python < 3.9. Astropy >= 6.0 is required for ellipsoid support
```

### Comparing `lunarsky-0.2.2/LICENSE` & `lunarsky-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lunarsky-0.2.2/PKG-INFO` & `lunarsky-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lunarsky
-Version: 0.2.2
+Version: 0.2.3
 Summary: Astropy support for selenocentric (Moon)reference frames and lunar surface observatories.
 Home-page: https://github.com/aelanman/lunarsky
 Download-URL: https://github.com/aelanman/lunarsky/archive/refs/tags/v0.1.1.tar.gz
 Author: Adam E. Lanman
 License: BSD
 Keywords: astronomy moon spice
 Classifier: Development Status :: 3 - Alpha
@@ -70,15 +70,15 @@
 The cartesian axes of the selenocentric system are those of the MCMF frame. In the selenodetic coordinates, "height" is defined relative to a sphere of radius 1737.1 km.
 * `SkyCoord` – A replacement for `astropy.coordinates.SkyCoord`, with modifications that ensure compatibility with the `MoonLocation` class.
 * `Time` – A replacement for the `astropy.time.Time` class, which can accept a `MoonLocation` instance as its location parameter, allowing for the calculation of local sidereal times on the Moon. The LST of an observer on the Moon is defined as the right ascension of the zenith.
 
 
 ## Credit
 
-This package makes use fo the ``spiceypy`` wrapper [2] for the JPl SPICE Toolkit, produced by the NASA Navigation and Ancillary Information Facility (NAIF) [3] [4]. The transformations are defined using data in kernel files ``pck/moon_pa_de421_1900-2050.bpc``, ``moon_080317.tf``, and ``moon_assoc_me.tf``. These may be found at [the NAIF website](https://naif.jpl.nasa.gov/pub/naif/generic_kernels), and were produced by Nat Bachman (NAIF/JPL) in March 2008. Further information may be found in the comments in these files in the `data` directory.
+This package makes use fo the ``spiceypy`` wrapper [2] for the JPL SPICE Toolkit, produced by the NASA Navigation and Ancillary Information Facility (NAIF) [3] [4]. The transformations are defined using data in kernel files ``pck/moon_pa_de421_1900-2050.bpc``, ``moon_080317.tf``, and ``moon_assoc_me.tf``. These may be found at [the NAIF website](https://naif.jpl.nasa.gov/pub/naif/generic_kernels), and were produced by Nat Bachman (NAIF/JPL) in March 2008. Further information may be found in the comments in these files in the `data` directory.
 
 ## References
 [1]: Ye, Hanlin, et al. "Looking Vector Direction Analysis for the Moon-Based Earth Observation Optical Sensor." IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing, vol. 11, no. 11, Nov. 2018, pp. 4488–99. IEEE Xplore, doi:10.1109/JSTARS.2018.2870247.
 
 [2]: Annex et al., (2020). SpiceyPy: a Pythonic Wrapper for the SPICE Toolkit. Journal of Open Source Software, 5(46), 2050, https://doi.org/10.21105/joss.02050
 
 [3]: Acton, C.H.; "Ancillary Data Services of NASA's Navigation and Ancillary Information Facility;" Planetary and Space Science, Vol. 44, No. 1, pp. 65-70, 1996.
```

### Comparing `lunarsky-0.2.2/README.md` & `lunarsky-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 The cartesian axes of the selenocentric system are those of the MCMF frame. In the selenodetic coordinates, "height" is defined relative to a sphere of radius 1737.1 km.
 * `SkyCoord` – A replacement for `astropy.coordinates.SkyCoord`, with modifications that ensure compatibility with the `MoonLocation` class.
 * `Time` – A replacement for the `astropy.time.Time` class, which can accept a `MoonLocation` instance as its location parameter, allowing for the calculation of local sidereal times on the Moon. The LST of an observer on the Moon is defined as the right ascension of the zenith.
 
 
 ## Credit
 
-This package makes use fo the ``spiceypy`` wrapper [2] for the JPl SPICE Toolkit, produced by the NASA Navigation and Ancillary Information Facility (NAIF) [3] [4]. The transformations are defined using data in kernel files ``pck/moon_pa_de421_1900-2050.bpc``, ``moon_080317.tf``, and ``moon_assoc_me.tf``. These may be found at [the NAIF website](https://naif.jpl.nasa.gov/pub/naif/generic_kernels), and were produced by Nat Bachman (NAIF/JPL) in March 2008. Further information may be found in the comments in these files in the `data` directory.
+This package makes use fo the ``spiceypy`` wrapper [2] for the JPL SPICE Toolkit, produced by the NASA Navigation and Ancillary Information Facility (NAIF) [3] [4]. The transformations are defined using data in kernel files ``pck/moon_pa_de421_1900-2050.bpc``, ``moon_080317.tf``, and ``moon_assoc_me.tf``. These may be found at [the NAIF website](https://naif.jpl.nasa.gov/pub/naif/generic_kernels), and were produced by Nat Bachman (NAIF/JPL) in March 2008. Further information may be found in the comments in these files in the `data` directory.
 
 ## References
 [1]: Ye, Hanlin, et al. "Looking Vector Direction Analysis for the Moon-Based Earth Observation Optical Sensor." IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing, vol. 11, no. 11, Nov. 2018, pp. 4488–99. IEEE Xplore, doi:10.1109/JSTARS.2018.2870247.
 
 [2]: Annex et al., (2020). SpiceyPy: a Pythonic Wrapper for the SPICE Toolkit. Journal of Open Source Software, 5(46), 2050, https://doi.org/10.21105/joss.02050
 
 [3]: Acton, C.H.; "Ancillary Data Services of NASA's Navigation and Ancillary Information Facility;" Planetary and Space Science, Vol. 44, No. 1, pp. 65-70, 1996.
```

### Comparing `lunarsky-0.2.2/ci/cache_kernels.py` & `lunarsky-0.2.3/ci/cache_kernels.py`

 * *Files identical despite different names*

### Comparing `lunarsky-0.2.2/docs/figure.png` & `lunarsky-0.2.3/docs/figure.png`

 * *Files identical despite different names*

### Comparing `lunarsky-0.2.2/lunarsky/data/fk/satellites/moon_080317.tf` & `lunarsky-0.2.3/lunarsky/data/fk/satellites/moon_080317.tf`

 * *Files identical despite different names*

### Comparing `lunarsky-0.2.2/lunarsky/data/fk/satellites/moon_assoc_me.tf` & `lunarsky-0.2.3/lunarsky/data/fk/satellites/moon_assoc_me.tf`

 * *Files identical despite different names*

### Comparing `lunarsky-0.2.2/lunarsky/data/pck/moon_pa_de421_1900-2050.bpc` & `lunarsky-0.2.3/lunarsky/data/pck/moon_pa_de421_1900-2050.bpc`

 * *Files identical despite different names*

### Comparing `lunarsky-0.2.2/lunarsky/mcmf.py` & `lunarsky-0.2.3/lunarsky/mcmf.py`

 * *Files identical despite different names*

### Comparing `lunarsky-0.2.2/lunarsky/moon.py` & `lunarsky-0.2.3/lunarsky/moon.py`

 * *Files identical despite different names*

### Comparing `lunarsky-0.2.2/lunarsky/sky_coordinate.py` & `lunarsky-0.2.3/lunarsky/sky_coordinate.py`

 * *Files identical despite different names*

### Comparing `lunarsky-0.2.2/lunarsky/spice_utils.py` & `lunarsky-0.2.3/lunarsky/spice_utils.py`

 * *Files identical despite different names*

### Comparing `lunarsky-0.2.2/lunarsky/tests/conftest.py` & `lunarsky-0.2.3/lunarsky/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lunarsky-0.2.2/lunarsky/tests/test_moon.py` & `lunarsky-0.2.3/lunarsky/tests/test_moon.py`

 * *Files identical despite different names*

### Comparing `lunarsky-0.2.2/lunarsky/tests/test_sky_coordinate.py` & `lunarsky-0.2.3/lunarsky/tests/test_sky_coordinate.py`

 * *Files identical despite different names*

### Comparing `lunarsky-0.2.2/lunarsky/tests/test_spice.py` & `lunarsky-0.2.3/lunarsky/tests/test_spice.py`

 * *Files identical despite different names*

### Comparing `lunarsky-0.2.2/lunarsky/tests/test_time.py` & `lunarsky-0.2.3/lunarsky/tests/test_time.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 @pytest.mark.parametrize("lat", np.linspace(-89, 89, 5))
 @pytest.mark.parametrize("lon", np.linspace(0, 360, 5))
 def test_sidereal_time_calculation(lat, lon):
     # Confirm that the ra of the zenith is close to the calculated LST.
 
     t0 = Time.now()
     loc = MoonLocation.from_selenodetic(lon, lat, 0)
-    t0.location = loc
+    t0 = Time(t0, location=loc)
 
     Ntimes = 200
     Ndays = 28
     times = t0 + TimeDelta(np.linspace(0, Ndays, Ntimes) * 3600 * 24, format="sec")
 
     for tt in times:
         src = SkyCoord(alt="90d", az="0d", frame="lunartopo", obstime=tt, location=loc)
```

### Comparing `lunarsky-0.2.2/lunarsky/tests/test_transforms.py` & `lunarsky-0.2.3/lunarsky/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `lunarsky-0.2.2/lunarsky/time.py` & `lunarsky-0.2.3/lunarsky/time.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Extension of astropy's Time class."""
 
 import numpy as np
 import astropy
+from astropy import version
 from astropy.coordinates import EarthLocation, Longitude
 
 from .moon import MoonLocation
 import spiceypy as spice
 
 __all__ = ["Time", "TimeDelta"]
 
@@ -45,15 +46,19 @@
             in_subfmt=in_subfmt,
             out_subfmt=out_subfmt,
             location=super_loc,
             copy=copy,
         )
 
         if isinstance(location, MoonLocation):
-            self.location = location
+            if (version.major == 6 and version.minor >= 1) or version.major > 6:
+                # In astropy >= 6.1, time.Time.location is a property that shouldn't be set directly
+                self._location = location
+            else:
+                self.location = location
 
     def sidereal_time(self, kind, longitude=None, model=None):
         # Currently returns the zenith RA as the LST.
         if self.location is None or isinstance(self.location, EarthLocation):
             return super().sidereal_time(kind, longitude=longitude, model=model)
 
         if model is not None:
```

### Comparing `lunarsky-0.2.2/lunarsky/topo.py` & `lunarsky-0.2.3/lunarsky/topo.py`

 * *Files identical despite different names*

### Comparing `lunarsky-0.2.2/lunarsky.egg-info/PKG-INFO` & `lunarsky-0.2.3/lunarsky.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lunarsky
-Version: 0.2.2
+Version: 0.2.3
 Summary: Astropy support for selenocentric (Moon)reference frames and lunar surface observatories.
 Home-page: https://github.com/aelanman/lunarsky
 Download-URL: https://github.com/aelanman/lunarsky/archive/refs/tags/v0.1.1.tar.gz
 Author: Adam E. Lanman
 License: BSD
 Keywords: astronomy moon spice
 Classifier: Development Status :: 3 - Alpha
@@ -70,15 +70,15 @@
 The cartesian axes of the selenocentric system are those of the MCMF frame. In the selenodetic coordinates, "height" is defined relative to a sphere of radius 1737.1 km.
 * `SkyCoord` – A replacement for `astropy.coordinates.SkyCoord`, with modifications that ensure compatibility with the `MoonLocation` class.
 * `Time` – A replacement for the `astropy.time.Time` class, which can accept a `MoonLocation` instance as its location parameter, allowing for the calculation of local sidereal times on the Moon. The LST of an observer on the Moon is defined as the right ascension of the zenith.
 
 
 ## Credit
 
-This package makes use fo the ``spiceypy`` wrapper [2] for the JPl SPICE Toolkit, produced by the NASA Navigation and Ancillary Information Facility (NAIF) [3] [4]. The transformations are defined using data in kernel files ``pck/moon_pa_de421_1900-2050.bpc``, ``moon_080317.tf``, and ``moon_assoc_me.tf``. These may be found at [the NAIF website](https://naif.jpl.nasa.gov/pub/naif/generic_kernels), and were produced by Nat Bachman (NAIF/JPL) in March 2008. Further information may be found in the comments in these files in the `data` directory.
+This package makes use fo the ``spiceypy`` wrapper [2] for the JPL SPICE Toolkit, produced by the NASA Navigation and Ancillary Information Facility (NAIF) [3] [4]. The transformations are defined using data in kernel files ``pck/moon_pa_de421_1900-2050.bpc``, ``moon_080317.tf``, and ``moon_assoc_me.tf``. These may be found at [the NAIF website](https://naif.jpl.nasa.gov/pub/naif/generic_kernels), and were produced by Nat Bachman (NAIF/JPL) in March 2008. Further information may be found in the comments in these files in the `data` directory.
 
 ## References
 [1]: Ye, Hanlin, et al. "Looking Vector Direction Analysis for the Moon-Based Earth Observation Optical Sensor." IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing, vol. 11, no. 11, Nov. 2018, pp. 4488–99. IEEE Xplore, doi:10.1109/JSTARS.2018.2870247.
 
 [2]: Annex et al., (2020). SpiceyPy: a Pythonic Wrapper for the SPICE Toolkit. Journal of Open Source Software, 5(46), 2050, https://doi.org/10.21105/joss.02050
 
 [3]: Acton, C.H.; "Ancillary Data Services of NASA's Navigation and Ancillary Information Facility;" Planetary and Space Science, Vol. 44, No. 1, pp. 65-70, 1996.
```

### Comparing `lunarsky-0.2.2/lunarsky.egg-info/SOURCES.txt` & `lunarsky-0.2.3/lunarsky.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lunarsky-0.2.2/setup.py` & `lunarsky-0.2.3/setup.py`

 * *Files identical despite different names*

