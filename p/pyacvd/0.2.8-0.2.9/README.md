# Comparing `tmp/pyacvd-0.2.8.tar.gz` & `tmp/pyacvd-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyacvd-0.2.8.tar", last modified: Tue Jul 12 14:53:00 2022, max compression
+gzip compressed data, was "pyacvd-0.2.9.tar", last modified: Fri Jan 13 00:17:23 2023, max compression
```

## Comparing `pyacvd-0.2.8.tar` & `pyacvd-0.2.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 14:53:00.931210 pyacvd-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-07-12 14:52:42.000000 pyacvd-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-12 14:52:42.000000 pyacvd-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2419 2022-07-12 14:53:00.931210 pyacvd-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1491 2022-07-12 14:52:42.000000 pyacvd-0.2.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 14:53:00.931210 pyacvd-0.2.8/pyacvd/
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-07-12 14:52:42.000000 pyacvd-0.2.8/pyacvd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-07-12 14:52:42.000000 pyacvd-0.2.8/pyacvd/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    10875 2022-07-12 14:52:42.000000 pyacvd-0.2.8/pyacvd/clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 14:53:00.931210 pyacvd-0.2.8/pyacvd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2419 2022-07-12 14:53:00.000000 pyacvd-0.2.8/pyacvd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-07-12 14:53:00.000000 pyacvd-0.2.8/pyacvd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-12 14:53:00.000000 pyacvd-0.2.8/pyacvd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-07-12 14:53:00.000000 pyacvd-0.2.8/pyacvd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-07-12 14:53:00.000000 pyacvd-0.2.8/pyacvd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      858 2022-07-12 14:52:42.000000 pyacvd-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-07-12 14:53:00.931210 pyacvd-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1856 2022-07-12 14:52:42.000000 pyacvd-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:17:23.683016 pyacvd-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-01-13 00:17:04.000000 pyacvd-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-13 00:17:04.000000 pyacvd-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-01-13 00:17:23.683016 pyacvd-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-01-13 00:17:04.000000 pyacvd-0.2.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:17:23.683016 pyacvd-0.2.9/pyacvd/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-13 00:17:04.000000 pyacvd-0.2.9/pyacvd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-01-13 00:17:04.000000 pyacvd-0.2.9/pyacvd/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-01-13 00:17:04.000000 pyacvd-0.2.9/pyacvd/clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:17:23.683016 pyacvd-0.2.9/pyacvd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-01-13 00:17:23.000000 pyacvd-0.2.9/pyacvd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-01-13 00:17:23.000000 pyacvd-0.2.9/pyacvd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 00:17:23.000000 pyacvd-0.2.9/pyacvd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-13 00:17:23.000000 pyacvd-0.2.9/pyacvd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-13 00:17:23.000000 pyacvd-0.2.9/pyacvd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-01-13 00:17:04.000000 pyacvd-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-01-13 00:17:23.683016 pyacvd-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-01-13 00:17:04.000000 pyacvd-0.2.9/setup.py
```

### Comparing `pyacvd-0.2.8/LICENSE` & `pyacvd-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyacvd-0.2.8/PKG-INFO` & `pyacvd-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: pyacvd
-Version: 0.2.8
+Version: 0.2.9
 Summary: Uniformly remeshes surface meshes
 Home-page: https://github.com/pyvista/pyacvd
 Author: Alex Kaszynski
 Author-email: akascap@gmail.com
 License: MIT
 Keywords: vtk uniform meshing remeshing,acvd
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6.*
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 pyacvd
 ======
 .. image:: https://img.shields.io/pypi/v/pyacvd.svg
     :target: https://pypi.org/project/pyacvd/
