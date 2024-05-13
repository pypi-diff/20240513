# Comparing `tmp/fenics_beat-0.0.4.tar.gz` & `tmp/fenics_beat-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenics_beat-0.0.4.tar", last modified: Fri Apr 26 08:41:49 2024, max compression
+gzip compressed data, was "fenics_beat-0.0.5.tar", last modified: Mon May 13 18:44:05 2024, max compression
```

## Comparing `fenics_beat-0.0.4.tar` & `fenics_beat-0.0.5.tar`

### file list

```diff
@@ -1,44 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:49.108979 fenics_beat-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-26 08:41:49.108979 fenics_beat-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 08:41:49.108979 fenics_beat-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:49.096979 fenics_beat-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:49.096979 fenics_beat-0.0.4/src/beat/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/bidomain_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:49.096979 fenics_beat-0.0.4/src/beat/cellmodels/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/cellmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22492 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/cellmodels/beeler_reuter_1977.py
--rw-r--r--   0 runner    (1001) docker     (127)     8725 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/cellmodels/fitzhughnagumo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:49.100979 fenics_beat-0.0.4/src/beat/cellmodels/tentusscher_panfilov_2006/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/cellmodels/tentusscher_panfilov_2006/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    68630 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/cellmodels/tentusscher_panfilov_2006/endo.py
--rw-r--r--   0 runner    (1001) docker     (127)    68719 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/cellmodels/tentusscher_panfilov_2006/epi.py
--rw-r--r--   0 runner    (1001) docker     (127)    68702 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/cellmodels/tentusscher_panfilov_2006/mid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:49.100979 fenics_beat-0.0.4/src/beat/cellmodels/torord_dyn_chloride/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/cellmodels/torord_dyn_chloride/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   286750 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/cellmodels/torord_dyn_chloride/endo.py
--rw-r--r--   0 runner    (1001) docker     (127)   286758 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/cellmodels/torord_dyn_chloride/epi.py
--rw-r--r--   0 runner    (1001) docker     (127)   286743 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/cellmodels/torord_dyn_chloride/mid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/ecg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/monodomain_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/monodomain_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/odesolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:49.104979 fenics_beat-0.0.4/src/fenics_beat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-26 08:41:49.000000 fenics_beat-0.0.4/src/fenics_beat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-26 08:41:49.000000 fenics_beat-0.0.4/src/fenics_beat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 08:41:49.000000 fenics_beat-0.0.4/src/fenics_beat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-26 08:41:49.000000 fenics_beat-0.0.4/src/fenics_beat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 08:41:49.000000 fenics_beat-0.0.4/src/fenics_beat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:49.104979 fenics_beat-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/tests/test_bidomain_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/tests/test_cellmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/tests/test_ecg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/tests/test_monodomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     8744 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/tests/test_monodomain_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/tests/test_odesolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:44:05.519651 fenics_beat-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-13 18:44:05.519651 fenics_beat-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:44:05.507651 fenics_beat-0.0.5/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/licenses/LICENSE_dolfin_pyvista_adapter
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 18:44:05.519651 fenics_beat-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:44:05.507651 fenics_beat-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:44:05.511651 fenics_beat-0.0.5/src/beat/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9724 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/bidomain_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:44:05.511651 fenics_beat-0.0.5/src/beat/cellmodels/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/cellmodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22492 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/cellmodels/beeler_reuter_1977.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8725 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/cellmodels/fitzhughnagumo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:44:05.511651 fenics_beat-0.0.5/src/beat/cellmodels/tentusscher_panfilov_2006/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/cellmodels/tentusscher_panfilov_2006/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68630 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/cellmodels/tentusscher_panfilov_2006/endo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68719 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/cellmodels/tentusscher_panfilov_2006/epi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68702 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/cellmodels/tentusscher_panfilov_2006/mid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:44:05.515651 fenics_beat-0.0.5/src/beat/cellmodels/torord_dyn_chloride/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/cellmodels/torord_dyn_chloride/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   286750 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/cellmodels/torord_dyn_chloride/endo.py
+-rw-r--r--   0 runner    (1001) docker     (127)   286758 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/cellmodels/torord_dyn_chloride/epi.py
+-rw-r--r--   0 runner    (1001) docker     (127)   286743 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/cellmodels/torord_dyn_chloride/mid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/ecg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/monodomain_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/monodomain_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/odesolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/single_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:44:05.515651 fenics_beat-0.0.5/src/fenics_beat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-13 18:44:05.000000 fenics_beat-0.0.5/src/fenics_beat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-13 18:44:05.000000 fenics_beat-0.0.5/src/fenics_beat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 18:44:05.000000 fenics_beat-0.0.5/src/fenics_beat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-13 18:44:05.000000 fenics_beat-0.0.5/src/fenics_beat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-13 18:44:05.000000 fenics_beat-0.0.5/src/fenics_beat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:44:05.515651 fenics_beat-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/tests/test_bidomain_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/tests/test_cellmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/tests/test_ecg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/tests/test_monodomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8744 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/tests/test_monodomain_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/tests/test_odesolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/tests/test_single_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/tests/test_utils.py
```

### Comparing `fenics_beat-0.0.4/LICENSE` & `fenics_beat-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.4/PKG-INFO` & `fenics_beat-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,54 @@
 Metadata-Version: 2.1
 Name: fenics-beat
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library to run cardiac EP simulations
 Author-email: Henrik Finsberg <henriknf@simula.no>
 License: MIT
 Project-URL: Homepage, https://finsberg.github.io/fenics-beat
 Project-URL: Documentation, https://finsberg.github.io/fenics-beat
 Project-URL: Source, https://github.com/finsberg/fenics-beat
 Project-URL: Tracker, https://github.com/finsberg/fenics-beat/issues
 Keywords: cardiac,electrophysiology
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: licenses/LICENSE_dolfin_pyvista_adapter
 Requires-Dist: numpy
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: gotranx; extra == "test"
+Requires-Dist: numba; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pdbpp; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: bump2version; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: pypi
 Requires-Dist: twine; extra == "pypi"
 Requires-Dist: build; extra == "pypi"
 Provides-Extra: demos
 Requires-Dist: cardiac-geometries; extra == "demos"
 Requires-Dist: ldrb; extra == "demos"
