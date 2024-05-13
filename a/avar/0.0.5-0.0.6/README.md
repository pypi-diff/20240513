# Comparing `tmp/avar-0.0.5.tar.gz` & `tmp/avar-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avar-0.0.5.tar", last modified: Wed May  8 18:50:34 2024, max compression
+gzip compressed data, was "avar-0.0.6.tar", last modified: Mon May 13 21:25:52 2024, max compression
```

## Comparing `avar-0.0.5.tar` & `avar-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-08 18:50:34.613287 avar-0.0.5/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-18 11:26:07.000000 avar-0.0.5/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     3313 2024-05-08 18:50:34.613231 avar-0.0.5/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     2845 2024-05-08 18:50:14.000000 avar-0.0.5/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2024-04-18 11:26:07.000000 avar-0.0.5/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      576 2024-05-08 18:50:34.613516 avar-0.0.5/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-08 18:50:34.611225 avar-0.0.5/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-08 18:50:34.612292 avar-0.0.5/src/avar/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-04-18 11:28:55.000000 avar-0.0.5/src/avar/__init__.py
--rwxr-xr-x   0 davidwoodburn   (501) staff       (20)    12354 2024-05-08 18:48:30.000000 avar-0.0.5/src/avar/avar.py
--rwxr-xr-x   0 davidwoodburn   (501) staff       (20)      782 2024-05-08 16:11:36.000000 avar-0.0.5/src/avar/test_avar.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-08 18:50:34.613030 avar-0.0.5/src/avar.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     3313 2024-05-08 18:50:34.000000 avar-0.0.5/src/avar.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      265 2024-05-08 18:50:34.000000 avar-0.0.5/src/avar.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-08 18:50:34.000000 avar-0.0.5/src/avar.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       12 2024-05-08 18:50:34.000000 avar-0.0.5/src/avar.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        5 2024-05-08 18:50:34.000000 avar-0.0.5/src/avar.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-13 21:25:52.312694 avar-0.0.6/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-18 11:26:07.000000 avar-0.0.6/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     3675 2024-05-13 21:25:52.312617 avar-0.0.6/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     3207 2024-05-13 21:24:48.000000 avar-0.0.6/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2024-04-18 11:26:07.000000 avar-0.0.6/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      576 2024-05-13 21:25:52.312944 avar-0.0.6/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-13 21:25:52.310376 avar-0.0.6/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-13 21:25:52.311593 avar-0.0.6/src/avar/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-04-18 11:28:55.000000 avar-0.0.6/src/avar/__init__.py
+-rwxr-xr-x   0 davidwoodburn   (501) staff       (20)    15925 2024-05-13 21:08:45.000000 avar-0.0.6/src/avar/avar.py
+-rwxr-xr-x   0 davidwoodburn   (501) staff       (20)     1130 2024-05-13 21:07:17.000000 avar-0.0.6/src/avar/test_avar.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-13 21:25:52.312412 avar-0.0.6/src/avar.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     3675 2024-05-13 21:25:52.000000 avar-0.0.6/src/avar.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      265 2024-05-13 21:25:52.000000 avar-0.0.6/src/avar.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-13 21:25:52.000000 avar-0.0.6/src/avar.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       12 2024-05-13 21:25:52.000000 avar-0.0.6/src/avar.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        5 2024-05-13 21:25:52.000000 avar-0.0.6/src/avar.egg-info/top_level.txt
```

### Comparing `avar-0.0.5/LICENSE.txt` & `avar-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `avar-0.0.5/PKG-INFO` & `avar-0.0.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avar
-Version: 0.0.5
+Version: 0.0.6
 Summary: Allan variance tools
 Home-page: https://gitlab.com/davidwoodburn/avar
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -37,49 +37,65 @@
 supply the array of window sizes `M` for which to calculate the Allan variance
 values. This function can take for `y` either a one-dimensional array or a
 two-dimensional array in which each row will be treated as a data set.
 
 ## Ideal Allan Variance
 
 ```python
-avar.ideal(tau, vc, taub=None)
+avar.ideal(tau, p)
 ```
 
-Given a set of five component noise variances `vc`, you can calculate what the
-ideal Allan variances would be over an array of averaging periods `tau`. The
-five component noises are quantization, white, flicker, walk, and ramp. Any
-noise components you wish not to include, set their corresponding variances to
-zero. If you wish to treat flicker noise as an idealized, flat Allan variance
-over averaging period, leave the first-order, Gauss-Markov (FOGM) time constant,
-`taub`, as None. If you wish to treat the flicker noise as a FOGM noise, set the
-time constant to some non-zero value.
+The `ideal` function will calculate the ideal Allan variances over an array of
+averaging periods `tau`. For any noise components you wish not to be included,
+set their corresponding variances to zero.
+
+This function make use of the `params` class. Objects of this type store the
+five basic component noise variances (quantization, white, flicker, walk, and
+ramp), `vc`, any first-order, Gauss-Markov (FOGM) noise variances, `vfogm`, and
+the corresponding FOGM time constants, `tfogm`. The `p` parameter is one such
+object. You can define it as shown in the following example:
+
+```python
+p = avar.params(
+        vc=np.array([0.5, 1.0, 0, 0.5, 0.1]) * 1e-9,
+        vfogm=[1e-8, 1e-7],
+        tfogm=[0.1, 1.0])
+```
+
+The `ideal` function will return the total Allan variance curve, `va`, as well
+as a matrix, `vac`, whose rows represent the component Allan variances over
+`tau`.
 
 ## Fitting to Signal Allan Variance
 
 ```python
