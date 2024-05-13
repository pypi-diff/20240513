# Comparing `tmp/cosmoplots-0.4.1.tar.gz` & `tmp/cosmoplots-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmoplots-0.4.1.tar", max compression
+gzip compressed data, was "cosmoplots-0.4.2.tar", max compression
```

## Comparing `cosmoplots-0.4.1.tar` & `cosmoplots-0.4.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1076 2024-04-29 12:58:09.470967 cosmoplots-0.4.1/LICENSE
--rw-r--r--   0        0        0     5994 2024-04-29 12:58:09.470967 cosmoplots-0.4.1/README.md
--rw-r--r--   0        0        0      167 2024-04-29 12:58:09.474967 cosmoplots-0.4.1/cosmoplots/__init__.py
--rw-r--r--   0        0        0     4014 2024-04-29 12:58:09.474967 cosmoplots-0.4.1/cosmoplots/axes.py
--rw-r--r--   0        0        0     2723 2024-04-29 12:58:09.474967 cosmoplots-0.4.1/cosmoplots/colors.py
--rw-r--r--   0        0        0    10355 2024-04-29 12:58:09.474967 cosmoplots-0.4.1/cosmoplots/concat.py
--rw-r--r--   0        0        0     1150 2024-04-29 12:58:09.474967 cosmoplots-0.4.1/cosmoplots/default.mplstyle
--rw-r--r--   0        0        0     5516 2024-04-29 12:58:09.474967 cosmoplots-0.4.1/cosmoplots/figure_defs.py
--rw-r--r--   0        0        0       37 2024-04-29 12:58:09.474967 cosmoplots-0.4.1/cosmoplots/thick_line.mplstyle
--rw-r--r--   0        0        0      251 2024-04-29 12:58:09.474967 cosmoplots-0.4.1/cosmoplots/two_columns.mplstyle
--rw-r--r--   0        0        0      577 2024-04-29 12:58:22.539075 cosmoplots-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     6809 1970-01-01 00:00:00.000000 cosmoplots-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-13 06:56:19.289572 cosmoplots-0.4.2/LICENSE
+-rw-r--r--   0        0        0     5971 2024-05-13 06:56:19.289572 cosmoplots-0.4.2/README.md
+-rw-r--r--   0        0        0      167 2024-05-13 06:56:19.293572 cosmoplots-0.4.2/cosmoplots/__init__.py
+-rw-r--r--   0        0        0     4726 2024-05-13 06:56:19.293572 cosmoplots-0.4.2/cosmoplots/axes.py
+-rw-r--r--   0        0        0     2723 2024-05-13 06:56:19.293572 cosmoplots-0.4.2/cosmoplots/colors.py
+-rw-r--r--   0        0        0    11852 2024-05-13 06:56:19.293572 cosmoplots-0.4.2/cosmoplots/concat.py
+-rw-r--r--   0        0        0     1150 2024-05-13 06:56:19.293572 cosmoplots-0.4.2/cosmoplots/default.mplstyle
+-rw-r--r--   0        0        0     5516 2024-05-13 06:56:19.293572 cosmoplots-0.4.2/cosmoplots/figure_defs.py
+-rw-r--r--   0        0        0       37 2024-05-13 06:56:19.293572 cosmoplots-0.4.2/cosmoplots/thick_line.mplstyle
+-rw-r--r--   0        0        0      251 2024-05-13 06:56:19.293572 cosmoplots-0.4.2/cosmoplots/two_columns.mplstyle
+-rw-r--r--   0        0        0      577 2024-05-13 06:56:34.621733 cosmoplots-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     6786 1970-01-01 00:00:00.000000 cosmoplots-0.4.2/PKG-INFO
```

### Comparing `cosmoplots-0.4.1/LICENSE` & `cosmoplots-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmoplots-0.4.1/README.md` & `cosmoplots-0.4.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,31 +20,30 @@
 ```
 
 ## Usage
 
 Set your `rcparams` before plotting in your code, for example:
 
 ```python
+import matplotlib.pyplot as plt
 import cosmoplots
-import matplotlib as mpl
-
 # If you only want the default style
