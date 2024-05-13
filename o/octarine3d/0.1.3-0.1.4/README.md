# Comparing `tmp/octarine3d-0.1.3.tar.gz` & `tmp/octarine3d-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octarine3d-0.1.3.tar", last modified: Wed Apr 24 10:07:23 2024, max compression
+gzip compressed data, was "octarine3d-0.1.4.tar", last modified: Mon May 13 10:24:49 2024, max compression
```

## Comparing `octarine3d-0.1.3.tar` & `octarine3d-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:07:23.577922 octarine3d-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-24 10:07:18.000000 octarine3d-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-04-24 10:07:23.577922 octarine3d-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-24 10:07:18.000000 octarine3d-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:07:23.573922 octarine3d-0.1.3/octarine/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-24 10:07:18.000000 octarine3d-0.1.3/octarine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 10:07:18.000000 octarine3d-0.1.3/octarine/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-24 10:07:18.000000 octarine3d-0.1.3/octarine/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-04-24 10:07:18.000000 octarine3d-0.1.3/octarine/controls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-24 10:07:18.000000 octarine3d-0.1.3/octarine/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-04-24 10:07:18.000000 octarine3d-0.1.3/octarine/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-24 10:07:18.000000 octarine3d-0.1.3/octarine/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-24 10:07:18.000000 octarine3d-0.1.3/octarine/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    41852 2024-04-24 10:07:18.000000 octarine3d-0.1.3/octarine/viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20188 2024-04-24 10:07:18.000000 octarine3d-0.1.3/octarine/visuals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:07:23.577922 octarine3d-0.1.3/octarine3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-04-24 10:07:23.000000 octarine3d-0.1.3/octarine3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-24 10:07:23.000000 octarine3d-0.1.3/octarine3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:07:23.000000 octarine3d-0.1.3/octarine3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:07:23.000000 octarine3d-0.1.3/octarine3d.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-24 10:07:23.000000 octarine3d-0.1.3/octarine3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 10:07:23.000000 octarine3d-0.1.3/octarine3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 10:07:18.000000 octarine3d-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 10:07:23.577922 octarine3d-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-24 10:07:18.000000 octarine3d-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:24:49.782918 octarine3d-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-13 10:24:47.000000 octarine3d-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-13 10:24:49.782918 octarine3d-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-13 10:24:47.000000 octarine3d-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:24:49.778918 octarine3d-0.1.4/octarine/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-13 10:24:47.000000 octarine3d-0.1.4/octarine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-13 10:24:47.000000 octarine3d-0.1.4/octarine/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-13 10:24:47.000000 octarine3d-0.1.4/octarine/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-05-13 10:24:47.000000 octarine3d-0.1.4/octarine/controls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-13 10:24:47.000000 octarine3d-0.1.4/octarine/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-05-13 10:24:47.000000 octarine3d-0.1.4/octarine/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-13 10:24:47.000000 octarine3d-0.1.4/octarine/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-05-13 10:24:47.000000 octarine3d-0.1.4/octarine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49574 2024-05-13 10:24:47.000000 octarine3d-0.1.4/octarine/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23722 2024-05-13 10:24:47.000000 octarine3d-0.1.4/octarine/visuals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:24:49.778918 octarine3d-0.1.4/octarine3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-13 10:24:49.000000 octarine3d-0.1.4/octarine3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-13 10:24:49.000000 octarine3d-0.1.4/octarine3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 10:24:49.000000 octarine3d-0.1.4/octarine3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 10:24:49.000000 octarine3d-0.1.4/octarine3d.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-13 10:24:49.000000 octarine3d-0.1.4/octarine3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-13 10:24:49.000000 octarine3d-0.1.4/octarine3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-13 10:24:47.000000 octarine3d-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 10:24:49.782918 octarine3d-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-13 10:24:47.000000 octarine3d-0.1.4/setup.py
```

### Comparing `octarine3d-0.1.3/LICENSE` & `octarine3d-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `octarine3d-0.1.3/PKG-INFO` & `octarine3d-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octarine3d
-Version: 0.1.3
+Version: 0.1.4
 Summary: WGPU-based 3d viewer
 Home-page: https://github.com/schlegelp/octarine
 Author: Philipp Schlegel
 Author-email: pms70@cam.ac.uk
 License: BSD-2-Clause
 Project-URL: Documentation, https://schlegelp.github.io/octarine/
 Project-URL: Source, https://github.com/schlegelp/octarine
@@ -36,14 +36,16 @@
 Requires-Dist: mkdocs-material[imaging]; extra == "docs"
 Requires-Dist: mkdocstrings-python; extra == "docs"
 Requires-Dist: mkdocs-minify-plugin; extra == "docs"
 Requires-Dist: mkdocs-literate-nav; extra == "docs"
 Requires-Dist: mkdocs-gen-files; extra == "docs"
 Requires-Dist: mkdocs-glightbox; extra == "docs"
 Requires-Dist: mkdocs-section-index; extra == "docs"
+Requires-Dist: trimesh; extra == "docs"
+Requires-Dist: importlib-metadata; extra == "docs"
 
 ![octarine banner](https://schlegelp.github.io/octarine/_static/octarine_logo_banner.png)
 <p align="center">
 <i>
 Octarine is the eighth color of the Discworld's spectrum, which is described as the color of magic itself. Only wizards and cats can see it.
 </i>
 </p>
@@ -97,14 +99,19 @@
 m = gfx.geometries.mobius_strip_geometry()
 v.add(m, color='b')
 
 # Close the viewer
 v.close()
 ```
 