+Requires-Dist: pint; extra == "demos"
+Requires-Dist: gotranx; extra == "demos"
+Requires-Dist: numba; extra == "demos"
+Provides-Extra: pyvista
+Requires-Dist: pyvista[trame]; extra == "pyvista"
 Provides-Extra: docs
 Requires-Dist: jupyter-book; extra == "docs"
 Requires-Dist: jupytext; extra == "docs"
 Requires-Dist: fenics-beat[demos]; extra == "docs"
 Provides-Extra: all
 Requires-Dist: fenics-beat[test]; extra == "all"
 Requires-Dist: fenics-beat[docs]; extra == "all"
 Requires-Dist: fenics-beat[pypi]; extra == "all"
 Requires-Dist: fenics-beat[dev]; extra == "all"
 Requires-Dist: fenics-beat[demos]; extra == "all"
-Provides-Extra: testpaths
-Requires-Dist: tests; extra == "testpaths"
 
 # fenics-beat
 
 A simplified version of `cbcbeat` for running cardiac electrophysiology simulations.
 
 - Source code: https://github.com/finsberg/fenics-beat
 - Documentation: https://finsberv.github.io/fenics-beat
```

### Comparing `fenics_beat-0.0.4/pyproject.toml` & `fenics_beat-0.0.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system] # Require setuptool version due to https://github.com/pypa/setuptools/issues/2938
 requires = ["setuptools>=61.0.0", "wheel"]
 
 [project]
 name = "fenics-beat"
-version = "0.0.4"
+version = "0.0.5"
 description = "Library to run cardiac EP simulations"
 authors = [{name = "Henrik Finsberg", email = "henriknf@simula.no"}]
 license = {text = "MIT"}
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["cardiac", "electrophysiology"]
 dependencies = [
@@ -20,47 +20,59 @@
 Source = "https://github.com/finsberg/fenics-beat"
 Tracker = "https://github.com/finsberg/fenics-beat/issues"
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "pytest-cov",
+    "gotranx",
+    "numba"
 ]
 dev = [
     "pdbpp",
     "ipython",
     "bump2version",
     "pre-commit",
 ]
 pypi = [
     "twine",
     "build"
 ]
 demos = [
    "cardiac-geometries",
    "ldrb",
+   "pint",
+   "gotranx",
+   "numba",
 ]
+pyvista = [
+    "pyvista[trame]",
+]
+
 docs = [
    "jupyter-book",
    "jupytext",
    "fenics-beat[demos]"
 ]
 all = [
    "fenics-beat[test]",
    "fenics-beat[docs]",
    "fenics-beat[pypi]",
    "fenics-beat[dev]",
    "fenics-beat[demos]"
 ]
 
 