```

### Comparing `pyacvd-0.2.8/README.rst` & `pyacvd-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `pyacvd-0.2.8/pyacvd/clustering.py` & `pyacvd-0.2.9/pyacvd/clustering.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """Point based clustering module"""
 import ctypes
-import numpy as np
-from scipy import sparse
-import pyvista as pv
 
+import numpy as np
 from pyacvd import _clustering
+import pyvista as pv
+from scipy import sparse
 
 
 class Clustering:
     """Uniform point clustering based on ACVD.
 
     Parameters
     ----------
     mesh : pyvista.PolyData
         Mesh to cluster.
 
     Examples
     --------
-    Perform a uniform recluster the stanford bunny
+    Perform a uniform recluster of the stanford bunny.
 
     >>> from pyvista import examples
     >>> import pyacvd
     >>> mesh = examples.download_bunny()
     >>> clus = pyacvd.Clustering()
     >>> clus.cluster()
     >>> remeshed = clus.create_mesh()
 
     """
 
     def __init__(self, mesh):
         """Check inputs and initializes neighbors"""
         # mesh must be triangular
-        if not mesh.is_all_triangles():
+        if not mesh.is_all_triangles:
             mesh = mesh.triangulate()
 
         self.mesh = mesh.copy()
         self.clusters = None
         self.nclus = None
         self.remesh = None
         self._area = None
@@ -43,47 +43,49 @@
         self._neigh = None
         self._nneigh = None
         self._edges = None
         self._update_data(None)
 
     def _update_data(self, weights=None):
         # Compute point weights and weighted points
-        self._area, self._wcent = weighted_points(self.mesh,
-                                                  additional_weights=weights)
+        self._area, self._wcent = weighted_points(self.mesh, additional_weights=weights)
 
         # neighbors and edges
         self._neigh, self._nneigh = neighbors_from_mesh(self.mesh)
         self._edges = _clustering.edge_id(self._neigh, self._nneigh)
 
     def cluster(self, nclus, maxiter=100, debug=False, iso_try=10):
-        """Cluster points """
-        self.clusters, _, self.nclus = _clustering.cluster(self._neigh,
-                                                           self._nneigh,
-                                                           nclus,
-                                                           self._area,
-                                                           self._wcent,
-                                                           self._edges,
-                                                           maxiter, debug,
-                                                           iso_try)
+        """Cluster points"""
+        self.clusters, _, self.nclus = _clustering.cluster(
+            self._neigh,
+            self._nneigh,
+            nclus,
+            self._area,
+            self._wcent,
+            self._edges,
+            maxiter,
+            debug,
+            iso_try,
+        )
 
         return self.clusters
 
     def subdivide(self, nsub):
-        """Perform a linear subdivision of the mesh
+        """Perform a linear subdivision of the mesh.
 
         Parameters
         ----------
         nsub : int
             Number of subdivisions
         """
-        self.mesh.overwrite(_subdivide(self.mesh, nsub))
+        self.mesh.copy_from(_subdivide(self.mesh, nsub))
         self._update_data()
 
     def plot(self, random_color=True, **kwargs):
-        """ Plot clusters if available
+        """Plot clusters if available.
 
         Parameters
         ----------
         random_color : bool, optional
             Plots clusters with a random color rather than a color
             based on the order of creation.
 
@@ -91,15 +93,15 @@
             See help(pyvista.plot)
 
         Returns
         -------
         cpos : list
             Camera position.  See help(pyvista.plot)
         """
-        if not hasattr(self, 'clusters'):
+        if not hasattr(self, "clusters"):
             return self.mesh.plot(**kwargs)
 
         # Setup color
         if random_color:
             rand_color = np.random.random(self.nclus)
         else:
             rand_color = np.linspace(0, 1, self.nclus)
@@ -111,74 +113,84 @@
             rng = [-0.25, 1]
         else:
             rng = [0, 1]
 
         return self.mesh.plot(scalars=colors, rng=rng, **kwargs)
 
     def create_mesh(self, flipnorm=True):
-        """ Generates mesh from clusters """
+        """Generates mesh from clusters"""
         if flipnorm:
             cnorm = self.cluster_norm
         else:
             cnorm = None
 
         # Generate mesh
-        self.remesh = create_mesh(self.mesh, self._area, self.clusters,
-                                  cnorm, flipnorm)
+        self.remesh = create_mesh(self.mesh, self._area, self.clusters, cnorm, flipnorm)
         return self.remesh
 
     @property
     def cluster_norm(self):
-        """ Return cluster norms """
-        if not hasattr(self, 'clusters'):
-            raise Exception('No clusters available')
+        """Return cluster norms"""
+        if not hasattr(self, "clusters"):
+            raise Exception("No clusters available")
 
         # Normals of original mesh
         self.mesh.compute_normals(cell_normals=False, inplace=True)
-        norm = self.mesh.point_data['Normals']
+        norm = self.mesh.point_data["Normals"]
 
         # Compute normalized mean cluster normals
         cnorm = np.empty((self.nclus, 3))
         cnorm[:, 0] = np.bincount(self.clusters, weights=norm[:, 0] * self._area)
         cnorm[:, 1] = np.bincount(self.clusters, weights=norm[:, 1] * self._area)
         cnorm[:, 2] = np.bincount(self.clusters, weights=norm[:, 2] * self._area)
-        weights = ((cnorm * cnorm).sum(1)**0.5).reshape((-1, 1))
+        weights = ((cnorm * cnorm).sum(1) ** 0.5).reshape((-1, 1))
         weights[weights == 0] = 1
         cnorm /= weights
         return cnorm
 
     @property
     def cluster_centroid(self):
-        """ Computes an area normalized value for each cluster """
+        """Computes an area normalized value for each cluster"""
         wval = self.mesh.points * self._area.reshape(-1, 1)
-        cval = np.vstack((np.bincount(self.clusters, weights=wval[:, 0]),
-                          np.bincount(self.clusters, weights=wval[:, 1]),
-                          np.bincount(self.clusters, weights=wval[:, 2])))
+        cval = np.vstack(
+            (
+                np.bincount(self.clusters, weights=wval[:, 0]),
+                np.bincount(self.clusters, weights=wval[:, 1]),
+                np.bincount(self.clusters, weights=wval[:, 2]),
+            )
+        )
         weights = np.bincount(self.clusters, weights=self._area)
         weights[weights == 0] = 1
         cval /= weights
         return cval.T
 
 
 def cluster_centroid(cent, area, clusters):
-    """ Computes an area normalized centroid for each cluster """
+    """Computes an area normalized centroid for each cluster"""
 
     # Check if null cluster exists
     null_clusters = np.any(clusters == -1)
     if null_clusters:
         clusters = clusters.copy()
         clusters[clusters == -1] = clusters.max() + 1
 
     wval = cent * area.reshape(-1, 1)
     cweight = np.bincount(clusters, weights=area)
     cweight[cweight == 0] = 1
 
-    cval = np.vstack((np.bincount(clusters, weights=wval[:, 0]),
-                      np.bincount(clusters, weights=wval[:, 1]),
-                      np.bincount(clusters, weights=wval[:, 2]))) / cweight
+    cval = (
+        np.vstack(
+            (
+                np.bincount(clusters, weights=wval[:, 0]),
+                np.bincount(clusters, weights=wval[:, 1]),
+                np.bincount(clusters, weights=wval[:, 2]),
+            )
+        )
+        / cweight
+    )
 
     if null_clusters:
         cval[:, -1] = np.inf
 
     return cval.T
 
 
@@ -193,21 +205,21 @@
     points = mesh.points
     if points.dtype != np.double:
         points = points.astype(np.double)
 
     # Compute centroids
     ccent = np.ascontiguousarray(cluster_centroid(points, area, clusters))
 
-    # Create sparse matrix storing the number of adjcent clusters a point has
+    # Create sparse matrix storing the number of adjacent clusters a point has
     rng = np.arange(faces.shape[0]).reshape((-1, 1))
     a = np.hstack((rng, rng, rng)).ravel()
     b = clusters[faces[:, 1:]].ravel()  # take?
-    c = np.ones(len(a), dtype='bool')
+    c = np.ones(len(a), dtype="bool")
 
-    boolmatrix = sparse.csr_matrix((c, (a, b)), dtype='bool')
+    boolmatrix = sparse.csr_matrix((c, (a, b)), dtype="bool")
 
     # Find all points with three neighboring clusters.  Each of the three
     # cluster neighbors becomes a point on a triangle
     nadjclus = boolmatrix.sum(1)
     adj = np.array(nadjclus == 3).nonzero()[0]
     idx = boolmatrix[adj].nonzero()[1]
 
@@ -225,42 +237,40 @@
 
         # and compare this with the normals of each face
         faces = np.empty((f.shape[0], 4), dtype=f.dtype)
         faces[:, 0] = 3
         faces[:, 1:] = f
 
         tmp_msh = pv.PolyData(points, faces.ravel())
-        tmp_msh.compute_normals(point_normals=False,
-                                inplace=True,
-                                consistent_normals=False)
-        newnorm = tmp_msh.cell_data['Normals']
+        tmp_msh.compute_normals(point_normals=False, inplace=True, consistent_normals=False)
+        newnorm = tmp_msh.cell_data["Normals"]
 
         # If the dot is negative, reverse the order of those faces
         agg = (adjcnorm * newnorm).sum(1)  # dot product
         mask = agg < 0.0
         f[mask] = f[mask, ::-1]
 
     # Create vtk surface
     triangles = np.empty((f.shape[0], 4), dtype=f.dtype)
     triangles[:, -3:] = f
     triangles[:, 0] = 3
     return pv.PolyData(points, triangles.ravel())
 
 
 def unique_row_indices(a):
-    """ Indices of unique rows """
-    b = np.ascontiguousarray(a).view(
-        np.dtype((np.void, a.dtype.itemsize * a.shape[1])))
+    """Indices of unique rows"""
+    b = np.ascontiguousarray(a).view(np.dtype((np.void, a.dtype.itemsize * a.shape[1])))
     _, idx = np.unique(b, return_index=True)
     return idx
 
 
 def weighted_points(mesh, return_weighted=True, additional_weights=None):
     """Returns point weight based on area weight and weighted points.
-    Points are weighted by adjcent area faces.
+
+    Points are weighted by adjacent area faces.
 
     Parameters
     ----------
     mesh : pv.PolyData
         All triangular surface mesh.
 
     return_weighted : bool, optional
@@ -280,21 +290,21 @@
     if faces.dtype != np.int32:
         faces = faces.astype(np.int32)
     points = mesh.points
 
     if additional_weights is not None:
         weights = additional_weights
         return_weighted = True
-        if not weights.flags['C_CONTIGUOUS']:
+        if not weights.flags["C_CONTIGUOUS"]:
             weights = np.ascontiguousarray(weights, dtype=ctypes.c_double)
         elif weights.dtype != ctypes.c_double:
             weights = weights.astype(ctypes.c_double)
 
         if (weights < 0).any():
-            raise Exception('Negtive weights not allowed')
+            raise Exception("Negative weights not allowed.")
 
     else:
         weights = np.array([])
 
     if points.dtype == np.float64:
         weighted_point_func = _clustering.weighted_points_double
     else:
```