+> [!NOTE]
+> The above example will work in interactive environments such as IPython and Jupyter. When using from the standard
+> REPL or when running as a script you will have to additionally start the event loop. Please see corresponding the
+> section in the [Introduction](https://schlegelp.github.io/octarine/intro/).
+
 ![demo gif](docs/_static/octarine_demo_720p.gif)
 
 ## Want to learn more?
 Head over to the [**Documentation**](https://schlegelp.github.io/octarine/)!
 
 ## Want to contribute?
 We welcome all kinds of contributions. For example:
```

### Comparing `octarine3d-0.1.3/README.md` & `octarine3d-0.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -54,14 +54,19 @@
 m = gfx.geometries.mobius_strip_geometry()
 v.add(m, color='b')
 
 # Close the viewer
 v.close()
 ```
 
+> [!NOTE]
+> The above example will work in interactive environments such as IPython and Jupyter. When using from the standard
+> REPL or when running as a script you will have to additionally start the event loop. Please see corresponding the
+> section in the [Introduction](https://schlegelp.github.io/octarine/intro/).
+
 ![demo gif](docs/_static/octarine_demo_720p.gif)
 
 ## Want to learn more?
 Head over to the [**Documentation**](https://schlegelp.github.io/octarine/)!
 
 ## Want to contribute?
 We welcome all kinds of contributions. For example:
```

### Comparing `octarine3d-0.1.3/octarine/config.py` & `octarine3d-0.1.4/octarine/config.py`

 * *Files identical despite different names*

### Comparing `octarine3d-0.1.3/octarine/controls.py` & `octarine3d-0.1.4/octarine/controls.py`

 * *Files identical despite different names*

### Comparing `octarine3d-0.1.3/octarine/conversion.py` & `octarine3d-0.1.4/octarine/conversion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pygfx as gfx
 import trimesh as tm
 
 from .utils import is_hashable, is_points, is_lines, is_volume, is_mesh_like, is_pygfx_visual, is_pygfx_geometry
-from .visuals import points2gfx, lines2gfx, mesh2gfx, trimesh2gfx, volume2gfx, scene2gfx
+from .visuals import points2gfx, lines2gfx, mesh2gfx, trimesh2gfx, volume2gfx, scene2gfx, geometry2gfx, visual_passthrough
 
 CONVERTERS = {
-    is_pygfx_visual: lambda x: x,  # pass-through
-    is_pygfx_geometry: lambda x: gfx.Mesh(x, gfx.MeshPhongMaterial()),  # add default material and return
+    is_pygfx_visual: visual_passthrough,  # pass-through
+    is_pygfx_geometry: geometry2gfx,  # add default material and return
     tm.Trimesh: trimesh2gfx,
     tm.Scene: scene2gfx,
     is_mesh_like: mesh2gfx,
     is_points: points2gfx,
     is_lines: lines2gfx,
     is_volume: volume2gfx
 }
```

### Comparing `octarine3d-0.1.3/octarine/jupyter.py` & `octarine3d-0.1.4/octarine/jupyter.py`

 * *Files identical despite different names*

### Comparing `octarine3d-0.1.3/octarine/plugins.py` & `octarine3d-0.1.4/octarine/plugins.py`

 * *Files identical despite different names*

### Comparing `octarine3d-0.1.3/octarine/utils.py` & `octarine3d-0.1.4/octarine/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,14 +190,20 @@
         if 'zmqshell' in ipy_str:
             return 'jupyter'
         elif 'colab' in ipy_str:
             return 'colab'
         else:  # if 'terminal' in ipy_str:
             return 'ipython'
     except BaseException:
+        try:
+            # This is not perfect but should work in most cases
+            if hasattr(__main__.__file__):  # noqa: F821
+                return 'script'
+        except BaseException:
+            pass
         return 'terminal'
 
 
 def is_jupyter() -> bool:
     """Test if navis is run in a Jupyter notebook.
 
     Also returns True if inside Google colaboratory!
```

### Comparing `octarine3d-0.1.3/octarine/viewer.py` & `octarine3d-0.1.4/octarine/viewer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import png
+import time
 import cmap
 import uuid
 import random
 import inspect
 
 import numpy as np
 import pygfx as gfx
 
 from functools import wraps
 from collections import OrderedDict
 
-from wgpu.gui.auto import WgpuCanvas
+from wgpu.gui.auto import WgpuCanvas, run
 from wgpu.gui.offscreen import WgpuCanvas as WgpuCanvasOffscreen
 
-from .visuals import mesh2gfx, volume2gfx, points2gfx, lines2gfx
+from .visuals import mesh2gfx, volume2gfx, points2gfx, lines2gfx, text2gfx
 from .conversion import get_converter
 from . import utils, config
 
 
 __all__ = ["Viewer"]
 
 logger = config.get_logger(__name__)
@@ -72,18 +73,20 @@
                 Size of the viewer window.
     camera :    "ortho" | "perspective", optional
                 Type of camera to use. Defaults to "ortho". Note you can always
                 change the camera type by adjust the `Viewer.camera.fov` attribute
                 (0 = ortho, >0 = perspective).
     control :   "trackball" | "panzoom" | "fly" | "orbit"
                 Controller type to use. Defaults to "trackball".
-    show :      bool, optional
-                Whether to immediately show the viewer. Note that this has no
-                effect in Jupyter. There you will have to call ``.show()`` manually
-                on the last line of a cell for the viewer to appear.
+    show :      bool
+                Whether to immediately show the viewer. A few notes:
+                 1. This has no effect in Jupyter. There you will have to call ``.show()``
+                    manually on the last line of a cell for the viewer to appear.
+                 2. When running in a non-interactive script or REPL, you have to also start
+                    the event loop manually. See the `Viewer.show()` method for more information.
     **kwargs
                 Keyword arguments are passed through to ``WgpuCanvas``.
 
     """
 
     # Palette used for assigning colors to objects
     palette = "seaborn:tab10"
@@ -167,77 +170,103 @@
             "orbit": gfx.OrbitController,
         }.get(control, None)
         if controller is None:
             raise ValueError(f"Unknown controller type: {control}")
 
         self.controller = controller(self.camera, register_events=self.renderer)
 
+        # Setup overlay
+        self.overlay_camera = gfx.NDCCamera()
+        self.overlay_scene = gfx.Scene()
+
         # Stats
         self.stats = gfx.Stats(self.renderer)
         self._show_fps = False
 
         # Setup key events
-        self.key_events = {}
-        self.key_events["1"] = lambda: self.set_view("XY")
-        self.key_events["2"] = lambda: self.set_view("XZ")
-        self.key_events["3"] = lambda: self.set_view("YZ")
-        self.key_events["f"] = lambda: self._toggle_fps()
-        self.key_events["c"] = lambda: self._toggle_controls()
+        self._key_events = {}
+        self._key_events["1"] = lambda: self.set_view("XY")
+        self._key_events["2"] = lambda: self.set_view("XZ")
+        self._key_events["3"] = lambda: self.set_view("YZ")
+        self._key_events["f"] = lambda: self._toggle_fps()
+        self._key_events["c"] = lambda: self._toggle_controls()
 
         def _keydown(event):
             """Handle key presses."""
-            if event.key in self.key_events:
-                self.key_events[event.key]()
+            if not event.modifiers:
+                if event.key in self._key_events:
+                    self._key_events[event.key]()
+            else:
+                tup = (event.key, tuple(event.modifiers))
+                if tup in self._key_events:
+                    self._key_events[tup]()
 
         # Register events
         self.renderer.add_event_handler(_keydown, "key_down")
 
         # Finally, setting some variables
         self._show_bounds = False
         self._shadows = False
-        self._animations = []
+        self._animations = {}
+        self._animations_flagged_for_removal = []
 
         # This starts the animation loop
         if show and not self._is_jupyter:
-            self.show()
+            self.show(start_loop=show == "start_loop")
 
     def _animate(self):
-        """Animate the scene."""
-        to_remove = []
-        for i, func in enumerate(self._animations):
+        """Run the rendering loop."""
+        # First run the user animations
+        # Note: we're iterating over the list because the user might add / remove
+        # animations during the loop
+        for i, (func, on_error) in enumerate(list(self._animations.items())):
             try:
                 func()
             except BaseException as e:
-                logger.error(
-                    f"Removing animation function {func} because of error: {e}"
-                )
-                to_remove.append(i)
-        for i in to_remove[::-1]:
-            self.remove_animation(i)
+                if on_error == "raise":
+                    raise e
+                elif on_error == "remove":
+                    logger.error(
+                        f"Removing animation function '{func}' because of error: {e}"
+                    )
+                    # Flag animation for removal
+                    self._animations_flagged_for_removal.append(i)
+
+        # Check if any animations need to be removed
+        for f in self._animations_flagged_for_removal[::-1]:
+            self._animations.pop(f)
+        self._animations_flagged_for_removal = []
 
+        # Now render the scene
         if self._show_fps:
             with self.stats:
                 self.renderer.render(self.scene, self.camera, flush=False)
+                self.renderer.render(
+                    self.overlay_scene, self.overlay_camera, flush=False
+                )
             self.stats.render()
         else:
-            self.renderer.render(self.scene, self.camera)
+            self.renderer.render(self.scene, self.camera, flush=False)
+            self.renderer.render(self.overlay_scene, self.overlay_camera)
+
         self.canvas.request_draw()
 
     def _next_color(self):
         """Return next color in the colormap."""
         # Cache the full palette. N.B. that ordering of colors in cmap depends on
         # the number of colors requested - i.e. we can't just grab the last color.
-        if (
-            not hasattr(self, "__cached_palette")
-            or self.palette != self.__cached_palette
-        ):
-            self.__cached_colors = list(cmap.Colormap(self.palette).iter_colors())
-            self.__cached_palette = self.palette
+        if not hasattr(self, "_cached_palette") or self.palette != self._cached_palette:
+            self._cached_colors = list(cmap.Colormap(self.palette).iter_colors())
+            self._cached_palette = self.palette
+
+        if not hasattr(self, "_palette_index"):
+            self._palette_index = -1
+        self._palette_index += 1
 
-        return self.__cached_colors[len(self.objects) % len(self.__cached_colors)]
+        return self._cached_colors[self._palette_index % len(self._cached_colors)]
 
     def _next_label(self, prefix="Object"):
         """Return next label."""
         existing = [o for o in self.objects if str(o).startswith(prefix)]
         if len(existing) == 0:
             return prefix
         return f"{prefix}.{len(existing) + 1:03}"
@@ -425,46 +454,55 @@
         for ob in self._object_ids:
             objects[ob] = [
                 v for v in self.visuals if getattr(v, "_object_id", None) == ob
             ]
 
         return objects
 
-    def add_animation(self, x):
+    def add_animation(self, x, on_error="remove"):
         """Add animation function to the Viewer.
 
         Parameters
         ----------
-        x :     callable
-                Function to add to the animation loop.
+        x :         callable
+                    Function to add to the animation loop.
+        on_error :  "remove" | "ignore" | "raise"
+                    What to do if the function throws an error. If "remove",
+                    the function will be removed from the animation loop. If
+                    "ignore", the error will be ignored and the function will
+                    continue to be called.
 
         """
         if not callable(x):
             raise TypeError(f"Expected callable, got {type(x)}")
 
-        self._animations.append(x)
+        assert on_error in ["remove", "ignore", "raise"]
+
+        self._animations[x] = on_error
 
     def remove_animation(self, x):
         """Remove animation function from the Viewer.
 
         Parameters
         ----------
         x :     callable | int
                 Either the function itself or its index
                 in the list of animations.
 
         """
         if callable(x):
-            self._animations.remove(x)
+            self._animations_flagged_for_removal.append(x)
         elif isinstance(x, int):
-            self._animations.pop(x)
+            self._animations_flagged_for_removal.append(
+                list(self._animations.keys())[x]
+            )
         else:
             raise TypeError(f"Expected callable or index (int), got {type(x)}")
 
-    def show(self, use_sidecar=False, toolbar=False):
+    def show(self, use_sidecar=False, toolbar=False, start_loop=False):
         """Show viewer.
 
         Parameters
         ----------
 
         For Jupyter lab only:
 
@@ -473,43 +511,139 @@
                       viewer outside the notebooks. Will throw an error if
                       Sidecar is not installed.
         toolbar :     bool
                       If True, will show a toolbar. You can always show/hide
                       the toolbar with ``viewer.show_controls()`` and
                       ``viewer.hide_controls()``, or the `c` hotkey.
 
+        For scripts & standard REPL:
+
+        start_loop :  bool
+                      If True, will start the blocking (!) event loop. This is
+                      the recommended way to show the viewer when using it in a script.
+                      From an interactive REPL such as IPython you should be able to
+                      just call ``Viewer.show()`` and the interactive viewer will appear
+                      while still allowing you to interact with the REPL.
+
         """
         # This is for e.g. headless testing
         if getattr(config, "HEADLESS", False):
             logger.info("Viewer widget not shown - running in headless mode.")
             return
 
         # Start the animation loop
         self.canvas.request_draw(self._animate)
 
         # If this is an offscreen canvas, we don't need to show anything
         if isinstance(self.canvas, WgpuCanvasOffscreen):
             return
         # In terminal we can just show the window
         elif not self._is_jupyter:
-            self.canvas.show()
+            # Not all backends have a show method
+            if hasattr(self.canvas, "show"):
+                self.canvas.show()
+
+            if start_loop:
+                run()
+            elif utils._type_of_script() in ("terminal", "script"):
+                logger.warning(
+                    "Running in a (potentially) non-interactive terminal or script "
+                    "environment. You may have to manually start the event loop "
+                    "for the canvas to render:\n\n"
+                    "  >>> v = octarine.Viewer(show=False)\n"
+                    "  >>> ...  # setup your viewer\n"
+                    "  >>> v.show(start_loop=True)\n\n"
+                    "Alternatively, use the `start_loop` argument:\n\n"
+                    "  >>> from wgpu.gui.auto import run\n"
+                    "  >>> ...  # setup your viewer\n"
+                    "  >>> run()\n\n"  # do not remove the \n\n here
+                )
         # For Jupyter we need to wrap the canvas in a widget
         else:
             # if not hasattr(self, 'widget'):
             from .jupyter import JupyterOutput
 
             # Construct the widget
             self.widget = JupyterOutput(
                 self,
                 use_sidecar=use_sidecar,
                 toolbar=toolbar,
                 sidecar_kwargs={"title": self._title},
             )
             return self.widget
 
+    def show_message(
+        self, message, position="top-right", font_size=20, color=None, duration=None
+    ):
+        """Show message on canvas.
+
+        Parameters
+        ----------
+        message :   str | None
+                    Message to show. Set to `None` to remove the existing message.
+        position :  "top-left" | "top-right" | "bottom-left" | "bottom-right" | "center"
+                    Position of the message on the canvas.
+        font_size : int, optional
+                    Font size of the message.
+        color :     str | tuple, optional
+                    Color of the message. If `None`, will use white.
+        duration :  int, optional
+                    Number of seconds after which to fade the message.
+
+        """
+        if message is None and hasattr(self, "_message_text"):
+            self.overlay_scene.remove(self._message_text)
+            del self._message_text
+            return
+
+        _positions = {
+            "top-left": (-0.95, 0.95, 0),
+            "top-right": (0.95, 0.95, 0),
+            "bottom-left": (-0.95, -0.95, 0),
+            "bottom-right": (0.95, -0.95, 0),
+            "center": (0, 0, 0),
+        }
+        if position not in _positions:
+            raise ValueError(f"Unknown position: {position}")
+
+        if not hasattr(self, "_message_text"):
+            self._message_text = text2gfx(
+                message, color="white", font_size=font_size, screen_space=True
+            )
+
+        # Make sure the text is in the scene
+        if self._message_text not in self.overlay_scene.children:
+            self.overlay_scene.add(self._message_text)
+
+        self._message_text.geometry.set_text(message)
+        self._message_text.geometry.font_size = font_size
+        self._message_text.geometry.anchor = position
+        if color is not None:
+            self._message_text.material.color = cmap.Color(color).rgba
+        self._message_text.material.opacity = 1
+        self._message_text.local.position = _positions[position]
+
+        # When do we need to start fading out?
+        if duration:
+            self._fade_out_time = time.time() + duration
+
+            def _fade_message():
+                if not hasattr(self, "_message_text"):
+                    self.remove_animation(_fade_message)
+                else:
+                    if time.time() > self._fade_out_time:
+                        # This means the text will fade fade over 1/0.02 = 50 frames
+                        self._message_text.material.opacity = max(self._message_text.material.opacity - 0.02, 0)
+
+                    if self._message_text.material.opacity <= 0:
+                        self.overlay_scene.remove(self._message_text)
+                        self.remove_animation(_fade_message)
+
+            self.add_animation(_fade_message)
+
     def show_controls(self):
         """Show controls."""
         if self._is_jupyter:
             if self.widget.toolbar:
                 self.widget.toolbar.show()
         else:
             if not hasattr(self, "_controls"):
@@ -553,18 +687,18 @@
     @update_viewer(legend=True, bounds=True)
     def remove_objects(self, to_remove):
         """Remove given neurons/visuals from canvas."""
         to_remove = utils.make_iterable(to_remove)
 
         for vis in self.scene.children:
             if vis in to_remove:
-                self.scene.children.remove(vis)
+                self.scene.remove(vis)
             elif hasattr(vis, "_object_id"):
                 if vis._object_id in to_remove:
-                    self.scene.children.remove(vis)
+                    self.scene.remove(vis)
 
     @update_viewer(legend=True, bounds=True)
     def pop(self, N=1):
         """Remove the most recently added N visuals."""
         for vis in list(self.objects.values())[-N:]:
             self.remove_objects(vis)
 
@@ -717,15 +851,17 @@
 
     def add_mesh(self, mesh, name=None, color=None, alpha=None, center=True):
         """Add mesh to canvas.
 
         Parameters
         ----------
         mesh :      Mesh-like
-                    Mesh to plot.
+                    Mesh to plot. If this is a pygfx.Mesh, it will be added
+                    directly to the scene without modification (i.e. `color`,
+                    `alpha`, etc. will be ignored).
         name :      str, optional
                     Name for the visual.
         color :     str | tuple, optional
                     Color to use for plotting. If multiple colors,
                     must be a list of colors with the same length as
                     the number of faces or vertices.
         alpha :     float, optional
@@ -740,15 +876,19 @@
         if color is None:
             color = self._next_color()
         if name is None:
             name = self._next_label("Mesh")
         elif not isinstance(name, str):
             name = str(name)
 
-        visual = mesh2gfx(mesh, color=color, alpha=alpha)
+        if not isinstance(mesh, gfx.Mesh):
+            visual = mesh2gfx(mesh, color=color, alpha=alpha)
+        else:
+            visual = mesh
+
         visual._object_id = name if name else uuid.uuid4()
 
         self._add_to_scene(visual, center)
 
     def add_points(
         self,
         points,
@@ -1220,7 +1360,44 @@
             )
         elif view == "YZ":
             self.camera.show_object(
                 self.scene, scale=1, view_dir=(-1.0, 0.0, 0.0), up=(0.0, -1.0, 0.0)
             )
         else:
             raise TypeError(f"Unable to set view from {type(view)}")
+
+    def bind_key(self, key, func, modifiers=None):
+        """Bind a function to a key press.
+
+        Note that any existing keybindings for `key` + `modifiers` will be
+        silently overwritten.
+
+        Parameters
+        ----------
+        key :       str
+                    Key to bind to. Can be any key on the keyboard.
+        func :      callable
+                    Function to call when key is pressed.
+        modifiers : str | list thereof, optional
+                    Modifier(s) to use with the key. Can be "Shift", "Control",
+                    "Alt" or "Meta".
+
+        """
+        if not callable(func):
+            raise TypeError("`func` needs to be callable")
+
+        if not isinstance(key, str):
+            raise TypeError(f"Expected `key` to be a string, got {type(key)}")
+
+        if modifiers is None:
+            self._key_events[key] = func
+        else:
+            # We need to make `modifiers` is hashable
+            if isinstance(key, str):
+                key = (key,)
+            elif isinstance(key, (set, list)):
+                key = tuple(key)
+
+            if not isinstance(modifiers, tuple):
+                raise TypeError(f"Unexpected datatype for `modifiers`: {type(modifiers)}")
+
+            self._key_events[(key, modifiers)] = func
```

### Comparing `octarine3d-0.1.3/octarine/visuals.py` & `octarine3d-0.1.4/octarine/visuals.py`

 * *Files 11% similar despite different names*

```diff
@@ -45,28 +45,59 @@
     # Add custom attributes
     vis._object_type = "mesh"
     vis._object_id = uuid.uuid4()
 
     return vis
 
 
+def geometry2gfx(geometry, color, alpha=None):
+    """Convert a pygfx.Geometry to a pygfx.Mesh.
+
+    Parameters
+    ----------
+    geometry :      pygfx.Geometry
+                    Geometry to convert.
+    color :         str | tuple | array
+                    Color to use for plotting. If multiple colors,
+                    must be a list of colors with the same length as
+                    the number of faces or vertices.
+    alpha :         float, optional
+                    Opacity value [0-1]. If provided, will override
+                    the alpha channel of the color.
+
+    """
+    # Parse color
+    mat_color_kwargs, obj_color_kwargs = parse_mesh_color(geometry, color, alpha)
+
+    if "colors" in obj_color_kwargs:
+        geometry.colors = obj_color_kwargs["colors"]
+
+    vis = gfx.Mesh(geometry, gfx.MeshPhongMaterial(**mat_color_kwargs))
+
+    # Add custom attributes
+    vis._object_type = "mesh"
+    vis._object_id = uuid.uuid4()
+
+    return vis
+
+
 def parse_mesh_color(mesh, color, alpha=None):
     """Parse color for mesh plotting."""
     mat_color_kwargs = dict()
     obj_color_kwargs = dict()
     if isinstance(color, np.ndarray) and color.ndim == 2:
         if alpha is not None:
             if color.shape[1] == 3:
                 color = np.hstack((color, np.ones((color.shape[0], 1))))
             elif color.shape[1] != 4:
                 raise ValueError("Expected colors to have 3 or 4 channels.")
             color[:, -1] = alpha
 
         # Make sure the color is what pygfx expects
-        if color.dtype in (np.float64, ):
+        if color.dtype in (np.float64,):
             color = color.astype(np.float32, copy=False)
 
         if len(color) == len(mesh.vertices):
             obj_color_kwargs = dict(colors=color)
             mat_color_kwargs = dict(color_mode="vertex")
         elif len(color) == len(mesh.faces):
             obj_color_kwargs = dict(colors=color)
@@ -313,32 +344,48 @@
 
     # Make sure coordinates are c-contiguous
     if not points.flags["C_CONTIGUOUS"]:
         points = np.ascontiguousarray(points)
 
     geometry_kwargs = {}
     material_kwargs = {}
+    # material_kwargs["pick_write"] = True  # for picking
+
+    # Parse sizes
     if utils.is_iterable(size):
         if len(size) != len(points):
             raise ValueError(
                 "Expected `size` to be a single value or "
                 "an array of the same length as `points`."
             )
         geometry_kwargs["sizes"] = np.asarray(size).astype(np.float32, copy=False)
-        material_kwargs["size_mode"] = 'vertex'
+        material_kwargs["size_mode"] = "vertex"
     else:
         material_kwargs["size"] = size
 
+    # Parse color(s)
+    if isinstance(color, np.ndarray) and color.ndim == 2:
+        # If colors are provided for each node we have to make sure
+        # that we also include `None` for the breaks in the segments
+        n_points = len(points)
+        if len(color) != n_points:
+            raise ValueError(f"Got {len(color)} colors for {n_points} points.")
+        color = color.astype(np.float32, copy=False)
+        geometry_kwargs["colors"] = color
+        material_kwargs["color_mode"] = "vertex"
+    else:
+        if isinstance(color, np.ndarray):
+            color = color.astype(np.float32, copy=False)
+        material_kwargs["color"] = color
+
     if marker is None:
-        material = gfx.PointsMaterial(
-            color=color, size_space=size_space, **material_kwargs
-        )
+        material = gfx.PointsMaterial(size_space=size_space, **material_kwargs)
     else:
         material = gfx.PointsMarkerMaterial(
-            color=color, marker=marker, size_space=size_space, **material_kwargs
+            marker=marker, size_space=size_space, **material_kwargs
         )
 
     vis = gfx.Points(gfx.Geometry(positions=points, **geometry_kwargs), material)
 
     # Add custom attributes
     vis._object_type = "points"
     vis._object_id = uuid.uuid4()
@@ -421,16 +468,16 @@
         # If colors are provided for each node we have to make sure
         # that we also include `None` for the breaks in the segments
         n_points = (~np.isnan(lines[:, 0])).sum()
         if n_points != len(lines):
             # See if we can rescue this
             if len(color) == n_points:
                 breaks = np.where(np.isnan(lines[:, 0]))[0]
-                for b in breaks:
-                    color = np.insert(color, b, np.nan, axis=0)
+                offset = np.arange(len(breaks))
+                color = np.insert(color, breaks - offset, np.nan, axis=0)
             else:
                 raise ValueError(f"Got {len(color)} colors for {n_points} points.")
         color = color.astype(np.float32, copy=False)
         geometry_kwargs["colors"] = color
         material_kwargs["color_mode"] = "vertex"
     else:
         if isinstance(color, np.ndarray):
@@ -585,7 +632,72 @@
             gfx_geometries[geometry_name].material,
         )
         vis.local.matrix = transform
 
         visuals.append(vis)
 
     return visuals
+
+
+def text2gfx(
+    text,
+    position=(0, 0, 0),
+    color="w",
+    font_size=1,
+    anchor="topright",
+    screen_space=False,
+    markdown=False,
+):
+    """Convert text to pygfx visuals.
+
+    Parameters
+    ----------
+    text :          str
+                    Text to plot.
+    position :      tuple
+                    Position of the text.
+    color :         tuple | str
+                    Color to use for plotting.
+    font_size :     int, optional
+                    Font size.
+    anchor :        str, optional
+                    Anchor point of the text. Can be one of "topleft", "topright",
+                    "bottomleft", "bottomright", "center", "topmiddle", "bottommiddle", "middleleft",
+                    "middleright".
+    screen_space :  bool, optional
+                    Whether to use screen space coordinates.
+    markdown :      bool, optional
+                    Whether the text should be interpreted as markdown.
+
+    Returns
+    -------
+    text :          gfx.Text
+                    Pygfx visual for text.
+
+    """
+    assert isinstance(text, str), "Expected string."
+    assert isinstance(position, (list, tuple, np.ndarray)), "Expected list or tuple."
+    assert len(position) == 3, "Expected (x, y, z) position."
+
+    defaults = {
+        "font_size": font_size,
+        "anchor": anchor,
+        "screen_space": screen_space,
+    }
+    if markdown:
+        defaults["markdown"] = text
+    else:
+        defaults["text"] = text
+
+    text = gfx.Text(
+        gfx.TextGeometry(**defaults),
+        gfx.TextMaterial(color=color),
+    )
+    text.local.position = position
+    return text
+
+
+def visual_passthrough(x, *args, **kwargs):
+    """Pass-through converter."""
+    if any(args) or any(kwargs):
+        logger.info("Pygfx visuals are passed-through as is. Any additional arguments are ignored.")
+    return x
```

### Comparing `octarine3d-0.1.3/octarine3d.egg-info/PKG-INFO` & `octarine3d-0.1.4/octarine3d.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octarine3d
-Version: 0.1.3
+Version: 0.1.4
 Summary: WGPU-based 3d viewer
 Home-page: https://github.com/schlegelp/octarine
 Author: Philipp Schlegel
 Author-email: pms70@cam.ac.uk
 License: BSD-2-Clause
 Project-URL: Documentation, https://schlegelp.github.io/octarine/
 Project-URL: Source, https://github.com/schlegelp/octarine
@@ -36,14 +36,16 @@
 Requires-Dist: mkdocs-material[imaging]; extra == "docs"
 Requires-Dist: mkdocstrings-python; extra == "docs"
 Requires-Dist: mkdocs-minify-plugin; extra == "docs"
 Requires-Dist: mkdocs-literate-nav; extra == "docs"
 Requires-Dist: mkdocs-gen-files; extra == "docs"
 Requires-Dist: mkdocs-glightbox; extra == "docs"
 Requires-Dist: mkdocs-section-index; extra == "docs"
+Requires-Dist: trimesh; extra == "docs"
+Requires-Dist: importlib-metadata; extra == "docs"
 
 ![octarine banner](https://schlegelp.github.io/octarine/_static/octarine_logo_banner.png)
 <p align="center">
 <i>
 Octarine is the eighth color of the Discworld's spectrum, which is described as the color of magic itself. Only wizards and cats can see it.
 </i>
 </p>
@@ -97,14 +99,19 @@
 m = gfx.geometries.mobius_strip_geometry()
 v.add(m, color='b')
 
 # Close the viewer
 v.close()
 ```
 
+> [!NOTE]
+> The above example will work in interactive environments such as IPython and Jupyter. When using from the standard
+> REPL or when running as a script you will have to additionally start the event loop. Please see corresponding the
+> section in the [Introduction](https://schlegelp.github.io/octarine/intro/).
+
 ![demo gif](docs/_static/octarine_demo_720p.gif)
 
 ## Want to learn more?
 Head over to the [**Documentation**](https://schlegelp.github.io/octarine/)!
 
 ## Want to contribute?
 We welcome all kinds of contributions. For example:
```

### Comparing `octarine3d-0.1.3/setup.py` & `octarine3d-0.1.4/setup.py`

 * *Files identical despite different names*