-mpl.style.use("cosmoplots.default")
+plt.style.use(["cosmoplots.default"])
 ```
 
 ### Muliple subfigures
-To make a figure with multiple rows or columns, use `cosmoplots.figure_multiple_rows_columns`:
+To make a figure with multiple rows or columns, use `cosmoplots.figure_multiple_rows_columns`.
+By default, the labels are $\mathrm{(a)}$, $\mathrm{(b)}$, $\mathrm{(c)}$, ..., but they may be replaced using the `labels` argument.
 ```python
-import matplotlib as mpl
 import matplotlib.pyplot as plt
-import numpy as np
-
 import cosmoplots
+plt.style.use(["cosmoplots.default"])
+
+import numpy as np
 
-mpl.style.use(["cosmoplots.default"])
 rows = 1
 columns = 2
 
 fig, ax = cosmoplots.figure_multiple_rows_columns(rows, columns)
 a = np.linspace(-3,3,100)
 for i in range(rows*columns):
     ax[i].set_xlabel("X Axis")
@@ -54,20 +53,18 @@
 ```
 ![multifig](./assets/multifig.png)
 
 ## `change_log_axis_base`
 
 ```python
 import matplotlib.pyplot as plt
-import numpy as np
 import cosmoplots
-import matplotlib as mpl
+plt.style.use(["cosmoplots.default"])
+import numpy as np
 
-# Setup
-mpl.style.use("cosmoplots.default")
 a = np.exp(np.linspace(-3, 1, 100))
 
 # Plotting
 fig = plt.figure()
 ax1 = plt.gca()
 ax1.set_xlabel("X Axis")
 ax1.set_ylabel("Y Axis")
@@ -92,35 +89,34 @@
 ax2.plot(a)
 plt.show()
 ```
 
 ## `matplotlib` vs. `cosmoplots` defaults
 
 ```python
-import cosmoplots
-import matplotlib as mpl
 import matplotlib.pyplot as plt
+import cosmoplots
 import numpy as np
 
 def plot() -> None:
     a = np.exp(np.linspace(-3, 5, 100))
     fig = plt.figure()
     ax = fig.add_subplot()
     ax.set_xlabel("X Axis")
     ax.set_ylabel("Y Axis")
     ax.semilogy(a)
 
 # Matplotlib ------------------------------------------------------------------------- #
-with mpl.style.context("default"):
+with plt.style.context("default"):
     plot()
     # plt.savefig("assets/matplotlib.png")
     plt.show()
 
 # Cosmoplots ------------------------------------------------------------------------- #
-with mpl.style.context("cosmoplots.default"):
+with plt.style.context("cosmoplots.default"):
     plot()
     # plt.savefig("assets/cosmoplots.png")
     plt.show()
 ```
 
 | `matplotlib` | `cosmoplots` |
 | :--------: | :--------: |
@@ -133,26 +129,25 @@
 ## `generate_hex_colors`
 
 This function generates the hex numbers for the colours extracted from a `matplotlib` colour map based on the number of points of interest.
 The colors change gradually from bright to dark or vice versa.
 ```python
 import matplotlib.pyplot as plt
 import cosmoplots
-
-axes_size = cosmoplots.set_rcparams_dynamo(plt.rcParams, num_cols=1, ls="thin")
+plt.style.use(["cosmoplots.default"])
 
 
 color_list = cosmoplots.generate_hex_colors(5, 'viridis', show_swatch=True, ascending=True)
 plt.savefig("./assets/hex_colors.png")
 
 # Print color_list to retrieve the hex numbers
 print(color_list) #['#fde725', '#5ec962', '#21918c', '#3b528b', '#440154']
 
 fig = plt.figure()
-ax = fig.add_axes(axes_size)
+ax = plt.gca()
 for i, color in enumerate(color_list):
     ax.plot([1,2],[i,i+1], c = color)
 
 plt.savefig("./assets/hex_colors_example.png")
 plt.show()
 ```
 | `hex_colors.png` | hex_colors_example.png |
@@ -170,21 +165,18 @@
 conveniently available from the `combine` function in `cosmoplots`.
 
 An example is shown below. Also see the [`tests`](./tests/) directory for more examples.
 A `help` method that prints the `imagemagick` commands that are used under the hood is
 also available.
 
 ```python