-testpaths = [
-    "tests"
+[tool.setuptools]
+license-files = [
+    "LICENSE",
+    "licenses/LICENSE_dolfin_pyvista_adapter",
 ]
 
+
 [tool.pytest.ini_options]
 markers = [
     "skip_in_parallel: Skip test when running in parallel",
 ]
 
 [tool.ruff]
```

### Comparing `fenics_beat-0.0.4/src/beat/__init__.py` & `fenics_beat-0.0.5/src/beat/__init__.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.4/src/beat/base_model.py` & `fenics_beat-0.0.5/src/beat/base_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -147,36 +147,20 @@
             "lu_solver": lu_solver_params,
         }
 
     @abc.abstractmethod
     def variational_forms(self, k_n: Expr | float) -> tuple[ufl.Form, ufl.Form]:
         """Create the variational forms corresponding to the given
         discretization of the given system of equations.
-
-        *Arguments*
-          k_n (:py:class:`ufl.Expr` or float)
-            The time step
-
-        *Returns*
-          (G, prec) (:py:class:`tuple` of :py:class:`ufl.Form`)
-
         """
         ...
 
     def step(self, interval):
         """
         Solve on the given time step (t0, t1).
-
-        *Arguments*
-          interval (:py:class:`tuple`)
-            The time interval (t0, t1) for the step
-
-        *Invariants*
-          Assuming that v_ is in the correct state for t0, gives
-          self.v in correct state at t1.
         """
 
         # timer = dolfin.Timer("PDE Step")
 
         # Extract interval and thus time-step
         (t0, t1) = interval
         dt = t1 - t0
```

### Comparing `fenics_beat-0.0.4/src/beat/bidomain_model.py` & `fenics_beat-0.0.5/src/beat/bidomain_model.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.4/src/beat/cellmodels/__init__.py` & `fenics_beat-0.0.5/src/beat/cellmodels/__init__.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.4/src/beat/cellmodels/beeler_reuter_1977.py` & `fenics_beat-0.0.5/src/beat/cellmodels/beeler_reuter_1977.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.4/src/beat/cellmodels/fitzhughnagumo.py` & `fenics_beat-0.0.5/src/beat/cellmodels/fitzhughnagumo.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.4/src/beat/cellmodels/tentusscher_panfilov_2006/endo.py` & `fenics_beat-0.0.5/src/beat/cellmodels/tentusscher_panfilov_2006/endo.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.4/src/beat/cellmodels/tentusscher_panfilov_2006/epi.py` & `fenics_beat-0.0.5/src/beat/cellmodels/tentusscher_panfilov_2006/epi.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.4/src/beat/cellmodels/tentusscher_panfilov_2006/mid.py` & `fenics_beat-0.0.5/src/beat/cellmodels/tentusscher_panfilov_2006/mid.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.4/src/beat/cellmodels/torord_dyn_chloride/endo.py` & `fenics_beat-0.0.5/src/beat/cellmodels/torord_dyn_chloride/endo.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.4/src/beat/cellmodels/torord_dyn_chloride/epi.py` & `fenics_beat-0.0.5/src/beat/cellmodels/torord_dyn_chloride/epi.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.4/src/beat/cellmodels/torord_dyn_chloride/mid.py` & `fenics_beat-0.0.5/src/beat/cellmodels/torord_dyn_chloride/mid.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.4/src/beat/ecg.py` & `fenics_beat-0.0.5/src/beat/ecg.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.4/src/beat/monodomain_model.py` & `fenics_beat-0.0.5/src/beat/monodomain_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,17 +28,18 @@
     def __init__(
         self,
         time: dolfin.Constant,
         mesh: dolfin.Mesh,
         M: ufl.Coefficient | float,
         I_s: Stimulus | ufl.Coefficient | None = None,
         params=None,
+        C_m: float = 1.0,
     ) -> None:
         self._M = M
-
+        self.C_m = dolfin.Constant(C_m)
         super().__init__(mesh=mesh, time=time, params=params, I_s=I_s)
 
     def _setup_state_space(self) -> None:
         # Set-up function spaces
         k = self.parameters["degree"]
         family = self.parameters["family"]
 