-avar.fit(tau, va, taub=None, mask=None, tol=0.007)
+avar.fit(tau, va, mask=None, fogms=0, tol=0.007)
 ```
 
 Given the Allan variance curve of some signal, `va`, at various averaging
-periods `tau`, you can get the best fit using the five component noises. As with
-the `ideal` function, if `taub` is left undefined, the flicker noise will be
-treated as the idealized, flat Allan variance over averaging period. Otherwise,
-the flicker noise will be treated as a first-order, Gauss-Markov noise. By
-default, this function will automatically attempt to determine if certain
-component noises are even at play based on the tolerance value `tol`. However,
-you can directly control which component noises you wish to include or exclude
-with the `mask` array. For each element of `mask` that is `False` the
-corresponding component noise will be excluded.
+periods `tau`, you can get the best fit using the five basic component noises
+and `fogms` number of first-order, Gauss-Markov (FOGM) noises. By default, this
+function will automatically attempt to determine if certain component noises are
+even at play based on the tolerance value `tol`. However, you can directly
+control which component noises you wish to include or exclude with the `mask`
+array. For each element of `mask` that is `False` the corresponding component
+noise will be excluded. This function will iterate through the various
+permutations of component noises, starting with 0 FOGMs. If a fit satisfies the
+specified `tol` tolerance, the search will end. Otherwise, the best fit will be
+used.
+
+The return values are the fitted Allan variance curve, `vf`, and a `params`
+object, `p` (see the section on Ideal Allan Variance), containing the variances
+of the basic component noise variances (quantization, white, flicker, walk, and
+ramp), `vc`, any first-order, Gauss-Markov (FOGM) noise variances, `vfogm`, and
+the corresponding FOGM time constants, `tfogm`.
 
 ## Noise Generation
 
 ```python
-avar.noise(vc, K, T, taub=None)
+avar.noise(K, T, p)
 ```
 
-Given a five-element array of component noise variances `vc`, you can create an
-artificially-generated noise signal of length `K` and sampling period `T`. Each
-element of `vc` corresponds to one of the five component noise types:
-quantization, white, flicker, walk, and ramp. As with the `ideal` function, if
-`taub` is left undefined, the flicker noise will be treated as the idealized,
-flat Allan variance over averaging period. Otherwise, the flicker noise will be
-treated as a first-order, Gauss-Markov noise.
+Generate a noise signal of length `K`, sampling period `T`, and parameters `p`.
+Parameter `p` is a `params` object (see the section on Ideal Allan Variance).
+
+This function returns the noise signal `y`.
```

### Comparing `avar-0.0.5/README.md` & `avar-0.0.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -21,49 +21,65 @@
 supply the array of window sizes `M` for which to calculate the Allan variance
 values. This function can take for `y` either a one-dimensional array or a
 two-dimensional array in which each row will be treated as a data set.
 
 ## Ideal Allan Variance
 
 ```python
-avar.ideal(tau, vc, taub=None)
+avar.ideal(tau, p)
 ```
 
-Given a set of five component noise variances `vc`, you can calculate what the
-ideal Allan variances would be over an array of averaging periods `tau`. The
-five component noises are quantization, white, flicker, walk, and ramp. Any
-noise components you wish not to include, set their corresponding variances to
-zero. If you wish to treat flicker noise as an idealized, flat Allan variance
-over averaging period, leave the first-order, Gauss-Markov (FOGM) time constant,
-`taub`, as None. If you wish to treat the flicker noise as a FOGM noise, set the
-time constant to some non-zero value.
+The `ideal` function will calculate the ideal Allan variances over an array of
+averaging periods `tau`. For any noise components you wish not to be included,
+set their corresponding variances to zero.
+
+This function make use of the `params` class. Objects of this type store the
+five basic component noise variances (quantization, white, flicker, walk, and
+ramp), `vc`, any first-order, Gauss-Markov (FOGM) noise variances, `vfogm`, and
+the corresponding FOGM time constants, `tfogm`. The `p` parameter is one such
+object. You can define it as shown in the following example:
+
+```python
+p = avar.params(
+        vc=np.array([0.5, 1.0, 0, 0.5, 0.1]) * 1e-9,
+        vfogm=[1e-8, 1e-7],
+        tfogm=[0.1, 1.0])
+```
+
+The `ideal` function will return the total Allan variance curve, `va`, as well
+as a matrix, `vac`, whose rows represent the component Allan variances over
+`tau`.
 
 ## Fitting to Signal Allan Variance
 
 ```python
-avar.fit(tau, va, taub=None, mask=None, tol=0.007)
+avar.fit(tau, va, mask=None, fogms=0, tol=0.007)
 ```
 
 Given the Allan variance curve of some signal, `va`, at various averaging