### Comparing `pyacvd-0.2.8/pyacvd.egg-info/PKG-INFO` & `pyacvd-0.2.9/pyacvd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: pyacvd
-Version: 0.2.8
+Version: 0.2.9
 Summary: Uniformly remeshes surface meshes
 Home-page: https://github.com/pyvista/pyacvd
 Author: Alex Kaszynski
 Author-email: akascap@gmail.com
 License: MIT
 Keywords: vtk uniform meshing remeshing,acvd
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6.*
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 pyacvd
 ======
 .. image:: https://img.shields.io/pypi/v/pyacvd.svg
     :target: https://pypi.org/project/pyacvd/
```

### Comparing `pyacvd-0.2.8/pyproject.toml` & `pyacvd-0.2.9/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 ]
 
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 junit_family= "legacy"
 filterwarnings = [
-    "ignore::FutureWarning",
-    "ignore::PendingDeprecationWarning",
-    "ignore::DeprecationWarning",
     # bogus numpy ABI warning (see numpy/#432)
     "ignore:.*numpy.dtype size changed.*:RuntimeWarning",
     "ignore:.*numpy.ufunc size changed.*:RuntimeWarning"
 ]
 
 [tool.cibuildwheel]
 archs = ["auto64"]  # 64-bit only
@@ -25,7 +22,18 @@
 test-requires = "pytest"
 test-command = "pytest {project}/tests"
 
 [tool.cibuildwheel.macos]
 # https://cibuildwheel.readthedocs.io/en/stable/faq/#apple-silicon
 archs = ["x86_64", "universal2"]
 test-skip = ["*_arm64", "*_universal2:arm64"]