-import matplotlib as mpl
 import matplotlib.pyplot as plt
-import numpy as np
-
 import cosmoplots
-
-mpl.style.use("cosmoplots.default")
+plt.style.use("cosmoplots.default")
+import numpy as np
 
 
 def plot(i) -> None:
     """Create a simple plot."""
     a = np.exp(np.linspace(-3, 5, 100))
     fig = plt.figure()
     ax = fig.add_subplot()
```

### Comparing `cosmoplots-0.4.1/cosmoplots/axes.py` & `cosmoplots-0.4.2/cosmoplots/axes.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """Module for modifying the axis properties of plots."""
 
 from typing import List, Tuple, Union
-import matplotlib as mpl
+from matplotlib.axes import Axes
+from matplotlib.figure import Figure
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib import ticker
 
 
 def _convert_scale_name(scale: str, axis: str) -> str:
     """Convert the scale name to a more readable format."""
     # All possible scale names:
     # ['asinh', 'function', 'functionlog', 'linear', 'log', 'logit', 'mercator', 'symlog']
     return f"{axis}axis" if scale == "log" else "none"
 
 
-def _check_axes_scales(axes: plt.Axes) -> Tuple[List[str], str]:
+def _check_axes_scales(axes: Axes) -> Tuple[List[str], str]:
     xscale, yscale = axes.get_xscale(), axes.get_yscale()
     xs, ys = _convert_scale_name(xscale, "x"), _convert_scale_name(yscale, "y")
     if xs == "xaxis" and ys == "yaxis":
         scales = [xs, ys]
         pltype = "loglog"
     elif xs == "xaxis":
         scales = [xs]
@@ -29,16 +30,16 @@
     else:
         scales = []
         pltype = "linear"
     return scales, pltype
 
 
 def change_log_axis_base(
-    axes: plt.Axes, which: Union[str, None] = None, base: float = 10
-) -> plt.Axes:
+    axes: Axes, which: Union[str, None] = None, base: float = 10
+) -> Axes:
     """Change the tick formatter to not use powers 0 and 1 in logarithmic plots.
 
     Change the logarithmic axis `10^0 -> 1` and `10^1 -> 10` (or the given base), i.e.
     without power, otherwise use the base to some power. For more robust and less error
     prone results, the plotting type is also re-set with the same base ('loglog',
     'semilogx' and 'semilogy').
 
@@ -86,37 +87,47 @@
                     + "{:g}".format(np.log(x) / np.log(base))
                     + r"}$"
                 )
             )
         )
     return axes
 
-def figure_multiple_rows_columns(rows: int, columns: int):
+def figure_multiple_rows_columns(rows: int, columns: int, 
+                                 labels: Union[List[str], None] = None,
+                                 label_x: float = -0.2, label_y: float = 0.95,
+                                 **kwargs) -> Tuple[Figure, List[Axes]]:
     """Returns a figure with axes which is appropriate for (rows, columns) subfigures.
 
     Parameters
     ----------
     rows : int
         The number of rows in the figure
     columns : int
         The number of columns in the figure
-
+    labels : List[str] | None
+        The labels to be applied to each subfigure. Defaults to (a), (b), (c), ...
+    label_x and label_y: float
+        x- and y- positions of the labels relative to each Axes object.
+    **kwargs:
+        Additional keyword arguments to be passed to Axes.text. 
+        
     Returns
     -------
     plt.Figure
         The figure object
