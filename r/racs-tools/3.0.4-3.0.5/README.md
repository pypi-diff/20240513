# Comparing `tmp/racs_tools-3.0.4.tar.gz` & `tmp/racs_tools-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "racs_tools-3.0.4.tar", max compression
+gzip compressed data, was "racs_tools-3.0.5.tar", max compression
```

## Comparing `racs_tools-3.0.4.tar` & `racs_tools-3.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1520 2024-04-09 09:02:51.590263 racs_tools-3.0.4/LICENSE
--rw-r--r--   0        0        0     9511 2024-04-09 09:02:51.590263 racs_tools-3.0.4/README.md
--rw-r--r--   0        0        0      738 2024-04-09 09:02:51.590263 racs_tools-3.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-09 09:02:51.590263 racs_tools-3.0.4/racs_tools/__init__.py
--rw-r--r--   0        0        0     5027 2024-04-09 09:02:51.590263 racs_tools-3.0.4/racs_tools/au2.py
--rw-r--r--   0        0        0    24627 2024-04-09 09:02:51.590263 racs_tools-3.0.4/racs_tools/beamcon_2D.py
--rw-r--r--   0        0        0    46086 2024-04-09 09:02:51.590263 racs_tools-3.0.4/racs_tools/beamcon_3D.py
--rw-r--r--   0        0        0     5430 2024-04-09 09:02:51.590263 racs_tools-3.0.4/racs_tools/convolve_uv.py
--rw-r--r--   0        0        0     2709 2024-04-09 09:02:51.590263 racs_tools-3.0.4/racs_tools/gaussft.py
--rw-r--r--   0        0        0     8670 2024-04-09 09:02:51.590263 racs_tools-3.0.4/racs_tools/getnoise_list.py
--rw-r--r--   0        0        0     1038 2024-04-09 09:02:51.590263 racs_tools-3.0.4/racs_tools/logging.py
--rw-r--r--   0        0        0    10315 1970-01-01 00:00:00.000000 racs_tools-3.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1520 2024-05-13 09:43:00.321484 racs_tools-3.0.5/LICENSE
+-rw-r--r--   0        0        0     9511 2024-05-13 09:43:00.321484 racs_tools-3.0.5/README.md
+-rw-r--r--   0        0        0      738 2024-05-13 09:43:00.321484 racs_tools-3.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-13 09:43:00.321484 racs_tools-3.0.5/racs_tools/__init__.py
+-rw-r--r--   0        0        0     5027 2024-05-13 09:43:00.321484 racs_tools-3.0.5/racs_tools/au2.py
+-rw-r--r--   0        0        0    25217 2024-05-13 09:43:00.321484 racs_tools-3.0.5/racs_tools/beamcon_2D.py
+-rw-r--r--   0        0        0    46086 2024-05-13 09:43:00.321484 racs_tools-3.0.5/racs_tools/beamcon_3D.py
+-rw-r--r--   0        0        0     5430 2024-05-13 09:43:00.321484 racs_tools-3.0.5/racs_tools/convolve_uv.py
+-rw-r--r--   0        0        0     2709 2024-05-13 09:43:00.321484 racs_tools-3.0.5/racs_tools/gaussft.py
+-rw-r--r--   0        0        0     8670 2024-05-13 09:43:00.321484 racs_tools-3.0.5/racs_tools/getnoise_list.py
+-rw-r--r--   0        0        0     1038 2024-05-13 09:43:00.321484 racs_tools-3.0.5/racs_tools/logging.py
+-rw-r--r--   0        0        0    10315 1970-01-01 00:00:00.000000 racs_tools-3.0.5/PKG-INFO
```

### Comparing `racs_tools-3.0.4/LICENSE` & `racs_tools-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `racs_tools-3.0.4/README.md` & `racs_tools-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `racs_tools-3.0.4/pyproject.toml` & `racs_tools-3.0.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "racs-tools"
-version = "3.0.4"
+version = "3.0.5"
 description = "Useful scripts for RACS."
 authors = ["Alec Thomson"]
 license = "BSD"
 readme = "README.md"
 packages = [{include = "racs_tools"}]
 
 [tool.poetry.dependencies]