+
+[tool.codespell]
+skip = '*.cxx,*.h,*.gif,*.png,*.jpg,*.js,*.html,*.doctree,*.ttf,*.woff,*.woff2,*.eot,*.mp4,*.inv,*.pickle,*.ipynb,flycheck*,./.git/*,./.hypothesis/*,*.yml,./doc/build/*,./doc/images/*,./dist/*,*~,.hypothesis*,*.cpp,*.c'
+quiet-level = 3
+
+[tool.isort]
+profile = "black"
+force_sort_within_sections = true
+default_section = "THIRDPARTY"
+skip_glob = ["__init__.py"]
+src_paths = ["doc", "src", "tests"]
```

### Comparing `pyacvd-0.2.8/setup.py` & `pyacvd-0.2.9/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,59 @@
 """Setup for pyacvd"""
-import os
 from io import open as io_open
+import os
 
-from setuptools import setup, Extension
 from Cython.Build import cythonize
 import numpy as np
+from setuptools import Extension, setup
 
 # Get version from version info
 __version__ = None
-version_file = os.path.join(os.path.dirname(__file__), 'pyacvd', '_version.py')
-with io_open(version_file, mode='r') as fd:
+version_file = os.path.join(os.path.dirname(__file__), "pyacvd", "_version.py")
+with io_open(version_file, mode="r") as fd:
     exec(fd.read())
 
 
 def read(*paths):