-periods `tau`, you can get the best fit using the five component noises. As with
-the `ideal` function, if `taub` is left undefined, the flicker noise will be
-treated as the idealized, flat Allan variance over averaging period. Otherwise,
-the flicker noise will be treated as a first-order, Gauss-Markov noise. By
-default, this function will automatically attempt to determine if certain
-component noises are even at play based on the tolerance value `tol`. However,
-you can directly control which component noises you wish to include or exclude
-with the `mask` array. For each element of `mask` that is `False` the
-corresponding component noise will be excluded.
+periods `tau`, you can get the best fit using the five basic component noises
+and `fogms` number of first-order, Gauss-Markov (FOGM) noises. By default, this
+function will automatically attempt to determine if certain component noises are
+even at play based on the tolerance value `tol`. However, you can directly
+control which component noises you wish to include or exclude with the `mask`
+array. For each element of `mask` that is `False` the corresponding component
+noise will be excluded. This function will iterate through the various
+permutations of component noises, starting with 0 FOGMs. If a fit satisfies the
+specified `tol` tolerance, the search will end. Otherwise, the best fit will be
+used.
+
+The return values are the fitted Allan variance curve, `vf`, and a `params`
+object, `p` (see the section on Ideal Allan Variance), containing the variances
+of the basic component noise variances (quantization, white, flicker, walk, and
+ramp), `vc`, any first-order, Gauss-Markov (FOGM) noise variances, `vfogm`, and
+the corresponding FOGM time constants, `tfogm`.
 
 ## Noise Generation
 
 ```python
-avar.noise(vc, K, T, taub=None)
+avar.noise(K, T, p)
 ```
 
-Given a five-element array of component noise variances `vc`, you can create an
-artificially-generated noise signal of length `K` and sampling period `T`. Each
-element of `vc` corresponds to one of the five component noise types:
-quantization, white, flicker, walk, and ramp. As with the `ideal` function, if
-`taub` is left undefined, the flicker noise will be treated as the idealized,
-flat Allan variance over averaging period. Otherwise, the flicker noise will be
-treated as a first-order, Gauss-Markov noise.
+Generate a noise signal of length `K`, sampling period `T`, and parameters `p`.
+Parameter `p` is a `params` object (see the section on Ideal Allan Variance).
+
+This function returns the noise signal `y`.
```

### Comparing `avar-0.0.5/setup.cfg` & `avar-0.0.6/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = avar
-version = 0.0.5
+version = 0.0.6
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = Allan variance tools
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/avar
 classifiers =
