# Comparing `tmp/squishyplanet-0.1.1.tar.gz` & `tmp/squishyplanet-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squishyplanet-0.1.1.tar", last modified: Wed May  8 21:09:33 2024, max compression
+gzip compressed data, was "squishyplanet-0.1.2.tar", last modified: Mon May 13 16:29:11 2024, max compression
```

## Comparing `squishyplanet-0.1.1.tar` & `squishyplanet-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-08 21:09:33.197397 squishyplanet-0.1.1/
--rw-r--r--   0 cassese    (501) staff       (20)     1068 2024-03-11 14:22:30.000000 squishyplanet-0.1.1/LICENSE
--rw-r--r--   0 cassese    (501) staff       (20)     2582 2024-05-08 21:09:33.197166 squishyplanet-0.1.1/PKG-INFO
--rw-r--r--   0 cassese    (501) staff       (20)     1761 2024-05-02 22:19:44.000000 squishyplanet-0.1.1/README.md
--rw-r--r--   0 cassese    (501) staff       (20)     1094 2024-05-08 21:09:27.000000 squishyplanet-0.1.1/pyproject.toml
--rw-r--r--   0 cassese    (501) staff       (20)       38 2024-05-08 21:09:33.197439 squishyplanet-0.1.1/setup.cfg
--rw-r--r--   0 cassese    (501) staff       (20)       90 2024-04-20 21:39:16.000000 squishyplanet-0.1.1/setup.py
-drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-08 21:09:33.193449 squishyplanet-0.1.1/squishyplanet/
--rw-r--r--   0 cassese    (501) staff       (20)      233 2024-04-24 13:17:25.000000 squishyplanet-0.1.1/squishyplanet/__init__.py
-drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-08 21:09:33.195825 squishyplanet-0.1.1/squishyplanet/engine/
--rw-r--r--   0 cassese    (501) staff       (20)        0 2024-05-03 15:21:35.000000 squishyplanet-0.1.1/squishyplanet/engine/__init__.py
-drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-08 21:09:33.196481 squishyplanet-0.1.1/squishyplanet/engine/development/
--rw-r--r--   0 cassese    (501) staff       (20)     4637 2024-04-20 21:39:16.000000 squishyplanet-0.1.1/squishyplanet/engine/development/lambertian_reflectance.py
--rw-r--r--   0 cassese    (501) staff       (20)     9098 2024-04-20 21:39:16.000000 squishyplanet-0.1.1/squishyplanet/engine/development/quadratic_limb_darkened_transit.py
--rw-r--r--   0 cassese    (501) staff       (20)    44246 2024-04-20 21:39:16.000000 squishyplanet-0.1.1/squishyplanet/engine/development/terminator.py
--rw-r--r--   0 cassese    (501) staff       (20)     4383 2024-04-24 17:49:36.000000 squishyplanet-0.1.1/squishyplanet/engine/development/test_emission_normalization.py
--rw-r--r--   0 cassese    (501) staff       (20)     3273 2024-04-20 21:39:16.000000 squishyplanet-0.1.1/squishyplanet/engine/greens_basis_transform.py
--rw-r--r--   0 cassese    (501) staff       (20)     5153 2024-04-20 21:39:16.000000 squishyplanet-0.1.1/squishyplanet/engine/kepler.py
--rw-r--r--   0 cassese    (501) staff       (20)     6370 2024-04-26 22:30:04.000000 squishyplanet-0.1.1/squishyplanet/engine/parametric_ellipse.py
--rw-r--r--   0 cassese    (501) staff       (20)    55767 2024-05-06 18:56:11.000000 squishyplanet-0.1.1/squishyplanet/engine/phase_curve_utils.py
--rw-r--r--   0 cassese    (501) staff       (20)     3482 2024-04-20 21:39:16.000000 squishyplanet-0.1.1/squishyplanet/engine/planet_2d.py
--rw-r--r--   0 cassese    (501) staff       (20)    28523 2024-05-07 11:56:22.000000 squishyplanet-0.1.1/squishyplanet/engine/planet_3d.py
--rw-r--r--   0 cassese    (501) staff       (20)    24392 2024-05-08 21:07:53.000000 squishyplanet-0.1.1/squishyplanet/engine/polynomial_limb_darkened_transit.py
--rw-r--r--   0 cassese    (501) staff       (20)    51442 2024-05-08 21:07:53.000000 squishyplanet-0.1.1/squishyplanet/oblate_system.py
-drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-08 21:09:33.196942 squishyplanet-0.1.1/squishyplanet.egg-info/
--rw-r--r--   0 cassese    (501) staff       (20)     2582 2024-05-08 21:09:33.000000 squishyplanet-0.1.1/squishyplanet.egg-info/PKG-INFO
--rw-r--r--   0 cassese    (501) staff       (20)      910 2024-05-08 21:09:33.000000 squishyplanet-0.1.1/squishyplanet.egg-info/SOURCES.txt
--rw-r--r--   0 cassese    (501) staff       (20)        1 2024-05-08 21:09:33.000000 squishyplanet-0.1.1/squishyplanet.egg-info/dependency_links.txt
--rw-r--r--   0 cassese    (501) staff       (20)       75 2024-05-08 21:09:33.000000 squishyplanet-0.1.1/squishyplanet.egg-info/requires.txt
--rw-r--r--   0 cassese    (501) staff       (20)       14 2024-05-08 21:09:33.000000 squishyplanet-0.1.1/squishyplanet.egg-info/top_level.txt
-drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-08 21:09:33.196740 squishyplanet-0.1.1/tests/
--rw-r--r--   0 cassese    (501) staff       (20)     3962 2024-05-08 21:08:21.000000 squishyplanet-0.1.1/tests/test_against_jaxoplanet_transit.py
--rw-r--r--   0 cassese    (501) staff       (20)    10438 2024-05-08 21:07:53.000000 squishyplanet-0.1.1/tests/test_oblate_system.py
+drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-13 16:29:11.105810 squishyplanet-0.1.2/
+-rw-r--r--   0 cassese    (501) staff       (20)     1068 2024-03-11 14:22:30.000000 squishyplanet-0.1.2/LICENSE
+-rw-r--r--   0 cassese    (501) staff       (20)     2582 2024-05-13 16:29:11.105554 squishyplanet-0.1.2/PKG-INFO
+-rw-r--r--   0 cassese    (501) staff       (20)     1761 2024-05-02 22:19:44.000000 squishyplanet-0.1.2/README.md
+-rw-r--r--   0 cassese    (501) staff       (20)     1094 2024-05-13 16:14:20.000000 squishyplanet-0.1.2/pyproject.toml
+-rw-r--r--   0 cassese    (501) staff       (20)       38 2024-05-13 16:29:11.105851 squishyplanet-0.1.2/setup.cfg
+-rw-r--r--   0 cassese    (501) staff       (20)       90 2024-04-20 21:39:16.000000 squishyplanet-0.1.2/setup.py
+drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-13 16:29:11.101682 squishyplanet-0.1.2/squishyplanet/
+-rw-r--r--   0 cassese    (501) staff       (20)      233 2024-04-24 13:17:25.000000 squishyplanet-0.1.2/squishyplanet/__init__.py
+drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-13 16:29:11.103783 squishyplanet-0.1.2/squishyplanet/engine/
+-rw-r--r--   0 cassese    (501) staff       (20)        0 2024-05-03 15:21:35.000000 squishyplanet-0.1.2/squishyplanet/engine/__init__.py
+drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-13 16:29:11.104709 squishyplanet-0.1.2/squishyplanet/engine/development/
+-rw-r--r--   0 cassese    (501) staff       (20)     4637 2024-04-20 21:39:16.000000 squishyplanet-0.1.2/squishyplanet/engine/development/lambertian_reflectance.py
+-rw-r--r--   0 cassese    (501) staff       (20)     9098 2024-04-20 21:39:16.000000 squishyplanet-0.1.2/squishyplanet/engine/development/quadratic_limb_darkened_transit.py
+-rw-r--r--   0 cassese    (501) staff       (20)    44246 2024-04-20 21:39:16.000000 squishyplanet-0.1.2/squishyplanet/engine/development/terminator.py
+-rw-r--r--   0 cassese    (501) staff       (20)     4383 2024-04-24 17:49:36.000000 squishyplanet-0.1.2/squishyplanet/engine/development/test_emission_normalization.py
+-rw-r--r--   0 cassese    (501) staff       (20)     3273 2024-04-20 21:39:16.000000 squishyplanet-0.1.2/squishyplanet/engine/greens_basis_transform.py
+-rw-r--r--   0 cassese    (501) staff       (20)     5153 2024-04-20 21:39:16.000000 squishyplanet-0.1.2/squishyplanet/engine/kepler.py
+-rw-r--r--   0 cassese    (501) staff       (20)     6370 2024-04-26 22:30:04.000000 squishyplanet-0.1.2/squishyplanet/engine/parametric_ellipse.py
+-rw-r--r--   0 cassese    (501) staff       (20)    55767 2024-05-06 18:56:11.000000 squishyplanet-0.1.2/squishyplanet/engine/phase_curve_utils.py
+-rw-r--r--   0 cassese    (501) staff       (20)     3482 2024-04-20 21:39:16.000000 squishyplanet-0.1.2/squishyplanet/engine/planet_2d.py
+-rw-r--r--   0 cassese    (501) staff       (20)    28523 2024-05-07 11:56:22.000000 squishyplanet-0.1.2/squishyplanet/engine/planet_3d.py
+-rw-r--r--   0 cassese    (501) staff       (20)    24392 2024-05-08 21:07:53.000000 squishyplanet-0.1.2/squishyplanet/engine/polynomial_limb_darkened_transit.py
+-rw-r--r--   0 cassese    (501) staff       (20)    51686 2024-05-13 15:47:31.000000 squishyplanet-0.1.2/squishyplanet/oblate_system.py
+drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-13 16:29:11.105269 squishyplanet-0.1.2/squishyplanet.egg-info/
+-rw-r--r--   0 cassese    (501) staff       (20)     2582 2024-05-13 16:29:11.000000 squishyplanet-0.1.2/squishyplanet.egg-info/PKG-INFO
+-rw-r--r--   0 cassese    (501) staff       (20)      910 2024-05-13 16:29:11.000000 squishyplanet-0.1.2/squishyplanet.egg-info/SOURCES.txt
+-rw-r--r--   0 cassese    (501) staff       (20)        1 2024-05-13 16:29:11.000000 squishyplanet-0.1.2/squishyplanet.egg-info/dependency_links.txt
+-rw-r--r--   0 cassese    (501) staff       (20)       75 2024-05-13 16:29:11.000000 squishyplanet-0.1.2/squishyplanet.egg-info/requires.txt
+-rw-r--r--   0 cassese    (501) staff       (20)       14 2024-05-13 16:29:11.000000 squishyplanet-0.1.2/squishyplanet.egg-info/top_level.txt
+drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-13 16:29:11.105017 squishyplanet-0.1.2/tests/
+-rw-r--r--   0 cassese    (501) staff       (20)     3962 2024-05-08 21:08:21.000000 squishyplanet-0.1.2/tests/test_against_jaxoplanet_transit.py
+-rw-r--r--   0 cassese    (501) staff       (20)    10502 2024-05-13 16:09:31.000000 squishyplanet-0.1.2/tests/test_oblate_system.py
```

### Comparing `squishyplanet-0.1.1/LICENSE` & `squishyplanet-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.1.1/PKG-INFO` & `squishyplanet-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squishyplanet
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for dealing with non-spherical exoplanets
 Author-email: Ben Cassese <b.c.cassese@columbia.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/ben-cassese/squishyplanet
 Project-URL: Documentation, https://squishyplanet.readthedocs.io/en/latest/
 Keywords: astronomy,exoplanets
 Classifier: Programming Language :: Python
