# Comparing `tmp/compas_occ-1.0.2.tar.gz` & `tmp/compas_occ-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compas_occ-1.0.2.tar", last modified: Mon Mar 18 15:58:57 2024, max compression
+gzip compressed data, was "compas_occ-1.1.0.tar", last modified: Mon May 13 20:41:54 2024, max compression
```

## Comparing `compas_occ-1.0.2.tar` & `compas_occ-1.1.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:58:57.309311 compas_occ-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-18 15:58:44.000000 compas_occ-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-03-18 15:58:57.305310 compas_occ-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-03-18 15:58:44.000000 compas_occ-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-03-18 15:58:44.000000 compas_occ-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-18 15:58:44.000000 compas_occ-1.0.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-18 15:58:44.000000 compas_occ-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 15:58:57.309311 compas_occ-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:58:57.297310 compas_occ-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:58:57.301310 compas_occ-1.0.2/src/compas_occ/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-18 15:58:44.000000 compas_occ-1.0.2/src/compas_occ/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:58:57.301310 compas_occ-1.0.2/src/compas_occ/brep/
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-03-18 15:58:44.000000 compas_occ-1.0.2/src/compas_occ/brep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45569 2024-03-18 15:58:44.000000 compas_occ-1.0.2/src/compas_occ/brep/brep.py
--rw-r--r--   0 runner    (1001) docker     (127)    23118 2024-03-18 15:58:44.000000 compas_occ-1.0.2/src/compas_occ/brep/brepedge.py
--rw-r--r--   0 runner    (1001) docker     (127)    22123 2024-03-18 15:58:44.000000 compas_occ-1.0.2/src/compas_occ/brep/brepface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-03-18 15:58:44.000000 compas_occ-1.0.2/src/compas_occ/brep/breploop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-03-18 15:58:44.000000 compas_occ-1.0.2/src/compas_occ/brep/brepvertex.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-18 15:58:44.000000 compas_occ-1.0.2/src/compas_occ/brep/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:58:57.301310 compas_occ-1.0.2/src/compas_occ/conversions/
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-03-18 15:58:44.000000 compas_occ-1.0.2/src/compas_occ/conversions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-03-18 15:58:44.000000 compas_occ-1.0.2/src/compas_occ/conversions/arrays.py
--rw-r--r--   0 runner    (1001) docker     (127)    29210 2024-03-18 15:58:44.000000 compas_occ-1.0.2/src/compas_occ/conversions/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-03-18 15:58:44.000000 compas_occ-1.0.2/src/compas_occ/conversions/meshes.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-18 15:58:44.000000 compas_occ-1.0.2/src/compas_occ/conversions/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:58:57.305310 compas_occ-1.0.2/src/compas_occ/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-18 15:58:44.000000 compas_occ-1.0.2/src/compas_occ/geometry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:58:57.305310 compas_occ-1.0.2/src/compas_occ/geometry/curves/
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-03-18 15:58:44.000000 compas_occ-1.0.2/src/compas_occ/geometry/curves/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 15:58:44.000000 compas_occ-1.0.2/src/compas_occ/geometry/curves/bezier.py
--rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-03-18 15:58:44.000000 compas_occ-1.0.2/src/compas_occ/geometry/curves/curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     8684 2024-03-18 15:58:44.000000 compas_occ-1.0.2/src/compas_occ/geometry/curves/curve2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    16900 2024-03-18 15:58:44.000000 compas_occ-1.0.2/src/compas_occ/geometry/curves/nurbs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:58:57.305310 compas_occ-1.0.2/src/compas_occ/geometry/surfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-03-18 15:58:44.000000 compas_occ-1.0.2/src/compas_occ/geometry/surfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-03-18 15:58:44.000000 compas_occ-1.0.2/src/compas_occ/geometry/surfaces/extrusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    17898 2024-03-18 15:58:44.000000 compas_occ-1.0.2/src/compas_occ/geometry/surfaces/nurbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-03-18 15:58:44.000000 compas_occ-1.0.2/src/compas_occ/geometry/surfaces/revolution.py
--rw-r--r--   0 runner    (1001) docker     (127)    14889 2024-03-18 15:58:44.000000 compas_occ-1.0.2/src/compas_occ/geometry/surfaces/surface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-03-18 15:58:44.000000 compas_occ-1.0.2/src/compas_occ/occ.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:58:57.305310 compas_occ-1.0.2/src/compas_occ.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-03-18 15:58:57.000000 compas_occ-1.0.2/src/compas_occ.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-03-18 15:58:57.000000 compas_occ-1.0.2/src/compas_occ.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 15:58:57.000000 compas_occ-1.0.2/src/compas_occ.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 15:58:57.000000 compas_occ-1.0.2/src/compas_occ.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-18 15:58:57.000000 compas_occ-1.0.2/src/compas_occ.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-18 15:58:57.000000 compas_occ-1.0.2/src/compas_occ.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:58:57.305310 compas_occ-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-03-18 15:58:44.000000 compas_occ-1.0.2/tests/test_data_nurbscurve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-03-18 15:58:44.000000 compas_occ-1.0.2/tests/test_data_nurbssurface.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-18 15:58:44.000000 compas_occ-1.0.2/tests/test_trivial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:41:54.580863 compas_occ-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-13 20:41:42.000000 compas_occ-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-13 20:41:54.580863 compas_occ-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-13 20:41:42.000000 compas_occ-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-13 20:41:42.000000 compas_occ-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-13 20:41:42.000000 compas_occ-1.1.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 20:41:42.000000 compas_occ-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 20:41:54.580863 compas_occ-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:41:54.572863 compas_occ-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:41:54.572863 compas_occ-1.1.0/src/compas_occ/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-13 20:41:42.000000 compas_occ-1.1.0/src/compas_occ/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:41:54.576863 compas_occ-1.1.0/src/compas_occ/brep/
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-13 20:41:42.000000 compas_occ-1.1.0/src/compas_occ/brep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47543 2024-05-13 20:41:42.000000 compas_occ-1.1.0/src/compas_occ/brep/brep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23058 2024-05-13 20:41:42.000000 compas_occ-1.1.0/src/compas_occ/brep/brepedge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22079 2024-05-13 20:41:42.000000 compas_occ-1.1.0/src/compas_occ/brep/brepface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-05-13 20:41:42.000000 compas_occ-1.1.0/src/compas_occ/brep/breploop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-13 20:41:42.000000 compas_occ-1.1.0/src/compas_occ/brep/brepvertex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-13 20:41:42.000000 compas_occ-1.1.0/src/compas_occ/brep/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:41:54.576863 compas_occ-1.1.0/src/compas_occ/conversions/
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-05-13 20:41:42.000000 compas_occ-1.1.0/src/compas_occ/conversions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-05-13 20:41:42.000000 compas_occ-1.1.0/src/compas_occ/conversions/arrays.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29210 2024-05-13 20:41:42.000000 compas_occ-1.1.0/src/compas_occ/conversions/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-05-13 20:41:42.000000 compas_occ-1.1.0/src/compas_occ/conversions/meshes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-13 20:41:42.000000 compas_occ-1.1.0/src/compas_occ/conversions/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:41:54.576863 compas_occ-1.1.0/src/compas_occ/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-13 20:41:42.000000 compas_occ-1.1.0/src/compas_occ/geometry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:41:54.580863 compas_occ-1.1.0/src/compas_occ/geometry/curves/
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-13 20:41:42.000000 compas_occ-1.1.0/src/compas_occ/geometry/curves/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:41:42.000000 compas_occ-1.1.0/src/compas_occ/geometry/curves/bezier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20586 2024-05-13 20:41:42.000000 compas_occ-1.1.0/src/compas_occ/geometry/curves/curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-05-13 20:41:42.000000 compas_occ-1.1.0/src/compas_occ/geometry/curves/curve2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16878 2024-05-13 20:41:42.000000 compas_occ-1.1.0/src/compas_occ/geometry/curves/nurbs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:41:54.580863 compas_occ-1.1.0/src/compas_occ/geometry/surfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-13 20:41:42.000000 compas_occ-1.1.0/src/compas_occ/geometry/surfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-13 20:41:42.000000 compas_occ-1.1.0/src/compas_occ/geometry/surfaces/extrusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17830 2024-05-13 20:41:42.000000 compas_occ-1.1.0/src/compas_occ/geometry/surfaces/nurbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-13 20:41:42.000000 compas_occ-1.1.0/src/compas_occ/geometry/surfaces/revolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14889 2024-05-13 20:41:42.000000 compas_occ-1.1.0/src/compas_occ/geometry/surfaces/surface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-13 20:41:42.000000 compas_occ-1.1.0/src/compas_occ/occ.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:41:54.580863 compas_occ-1.1.0/src/compas_occ.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-13 20:41:54.000000 compas_occ-1.1.0/src/compas_occ.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-13 20:41:54.000000 compas_occ-1.1.0/src/compas_occ.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:41:54.000000 compas_occ-1.1.0/src/compas_occ.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:41:54.000000 compas_occ-1.1.0/src/compas_occ.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-13 20:41:54.000000 compas_occ-1.1.0/src/compas_occ.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 20:41:54.000000 compas_occ-1.1.0/src/compas_occ.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:41:54.580863 compas_occ-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-13 20:41:42.000000 compas_occ-1.1.0/tests/test_data_nurbscurve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-13 20:41:42.000000 compas_occ-1.1.0/tests/test_data_nurbssurface.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-13 20:41:42.000000 compas_occ-1.1.0/tests/test_trivial.py
```

### Comparing `compas_occ-1.0.2/LICENSE` & `compas_occ-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `compas_occ-1.0.2/PKG-INFO` & `compas_occ-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas_occ
-Version: 1.0.2
+Version: 1.1.0
 Summary: COMPAS wrapper for the Python bindings of OCC.
 Author-email: tom van mele <tom.v.mele@gmail.com>, Lotte Aldinger <aldinger@arch.ethz.ch>, Chen Kasirer <kasirer@arch.ethz.ch>
 License: MIT License
         
         Copyright (c) ETH Zurich - Block Research Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,31 +23,32 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://compas-dev.github.io/compas_occ
 Project-URL: Repository, https://github.com/compas-dev/compas_occ
-Keywords: form finding,dynamic relaxation
+Keywords: compas,nurbs,brep,occ
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: compas>=2.0.0
+Requires-Dist: compas>=2.0.1
 Provides-Extra: dev
 Requires-Dist: attrs>=17.4; extra == "dev"
 Requires-Dist: black>=22.12.0; extra == "dev"
 Requires-Dist: bump-my-version; extra == "dev"
 Requires-Dist: compas_invocations2; extra == "dev"
+Requires-Dist: compas_viewer; extra == "dev"
 Requires-Dist: invoke>=0.14; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: sphinx_compas2_theme; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 
 # COMPAS OCC
```