```

### Comparing `avar-0.0.5/src/avar/avar.py` & `avar-0.0.6/src/avar/avar.py`

 * *Files 27% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 __maintainer__ = "David Woodburn"
 __email__ = "david.woodburn@icloud.com"
 __status__ = "Development"
 
 import numpy as np
 import scipy.optimize as opt
 
-
 def windows(K, density=64):
     """
     Build an array of averaging window sizes for Allan variances analysis.
 
     Parameters
     ----------
     K : int
@@ -98,207 +97,334 @@
             yj = y[:, :(1 - 2*m)] # Beginning
             delta = (Yc - 2*Yb + Yj - yj)/m
             v[:, n_tau] = np.mean(delta**2, axis=1)/2
 
     return v
 
 
-def ideal(tau, vc, taub=None):
+class params:
+    def __init__(self, vc, vfogm=None, tfogm=None):
+        """
+        Parameters
+        ----------
+        vc : (5,) np.ndarray
+            Variances of the five basic component noises: quantization, white,
+            flicker, walk, and ramp. If `fogms` is not 0, the third element of `vc`
+            will be zero. For any elements of `mask` which are `False`, the
+            corresponding elements of `vc` will be zero.
+        vfogm : (F,) np.ndarray, default None
+            Array of FOGM variances.
+        tfogm : (F,) np.ndarray, default None
+            Array of FOGM time constants (s).
+        """
+
+        # Convert lists and tuples to arrays.
+        if isinstance(vc, (list, tuple)):
+            vc = np.array(vc)
+        if len(vc) != 5:
+            raise ValueError("vc should be a 5-element array.")
+        if isinstance(vfogm, (list, tuple)):
+            vfogm = np.array(vfogm, dtype=float)
+        elif isinstance(vfogm, (int, float)):
+            vfogm = np.array([vfogm], dtype=float)
+        if isinstance(tfogm, (list, tuple)):
+            tfogm = np.array(tfogm, dtype=float)
+        elif isinstance(tfogm, (int, float)):
+            tfogm = np.array([tfogm], dtype=float)
+
+        # Get the number of FOGMs.
+        self.F = 0 if vfogm is None else len(vfogm)
+        
+        # Save the arrays.
+        self.vc = vc
+        self.vfogm = vfogm
+        self.tfogm = tfogm
+
+
+def ideal(tau, p):
     """
     Generate an ideal Allan variance curve given the component variances.
 
     Parameters
     ----------
     tau : (I,) np.ndarray
         Array of averaging periods (s).
-    vc : (5,) np.ndarray
-        Component variances: quantization, white, flicker, walk, and ramp.
-    taub : float, default None
-        The time constant of the first-order, Gauss-Markov noise. If it is
-        `None` then a constant-amplitude Allan variance curve is used.
+    p : params object
+        Object defining the variances and time constants of the noise.
 
     Returns
     -------
     va : (I,) np.ndarray
-        Array of ideal Allan variances.
-    va_comps : (5, I) np.ndarray
-        Matrix of the 5 ideal Allan variance components.
+        Array of the ideal sum of component Allan variances.
+    vac : (5+F, I) np.ndarray
+        Matrix of the component Allan variances. `F` is the number of
+        first-order, Gauss-Markov noise components.
     """
 
-    # Get the flicker Allan variance.
-    if (taub is None) or (taub == 0.0):
-        flkr = (2*np.log(2))/np.pi + 0*tau
-    else:
-        p = np.exp(-tau[0]/taub)
-        M = tau/tau[0]
-        flkr = 1.0/M**2*(M*(1 - p)**2 + 2*p*M*(1 - p) - 2*p*(1 - p**M)
-            - p*(1 - p**M)**2)/(1 - p)**2
-
-    # Build the total Allan variance.
-    va_comps = np.array([vc[0]*3/(tau**2), vc[1]*1/tau,
-        vc[2]*flkr, vc[3]*tau/3, vc[4]*(tau**2)/2])
-    va = np.sum(va_comps, axis=0)
+    # Define the basic component noise Allan variances.
+    vac = np.zeros((5 + p.F, len(tau)))
+    vac[0, :] = p.vc[0] * 3/(tau**2)
+    vac[1, :] = p.vc[1] * 1/tau
+    vac[2, :] = p.vc[2] * 2*np.log(2)/np.pi + 0*tau
+    vac[3, :] = p.vc[3] * tau/3
+    vac[4, :] = p.vc[4] * (tau**2)/2
+
+    # Include any FOGMs.
+    if p.F != 0:
+        T = tau[0]
+        M = tau/T
+    for f in range(p.F):
+        q = np.exp(-T/p.tfogm[f])
+        vac[5 + f, :] = (p.vfogm[f]/M**2)*(M*(1 - q)**2 + 2*q*M*(1 - q)
+                - 2*q*(1 - q**M) - q*(1 - q**M)**2)/(1 - q)**2
+
+    # Sum the component Allan variances.
+    va = np.sum(vac, axis=0)
+
+    return va, vac
+
+
+class fit_metrics:
+    n = 0
+    nmae = None
+    mask = None
+    fogm = None
+
+    def init(N):
+        fit_metrics.n = 0
+        fit_metrics.nmae = np.zeros(N)
+        fit_metrics.mask = np.zeros(N)
+        fit_metrics.fogm = np.zeros(N)
+
+    def append(nmae, mask, fogm):
+        fit_metrics.nmae[fit_metrics.n] = nmae
+        fit_metrics.mask[fit_metrics.n] = mask
+        fit_metrics.fogm[fit_metrics.n] = fogm
+        fit_metrics.n += 1
+
+    def trim():
+        fit_metrics.nmae = fit_metrics.nmae[:fit_metrics.n]
+        fit_metrics.mask = fit_metrics.mask[:fit_metrics.n]
+        fit_metrics.fogm = fit_metrics.fogm[:fit_metrics.n]
 
-    return va, va_comps
 
-
-def fit(tau, va, taub=None, mask=None, tol=0.007):
+def fit(tau, va, mask=None, fogms=0, tol=0.007):
     """
-    Fit component variances to an Allan variance curve.
+    Fit component variances to a single Allan variance curve.
 
     Parameters
     ----------
     tau : (I,) np.ndarray
         Array of averaging periods (s).
-    va : (I,) or (J, I) np.ndarray
-        Array of Allan variances or matrix of rows of such arrays.
-    taub : float, default None
-        The time constant of the first-order, Gauss-Markov noise. If it is
-        `None` then a constant-amplitude Allan variance curve is used.
+    va : (I,) np.ndarray
+        Array of Allan variances.
     mask : (5,) bool array_like, default None
-        Array to mask which component variances to use. If it is `None`, then no
-        mask will be applied. When it is not `None`, the function will still
-        return an array of 5 values for `vc`, but the values corresponding to
-        `False` or `0` should be `0`.
+        Array to mask which component variances to use. Left as `None`, no basic
+        component variances will be excluded. However, a positive value for
+        `fogms` will override the third element of the mask, regardless of
+        whether it is `True` or `False`.
+    fogms : int, default 0
+        The maximum number of first-order, Gauss-Markov (FOGM) noise components
+        to try to fit to the data. This is the maximum number, not the required
+        number. The best fit might not use any.
     tol : float, default 0.007
         Normalized mean absolute error tolerance to meet as various combinations
         of the component noises are applied to the fitting.
 
     Returns
     -------
     vf : (I,) np.ndarray
         Fitted Allan variance curve.
-    vc : (5,) np.ndarray
-        Component variances: quantization, white, flicker, walk, and ramp.
+    p : params object
+        Object defining the variances and time constants of the noise.
 
     Notes
     -----
-    Fit using non-negative least squares solver. It is better to normalize the
-    `H` matrix by the `va` vector this way because it produces better results
-    than fitting with `opt.nnls(H, va)[0]`.
+    This function will iterate through the various permutations of component
+    noises, starting with 0 FOGMs. If a fit satisfies the specified `tol`, the
+    search will end. Otherwise, the best fit will be used.
     """
 
-    # Get the flicker Allan variance based on whether a FOGM tau was given.
-    if taub is None:
-        flkr = 2*np.log(2)/np.pi + 0*tau
-    else:
-        p = np.exp(-tau[0]/taub)
-        M = tau/tau[0]
-        flkr = 1.0/M**2*(M*(1 - p)**2 + 2*p*M*(1 - p) - 2*p*(1 - p**M)
-            - p*(1 - p**M)**2)/(1 - p)**2
+    def fopt(k, H, M, T, va):
+        """
+        Parameters
+        ----------
+        k : (B + 2*F,) np.ndarray
+            Array of variables to tune for, starting with some `B` basic noise
+            component variances followed by `F` pairs of FOGM variances and time
+            constants.
+        H : (I, B) np.ndarray
+            Matrix of functions of the averaging period.
+        M : (I,) np.ndarray
+            Array of averaging window sizes.
+        T : float
+            Sampling period.
+        va : (I,) np.ndarray
+            Array of Allan variances to fit.
+        """
+
+        # Get the number of basic components and FOGM components.
+        B = H.shape[1]
+        F = (len(k) - B)//2
+
+        # Initialize the normalized fit with the basic components.
+        vfn = H/va[:, None] @ np.abs(k[:B])
+
+        # Add to the fit each of the FOGM components.
+        for f in range(F):
+            v = abs(k[B + 2*f])
+            t = abs(k[B + 2*f + 1])
+            q = np.exp(-T/t)
+            vfn += (1/va)*(v/M**2)*(M*(1 - q)**2 + 2*q*M*(1 - q)
+                    - 2*q*(1 - q**M) - q*(1 - q**M)**2)/(1 - q)**2
+
+        return vfn - 1
+
+    # Adjust the mask.
+    if mask is None:
+        mask = np.ones(5, dtype=bool)
+    if isinstance(mask, (list, tuple)):
+        mask = np.array(mask, dtype=bool)
+    if fogms > 0:
+        mask[2] = False
 
-    # Build the other component Allan variance factors.
+    # Build the basic component Allan variances.
     qnt = 3/(tau**2)
     wht = 1/tau
+    flk = 2*np.log(2)/np.pi + 0*tau
     bwn = tau/3
     rmp = (tau**2)/2
+    H5 = np.array([qnt, wht, flk, bwn, rmp]).T
+    H = H5[:, mask]
 
-    # Assemble the full, normalized Allan variance factor matrix.
-    H_full = np.array([qnt, wht, flkr, bwn, rmp]).T
+    # Get the dimensions.
+    B = H.shape[1] # number of basic components to consider
 
-    # Get size of va.
-    if np.ndim(va) == 1:
-        J = 0
-        I = len(va)
-    else:
-        J, I = va.shape
+    # Get the range of averaging periods.
+    T = tau[0] # sampling period
+    talg = np.log10(T)
+    tblg = np.log10(tau[-1])
+
+    # Define the reused arrays.
+    I = len(va)
+    OI = np.ones(I)
+    M = tau/T # averaging window sizes
+
+    # Initialize the outputs.
+    vf = np.zeros(I)
+    p = params(np.zeros(5), np.zeros(fogms), np.zeros(fogms))
+
+    # Define the NMAE components.
+    va_lg = np.log10(va)
+    range_lg = np.max(va_lg) - np.min(va_lg)
+    nmae_min = np.inf
+
+    # Initialize the metrics
+    fit_metrics.init((2**B - 1)*(fogms + 1))
 
     # Estimate the component variances.
-    if (mask is not None) and (len(mask) == 5) and (np.sum(mask) < 5):
-        H = H_full[:, mask]
-        N = H.shape[1] # number of components to consider
-        if J == 0:
-            vcp = opt.nnls(H/va[:, None], np.ones(len(tau)))[0]
-            vf = H @ vcp # fitted Allan variance
-            vc = np.zeros(5) # complete array of component variances
-            vc[mask] = vcp # copy into the appropriate places
-        else:
-            vc = np.zeros((J, 5)) # complete array of component variances
-            vf = np.zeros((J, I))
-            for j in range(J):
-                vcp = opt.nnls(H/va[j:j+1].T, np.ones(len(tau)))[0]
-                vf[j] = H @ vcp # fitted Allan variance
-                vc[j, mask] = vcp # copy into the appropriate places
-    else:
-        valg = np.log10(va)
-        span = np.max(valg, axis=-1) - np.min(valg, axis=-1)
-        mask_values = np.concatenate((np.arange(15)*2 + 2, np.arange(16)*2 + 1))
-        if J == 0:
-            vc = np.zeros(5) # complete array of component variances
-            vf = np.zeros(I) # fitted Allan variance
-            nmae_min = np.inf # minimum normalized mean absolute error
-            for m in mask_values:
-                mask = [bool((m >> i) & 1) for i in range(5)]
-                H = H_full[:, mask]
-                try:
-                    vcp = opt.nnls(H/va[:, None], np.ones(len(tau)))[0]
+    for F in range(fogms + 1): # the number of possible FOGMs
+        # Define the starting mask value. Allow for no basic components
+        # if the number of FOGMs is nonzero.
+        m = 1 if F == 0 else 0
+
+        # For each mask value,
+        for mask_value in range(m, 2**B): # the basic mask value
+            # Get the H matrix for this permutation.
+            maskp = [bool((mask_value >> i) & 1) for i in range(B)]
+            Hp = H[:, maskp]
+            Bp = Hp.shape[1] # number of components to consider
+
+            # Optimize for this permutation.
+            if F == 0: # no FOGMs
+                try: # This can fail.
+                    k = opt.nnls(Hp/va[:, None], OI)[0]
+                except ValueError or RuntimeError:
+                    continue
+                # Get the fitted Allan variance.
+                vfp = Hp @ k
+            else: # some FOGMs
+                try: # This can fail.
+                    # Initialize the parameters, spacing out the FOGM time
+                    # constants.
+                    k = np.ones(Bp + 2*F)
+                    k[Bp + 1::2] = np.logspace(talg, tblg, F + 2)[1:-1]
+                    # Optimize.
+                    k = np.abs(opt.leastsq(fopt, k,
+                            args=(Hp, M, T, va), maxfev=1000)[0])
                 except ValueError or RuntimeError:
                     continue
-                vfp = H @ vcp # fitted Allan variance
-                er = valg - np.log10(vfp)
-                nmae = np.mean(np.abs(er))/span
-                if nmae < nmae_min: # save the best
-                    nmae_min = nmae
-                    vf = vfp.copy() # save this fitted Allan variance
-                    vc[mask] = vcp # copy into the appropriate places
-                if nmae < tol: # quit early
-                    break
-        else:
-            vc = np.zeros((J, 5))
-            vf = np.zeros((J, I))
-            for j in range(J):
-                nmae_min = np.inf # minimum normalized mean absolute error
-                for m in mask_values:
-                    mask = [bool((m >> i) & 1) for i in range(5)]
-                    H = H_full[:, mask]
-                    try:
-                        vcp = opt.nnls(H/va[j:j+1].T, np.ones(len(tau)))[0]
-                    except ValueError or RuntimeError:
-                        continue
-                    vfp = H @ vcp # fitted Allan variance
-                    er = valg[j] - np.log10(vfp)
-                    nmae = np.mean(np.abs(er))/span[j]
-                    if nmae < nmae_min: # save the best
-                        nmae_min = nmae
-                        vf[j] = vfp.copy() # save this fitted Allan variance
-                        vc[j, mask] = vcp # copy into the appropriate places
-                    if nmae < tol: # quit early
-                        break
+                # Get the fitted Allan variance.
+                vfp = Hp @ np.abs(k[:Bp])
+                for f in range(F):
+                    v = abs(k[Bp + 2*f])
+                    t = abs(k[Bp + 2*f + 1])
+                    q = np.exp(-T/t)
+                    vfp += (v/M**2)*(M*(1 - q)**2 + 2*q*M*(1 - q)
+                            - 2*q*(1 - q**M) - q*(1 - q**M)**2)/(1 - q)**2
+
+            # Evaluate the fit.
+            er = va_lg - np.log10(vfp)
+            nmae = np.mean(np.abs(er))/range_lg
+            if nmae < nmae_min: # save the best
+                # Track the minimum error.
+                nmae_min = nmae
+
+                # Save the metrics.
+                fit_metrics.append(nmae, mask_value, F)
+
+                # Save this fitted Allan variance.
+                vf = vfp 
+
+                # Save the basic component variances.
+                vcp = np.zeros(B)
+                vcp[maskp] = k[:Bp]
+                p.vc[mask] = vcp
+
+                if F > 0:
+                    p.vfogm[:F] = k[Bp::2]
+                    p.tfogm[:F] = k[Bp + 1::2]
+            if nmae < tol: # quit early
+                break
+
+    # Save the number of FOGMs estimated.
+    p.F = F
 
-    return vf, vc
+    # Trim the fit metrics.
+    fit_metrics.trim()
 
+    return vf, p
 
-def noise(vc, K, T, taub=None):
+
+def noise(K, T, p):
     """
-    Generate noise using the 5 component variances of the Allan variance
-    analysis. The component noises are generated as the following:
+    Generate noise using the 5 basic component noise variances of the Allan
+    variance analysis and any first-order, Gauss-Markov (FOGM) noises specified.
+    The basic component noises are generated as the following:
 
         Type            Implementation
         ------------    ---------------------------------------
         quantization    differentiated white, Gaussian noise
         white           white, Gaussian noise
         flicker         first-order, Gauss-Markov (FOGM) noise
         walk            integrated white, Gaussian noise
         ramp            doubly integrated white, Gaussian noise
 
     Parameters
     ----------
-    vc : (5,) np.ndarray
-        Component variances: quantization, white, flicker, walk, and ramp.
     K : int
         Number of samples.
     T : float
         Sampling period (s).
-    taub : float, default None
-        The time constant of the FOGM noise (s). If it is None, it will default
-        to the `T sqrt(K/2)`.
+    p : params object
+        Object defining the variances and time constants of the noise.
 
     Returns
     -------
-    n : (K,) np.ndarray
+    y : (K,) np.ndarray
         Array of noise values over time.
 
     Notes
     -----
     Vectorizing this function to generate multiple rows of noise data does not
     actually improve the computation time above calling this function within a
     loop.
@@ -312,42 +438,50 @@
     ally, not analytically, derived. However, given their simplicity (`1` and
     `sqrt(2)`, respectively) and the very small errors between the average Allan
     variance curves of 10 thousand Monte-Carlo samples of noise and the ideal
     Allan variance curve, it seems they are correct.
     """
 
     # Initialize the noise array.
-    n = np.zeros(K)
+    y = np.zeros(K)
 
     # Quantization noise
-    if vc[0] != 0:
+    if p.vc[0] != 0:
         w = np.random.randn(K + 1)
-        n += np.sqrt(vc[0])*np.diff(w)/T
+        y += np.sqrt(p.vc[0])*np.diff(w)/T
 
     # White noise
-    if vc[1] != 0:
+    if p.vc[1] != 0:
         w = np.random.randn(K)
-        n += np.sqrt(vc[1]/T)*w
+        y += np.sqrt(p.vc[1]/T)*w
 
     # Bias instability (flicker)
-    if vc[2] != 0:
-        if taub is None:
-            taub = T*np.sqrt(K/2)
-        ka = np.exp(-T/taub)
-        kb = np.sqrt(vc[2]*(1 - np.exp(-2*T/taub)))
-        eta = kb*np.random.randn(K)
-        x = np.sqrt(vc[2])*np.random.randn() # state
-        for k in range(K):
-            n[k] += x
-            x = ka*x + eta[k]
+    #if p.vc[2] != 0:
+    #    ka = np.exp(-T/taub)
+    #    kb = np.sqrt(p.vc[2]*(1 - np.exp(-2*T/taub)))
+    #    eta = kb*np.random.randn(K)
+    #    x = np.sqrt(p.vc[2])*np.random.randn() # state
+    #    for k in range(K):
+    #        y[k] += x
+    #        x = ka*x + eta[k]
 
     # Random walk noise
-    if vc[3] != 0:
+    if p.vc[3] != 0:
         w = np.random.randn(K)
-        n += np.cumsum(np.sqrt(vc[3]*T)*w)
+        y += np.cumsum(np.sqrt(p.vc[3]*T)*w)
 
     # Ramp noise
-    if vc[4] != 0:
-        eta = np.sqrt(2*vc[4]/K) * T * np.random.randn(K)
-        n += np.cumsum(np.cumsum(eta))
+    if p.vc[4] != 0:
+        eta = np.sqrt(2*p.vc[4]/K) * T * np.random.randn(K)
+        y += np.cumsum(np.cumsum(eta))
+
+    # FOGM noises
+    for f in range(p.F):
+        ka = np.exp(-T/p.tfogm[f])
+        kb = np.sqrt(p.vfogm[f]*(1 - np.exp(-2*T/p.tfogm[f])))
+        eta = kb*np.random.randn(K)
+        x = np.sqrt(p.vfogm[f])*np.random.randn() # state
+        for k in range(K):
+            y[k] += x
+            x = ka*x + eta[k]
 
-    return n
+    return y
```

