# Comparing `tmp/npdoseresponse-0.0.2.tar.gz` & `tmp/npdoseresponse-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npdoseresponse-0.0.2.tar", last modified: Sun May 12 19:30:05 2024, max compression
+gzip compressed data, was "npdoseresponse-0.0.3.tar", last modified: Mon May 13 19:35:34 2024, max compression
```

## Comparing `npdoseresponse-0.0.2.tar` & `npdoseresponse-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-12 19:30:05.513621 npdoseresponse-0.0.2/
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1070 2024-05-07 04:36:16.000000 npdoseresponse-0.0.2/LICENSE
-drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-12 19:30:05.507653 npdoseresponse-0.0.2/NPDoseResponse/
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)    22017 2024-05-12 19:24:12.000000 npdoseresponse-0.0.2/NPDoseResponse/NPDoseResponse.py
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)      211 2024-05-12 19:29:36.000000 npdoseresponse-0.0.2/NPDoseResponse/__init__.py
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     2765 2024-03-11 06:18:32.000000 npdoseresponse-0.0.2/NPDoseResponse/rbf.py
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     5430 2024-05-12 19:21:37.000000 npdoseresponse-0.0.2/NPDoseResponse/utils.py
-drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-12 19:30:05.512094 npdoseresponse-0.0.2/NPDoseResponse.egg-info/
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1926 2024-05-12 19:30:05.000000 npdoseresponse-0.0.2/NPDoseResponse.egg-info/PKG-INFO
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)      321 2024-05-12 19:30:05.000000 npdoseresponse-0.0.2/NPDoseResponse.egg-info/SOURCES.txt
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)        1 2024-05-12 19:30:05.000000 npdoseresponse-0.0.2/NPDoseResponse.egg-info/dependency_links.txt
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)       12 2024-05-12 19:30:05.000000 npdoseresponse-0.0.2/NPDoseResponse.egg-info/requires.txt
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)       15 2024-05-12 19:30:05.000000 npdoseresponse-0.0.2/NPDoseResponse.egg-info/top_level.txt
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1926 2024-05-12 19:30:05.512911 npdoseresponse-0.0.2/PKG-INFO
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1426 2024-05-07 06:22:29.000000 npdoseresponse-0.0.2/README.md
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)       38 2024-05-12 19:30:05.513817 npdoseresponse-0.0.2/setup.cfg
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)      805 2024-05-12 19:29:33.000000 npdoseresponse-0.0.2/setup.py
+drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-13 19:35:34.444910 npdoseresponse-0.0.3/
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1070 2024-05-07 04:36:16.000000 npdoseresponse-0.0.3/LICENSE
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1928 2024-05-13 19:35:34.444302 npdoseresponse-0.0.3/PKG-INFO
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1428 2024-05-13 19:23:52.000000 npdoseresponse-0.0.3/README.md
+drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-13 19:35:34.439766 npdoseresponse-0.0.3/npDoseResponse/
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)      211 2024-05-13 19:35:15.000000 npdoseresponse-0.0.3/npDoseResponse/__init__.py
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)    22845 2024-05-13 01:22:31.000000 npdoseresponse-0.0.3/npDoseResponse/npDoseResponse.py
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     2837 2024-05-13 01:23:42.000000 npdoseresponse-0.0.3/npDoseResponse/rbf.py
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     5430 2024-05-12 19:21:37.000000 npdoseresponse-0.0.3/npDoseResponse/utils.py
+drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-13 19:35:34.443759 npdoseresponse-0.0.3/npDoseResponse.egg-info/
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1928 2024-05-13 19:35:34.000000 npdoseresponse-0.0.3/npDoseResponse.egg-info/PKG-INFO
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)      321 2024-05-13 19:35:34.000000 npdoseresponse-0.0.3/npDoseResponse.egg-info/SOURCES.txt
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)        1 2024-05-13 19:35:34.000000 npdoseresponse-0.0.3/npDoseResponse.egg-info/dependency_links.txt
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)       12 2024-05-13 19:35:34.000000 npdoseresponse-0.0.3/npDoseResponse.egg-info/requires.txt
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)       15 2024-05-13 19:35:34.000000 npdoseresponse-0.0.3/npDoseResponse.egg-info/top_level.txt
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)       38 2024-05-13 19:35:34.445093 npdoseresponse-0.0.3/setup.cfg
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)      805 2024-05-13 19:35:18.000000 npdoseresponse-0.0.3/setup.py
```

### Comparing `npdoseresponse-0.0.2/LICENSE` & `npdoseresponse-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `npdoseresponse-0.0.2/NPDoseResponse/NPDoseResponse.py` & `npdoseresponse-0.0.3/npDoseResponse/npDoseResponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -453,15 +453,16 @@
         beta = np.linalg.lstsq(lhs, rhs, rcond=rcond)[0]
         Y_est[i] = np.math.factorial(deriv_ord)*beta[deriv_ord]
     return Y_est
 
 
 
 def RegAdjust(Y, X, t_eval=None, h=None, b=None, degree=2, deriv_ord=0, 
-              kernT="epanechnikov", kernS="epanechnikov"):
+              kernT="epanechnikov", kernS="epanechnikov", parallel=False, 
+              processes=20):
     '''
     Estimating the dose-response curve via simple integral estimator with linear interpolation approximation.
     
     
     Parameters
     ----------
         Y: (n,)-array
@@ -485,21 +486,36 @@
         deriv_ord: int
             The order of the estimated derivative of the conditional mean outcome function. 
             (Default: deriv_ord=0. Then, it estimates the conditional mean outcome function itself.)
             
         kernT, kernS: str
             The names of kernel functions for the treatment/exposure variable and confounding variables.
             (Default: "epanechnikov".)
+            
+        parallel: boolean
+            The indicator of whether the function should be parallel executed by
+            multi-processing. (Default: parallel=False.)
+            
+        processes: int
+            The number of processes for parallel execution. (Default: processes=20.)
     '''
     
     if t_eval is None: 
         t_eval = X[:,0].copy()
     
     n = X.shape[0]  ## Number of data points
-    beta_mat = np.zeros((n, t_eval.shape[0]))
-    for i in range(t_eval.shape[0]):
-        X_mat = np.concatenate([t_eval[i]*np.ones((n,1)), X[:,1:]], axis=1)
-        beta_mat[:,i] = LocalPolyReg(Y, X, x_eval=X_mat, degree=degree, deriv_ord=deriv_ord, 
-                                     h=h, b=b, kernT=kernT, kernS=kernS)
+    
+    if parallel:
+        with Pool(processes=processes) as pool:
+            part_fun = partial(LocalPolyReg_Fs, Y=Y, X=X, degree=degree, deriv_ord=deriv_ord, 
+                               h=h, b=b, kernT=kernT, kernS=kernS)
+            beta_mat = pool.map(part_fun, [np.concatenate([t_eval[i]*np.ones((n,1)), X[:,1:]], axis=1) for i in range(t_eval.shape[0])])
+            beta_mat = np.concatenate(beta_mat, axis=0).reshape(t_eval.shape[0], n).T
+    else:
+        beta_mat = np.zeros((n, t_eval.shape[0]))
+        for i in range(t_eval.shape[0]):
+            X_mat = np.concatenate([t_eval[i]*np.ones((n,1)), X[:,1:]], axis=1)
+            beta_mat[:,i] = LocalPolyReg(Y, X, x_eval=X_mat, degree=degree, deriv_ord=deriv_ord, 
+                                         h=h, b=b, kernT=kernT, kernS=kernS)
     m_est = np.mean(beta_mat, axis=0)
     return m_est
```