```

### Comparing `squishyplanet-0.1.1/README.md` & `squishyplanet-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.1.1/pyproject.toml` & `squishyplanet-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "squishyplanet"
-version = "0.1.1"
+version = "0.1.2"
 requires-python = ">=3.9"
 dependencies = [
     "requests",
     "jax",
     "jaxlib",
     "quadax",
     "tqdm",
```

### Comparing `squishyplanet-0.1.1/squishyplanet/engine/development/lambertian_reflectance.py` & `squishyplanet-0.1.2/squishyplanet/engine/development/lambertian_reflectance.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.1.1/squishyplanet/engine/development/quadratic_limb_darkened_transit.py` & `squishyplanet-0.1.2/squishyplanet/engine/development/quadratic_limb_darkened_transit.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.1.1/squishyplanet/engine/development/terminator.py` & `squishyplanet-0.1.2/squishyplanet/engine/development/terminator.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.1.1/squishyplanet/engine/development/test_emission_normalization.py` & `squishyplanet-0.1.2/squishyplanet/engine/development/test_emission_normalization.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.1.1/squishyplanet/engine/greens_basis_transform.py` & `squishyplanet-0.1.2/squishyplanet/engine/greens_basis_transform.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.1.1/squishyplanet/engine/kepler.py` & `squishyplanet-0.1.2/squishyplanet/engine/kepler.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.1.1/squishyplanet/engine/parametric_ellipse.py` & `squishyplanet-0.1.2/squishyplanet/engine/parametric_ellipse.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.1.1/squishyplanet/engine/phase_curve_utils.py` & `squishyplanet-0.1.2/squishyplanet/engine/phase_curve_utils.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.1.1/squishyplanet/engine/planet_2d.py` & `squishyplanet-0.1.2/squishyplanet/engine/planet_2d.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.1.1/squishyplanet/engine/planet_3d.py` & `squishyplanet-0.1.2/squishyplanet/engine/planet_3d.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.1.1/squishyplanet/engine/polynomial_limb_darkened_transit.py` & `squishyplanet-0.1.2/squishyplanet/engine/polynomial_limb_darkened_transit.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.1.1/squishyplanet/oblate_system.py` & `squishyplanet-0.1.2/squishyplanet/oblate_system.py`

 * *Files 1% similar despite different names*

```diff
@@ -938,14 +938,15 @@
                 }
             >>> system = OblateSystem(**state)
             >>> system.lightcurve()
 
         """
 
         return _lightcurve(
+            tidally_locked=self._state["tidally_locked"],
             compute_reflected_phase_curve=self._state["compute_reflected_phase_curve"],
             compute_emitted_phase_curve=self._state["compute_emitted_phase_curve"],
             compute_stellar_ellipsoidal_variations=self._state[
                 "compute_stellar_ellipsoidal_variations"
             ],
             compute_stellar_doppler_variations=self._state[
                 "compute_stellar_doppler_variations"
@@ -979,14 +980,15 @@
         Returns:
             float:
             The log likelihood of the system given the observed data and the
             provided parameters.
 
         """
         return _loglike(
+            tidally_locked=self._state["tidally_locked"],
             compute_reflected_phase_curve=self._state["compute_reflected_phase_curve"],
             compute_emitted_phase_curve=self._state["compute_emitted_phase_curve"],
             compute_stellar_ellipsoidal_variations=self._state[
                 "compute_stellar_ellipsoidal_variations"
             ],
             compute_stellar_doppler_variations=self._state[
                 "compute_stellar_doppler_variations"
@@ -1011,17 +1013,19 @@
         2,
         3,
         4,
         5,
         6,
         7,
         8,
+        9,
     ),
 )
 def _lightcurve(
+    tidally_locked,
     compute_reflected_phase_curve,
     compute_emitted_phase_curve,
     compute_stellar_ellipsoidal_variations,
     compute_stellar_doppler_variations,
     parameterize_with_projected_ellipse,
     oversample,
     random_seed,
@@ -1055,14 +1059,22 @@
 
     # generate the radii and thetas that you'll reuse at each timestep
     sample_radii, sample_thetas = generate_sample_radii_thetas(
         jax.random.key(random_seed),
         jnp.arange(phase_curve_nsamples),
     )
 
+    # solve Kepler's equation to get the true anomalies
+    time_deltas = state["times"] - state["t_peri"]
+    mean_anomalies = 2 * jnp.pi * time_deltas / state["period"]
+    true_anomalies = kepler(mean_anomalies, state["e"])
+    state["f"] = true_anomalies
+    if tidally_locked:
+        state["prec"] = state["f"]
+
     # technically these are all calculated in "transit", but since phase
     # curves are a) rare and b) expensive, we'll just do it again to keep
     # the transit section of the code more self-contained
     three = planet_3d_coeffs(**state)
     two = planet_2d_coeffs(**three)
     positions = skypos(**state)
     x_c = positions[0, :]
@@ -1121,29 +1133,24 @@
         reflected = 0.0
         emitted = 0.0
 
     ####################################################
     # compute the star's contribution to the phase curve
     ####################################################
 
-    if compute_stellar_ellipsoidal_variations | compute_stellar_doppler_variations:
-        time_deltas = state["times"] - state["t_peri"]
-        mean_anomalies = 2 * jnp.pi * time_deltas / state["period"]
-        true_anomalies = kepler(mean_anomalies, state["e"])
-
     if compute_stellar_ellipsoidal_variations:
         ellipsoidal = stellar_ellipsoidal_variations(
-            true_anomalies, state["stellar_ellipsoidal_alpha"], state["period"]
+            state["f"], state["stellar_ellipsoidal_alpha"], state["period"]
         )
     else:
         ellipsoidal = 0.0
 
     if compute_stellar_doppler_variations:
         doppler = stellar_doppler_variations(
-            true_anomalies, state["stellar_doppler_alpha"], state["period"]
+            state["f"], state["stellar_doppler_alpha"], state["period"]
         )
     else:
         doppler = 0.0
 
     ####################################################
     # put it all together
     ####################################################
@@ -1166,30 +1173,33 @@
         2,
         3,
         4,
         5,
         6,
         7,
         8,
+        9,
     ),
 )
 def _loglike(
+    tidally_locked,
     compute_reflected_phase_curve,
     compute_emitted_phase_curve,
     compute_stellar_ellipsoidal_variations,
     compute_stellar_doppler_variations,
     parameterize_with_projected_ellipse,
     oversample,
     random_seed,
     phase_curve_nsamples,
     extended_illumination_npts,
     state,
     params,
 ):
     lc = _lightcurve(
+        tidally_locked,
         compute_reflected_phase_curve,
         compute_emitted_phase_curve,
         compute_stellar_ellipsoidal_variations,
         compute_stellar_doppler_variations,
         parameterize_with_projected_ellipse,
         oversample,
         random_seed,
```

### Comparing `squishyplanet-0.1.1/squishyplanet.egg-info/PKG-INFO` & `squishyplanet-0.1.2/squishyplanet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squishyplanet
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for dealing with non-spherical exoplanets
 Author-email: Ben Cassese <b.c.cassese@columbia.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/ben-cassese/squishyplanet
 Project-URL: Documentation, https://squishyplanet.readthedocs.io/en/latest/
 Keywords: astronomy,exoplanets
 Classifier: Programming Language :: Python
```

### Comparing `squishyplanet-0.1.1/squishyplanet.egg-info/SOURCES.txt` & `squishyplanet-0.1.2/squishyplanet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.1.1/tests/test_against_jaxoplanet_transit.py` & `squishyplanet-0.1.2/tests/test_against_jaxoplanet_transit.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.1.1/tests/test_oblate_system.py` & `squishyplanet-0.1.2/tests/test_oblate_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,14 +204,17 @@
     state["parameterize_with_projected_ellipse"] = False
     state["tidally_locked"] = True
     state["compute_reflected_phase_curve"] = True
     state["compute_emitted_phase_curve"] = True
     state["compute_stellar_ellipsoidal_variations"] = True
     state["compute_stellar_doppler_variations"] = True
 
+    planet = OblateSystem(**state)
+    _ = planet.lightcurve()
+
     # for key, value in state.items():
     #     if (type(value) != int) & (type(value) != bool):
     #         if key in ["times", "data", "uncertainties", "exoposure_time"]:
     #             continue
     #         new_val = value + 0.01
     #         _ = planet.lightcurve({key: new_val})
```

