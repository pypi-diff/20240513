# Comparing `tmp/unite_toolbox-0.1.6.tar.gz` & `tmp/unite_toolbox-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unite_toolbox-0.1.6.tar", last modified: Sat Apr 13 13:42:02 2024, max compression
+gzip compressed data, was "unite_toolbox-0.1.9.tar", last modified: Mon May 13 13:10:38 2024, max compression
```

## Comparing `unite_toolbox-0.1.6.tar` & `unite_toolbox-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:42:02.049980 unite_toolbox-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-13 13:41:56.000000 unite_toolbox-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-13 13:42:02.049980 unite_toolbox-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-13 13:41:56.000000 unite_toolbox-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-13 13:41:56.000000 unite_toolbox-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 13:42:02.049980 unite_toolbox-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-13 13:41:56.000000 unite_toolbox-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:42:02.049980 unite_toolbox-0.1.6/unite_toolbox/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-13 13:41:56.000000 unite_toolbox-0.1.6/unite_toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11593 2024-04-13 13:41:56.000000 unite_toolbox-0.1.6/unite_toolbox/bin_estimators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-13 13:41:56.000000 unite_toolbox-0.1.6/unite_toolbox/kde_estimators.py
--rw-r--r--   0 runner    (1001) docker     (127)     7898 2024-04-13 13:41:56.000000 unite_toolbox-0.1.6/unite_toolbox/knn_estimators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:42:02.049980 unite_toolbox-0.1.6/unite_toolbox/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:41:56.000000 unite_toolbox-0.1.6/unite_toolbox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-13 13:41:56.000000 unite_toolbox-0.1.6/unite_toolbox/utils/bootstrapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-13 13:41:56.000000 unite_toolbox-0.1.6/unite_toolbox/utils/data_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-13 13:41:56.000000 unite_toolbox-0.1.6/unite_toolbox/utils/marginal_information.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-13 13:41:56.000000 unite_toolbox-0.1.6/unite_toolbox/utils/sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:42:02.049980 unite_toolbox-0.1.6/unite_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-13 13:42:02.000000 unite_toolbox-0.1.6/unite_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-13 13:42:02.000000 unite_toolbox-0.1.6/unite_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:42:02.000000 unite_toolbox-0.1.6/unite_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-13 13:42:02.000000 unite_toolbox-0.1.6/unite_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-13 13:42:02.000000 unite_toolbox-0.1.6/unite_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:10:38.530645 unite_toolbox-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-13 13:10:34.000000 unite_toolbox-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-13 13:10:38.530645 unite_toolbox-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-13 13:10:34.000000 unite_toolbox-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-13 13:10:34.000000 unite_toolbox-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:10:38.530645 unite_toolbox-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-13 13:10:34.000000 unite_toolbox-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:10:38.526645 unite_toolbox-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-13 13:10:34.000000 unite_toolbox-0.1.9/tests/test_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-13 13:10:34.000000 unite_toolbox-0.1.9/tests/test_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-13 13:10:34.000000 unite_toolbox-0.1.9/tests/test_kld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-13 13:10:34.000000 unite_toolbox-0.1.9/tests/test_mutual_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-05-13 13:10:34.000000 unite_toolbox-0.1.9/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:10:38.526645 unite_toolbox-0.1.9/unite_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 13:10:34.000000 unite_toolbox-0.1.9/unite_toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12429 2024-05-13 13:10:34.000000 unite_toolbox-0.1.9/unite_toolbox/bin_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-13 13:10:34.000000 unite_toolbox-0.1.9/unite_toolbox/kde_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8839 2024-05-13 13:10:34.000000 unite_toolbox-0.1.9/unite_toolbox/knn_estimators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:10:38.530645 unite_toolbox-0.1.9/unite_toolbox/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:10:34.000000 unite_toolbox-0.1.9/unite_toolbox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-05-13 13:10:34.000000 unite_toolbox-0.1.9/unite_toolbox/utils/bootstrapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-13 13:10:34.000000 unite_toolbox-0.1.9/unite_toolbox/utils/data_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-13 13:10:34.000000 unite_toolbox-0.1.9/unite_toolbox/utils/marginal_scores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-13 13:10:34.000000 unite_toolbox-0.1.9/unite_toolbox/utils/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:10:38.530645 unite_toolbox-0.1.9/unite_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-13 13:10:38.000000 unite_toolbox-0.1.9/unite_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-13 13:10:38.000000 unite_toolbox-0.1.9/unite_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:10:38.000000 unite_toolbox-0.1.9/unite_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-13 13:10:38.000000 unite_toolbox-0.1.9/unite_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-13 13:10:38.000000 unite_toolbox-0.1.9/unite_toolbox.egg-info/top_level.txt
```

### Comparing `unite_toolbox-0.1.6/LICENSE` & `unite_toolbox-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `unite_toolbox-0.1.6/PKG-INFO` & `unite_toolbox-0.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unite_toolbox
-Version: 0.1.6
+Version: 0.1.9
 Summary: A toolbox for practical applications of information theory.
 Author-email: Manuel Álvarez Chaves <manuel.alvarezchaves@simtech.uni-stuttgart.de>, Anneli Guthke <anneli.guthke@simtech.uni-stuttgart.de>, Uwe Ehret <uwe.ehret@kit.edu>, Hoshin Gupta <hoshin@arizona.edu>
 Maintainer-email: Manuel Álvarez Chaves <manuel.alvarezchaves@simtech.uni-stuttgart.de>
 License: MIT License
 Project-URL: Documentation, https://unite-toolbox.readthedocs.io/
 Project-URL: Repository, https://github.com/manuel-alvarez-chaves/unite_toolbox
 Project-URL: Team, https://www.simtech.uni-stuttgart.de/exc/research/junior-research-groups/statistical-model-data-integration/
@@ -13,25 +13,26 @@
 License-File: LICENSE
 Requires-Dist: numpy>=1.25.0
 Requires-Dist: scipy>=1.12.0
 Requires-Dist: tqdm>=4.66.2
 Provides-Extra: dev
 Requires-Dist: jupyterlab>=4.1.2; extra == "dev"
 Requires-Dist: matplotlib>=3.8.3; extra == "dev"
-Requires-Dist: numpy>=1.26.4; extra == "dev"
-Requires-Dist: pandas>=2.2.1; extra == "dev"
-Requires-Dist: pyarrow>=15.0.0; extra == "dev"
-Requires-Dist: scipy>=1.12.0; extra == "dev"
-Requires-Dist: tqdm>=4.66.2; extra == "dev"
-Requires-Dist: xarray>=2024.2.0; extra == "dev"
+Requires-Dist: nbsphinx>=0.9.4; extra == "dev"
+Requires-Dist: pytest>=8.2.0; extra == "dev"
+Requires-Dist: ruff>=0.4.3; extra == "dev"
+Requires-Dist: Sphinx>=7.3.7; extra == "dev"
+Requires-Dist: sphinx_rtd_theme>=2.0.0; extra == "dev"
 
 # UNITE Toolbox
 
 ### Unified diagnostic evaluation of scientific models based on information theory
 
+![PyPI - Version](https://img.shields.io/pypi/v/unite_toolbox) ![Tests Badge](https://github.com/manuel-alvarez-chaves/unite_toolbox/actions/workflows/run-tests.yml/badge.svg) [![Coverage](https://codecov.io/gh/manuel-alvarez-chaves/unite_toolbox/graph/badge.svg?token=MWNDWXLZ9B)](https://codecov.io/gh/manuel-alvarez-chaves/unite_toolbox)
+
 The **UNITE Toolbox** is a Python library for incorporating _Information Theory_
 into data analysis and modeling workflows.
 The toolbox collects different methods of estimating information-theoretic quantities
 in one easy-to-use Python package.
 Currently, UNITE includes functions to calculate entropy $H(X)$,
 Kullback-Leibler divergence $D_{KL}(p||q)$, and mutual information $I(X; Y)$,
 using three methods:
```

