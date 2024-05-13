# Comparing `tmp/tikzplotly-0.1.3.tar.gz` & `tmp/tikzplotly-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tikzplotly-0.1.3.tar", last modified: Sun Mar  3 09:06:05 2024, max compression
+gzip compressed data, was "tikzplotly-0.1.4.tar", last modified: Mon May 13 07:19:33 2024, max compression
```

## Comparing `tikzplotly-0.1.3.tar` & `tikzplotly-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 09:06:05.490970 tikzplotly-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-03 09:05:56.000000 tikzplotly-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-03-03 09:06:05.490970 tikzplotly-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-03-03 09:05:56.000000 tikzplotly-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-03-03 09:05:56.000000 tikzplotly-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-03 09:06:05.490970 tikzplotly-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 09:06:05.486971 tikzplotly-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 09:06:05.490970 tikzplotly-0.1.3/src/tikzplotly/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-03 09:05:56.000000 tikzplotly-0.1.3/src/tikzplotly/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-03 09:05:56.000000 tikzplotly-0.1.3/src/tikzplotly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-03-03 09:05:56.000000 tikzplotly-0.1.3/src/tikzplotly/_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-03-03 09:05:56.000000 tikzplotly-0.1.3/src/tikzplotly/_axis.py
--rw-r--r--   0 runner    (1001) docker     (127)    38503 2024-03-03 09:05:56.000000 tikzplotly-0.1.3/src/tikzplotly/_color.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-03 09:05:56.000000 tikzplotly-0.1.3/src/tikzplotly/_dash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-03 09:05:56.000000 tikzplotly-0.1.3/src/tikzplotly/_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-03-03 09:05:56.000000 tikzplotly-0.1.3/src/tikzplotly/_dataContainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-03-03 09:05:56.000000 tikzplotly-0.1.3/src/tikzplotly/_marker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-03-03 09:05:56.000000 tikzplotly-0.1.3/src/tikzplotly/_save.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-03-03 09:05:56.000000 tikzplotly-0.1.3/src/tikzplotly/_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-03-03 09:05:56.000000 tikzplotly-0.1.3/src/tikzplotly/_tex.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-03-03 09:05:56.000000 tikzplotly-0.1.3/src/tikzplotly/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 09:06:05.490970 tikzplotly-0.1.3/src/tikzplotly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-03-03 09:06:05.000000 tikzplotly-0.1.3/src/tikzplotly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-03 09:06:05.000000 tikzplotly-0.1.3/src/tikzplotly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 09:06:05.000000 tikzplotly-0.1.3/src/tikzplotly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-03 09:06:05.000000 tikzplotly-0.1.3/src/tikzplotly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-03 09:06:05.000000 tikzplotly-0.1.3/src/tikzplotly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 09:06:05.490970 tikzplotly-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    14231 2024-03-03 09:05:56.000000 tikzplotly-0.1.3/tests/test_line_charts.py
--rw-r--r--   0 runner    (1001) docker     (127)    11509 2024-03-03 09:05:56.000000 tikzplotly-0.1.3/tests/test_markers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:19:33.438336 tikzplotly-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-13 07:19:29.000000 tikzplotly-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-05-13 07:19:33.438336 tikzplotly-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-13 07:19:29.000000 tikzplotly-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-13 07:19:29.000000 tikzplotly-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 07:19:33.438336 tikzplotly-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:19:33.434337 tikzplotly-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:19:33.434337 tikzplotly-0.1.4/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-05-13 07:19:29.000000 tikzplotly-0.1.4/src/tests/test_heatmaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14231 2024-05-13 07:19:29.000000 tikzplotly-0.1.4/src/tests/test_line_charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11509 2024-05-13 07:19:29.000000 tikzplotly-0.1.4/src/tests/test_markers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:19:33.438336 tikzplotly-0.1.4/src/tikzplotly/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       21 2024-05-13 07:19:29.000000 tikzplotly-0.1.4/src/tikzplotly/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-13 07:19:29.000000 tikzplotly-0.1.4/src/tikzplotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-13 07:19:29.000000 tikzplotly-0.1.4/src/tikzplotly/_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-13 07:19:29.000000 tikzplotly-0.1.4/src/tikzplotly/_axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39173 2024-05-13 07:19:29.000000 tikzplotly-0.1.4/src/tikzplotly/_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-13 07:19:29.000000 tikzplotly-0.1.4/src/tikzplotly/_dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-13 07:19:29.000000 tikzplotly-0.1.4/src/tikzplotly/_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-13 07:19:29.000000 tikzplotly-0.1.4/src/tikzplotly/_dataContainer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4801 2024-05-13 07:19:29.000000 tikzplotly-0.1.4/src/tikzplotly/_heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-13 07:19:29.000000 tikzplotly-0.1.4/src/tikzplotly/_marker.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3919 2024-05-13 07:19:29.000000 tikzplotly-0.1.4/src/tikzplotly/_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-13 07:19:29.000000 tikzplotly-0.1.4/src/tikzplotly/_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-13 07:19:29.000000 tikzplotly-0.1.4/src/tikzplotly/_tex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-13 07:19:29.000000 tikzplotly-0.1.4/src/tikzplotly/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:19:33.438336 tikzplotly-0.1.4/src/tikzplotly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-05-13 07:19:33.000000 tikzplotly-0.1.4/src/tikzplotly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-13 07:19:33.000000 tikzplotly-0.1.4/src/tikzplotly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 07:19:33.000000 tikzplotly-0.1.4/src/tikzplotly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-13 07:19:33.000000 tikzplotly-0.1.4/src/tikzplotly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-13 07:19:33.000000 tikzplotly-0.1.4/src/tikzplotly.egg-info/top_level.txt
```

### Comparing `tikzplotly-0.1.3/LICENSE` & `tikzplotly-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tikzplotly-0.1.3/PKG-INFO` & `tikzplotly-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tikzplotly
-Version: 0.1.3
+Version: 0.1.4
 Summary: Convert plotly figures to LaTeX / tikz figures
 Author-email: Thomas Saigre <tikzplotly@outlook.fr>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 @thomas-saigre
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,14 +38,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: plotly
+Requires-Dist: PIL
 Provides-Extra: dev
 Requires-Dist: pandas; extra == "dev"
 
 ![logo-tikzplotly](https://raw.githubusercontent.com/thomas-saigre/tikzplotly/main/doc/img/logo.svg "Tikzplotly")
 
 [![PyPi Version](https://img.shields.io/pypi/v/tikzplotly.svg?style=flat-square)](https://pypi.org/project/tikzplotly)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/tikzplotly.svg?style=flat-square)](https://pypi.org/pypi/tikzplotly/)
```

### Comparing `tikzplotly-0.1.3/README.md` & `tikzplotly-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `tikzplotly-0.1.3/pyproject.toml` & `tikzplotly-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tikzplotly"
-version = "0.1.3"
+version = "0.1.4"
 description = "Convert plotly figures to LaTeX / tikz figures"
 readme = "README.md"
 authors = [{name = "Thomas Saigre", email = "tikzplotly@outlook.fr"}]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
@@ -21,15 +21,16 @@
     "Operating System :: OS Independent",
     "Topic :: Multimedia :: Graphics :: Graphics Conversion",
     "Topic :: Scientific/Engineering :: Visualization",
 ]
 keywords = ["plotly", "latex", "tikz", "figure", "conversion", "graphics"]
 dependencies = [
     "numpy",
-    "plotly"
+    "plotly",
+    "PIL"
 ]
 
 [project.optional-dependencies]
 dev = ["pandas"]
 
 [project.urls]
 Code = "https://github.com/thomas-saigre/tikzplotly"
```

### Comparing `tikzplotly-0.1.3/src/tikzplotly/_annotations.py` & `tikzplotly-0.1.4/src/tikzplotly/_annotations.py`

 * *Files identical despite different names*

### Comparing `tikzplotly-0.1.3/src/tikzplotly/_axis.py` & `tikzplotly-0.1.4/src/tikzplotly/_axis.py`

 * *Files identical despite different names*

### Comparing `tikzplotly-0.1.3/src/tikzplotly/_color.py` & `tikzplotly-0.1.4/src/tikzplotly/_color.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,30 @@
     elif color.lower() in colors:
         return color.lower(), "RGB", colors[color.lower()], 1
 
     else:
         warn(f"Color {color} type is not supported yet. Returning the same color.")
         return color, 1
 
+def hex2rgb(hex_color):
+    """Convert a hex color to a RGB color.
+
+    Parameters
+    ----------
+    hex_color
+        hex color string
+
+    Returns
+    -------
+        RGB color string
+    """
+    hex_color = hex_color.lstrip("#")
+    return str(int(hex_color[:2], 16)) + ", " + str(int(hex_color[2:4], 16)) + ", " + str(int(hex_color[4:], 16))
+
+DEFAULT_COLORSCALE = ((0.0, '#0d0887'), (0.1111111111111111, '#46039f'), (0.2222222222222222, '#7201a8'), (0.3333333333333333, '#9c179e'), (0.4444444444444444, '#bd3786'), (0.5555555555555556, '#d8576b'), (0.6666666666666666, '#ed7953'), (0.7777777777777778, '#fb9f3a'), (0.8888888888888888, '#fdca26'), (1.0, '#f0f921'))
 
 
 ALICEBLUE = rgb_str(240, 248, 255)
 ANTIQUEWHITE = rgb_str(250, 235, 215)
 ANTIQUEWHITE1 = rgb_str(255, 239, 219)
 ANTIQUEWHITE2 = rgb_str(238, 223, 204)
 ANTIQUEWHITE3 = rgb_str(205, 192, 176)
```

### Comparing `tikzplotly-0.1.3/src/tikzplotly/_data.py` & `tikzplotly-0.1.4/src/tikzplotly/_data.py`

 * *Files identical despite different names*

### Comparing `tikzplotly-0.1.3/src/tikzplotly/_dataContainer.py` & `tikzplotly-0.1.4/src/tikzplotly/_dataContainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,16 @@
             name of the y data, by default None
 
         Returns
         -------
             tuple (macro_name, y_label), where macro_name is the name of the data in LaTeX and y_label the name of the y data in LaTeX
         """
         for data in self.data:
+            if len(data.x) != len(x):
+                continue
             are_equals = data.x == x
             if type(are_equals) == bool:
                 if are_equals:
                     y_label = data.addYData(y, y_label)
                     return data.macro_name, y_label
             elif are_equals.all():
                 if (data.x == x).all():
```

### Comparing `tikzplotly-0.1.3/src/tikzplotly/_marker.py` & `tikzplotly-0.1.4/src/tikzplotly/_marker.py`

 * *Files identical despite different names*

### Comparing `tikzplotly-0.1.3/src/tikzplotly/_save.py` & `tikzplotly-0.1.4/src/tikzplotly/_save.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 from pathlib import Path
 from .__about__ import __version__
 from ._tex import *
 from ._scatter import draw_scatter2d
+from ._heatmap import draw_heatmap
 from ._axis import Axis
 from ._color import *
 from ._annotations import str_from_annotation
 from ._dataContainer import DataContainer
 from ._utils import sanitize_TeX_text
 from warnings import warn
 import re
 
 def get_tikz_code(
         fig,
         tikz_options = None,
         axis_options = None,
         include_disclamer = True,
+        img_name = "heatmap.png",
     ):
     """Get the tikz code of a figure.
 
     Parameters
     ----------
     fig
         Plotly figure
     tikz_options, optional
         options given to the tikzpicture environment, by default None
     axis_options, optional
         options given to the axis environment, by default None
     include_disclamer, optional
         include a disclamer in the code, by default True
+    img_name, optional
+        name of the PNG file for heatmap, by default "heatmap.png"
 
     Returns
     -------
         string of tikz code
     """
     figure_data = fig.data
     figure_layout = fig.layout
@@ -55,14 +59,18 @@
             data_str.append( draw_scatter2d(data_name_macro, trace, y_name, axis, colors_set) )
             if trace.name and trace['showlegend'] != False:
                 data_str.append( tex_add_legendentry(sanitize_TeX_text(trace.name)) )
             if trace.line.color is not None:
                 colors_set.add(convert_color(trace.line.color)[:3])
             if trace.fillcolor is not None:
                 colors_set.add(convert_color(trace.fillcolor)[:3])
+
+        elif trace.type == "heatmap":
+            data_str.append( draw_heatmap(trace, fig, img_name, axis) )
+
         else:
             warn(f"Trace type {trace.type} is not supported yet.")
 
     annotation_str = str_from_annotation(figure_layout.annotations, axis, colors_set)
 
     code = """"""
     stack_env = []
@@ -106,9 +114,12 @@
     ----------
     filepath : str or Path
         A string containing a path to a filename, or a Path object.
     *args, **kwargs
         Additional arguments are passed to the backend.
     """
     code = get_tikz_code(*args, **kwargs)
+    directory = Path(filepath).parent
+    if not directory.exists():
+        directory.mkdir(parents=True)
     with open(filepath, "w") as fd:
         fd.write(code)
```

### Comparing `tikzplotly-0.1.3/src/tikzplotly/_scatter.py` & `tikzplotly-0.1.4/src/tikzplotly/_scatter.py`

 * *Files identical despite different names*

### Comparing `tikzplotly-0.1.3/src/tikzplotly/_tex.py` & `tikzplotly-0.1.4/src/tikzplotly/_tex.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from ._color import hex2rgb
 
 def tex_comment(text):
     """Create a LaTeX comment.
 
     Parameters
     ----------
     text :
@@ -186,8 +187,17 @@
     return code
 
 
 def tex_text(text):
     """Convert a string to LaTeX,
     escaping the special characters %, _, &, #, $, {, }, ~.
     """
-    return text.replace("%", "\\%").replace("_", "\\_").replace("&", "\\&").replace("#", "\\#").replace("$", "\\$").replace("{", "\\{").replace("}", "\\}").replace("~", "\\textasciitilde ")
+    return text.replace("%", "\\%").replace("_", "\\_").replace("&", "\\&").replace("#", "\\#").replace("$", "\\$").replace("{", "\\{").replace("}", "\\}").replace("~", "\\textasciitilde ")
+
+def get_tikz_colorscale(colorscale, name="mycolor"):
+
+    code = "{" + str(name) + "}{\n"
+    for dist, color in colorscale:
+        rgb_color = hex2rgb(color)
+        code += f"  rgb255({dist}cm)=({rgb_color})".replace(" ", "") + ";\n"
+    code += "}"
+    return code
```

### Comparing `tikzplotly-0.1.3/src/tikzplotly/_utils.py` & `tikzplotly-0.1.4/src/tikzplotly/_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
 import warnings
 from math import floor
+import numpy as np
 
 rep_digit = {'0': 'Z', '1': 'O', '2': 'T', '3': 'Th', '4': 'F', '5': 'Fi', '6': 'S', '7': 'Se', '8': 'E', '9': 'N'}
 rep_digit = dict((re.escape(k), v) for k, v in rep_digit.items())
 pattern_digit = re.compile("|".join(rep_digit.keys()))
 
 def replace_all_digits(text):
     """Replace all digits in a string with their corresponding letter.
@@ -106,8 +107,26 @@
     for key, value in options_dict.items():
         if value is None:
             options += f"{key},{sep}"
         else:
             options += f"{key}={value},{sep}"
     if options == "":
         return None
-    return options.strip()[:-1]
+    return options.strip()[:-1]
+
+def get_ticks_str(data, nticks):
+    indices = np.arange(len(data))
+    if nticks is not None:
+        data_ = data[::len(data)//(nticks-1)]
+        data = np.append(data_, [data[-1]])
+        indices_ = indices[::len(indices)//(nticks-1)]
+        indices = np.append(indices_, [indices[-1]])
+
+    ticks = "{"
+    ticklabels = "{"
+    for i, val in zip(indices, data):
+        ticks += str(i) + ","
+        ticklabels += str(val) + ","
+    ticks = ticks[:-1] + "}"
+    ticklabels = ticklabels[:-1] + "}"
+
+    return ticks, ticklabels
```

### Comparing `tikzplotly-0.1.3/src/tikzplotly.egg-info/PKG-INFO` & `tikzplotly-0.1.4/src/tikzplotly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tikzplotly
-Version: 0.1.3
+Version: 0.1.4
 Summary: Convert plotly figures to LaTeX / tikz figures
 Author-email: Thomas Saigre <tikzplotly@outlook.fr>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 @thomas-saigre
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,14 +38,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: plotly
+Requires-Dist: PIL
 Provides-Extra: dev
 Requires-Dist: pandas; extra == "dev"
 
 ![logo-tikzplotly](https://raw.githubusercontent.com/thomas-saigre/tikzplotly/main/doc/img/logo.svg "Tikzplotly")
 
 [![PyPi Version](https://img.shields.io/pypi/v/tikzplotly.svg?style=flat-square)](https://pypi.org/project/tikzplotly)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/tikzplotly.svg?style=flat-square)](https://pypi.org/pypi/tikzplotly/)
```

### Comparing `tikzplotly-0.1.3/src/tikzplotly.egg-info/SOURCES.txt` & `tikzplotly-0.1.4/src/tikzplotly.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 LICENSE
 README.md
 pyproject.toml
+src/tests/test_heatmaps.py
+src/tests/test_line_charts.py
+src/tests/test_markers.py
 src/tikzplotly/__about__.py
 src/tikzplotly/__init__.py
 src/tikzplotly/_annotations.py
 src/tikzplotly/_axis.py
 src/tikzplotly/_color.py
 src/tikzplotly/_dash.py
 src/tikzplotly/_data.py
 src/tikzplotly/_dataContainer.py
+src/tikzplotly/_heatmap.py
 src/tikzplotly/_marker.py
 src/tikzplotly/_save.py
 src/tikzplotly/_scatter.py
 src/tikzplotly/_tex.py
 src/tikzplotly/_utils.py
 src/tikzplotly.egg-info/PKG-INFO
 src/tikzplotly.egg-info/SOURCES.txt
 src/tikzplotly.egg-info/dependency_links.txt
 src/tikzplotly.egg-info/requires.txt
-src/tikzplotly.egg-info/top_level.txt
-tests/test_line_charts.py
-tests/test_markers.py
+src/tikzplotly.egg-info/top_level.txt
```

### Comparing `tikzplotly-0.1.3/tests/test_line_charts.py` & `tikzplotly-0.1.4/src/tests/test_line_charts.py`

 * *Files identical despite different names*

### Comparing `tikzplotly-0.1.3/tests/test_markers.py` & `tikzplotly-0.1.4/src/tests/test_markers.py`

 * *Files identical despite different names*