-    plt.Axes
+    List[plt.Axes]
         A list of all the axes objects owned by the figure
     """
     fig = plt.figure(figsize = (columns*3.37, rows*2.08277))
-    axes = [None]*rows*columns
+    axes = []
+    labels = labels or [r"$\mathrm{{({})}}$".format(chr(97+l)) for l in range(rows*columns)] 
     for c in range(columns):
         for r in range(rows):
-            index = r*columns + c
             left = (0.2)/columns + c/columns
             bottom = (0.2)/rows + (rows-1-r)/rows # Start at the top
             width = 0.75/columns
             height = 0.75/rows
-            axes[index]  = fig.add_axes([left, bottom, width, height])
+            axes.append(fig.add_axes((left, bottom, width, height)))
+            axes[-1].text(label_x, label_y, labels[columns*r+c], transform=axes[-1].transAxes, **kwargs)
 
     return fig, axes
```

### Comparing `cosmoplots-0.4.1/cosmoplots/colors.py` & `cosmoplots-0.4.2/cosmoplots/colors.py`

 * *Files identical despite different names*

### Comparing `cosmoplots-0.4.1/cosmoplots/concat.py` & `cosmoplots-0.4.2/cosmoplots/concat.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,55 @@
 """Combine images in a subfigure layout."""
 
 # `Self` was introduced in 3.11, but returning the class type works from 3.7 onwards.
 from __future__ import annotations
-import warnings
 
+import logging
 import pathlib
 import subprocess
 import tempfile
+import warnings
+from contextlib import contextmanager
+
+import matplotlib.pyplot as plt
+from matplotlib.font_manager import FontProperties, findfont
+
+
+@contextmanager
+def _ignore_logging_context():
+    loggers = [logging.getLogger(name) for name in logging.root.manager.loggerDict]
+    # turn loggers off
+    for logger in loggers:
+        logger.disabled = True
+    logging.root.disabled = True
+    yield
+    # turn loggers back on
+    for logger in loggers:
+        logger.disabled = False
+    logging.root.disabled = False
 
 
 class Combine:
     """Combine images into a subfigure layout."""
 
     def __init__(self) -> None:
         self._gravity = "northwest"
-        self._fontsize = 100
         self._pos = (10.0, 10.0)
-        self._font = "Times-New-Roman"
+        with _ignore_logging_context():
+            font = findfont(FontProperties(family=plt.rcParams["font.serif"]))
+        self._font = font
+        self._fontsize = int(plt.rcParams["font.size"])
         self._color = "black"
         self._ft: str = ".png"
         self._output = pathlib.Path(f"output{self._ft}")
+        self._dpi = (
+            plt.rcParams["savefig.dpi"]
+            if isinstance(plt.rcParams["savefig.dpi"], float)
+            else plt.rcParams["figure.dpi"]
+        )
         self._files: list[pathlib.Path] = []
         self._labels: list[str] = []
         self._w: int | None = None
         self._h: int | None = None
 
     def combine(self, *files: str | pathlib.Path) -> Combine:
         """Give all files that should be combined.
@@ -39,44 +65,48 @@
                 self._files.append(current_file)
             else:
                 raise FileNotFoundError(f"The input file {current_file} was not found.")
         return self
 
     def using(
         self,
-        gravity: str = "northwest",
-        pos: tuple[float, float] = (10.0, 10.0),
-        font: str = "Times-New-Roman",
-        fontsize: int = 100,
-        color: str = "black",
+        *,
+        gravity: str | None = None,
+        pos: tuple[float, float] | None = None,
+        font: str | None = None,
+        fontsize: int | None = None,
+        color: str | None = None,
     ) -> Combine:
         """Set text properties.
 
+        The properties must be given as keyword arguments to take effect.
+
         Parameters
         ----------
-        gravity : str
+        gravity : str, optional
             Where the position of the text is relative to in the subfigure. Default is
             `northwest`. Possible values are `north`, `northeast`, `northwest`, `south`,
             `southeast`, `southwest`, `west`, `east` and `center`.
-        pos : tuple[float, float]
+        pos : tuple[float, float], optional
             The position in the subfigure relative to `gravity`. Default is `(10.0,
             10.0)`.
-        font : str
+        font : str, optional
             The type of font to use, default is Times New Roman. See `convert -list
             font` for a list of available fonts.
-        fontsize : int
-            The size of the font in pointsize. Default is `100`.
-        color : str
+        fontsize : int, optional
+            The size of the font in pointsize. Default is to use the "font.size" field
+            in the matplotlib rcParams.
+        color : str, optional
             The color of the text. Default is `black`.
         """
