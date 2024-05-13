# Comparing `tmp/dsp_cvxpy-0.1.1.tar.gz` & `tmp/dsp-cvxpy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsp_cvxpy-0.1.1.tar", last modified: Mon May 13 05:30:55 2024, max compression
+gzip compressed data, was "dsp-cvxpy-0.2.0.tar", last modified: Mon Jan 22 17:43:42 2024, max compression
```

## Comparing `dsp_cvxpy-0.1.1.tar` & `dsp-cvxpy-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:30:55.275797 dsp_cvxpy-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-05-13 05:27:34.000000 dsp_cvxpy-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7857 2024-05-13 05:30:55.275797 dsp_cvxpy-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-05-13 05:27:34.000000 dsp_cvxpy-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:30:55.271797 dsp_cvxpy-0.1.1/dsp/
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-13 05:27:34.000000 dsp_cvxpy-0.1.1/dsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18178 2024-05-13 05:27:34.000000 dsp_cvxpy-0.1.1/dsp/cone_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-13 05:27:34.000000 dsp_cvxpy-0.1.1/dsp/cvxpy_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-13 05:27:34.000000 dsp_cvxpy-0.1.1/dsp/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    12124 2024-05-13 05:27:34.000000 dsp_cvxpy-0.1.1/dsp/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9636 2024-05-13 05:27:34.000000 dsp_cvxpy-0.1.1/dsp/problem.py
--rw-r--r--   0 runner    (1001) docker     (127)    23048 2024-05-13 05:27:34.000000 dsp_cvxpy-0.1.1/dsp/saddle_atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)     7600 2024-05-13 05:27:34.000000 dsp_cvxpy-0.1.1/dsp/saddle_extremum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-13 05:27:34.000000 dsp_cvxpy-0.1.1/dsp/semi_infinite_canon.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-13 05:27:34.000000 dsp_cvxpy-0.1.1/dsp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:30:55.275797 dsp_cvxpy-0.1.1/dsp_cvxpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7857 2024-05-13 05:30:55.000000 dsp_cvxpy-0.1.1/dsp_cvxpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-13 05:30:55.000000 dsp_cvxpy-0.1.1/dsp_cvxpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 05:30:55.000000 dsp_cvxpy-0.1.1/dsp_cvxpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-13 05:30:55.000000 dsp_cvxpy-0.1.1/dsp_cvxpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-13 05:30:55.000000 dsp_cvxpy-0.1.1/dsp_cvxpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 05:28:11.000000 dsp_cvxpy-0.1.1/dsp_cvxpy.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-13 05:27:34.000000 dsp_cvxpy-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-13 05:30:55.275797 dsp_cvxpy-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:30:55.275797 dsp_cvxpy-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 05:27:34.000000 dsp_cvxpy-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-13 05:27:34.000000 dsp_cvxpy-0.1.1/tests/test_cone_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     9189 2024-05-13 05:27:34.000000 dsp_cvxpy-0.1.1/tests/test_cvxpy_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    17008 2024-05-13 05:27:34.000000 dsp_cvxpy-0.1.1/tests/test_dsp.py
--rw-r--r--   0 runner    (1001) docker     (127)    17142 2024-05-13 05:27:34.000000 dsp_cvxpy-0.1.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     8660 2024-05-13 05:27:34.000000 dsp_cvxpy-0.1.1/tests/test_is_dsp.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-13 05:27:34.000000 dsp_cvxpy-0.1.1/tests/test_minimizemaximize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-05-13 05:27:34.000000 dsp_cvxpy-0.1.1/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-13 05:27:34.000000 dsp_cvxpy-0.1.1/tests/test_pathology.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-13 05:27:34.000000 dsp_cvxpy-0.1.1/tests/test_quasidef_quad_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-13 05:27:34.000000 dsp_cvxpy-0.1.1/tests/test_saddle_quad_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-13 05:27:34.000000 dsp_cvxpy-0.1.1/tests/test_snippets.py
--rw-r--r--   0 runner    (1001) docker     (127)    10192 2024-05-13 05:27:34.000000 dsp_cvxpy-0.1.1/tests/test_weighted_log_sum_exp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-05-13 05:27:34.000000 dsp_cvxpy-0.1.1/tests/test_weighted_norm2.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-01-22 17:43:42.105292 dsp-cvxpy-0.2.0/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10760 2024-01-22 17:38:17.000000 dsp-cvxpy-0.2.0/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     7805 2024-01-22 17:43:42.105292 dsp-cvxpy-0.2.0/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7302 2024-01-22 17:38:17.000000 dsp-cvxpy-0.2.0/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-01-22 17:43:42.097293 dsp-cvxpy-0.2.0/dsp/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      675 2024-01-22 17:38:17.000000 dsp-cvxpy-0.2.0/dsp/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17995 2024-01-22 17:38:17.000000 dsp-cvxpy-0.2.0/dsp/cone_transforms.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      904 2024-01-22 17:38:17.000000 dsp-cvxpy-0.2.0/dsp/cvxpy_integration.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1662 2024-01-22 17:38:17.000000 dsp-cvxpy-0.2.0/dsp/local.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12127 2024-01-22 17:38:17.000000 dsp-cvxpy-0.2.0/dsp/parser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9631 2024-01-22 17:38:17.000000 dsp-cvxpy-0.2.0/dsp/problem.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22957 2024-01-22 17:38:17.000000 dsp-cvxpy-0.2.0/dsp/saddle_atoms.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7606 2024-01-22 17:38:17.000000 dsp-cvxpy-0.2.0/dsp/saddle_extremum.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1047 2024-01-22 17:38:17.000000 dsp-cvxpy-0.2.0/dsp/semi_infinite_canon.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      240 2024-01-22 17:38:17.000000 dsp-cvxpy-0.2.0/dsp/utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-01-22 17:43:42.105292 dsp-cvxpy-0.2.0/dsp_cvxpy.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     7805 2024-01-22 17:43:42.000000 dsp-cvxpy-0.2.0/dsp_cvxpy.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      792 2024-01-22 17:43:42.000000 dsp-cvxpy-0.2.0/dsp_cvxpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-01-22 17:43:42.000000 dsp-cvxpy-0.2.0/dsp_cvxpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       34 2024-01-22 17:43:42.000000 dsp-cvxpy-0.2.0/dsp_cvxpy.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       10 2024-01-22 17:43:42.000000 dsp-cvxpy-0.2.0/dsp_cvxpy.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-01-22 17:43:41.000000 dsp-cvxpy-0.2.0/dsp_cvxpy.egg-info/zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      281 2024-01-22 17:38:17.000000 dsp-cvxpy-0.2.0/pyproject.toml
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      657 2024-01-22 17:43:42.105292 dsp-cvxpy-0.2.0/setup.cfg
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-01-22 17:43:42.105292 dsp-cvxpy-0.2.0/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-01-22 17:38:55.000000 dsp-cvxpy-0.2.0/tests/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      364 2024-01-22 17:38:17.000000 dsp-cvxpy-0.2.0/tests/test_cone_transforms.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9189 2024-01-22 17:38:17.000000 dsp-cvxpy-0.2.0/tests/test_cvxpy_integration.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17008 2024-01-22 17:38:17.000000 dsp-cvxpy-0.2.0/tests/test_dsp.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11189 2024-01-22 17:38:17.000000 dsp-cvxpy-0.2.0/tests/test_examples.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8660 2024-01-22 17:38:17.000000 dsp-cvxpy-0.2.0/tests/test_is_dsp.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      740 2024-01-22 17:38:17.000000 dsp-cvxpy-0.2.0/tests/test_minimizemaximize.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4136 2024-01-22 17:38:17.000000 dsp-cvxpy-0.2.0/tests/test_parser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1910 2024-01-22 17:38:17.000000 dsp-cvxpy-0.2.0/tests/test_pathology.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1433 2024-01-22 17:38:17.000000 dsp-cvxpy-0.2.0/tests/test_quasidef_quad_form.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2414 2024-01-22 17:38:17.000000 dsp-cvxpy-0.2.0/tests/test_saddle_quad_form.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3585 2024-01-22 17:38:17.000000 dsp-cvxpy-0.2.0/tests/test_snippets.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10192 2024-01-22 17:38:17.000000 dsp-cvxpy-0.2.0/tests/test_weighted_log_sum_exp.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4621 2024-01-22 17:38:17.000000 dsp-cvxpy-0.2.0/tests/test_weighted_norm2.py
```

### Comparing `dsp_cvxpy-0.1.1/LICENSE` & `dsp-cvxpy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsp_cvxpy-0.1.1/PKG-INFO` & `dsp-cvxpy-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsp-cvxpy
-Version: 0.1.1
+Version: 0.2.0
 Summary: Disciplined Saddle Programming
 Home-page: https://github.com/cvxgrp/dsp
 Author: Philipp Schiele, Eric Luxenberg, Stephen Boyd
 Author-email: philipp.schiele@stat.uni-muenchen.de, ericlux@stanford.edu, boyd@stanford.edu
 License: Apache License, Version 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -176,16 +176,15 @@
 x.value # array([0.66666667, 0.33333333])
 ```
 
 ## Citation
 If you want to reference DSP in your research, please consider citing us by using the following BibTeX:
 
 ```BibTeX