### Comparing `npdoseresponse-0.0.2/NPDoseResponse/rbf.py` & `npdoseresponse-0.0.3/npDoseResponse/rbf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-#!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-"""
-@author: Yikun Zhang
-Last Editing: March 10, 2024
 
-This file contains the implementation of all the common kernel functions.
-"""
+# Author: Yikun Zhang
+# Last Editing: March 10, 2024
+
+# Description: This file contains the implementations of common kernel functions.
 
 import numpy as np
 
+#=======================================================================================#
+
 def rectangular(t):
     ind = (np.abs(t)<=1)
     res = np.abs(0.5*ind)
     return res
 
 def triangular(t):
     ind = (np.abs(t)<=1)
```

### Comparing `npdoseresponse-0.0.2/NPDoseResponse/utils.py` & `npdoseresponse-0.0.3/npDoseResponse/utils.py`

 * *Files identical despite different names*

### Comparing `npdoseresponse-0.0.2/NPDoseResponse.egg-info/PKG-INFO` & `npdoseresponse-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 Metadata-Version: 2.1
-Name: NPDoseResponse
-Version: 0.0.2
+Name: npDoseResponse
+Version: 0.0.3
 Summary: Nonparametric Estimation and Inference on Dose-Response Curves
-Home-page: https://github.com/zhangyk8/NPDoseResponse
+Home-page: https://github.com/zhangyk8/npDoseResponse
 Author: Yikun Zhang
 Author-email: yikunzhang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.16
 
-[![PyPI pyversions](https://img.shields.io/pypi/pyversions/NPDoseResponse.svg)](https://pypi.python.org/pypi/NPDoseResponse/)
-[![PyPI version](https://badge.fury.io/py/NPDoseResponse.svg)](https://badge.fury.io/py/NPDoseResponse)
-[![Downloads](https://static.pepy.tech/badge/NPDoseResponse)](https://pepy.tech/project/NPDoseResponse)
-[![Documentation Status](https://readthedocs.org/projects/doseresponse/badge/?version=latest)](http://npdoseresponse.readthedocs.io/?badge=latest)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/npDoseResponse.svg)](https://pypi.python.org/pypi/npDoseResponse/)
+[![PyPI version](https://badge.fury.io/py/npDoseResponse.svg)](https://badge.fury.io/py/NPDoseResponse)
+[![Downloads](https://static.pepy.tech/badge/npDoseResponse)](https://pepy.tech/project/npDoseResponse)
+[![Documentation Status](https://readthedocs.org/projects/npdoseresponse/badge/?version=latest)](http://npdoseresponse.readthedocs.io/?badge=latest)
 
 # Nonparametric Estimation and Inference on Dose-Response Curves
 
 This package implements the proposed integral estimator and a localized derivative estimator for estimating the covariate-adjusted regression function (or the dose-response curve in causal inference) and its derivative. We also document all the code for simulations and real-world case study in our paper [here](https://github.com/zhangyk8/NPDoseResponse/tree/main/Paper_Code).
 
 * Free software: MIT license
 * Python Package Documentation: [https://npdoseresponse.readthedocs.io](https://npdoseresponse.readthedocs.io).
 
 Installation guide
 --------
 
-```NPDoseResponse``` requires Python 3.8+ (earlier version might be applicable) and [NumPy](http://www.numpy.org/). To install the latest version of ```NPDoseResponse``` from this repository, run:
+```npDoseResponse``` requires Python 3.8+ (earlier version might be applicable) and [NumPy](http://www.numpy.org/). To install the latest version of ```npDoseResponse``` from this repository, run:
 
 ```
 python setup.py install
 ```
 
 To pip install a stable release, run:
 ```
-pip install NPDoseResponse
+pip install npDoseResponse
 ```
 
 References
 --------
```

### Comparing `npdoseresponse-0.0.2/PKG-INFO` & `npdoseresponse-0.0.3/npDoseResponse.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 Metadata-Version: 2.1
-Name: NPDoseResponse
-Version: 0.0.2
+Name: npDoseResponse
+Version: 0.0.3
 Summary: Nonparametric Estimation and Inference on Dose-Response Curves
-Home-page: https://github.com/zhangyk8/NPDoseResponse
+Home-page: https://github.com/zhangyk8/npDoseResponse
 Author: Yikun Zhang
 Author-email: yikunzhang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.16
 
-[![PyPI pyversions](https://img.shields.io/pypi/pyversions/NPDoseResponse.svg)](https://pypi.python.org/pypi/NPDoseResponse/)
-[![PyPI version](https://badge.fury.io/py/NPDoseResponse.svg)](https://badge.fury.io/py/NPDoseResponse)
-[![Downloads](https://static.pepy.tech/badge/NPDoseResponse)](https://pepy.tech/project/NPDoseResponse)
-[![Documentation Status](https://readthedocs.org/projects/doseresponse/badge/?version=latest)](http://npdoseresponse.readthedocs.io/?badge=latest)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/npDoseResponse.svg)](https://pypi.python.org/pypi/npDoseResponse/)
+[![PyPI version](https://badge.fury.io/py/npDoseResponse.svg)](https://badge.fury.io/py/NPDoseResponse)
+[![Downloads](https://static.pepy.tech/badge/npDoseResponse)](https://pepy.tech/project/npDoseResponse)
+[![Documentation Status](https://readthedocs.org/projects/npdoseresponse/badge/?version=latest)](http://npdoseresponse.readthedocs.io/?badge=latest)
 
 # Nonparametric Estimation and Inference on Dose-Response Curves
 
 This package implements the proposed integral estimator and a localized derivative estimator for estimating the covariate-adjusted regression function (or the dose-response curve in causal inference) and its derivative. We also document all the code for simulations and real-world case study in our paper [here](https://github.com/zhangyk8/NPDoseResponse/tree/main/Paper_Code).
 
 * Free software: MIT license
 * Python Package Documentation: [https://npdoseresponse.readthedocs.io](https://npdoseresponse.readthedocs.io).
 
 Installation guide
 --------
 
-```NPDoseResponse``` requires Python 3.8+ (earlier version might be applicable) and [NumPy](http://www.numpy.org/). To install the latest version of ```NPDoseResponse``` from this repository, run:
+```npDoseResponse``` requires Python 3.8+ (earlier version might be applicable) and [NumPy](http://www.numpy.org/). To install the latest version of ```npDoseResponse``` from this repository, run:
 
 ```
 python setup.py install
 ```
 
 To pip install a stable release, run:
 ```
-pip install NPDoseResponse
+pip install npDoseResponse
 ```
 
 References
 --------
```

### Comparing `npdoseresponse-0.0.2/README.md` & `npdoseresponse-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-[![PyPI pyversions](https://img.shields.io/pypi/pyversions/NPDoseResponse.svg)](https://pypi.python.org/pypi/NPDoseResponse/)
-[![PyPI version](https://badge.fury.io/py/NPDoseResponse.svg)](https://badge.fury.io/py/NPDoseResponse)
-[![Downloads](https://static.pepy.tech/badge/NPDoseResponse)](https://pepy.tech/project/NPDoseResponse)
-[![Documentation Status](https://readthedocs.org/projects/doseresponse/badge/?version=latest)](http://npdoseresponse.readthedocs.io/?badge=latest)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/npDoseResponse.svg)](https://pypi.python.org/pypi/npDoseResponse/)
+[![PyPI version](https://badge.fury.io/py/npDoseResponse.svg)](https://badge.fury.io/py/NPDoseResponse)
+[![Downloads](https://static.pepy.tech/badge/npDoseResponse)](https://pepy.tech/project/npDoseResponse)
+[![Documentation Status](https://readthedocs.org/projects/npdoseresponse/badge/?version=latest)](http://npdoseresponse.readthedocs.io/?badge=latest)
 
 # Nonparametric Estimation and Inference on Dose-Response Curves
 
 This package implements the proposed integral estimator and a localized derivative estimator for estimating the covariate-adjusted regression function (or the dose-response curve in causal inference) and its derivative. We also document all the code for simulations and real-world case study in our paper [here](https://github.com/zhangyk8/NPDoseResponse/tree/main/Paper_Code).
 
 * Free software: MIT license
 * Python Package Documentation: [https://npdoseresponse.readthedocs.io](https://npdoseresponse.readthedocs.io).
 
 Installation guide
 --------
 
-```NPDoseResponse``` requires Python 3.8+ (earlier version might be applicable) and [NumPy](http://www.numpy.org/). To install the latest version of ```NPDoseResponse``` from this repository, run:
+```npDoseResponse``` requires Python 3.8+ (earlier version might be applicable) and [NumPy](http://www.numpy.org/). To install the latest version of ```npDoseResponse``` from this repository, run:
 
 ```
 python setup.py install
 ```
 
 To pip install a stable release, run:
 ```
-pip install NPDoseResponse
+pip install npDoseResponse
 ```
 
 References
 --------
```

### Comparing `npdoseresponse-0.0.2/setup.py` & `npdoseresponse-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name="NPDoseResponse",
-    version="0.0.2",
+    name="npDoseResponse",
+    version="0.0.3",
     author="Yikun Zhang",
     author_email="yikunzhang@foxmail.com",
     description="Nonparametric Estimation and Inference on Dose-Response Curves",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/zhangyk8/NPDoseResponse",
+    url="https://github.com/zhangyk8/npDoseResponse",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=setuptools.find_packages(),
-    # packages=["NPDoseResponse"],
+    # packages=["npDoseResponse"],
     install_requires=["numpy >= 1.16"],
     python_requires=">=3.8",
 )
```