### Comparing `unite_toolbox-0.1.6/README.md` & `unite_toolbox-0.1.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # UNITE Toolbox
 
 ### Unified diagnostic evaluation of scientific models based on information theory
 
+![PyPI - Version](https://img.shields.io/pypi/v/unite_toolbox) ![Tests Badge](https://github.com/manuel-alvarez-chaves/unite_toolbox/actions/workflows/run-tests.yml/badge.svg) [![Coverage](https://codecov.io/gh/manuel-alvarez-chaves/unite_toolbox/graph/badge.svg?token=MWNDWXLZ9B)](https://codecov.io/gh/manuel-alvarez-chaves/unite_toolbox)
+
 The **UNITE Toolbox** is a Python library for incorporating _Information Theory_
 into data analysis and modeling workflows.
 The toolbox collects different methods of estimating information-theoretic quantities
 in one easy-to-use Python package.
 Currently, UNITE includes functions to calculate entropy $H(X)$,
 Kullback-Leibler divergence $D_{KL}(p||q)$, and mutual information $I(X; Y)$,
 using three methods:
```

### Comparing `unite_toolbox-0.1.6/unite_toolbox/bin_estimators.py` & `unite_toolbox-0.1.9/unite_toolbox/bin_estimators.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import numpy as np
 
 
-def estimate_ideal_bins(data, counts=True):
-    """Estimate the number of ideal bins
+def estimate_ideal_bins(
+    data: np.ndarray,
+    *,
+    counts: bool | None = True,
+) -> dict[str, int | list[float]]:
+    """Estimate the number of ideal bins.
 
     Estimates the ideal number of bins for each feature (column) of a 2D data
     array using different methods. See numpy.histogram_bin_edges for a list
     of available methods.
 
     Parameters
     ----------
@@ -15,186 +19,205 @@
     counts : bool, optional
         Whether to return the number of bins (True) or the bin edges (False).
 
     Returns
     -------
     dict
         A dictionary with a key for each method, and the values are lists of
-        number of bins or bin edges for each feature of the data (if counts=False).
-    """
+        number of bins or bin edges for each feature of the data
+        (if counts=False).
 
+    """
     _, d_features = data.shape
 
     methods = ["fd", "scott", "sturges", "doane"]
     ideal_bins = []
 
     for m in methods:
         d_bins = []
         for d in range(d_features):
             num_bins = np.histogram_bin_edges(data[:, d], bins=m)
             num_bins = len(num_bins) if counts is True else num_bins
             d_bins.append(num_bins)
         ideal_bins.append(d_bins)
 
-    return dict(zip(methods, ideal_bins))
-
+    return dict(zip(methods, ideal_bins, strict=True))
 
-def calc_bin_density(x, data, edges):
-    """Calculates density using binning
 
-    Calculates the density of every point of the 2D array x within the d-dimensional
-    histogram created from data and edges.
-
-    Similar to a lookup operation where the entries in x are replaced by the bin indices
-    in which they would fall given the binning scheme defined in edges. Then the indices
-    are used to "look up" each value of x in the d-dimensional histogram created from
-    data and edges.
+def calc_bin_density(
+    x: np.ndarray,
+    data: np.ndarray,
+    edges: list[int | list[float]],
+) -> np.ndarray:
+    """Calculate density using binning.
+
+    Calculates the density of every point of the 2D array x within the
+    d-dimensional histogram created from data and edges.
+
+    Similar to a lookup operation where the entries in x are replaced by the
+    bin indices in which they would fall given the binning scheme defined in
+    edges. Then the indices are used to "look up" each value of x in the
+    d-dimensional histogram created from data and edges.
 
     Parameters
     ----------
     x : numpy.ndarray
         Array of shape (n_samples, d_features)
     data : numpy.ndarray
         Array of shape (n_samples, d_features)
     edges : list or int
-        A list of length d_features which contains arrays describing the bin edges
-        along each dimension or a list of ints describing the number of bins to use
-        in each dimension.
+        A list of length d_features which contains arrays describing the bin
+        edges along each dimension or a list of ints describing the number of
+        bins to use in each dimension.
 
     Returns
     -------
     fx : numpy.ndarray
         Array of shape (n_samples, 1)
+
     """
     fi, edges = np.histogramdd(data, edges, density=True)
     res = []
     # Loop over dimensions
     for i in range(len(edges)):
         dimbins = np.digitize(x[:, i], edges[i])
-        dimbins = np.where((dimbins > 0) & (dimbins < len(edges[i])), dimbins, -9998) - 1
+        dimbins = (
+            np.where((dimbins > 0) & (dimbins < len(edges[i])), dimbins, -9998)
+            - 1
+        )
         res.append(dimbins)
 
     # Loop over elements
     indexes = np.column_stack(res)
     fx = np.zeros(shape=(x.shape[0], 1))
     for i, idx in enumerate(indexes):
         if -9999 not in idx:
             fx[i, 0] += fi[tuple(idx)]
     return fx
 
 
-def calc_vol_array(edges):
-    """Calculates the volume of the multidimensional array
+def calc_vol_array(edges: list[np.ndarray]) -> np.ndarray:
+    """Calculate the volume of a multidimensional array.
 
     Calculates the volume of each cell of the multidimensional array defined
-    by edges where edges is a list of arrays. As an example, if edges contains
-    two arrays, this functions returns a 2D grid where each element in the grid
-    contains the value for the area of that specific cell. If edges contains three
-    arrays, the returned grid is 3D where each element of the grid is the volume of
-    the cell, and so on.
-
-    As this is done to calculate the volume of each bin of a multidimensional histogram,
-    the returned grid can be indexed by the same indices as a histogramdd from NumPy.
+    by `edges` where `edges` is a list of arrays. As an example, if `edges`
+    contains two arrays, this functions returns a 2D grid where each element
+    in the grid contains the value for the area of that specific cell.
+    If `edges` contains three arrays, the returned grid is 3D where each
+    element of the grid is the volume of the cell, and so on.
+
+    As this is done to calculate the volume of each bin of a multidimensional
+    histogram, the returned grid can be indexed by the same indices as a
+    `histogramdd` from NumPy.
 
     Parameters
     ----------
-    edges : list of 1D numpy.ndarray
+    edges : list[np.ndarray]
+        List of 1D NumPy arrays
 
     Returns
     -------
     vol : numpy.ndarray
         Array of shape (len(arr0) - 1, len(arr1) - 1, ..., len(arrn) - 1)
 
     Example
     -------
-        >>> a = np.array([0., 1., 3., 7., 12.])
-        >>> b = np.array([4., 8., 10.])
+        >>> a = np.array([0.0, 1.0, 3.0, 7.0, 12.0])
+        >>> b = np.array([4.0, 8.0, 10.0])
         >>> calc_vol_array([a, b])
         array([[ 4.,  2.],
                [ 8.,  4.],
                [16.,  8.],
                [20., 10.]])
 
     """
-
     vol = np.diff(edges[0])
     for e in edges[1:]:
         vol = np.stack([vol] * (len(e) - 1), axis=-1)
         for idx, val in enumerate(np.diff(e)):
             vol[..., idx] = vol[..., idx] * val
     return vol
 
 
-def calc_bin_entropy(data, edges):
-    """Calculates entropy using binning
+def calc_bin_entropy(
+    data: np.ndarray,
+    edges: list[int | float] | int,
+) -> tuple[float]:
+    """Calculate entropy using binning.
 
-    Calculates the (joint) entropy of the input data after binning it along each
-    dimension using specified bin edges or number of bins.
+    Calculates the (joint) entropy of the input data after binning it along
+    each dimension using specified bin edges or number of bins.
 
     Parameters
     ----------
     data : numpy.ndarray
         Array of shape (n_samples, d_features)
     edges : list or int
-        A list of length d_features which contains arrays describing the bin edges
-        along each dimension or a list of ints describing the number of bins to use
-        in each dimension. Input can also be a single int and the histogram will be
-        created with the same number of bins for each dimension.
+        A list of length d_features which contains arrays describing the bin
+        edges along each dimension or a list of ints describing the number of
+        bins to use in each dimension. Input can also be a single int and the
+        histogram will be created with the same number of bins for each
+        dimension.
 
     Returns
     -------
     h : float
         The (joint) entropy of the input data after binning.
     cf : float
         The correction factor due to bin spacing. See Cover &
         Thomas (2006) Eq. 8.28 ISBN: 978-0-471-24195-9
-    """
 
-    # binning
+    """
+    # Binning
     f, edges = np.histogramdd(data, bins=edges, density=True)
 
-    # volume
+    # Volume
     volume = calc_vol_array(edges)
 
-    # entropy
+    # Entropy
     idx = f.nonzero()
     delta = volume[idx]
     f = f[idx]
-    h = -1.0 * np.sum(delta * f * np.log(f * delta))
-    cf = np.sum(f * delta * np.log(delta))
-
-    return h, cf
-
+    h = -1.0 * np.sum(delta * f * np.log(f))
+    corr_fact = -1.0 * np.sum(f * delta * np.log(delta))
 
-def calc_uniform_bin_entropy(data, edges):
-    """Alternative method to calculate entropy using binning
+    return h, corr_fact
 
-    Calculates the (joint) entropy of the input data. Using this method, every data
-    point is substituted by the specific bin it occupies in `edges`. Therefore limiting
-    the required memory to only store the number of entries in data.
 
-    NOTE: this only works for uniform binning schemes as the correction factor for
-    differential entropy is calculated as assuming that every bin is of the same size.
+def calc_uniform_bin_entropy(
+    data: np.ndarray,
+    edges: list[list[float]],
+) -> tuple[float]:
+    """Alternative method to calculate entropy using binning.
+
+    Calculates the (joint) entropy of the input data. Using this method, every
+    data point is substituted by the specific bin it occupies in `edges`.
+    Therefore limiting the required memory to only store the number of entries
+    in data.
+
+    NOTE: this only works for uniform binning schemes as the correction factor
+    for differential entropy is calculated as assuming that every bin is of the
+    same size.
 
     Parameters
     ----------
     data : numpy.ndarray
         Array of shape (n_samples, d_features)
     edges : list or int
-        A list of length d_features which contains arrays describing the bin edges
-        along each dimension or a list of ints describing the number of bins to use
-        in each dimension.
+        A list of length d_features which contains arrays describing the bin
+        edges along each dimension
 
     Returns
     -------
     h : float
         The (joint) entropy of the input data after binning.
     corr_fact : float
         The correction factor due to bin spacing. See Cover &
         Thomas (2006) Eq. 8.28 ISBN: 978-0-471-24195-9
+
     """
     # Digitize data and get count of unique rows
     data_binned = np.empty(shape=data.shape, dtype=np.int64)
     for idy in range(data.shape[1]):
         data_binned[:, idy] = np.digitize(data[:, idy], edges[idy])
     _, counts = np.unique(data_binned, return_counts=True, axis=0)
 
@@ -209,38 +232,43 @@
     # Calculate entropy and correction factor
     h = -1 * np.sum(delta * density * np.log(density))
     corr_fact = -1 * np.sum(density * delta * np.log(delta))
 
     return h, corr_fact
 
 
-def calc_bin_kld(p, q, edges):
-    """Calculates Kullback-Leibler divergence (relative entropy) using binning
-
-    Calculates the Kullback-Leibler divergence (relative entropy) between p and q
-    [in nats] by approximating both distributions using some binning scheme defined
-    by edges. Edges *must* be able to support the values in q.
+def calc_bin_kld(
+    p: np.ndarray,
+    q: np.ndarray,
+    edges: list[list[float]],
+) -> float:
+    """Calculate Kullback-Leibler divergence (relative entropy) using binning.
+
+    Calculates the Kullback-Leibler divergence (relative entropy) between `p`
+    and `q` [in nats] by approximating both distributions using some binning
+    scheme defined by `edges`. `edges` *must* be able to support the values in
+    `q`.
 
     Parameters
     ----------
     p : numpy.ndarray
         Array of shape (n_samples, d_features)
     q : numpy.ndarray
         Array of shape (m_samples, d_features)
     edges : list or int
-        A list of length d_features which contains arrays describing the bin edges
-        along each dimension or a list of ints describing the number of bins to use
-        in each dimension.
+        A list of length d_features which contains arrays describing the bin
+        edges along each dimension or a list of ints describing the number of
+        bins to use in each dimension.
 
     Returns
     -------
     kld : float
         Kullback-Leibler divergence between p and q [in nats]
-    """
 
+    """
     # Bin according to support of q!
     p_binned = np.empty(shape=p.shape, dtype=np.int64)
     q_binned = np.empty(shape=q.shape, dtype=np.int64)
     for idy in range(q.shape[1]):
         p_binned[:, idy] = np.digitize(p[:, idy], edges[idy])
         q_binned[:, idy] = np.digitize(q[:, idy], edges[idy])
 
@@ -261,22 +289,27 @@
     for idx in matching_bins:
         a = np.where((bins_p == idx).all(axis=1))[0][0]
         b = np.where((bins_q == idx).all(axis=1))[0][0]
         kld += density_p[a] * np.log(density_p[a] / density_q[b])
     return kld
 
 
-def calc_bin_mutual_information(x, y, edges):
-    """Calculates mutual information between X and Y using binning
-
-    Calculates the mutual information between an array X and an array Y. Both X and
-    don't necesarily need the same number of samples as binning is used. This approach
-    builds multivariate histograms for X, Y and X-Y using the specified edges, and
-    evaluates MI in every bin where the density of X-Y is not zero.
-    This is a resubstitution estimate.
+def calc_bin_mutual_information(
+    x: np.ndarray,
+    y: np.ndarray,
+    edges: list[list[float]],
+) -> float:
+    """Calculate mutual information between `x` and `y` using binning.
+
+    Calculates the mutual information between an array `x` and an array `y`.
+    Both `x` and `y` don't necesarily need the same number of samples as
+    binning is used. This approach builds multivariate histograms for `x`, `y`
+    and `x`-`y` using the specified edges, and evaluates I(X; Y) in every bin
+    where the density of `x`-`y` is not zero. This is a resubstitution
+    estimate.
 
     Parameters
     ----------
     x : numpy.ndarray
         Array of shape (n_samples, d1_features)
     y : numpy.ndarray
         Array of shape (m_samples, d2_features)
@@ -285,65 +318,84 @@
         the number of bins in each axis or arrays of the edges for
         the binning scheme of each axis.
 
     Returns
     -------
     mi : float
         Mutual information between x and y [in nats]
+
     """
     _, d1 = x.shape
     _, d2 = y.shape
     data = np.hstack((x, y))
-    fxy, joint_edges = np.histogramdd(data, bins=edges[0] + edges[1], density=True)
+    fxy, joint_edges = np.histogramdd(
+        data,
+        bins=edges[0] + edges[1],
+        density=True,
+    )
     fx, _ = np.histogramdd(x, bins=edges[0], density=True)
     fy, _ = np.histogramdd(y, bins=edges[1], density=True)
 
     volume = calc_vol_array(joint_edges)
 
     mi = 0.0
     for idx in np.ndindex(fxy.shape):
         if fxy[idx] != 0.0:
-            mi += fxy[idx] * volume[idx] * np.log(fxy[idx] / (fx[idx[:d1]] * fy[idx[-d2:]]))
+            mi += (
+                fxy[idx]
+                * volume[idx]
+                * np.log(fxy[idx] / (fx[idx[:d1]] * fy[idx[-d2:]]))
+            )
     return max(0.0, mi)
 
 
-def calc_qs_entropy(sample, alpha=0.25, N_k=500):
-    """Calculates the 1-D entropy of the input data.
+def calc_qs_entropy(
+    sample: np.ndarray,
+    alpha: float = 0.25,
+    N_k: int = 500,
+    seed: int | None = None,
+) -> float:
+    """Calculate the 1-D entropy of the input data.
 
     Calculates the 1-D entropy of the input data [in nats] using
     the  quantile spacing (QS) estimator proposed by: Gupta et al.
     (2021) https://doi.org/10.3390/e23060740
 
     Adapted from: https://github.com/rehsani/Entropy
 
 
     Parameters
     ----------
-    data : numpy.ndarray
+    sample : numpy.ndarray
         Flat array
     alpha : float, optional
         percent of the instances from the sample used for estimation of
         entropy (i.e., number of quantile-spacings).
     N_k : int, optional
         number of sample subsets, used to estimate the sample distribution
         for each quantile empirically
+    seed: int, optional
+        random seed, if None: default is used
 
     Returns
     -------
     h : float
         Entropy [in nats] of 'alpha' percent of the instances
-    """
 
+    """
+    rng = np.random.default_rng(seed=seed)
     sample = sample.flatten()
     n = int(np.ceil(alpha * sample.size))
     x_min = sample.min()
     x_max = sample.max()
     sample.sort()
 
-    sample_b = np.random.choice(sample, sample.size, replace=True)
-    X_alpha = [np.random.choice(sample_b[1:-1], n - 1, replace=False) for _ in range(N_k)]
+    sample_b = rng.choice(sample, sample.size, replace=True)
+    X_alpha = [
+        rng.choice(sample_b[1:-1], n - 1, replace=False) for _ in range(N_k)
+    ]
     X_alpha = np.vstack(X_alpha)
     X_alpha.sort(axis=1)
     Z = np.hstack([x_min, X_alpha.mean(axis=0), x_max])
     dZ = np.diff(Z)
     h = 1 / (n + 1) * np.log((n + 1) * dZ).sum()
     return h
```

### Comparing `unite_toolbox-0.1.6/unite_toolbox/kde_estimators.py` & `unite_toolbox-0.1.9/unite_toolbox/kde_estimators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,223 +1,232 @@
+from enum import Enum
+
 import numpy as np
-from scipy.stats import gaussian_kde
 from scipy.integrate import nquad
+from scipy.stats import gaussian_kde
+
+from unite_toolbox.utils.data_validation import validate_array
 
 
-def calc_kde_density(x, data, bandwidth=None):
-    """Calculates density using KDE
+class KDEMode(Enum):
+    """
+    Enumeration representing different modes for calculating KDE estimates.
+
+    Attributes
+    ----------
+        RESUBSTITUTION : str
+            Calculate an estimate using resubstitution.
+        INTEGRAL : str
+            Calculate an estimate by integrating over the KDE.
+    """
+
+    RESUBSTITUTION = "resubstitution"
+    INTEGRAL = "integral"
+
+
+def calc_kde_density(
+    x: np.ndarray,
+    data: np.ndarray,
+    bandwidth: float | None = None,
+) -> np.ndarray:
+    """Calculate density using KDE.
 
     Calculates the density of every point of the 2D array `x` within KDE
-    representation of `data`. Simply, every point in `x` is evaluated
-    in a KDE-based distribution of `data`.
+    representation of `data`. Simply, every point in `x` is evaluated in a
+    KDE-based distribution of `data`.
 
     Parameters
     ----------
     x : numpy.ndarray
         Array of shape (n_samples, d_features)
     data : numpy.ndarray
         Array of shape (m_samples, d_features)
+    bandwidth : float, optional
+        bandwidth of the gaussian kernel
 
     Returns
     -------
     p : numpy.ndarray
         Array of shape (n_samples, 1)
+
     """
     kde = gaussian_kde(data.T, bw_method=bandwidth)
     p = kde.evaluate(x.T).reshape(-1, 1)
     return p
 
 
-def calc_kde_entropy(data, bandwidth=None):
-    """Calculates entropy using KDE
-
-    Calculates the (joint) entropy of the input data [in nats] by
-    approximating the (joint) density of the distribution using a
-    Gaussian kernel density estimator (KDE). By defaul the Scott
-    estimate for the bandwith is used for the Gaussian kernel.
-    This is a resubstitution estimate.
+def calc_kde_entropy(
+    data: np.ndarray,
+    bandwidth: float | None = None,
+    mode: str = "resubstitution",
+) -> float:
+    """
+    Calculate the entropy of a dataset using kernel density estimation (KDE).
+
+    Calculates the (joint) entropy of the input `data` [in nats] by
+    approximating the (joint) density of the distribution using a Gaussian
+    kernel density estimator (KDE). By defaul the Scott estimate for the
+    bandwith is used for the Gaussian kernel.
+    This function has two modes: `resubstition` and `integral`.
 
     Parameters
     ----------
-    data : numpy.ndarray
-        Array of shape (n_samples, d_features)
+    data : np.ndarray
+        Array of shape (n_samples, n_features)
     bandwidth : float, optional
-        bandwidth of the gaussian kernel
+        Bandwidth of the Gaussian kernel
+    mode : str, "resubstitution" or "integral", optional
+        Method for entropy calculation, defaults to 'resubstitution'
 
     Returns
     -------
     h : float
-        Entropy of the data set [in nats]
-    """
-
-    kde = gaussian_kde(data.T, bw_method=bandwidth)
-    p = kde.evaluate(data.T)
-    h = -1 * np.mean(np.log(p))
-    return h
-
+        Entropy of the dataset [in nats]
 
-def calc_ikde_entropy(data, bandwidth=None):
-    """Calculates entropy using numerical integration and KDE
-
-    Calculates the (joint) entropy of the input data [in nats] by
-    approximating the (joint) density of the distribution using a
-    Gaussian kernel density estimator (KDE).
-    The method creates a helper function that as the basis
-    for numerical integration. The integration limits are set as the maximum
-    and minimum values of X and Y, plus and minus one magnitude of the bandwidth
-    respectively.
-    This is an integral estimate.
     """
-
-    lims = np.vstack((data.min(axis=0), data.max(axis=0))).T
+    mode = KDEMode(mode)
+    data = validate_array(data)
     kde = gaussian_kde(data.T, bw_method=bandwidth)
 
-    def eval_entropy(*args):
-        p = kde.evaluate(np.vstack(args))
-        return -1 * p * np.log(p)
-
-    h = nquad(eval_entropy, ranges=lims)[0]
-    return h
-
-
-def calc_kde_kld(p, q, bandwidth=None):
-    """Calculates Kullback-Leibler divergence (relative entropy) using KDE
-
-    Calculates the Kullback-Leibler divergence (relative entropy) between
-    two data sets (f and g) [in nats] by approximating both distributions using
-    a Gaussian kernel density estimate (KDE). The divergence is measured between
-    both of the estimated densities. Both density estimates are independent, therefore
-    a different number of total samples in p and q is valid.
+    if mode == KDEMode.RESUBSTITUTION:
+        p = kde.evaluate(data.T)
+        h = -1 * np.mean(np.log(p))
+        return h
+
+    elif mode == KDEMode.INTEGRAL:
+        lims = np.vstack((data.min(axis=0), data.max(axis=0))).T
+
+        def eval_entropy(*args: float) -> float:  # helper function
+            p = kde.evaluate(np.vstack(args))
+            return -1 * p * np.log(p)
+
+        h = nquad(eval_entropy, ranges=lims)[0]
+        return h
+
+
+def calc_kde_kld(
+    p: np.ndarray,
+    q: np.ndarray,
+    bandwidth: float | None = None,
+    mode: str = "resubstitution",
+) -> float:
+    """Calculate KLD using KDE.
+
+    Calculates the Kullback-Leibler divergence (relative entropy) between two
+    data sets (`p` and `q`) [in nats] by approximating both distributions using
+    a Gaussian kernel density estimate (KDE). The divergence is measured
+    between both of the estimated densities. Both density estimates are
+    independent, therefore a different number of total samples in `p` and `q`
+    is valid.
+    This function has two modes: `resubstition` and `integral`.
 
     Parameters
     ----------
-    data_p : numpy.ndarray
+    p : numpy.ndarray
         Array of shape (n_samples, d_features)
-    data_q : numpy.ndarray
+    q : numpy.ndarray
         Array of shape (m_samples, d_features)
-    bw : float, optional
+    bandwidth : float, optional
         bandwith of the gaussian kernel
+    mode : str, "resubstitution" or "integral", optional
+        Method for entropy calculation, defaults to 'resubstitution'
 
     Returns
     -------
     kld : float
-        Kullback-Leibler divergence between f and g [in nats]"""
-
-    p_kde = gaussian_kde(p.T, bw_method=bandwidth)
-    q_kde = gaussian_kde(q.T, bw_method=bandwidth)
-
-    pi_kde = p_kde.evaluate(p.T)
-    qi_kde = q_kde.evaluate(q.T)
-
-    kld = np.abs(np.mean(np.log(pi_kde / qi_kde)))
-
-    return kld
-
-
-def calc_ikde_kld(p, q, bandwidth=None):
-    """Calculates Kullback-Leibler divergence (relative entropy) using
-    numerical integration and KDE
+        Kullback-Leibler divergence between p and q [in nats]
 
     """
 
+    mode = KDEMode(mode)
+    p = validate_array(p)
+    q = validate_array(q)
+
     p_kde = gaussian_kde(p.T, bw_method=bandwidth)
     q_kde = gaussian_kde(q.T, bw_method=bandwidth)
-    bw = q_kde.factor
 
-    lims = np.vstack((q.min(axis=0) - bw, q.max(axis=0) + bw)).T
-
-    def eval_kld(*args):
-        pi = p_kde.evaluate(np.vstack(args))
-        qi = q_kde.evaluate(np.vstack(args))
-        if pi == 0.0 or qi == 0.0:
-            return 0.0
-        else:
-            return pi * np.log(pi / qi)
-
-    kld = nquad(eval_kld, ranges=lims)[0]
-    return kld
-
-
-def calc_kde_mutual_information(x, y, bandwidth=None):
-    """Calculates mutual information between X and Y using KDE
-
-    Calculates the mutual information between X and Y [in nats] using KDE.
-    This method uses a multivariate Gaussian kernel so, both X an Y can have
-    multivariate data. The method evaluates density at every point in X, Y and
-    X-Y, therefore, X and Y must have the same number of entries.
-    This is a resubstition method.
+    if mode == KDEMode.RESUBSTITUTION:
+        pi_kde = p_kde.evaluate(q.T)
+        qi_kde = q_kde.evaluate(q.T)
+
+        kld = np.abs(np.mean(np.log(pi_kde / qi_kde)))
+        return max(0.0, kld)
+
+    if mode == KDEMode.INTEGRAL:
+        bw = q_kde.factor
+        lims = np.vstack((q.min(axis=0) - bw, q.max(axis=0) + bw)).T
+
+        def eval_kld(*args: float) -> float:  # helper function
+            pi = p_kde.evaluate(np.vstack(args))
+            qi = q_kde.evaluate(np.vstack(args))
+            res = 0.0
+            if pi != 0.0 or qi != 0.0:
+                res = pi * np.log(pi / qi)
+            return res
+
+        kld = nquad(eval_kld, ranges=lims)[0]
+        return max(0.0, kld)
+
+
+def calc_kde_mutual_information(
+    x: np.ndarray,
+    y: np.ndarray,
+    bandwidth: float | None = None,
+    mode: str = "resubstitution",
+) -> float:
+    """Calculate MI between `x` and `y` using KDE.
+
+    Calculates the mutual information between `x` and `y` [in nats] using KDE.
+    This method uses a multivariate Gaussian kernel so, both `x` an `y` can
+    have multivariate data. The method evaluates density at every point in `x`,
+    `y` and `x`-`y`, therefore, `x` and `y` must have the same number of
+    entries.
+    This function has two modes: `resubstition` and `integral`.
 
     Parameters
     ----------
     x : numpy.ndarray
         Array of shape (n_samples, d1_features)
     y : numpy.ndarray
         Array of shape (n_samples, d2_features)
     bandwidth : float, optional
         bandwith of the gaussian kernel, "scott" by default
+    mode : str, "resubstitution" or "integral", optional
+        Method for entropy calculation, defaults to 'resubstitution'
 
     Returns
     -------
     mi : float
         Mutual information between x and y [in nats]
-    """
-
-    xy = np.hstack((x, y))
 
-    kde_x = gaussian_kde(x.T, bw_method=bandwidth)
-    kde_y = gaussian_kde(y.T, bw_method=bandwidth)
-    kde_xy = gaussian_kde(xy.T, bw_method=bandwidth)
-
-    px_kde = kde_x.evaluate(x.T)
-    py_kde = kde_y.evaluate(y.T)
-    pxy_kde = kde_xy.evaluate(xy.T)
-
-    mi = np.mean(np.log(pxy_kde / (px_kde * py_kde)))
-    return max(0.0, mi)
-
-
-def calc_ikde_mutual_information(x, y, bandwidth=None):
-    """Calculates mutual information between X and Y using numerical
-    integration and KDE
-
-    Calculates the mutual information between X and Y [in nats] using numerical
-    integration and KDE.
-    This method uses a multivariate Gaussian kernel so, both X an Y can have
-    multivariate data. The method creates a helper function that as the basis
-    for numerical integration. The integration limits are set as the maximum
-    and minimum values of X and Y, plus and minus one magnitude of the bandwidth
-    respectively.
-    This is an integral estimate.
-
-    Parameters
-    ----------
-    x : numpy.ndarray
-        Array of shape (n_samples, d1_features)
-    y : numpy.ndarray
-        Array of shape (n_samples, d2_features)
-    bandwidth : float, optional
-        bandwith of the gaussian kernel, "scott" by default
-
-    Returns
-    -------
-    mi : float
-        Mutual information between x and y [in nats]
     """
+    mode = KDEMode(mode)
+    x = validate_array(x)
+    y = validate_array(y)
+    _, d = x.shape
 
     xy = np.hstack((x, y))
-    _, d = xy.shape
 
     kde_x = gaussian_kde(x.T, bw_method=bandwidth)
     kde_y = gaussian_kde(y.T, bw_method=bandwidth)
     kde_xy = gaussian_kde(xy.T, bw_method=bandwidth)
-    bw = kde_xy.factor
-
-    lims = np.vstack((xy.min(axis=0) - bw, xy.max(axis=0) + bw)).T
 
-    def eval_mi(*args):  # helper function
-        px = kde_x.evaluate(np.vstack(args[: d - 1]))
-        py = kde_y.evaluate(np.vstack((args[d - 1],)))
-        pxy = kde_xy.evaluate(np.vstack(args))
-        return pxy * np.log(pxy / (px * py))
+    if mode == KDEMode.RESUBSTITUTION:
+        px_kde = kde_x.evaluate(x.T)
+        py_kde = kde_y.evaluate(y.T)
+        pxy_kde = kde_xy.evaluate(xy.T)
+
+        mi = np.mean(np.log(pxy_kde / (px_kde * py_kde)))
+        return max(0.0, mi)
+
+    if mode == KDEMode.INTEGRAL:
+        bw = kde_xy.factor
+        lims = np.vstack((xy.min(axis=0) - bw, xy.max(axis=0) + bw)).T
+
+        def eval_mi(*args: float) -> float:
+            px = kde_x.evaluate(np.vstack(args[:d]))
+            py = kde_y.evaluate(np.vstack((args[d:])))
+            pxy = kde_xy.evaluate(np.vstack(args))
+            return pxy * np.log(pxy / (px * py))
 
-    mi = nquad(eval_mi, ranges=lims)[0]
-    return max(0.0, mi)
+        mi = nquad(eval_mi, ranges=lims)[0]
+        return max(0.0, mi)
```

### Comparing `unite_toolbox-0.1.6/unite_toolbox/knn_estimators.py` & `unite_toolbox-0.1.9/unite_toolbox/knn_estimators.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,240 +1,298 @@
 import numpy as np
 from scipy.spatial import KDTree
-from scipy.special import gamma, digamma
+from scipy.special import digamma, gamma
 
 
-def vol_lp_ball(r, d, p_norm):
-    r"""Calculates the volume of a :math:`L^p` ball of radius *R* in d-
-    dimensional space.
+def vol_lp_ball(r: float, d: int, p_norm: float) -> float:
+    r"""Calculate volume of :math:`L^p` ball.
+
+    Calculates the volume of a :math:`L^p` ball of radius `r` in
+    `d`-dimensional space.
 
     .. math::
-         V_d^p(R) = \frac{(2\,\Gamma(\frac{1}{p}+1))^d}{\Gamma(\frac{d}{p}+1)}\,R^d
+         V_d^p(R) = \frac{(2\,\Gamma(\frac{1}{p}+1))^d}{\Gamma(\frac{d}{p}+1)}
+         \,R^d
 
     Where:
         * :math:`\Gamma` is the Gamma function.
         * :math:`p` is the order of the Minkowski distance.
         * :math:`d` is the number of dimensions of the d-ball.
         * :math:`R` is the radius of the d-ball.
 
     Parameters
     ----------
     r : float
         radius of the d-ball
     d : int
         dimension of the d-ball
-    p_norm : int
+    p_norm : float
         p (Minkowski) distance. p = 1 is the Manhattan distance,
-        p = 2 is the Euclidian distance, etc.
+        p = 2 is the Euclidian distance, etc. np.inf is the maximum
+        (Chebyshev) distance.
 
     Returns
     -------
     vol : float
         Volume of the L^p ball
-    """
 
+    """
     if p_norm == np.inf:  # faster
         vol = (2**d) * (r**d)
         return vol
 
     a = (2 * gamma(1 / p_norm + 1)) ** d
     b = gamma(d / p_norm + 1)
     c = r**d
     vol = c * a / b
     return vol
 
 
-def calc_knn_density(x, data, k=5, p_norm=2):
-    r"""Calculates the probability density of every point in x.
-
-    Calculates the probability density of every point in x based on
-    the proximity to the data using k-nearest neighbors and the equation
-    proposed by Wang et al. (2009). Note: x and data must have the
+def calc_knn_density(
+    x: np.ndarray,
+    data: np.ndarray,
+    k: int = 5,
+    p_norm: float = 2,
+) -> np.ndarray:
+    r"""Calculate the probability density of `x` using *k*-NN.
+
+    Calculates the probability density of every point in `x` based on
+    the proximity to the `data` using *k*-nearest neighbors and the equation
+    proposed by Wang et al. (2009). Note: `x` and data must have the
     same number of d_features. 10.1109/TIT.2009.2016060
 
     .. math::
-        \hat{p}_k(x_i) = \frac{k}{N-1} \cdot \frac{1}{c_1(d) \cdot \rho^{d}_k(i)}
+        \hat{p}_k(x_i) = \frac{k}{N-1} \cdot \frac{1}{c_1(d)
+        \cdot \rho^{d}_k(i)}
 
     Where:
         * :math:`k` is the number of neighbors used.
         * :math:`N` is the number of samples in the data.
-        * :math:`c_1(d)` is the volume of a d-dimensional unit :math:`L^p` ball.
+        * :math:`c_1(d)` is the volume of a d-dimensional unit :math:`L^p`
+            ball.
         * :math:`d` is the number of dimensions of the data.
-        * :math:`\rho^{d}_k(i)` is the distance between a point :math:`i` and its *k*-th nearest neighbor.
+        * :math:`\rho^{d}_k(i)` is the distance between a point :math:`i` and
+            its *k*-th nearest neighbor.
 
     Parameters
     ----------
     x : numpy.ndarray
         Array of shape (n_samples, d_features)
     data : numpy.ndarray
         Array of shape (n_samples, d_features)
     k : int, optional
         no. of nearest neighbors to use
-    p_norm : int
+    p_norm : float
         p (Minkowski) distance. p = 1 is the Manhattan distance,
-        p = 2 is the Euclidian distance, etc.
+        p = 2 is the Euclidian distance, etc. np.inf is the maximum
+        (Chebyshev) distance.
 
     Returns
     -------
-    p : numpy.array
-        Array of shape (n_samples, d_features)
+    p : numpy.ndarray
+        Array of shape (n_samples, 1)
+
     """
     n, d = data.shape
     vol = vol_lp_ball(r=1.0, d=d, p_norm=p_norm)
 
     knn_tree = KDTree(data)
     radius = knn_tree.query(x, k + 1, p=p_norm)[0][:, k]
     p = (k / (n - 1)) * (1 / (vol * radius))
     return p
 
 
-def calc_knn_entropy(data, k=1, p_norm=2):
-    r"""Calculates the (joint) entropy of the input n-d array.
+def calc_knn_entropy(data: np.ndarray, k: int = 1, p_norm: float = 2) -> float:
+    r"""Calculate the (joint) entropy of the input n-d array.
 
-    Calculates the (joint) entropy of the input data [in nats] using
+    Calculates the (joint) entropy of the input `data` [in nats] using
     the  Kozachenko and Leonenko (KL) (1987) estimator which is an approach
     based on k-nearest neighbors (k-NN). By default, the Euclidean norm
     distance (p-norm = 2) is used to calculate distances.
     http://mi.mathnet.ru/ppi797
 
     .. math::
-        \hat{H}(X) = \psi(N) - \psi(k) + log(c_1(d)) + \frac{d}{N}\sum_{i=1}^{N}\log(\rho^{d}_k(i))
+        \hat{H}(X) = \psi(N) - \psi(k) + log(c_1(d))
+        + \frac{d}{N}\sum_{i=1}^{N}\log(\rho^{d}_k(i))
 
     Where:
         * :math:`\psi` is the digamma function.
         * :math:`N` is the number of samples in the data.
         * :math:`k` is the number of neighbors used.
-        * :math:`c_1(d)` is the volume of a d-dimensional unit :math:`L^p` ball.
+        * :math:`c_1(d)` is the volume of a d-dimensional unit :math:`L^p`
+            ball.
         * :math:`d` is the number of dimensions of the data.
-        * :math:`\rho^{d}_k(i)` is the distance between a point :math:`i` and its *k*-th nearest neighbor.
+        * :math:`\rho^{d}_k(i)` is the distance between a point :math:`i` and
+            its *k*-th nearest neighbor.
 
     Parameters
     ----------
     data : numpy.ndarray
         Array of shape (n_samples, d_features)
     k : int, optional
         no. of nearest neighbors to use
+    p_norm : float
+        p (Minkowski) distance. p = 1 is the Manhattan distance,
+        p = 2 is the Euclidian distance, etc. np.inf is the maximum
+        (Chebyshev) distance.
 
     Returns
     -------
     h : float
         Entropy of the data set [in nats]
-    """
 
+    """
     if len(data.shape) == 1:
         data = data.reshape(-1, 1)
 
     n, d = data.shape
 
     knn_tree = KDTree(data)
     radius = knn_tree.query(data, k + 1, p=p_norm)[0][:, k]
-    h = digamma(n) - digamma(k) + np.log(vol_lp_ball(1.0, d, p_norm)) + d * np.mean(np.log(radius))
+    h = (
+        digamma(n)
+        - digamma(k)
+        + np.log(vol_lp_ball(1.0, d, p_norm))
+        + d * np.mean(np.log(radius))
+    )
     return h
 
 
-def calc_knn_kld(p, q, k=1, p_norm=2):
-    r"""Calculates the the Kullback-Leibler divergence (relative entropy) between
-    two n-d arrays of data.
+def calc_knn_kld(
+    p: np.ndarray,
+    q: np.ndarray,
+    k: int = 1,
+    p_norm: float = 2,
+) -> float:
+    r"""Calculate the Kullback-Leibler divergence between two arrays of data.
 
     Calculates the Kullback-Leibler divergence (relative entropy) between
-    two data sets (p and q) [in nats] using the estimation method proposed
-    by Wang et al. (2009). Both p and q are n-d arrays where d >= 1 which means
-    they can have multiple features. Typically p represents the true distribution
-    while q is the approximate distribution. Different number of total
-    samples in p and q is acceptable, 10.1109/TIT.2009.2016060
+    two data sets (`p` and `q`) [in nats] using the estimation method proposed
+    by Wang et al. (2009). Both `p` and `q` are n-d arrays where d >= 1 which
+    means they can have multiple features. Typically `p` represents the true
+    distribution while `q` is the approximate distribution. A different
+    number of total samples in `p` and `q` is acceptable,
+    10.1109/TIT.2009.2016060
 
     .. math::
         \hat{D}_{KL\,n,m}(p||q)
-        = \frac{d}{n} \sum_{i=1}^{n} \log \left ( \frac{\nu_k(i)}{\rho_k(i)} \right )
+        = \frac{d}{n}
+        \sum_{i=1}^{n} \log \left ( \frac{\nu_k(i)}{\rho_k(i)} \right )
         + \log\left (\frac{m}{n-1}\right )
 
     Where:
         * :math:`d` is the number of dimensions of the data.
-        * :math:`n` is the number of samples in *p*.
-        * :math:`\rho_k(i)` is the distance between :math:`x_i` and its *k*-NN in :math:`{x_j}_(j \neq i)`.
-        * :math:`\nu_k(i)` is the distance between :math:`x_i` and its *k*-NN in :math:`y_j`.
-        * :math:`m` is the number of points in *q*.
+        * :math:`n` is the number of samples in `p`.
+        * :math:`\rho_k(i)` is the distance between :math:`x_i` and its *k*-NN
+            in :math:`{x_j}_(j \neq i)`.
+        * :math:`\nu_k(i)` is the distance between :math:`x_i` and its *k*-NN
+            in :math:`y_j`.
+        * :math:`m` is the number of points in `q`.
 
     Parameters
     ----------
     p : numpy.ndarray
         Array of shape (n_samples, d_features)
     q : numpy.ndarray
         Array of shape (m_samples, d_features)
     k : int, optional
         no. of nearest neighbors to use
-    p_norm : int, optional
+    p_norm : float
         p (Minkowski) distance. p = 1 is the Manhattan distance,
-        p = 2 is the Euclidian distance, etc.
+        p = 2 is the Euclidian distance, etc. np.inf is the maximum
+        (Chebyshev) distance.
 
     Returns
     -------
     kld : float
         Kullback-Leibler divergence between p and q [in nats]
-    """
 
+    """
     n, m = len(p), len(q)
     d = len(p[0])
 
     rho, _ = KDTree(p).query(p, k + 1, p=p_norm)
     nu, _ = KDTree(q).query(p, k, p=p_norm)
     rho = rho.reshape(-1, k + 1)[:, -1]
     nu = nu.reshape(-1, k)[:, -1]
 
     kld = (d / n) * np.sum(np.log(nu / rho)) + np.log(m / (n - 1))
 
     return max(0.0, kld)
 
 
-def calc_knn_mutual_information(x, y, k=15):
-    r"""Calculates mutual information between X and Y using $k$-NN.
+def calc_knn_mutual_information(
+    x: np.ndarray,
+    y: np.ndarray,
+    k: int = 15,
+) -> float:
+    r"""Calculate mutual information between `x` and `y` using *k*-NN.
 
-    Estimates the mutual information between X and Y [in nats] using
-    the method of estimation proposed Kraskov et al. (2004). Both X and Y
+    Estimates the mutual information between `x` and `y` [in nats] using
+    the method of estimation proposed Kraskov et al. (2004). Both `x` and `y`
     can have d >= 1 which means they can have multiple features. By default,
-    the maximum norm (p-norm = ∞) and fifteen neighbors (k = 15) are used.
+    the maximum norm (`p-norm` = ∞) and fifteen neighbors (`k` = 15) are used.
     10.1103/PhysRevE.69.066138
 
     .. math::
         \hat{I}(X;Y)
-        = \psi(k) - \frac{1}{N} \sum_{i=1}^{N} \mathbb{E} \left[\psi(n_{i,x} + 1) + \psi(n_{i,y} + 1) \right]
+        = \psi(k) - \frac{1}{N}
+        \sum_{i=1}^{N} \mathbb{E} \left[\psi(n_{i,x} + 1)
+        + \psi(n_{i,y} + 1) \right]
         + \psi(N)
 
     Where:
         * :math:`\psi` is the digamma function.
         * :math:`N` is the number of samples.
         * :math:`\mathbb{E}` is the expectation operation.
-        * :math:`n_{i,x}` and :math:`n_{i,y}` are the number of neighbors
-        of every point within a given radius calculated as the distance to
+        * :math:`n_{i,x}` and :math:`n_{i,y}` are the number of neighbors of
+        every point within a given radius calculated as the distance to
         the *k*-th nearest neighbor in the joint X-Y space.
 
     Parameters
     ----------
     x : numpy.ndarray
         Array of shape (n_samples, d_features)
     y : numpy.ndarray
         Array of shape (n_samples, d_features)
     k : int, optional
         no. of nearest neighbors to use
 
+
     Returns
     -------
     mi : float
-        Mutual information between x and y [in nats]
-    """
+        Mutual information between `x` and `y` [in nats]
 
-    assert len(x) == len(y), "x and y must have the same number of samples."
+    """
+    assert len(x) == len(
+        y
+    ), "`x` and `y` must have the same number of samples."
 
     n_samples = len(x)
     xy = np.hstack((x, y))
 
     xy_tree = KDTree(xy)
     x_tree = KDTree(x)
     y_tree = KDTree(y)
 
     radius = xy_tree.query(xy, k=[k + 1], p=np.inf)[0].flatten()
-    nx = x_tree.query_ball_point(x, radius - 1e-12, p=np.inf, return_length=True)
-    ny = y_tree.query_ball_point(y, radius - 1e-12, p=np.inf, return_length=True)
-
-    mi = digamma(n_samples) + digamma(k) - np.mean(digamma(nx + 1) + digamma(ny + 1))
+    nx = x_tree.query_ball_point(
+        x,
+        radius - 1e-12,
+        p=np.inf,
+        return_length=True,
+    )
+    ny = y_tree.query_ball_point(
+        y,
+        radius - 1e-12,
+        p=np.inf,
+        return_length=True,
+    )
+
+    mi = (
+        digamma(n_samples)
+        + digamma(k)
+        - np.mean(digamma(nx + 1) + digamma(ny + 1))
+    )
 
     return max(0.0, mi)
```

### Comparing `unite_toolbox-0.1.6/unite_toolbox/utils/data_validation.py` & `unite_toolbox-0.1.9/unite_toolbox/utils/data_validation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,108 @@
+from __future__ import annotations
+
 import numpy as np
+from numpy.typing import ArrayLike
 from scipy import stats
 
 
-def find_repeats(data):
-    """Returns a boolean mask for repeat rows in data
-    where True is a repeated row.
+def validate_array(arr: ArrayLike) -> np.ndarray:
+    """Validate array.
+
+    Simple function to validate the dimensions and transform into a type
+    suitable for usage in the UNITE toolbox.
+
+    Parameters
+    ----------
+    arr : array_like
+        Array like object that can be transformed into a 2d Numpy array
+
+    Returns
+    -------
+    arr : numpy.ndarray
+        Array of shape (n_samples, d_features)
+
+    """
+    arr = np.asarray(arr, dtype=np.float64)
+    if arr.ndim != 2:
+        err = "UNITE only uses 2d arrays!"
+        raise TypeError(err)
+    return arr
+
+
+def find_repeats(data: np.ndarray) -> np.ndarray:
+    """Find repeats.
+
+    Returns a boolean mask for repeat rows in `data` where True is a repeated
+    row.
 
     Parameters
     ----------
     data : array_like
         2D array like of shape (n_samples, d_features)
 
     Returns
     -------
     mask : numpy.ndarray
-        Boolean array of shape (n_samples,)"""
+        Boolean array of shape (n_samples,)
 
-    data = np.asarray(data, dtype=np.float64)
-    _, inv, counts = np.unique(data, return_inverse=True, return_counts=True, axis=0)
+    """
+    _, inv, counts = np.unique(
+        data,
+        return_inverse=True,
+        return_counts=True,
+        axis=0,
+    )
     mask = np.where(counts[inv] > 1, True, False)
     return mask
 
 
-def add_noise_to_data(data):
-    """Adds noise to repeated rows in data.
+def add_noise_to_data(data: np.ndarray) -> np.ndarray:
+    """Add noise to repeated rows in `data`.
 
     Adds Gaussian noise to only the repeated rows in a 2D array.
-    The noise added is one order of magnitude below the order of magnitude
-    of the std. dev. of each specific column in the data. This was empirically
+    The noise added is one order of magnitude below the order of magnitude of
+    the std. dev. of each specific column in the data. This was empirically
     determined to be adequate for distance based measures.
 
     Parameters
     ----------
     data : array_like
         2D array like of shape (n_samples, d_features)
 
     Returns
     -------
     noisy_data : numpy.ndarray
-        2D array of shape (n_samples, d_features)"""
+        2D array of shape (n_samples, d_features)
 
+    """
     data = np.asarray(data, dtype=np.float64)
     _, d = data.shape
 
     # Determine the scale of the noise
     data_std = np.std(data, axis=0).reshape(1, -1) / 10
     noise_scale = 10 ** (np.floor(np.log10(np.abs(data_std))))
 
     # Generate only the required noise for the data
     mask = find_repeats(data)
-    noise = stats.multivariate_normal.rvs(cov=np.diag(noise_scale.flatten()), size=mask.sum(), random_state=42).reshape(-1, d)
+    noise = stats.multivariate_normal.rvs(
+        cov=np.diag(noise_scale.flatten()),
+        size=mask.sum(),
+        random_state=42,
+    ).reshape(-1, d)
 
     # Add noise to specific rows
     noisy_data = data.copy()
     noisy_data[mask] += noise
 
     return noisy_data
 
 
-def valida_data_kld(a, b, verbose=False):
-    """Validate data for kNN-based KLD
+def validate_data_kld(a: np.ndarray, b: np.ndarray) -> tuple[np.ndarray]:
+    """Validate data for kNN-based KLD.
 
     Eliminates repeated values from a and the joint array a-b to perform a
     distance based calculation of KLD, or other method which requires only
     unique values in two arrays.
 
     The code finds repeats in `a`, deletes them, and adds back the unique
     values that were repreated so that not a lot of the data is lost. A
@@ -79,25 +118,23 @@
 
     Returns
     -------
     p : numpy.ndarray
         2D array of shape (<=n_samples, d_features)
     q : numpy.ndarray
         2D array of shape (<=m_samples, d_features)
+
     """
     # Clean a
     mask_a = np.argwhere(find_repeats(a)).flatten()
     repeats = a[mask_a]
     p = np.delete(a, mask_a, axis=0)
     unique_repeats = np.unique(repeats, axis=0)
     p = np.vstack((p, unique_repeats))
 
     # Clean b
     nrows, _ = p.shape
     aux = np.vstack((p, b))
     mask_b = find_repeats(aux)[nrows:]
     q = b[~mask_b]
-    if verbose and (len(mask_a) > 0 or len(mask_b) > 0):
-        counts_a = len(mask_a) - unique_repeats.shape[0]
-        counts_b = len(np.argwhere(mask_b))
-        print(f"Removed: {counts_a} from `p` and {counts_b} from `q`")
+
     return p, q
```

### Comparing `unite_toolbox-0.1.6/unite_toolbox.egg-info/PKG-INFO` & `unite_toolbox-0.1.9/unite_toolbox.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unite_toolbox
-Version: 0.1.6
+Version: 0.1.9
 Summary: A toolbox for practical applications of information theory.
 Author-email: Manuel Álvarez Chaves <manuel.alvarezchaves@simtech.uni-stuttgart.de>, Anneli Guthke <anneli.guthke@simtech.uni-stuttgart.de>, Uwe Ehret <uwe.ehret@kit.edu>, Hoshin Gupta <hoshin@arizona.edu>
 Maintainer-email: Manuel Álvarez Chaves <manuel.alvarezchaves@simtech.uni-stuttgart.de>
 License: MIT License
 Project-URL: Documentation, https://unite-toolbox.readthedocs.io/
 Project-URL: Repository, https://github.com/manuel-alvarez-chaves/unite_toolbox
 Project-URL: Team, https://www.simtech.uni-stuttgart.de/exc/research/junior-research-groups/statistical-model-data-integration/
@@ -13,25 +13,26 @@
 License-File: LICENSE
 Requires-Dist: numpy>=1.25.0
 Requires-Dist: scipy>=1.12.0
 Requires-Dist: tqdm>=4.66.2
 Provides-Extra: dev
 Requires-Dist: jupyterlab>=4.1.2; extra == "dev"
 Requires-Dist: matplotlib>=3.8.3; extra == "dev"
-Requires-Dist: numpy>=1.26.4; extra == "dev"
-Requires-Dist: pandas>=2.2.1; extra == "dev"
-Requires-Dist: pyarrow>=15.0.0; extra == "dev"
-Requires-Dist: scipy>=1.12.0; extra == "dev"
-Requires-Dist: tqdm>=4.66.2; extra == "dev"
-Requires-Dist: xarray>=2024.2.0; extra == "dev"
+Requires-Dist: nbsphinx>=0.9.4; extra == "dev"
+Requires-Dist: pytest>=8.2.0; extra == "dev"
+Requires-Dist: ruff>=0.4.3; extra == "dev"
+Requires-Dist: Sphinx>=7.3.7; extra == "dev"
+Requires-Dist: sphinx_rtd_theme>=2.0.0; extra == "dev"
 
 # UNITE Toolbox
 
 ### Unified diagnostic evaluation of scientific models based on information theory
 
+![PyPI - Version](https://img.shields.io/pypi/v/unite_toolbox) ![Tests Badge](https://github.com/manuel-alvarez-chaves/unite_toolbox/actions/workflows/run-tests.yml/badge.svg) [![Coverage](https://codecov.io/gh/manuel-alvarez-chaves/unite_toolbox/graph/badge.svg?token=MWNDWXLZ9B)](https://codecov.io/gh/manuel-alvarez-chaves/unite_toolbox)
+
 The **UNITE Toolbox** is a Python library for incorporating _Information Theory_
 into data analysis and modeling workflows.
 The toolbox collects different methods of estimating information-theoretic quantities
 in one easy-to-use Python package.
 Currently, UNITE includes functions to calculate entropy $H(X)$,
 Kullback-Leibler divergence $D_{KL}(p||q)$, and mutual information $I(X; Y)$,
 using three methods:
```

### Comparing `unite_toolbox-0.1.6/unite_toolbox.egg-info/SOURCES.txt` & `unite_toolbox-0.1.9/unite_toolbox.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
+tests/test_density.py
+tests/test_entropy.py
+tests/test_kld.py
+tests/test_mutual_information.py
+tests/test_utils.py
 unite_toolbox/__init__.py
 unite_toolbox/bin_estimators.py
 unite_toolbox/kde_estimators.py
 unite_toolbox/knn_estimators.py
 unite_toolbox.egg-info/PKG-INFO
 unite_toolbox.egg-info/SOURCES.txt
 unite_toolbox.egg-info/dependency_links.txt
 unite_toolbox.egg-info/requires.txt
 unite_toolbox.egg-info/top_level.txt
 unite_toolbox/utils/__init__.py
 unite_toolbox/utils/bootstrapping.py
 unite_toolbox/utils/data_validation.py
-unite_toolbox/utils/marginal_information.py
+unite_toolbox/utils/marginal_scores.py
 unite_toolbox/utils/sampling.py
```