### Comparing `compas_occ-1.0.2/README.md` & `compas_occ-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `compas_occ-1.0.2/pyproject.toml` & `compas_occ-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 # ============================================================================
 # project info
 # ============================================================================
 
 [project]
 name = "compas_occ"
 description = "COMPAS wrapper for the Python bindings of OCC."
-keywords = ["form finding", "dynamic relaxation"]
+keywords = ["compas", "nurbs", "brep", "occ"]
 authors = [
     { name = "tom van mele", email = "tom.v.mele@gmail.com" },
     { name = "Lotte Aldinger", email = "aldinger@arch.ethz.ch" },
     { name = "Chen Kasirer", email = "kasirer@arch.ethz.ch" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">=3.9"
-dynamic = ['dependencies', 'optional-dependencies', 'version']
+dynamic = ["dependencies", "optional-dependencies", "version"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Topic :: Scientific/Engineering",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -70,15 +70,15 @@
 ]
 
 # ============================================================================
 # replace bumpversion.cfg
 # ============================================================================
 
 [tool.bumpversion]
-current_version = "1.0.2"
+current_version = "1.1.0"
 message = "Bump version to {new_version}"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "src/compas_occ/__init__.py"
 search = "{current_version}"
@@ -90,18 +90,18 @@
 replace = "[{new_version}] {now:%Y-%m-%d}"
 
 # ============================================================================
 # replace setup.cfg
 # ============================================================================
 
 [tool.black]
-line-length = 119
+line-length = 179
 
 [tool.ruff]
-line-length = 119
+line-length = 179
 indent-width = 4
 target-version = "py39"
 
 [tool.ruff.lint]
 select = ["E", "F", "I"]
 
 [tool.ruff.lint.per-file-ignores]
```

### Comparing `compas_occ-1.0.2/src/compas_occ/brep/__init__.py` & `compas_occ-1.1.0/src/compas_occ/brep/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,19 @@
 
 @plugin(category="factories", requires=["compas_occ"])
 def from_native(*args, **kwargs):
     return OCCBrep.from_native(*args, **kwargs)
 
 
 @plugin(category="factories", requires=["compas_occ"])
+def from_plane(*args, **kwargs):
+    return OCCBrep.from_plane(*args, **kwargs)
+
+
+@plugin(category="factories", requires=["compas_occ"])
 def from_planes(*args, **kwargs):
     return OCCBrep.from_planes(*args, **kwargs)
 
 
 @plugin(category="factories", requires=["compas_occ"])
 def from_polygons(*args, **kwargs):
     return OCCBrep.from_polygons(*args, **kwargs)
```

### Comparing `compas_occ-1.0.2/src/compas_occ/brep/brep.py` & `compas_occ-1.1.0/src/compas_occ/brep/brep.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from OCC.Core import BRepMesh
 from OCC.Core import BRepPrimAPI
 from OCC.Core import GProp
 from OCC.Core import IFSelect
 from OCC.Core import IGESControl
 from OCC.Core import Interface
 from OCC.Core import ShapeFix
+from OCC.Core import ShapeUpgrade
 from OCC.Core import STEPControl
 from OCC.Core import StlAPI
 from OCC.Core import TopAbs
 from OCC.Core import TopExp
 from OCC.Core import TopLoc
 from OCC.Core import TopoDS
 from OCC.Core import TopTools
@@ -691,14 +692,37 @@
             builder.Add(shell, face.occ_face)
         brep = cls.from_native(shell)
         brep.sew()
         brep.fix()
         return brep
 
     @classmethod
+    def from_plane(
+        cls,
+        plane: Plane,
+        domain_u: Tuple[float, float] = (-1.0, +1.0),
+        domain_v: Tuple[float, float] = (-1.0, +1.0),
+    ) -> "OCCBrep":
+        """
+        Make a BRep from a plane.
+
+        Parameters
+        ----------
+        plane : :class:`compas.geometry.Plane`
+        domain_u : tuple[float, float], optional
+        domain_v : tuple[float, float], optional
+
+        Returns
+        -------
+        :class:`OCCBrep`
+
+        """
+        return cls.from_brepfaces([OCCBrepFace.from_plane(plane, domain_u=domain_u, domain_v=domain_v)])
+
+    @classmethod
     def from_planes(cls, planes: List[Plane]) -> "OCCBrep":
         """
         Make a BRep from a list of planes.
 
         Parameters
         ----------
         planes : list[:class:`compas.geometry.Plane`]
@@ -823,28 +847,36 @@
         return cls.from_brepfaces([face])
 
     # ==============================================================================
     # Boolean Constructors
     # ==============================================================================
 
     @classmethod
-    def from_boolean_difference(cls, A: "OCCBrep", B: "OCCBrep") -> "OCCBrep":
+    def from_boolean_difference(cls, A: "OCCBrep", B: Union["OCCBrep", list["OCCBrep"]]) -> "OCCBrep":
         """
         Construct a BRep from the boolean difference of two other BReps.
 
         Parameters
         ----------
         A : :class:`~compas_occ.brep.OCCBrep`
-        B : :class:`~compas_occ.brep.OCCBrep`
+        B : :class:`~compas_occ.brep.OCCBrep` | list[:class:`~compas_occ.brep.OCCBrep`]
 
         Returns
         -------
         :class:`~compas_occ.brep.OCCBrep`
 
         """
+        if isinstance(B, list):
+            compound = TopoDS.TopoDS_Compound()
+            builder = BRep.BRep_Builder()
+            builder.MakeCompound(compound)
+            for brep in B:
+                builder.Add(compound, brep.native_brep)
+            B = Brep.from_native(compound)
+
         cut = BRepAlgoAPI.BRepAlgoAPI_Cut(A.native_brep, B.native_brep)
         if not cut.IsDone():
             raise Exception("Boolean difference operation could not be completed.")
         brep = cls.from_native(cut.Shape())
         brep.sew()
         brep.fix()
         brep.make_solid()
@@ -898,29 +930,31 @@
         brep.make_solid()
         return brep
 
     # ==============================================================================
     # Converters
     # ==============================================================================
 
-    def to_tesselation(self, linear_deflection: float = 1) -> Tuple[Mesh, List[Polyline]]:
+    def to_tesselation(self, linear_deflection: float = 1, angular_deflection: float = 0.1) -> Tuple[Mesh, List[Polyline]]:
         """
         Create a tesselation of the shape for visualisation.
 
         Parameters
         ----------
         linear_deflection : float, optional
-            Allowable deviation between curved geometry and mesh discretisation.
+            Allowable "distance" deviation between curved geometry and mesh discretisation.
+        angular_deflection : float, optional
+            Allowable "curvature" deviation between curved geometry and mesh discretisation.
 
         Returns
         -------
         tuple[:class:`~compas.datastructures.Mesh`, list[:class:`~compas.geometry.Polyline`]]
 
         """
-        BRepMesh.BRepMesh_IncrementalMesh(self.occ_shape, linear_deflection)
+        BRepMesh.BRepMesh_IncrementalMesh(self.occ_shape, linear_deflection, False, angular_deflection, True)
         bt = BRep.BRep_Tool()
         mesh = Mesh()
         polylines = []
         seen = []
         for face in self.faces:
             location = TopLoc.TopLoc_Location()
             triangulation = bt.Triangulation(face.occ_face, location)
@@ -1025,15 +1059,15 @@
 
         Returns
         -------
         List[:class:`OCCBrepVertex`]
 
         """
         map = TopTools.TopTools_IndexedDataMapOfShapeListOfShape()
-        TopExp.topexp_MapShapesAndUniqueAncestors(self.occ_shape, TopAbs.TopAbs_VERTEX, TopAbs.TopAbs_EDGE, map)
+        TopExp.topexp.MapShapesAndUniqueAncestors(self.occ_shape, TopAbs.TopAbs_VERTEX, TopAbs.TopAbs_EDGE, map)
         results = map.FindFromKey(vertex.occ_vertex)
         iterator = TopTools.TopTools_ListIteratorOfListOfShape(results)  # type: ignore
         vertices = []
         while iterator.More():
             edge = TopoDS.topods.Edge(iterator.Value())
             edge = OCCBrepEdge(edge)
             iterator.Next()
@@ -1053,15 +1087,15 @@
 
         Returns
         -------
         List[:class:`OCCBrepEdge`]
 
         """
         map = TopTools.TopTools_IndexedDataMapOfShapeListOfShape()
-        TopExp.topexp_MapShapesAndUniqueAncestors(self.occ_shape, TopAbs.TopAbs_VERTEX, TopAbs.TopAbs_EDGE, map)
+        TopExp.topexp.MapShapesAndUniqueAncestors(self.occ_shape, TopAbs.TopAbs_VERTEX, TopAbs.TopAbs_EDGE, map)
         results = map.FindFromKey(vertex.occ_vertex)
         iterator = TopTools.TopTools_ListIteratorOfListOfShape(results)  # type: ignore
         edges = []
         while iterator.More():
             edge = iterator.Value()
             edges.append(OCCBrepEdge(edge))
             iterator.Next()
@@ -1077,15 +1111,15 @@
 
         Returns
         -------
         List[:class:`OCCBrepFace`]
 
         """
         map = TopTools.TopTools_IndexedDataMapOfShapeListOfShape()
-        TopExp.topexp_MapShapesAndUniqueAncestors(self.occ_shape, TopAbs.TopAbs_VERTEX, TopAbs.TopAbs_FACE, map)
+        TopExp.topexp.MapShapesAndUniqueAncestors(self.occ_shape, TopAbs.TopAbs_VERTEX, TopAbs.TopAbs_FACE, map)
         results = map.FindFromKey(vertex.occ_vertex)
         iterator = TopTools.TopTools_ListIteratorOfListOfShape(results)  # type: ignore
         faces = []
         while iterator.More():
             face = iterator.Value()
             faces.append(OCCBrepFace(face))
             iterator.Next()
@@ -1101,15 +1135,15 @@
 
         Returns
         -------
         List[:class:`OCCBrepFace`]
 
         """
         map = TopTools.TopTools_IndexedDataMapOfShapeListOfShape()
-        TopExp.topexp_MapShapesAndUniqueAncestors(self.occ_shape, TopAbs.TopAbs_EDGE, TopAbs.TopAbs_FACE, map)
+        TopExp.topexp.MapShapesAndUniqueAncestors(self.occ_shape, TopAbs.TopAbs_EDGE, TopAbs.TopAbs_FACE, map)
         results = map.FindFromKey(edge.occ_edge)
         iterator = TopTools.TopTools_ListIteratorOfListOfShape(results)  # type: ignore
         faces = []
         while iterator.More():
             face = iterator.Value()
             faces.append(OCCBrepFace(face))
             iterator.Next()
@@ -1127,15 +1161,15 @@
         -------
         List[:class:`OCCBrepLoop`]
             The loops.
 
         """
 
         map = TopTools.TopTools_IndexedDataMapOfShapeListOfShape()
-        TopExp.topexp_MapShapesAndUniqueAncestors(self.occ_shape, TopAbs.TopAbs_EDGE, TopAbs.TopAbs_WIRE, map)
+        TopExp.topexp.MapShapesAndUniqueAncestors(self.occ_shape, TopAbs.TopAbs_EDGE, TopAbs.TopAbs_WIRE, map)
         results = map.FindFromKey(edge.occ_edge)
         iterator = TopTools.TopTools_ListIteratorOfListOfShape(results)  # type: ignore
         loops = []
         while iterator.More():
             wire = iterator.Value()
             loops.append(OCCBrepLoop(wire))
             iterator.Next()
@@ -1223,14 +1257,37 @@
         -------
         None
 
         """
         self.sew()
         self.fix()
 
+    def simplify(self, merge_edges=True, merge_faces=True):
+        """Simplify the shape by merging colinear edges and coplanar faces.
+
+        Parameters
+        ----------
+        merge_edges : bool, optional
+            Merge edges with the same underlying geometry.
+        merge_faces : bool, optional
+            Merge faces with the same underlying geometry.
+
+        Returns
+        -------
+        None
+
+        """
+        if not merge_edges and not merge_faces:
+            return
+        simplifier = ShapeUpgrade.ShapeUpgrade_UnifySameDomain()
+        simplifier.Initialize(self.native_brep, merge_edges, merge_faces)
+        simplifier.Build()
+        shape = simplifier.Shape()
+        self.native_brep = shape
+
     def cull_unused_vertices(self) -> None:
         """
         Remove all unused vertices.
 
         Returns
         -------
         None
@@ -1361,22 +1418,22 @@
         proximity.Perform()
 
         overlaps1 = proximity.OverlapSubShapes1()
         keys1 = overlaps1.Keys()
         faces1 = []
         for key in keys1:
             face = proximity.GetSubShape1(key)
-            faces1.append(OCCBrepFace(face))
+            faces1.append(OCCBrepFace(face))  # type: ignore
 
         overlaps2 = proximity.OverlapSubShapes2()
         keys2 = overlaps2.Keys()
         faces2 = []
         for key in keys2:
             face = proximity.GetSubShape2(key)
-            faces2.append(OCCBrepFace(face))
+            faces2.append(OCCBrepFace(face))  # type: ignore
 
         return faces1, faces2
 
     def slice(self, plane: compas.geometry.Plane) -> Union["OCCBrep", None]:
         """Slice a BRep with a plane.
 
         Parameters
```

### Comparing `compas_occ-1.0.2/src/compas_occ/brep/brepedge.py` & `compas_occ-1.1.0/src/compas_occ/brep/brepedge.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from compas_occ.conversions import ellipse_to_compas
 from compas_occ.conversions import hyperbola_to_compas
 from compas_occ.conversions import line_to_occ
 from compas_occ.conversions import parabola_to_compas
 from compas_occ.conversions import point_to_occ
 from compas_occ.geometry import OCCCurve
 from compas_occ.geometry import OCCCurve2d
+from compas_occ.geometry import OCCNurbsCurve
 from compas_occ.geometry import OCCSurface
 
 
 class CurveType:
     LINE = 0
     CIRCLE = 1
     ELLIPSE = 2
@@ -196,21 +197,21 @@
     # @property
     # def curve(self) -> OCCCurve:
     #     if not self._curve:
     #         occ_curve = self.occ_adaptor.Curve()
     #         self._curve = OCCCurve(occ_curve)  # type: ignore
     #     return self._curve
 
-    # # remove this if possible
-    # @property
-    # def nurbscurve(self) -> OCCNurbsCurve:
-    #     if not self._nurbscurve:
-    #         occ_curve = self.occ_adaptor.BSpline()
-    #         self._nurbscurve = OCCNurbsCurve(occ_curve)  # type: ignore
-    #     return self._nurbscurve  # type: ignore (don't understand why this is necessary)
+    # remove this if possible
+    @property
+    def nurbscurve(self) -> OCCNurbsCurve:
+        if not self._nurbscurve:
+            occ_curve = self.occ_adaptor.BSpline()
+            self._nurbscurve = OCCNurbsCurve(occ_curve)  # type: ignore
+        return self._nurbscurve  # type: ignore (don't understand why this is necessary)
 
     @property
     def curve(self):
         if self.is_line:
             return self.to_line()
         if self.is_circle:
             return self.to_circle()
@@ -269,38 +270,38 @@
 
     @property
     def is_other(self) -> bool:
         return self.type == CurveType.OTHER
 
     @property
     def is_valid(self) -> bool:
-        return BRepAlgo.brepalgo_IsValid(self.occ_edge)
+        return BRepAlgo.brepalgo.IsValid(self.occ_edge)
 
     @property
     def vertices(self) -> List[OCCBrepVertex]:
         vertices = []
         explorer = TopExp.TopExp_Explorer(self.occ_edge, TopAbs.TopAbs_VERTEX)
         while explorer.More():
             vertex = explorer.Current()
             vertices.append(OCCBrepVertex(vertex))  # type: ignore
             explorer.Next()
         return vertices
 
     @property
     def first_vertex(self) -> OCCBrepVertex:
-        return OCCBrepVertex(TopExp.topexp_FirstVertex(self.occ_edge))
+        return OCCBrepVertex(TopExp.topexp.FirstVertex(self.occ_edge))
 
     @property
     def last_vertex(self) -> OCCBrepVertex:
-        return OCCBrepVertex(TopExp.topexp_LastVertex(self.occ_edge))
+        return OCCBrepVertex(TopExp.topexp.LastVertex(self.occ_edge))
 
     @property
     def length(self) -> float:
         props = GProp.GProp_GProps()
-        BRepGProp.brepgprop_LinearProperties(self.occ_edge, props)
+        BRepGProp.brepgprop.LinearProperties(self.occ_edge, props)
         return props.Mass()
 
     @property
     def domain(self) -> Tuple[float, float]:
         return self.occ_adaptor.FirstParameter(), self.occ_adaptor.LastParameter()
 
     # ==============================================================================
@@ -500,26 +501,22 @@
             if not curve2d:
                 raise ValueError("No curve was provided.")
 
             if points:
                 p1 = point_to_occ(points[0])
                 p2 = point_to_occ(points[1])
                 if params:
-                    builder = BRepBuilderAPI.BRepBuilderAPI_MakeEdge(
-                        curve2d.occ_curve, surface.occ_surface, p1, p2, *params
-                    )
+                    builder = BRepBuilderAPI.BRepBuilderAPI_MakeEdge(curve2d.occ_curve, surface.occ_surface, p1, p2, *params)
                 else:
                     builder = BRepBuilderAPI.BRepBuilderAPI_MakeEdge(curve2d.occ_curve, surface.occ_surface, p1, p2)
             elif vertices:
                 v1 = vertices[0].occ_vertex
                 v2 = vertices[1].occ_vertex
                 if params:
-                    builder = BRepBuilderAPI.BRepBuilderAPI_MakeEdge(
-                        curve2d.occ_curve, surface.occ_surface, v1, v2, *params
-                    )
+                    builder = BRepBuilderAPI.BRepBuilderAPI_MakeEdge(curve2d.occ_curve, surface.occ_surface, v1, v2, *params)
                 else:
                     builder = BRepBuilderAPI.BRepBuilderAPI_MakeEdge(curve2d.occ_curve, surface.occ_surface, v1, v2)
             else:
                 if params:
                     builder = BRepBuilderAPI.BRepBuilderAPI_MakeEdge(curve2d.occ_curve, surface.occ_surface, *params)
                 else:
                     builder = BRepBuilderAPI.BRepBuilderAPI_MakeEdge(curve2d.occ_curve, surface.occ_surface)
```

### Comparing `compas_occ-1.0.2/src/compas_occ/brep/brepface.py` & `compas_occ-1.1.0/src/compas_occ/brep/brepface.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,21 +180,21 @@
     # @property
     # def surface(self) -> OCCSurface:
     #     if not self._surface:
     #         occ_surface = self.occ_adaptor.Surface().Surface()  # this is weird
     #         self._surface = OCCSurface(occ_surface)
     #     return self._surface
 
-    # # remove this if possible
-    # @property
-    # def nurbssurface(self) -> OCCNurbsSurface:
-    #     if not self._nurbssurface:
-    #         occ_surface = self.occ_adaptor.BSpline()
-    #         self._nurbssurface = OCCNurbsSurface(occ_surface)
-    #     return self._nurbssurface
+    # remove this if possible
+    @property
+    def nurbssurface(self) -> OCCNurbsSurface:
+        if not self._nurbssurface:
+            occ_surface = self.occ_adaptor.BSpline()
+            self._nurbssurface = OCCNurbsSurface(occ_surface)
+        return self._nurbssurface
 
     @property
     def surface(self):
         if self.is_plane:
             return self.to_plane()
         if self.is_cylinder:
             return self.to_cylinder()
@@ -274,15 +274,15 @@
             wire = explorer.Current()
             loops.append(OCCBrepLoop(wire))  # type: ignore
             explorer.Next()
         return loops
 
     @property
     def outerloop(self) -> OCCBrepLoop:
-        wire = BRepTools.breptools_OuterWire(self.occ_face)
+        wire = BRepTools.breptools.OuterWire(self.occ_face)
         return OCCBrepLoop(wire)
 
     @property
     def innerloops(self) -> List[OCCBrepLoop]:
         outerloop = self.outerloop
         inner = []
         for loop in self.loops:
@@ -537,17 +537,15 @@
         -------
         :class:`OCCBrepFace`
 
         """
         if domain_u and domain_v:
             min_u, max_u = domain_u
             min_v, max_v = domain_v
-            builder = BRepBuilderAPI.BRepBuilderAPI_MakeFace(
-                surface.occ_surface, min_u, max_u, min_v, max_v, precision
-            )
+            builder = BRepBuilderAPI.BRepBuilderAPI_MakeFace(surface.occ_surface, min_u, max_u, min_v, max_v, precision)
         elif loop:
             builder = BRepBuilderAPI.BRepBuilderAPI_MakeFace(surface.occ_surface, loop.occ_wire, inside)
         else:
             builder = BRepBuilderAPI.BRepBuilderAPI_MakeFace(surface.occ_surface, precision)
         face = cls(builder.Face())
         face.precision = precision
         return face
@@ -693,15 +691,15 @@
         Verify that the face is valid.
 
         Returns
         -------
         bool
 
         """
-        return BRepAlgo.brepalgo_IsValid(self.occ_face)
+        return BRepAlgo.brepalgo.IsValid(self.occ_face)
 
     def fix(self) -> None:
         """
         Try to fix the face.
 
         Returns
         -------
```

### Comparing `compas_occ-1.0.2/src/compas_occ/brep/breploop.py` & `compas_occ-1.1.0/src/compas_occ/brep/breploop.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
 from compas.geometry import BrepLoop
 from compas.geometry import Polygon
 from compas.geometry import Polyline
-from compas.utilities import pairwise
+from compas.itertools import pairwise
 from OCC.Core import BRepAlgo
 from OCC.Core import BRepBuilderAPI
 from OCC.Core import BRepTools
 from OCC.Core import ShapeFix
 from OCC.Core import TopoDS
 
 from compas_occ.brep import OCCBrepEdge
```

### Comparing `compas_occ-1.0.2/src/compas_occ/brep/brepvertex.py` & `compas_occ-1.1.0/src/compas_occ/brep/brepvertex.py`

 * *Files identical despite different names*

### Comparing `compas_occ-1.0.2/src/compas_occ/conversions/__init__.py` & `compas_occ-1.1.0/src/compas_occ/conversions/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_occ-1.0.2/src/compas_occ/conversions/arrays.py` & `compas_occ-1.1.0/src/compas_occ/conversions/arrays.py`

 * *Files identical despite different names*

### Comparing `compas_occ-1.0.2/src/compas_occ/conversions/geometry.py` & `compas_occ-1.1.0/src/compas_occ/conversions/geometry.py`

 * *Files identical despite different names*

### Comparing `compas_occ-1.0.2/src/compas_occ/conversions/meshes.py` & `compas_occ-1.1.0/src/compas_occ/conversions/meshes.py`

 * *Files identical despite different names*

### Comparing `compas_occ-1.0.2/src/compas_occ/conversions/transformations.py` & `compas_occ-1.1.0/src/compas_occ/conversions/transformations.py`

 * *Files identical despite different names*

### Comparing `compas_occ-1.0.2/src/compas_occ/geometry/curves/curve.py` & `compas_occ-1.1.0/src/compas_occ/geometry/curves/curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,31 +6,32 @@
 from compas.geometry import Curve
 from compas.geometry import Frame
 from compas.geometry import Point
 from compas.geometry import Polyline
 from compas.geometry import Transformation
 from compas.geometry import Vector
 from compas.geometry import distance_point_point
+from OCC.Core import IFSelect
+from OCC.Core import Interface
+from OCC.Core import STEPControl
 from OCC.Core.Bnd import Bnd_Box
-from OCC.Core.BndLib import BndLib_Add3dCurve_Add
+from OCC.Core.BndLib import BndLib_Add3dCurve
 from OCC.Core.BRepBuilderAPI import BRepBuilderAPI_MakeEdge
 from OCC.Core.GCPnts import GCPnts_AbscissaPoint
-from OCC.Core.GCPnts import GCPnts_AbscissaPoint_Length
 from OCC.Core.Geom import Geom_Curve
 from OCC.Core.Geom import Geom_OffsetCurve
 from OCC.Core.GeomAdaptor import GeomAdaptor_Curve
 from OCC.Core.GeomAPI import GeomAPI_ExtremaCurveCurve
 from OCC.Core.GeomAPI import GeomAPI_ProjectPointOnCurve
-from OCC.Core.GeomProjLib import geomprojlib_Curve2d
-from OCC.Core.GeomProjLib import geomprojlib_Project
+from OCC.Core.GeomProjLib import geomprojlib
 from OCC.Core.gp import gp_Pnt
 from OCC.Core.gp import gp_Vec
 from OCC.Core.TopoDS import TopoDS_Edge
 from OCC.Core.TopoDS import TopoDS_Shape
-from OCC.Core.TopoDS import topods_Edge
+from OCC.Core.TopoDS import topods
 
 from compas_occ.conversions import compas_transformation_to_trsf
 from compas_occ.conversions import direction_to_occ
 from compas_occ.conversions import point_to_compas
 from compas_occ.conversions import point_to_occ
 from compas_occ.conversions import vector_to_compas
 
@@ -58,19 +59,18 @@
     is_periodic : bool, read-only
         Flag indicating that the curve is periodic.
     start : :class:`~compas.geometry.Point`, read-only
         The start point of the curve.
 
     """
 
-    _occ_curve: Geom_Curve
-
     def __init__(self, occ_curve: Geom_Curve, name=None):
         super().__init__(name=name)
         self._dimension = 3
+        self._occ_curve: Geom_Curve = None  # type: ignore
         self.occ_curve = occ_curve
 
     def __eq__(self, other: "OCCCurve") -> bool:
         raise NotImplementedError
 
     # ==============================================================================
     # Data
@@ -90,15 +90,15 @@
 
     @property
     def occ_shape(self) -> TopoDS_Shape:
         return BRepBuilderAPI_MakeEdge(self.occ_curve).Shape()
 
     @property
     def occ_edge(self) -> TopoDS_Edge:
-        return topods_Edge(self.occ_shape)
+        return topods.Edge(self.occ_shape)
 
     # ==============================================================================
     # Properties
     # ==============================================================================
 
     @property
     def dimension(self) -> int:
@@ -157,24 +157,19 @@
         schema : str, optional
 
         Returns
         -------
         None
 
         """
-        from OCC.Core.IFSelect import IFSelect_RetDone
-        from OCC.Core.Interface import Interface_Static_SetCVal
-        from OCC.Core.STEPControl import STEPControl_AsIs
-        from OCC.Core.STEPControl import STEPControl_Writer
-
-        step_writer = STEPControl_Writer()
-        Interface_Static_SetCVal("write.step.schema", schema)
-        step_writer.Transfer(self.occ_edge, STEPControl_AsIs)
+        step_writer = STEPControl.STEPControl_Writer()
+        Interface.Interface_Static.SetCVal("write.step.schema", schema)
+        step_writer.Transfer(self.occ_edge, STEPControl.STEPControl_AsIs)
         status = step_writer.Write(filepath)
-        if status != IFSelect_RetDone:
+        if status != IFSelect.IFSelect_RetDone:
             raise AssertionError("Operation failed.")
 
     def to_polyline(self, n: int = 100) -> Polyline:
         """Convert the curve to a polyline.
 
         Parameters
         ----------
@@ -244,17 +239,15 @@
         ------
         ValueError
             If the parameter is not in the curve domain.
 
         """
         start, end = self.domain  # type: ignore (domain could be None if no occ_curve is set)
         if t < start or t > end:
-            raise ValueError(
-                "The parameter is not in the domain of the curve. t = {}, domain: {}".format(t, self.domain)
-            )
+            raise ValueError("The parameter is not in the domain of the curve. t = {}, domain: {}".format(t, self.domain))
 
         point = self.occ_curve.Value(t)
         return point_to_compas(point)
 
     def tangent_at(self, t: float) -> Vector:
         """Compute the tangent vector at a curve parameter.
 
@@ -382,15 +375,15 @@
 
         Returns
         -------
         :class:`~compas.geometry.Box`
 
         """
         box = Bnd_Box()
-        BndLib_Add3dCurve_Add(GeomAdaptor_Curve(self.occ_curve), precision, box)
+        BndLib_Add3dCurve.Add(GeomAdaptor_Curve(self.occ_curve), precision, box)
         return Box.from_diagonal(
             (
                 point_to_compas(box.CornerMin()),
                 point_to_compas(box.CornerMax()),
             )
         )
 
@@ -402,15 +395,15 @@
         precision : float, optional
 
         Returns
         -------
         float
 
         """
-        return GCPnts_AbscissaPoint_Length(GeomAdaptor_Curve(self.occ_curve), precision)
+        return GCPnts_AbscissaPoint.Length(GeomAdaptor_Curve(self.occ_curve), precision)
 
     def closest_point(
         self,
         point: Point,
         return_parameter: bool = False,
     ) -> Union[Point, Tuple[Point, float], None]:
         """
@@ -614,15 +607,15 @@
             The projection surface.
 
         Returns
         -------
         :class:`OCCCurve`
 
         """
-        result = geomprojlib_Project(self.occ_curve, surface.occ_surface)
+        result = geomprojlib.Project(self.occ_curve, surface.occ_surface)
         curve = OCCCurve.from_occ(result)
         return curve
 
     def embedded(self, surface) -> OCCCurve2d:
         """Return a new curve embedded in the parameter space of the surface.
 
         Parameters
@@ -631,15 +624,15 @@
             The embedding surface.
 
         Returns
         -------
         :class:`OCCCurve2d`
 
         """
-        result = geomprojlib_Curve2d(self.occ_curve, surface.occ_surface)
+        result = geomprojlib.Curve2d(self.occ_curve, surface.occ_surface)
         curve = OCCCurve2d.from_occ(result)
         return curve
 
     def offset(self, distance: float, direction: Vector) -> "OCCCurve":
         """Return a new curve that is the offset of this curve over the specified distance in the given direction.
 
         Parameters
```

### Comparing `compas_occ-1.0.2/src/compas_occ/geometry/curves/curve2d.py` & `compas_occ-1.1.0/src/compas_occ/geometry/curves/curve2d.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import Tuple
 
 from compas.geometry import Curve
 from compas.geometry import Frame
 from compas.geometry import Point
 from compas.geometry import Polyline
 from compas.geometry import Vector
-from OCC.Core.BRepBuilderAPI import BRepBuilderAPI_MakeEdge2d
-from OCC.Core.Geom2d import Geom2d_Curve
-from OCC.Core.gp import gp_Pnt2d
-from OCC.Core.gp import gp_Vec2d
-from OCC.Core.TopoDS import TopoDS_Edge
-from OCC.Core.TopoDS import TopoDS_Shape
-from OCC.Core.TopoDS import topods_Edge
+from OCC.Core import BRepBuilderAPI
+from OCC.Core import Geom2d
+from OCC.Core import IFSelect
+from OCC.Core import Interface
+from OCC.Core import STEPControl
+from OCC.Core import TopoDS
+from OCC.Core import gp
 
 from compas_occ.conversions import point2d_to_compas
 from compas_occ.conversions import vector2d_to_compas
 
 
 class OCCCurve2d(Curve):
     """Class representing a general 2D curve object ussually generated through an embedding in a surface.
@@ -38,47 +38,46 @@
     is_periodic : bool, read-only
         Flag indicating that the curve is periodic.
     start : :class:`~compas.geometry.Point`, read-only
         The start point of the curve.
 
     """
 
-    _occ_curve: Geom2d_Curve
-
-    def __init__(self, occ_curve: Geom2d_Curve, name=None):
+    def __init__(self, occ_curve: Geom2d.Geom2d_Curve, name=None):
         super().__init__(name=name)
         self._dimension = 2
+        self._occ_curve: Geom2d.Geom2d_Curve = None  # type: ignore
         self.occ_curve = occ_curve
 
     def __eq__(self, other: "OCCCurve2d") -> bool:
         raise NotImplementedError
 
     # ==============================================================================
     # Data
     # ==============================================================================
 
     # ==============================================================================
     # OCC Properties
     # ==============================================================================
 
     @property
-    def occ_curve(self) -> Geom2d_Curve:
+    def occ_curve(self) -> Geom2d.Geom2d_Curve:
         return self._occ_curve
 
     @occ_curve.setter
-    def occ_curve(self, curve: Geom2d_Curve):
+    def occ_curve(self, curve: Geom2d.Geom2d_Curve):
         self._occ_curve = curve
 
     @property
-    def occ_shape(self) -> TopoDS_Shape:
-        return BRepBuilderAPI_MakeEdge2d(self.occ_curve).Shape()
+    def occ_shape(self) -> TopoDS.TopoDS_Shape:
+        return BRepBuilderAPI.BRepBuilderAPI_MakeEdge2d(self.occ_curve).Shape()
 
     @property
-    def occ_edge(self) -> TopoDS_Edge:
-        return topods_Edge(self.occ_shape)
+    def occ_edge(self) -> TopoDS.TopoDS_Edge:
+        return TopoDS.topods.Edge(self.occ_shape)
 
     # ==============================================================================
     # Properties
     # ==============================================================================
 
     @property
     def dimension(self) -> int:
@@ -105,15 +104,15 @@
         return self.occ_curve.IsPeriodic()
 
     # ==============================================================================
     # Constructors
     # ==============================================================================
 
     @classmethod
-    def from_occ(cls, occ_curve: Geom2d_Curve) -> "OCCCurve2d":
+    def from_occ(cls, occ_curve: Geom2d.Geom2d_Curve) -> "OCCCurve2d":
         """Construct a NURBS curve from an existing OCC BSplineCurve.
 
         Parameters
         ----------
         occ_curve : Geom2d_Curve
 
         Returns
@@ -136,24 +135,19 @@
         schema : str, optional
 
         Returns
         -------
         None
 
         """
-        from OCC.Core.IFSelect import IFSelect_RetDone
-        from OCC.Core.Interface import Interface_Static_SetCVal
-        from OCC.Core.STEPControl import STEPControl_AsIs
-        from OCC.Core.STEPControl import STEPControl_Writer
-
-        step_writer = STEPControl_Writer()
-        Interface_Static_SetCVal("write.step.schema", schema)
-        step_writer.Transfer(self.occ_edge, STEPControl_AsIs)
+        step_writer = STEPControl.STEPControl_Writer()
+        Interface.Interface_Static.SetCVal("write.step.schema", schema)
+        step_writer.Transfer(self.occ_edge, STEPControl.STEPControl_AsIs)
         status = step_writer.Write(filepath)
-        if status != IFSelect_RetDone:
+        if status != IFSelect.IFSelect_RetDone:
             raise AssertionError("Operation failed.")
 
     def to_polyline(self, n: int = 100) -> Polyline:
         """Convert the curve to a polyline.
 
         Parameters
         ----------
@@ -199,17 +193,15 @@
         ------
         ValueError
             If the parameter is not in the curve domain.
 
         """
         start, end = self.domain  # type: ignore (domain could be None if no occ_curve is set)
         if t < start or t > end:
-            raise ValueError(
-                "The parameter is not in the domain of the curve. t = {}, domain: {}".format(t, self.domain)
-            )
+            raise ValueError("The parameter is not in the domain of the curve. t = {}, domain: {}".format(t, self.domain))
 
         point = self.occ_curve.Value(t)
         return point2d_to_compas(point)
 
     def tangent_at(self, t: float) -> Vector:
         """Compute the tangent vector at a curve parameter.
 
@@ -228,16 +220,16 @@
             If the parameter is not in the curve domain.
 
         """
         start, end = self.domain  # type: ignore (domain could be None if no occ_curve is set)
         if t < start or t > end:
             raise ValueError("The parameter is not in the domain of the curve.")
 
-        point = gp_Pnt2d()
-        uvec = gp_Vec2d()
+        point = gp.gp_Pnt2d()
+        uvec = gp.gp_Vec2d()
         self.occ_curve.D1(t, point, uvec)
         return vector2d_to_compas(uvec)
 
     def curvature_at(self, t: float) -> Vector:
         """Compute the curvature vector at a curve parameter.
 
         Parameters
@@ -255,17 +247,17 @@
             If the parameter is not in the curve domain.
 
         """
         start, end = self.domain  # type: ignore (domain could be None if no occ_curve is set)
         if t < start or t > end:
             raise ValueError("The parameter is not in the domain of the curve.")
 
-        point = gp_Pnt2d()
-        uvec = gp_Vec2d()
-        vvec = gp_Vec2d()
+        point = gp.gp_Pnt2d()
+        uvec = gp.gp_Vec2d()
+        vvec = gp.gp_Vec2d()
         self.occ_curve.D2(t, point, uvec, vvec)
         return vector2d_to_compas(vvec)
 
     def frame_at(self, t: float) -> Frame:
         """Compute the local frame at a curve parameter.
 
         Parameters
@@ -283,17 +275,17 @@
             If the parameter is not in the curve domain.
 
         """
         start, end = self.domain  # type: ignore (domain could be None if no occ_curve is set)
         if t < start or t > end:
             raise ValueError("The parameter is not in the domain of the curve.")
 
-        point = gp_Pnt2d()
-        uvec = gp_Vec2d()
-        vvec = gp_Vec2d()
+        point = gp.gp_Pnt2d()
+        uvec = gp.gp_Vec2d()
+        vvec = gp.gp_Vec2d()
         self.occ_curve.D2(t, point, uvec, vvec)
 
         return Frame(
             point2d_to_compas(point),
             vector2d_to_compas(uvec),
             vector2d_to_compas(vvec),
         )
```

### Comparing `compas_occ-1.0.2/src/compas_occ/geometry/curves/nurbs.py` & `compas_occ-1.1.0/src/compas_occ/geometry/curves/nurbs.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from typing import Union
 
 from compas.geometry import Circle
 from compas.geometry import Ellipse
 from compas.geometry import Frame
 from compas.geometry import Line
 from compas.geometry import NurbsCurve
+from compas.geometry import Point
 
 # from OCC.Core.TopoDS import TopoDS_Edge
-from compas.geometry import Point
 from OCC.Core.Geom import Geom_BSplineCurve
 from OCC.Core.GeomAPI import GeomAPI_Interpolate
 from OCC.Core.GeomConvert import GeomConvert_CompCurveToBSplineCurve
 from OCC.Core.TColgp import TColgp_Array1OfPnt
 from OCC.Core.TColStd import TColStd_Array1OfInteger
 from OCC.Core.TColStd import TColStd_Array1OfReal
 
@@ -87,17 +87,15 @@
     >>> curve = OCCNurbsCurve.from_points(points)
 
     Curve from parameters...
 
     >>> from compas.geometry import Point
     >>> from compas_occ.geometry import OCCNurbsCurve
     >>> points = [Point(0, 0, 0), Point(3, 6, 0), Point(6, -3, 3), Point(10, 0, 0)]
-    >>> curve = OCCNurbsCurve.from_parameters(
-    ...     points=points, weights=[1.0, 1.0, 1.0, 1.0], knots=[0.0, 1.0], multiplicities=[4, 4], degree=3
-    ... )
+    >>> curve = OCCNurbsCurve.from_parameters(points=points, weights=[1.0, 1.0, 1.0, 1.0], knots=[0.0, 1.0], multiplicities=[4, 4], degree=3)
 
     """
 
     _occ_curve: Geom_BSplineCurve
 
     @property
     def __data__(self) -> Dict:
```

### Comparing `compas_occ-1.0.2/src/compas_occ/geometry/surfaces/__init__.py` & `compas_occ-1.1.0/src/compas_occ/geometry/surfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_occ-1.0.2/src/compas_occ/geometry/surfaces/extrusion.py` & `compas_occ-1.1.0/src/compas_occ/geometry/surfaces/extrusion.py`

 * *Files identical despite different names*

### Comparing `compas_occ-1.0.2/src/compas_occ/geometry/surfaces/nurbs.py` & `compas_occ-1.1.0/src/compas_occ/geometry/surfaces/nurbs.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import Union
 
 from compas.geometry import Curve
 from compas.geometry import NurbsSurface
 from compas.geometry import Point
 from compas.geometry import Translation
 from compas.geometry import Vector
-from compas.utilities import flatten
+from compas.itertools import flatten
 from OCC.Core.Geom import Geom_BSplineSurface
 from OCC.Core.GeomAbs import GeomAbs_C2
 from OCC.Core.GeomAPI import GeomAPI_PointsToBSplineSurface
 from OCC.Core.GeomFill import GeomFill_BSplineCurves
 from OCC.Core.GeomFill import GeomFill_CoonsStyle
 from OCC.Core.GeomFill import GeomFill_CurvedStyle
 from OCC.Core.GeomFill import GeomFill_StretchStyle
@@ -377,19 +377,15 @@
         if style == "stretch":
             occ_style = GeomFill_StretchStyle
         elif style == "coons":
             occ_style = GeomFill_CoonsStyle
         elif style == "curved":
             occ_style = GeomFill_CurvedStyle
         else:
-            warnings.warn(
-                'This fill style is not supported: {}. We will use GeomFill_StretchStyle ("stretch") instead.'.format(
-                    style
-                )
-            )
+            warnings.warn('This fill style is not supported: {}. We will use GeomFill_StretchStyle ("stretch") instead.'.format(style))
             occ_style = GeomFill_StretchStyle
 
         if curve3 and curve4:
             occ_fill = GeomFill_BSplineCurves(
                 curve1.occ_curve,
                 curve2.occ_curve,
                 curve3.occ_curve,
```

### Comparing `compas_occ-1.0.2/src/compas_occ/geometry/surfaces/revolution.py` & `compas_occ-1.1.0/src/compas_occ/geometry/surfaces/revolution.py`

 * *Files identical despite different names*

### Comparing `compas_occ-1.0.2/src/compas_occ/geometry/surfaces/surface.py` & `compas_occ-1.1.0/src/compas_occ/geometry/surfaces/surface.py`

 * *Files identical despite different names*

### Comparing `compas_occ-1.0.2/src/compas_occ/occ.py` & `compas_occ-1.1.0/src/compas_occ/occ.py`

 * *Files identical despite different names*

### Comparing `compas_occ-1.0.2/src/compas_occ.egg-info/PKG-INFO` & `compas_occ-1.1.0/src/compas_occ.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas_occ
-Version: 1.0.2
+Version: 1.1.0
 Summary: COMPAS wrapper for the Python bindings of OCC.
 Author-email: tom van mele <tom.v.mele@gmail.com>, Lotte Aldinger <aldinger@arch.ethz.ch>, Chen Kasirer <kasirer@arch.ethz.ch>
 License: MIT License
         
         Copyright (c) ETH Zurich - Block Research Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,31 +23,32 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://compas-dev.github.io/compas_occ
 Project-URL: Repository, https://github.com/compas-dev/compas_occ
-Keywords: form finding,dynamic relaxation
+Keywords: compas,nurbs,brep,occ
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: compas>=2.0.0
+Requires-Dist: compas>=2.0.1
 Provides-Extra: dev
 Requires-Dist: attrs>=17.4; extra == "dev"
 Requires-Dist: black>=22.12.0; extra == "dev"
 Requires-Dist: bump-my-version; extra == "dev"
 Requires-Dist: compas_invocations2; extra == "dev"
+Requires-Dist: compas_viewer; extra == "dev"
 Requires-Dist: invoke>=0.14; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: sphinx_compas2_theme; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 
 # COMPAS OCC
```

### Comparing `compas_occ-1.0.2/src/compas_occ.egg-info/SOURCES.txt` & `compas_occ-1.1.0/src/compas_occ.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `compas_occ-1.0.2/tests/test_data_nurbscurve.py` & `compas_occ-1.1.0/tests/test_data_nurbscurve.py`

 * *Files identical despite different names*

### Comparing `compas_occ-1.0.2/tests/test_data_nurbssurface.py` & `compas_occ-1.1.0/tests/test_data_nurbssurface.py`

 * *Files identical despite different names*