-    with open(os.path.join(*paths), 'r') as fid:
+    with open(os.path.join(*paths), "r") as fid:
         return fid.read()
 
+
 setup(
-    name='pyacvd',
-    packages=['pyacvd'],
+    name="pyacvd",
+    packages=["pyacvd"],
     version=__version__,
-    description='Uniformly remeshes surface meshes',
-    long_description=read('README.rst'),
-    long_description_content_type='text/x-rst',
+    description="Uniformly remeshes surface meshes",
+    long_description=read("README.rst"),
+    long_description_content_type="text/x-rst",
     ext_modules=cythonize(
         [
             Extension(
                 "pyacvd._clustering",
                 ["pyacvd/cython/_clustering.pyx"],
                 language="c++",
                 include_dirs=[np.get_include()],
             )
         ]
     ),
-    url='https://github.com/pyvista/pyacvd',
-    author='Alex Kaszynski',
-    author_email='akascap@gmail.com',
-    license='MIT',
+    url="https://github.com/pyvista/pyacvd",
+    author="Alex Kaszynski",
+    author_email="akascap@gmail.com",
+    license="MIT",
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'Intended Audience :: Science/Research',
-        'Topic :: Scientific/Engineering :: Information Analysis',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: Microsoft :: Windows',
-        'Operating System :: POSIX',
-        'Operating System :: MacOS',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: Science/Research",
+        "Topic :: Scientific/Engineering :: Information Analysis",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: Microsoft :: Windows",
+        "Operating System :: POSIX",
+        "Operating System :: MacOS",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
-
-    python_requires='>=3.6.*',
-    install_requires=['pyvista>=0.32.0',
-                      'numpy',
-                      'scipy'],
-    keywords='vtk uniform meshing remeshing, acvd',
+    python_requires=">=3.7",
+    install_requires=["pyvista>=0.37.0", "numpy", "scipy"],
+    keywords="vtk uniform meshing remeshing, acvd",
 )
```