@@ -90,15 +91,17 @@
         Dt_v_k_n = v - self.v_
         v_mid = theta * v + (1.0 - theta) * self.v_
 
         theta_parabolic = ufl.inner(self._M * ufl.grad(v_mid), ufl.grad(w))
         # breakpoint()
         G_stim = self._I_s.expr * w * self._I_s.dz
 
-        G = (Dt_v_k_n * w + k_n * theta_parabolic) * dolfin.dx(domain=self._mesh) - k_n * G_stim
+        G = (self.C_m * Dt_v_k_n * w + k_n * theta_parabolic) * dolfin.dx(
+            domain=self._mesh
+        ) - k_n * G_stim
 
         # Define preconditioner based on educated(?) guess by Marie
         if self.parameters["use_custom_preconditioner"]:
             prec = (v * w + k_n / 2.0 * ufl.inner(self._M * ufl.grad(v), ufl.grad(w))) * dolfin.dx(
                 domain=self._mesh
             )
         else:
```

### Comparing `fenics_beat-0.0.4/src/beat/monodomain_solver.py` & `fenics_beat-0.0.5/src/beat/monodomain_solver.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.4/src/beat/odesolver.py` & `fenics_beat-0.0.5/src/beat/odesolver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 import abc
 from typing import NamedTuple, Callable, Any
 
 import numpy as np
 import numpy.typing as npt
 import dolfin
 
@@ -35,30 +35,38 @@
     while t + dt < t_bound:
         fun(states=states, t=t, parameters=parameters, dt=dt, **extra)
         V[i, :] = states[V_index, :]
         i += 1
         t += dt
 
 
-@dataclass
+@dataclass(frozen=True, slots=True)
 class ODESystemSolver:
     fun: Callable
     states: npt.NDArray
     parameters: npt.NDArray
+    missing_variables: npt.NDArray | None = None
+    _kwargs: dict[str, npt.NDArray] = field(default_factory=dict)
+
+    def __post_init__(self):
+        if self.missing_variables is not None:
+            self._kwargs["missing_variables"] = self.missing_variables
 
     @property
     def num_points(self) -> int:
         return self.states.shape[1]
 
     @property
     def num_states(self) -> int:
         return self.states.shape[0]
 
     def step(self, t0: float, dt: float) -> None:
-        self.states[:] = self.fun(states=self.states, t=t0, parameters=self.parameters, dt=dt)
+        self.states[:] = self.fun(
+            states=self.states, t=t0, parameters=self.parameters, dt=dt, **self._kwargs
+        )
 
 
 class BaseDolfinODESolver(abc.ABC):
     v_ode: dolfin.Function
     v_pde: dolfin.Function
     _metadata: dict[str, Any] | None = None
 
@@ -109,26 +117,29 @@
     v_ode: dolfin.Function
     v_pde: dolfin.Function
     init_states: npt.NDArray
     parameters: npt.NDArray
     fun: Callable
     num_states: int
     v_index: int = 0
+    missing_variables: npt.NDArray | None = None
+    num_missing_variables: int = 0
 
     def __post_init__(self):
         if np.shape(self.init_states) == self.shape:
             self._values = np.copy(self.init_states)
         else:
             self._values = np.zeros(self.shape)
             self._values.T[:] = self.init_states
 
         self._ode = ODESystemSolver(
             fun=self.fun,
             states=self._values,
             parameters=self.parameters,
+            missing_variables=self.missing_variables,
         )
         self._initialize_metadata()
 
     def to_dolfin(self) -> None:
         """Assign values from numpy array to dolfin function"""
         self.v_ode.vector()[:] = self._values[self.v_index, :]
 
@@ -145,14 +156,18 @@
         return len(self.parameters)
 
     @property
     def shape(self) -> tuple[int, int]:
         return (self.num_states, self.num_points)
 
     @property
+    def shape_missing_values(self) -> tuple[int, int]:
+        return (self.num_missing_variables, self.num_points)
+
+    @property
     def num_points(self) -> int:
         return self.v_ode.vector().local_size()
 
     def step(self, t0: float, dt: float):
         self._ode.step(t0=t0, dt=dt)
 
     @property
```

### Comparing `fenics_beat-0.0.4/src/beat/utils.py` & `fenics_beat-0.0.5/src/beat/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 from typing import Any
 import logging
 from contextlib import contextmanager
 import dolfin
-import numpy.typing as npt
 import numpy as np
 from mpi4py import MPI as pyMPI
 
 try:
     import ufl_legacy as ufl
 except ImportError:
     import ufl