### Comparing `avar-0.0.5/src/avar.egg-info/PKG-INFO` & `avar-0.0.6/src/avar.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avar
-Version: 0.0.5
+Version: 0.0.6
 Summary: Allan variance tools
 Home-page: https://gitlab.com/davidwoodburn/avar
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -37,49 +37,65 @@
 supply the array of window sizes `M` for which to calculate the Allan variance
 values. This function can take for `y` either a one-dimensional array or a
 two-dimensional array in which each row will be treated as a data set.
 
 ## Ideal Allan Variance
 
 ```python
-avar.ideal(tau, vc, taub=None)
+avar.ideal(tau, p)
 ```
 
-Given a set of five component noise variances `vc`, you can calculate what the
-ideal Allan variances would be over an array of averaging periods `tau`. The
-five component noises are quantization, white, flicker, walk, and ramp. Any
-noise components you wish not to include, set their corresponding variances to
-zero. If you wish to treat flicker noise as an idealized, flat Allan variance
-over averaging period, leave the first-order, Gauss-Markov (FOGM) time constant,
-`taub`, as None. If you wish to treat the flicker noise as a FOGM noise, set the
-time constant to some non-zero value.
+The `ideal` function will calculate the ideal Allan variances over an array of
+averaging periods `tau`. For any noise components you wish not to be included,
+set their corresponding variances to zero.
+
+This function make use of the `params` class. Objects of this type store the
+five basic component noise variances (quantization, white, flicker, walk, and
+ramp), `vc`, any first-order, Gauss-Markov (FOGM) noise variances, `vfogm`, and
+the corresponding FOGM time constants, `tfogm`. The `p` parameter is one such
+object. You can define it as shown in the following example:
+
+```python
+p = avar.params(
+        vc=np.array([0.5, 1.0, 0, 0.5, 0.1]) * 1e-9,
+        vfogm=[1e-8, 1e-7],
+        tfogm=[0.1, 1.0])
+```
+
+The `ideal` function will return the total Allan variance curve, `va`, as well
+as a matrix, `vac`, whose rows represent the component Allan variances over
+`tau`.
 
 ## Fitting to Signal Allan Variance
 
 ```python
-avar.fit(tau, va, taub=None, mask=None, tol=0.007)
+avar.fit(tau, va, mask=None, fogms=0, tol=0.007)
 ```
 
 Given the Allan variance curve of some signal, `va`, at various averaging