-@article{schiele2024dsp,
+@misc{schiele2023dsp,
   title = {Disciplined Saddle Programming},
   author = {Schiele, Philipp and Luxenberg, Eric and Boyd, Stephen},
-  journal = {Transactions on Machine Learning Research},
-  year = {2024},
-  pages = {1--25},
-  url = {https://openreview.net/forum?id=KhMLfEIoUm},
+  year = {2023},
+  doi = {10.48550/arXiv.2301.13427},
+  url = {https://arxiv.org/abs/2301.13427},
 }
 ```
```

### Comparing `dsp_cvxpy-0.1.1/README.md` & `dsp-cvxpy-0.2.0/dsp_cvxpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: dsp-cvxpy
+Version: 0.2.0
+Summary: Disciplined Saddle Programming
+Home-page: https://github.com/cvxgrp/dsp
+Author: Philipp Schiele, Eric Luxenberg, Stephen Boyd
+Author-email: philipp.schiele@stat.uni-muenchen.de, ericlux@stanford.edu, boyd@stanford.edu
+License: Apache License, Version 2.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: cvxpy>=1.3
+Requires-Dist: numpy
+Requires-Dist: scipy
+Provides-Extra: dev
+Requires-Dist: tox; extra == "dev"
+
 # DSP -  Disciplined Saddle Programming
 [![build](https://github.com/cvxgrp/dsp/actions/workflows/build.yml/badge.svg)](https://github.com/cvxgrp/dsp/actions/workflows/build.yml)
 [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=dsp&metric=coverage)](https://sonarcloud.io/summary/new_code?id=dsp)
 
 A CVXPY extension for Disciplined Saddle Programming.
 DSP allows solving convex-concave saddle point problems, and more generally
 convex optimization problems we refer to as _saddle problems_, which include the partial
@@ -160,16 +176,15 @@
 x.value # array([0.66666667, 0.33333333])
 ```
 
 ## Citation
 If you want to reference DSP in your research, please consider citing us by using the following BibTeX:
 
 ```BibTeX
-@article{schiele2024dsp,
+@misc{schiele2023dsp,
   title = {Disciplined Saddle Programming},
   author = {Schiele, Philipp and Luxenberg, Eric and Boyd, Stephen},
-  journal = {Transactions on Machine Learning Research},
-  year = {2024},
-  pages = {1--25},
-  url = {https://openreview.net/forum?id=KhMLfEIoUm},
+  year = {2023},
+  doi = {10.48550/arXiv.2301.13427},
+  url = {https://arxiv.org/abs/2301.13427},
 }
 ```
```

### Comparing `dsp_cvxpy-0.1.1/dsp/__init__.py` & `dsp-cvxpy-0.2.0/dsp/__init__.py`

 * *Files identical despite different names*

### Comparing `dsp_cvxpy-0.1.1/dsp/cone_transforms.py` & `dsp-cvxpy-0.2.0/dsp/cone_transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
         all_constraints = [K.constraints for K in reprs]
         constraints = list(itertools.chain.from_iterable(all_constraints))
 
         offset = np.sum([K.offset for K in reprs])
 
         def f_concave(x: np.ndarray) -> cp.Expression:
-            nones = any(K.concave_expr(x) is None for K in reprs)
+            nones = any([K.concave_expr(x) is None for K in reprs])
             return cp.sum([K.concave_expr(x) for K in reprs]) if not nones else None
 
         concave_expr = f_concave
 
         y_constraints = list(itertools.chain.from_iterable([K.y_constraints for K in reprs]))
 
         return KRepresentation(
@@ -70,19 +70,14 @@
             concave_expr=lambda x: self.concave_expr(x) * scalar
             if self.concave_expr(x) is not None
             else None,
         )
 
     @classmethod
     def constant_repr(cls, value: float | int) -> KRepresentation:
-        if not isinstance(value, (float, int)):
-            assert value.size == 1
-            assert isinstance(value, np.ndarray)
-            value = np.squeeze(value)
-
         return KRepresentation(
             f=cp.Constant(0),
             t=cp.Constant(0),
             constraints=[],
             offset=float(value),
             concave_expr=lambda x: float(value),
         )
@@ -205,24 +200,25 @@
     return KRepresentation(f=f, t=t, constraints=K_constr)
 
 
 def K_repr_ax(a: cp.Expression) -> KRepresentation:
     assert a.is_convex()
     assert a.size == 1
 
-    f = cp.Variable(name="f_ax")
+    f = cp.Constant(0)
     t = cp.Variable(name="t_ax")
 
-    constraints = [t >= a, f == 0]
+    constraints = [t >= a]
 
     return KRepresentation(f=f, t=t, constraints=constraints, concave_expr=lambda x: a.value)
 
 
 class LocalToGlob:
     def __init__(self, x_variables: list[cp.Variable], y_variables: list[cp.Variable]) -> None:
+
         self.outer_x_vars = x_variables
         self.var_to_glob: dict[int, tuple[int, int]] = {}
 
         self.x_size = self.add_vars_to_map(x_variables)
         self.y_size = self.add_vars_to_map(y_variables)
 
     def add_vars_to_map(self, variables: list[cp.Variable]) -> int:
@@ -296,14 +292,15 @@
 
 def K_repr_FxGy(
     Fx: cp.Expression,
     Gy: cp.Expression,
     local_to_glob: LocalToGlob,
     switched: bool = False,
 ) -> KRepresentation:
+
     z = cp.Variable(Fx.shape)
     constraints = [z >= Fx]
 
     K_repr_zGy = K_repr_x_Gy(Gy, z, local_to_glob, switched=switched)
 
     K_unswitched = KRepresentation(
         f=K_repr_zGy.f, t=K_repr_zGy.t, constraints=constraints + K_repr_zGy.constraints
@@ -334,14 +331,15 @@
 
     return KRepresentation(f=C.T @ Fx, t=Fx.T @ d, constraints=[])
 
 
 def get_cone_repr(
     const: list[Constraint], variables: list[cp.Variable]
 ) -> tuple[dict[int, np.ndarray], np.ndarray, ConeDims]:
+
     assert all(isinstance(v, cp.Variable) for v in variables)
 
     # TODO: CVXPY does not have a stable API for getting the cone representation that is
     #  solver independent. We use SCS in line with the CVXPY documentation.
     #  Compare https://www.cvxpy.org/tutorial/advanced/index.html#getting-the-standard-form
 
     aux_prob = cp.Problem(cp.Minimize(0), const)
@@ -502,14 +500,15 @@
 
 def create_sparse_matrix_from_columns(
     shape: tuple[int, int],
     variables: list[cp.Variable],
     local_to_glob: LocalToGlob,
     var_to_mat_mapping: dict[int, sp.csc_matrix],
 ) -> sp.csc_matrix:
+
     cols = []
     for v in variables:
         start, end = local_to_glob.var_to_glob[v.id]
         cols.append((start, end, v.id))
 
     cols = sorted(cols, key=lambda x: x[0])
```

### Comparing `dsp_cvxpy-0.1.1/dsp/cvxpy_integration.py` & `dsp-cvxpy-0.2.0/dsp/cvxpy_integration.py`

 * *Files identical despite different names*

### Comparing `dsp_cvxpy-0.1.1/dsp/local.py` & `dsp-cvxpy-0.2.0/dsp/local.py`

 * *Files identical despite different names*

### Comparing `dsp_cvxpy-0.1.1/dsp/parser.py` & `dsp-cvxpy-0.2.0/dsp/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         f"Specify curvature of these variables as "
         f"SaddleProblem(obj, constraints, minimization_vars, maximization_vars)."
     )
 
 
 class Parser:
     def __init__(self, convex_vars: set[cp.Variable], concave_vars: set[cp.Variable]) -> None:
+
         self.convex_vars: set[cp.Variable] = convex_vars
         self.concave_vars: set[cp.Variable] = concave_vars
         if self.convex_vars & self.concave_vars:
             raise DSPError("Cannot have variables in both maximization_vars and minimization_vars.")
 
         self.affine_vars: set[cp.Variable] = set()
         self._x_constraints = None
@@ -165,14 +166,15 @@
 
     def parse_expr_variables(self, expr: cp.Expression, switched: bool, **kwargs: dict) -> None:
         self._parse_expr(expr, switched, repr_parse=False, **kwargs)
 
     def parse_expr_repr(
         self, expr: cp.Expression, switched: bool, local_to_glob: LocalToGlob
     ) -> KRepresentation:
+
         K_repr = self._parse_expr(expr, switched, repr_parse=True, local_to_glob=local_to_glob)
         assert isinstance(K_repr, KRepresentation)
         return K_repr
 
     @staticmethod
     def contains_curvature_lumping(expr: cp.Expression) -> bool:
         """
@@ -186,14 +188,15 @@
             return affine_term and non_affine_term
         else:
             return any(Parser.contains_curvature_lumping(expr_arg) for expr_arg in expr.args)
 
     def _parse_expr(
         self, expr: cp.Expression, switched: bool, repr_parse: bool, **kwargs: dict
     ) -> KRepresentation | None:
+
         # constant
         if not expr.variables():
             assert expr.size == 1
             return (
                 KRepresentation.constant_repr(expr.value * (1 if not switched else -1))
                 if repr_parse
                 else None
```

### Comparing `dsp_cvxpy-0.1.1/dsp/problem.py` & `dsp-cvxpy-0.2.0/dsp/problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,15 @@
     def dualized_problem(
         self,
         obj_expr: cp.Expression,
         constraints: list[Constraint],
         minimization_vars: Iterable[cp.Variable],
         maximization_vars: Iterable[cp.Variable],
     ) -> tuple[list[Constraint], Objective]:
+
         parser = initialize_parser(obj_expr, minimization_vars, maximization_vars, constraints)
 
         local_to_glob_y = LocalToGlob(parser.convex_vars, parser.concave_vars)
 
         K_repr = parser.parse_expr_repr(obj_expr, switched=False, local_to_glob=local_to_glob_y)
 
         single_obj, constraints = minimax_to_min(
@@ -142,15 +143,15 @@
         been successfully solved.
         """
         return self._value
 
     def is_dsp(self) -> bool:
         # try to form x_prob and catch the exception
         try:
-            self.x_prob  # noqa
+            self.x_prob
             return True
         except DSPError:
             return False
 
     def convex_variables(self) -> list[cp.Variable]:
         parser = initialize_parser(
             self.obj_expr, self._minimization_vars, self._maximization_vars, self._constraints_
@@ -264,12 +265,12 @@
 
 
 def is_dsp(obj: cp.Problem | SaddlePointProblem | cp.Expression) -> bool:
     if isinstance(obj, SaddlePointProblem):
         return obj.is_dsp()
     elif isinstance(obj, cp.Problem):
         all_SE_atoms = get_problem_SE_atoms(obj)
-        return obj.is_dcp() and all(atom.is_dsp() for atom in all_SE_atoms)
+        return obj.is_dcp() and all([atom.is_dsp() for atom in all_SE_atoms])
     elif isinstance(obj, cp.Expression):
         return is_dsp_expr(obj)
     else:
         return False
```

### Comparing `dsp_cvxpy-0.1.1/dsp/saddle_atoms.py` & `dsp-cvxpy-0.2.0/dsp/saddle_atoms.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         raise NotImplementedError
 
     @abstractmethod
     def is_dsp(self) -> bool:
         raise NotImplementedError
 
     def numeric(self, values: list[np.ndarray | None]) -> np.ndarray | None:
-        if any(v is None for v in values):
+        if any([v is None for v in values]):
             return None
         return self._numeric(values)
 
     @abstractmethod
     def _numeric(self, values: list[np.ndarray]) -> np.ndarray:
         raise NotImplementedError
 
@@ -97,16 +97,15 @@
         assert isinstance(Fx, cp.Expression)
         assert isinstance(Gy, cp.Expression)
 
         self.bilinear = Fx.is_affine() and Gy.is_affine()
         if (not self.bilinear) and (not Gy.is_nonneg()):
             warnings.warn(
                 "Gy is non-positive. The y domain of saddle_inner is Gy >="
-                " 0. The implicit constraint Gy >= 0 will be added to the problem.",
-                stacklevel=1,
+                " 0. The implicit constraint Gy >= 0 will be added to the problem."
             )
 
         self.Fx = Fx
         self.Gy = Gy
 
         assert len(Fx.shape) <= 1 or (
             len(Fx.shape) == 2 and min(Fx.shape) == 1
@@ -223,16 +222,15 @@
         assert isinstance(exponents, cp.Expression)
         assert isinstance(weights, cp.Expression)
 
         if not weights.is_nonneg():
             warnings.warn(
                 "Weights are non-positive. The domain of weighted log-sum-exp is y >="
                 " 0. The implicit constraint y >= 0 will be added to"
-                " the problem.",
-                stacklevel=1,
+                " the problem."
             )
 
         self.concave_composition = not weights.is_affine()
 
         self.exponents = exponents
         self.weights = weights
 
@@ -558,16 +556,15 @@
         assert isinstance(x, cp.Expression)
         assert isinstance(y, cp.Expression)
 
         if not y.is_nonneg():
             warnings.warn(
                 "Weights are non-positive. The domain of weighted_norm2 is y >="
                 " 0. The implicit constraint y >= 0 will be added to"
-                " the problem.",
-                stacklevel=1,
+                " the problem."
             )
 
         self.concave_composition = not y.is_affine()
 
         self.x = x
         self.y = y
```

### Comparing `dsp_cvxpy-0.1.1/dsp/saddle_extremum.py` & `dsp-cvxpy-0.2.0/dsp/saddle_extremum.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 class SaddleExtremum(Atom):
     def __init__(
         self,
         f: cp.Expression,
         constraints: Iterable[cp.Constraint],
     ) -> None:
+
         self.f = f
         self._parser = None
 
         self._validate_arguments(constraints)
         self.constraints = list(constraints)
         self.other_variables = [v for v in f.variables() if not isinstance(v, dsp.LocalVariable)]
 
@@ -39,15 +40,15 @@
                         "All variables in constraints must be instances of LocalVariable."
                     )
         assert isinstance(self.f, cp.Expression)
 
     def is_dsp(self) -> bool:
         try:
             self.parser  # noqa
-            return all(c.is_dcp() for c in self.constraints)
+            return all([c.is_dcp() for c in self.constraints])
         except DSPError:
             return False
 
     def is_incr(self, idx: int) -> bool:
         return False
 
     def is_decr(self, idx: int) -> bool:
@@ -76,14 +77,15 @@
     r"""sup_{y\in Y}f(x,y)"""
 
     def __init__(
         self,
         f: cp.Expression,
         constraints: Iterable[cp.Constraint],
     ) -> None:
+
         super().__init__(f, constraints)
 
         self._concave_vars = set(filter(lambda v: isinstance(v, dsp.LocalVariable), f.variables()))
         self._concave_vars |= set(itertools.chain.from_iterable(c.variables() for c in constraints))
 
         for v in self._concave_vars:
             v.expr = self
@@ -93,14 +95,15 @@
 
     def concave_variables(self) -> list[cp.Variable]:
         return sorted(self._concave_vars, key=lambda x: x.id)
 
     @property
     def parser(self) -> Parser:
         if self._parser is None:
+
             parser = initialize_parser(
                 self.f,
                 minimization_vars=self.other_variables,
                 maximization_vars=self._concave_vars,
                 constraints=self.constraints,
             )
 
@@ -148,14 +151,15 @@
     r"""inf_{x\in X}f(x,y)"""
 
     def __init__(
         self,
         f: cp.Expression,
         constraints: Iterable[cp.Constraint],
     ) -> None:
+
         super().__init__(f, constraints)
 
         self._convex_vars = set(filter(lambda v: isinstance(v, dsp.LocalVariable), f.variables()))
         self._convex_vars |= set(itertools.chain.from_iterable(c.variables() for c in constraints))
 
         for v in self._convex_vars:
             v.expr = self
```

### Comparing `dsp_cvxpy-0.1.1/dsp/semi_infinite_canon.py` & `dsp-cvxpy-0.2.0/dsp/semi_infinite_canon.py`

 * *Files identical despite different names*

### Comparing `dsp_cvxpy-0.1.1/dsp_cvxpy.egg-info/PKG-INFO` & `dsp-cvxpy-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: dsp-cvxpy
-Version: 0.1.1
-Summary: Disciplined Saddle Programming
-Home-page: https://github.com/cvxgrp/dsp
-Author: Philipp Schiele, Eric Luxenberg, Stephen Boyd
-Author-email: philipp.schiele@stat.uni-muenchen.de, ericlux@stanford.edu, boyd@stanford.edu
-License: Apache License, Version 2.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: cvxpy>=1.3
-Requires-Dist: numpy
-Requires-Dist: scipy
-Provides-Extra: dev
-Requires-Dist: tox; extra == "dev"
-
 # DSP -  Disciplined Saddle Programming
 [![build](https://github.com/cvxgrp/dsp/actions/workflows/build.yml/badge.svg)](https://github.com/cvxgrp/dsp/actions/workflows/build.yml)
 [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=dsp&metric=coverage)](https://sonarcloud.io/summary/new_code?id=dsp)
 
 A CVXPY extension for Disciplined Saddle Programming.
 DSP allows solving convex-concave saddle point problems, and more generally
 convex optimization problems we refer to as _saddle problems_, which include the partial
@@ -176,16 +160,15 @@
 x.value # array([0.66666667, 0.33333333])
 ```
 
 ## Citation
 If you want to reference DSP in your research, please consider citing us by using the following BibTeX:
 
 ```BibTeX
-@article{schiele2024dsp,
+@misc{schiele2023dsp,
   title = {Disciplined Saddle Programming},
   author = {Schiele, Philipp and Luxenberg, Eric and Boyd, Stephen},
-  journal = {Transactions on Machine Learning Research},
-  year = {2024},
-  pages = {1--25},
-  url = {https://openreview.net/forum?id=KhMLfEIoUm},
+  year = {2023},
+  doi = {10.48550/arXiv.2301.13427},
+  url = {https://arxiv.org/abs/2301.13427},
 }
 ```
```

### Comparing `dsp_cvxpy-0.1.1/dsp_cvxpy.egg-info/SOURCES.txt` & `dsp-cvxpy-0.2.0/dsp_cvxpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dsp_cvxpy-0.1.1/setup.cfg` & `dsp-cvxpy-0.2.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dsp-cvxpy
-version = 0.1.1
+version = 0.2.0
 author = Philipp Schiele, Eric Luxenberg, Stephen Boyd
 author_email = philipp.schiele@stat.uni-muenchen.de, ericlux@stanford.edu, boyd@stanford.edu
 url = https://github.com/cvxgrp/dsp
 description = Disciplined Saddle Programming
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache License, Version 2.0
@@ -20,11 +20,14 @@
 
 [options.extras_require]
 dev = tox
 
 [options.package_data]
 * = README.md
 
+[flake8]
+max-line-length = 100
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `dsp_cvxpy-0.1.1/tests/test_cvxpy_integration.py` & `dsp-cvxpy-0.2.0/tests/test_cvxpy_integration.py`

 * *Files identical despite different names*

### Comparing `dsp_cvxpy-0.1.1/tests/test_dsp.py` & `dsp-cvxpy-0.2.0/tests/test_dsp.py`

 * *Files identical despite different names*

### Comparing `dsp_cvxpy-0.1.1/tests/test_is_dsp.py` & `dsp-cvxpy-0.2.0/tests/test_is_dsp.py`

 * *Files identical despite different names*

### Comparing `dsp_cvxpy-0.1.1/tests/test_minimizemaximize.py` & `dsp-cvxpy-0.2.0/tests/test_minimizemaximize.py`

 * *Files identical despite different names*

### Comparing `dsp_cvxpy-0.1.1/tests/test_parser.py` & `dsp-cvxpy-0.2.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `dsp_cvxpy-0.1.1/tests/test_pathology.py` & `dsp-cvxpy-0.2.0/tests/test_pathology.py`

 * *Files identical despite different names*

### Comparing `dsp_cvxpy-0.1.1/tests/test_quasidef_quad_form.py` & `dsp-cvxpy-0.2.0/tests/test_quasidef_quad_form.py`

 * *Files identical despite different names*

### Comparing `dsp_cvxpy-0.1.1/tests/test_saddle_quad_form.py` & `dsp-cvxpy-0.2.0/tests/test_saddle_quad_form.py`

 * *Files identical despite different names*

### Comparing `dsp_cvxpy-0.1.1/tests/test_snippets.py` & `dsp-cvxpy-0.2.0/tests/test_snippets.py`

 * *Files identical despite different names*

### Comparing `dsp_cvxpy-0.1.1/tests/test_weighted_log_sum_exp.py` & `dsp-cvxpy-0.2.0/tests/test_weighted_log_sum_exp.py`

 * *Files identical despite different names*

### Comparing `dsp_cvxpy-0.1.1/tests/test_weighted_norm2.py` & `dsp-cvxpy-0.2.0/tests/test_weighted_norm2.py`

 * *Files identical despite different names*