@@ -34,58 +33,144 @@
     comm = mpi4py_comm(f.function_space().mesh().mpi_comm())
     yglob = np.zeros_like(yloc)
     comm.Allreduce(yloc, yglob, op=pyMPI.MIN)
     return yglob
 
 
 def expand_layer(
-    markers: dolfin.Function,
+    V: dolfin.FunctionSpace,
     mfun: dolfin.MeshFunction,
-    endo_markers: list[int],
-    epi_markers: list[int],
     endo_marker: int,
     epi_marker: int,
     endo_size: float,
     epi_size: float,
-) -> npt.NDArray:
+) -> dolfin.Function:
     """Expand the endo and epi markers to the rest of the mesh
     with a given size
 
     Parameters
     ----------
     markers : dolfin.Function
-        Function where the markers are stored
+        Function space where the markers should be stored
     mfun : dolfin.MeshFunction
         Mesh function where the markers are stored
-    endo_markers: list[int]
-        List of markers for the endocardium. Should
-        be a subset of the markers in mfun
-    epimarkers: list[int]
-        List of markers for the epicardium. Should
-        be a subset of the markers in mfun
     endo_marker : int
-        Marker for the endocardium. Used to set the
-        marker on the array that is returned.
+        Marker for the endocardium.
     epi_marker : int
-        Marker for the epicardium. Used to set the
-        marker on the array that is returned.
+        Marker for the epicardium.
     endo_size : float
         Size of the endocardium
     epi_size : float
         Size of the epicardium
 
     Returns
     -------
-    npt.NDArray
-        Array with the markers
+    dolfin.Function
+        Function with the markers with the value 1
+        on the endocardium, 2 on the epicardium
+        and 0 on the mid layer
     """
     # Find the rest of the laplace solutions
-    V = markers.function_space()
+
     u = ufl.TrialFunction(V)
     v = ufl.TestFunction(V)
+    mesh = V.mesh()
+
+    markers = dolfin.Function(V)
+    arr = markers.vector().get_local().copy()
+    sol = dolfin.Function(V)
+
+    a = ufl.dot(ufl.grad(u), ufl.grad(v)) * ufl.dx(domain=mesh)
+    L = v * dolfin.Constant(0) * ufl.dx(domain=mesh)
+
+    solver = dolfin.PETScKrylovSolver()
+    dolfin.PETScOptions.set("ksp_type", "cg")
+    dolfin.PETScOptions.set("ksp_norm_type", "unpreconditioned")
+    dolfin.PETScOptions.set("ksp_atol", 1e-15)
+    dolfin.PETScOptions.set("ksp_rtol", 1e-10)
+    dolfin.PETScOptions.set("ksp_max_it", 10_000)
+    dolfin.PETScOptions.set("ksp_error_if_not_converged", False)
+    # if ksp_monitor:
+    #     dolfin.PETScOptions.set("ksp_monitor")
+    # if ksp_view:
+    #     dolfin.PETScOptions.set("ksp_view")
+    dolfin.PETScOptions.set("pc_type", "hypre")
+    dolfin.PETScOptions.set("pc_hypre_type", "boomeramg")
+    # if pc_view:
+    #     dolfin.PETScOptions.set("pc_view")
+    solver.set_from_options()
+    sol_arrs = []
+
+    sol.vector()[:] = 0
+
+    # Iterate over the three different cases
+    logger.info("Solving Laplace equation")
+    bcs = [
+        dolfin.DirichletBC(V, 0, mfun, endo_marker, "topological"),
+        dolfin.DirichletBC(V, 1, mfun, epi_marker, "topological"),
+    ]
+    A, b = dolfin.assemble_system(a, L, bcs)
+
+    solver.set_operator(A)
+    solver.solve(sol.vector(), b)
+
+    sol_arrs.append(sol.vector().get_local())
+
+    # In BiV we have have one epi and two endo solutions
+    # We take the minimum of the two endo solutions
+    sol_arr = np.min(sol_arrs, axis=0)
+    arr[sol_arr < endo_size] = 1
+    arr[sol_arr > 1 - epi_size] = 2
+    markers.vector().set_local(arr)
+
+    return markers
+
+
+def expand_layer_biv(
+    V: dolfin.FunctionSpace,
+    mfun: dolfin.MeshFunction,
+    endo_lv_marker: int,
+    endo_rv_marker: int,
+    epi_marker: int,
+    endo_size: float,
+    epi_size: float,
+) -> dolfin.Function:
+    """Expand the endo and epi markers to the rest of the mesh
+    with a given size. Used for BiV geometries.
+
+    Parameters
+    ----------
+    markers : dolfin.FunctionSpace
+        Function space where the markers should be stored
+    mfun : dolfin.MeshFunction
+        Mesh function where the markers are stored
+    endo_lv_marker : int
+        Marker for the LV endocardium.
+    endo_lv_marker : int
+        Marker for the RV endocardium.
+    epi_marker : int
+        Marker for the epicardium.
+    endo_size : float
+        Size of the endocardium
+    epi_size : float
+        Size of the epicardium
+
+    Returns
+    -------
+    dolfin.Function
+        Function with the markers with the value 1
+        on the endocardium, 2 on the epicardium
+        and 0 on the mid layer
+
+    """
+
+    u = ufl.TrialFunction(V)
+    v = ufl.TestFunction(V)
+
+    markers = dolfin.Function(V)
     arr = markers.vector().get_local().copy()
     sol = dolfin.Function(V)
 
     a = ufl.dot(ufl.grad(u), ufl.grad(v)) * ufl.dx
     L = v * dolfin.Constant(0) * ufl.dx
 
     solver = dolfin.PETScKrylovSolver()