-periods `tau`, you can get the best fit using the five component noises. As with
-the `ideal` function, if `taub` is left undefined, the flicker noise will be
-treated as the idealized, flat Allan variance over averaging period. Otherwise,
-the flicker noise will be treated as a first-order, Gauss-Markov noise. By
-default, this function will automatically attempt to determine if certain
-component noises are even at play based on the tolerance value `tol`. However,
-you can directly control which component noises you wish to include or exclude
-with the `mask` array. For each element of `mask` that is `False` the
-corresponding component noise will be excluded.
+periods `tau`, you can get the best fit using the five basic component noises
+and `fogms` number of first-order, Gauss-Markov (FOGM) noises. By default, this
+function will automatically attempt to determine if certain component noises are
+even at play based on the tolerance value `tol`. However, you can directly
+control which component noises you wish to include or exclude with the `mask`
+array. For each element of `mask` that is `False` the corresponding component
+noise will be excluded. This function will iterate through the various
+permutations of component noises, starting with 0 FOGMs. If a fit satisfies the
+specified `tol` tolerance, the search will end. Otherwise, the best fit will be
+used.
+
+The return values are the fitted Allan variance curve, `vf`, and a `params`
+object, `p` (see the section on Ideal Allan Variance), containing the variances
+of the basic component noise variances (quantization, white, flicker, walk, and
+ramp), `vc`, any first-order, Gauss-Markov (FOGM) noise variances, `vfogm`, and
+the corresponding FOGM time constants, `tfogm`.
 
 ## Noise Generation
 
 ```python
-avar.noise(vc, K, T, taub=None)
+avar.noise(K, T, p)
 ```
 
-Given a five-element array of component noise variances `vc`, you can create an
-artificially-generated noise signal of length `K` and sampling period `T`. Each
-element of `vc` corresponds to one of the five component noise types:
-quantization, white, flicker, walk, and ramp. As with the `ideal` function, if
-`taub` is left undefined, the flicker noise will be treated as the idealized,
-flat Allan variance over averaging period. Otherwise, the flicker noise will be
-treated as a first-order, Gauss-Markov noise.
+Generate a noise signal of length `K`, sampling period `T`, and parameters `p`.
+Parameter `p` is a `params` object (see the section on Ideal Allan Variance).
+
+This function returns the noise signal `y`.
```

