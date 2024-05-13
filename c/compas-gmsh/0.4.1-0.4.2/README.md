# Comparing `tmp/compas_gmsh-0.4.1.tar.gz` & `tmp/compas_gmsh-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compas_gmsh-0.4.1.tar", last modified: Fri Oct  7 12:55:12 2022, max compression
+gzip compressed data, was "compas_gmsh-0.4.2.tar", last modified: Mon May 13 20:54:46 2024, max compression
```

## Comparing `compas_gmsh-0.4.1.tar` & `compas_gmsh-0.4.2.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 12:55:12.600364 compas_gmsh-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-07 12:54:59.000000 compas_gmsh-0.4.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (121)     1227 2022-10-07 12:54:59.000000 compas_gmsh-0.4.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-10-07 12:54:59.000000 compas_gmsh-0.4.1/LICENSE.GPL
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-10-07 12:54:59.000000 compas_gmsh-0.4.1/LICENSE.MIT
--rw-r--r--   0 runner    (1001) docker     (121)      390 2022-10-07 12:54:59.000000 compas_gmsh-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1952 2022-10-07 12:55:12.600364 compas_gmsh-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      902 2022-10-07 12:54:59.000000 compas_gmsh-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-07 12:54:59.000000 compas_gmsh-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      697 2022-10-07 12:55:12.604364 compas_gmsh-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2012 2022-10-07 12:54:59.000000 compas_gmsh-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 12:55:12.600364 compas_gmsh-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 12:55:12.600364 compas_gmsh-0.4.1/src/compas_gmsh/
--rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-10-07 12:54:59.000000 compas_gmsh-0.4.1/src/compas_gmsh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 12:55:12.600364 compas_gmsh-0.4.1/src/compas_gmsh/interop/
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-10-07 12:54:59.000000 compas_gmsh-0.4.1/src/compas_gmsh/interop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 12:55:12.600364 compas_gmsh-0.4.1/src/compas_gmsh/models/
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-10-07 12:54:59.000000 compas_gmsh-0.4.1/src/compas_gmsh/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4644 2022-10-07 12:54:59.000000 compas_gmsh-0.4.1/src/compas_gmsh/models/csg.py
--rw-r--r--   0 runner    (1001) docker     (121)     2034 2022-10-07 12:54:59.000000 compas_gmsh-0.4.1/src/compas_gmsh/models/mesh.py
--rw-r--r--   0 runner    (1001) docker     (121)    11517 2022-10-07 12:54:59.000000 compas_gmsh-0.4.1/src/compas_gmsh/models/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     4952 2022-10-07 12:54:59.000000 compas_gmsh-0.4.1/src/compas_gmsh/models/shape.py
--rw-r--r--   0 runner    (1001) docker     (121)     1008 2022-10-07 12:54:59.000000 compas_gmsh-0.4.1/src/compas_gmsh/options.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 12:55:12.600364 compas_gmsh-0.4.1/src/compas_gmsh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1952 2022-10-07 12:55:12.000000 compas_gmsh-0.4.1/src/compas_gmsh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-10-07 12:55:12.000000 compas_gmsh-0.4.1/src/compas_gmsh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-07 12:55:12.000000 compas_gmsh-0.4.1/src/compas_gmsh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-07 12:55:12.000000 compas_gmsh-0.4.1/src/compas_gmsh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-07 12:55:12.000000 compas_gmsh-0.4.1/src/compas_gmsh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-07 12:55:12.000000 compas_gmsh-0.4.1/src/compas_gmsh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:54:46.329769 compas_gmsh-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-13 20:54:35.000000 compas_gmsh-0.4.2/LICENSE.GPL
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-13 20:54:35.000000 compas_gmsh-0.4.2/LICENSE.MIT
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-13 20:54:46.329769 compas_gmsh-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-13 20:54:35.000000 compas_gmsh-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-13 20:54:35.000000 compas_gmsh-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-13 20:54:35.000000 compas_gmsh-0.4.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-13 20:54:35.000000 compas_gmsh-0.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 20:54:46.329769 compas_gmsh-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:54:46.321768 compas_gmsh-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:54:46.325768 compas_gmsh-0.4.2/src/compas_gmsh/
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-13 20:54:35.000000 compas_gmsh-0.4.2/src/compas_gmsh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:54:46.325768 compas_gmsh-0.4.2/src/compas_gmsh/conversions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:54:35.000000 compas_gmsh-0.4.2/src/compas_gmsh/conversions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:54:46.325768 compas_gmsh-0.4.2/src/compas_gmsh/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-13 20:54:35.000000 compas_gmsh-0.4.2/src/compas_gmsh/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-05-13 20:54:35.000000 compas_gmsh-0.4.2/src/compas_gmsh/models/csg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-05-13 20:54:35.000000 compas_gmsh-0.4.2/src/compas_gmsh/models/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24848 2024-05-13 20:54:35.000000 compas_gmsh-0.4.2/src/compas_gmsh/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-05-13 20:54:35.000000 compas_gmsh-0.4.2/src/compas_gmsh/models/shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7371 2024-05-13 20:54:35.000000 compas_gmsh-0.4.2/src/compas_gmsh/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:54:46.325768 compas_gmsh-0.4.2/src/compas_gmsh/triangulation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:54:35.000000 compas_gmsh-0.4.2/src/compas_gmsh/triangulation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:54:46.325768 compas_gmsh-0.4.2/src/compas_gmsh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-13 20:54:46.000000 compas_gmsh-0.4.2/src/compas_gmsh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-13 20:54:46.000000 compas_gmsh-0.4.2/src/compas_gmsh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:54:46.000000 compas_gmsh-0.4.2/src/compas_gmsh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:54:46.000000 compas_gmsh-0.4.2/src/compas_gmsh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 20:54:46.000000 compas_gmsh-0.4.2/src/compas_gmsh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 20:54:46.000000 compas_gmsh-0.4.2/src/compas_gmsh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:54:46.325768 compas_gmsh-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-13 20:54:35.000000 compas_gmsh-0.4.2/tests/test_dummy.py
```

### Comparing `compas_gmsh-0.4.1/LICENSE.GPL` & `compas_gmsh-0.4.2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `compas_gmsh-0.4.1/LICENSE.MIT` & `compas_gmsh-0.4.2/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `compas_gmsh-0.4.1/README.md` & `compas_gmsh-0.4.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Latest Release](https://img.shields.io/pypi/v/compas_gmsh.svg)](https://pypi.python.org/project/compas_gmsh)
 
 COMPAS friendly interface for Gmsh.
 
 ## Installation
 
 ```bash
-conda create -n gmsh -c conda-forge compas compas_view2 --yes
+conda create -n gmsh -c conda-forge compas
 conda activate gmsh
 pip install compas_gmsh
 ```
 
 ## Getting Started
 
 Have a look at some of the first [examples in the documentation](https://compas.dev/compas_gmsh/latest/examples.html).
```

### Comparing `compas_gmsh-0.4.1/src/compas_gmsh/models/csg.py` & `compas_gmsh-0.4.2/src/compas_gmsh/models/csg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from typing import Tuple
 from typing import List
-from compas_gmsh.models.model import Model
+from typing import Tuple
 
 import compas.geometry
 from compas.geometry import Box
-from compas.geometry import Sphere
 from compas.geometry import Cylinder
+from compas.geometry import Sphere
+
+from .model import Model
 
 
 def add_cylinder(self, cylinder: Cylinder) -> Tuple[int, int]:
     """Add a cylinder to the model."""
     H = cylinder.height
     R = cylinder.radius
     base = cylinder.plane.point
```

### Comparing `compas_gmsh-0.4.1/src/compas_gmsh/models/mesh.py` & `compas_gmsh-0.4.2/src/compas_gmsh/models/mesh.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,29 @@
+from typing import Dict
+from typing import Optional
+from typing import Union
+
 from compas.datastructures import Mesh
-from compas_gmsh.models.model import Model
+
+from .model import Model
 
 
 class MeshModel(Model):
     """Model for mesh (re)meshing."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.vertex_tag = {}
 
     @classmethod
     def from_mesh(
         cls: "MeshModel",
         mesh: Mesh,
         name: str = "Mesh",
-        targetlength: float = 1.0,
+        targetlength: Optional[Union[float, Dict]] = None,
     ) -> "MeshModel":
         """
         Create a mesh model from a mesh.
 
         Parameters
         ----------
         mesh : :class:`Mesh`
@@ -29,39 +34,80 @@
             Target value for the length of the mesh edges.
 
         Returns
         -------
         :class:`MeshModel`
 
         """
-        model = cls(name)
-        model.vertex_tag = {}
+        model: MeshModel = cls(name)
+
         for vertex in mesh.vertices():
             point = mesh.vertex_coordinates(vertex)
-            model.vertex_tag[vertex] = model.occ.add_point(*point, targetlength)
+            if targetlength:
+                if isinstance(targetlength, dict):
+                    length = targetlength.get(vertex)
+                else:
+                    length = targetlength
+                tag = model.occ.add_point(*point, length)
+            else:
+                tag = model.occ.add_point(*point)
+            model.vertex_tag[vertex] = tag
+
         for face in mesh.faces():
             loop = []
             for u, v in mesh.face_halfedges(face):
                 tag = model.occ.add_line(model.vertex_tag[u], model.vertex_tag[v])
                 loop.append(tag)
             tag = model.occ.add_curve_loop(loop)
             model.occ.add_surface_filling(tag)
+
+        model.synchronize()
         return model
 
-    def heal(self) -> None:
+    def generate_mesh(self, dim: int = 2) -> None:
         """
-        Heal the underlying OCC model.
+        Generate a mesh of the current model.
+
+        Parameters
+        ----------
+        dim : int, optional
+            The dimension of the mesh.
 
         Returns
         -------
         None
+            The mesh is stored in the model for further refinement and optimisation.
+            To retrieve the generated mesh, use :meth:`mesh_to_compas`, :meth:`mesh_to_openmesh`, or :meth:`mesh_to_tets`.
+
+        Notes
+        -----
+        The geometry is automatically synchronised with the underlying OCC model.
+        Therefore, there is no need to call :meth:`synchronize` before generating the mesh.
+        To influence the meshing process, use the options of the model (:attr:`options.mesh`).
 
         """
-        self.occ.synchronize()
         self.occ.heal_shapes()
+        self.occ.synchronize()
+        self.mesh.generate(dim)
+
+    def find_point_at_vertex(self, vertex: int) -> int:
+        """Find the model point at a vertex of the input mesh.
+
+        Parameters
+        ----------
+        vertex : int
+            A vertex of the input mesh.
+
+        Returns
+        -------
+        int
+            The point identifier.
+
+        """
+        return self.vertex_tag[vertex]
 
     def mesh_targetlength_at_vertex(self, vertex: int, target: float) -> None:
         """
         Set the target length at a particular mesh vertex.
 
         Parameters
         ----------
@@ -73,7 +119,17 @@
         Returns
         -------
         None
 
         """
         tag = self.vertex_tag[vertex]
         self.occ.mesh.set_size([(0, tag)], target)
+
+    def read_options_from_attributes(self) -> None:
+        """Read the model options from the attributes of the mesh data structure.
+
+        Returns
+        -------
+        None
+
+        """
+        pass
```

### Comparing `compas_gmsh-0.4.1/src/compas_gmsh/models/shape.py` & `compas_gmsh-0.4.2/src/compas_gmsh/models/shape.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from typing import Tuple, List
+from typing import List
+from typing import Tuple
 
+from compas.geometry import Box
 from compas.geometry import Cylinder
 from compas.geometry import Sphere
-from compas.geometry import Box
 
-from compas_gmsh.models.model import Model
+from .model import Model
 
 
 class ShapeModel(Model):
     """
     Model for shape combinations.
     """
 
@@ -54,28 +55,26 @@
         Parameters
         ----------
         A : list of tuple
             The *dimtags* of the *object* shapes.
         B : tuple
             The *dimtags* of the *tool* shapes.
 
-        Results
+        Returns
         -------
         list of tuple
             The dimtags of the resulting shapes.
 
         Notes
         -----
         The *objects* are the shapes to which the boolean operation should be applied.
         The *tools* are the shapes used to perform the operation.
 
         """
-        result = self.occ.intersect(
-            A, B, removeObject=remove_objects, removeTool=remove_tools
-        )
+        result = self.occ.intersect(A, B, removeObject=remove_objects, removeTool=remove_tools)
         dimtags = result[0]
         return dimtags
 
     def boolean_union(
         self,
         A: List[Tuple[int, int]],
         B: List[Tuple[int, int]],
@@ -88,28 +87,26 @@
         Parameters
         ----------
         A : list of tuple
             The *dimtags* of the *object* shapes.
         B : tuple
             The *dimtags* of the *tool* shapes.
 
-        Results
+        Returns
         -------
         list of tuple
             The dimtags of the resulting shapes.
 
         Notes
         -----
         The *objects* are the shapes to which the boolean operation should be applied.
         The *tools* are the shapes used to perform the operation.
 
         """
-        result = self.occ.fuse(
-            A, B, removeObject=remove_objects, removeTool=remove_tools
-        )
+        result = self.occ.fuse(A, B, removeObject=remove_objects, removeTool=remove_tools)
         dimtags = result[0]
         return dimtags
 
     def boolean_difference(
         self,
         A: List[Tuple[int, int]],
         B: List[Tuple[int, int]],
@@ -122,28 +119,26 @@
         Parameters
         ----------
         A : list of tuple
             The *dimtags* of the *object* shapes.
         B : tuple
             The *dimtags* of the *tool* shapes.
 
-        Results
+        Returns
         -------
         list of tuple
             The dimtags of the resulting shapes.
 
         Notes
         -----
         The *objects* are the shapes to which the boolean operation should be applied.
         The *tools* are the shapes used to perform the operation.
 
         """
-        result = self.occ.cut(
-            A, B, removeObject=remove_objects, removeTool=remove_tools
-        )
+        result = self.occ.cut(A, B, removeObject=remove_objects, removeTool=remove_tools)
         dimtags = result[0]
         return dimtags
 
     def boolean_fragment(
         self,
         A: List[Tuple[int, int]],
         B: List[Tuple[int, int]],
@@ -156,23 +151,21 @@
         Parameters
         ----------
         A : list of tuple
             The *dimtags* of the *object* shapes.
         B : tuple
             The *dimtags* of the *tool* shapes.
 
-        Results
+        Returns
         -------
         list of tuple
             The dimtags of the resulting shapes.
 
         Notes
         -----
         The *objects* are the shapes to which the boolean operation should be applied.
         The *tools* are the shapes used to perform the operation.
 
         """
-        result = self.occ.fragment(
-            A, B, removeObject=remove_objects, removeTool=remove_tools
-        )
+        result = self.occ.fragment(A, B, removeObject=remove_objects, removeTool=remove_tools)
         dimtags = result[0]
         return dimtags
```

### Comparing `compas_gmsh-0.4.1/src/compas_gmsh.egg-info/SOURCES.txt` & `compas_gmsh-0.4.2/src/compas_gmsh.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-AUTHORS.md
-CHANGELOG.md
 LICENSE.GPL
 LICENSE.MIT
-MANIFEST.in
 README.md
+pyproject.toml
+requirements-dev.txt
 requirements.txt
-setup.cfg
-setup.py
 src/compas_gmsh/__init__.py
 src/compas_gmsh/options.py
 src/compas_gmsh.egg-info/PKG-INFO
 src/compas_gmsh.egg-info/SOURCES.txt
 src/compas_gmsh.egg-info/dependency_links.txt
 src/compas_gmsh.egg-info/not-zip-safe
 src/compas_gmsh.egg-info/requires.txt
 src/compas_gmsh.egg-info/top_level.txt
-src/compas_gmsh/interop/__init__.py
+src/compas_gmsh/conversions/__init__.py
 src/compas_gmsh/models/__init__.py
 src/compas_gmsh/models/csg.py
 src/compas_gmsh/models/mesh.py
 src/compas_gmsh/models/model.py
-src/compas_gmsh/models/shape.py
+src/compas_gmsh/models/shape.py
+src/compas_gmsh/triangulation/__init__.py
+tests/test_dummy.py
```