@@ -102,37 +187,57 @@
     dolfin.PETScOptions.set("pc_type", "hypre")
     dolfin.PETScOptions.set("pc_hypre_type", "boomeramg")
     # if pc_view:
     #     dolfin.PETScOptions.set("pc_view")
     solver.set_from_options()
     sol_arrs = []
 
-    for endo in endo_markers:
-        for epi in epi_markers:
-            sol.vector()[:] = 0
-
-            # Iterate over the three different cases
-            logger.info("Solving Laplace equation")
-            bcs = [
-                dolfin.DirichletBC(V, 0, mfun, endo, "topological"),
-                dolfin.DirichletBC(V, 1, mfun, epi, "topological"),
-            ]
-            A, b = dolfin.assemble_system(a, L, bcs)
+    mfun_original = mfun.array().copy()
 
-            solver.set_operator(A)
-            solver.solve(sol.vector(), b)
-
-            sol_arrs.append(sol.vector().get_local())
+    # Solve LV - RV + EPI
+    sol.vector()[:] = 0
+    # Iterate over the three different cases
+    logger.info("Solving Laplace equation for LV - RV + EPI")
+    mfun.array()[mfun_original == endo_rv_marker] = epi_marker
+    bcs = [
+        dolfin.DirichletBC(V, 0, mfun, endo_lv_marker, "topological"),
+        dolfin.DirichletBC(V, 1, mfun, epi_marker, "topological"),
+    ]
+    A, b = dolfin.assemble_system(a, L, bcs)
+
+    solver.set_operator(A)
+    solver.solve(sol.vector(), b)
+    sol_arrs.append(sol.vector().get_local())
+
+    # Solve RV - LV + EPI
+    sol.vector()[:] = 0
+    # Iterate over the three different cases
+    logger.info("Solving Laplace equation for RV - LV + EPI")
+    mfun.array()[:] = mfun_original
+    mfun.array()[mfun_original == endo_lv_marker] = epi_marker
+    bcs = [
+        dolfin.DirichletBC(V, 0, mfun, endo_rv_marker, "topological"),
+        dolfin.DirichletBC(V, 1, mfun, epi_marker, "topological"),
+    ]
+    A, b = dolfin.assemble_system(a, L, bcs)
+
+    solver.set_operator(A)
+    solver.solve(sol.vector(), b)
+    sol_arrs.append(sol.vector().get_local())
 
     # In BiV we have have one epi and two endo solutions
     # We take the minimum of the two endo solutions
     sol_arr = np.min(sol_arrs, axis=0)
-    arr[sol_arr < endo_size] = endo_marker
-    arr[sol_arr > 1 - epi_size] = epi_marker
-    return arr
+    arr[sol_arr < endo_size] = 1
+    arr[sol_arr > 1 - epi_size] = 2
+
+    mfun.array()[:] = mfun_original
+
+    markers.vector().set_local(arr)
+    return markers
 
 
 @contextmanager
 def form_compiler_representation(name: str):
     """Context manager to set the form compiler representation"""
     old = dolfin.parameters["form_compiler"]["representation"]
     dolfin.parameters["form_compiler"]["representation"] = name