-        self._gravity = gravity
-        self._fontsize = fontsize
-        self._pos = pos
-        self._font = font
-        self._color = color
+        self._gravity = gravity or self._gravity
+        self._fontsize = fontsize or self._fontsize
+        self._pos = pos or self._pos
+        self._font = font or self._font
+        self._color = color or self._color
         return self
 
     def in_grid(self, w: int, h: int) -> Combine:
         """Specify the grid layout.
 
         Parameters
         ----------
@@ -125,22 +155,28 @@
             if quotient > 0:
                 current_char = alphabet[quotient - 1] + current_char
 
             characters.append(f"({current_char})")
             count += 1
         return characters
 
-    def save(self, output: pathlib.Path | str | None = None) -> None:
+    def save(
+        self, output: pathlib.Path | str | None = None, dpi: float | int | None = None
+    ) -> None:
         """Save the combined images as a png file.
 
         Parameters
         ----------
         output : pathlib.Path | str, optional
             Give the name of the output file, default is `output.png`.
+        dpi : float | int, optional
+            The resolution that the input files were saved with. Default is the same as
+            the matplotlib savefig dpi.
         """
+        self._dpi = dpi or self._dpi
         self._check_params_before_save(output)
         self._check_cli_available()
         self._run_subprocess()
 
     def _check_params_before_save(
         self, output: pathlib.Path | str | None = None, ft: str | None = None
     ) -> None:
@@ -191,15 +227,19 @@
         idx = list(range(len(self._files)))
         tmp_path = pathlib.Path(tmp_dir.name)
         for i, file, label in zip(idx, self._files, self._labels):
             # Add label to images
             subprocess.call(
                 [
                     "convert",
+                    "-units",
+                    "PixelsPerInch",
                     file,
+                    "-density",
+                    str(self._dpi),
                     "-font",
                     self._font,
                     "-pointsize",
                     str(self._fontsize),
                     "-draw",
                     (
                         f"gravity {self._gravity} fill {self._color} text"
```

### Comparing `cosmoplots-0.4.1/cosmoplots/default.mplstyle` & `cosmoplots-0.4.2/cosmoplots/default.mplstyle`

 * *Files identical despite different names*

### Comparing `cosmoplots-0.4.1/cosmoplots/figure_defs.py` & `cosmoplots-0.4.2/cosmoplots/figure_defs.py`

 * *Files identical despite different names*

### Comparing `cosmoplots-0.4.1/pyproject.toml` & `cosmoplots-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cosmoplots"
-version = "0.4.1"
+version = "0.4.2"
 description = "Routines to get a sane default configuration for production quality plots."
 homepage = "https://github.com/uit-cosmo/cosmoplots"
 authors = ["gregordecristoforo <gregor.decristoforo@gmail.com>"]
 license = "MIT License"
 readme = 'README.md'
 
 [tool.poetry.dependencies]
```

### Comparing `cosmoplots-0.4.1/PKG-INFO` & `cosmoplots-0.4.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosmoplots
-Version: 0.4.1
+Version: 0.4.2
 Summary: Routines to get a sane default configuration for production quality plots.
 Home-page: https://github.com/uit-cosmo/cosmoplots
 License: MIT
 Author: gregordecristoforo
 Author-email: gregor.decristoforo@gmail.com
 Requires-Python: >=3.8,<3.13
 Classifier: License :: OSI Approved :: MIT License
@@ -41,31 +41,30 @@
 ```
 
 ## Usage
 
 Set your `rcparams` before plotting in your code, for example:
 
 ```python
+import matplotlib.pyplot as plt
 import cosmoplots
-import matplotlib as mpl
-
 # If you only want the default style
-mpl.style.use("cosmoplots.default")
+plt.style.use(["cosmoplots.default"])
 ```
 
 ### Muliple subfigures
-To make a figure with multiple rows or columns, use `cosmoplots.figure_multiple_rows_columns`:
+To make a figure with multiple rows or columns, use `cosmoplots.figure_multiple_rows_columns`.
+By default, the labels are $\mathrm{(a)}$, $\mathrm{(b)}$, $\mathrm{(c)}$, ..., but they may be replaced using the `labels` argument.
 ```python
-import matplotlib as mpl
 import matplotlib.pyplot as plt
-import numpy as np
-
 import cosmoplots
+plt.style.use(["cosmoplots.default"])
+
+import numpy as np
 
-mpl.style.use(["cosmoplots.default"])
 rows = 1
 columns = 2
 
 fig, ax = cosmoplots.figure_multiple_rows_columns(rows, columns)
 a = np.linspace(-3,3,100)
 for i in range(rows*columns):
     ax[i].set_xlabel("X Axis")
@@ -75,20 +74,18 @@
 ```
 ![multifig](./assets/multifig.png)
 
 ## `change_log_axis_base`
 
 ```python
 import matplotlib.pyplot as plt
-import numpy as np
 import cosmoplots
-import matplotlib as mpl
+plt.style.use(["cosmoplots.default"])
+import numpy as np
 
-# Setup
-mpl.style.use("cosmoplots.default")
 a = np.exp(np.linspace(-3, 1, 100))
 
 # Plotting
 fig = plt.figure()
 ax1 = plt.gca()
 ax1.set_xlabel("X Axis")
 ax1.set_ylabel("Y Axis")
@@ -113,35 +110,34 @@
 ax2.plot(a)
 plt.show()
 ```
 
 ## `matplotlib` vs. `cosmoplots` defaults
 
 ```python
-import cosmoplots
-import matplotlib as mpl
 import matplotlib.pyplot as plt
+import cosmoplots
 import numpy as np
 
 def plot() -> None:
     a = np.exp(np.linspace(-3, 5, 100))
     fig = plt.figure()
     ax = fig.add_subplot()
     ax.set_xlabel("X Axis")
     ax.set_ylabel("Y Axis")
     ax.semilogy(a)
 
 # Matplotlib ------------------------------------------------------------------------- #
-with mpl.style.context("default"):
+with plt.style.context("default"):
     plot()
     # plt.savefig("assets/matplotlib.png")
     plt.show()
 
 # Cosmoplots ------------------------------------------------------------------------- #
-with mpl.style.context("cosmoplots.default"):
+with plt.style.context("cosmoplots.default"):
     plot()
     # plt.savefig("assets/cosmoplots.png")
     plt.show()
 ```
 
 | `matplotlib` | `cosmoplots` |
 | :--------: | :--------: |
@@ -154,26 +150,25 @@
 ## `generate_hex_colors`
 
 This function generates the hex numbers for the colours extracted from a `matplotlib` colour map based on the number of points of interest.
 The colors change gradually from bright to dark or vice versa.
 ```python
 import matplotlib.pyplot as plt
 import cosmoplots
-
-axes_size = cosmoplots.set_rcparams_dynamo(plt.rcParams, num_cols=1, ls="thin")
+plt.style.use(["cosmoplots.default"])
 
 
 color_list = cosmoplots.generate_hex_colors(5, 'viridis', show_swatch=True, ascending=True)
 plt.savefig("./assets/hex_colors.png")
 
 # Print color_list to retrieve the hex numbers
 print(color_list) #['#fde725', '#5ec962', '#21918c', '#3b528b', '#440154']
 
 fig = plt.figure()
-ax = fig.add_axes(axes_size)
+ax = plt.gca()
 for i, color in enumerate(color_list):
     ax.plot([1,2],[i,i+1], c = color)
 
 plt.savefig("./assets/hex_colors_example.png")
 plt.show()
 ```
 | `hex_colors.png` | hex_colors_example.png |
@@ -191,21 +186,18 @@
 conveniently available from the `combine` function in `cosmoplots`.
 
 An example is shown below. Also see the [`tests`](./tests/) directory for more examples.
 A `help` method that prints the `imagemagick` commands that are used under the hood is
 also available.
 
 ```python
-import matplotlib as mpl
 import matplotlib.pyplot as plt
-import numpy as np
-
 import cosmoplots
-
-mpl.style.use("cosmoplots.default")
+plt.style.use("cosmoplots.default")
+import numpy as np
 
 
 def plot(i) -> None:
     """Create a simple plot."""
     a = np.exp(np.linspace(-3, 5, 100))
     fig = plt.figure()
     ax = fig.add_subplot()
```