```

### Comparing `racs_tools-3.0.4/racs_tools/au2.py` & `racs_tools-3.0.5/racs_tools/au2.py`

 * *Files identical despite different names*

### Comparing `racs_tools-3.0.4/racs_tools/beamcon_2D.py` & `racs_tools-3.0.5/racs_tools/beamcon_2D.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,17 +100,20 @@
         fac = 1.0
         logger.warning(
             f"New beam {new_beam!r} and old beam {old_beam!r} are the same. Won't attempt convolution."
         )
         return conbm, fac
     try:
         conbm = new_beam.deconvolve(old_beam)
-    except Exception as err:
-        logger.warning(f"Could not deconvolve. New: {new_beam!r}, Old: {old_beam!r}")
-        raise err
+    except BeamError as err:
+        logger.error(err)
+        logger.warning(
+            f"Could not deconvolve. New: {new_beam!r}, Old: {old_beam!r} - will set convolving beam to 0.0"
+        )
+        conbm = new_beam.deconvolve(old_beam, failure_returns_pointlike=True)
     fac, amp, outbmaj, outbmin, outbpa = au2.gauss_factor(
         beamConv=[
             conbm.major.to(u.arcsec).value,
             conbm.minor.to(u.arcsec).value,
             conbm.pa.to(u.deg).value,
         ],
         beamOrig=[
@@ -362,15 +365,26 @@
     if not np.isclose(dx, dy):
         raise Exception("GRID MUST BE SAME IN X AND Y")
     grid = dy
     if conv_mode != "robust":
         # Get the minor axis of the convolving beams
         minorcons = []
         for beam in beams:
-            minorcons += [cmn_beam.deconvolve(beam).minor.to(u.arcsec).value]
+            try:
+                minorcons += [cmn_beam.deconvolve(beam).minor.to(u.arcsec).value]
+            except BeamError as err:
+                logger.error(err)
+                logger.warning(
+                    f"Could not deconvolve. New: {cmn_beam!r}, Old: {beam!r} - will set convolving beam to 0.0"
+                )
+                minorcons += [
+                    cmn_beam.deconvolve(beam, failure_returns_pointlike=True)
+                    .minor.to(u.arcsec)
+                    .value
+                ]
         minorcons = np.array(minorcons) * u.arcsec
         samps = minorcons / grid.to(u.arcsec)
         # Check that convolving beam will be Nyquist sampled
         if any(samps.value < 2):
             # Set the convolving beam to be Nyquist sampled
             nyq_con_beam = Beam(major=grid * 2, minor=grid * 2, pa=0 * u.deg)
             # Find new target based on common beam * Nyquist beam
```

### Comparing `racs_tools-3.0.4/racs_tools/beamcon_3D.py` & `racs_tools-3.0.5/racs_tools/beamcon_3D.py`

 * *Files identical despite different names*

### Comparing `racs_tools-3.0.4/racs_tools/convolve_uv.py` & `racs_tools-3.0.5/racs_tools/convolve_uv.py`

 * *Files identical despite different names*

### Comparing `racs_tools-3.0.4/racs_tools/gaussft.py` & `racs_tools-3.0.5/racs_tools/gaussft.py`

 * *Files identical despite different names*

### Comparing `racs_tools-3.0.4/racs_tools/getnoise_list.py` & `racs_tools-3.0.5/racs_tools/getnoise_list.py`

 * *Files identical despite different names*

### Comparing `racs_tools-3.0.4/racs_tools/logging.py` & `racs_tools-3.0.5/racs_tools/logging.py`

 * *Files identical despite different names*

### Comparing `racs_tools-3.0.4/PKG-INFO` & `racs_tools-3.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: racs-tools
-Version: 3.0.4
+Version: 3.0.5
 Summary: Useful scripts for RACS.
 License: BSD
 Author: Alec Thomson
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