```

### Comparing `fenics_beat-0.0.4/src/fenics_beat.egg-info/PKG-INFO` & `fenics_beat-0.0.5/src/fenics_beat.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,54 @@
 Metadata-Version: 2.1
 Name: fenics-beat
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library to run cardiac EP simulations
 Author-email: Henrik Finsberg <henriknf@simula.no>
 License: MIT
 Project-URL: Homepage, https://finsberg.github.io/fenics-beat
 Project-URL: Documentation, https://finsberg.github.io/fenics-beat
 Project-URL: Source, https://github.com/finsberg/fenics-beat
 Project-URL: Tracker, https://github.com/finsberg/fenics-beat/issues
 Keywords: cardiac,electrophysiology
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: licenses/LICENSE_dolfin_pyvista_adapter
 Requires-Dist: numpy
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: gotranx; extra == "test"
+Requires-Dist: numba; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pdbpp; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: bump2version; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: pypi
 Requires-Dist: twine; extra == "pypi"
 Requires-Dist: build; extra == "pypi"
 Provides-Extra: demos
 Requires-Dist: cardiac-geometries; extra == "demos"
 Requires-Dist: ldrb; extra == "demos"
+Requires-Dist: pint; extra == "demos"
+Requires-Dist: gotranx; extra == "demos"
+Requires-Dist: numba; extra == "demos"
+Provides-Extra: pyvista
+Requires-Dist: pyvista[trame]; extra == "pyvista"
 Provides-Extra: docs
 Requires-Dist: jupyter-book; extra == "docs"
 Requires-Dist: jupytext; extra == "docs"
 Requires-Dist: fenics-beat[demos]; extra == "docs"
 Provides-Extra: all
 Requires-Dist: fenics-beat[test]; extra == "all"
 Requires-Dist: fenics-beat[docs]; extra == "all"
 Requires-Dist: fenics-beat[pypi]; extra == "all"
 Requires-Dist: fenics-beat[dev]; extra == "all"
 Requires-Dist: fenics-beat[demos]; extra == "all"
-Provides-Extra: testpaths
-Requires-Dist: tests; extra == "testpaths"
 
 # fenics-beat
 
 A simplified version of `cbcbeat` for running cardiac electrophysiology simulations.
 
 - Source code: https://github.com/finsberg/fenics-beat
 - Documentation: https://finsberv.github.io/fenics-beat
```

### Comparing `fenics_beat-0.0.4/src/fenics_beat.egg-info/SOURCES.txt` & `fenics_beat-0.0.5/src/fenics_beat.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 LICENSE
 README.md
 pyproject.toml
+licenses/LICENSE_dolfin_pyvista_adapter
 src/beat/__init__.py
 src/beat/base_model.py
 src/beat/bidomain_model.py
 src/beat/ecg.py
 src/beat/monodomain_model.py
 src/beat/monodomain_solver.py
 src/beat/odesolver.py
+src/beat/single_cell.py
 src/beat/utils.py
+src/beat/viz.py
 src/beat/cellmodels/__init__.py
 src/beat/cellmodels/beeler_reuter_1977.py
 src/beat/cellmodels/fitzhughnagumo.py
 src/beat/cellmodels/tentusscher_panfilov_2006/__init__.py
 src/beat/cellmodels/tentusscher_panfilov_2006/endo.py
 src/beat/cellmodels/tentusscher_panfilov_2006/epi.py
 src/beat/cellmodels/tentusscher_panfilov_2006/mid.py
@@ -27,8 +30,9 @@
 src/fenics_beat.egg-info/top_level.txt
 tests/test_bidomain_model.py
 tests/test_cellmodels.py
 tests/test_ecg.py
 tests/test_monodomain.py
 tests/test_monodomain_solver.py
 tests/test_odesolver.py
+tests/test_single_cell.py
 tests/test_utils.py
```

### Comparing `fenics_beat-0.0.4/tests/test_bidomain_model.py` & `fenics_beat-0.0.5/tests/test_bidomain_model.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.4/tests/test_cellmodels.py` & `fenics_beat-0.0.5/tests/test_cellmodels.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.4/tests/test_ecg.py` & `fenics_beat-0.0.5/tests/test_ecg.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.4/tests/test_monodomain.py` & `fenics_beat-0.0.5/tests/test_monodomain.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.4/tests/test_monodomain_solver.py` & `fenics_beat-0.0.5/tests/test_monodomain_solver.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.4/tests/test_odesolver.py` & `fenics_beat-0.0.5/tests/test_odesolver.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.4/tests/test_utils.py` & `fenics_beat-0.0.5/tests/test_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -35,62 +35,66 @@
     endo_marker = 1
     epi_marker = 2
     dolfin.CompiledSubDomain("near(x[0], 0)").mark(mfun, endo_marker)
     dolfin.CompiledSubDomain("near(x[0], 1)").mark(mfun, epi_marker)
 
     V = dolfin.FunctionSpace(mesh, "Lagrange", 1)
     markers = dolfin.Function(V)
-    arr = beat.utils.expand_layer(
-        markers=markers,
+    markers = beat.utils.expand_layer(
+        V=V,
         mfun=mfun,
-        endo_markers=[endo_marker],
-        epi_markers=[epi_marker],
         endo_marker=endo_marker,
         epi_marker=epi_marker,
         endo_size=0.3,
         epi_size=0.3,
     )
 
-    markers.vector().set_local(arr)
-
     # Just check a few values
     for x in [0.0, 0.1, 0.2]:
         for y in [0.0, 0.5, 1.0]:
             assert np.isclose(peval(markers, (x, y)), endo_marker)
             assert np.isclose(peval(markers, (x + 0.4, y)), mid_marker)
             assert np.isclose(peval(markers, (1 - x, y)), epi_marker)
 
 
 def test_expand_layer_double():
-    mesh = dolfin.UnitSquareMesh(10, 10)
+    mesh = dolfin.UnitSquareMesh(40, 40)
 
     mfun = dolfin.MeshFunction("size_t", mesh, mesh.topology().dim() - 1)
     mfun.set_all(0)
-    mid_marker = 0
-    endo_marker = 1
-    endo_marker2 = 2
+    endo_lv_marker = 1
+    endo_rv_marker = 2
     epi_marker = 3
-    dolfin.CompiledSubDomain("near(x[0], 0) && x[1] <= 0.5").mark(mfun, endo_marker)
-    dolfin.CompiledSubDomain("near(x[0], 0) && x[1] >= 0.5").mark(mfun, endo_marker2)
+    dolfin.CompiledSubDomain("near(x[1], 0) && x[0] <= 0.5").mark(mfun, endo_lv_marker)
+    dolfin.CompiledSubDomain("near(x[1], 1) && x[0] <= 0.5").mark(mfun, endo_rv_marker)
     dolfin.CompiledSubDomain("near(x[0], 1)").mark(mfun, epi_marker)
 
     V = dolfin.FunctionSpace(mesh, "Lagrange", 1)
-    markers = dolfin.Function(V)
-    arr = beat.utils.expand_layer(
-        markers=markers,
+    markers = beat.utils.expand_layer_biv(
+        V=V,
         mfun=mfun,
-        endo_markers=[endo_marker, endo_marker2],
-        epi_markers=[epi_marker],
-        endo_marker=1,
+        endo_lv_marker=endo_lv_marker,
+        endo_rv_marker=endo_rv_marker,
         epi_marker=epi_marker,
         endo_size=0.3,
         epi_size=0.3,
     )
 
-    markers.vector().set_local(arr)
-
-    # Just check a few values
-    for x in [0.0, 0.1, 0.2]:
-        for y in [0.0, 0.5, 1.0]:
-            assert np.isclose(peval(markers, (x, y)), endo_marker)
-            assert np.isclose(peval(markers, (x + 0.4, y)), mid_marker)
-            assert np.isclose(peval(markers, (1 - x, y)), epi_marker)
+    # Endo in the upp left and lower left coners
+    for y_value in [0.0, 1.0, 0.2, 0.8]:
+        for x_value in [0.0, 0.1]:
+            assert np.isclose(peval(markers, (x_value, y_value)), 1.0)
+
+    # Mid should be beween the two endo
+    for y_value in [0.4, 0.6]:
+        for x_value in [0.0, 0.1]:
+            assert np.isclose(peval(markers, (x_value, y_value)), 0.0)
+
+    # and between endo and epi
+    for y_value in [0.0, 1.0]:
+        for x_value in [0.6, 0.7]:
+            assert np.isclose(peval(markers, (x_value, y_value)), 0.0)
+
+    # Epi should be to the right
+    for y_value in [0.0, 0.5, 1.0]:
+        for x_value in [0.9, 1.0]:
+            assert np.isclose(peval(markers, (x_value, y_value)), 2.0)
```

