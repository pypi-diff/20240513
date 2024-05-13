# Comparing `tmp/itrm-0.1.9.tar.gz` & `tmp/itrm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itrm-0.1.9.tar", last modified: Mon May  6 20:37:44 2024, max compression
+gzip compressed data, was "itrm-0.2.0.tar", last modified: Mon May 13 17:04:42 2024, max compression
```

## Comparing `itrm-0.1.9.tar` & `itrm-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:37:44.035175 itrm-0.1.9/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 itrm-0.1.9/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     8988 2024-05-06 20:37:44.035064 itrm-0.1.9/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     8531 2024-05-06 19:59:43.000000 itrm-0.1.9/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 itrm-0.1.9/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      579 2024-05-06 20:37:44.035406 itrm-0.1.9/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:37:44.033139 itrm-0.1.9/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:37:44.034013 itrm-0.1.9/src/itrm/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-05-06 19:09:39.000000 itrm-0.1.9/src/itrm/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      308 2024-05-06 20:32:31.000000 itrm-0.1.9/src/itrm/eg_iplot.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    49360 2024-05-06 20:37:11.000000 itrm-0.1.9/src/itrm/itrm.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:37:44.034865 itrm-0.1.9/src/itrm.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     8988 2024-05-06 20:37:44.000000 itrm-0.1.9/src/itrm.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      264 2024-05-06 20:37:44.000000 itrm-0.1.9/src/itrm.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-06 20:37:44.000000 itrm-0.1.9/src/itrm.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-05-06 20:37:44.000000 itrm-0.1.9/src/itrm.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        5 2024-05-06 20:37:44.000000 itrm-0.1.9/src/itrm.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-13 17:04:42.397034 itrm-0.2.0/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 itrm-0.2.0/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    15006 2024-05-13 17:04:42.396902 itrm-0.2.0/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    14549 2024-05-13 17:03:52.000000 itrm-0.2.0/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 itrm-0.2.0/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      579 2024-05-13 17:04:42.397272 itrm-0.2.0/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-13 17:04:42.395173 itrm-0.2.0/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-13 17:04:42.395916 itrm-0.2.0/src/itrm/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-05-06 19:09:39.000000 itrm-0.2.0/src/itrm/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    64134 2024-05-13 17:00:18.000000 itrm-0.2.0/src/itrm/itrm.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-13 17:04:42.396686 itrm-0.2.0/src/itrm.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    15006 2024-05-13 17:04:42.000000 itrm-0.2.0/src/itrm.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      243 2024-05-13 17:04:42.000000 itrm-0.2.0/src/itrm.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-13 17:04:42.000000 itrm-0.2.0/src/itrm.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-05-13 17:04:42.000000 itrm-0.2.0/src/itrm.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        5 2024-05-13 17:04:42.000000 itrm-0.2.0/src/itrm.egg-info/top_level.txt
```

### Comparing `itrm-0.1.9/LICENSE.txt` & `itrm-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `itrm-0.1.9/PKG-INFO` & `itrm-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itrm
-Version: 0.1.9
+Version: 0.2.0
 Summary: Interactive Terminal Utilities
 Home-page: https://gitlab.com/davidwoodburn/itrm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,33 +22,64 @@
 This library provides several functions for nicely printing data to the
 terminal. MatPlotLib is a very nice library, but it can be a bit tedious at
 times when all you want is something quick and dirty.
 
 -   Every separate plot needs to be introduced with a `plt.figure()` statement.
 -   Large sets of data can be slow to render.
 -   If you are working in full screen on the terminal, plots can pull you to
-    another window.
+    another window which can be obnoxious.
 -   The entire python program and the terminal is locked up after any
     `plt.show()` command until you close all figure windows.
 -   Unless you save the figures to individual files, there is no buffer to show
     plots from past runs.
+-   Sometimes it it not available, such as when running code on a server through
+    SSH.
 
 These are all excuses to use this library. But, the biggest reason to use this
 library is that the terminal is cool, and the more you can do your work in the
 terminal the better!
 
-## Plots
+As a warning, the terminal emulator built into Neovim does seem to struggle to
+correctly handle string buffering of Unicode characters. Consequently, with
+`itrm.config.uni` set to `True` (the default) the plots can have garbled
+characters and not display correctly. Setting the `uni` property to `False` will
+remove that problem. Other terminal emulators tested do not have this problem.
+
+## Defaults
+
+While `itrm` does not use dotfiles, you can set some "defaults" with the
+`config` class. For example, by default Unicode characters are used throughout,
+but you can change this by setting `itrm.config.uni` to `False` before any other
+call to `itrm`. The following table lists the configuration options:
+
+| Setting       | Default       | Description                       |
+| ---------     | :-----------: | --------------------------------- |
+| `uni`         | `True`        | flag to use Unicode characters    |
+| `cols`        | `60`          | default column width              |
+| `rows`        | `20`          | default row height                |
+| `ar`          | `0.48`        | aspect ratio of characters        |
+
+There is also a method for changing the color map: `itrm.config.cmap()`. It
+takes a string: `"colors"`, `"grays"`, `"reds"`, `"greens"`, or `"blues"`.
+
+## Interactive Plots
 
 ```python
-itrm.plot(x, y=None, label='', rows=1, cols=1, equal=0)
+itrm.iplot(x, y=None, label=None, rows=1, cols=1,
+        lg=None, overlay=False):
 ```
 
-The plot function will render all the data points defined by `x` and `y` to the
-terminal. The inputs `x` and `y` can be vectors or matrices. If they are
-matrices, each row is treated as a separate curve.
+The `iplot` function will render all the data points defined by `x` and `y` to
+the terminal. The inputs `x` and `y` can be vectors or matrices. If they are
+matrices, each **row** is treated as a separate curve. Note, this is different
+from MatPlotLib, in which each *column* is treated as a separate row. (This
+difference is intentional, as in the author's opinion varying time along columns
+means each column in a matrix can be treated as a vector. This arrangement works
+very well with in linear algebra, especially matrix multiplication with a "set"
+of vectors over time.)
 
 The shapes of `x` and `y` do not have to be the same, but they must be
 compatible. So, `x` could be a vector and `y` could be a matrix as long as the
 length of `x` equals the number of columns of `y`.
 
 If only `x` is given, it will be interpreted as the `y` values, and the `x`
 values will be the array of indices.
@@ -65,61 +96,139 @@
 If a `label` is given, this will be printed in the bottom right of the plot box.
 
 The `rows` and `cols` parameters let you specify the number of terminal text
 rows and columns to use for the plot, respectively. For each of these, if the
 value is less than or equal to 1, it represents a portion of the available space
 to use. For example, if `rows` is `0.5`, then half the number of rows of the
 current terminal window will be used for the plot. If the value is greater than
-1, it represents the absolute number of columns or rows to use. Also, if the
+1, it represents the absolute number of rows or columns to use. Also, if the
 size of the current terminal cannot be obtained, the available space will
 default to `20` rows and `60` columns. These defaults can be redefined by
-changing `itrm.config.rows` and `itrm.config.cols`.
+changing `itrm.config.rows` and `itrm.config.cols`, respectively.
 
 By default, this library will use Unicode symbols (specifically braille) for
-plotting. A good font to use is JuliaMono. However, if your font does not
+plotting. A recommended font is JuliaMono. However, if your font does not
 support the necessary Unicode symbols, you can tell the library to not use them
 by setting `itrm.config.uni` to `False` before calling the `itrm.plot` function.
+In that case, only ASCII characters will be used.
 
-If only one curve is being plotted, the characters will be written in whatever
-the default font color is set to in your terminal. If more than one curve is
-plotted, color will be used. The color map is blue, green, yellow, orange, and
-magenta. If you have more than 5 curves (This is just a terminal-based plot; why
-would you do that?), then the colors will recycle.
-
-If you want equal axis scaling, set `equal` to `1`. However, since terminal
-fonts are not always the same aspect ratio and because the line spacing in your
-terminal might be adjustable, you can adjust this value to tune.
+To distinguish multiple curves from each other, colors will be used. The color
+map is blue, green, yellow, orange, magenta, and purple. If you have more than 6
+curves (This is just a terminal-based plot; why would you do that?), then the
+colors will recycle.
+
+You can set the x or y axes to logarithmic scaling by setting the `lg` parameter
+to one of `"x"`, `"y"`, or `"xy"`. Note that the values reported for the view
+and the cursor will also be logarithmic.
+
+To prevent your terminal history from extending each time a new plot is
+rendered, you can print a new plot over a previous plot by setting the `overlay`
+parameter to `True`. This can be especially useful when there a multiple plots
+to render but you do not want your terminal history to fill up quickly.
+
+The `iplot` function provides interactivity through a vertical cursor. You can
+move the cursor left and right, at normal speed or fast speed. You can zoom in
+and out. And, you can cycle through which rows of the `x` and `y` data to focus
+on. Note, `iplot` is designed for monotonically-increasing `x` values, and,
+consequently, does not support equal axis scaling.
 
-| Single curve    | Multiple curves |
-| --------------- | --------------- |
-| ![](https://gitlab.com/davidwoodburn/itrm/-/raw/main/figures/fig_plot_1.png) | ![](https://gitlab.com/davidwoodburn/itrm/-/raw/main/figures/fig_plot_5.png) |
+![](https://gitlab.com/davidwoodburn/itrm/-/raw/main/figures/fig_iplot.png)
 
-## Interactive Plots
+The following table details the shortcut keys:
+
+| Keys               | Function                 |   | Keys           | Function                 |
+| :----------------: | ------------------------ | - | :------------: | ------------------------ |
+| `q`, `x`, `⌫`, `↵` | exit interactive plot    |   | `j`, `s`, `↓`  | zoom in                  |
+| `h`, `a`, `←`      | move cursor left         |   | `k`, `w`, `↑`  | zoom out                 |
+| `l`, `d`, `→`      | move cursor right        |   | `J`, `S`, `⇧↓` | zoom in fast             |
+| `H`, `A`, `⇧←`     | move cursor left fast    |   | `K`, `W`, `⇧↑` | zoom out fast            |
+| `L`, `D`, `⇧→`     | move cursor right fast   |   | `n`            | next data row            |
+| `g`                | move cursor to start     |   | `p`            | previous data row        |
+| `G`                | move cursor to end       |   | `i`            | toggle individual view   |
+| `c`, `z`           | center view on cursor    |   | `r`            | redraw the whole plot    |
+
+## Plots
 
 ```python
-itrm.iplot(x, y=None, label='', rows=1, cols=1)
+itrm.plot(x, y=None, label=None, rows=1, cols=1,
+        equal_axes=0, lg=None, overlay=False):
 ```
 
-The `iplot` function is nearly identical to the `plot` function, except that the
-resulting plot will be interactive with a cursor you can move to inspect the
-values. You can move the cursor left and right, at normal speed or fast speed.
-You can zoom in and out. And, you can cycle through which rows of the `x` and
-`y` data to focus on.
+The `plot` function is a non-interactive version of the `iplot` function.
 
-The following table details the shortcut keys:
+The `plot` function will render all the data points defined by `x` and `y` to
+the terminal. The inputs `x` and `y` can be vectors or matrices. If they are
+matrices, each **row** is treated as a separate curve. Note, this is different
+from MatPlotLib, in which each *column* is treated as a separate row. (This
+difference is intentional, as in the author's opinion varying time along columns
+means each column in a matrix can be treated as a vector. This arrangement works
+very well with in linear algebra, especially matrix multiplication with a "set"
+of vectors over time.)
 
-| Keys           | Function                 |   | Keys           | Function                 |
-| :------------: | ------------------------ | - | :------------: | ------------------------ |
-| `q`, `x`, `⌫`  | exit interactive plot    |   | `j`, `s`, `↓`  | zoom in                  |
-| `h`, `a`, `←`  | move cursor left         |   | `k`, `w`, `↑`  | zoom out                 |
-| `l`, `d`, `→`  | move cursor right        |   | `J`, `S`, `⇧↓` | zoom in fast             |
-| `H`, `A`, `⇧←` | move cursor left fast    |   | `K`, `W`, `⇧↑` | zoom out fast            |
-| `L`, `D`, `⇧→` | move cursor right fast   |   | `n`            | next data row            |
-| `g`            | move cursor to start     |   | `p`            | previous data row        |
-| `G`            | move cursor to end       |   | `c`, `z`       | center view on cursor    |
+The shapes of `x` and `y` do not have to be the same, but they must be
+compatible. So, `x` could be a vector and `y` could be a matrix as long as the
+length of `x` equals the number of columns of `y`.
+
+If only `x` is given, it will be interpreted as the `y` values, and the `x`
+values will be the array of indices.
+
+When the plot is printed, the graph is rendered within a box and the ranges of
+`x` and `y` are listed in the bottom left corner. So,
+
+```
+(0:99, -1.5:1.5)
+```
+
+means that `x` ranges from `0` to `99` and `y` ranges from `-1.5` to `1.5`.
+
+If a `label` is given, this will be printed in the bottom right of the plot box.
+
+The `rows` and `cols` parameters let you specify the number of terminal text
+rows and columns to use for the plot, respectively. For each of these, if the
+value is less than or equal to 1, it represents a portion of the available space
+to use. For example, if `rows` is `0.5`, then half the number of rows of the
+current terminal window will be used for the plot. If the value is greater than
+1, it represents the absolute number of rows or columns to use. Also, if the
+size of the current terminal cannot be obtained, the available space will
+default to `20` rows and `60` columns. These defaults can be redefined by
+changing `itrm.config.rows` and `itrm.config.cols`, respectively.
+
+By default, this library will use Unicode symbols (specifically braille) for
+plotting. A recommended font is JuliaMono. However, if your font does not
+support the necessary Unicode symbols, you can tell the library to not use them
+by setting `itrm.config.uni` to `False` before calling the `itrm.plot` function.
+In that case, only ASCII characters will be used.
+
+To distinguish multiple curves from each other, colors will be used. The color
+map is blue, green, yellow, orange, magenta, and purple. If you have more than 6
+curves (This is just a terminal-based plot; why would you do that?), then the
+colors will recycle.
+
+If you want equal axis scaling, set `equal_axes` to `True`. However, since
+terminal fonts are not always the same aspect ratio and because the line spacing
+in your terminal might be adjustable, you can adjust the understood character
+aspect ratio with `itrm.config.ar`. The default value is `0.48`. This means the
+width of a character is understood to be about 0.48 of the height of a
+character. Making this value larger means the characters are interpreted to be
+wider, making the plot narrower horizontally. This is a feature the `iplot`
+function does not share. Because the `plot` supports equal axis scaling, it does
+not require that the `x` axis data monotonically increase.
+
+You can set the x or y axes to logarithmic scaling by setting the `lg` parameter
+to one of `"x"`, `"y"`, or `"xy"`. Note that the values reported for the view
+will also be logarithmic.
+
+To prevent your terminal history from extending each time a new plot is
+rendered, you can print a new plot over a previous plot by setting the `overlay`
+parameter to `True`. This can be especially useful when creating a live
+animation.
+
+| Single curve    | Multiple curves |
+| --------------- | --------------- |
+| ![](https://gitlab.com/davidwoodburn/itrm/-/raw/main/figures/fig_plot_1.png) | ![](https://gitlab.com/davidwoodburn/itrm/-/raw/main/figures/fig_plot_6.png) |
 
 ## Bars
 
 ```python
 itrm.bars(x, labels=None, cols=1, fat=False)
 ```
```

### Comparing `itrm-0.1.9/README.md` & `itrm-0.2.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -7,33 +7,64 @@
 This library provides several functions for nicely printing data to the
 terminal. MatPlotLib is a very nice library, but it can be a bit tedious at
 times when all you want is something quick and dirty.
 
 -   Every separate plot needs to be introduced with a `plt.figure()` statement.
 -   Large sets of data can be slow to render.
 -   If you are working in full screen on the terminal, plots can pull you to
-    another window.
+    another window which can be obnoxious.
 -   The entire python program and the terminal is locked up after any
     `plt.show()` command until you close all figure windows.
 -   Unless you save the figures to individual files, there is no buffer to show
     plots from past runs.
+-   Sometimes it it not available, such as when running code on a server through
+    SSH.
 
 These are all excuses to use this library. But, the biggest reason to use this
 library is that the terminal is cool, and the more you can do your work in the
 terminal the better!
 
-## Plots
+As a warning, the terminal emulator built into Neovim does seem to struggle to
+correctly handle string buffering of Unicode characters. Consequently, with
+`itrm.config.uni` set to `True` (the default) the plots can have garbled
+characters and not display correctly. Setting the `uni` property to `False` will
+remove that problem. Other terminal emulators tested do not have this problem.
+
+## Defaults
+
+While `itrm` does not use dotfiles, you can set some "defaults" with the
+`config` class. For example, by default Unicode characters are used throughout,
+but you can change this by setting `itrm.config.uni` to `False` before any other
+call to `itrm`. The following table lists the configuration options:
+
+| Setting       | Default       | Description                       |
+| ---------     | :-----------: | --------------------------------- |
+| `uni`         | `True`        | flag to use Unicode characters    |
+| `cols`        | `60`          | default column width              |
+| `rows`        | `20`          | default row height                |
+| `ar`          | `0.48`        | aspect ratio of characters        |
+
+There is also a method for changing the color map: `itrm.config.cmap()`. It
+takes a string: `"colors"`, `"grays"`, `"reds"`, `"greens"`, or `"blues"`.
+
+## Interactive Plots
 
 ```python
-itrm.plot(x, y=None, label='', rows=1, cols=1, equal=0)
+itrm.iplot(x, y=None, label=None, rows=1, cols=1,
+        lg=None, overlay=False):
 ```
 
-The plot function will render all the data points defined by `x` and `y` to the
-terminal. The inputs `x` and `y` can be vectors or matrices. If they are
-matrices, each row is treated as a separate curve.
+The `iplot` function will render all the data points defined by `x` and `y` to
+the terminal. The inputs `x` and `y` can be vectors or matrices. If they are
+matrices, each **row** is treated as a separate curve. Note, this is different
+from MatPlotLib, in which each *column* is treated as a separate row. (This
+difference is intentional, as in the author's opinion varying time along columns
+means each column in a matrix can be treated as a vector. This arrangement works
+very well with in linear algebra, especially matrix multiplication with a "set"
+of vectors over time.)
 
 The shapes of `x` and `y` do not have to be the same, but they must be
 compatible. So, `x` could be a vector and `y` could be a matrix as long as the
 length of `x` equals the number of columns of `y`.
 
 If only `x` is given, it will be interpreted as the `y` values, and the `x`
 values will be the array of indices.
@@ -50,61 +81,139 @@
 If a `label` is given, this will be printed in the bottom right of the plot box.
 
 The `rows` and `cols` parameters let you specify the number of terminal text
 rows and columns to use for the plot, respectively. For each of these, if the
 value is less than or equal to 1, it represents a portion of the available space
 to use. For example, if `rows` is `0.5`, then half the number of rows of the
 current terminal window will be used for the plot. If the value is greater than
-1, it represents the absolute number of columns or rows to use. Also, if the
+1, it represents the absolute number of rows or columns to use. Also, if the
 size of the current terminal cannot be obtained, the available space will
 default to `20` rows and `60` columns. These defaults can be redefined by
-changing `itrm.config.rows` and `itrm.config.cols`.
+changing `itrm.config.rows` and `itrm.config.cols`, respectively.
 
 By default, this library will use Unicode symbols (specifically braille) for
-plotting. A good font to use is JuliaMono. However, if your font does not
+plotting. A recommended font is JuliaMono. However, if your font does not
 support the necessary Unicode symbols, you can tell the library to not use them
 by setting `itrm.config.uni` to `False` before calling the `itrm.plot` function.
+In that case, only ASCII characters will be used.
 
-If only one curve is being plotted, the characters will be written in whatever
-the default font color is set to in your terminal. If more than one curve is
-plotted, color will be used. The color map is blue, green, yellow, orange, and
-magenta. If you have more than 5 curves (This is just a terminal-based plot; why
-would you do that?), then the colors will recycle.
-
-If you want equal axis scaling, set `equal` to `1`. However, since terminal
-fonts are not always the same aspect ratio and because the line spacing in your
-terminal might be adjustable, you can adjust this value to tune.
+To distinguish multiple curves from each other, colors will be used. The color
+map is blue, green, yellow, orange, magenta, and purple. If you have more than 6
+curves (This is just a terminal-based plot; why would you do that?), then the
+colors will recycle.
+
+You can set the x or y axes to logarithmic scaling by setting the `lg` parameter
+to one of `"x"`, `"y"`, or `"xy"`. Note that the values reported for the view
+and the cursor will also be logarithmic.
+
+To prevent your terminal history from extending each time a new plot is
+rendered, you can print a new plot over a previous plot by setting the `overlay`
+parameter to `True`. This can be especially useful when there a multiple plots
+to render but you do not want your terminal history to fill up quickly.
+
+The `iplot` function provides interactivity through a vertical cursor. You can
+move the cursor left and right, at normal speed or fast speed. You can zoom in
+and out. And, you can cycle through which rows of the `x` and `y` data to focus
+on. Note, `iplot` is designed for monotonically-increasing `x` values, and,
+consequently, does not support equal axis scaling.
 
-| Single curve    | Multiple curves |
-| --------------- | --------------- |
-| ![](https://gitlab.com/davidwoodburn/itrm/-/raw/main/figures/fig_plot_1.png) | ![](https://gitlab.com/davidwoodburn/itrm/-/raw/main/figures/fig_plot_5.png) |
+![](https://gitlab.com/davidwoodburn/itrm/-/raw/main/figures/fig_iplot.png)
 
-## Interactive Plots
+The following table details the shortcut keys:
+
+| Keys               | Function                 |   | Keys           | Function                 |
+| :----------------: | ------------------------ | - | :------------: | ------------------------ |
+| `q`, `x`, `⌫`, `↵` | exit interactive plot    |   | `j`, `s`, `↓`  | zoom in                  |
+| `h`, `a`, `←`      | move cursor left         |   | `k`, `w`, `↑`  | zoom out                 |
+| `l`, `d`, `→`      | move cursor right        |   | `J`, `S`, `⇧↓` | zoom in fast             |
+| `H`, `A`, `⇧←`     | move cursor left fast    |   | `K`, `W`, `⇧↑` | zoom out fast            |
+| `L`, `D`, `⇧→`     | move cursor right fast   |   | `n`            | next data row            |
+| `g`                | move cursor to start     |   | `p`            | previous data row        |
+| `G`                | move cursor to end       |   | `i`            | toggle individual view   |
+| `c`, `z`           | center view on cursor    |   | `r`            | redraw the whole plot    |
+
+## Plots
 
 ```python
-itrm.iplot(x, y=None, label='', rows=1, cols=1)
+itrm.plot(x, y=None, label=None, rows=1, cols=1,
+        equal_axes=0, lg=None, overlay=False):
 ```
 
-The `iplot` function is nearly identical to the `plot` function, except that the
-resulting plot will be interactive with a cursor you can move to inspect the
-values. You can move the cursor left and right, at normal speed or fast speed.
-You can zoom in and out. And, you can cycle through which rows of the `x` and
-`y` data to focus on.
+The `plot` function is a non-interactive version of the `iplot` function.
 
-The following table details the shortcut keys:
+The `plot` function will render all the data points defined by `x` and `y` to
+the terminal. The inputs `x` and `y` can be vectors or matrices. If they are
+matrices, each **row** is treated as a separate curve. Note, this is different
+from MatPlotLib, in which each *column* is treated as a separate row. (This
+difference is intentional, as in the author's opinion varying time along columns
+means each column in a matrix can be treated as a vector. This arrangement works
+very well with in linear algebra, especially matrix multiplication with a "set"
+of vectors over time.)
 
-| Keys           | Function                 |   | Keys           | Function                 |
-| :------------: | ------------------------ | - | :------------: | ------------------------ |
-| `q`, `x`, `⌫`  | exit interactive plot    |   | `j`, `s`, `↓`  | zoom in                  |
-| `h`, `a`, `←`  | move cursor left         |   | `k`, `w`, `↑`  | zoom out                 |
-| `l`, `d`, `→`  | move cursor right        |   | `J`, `S`, `⇧↓` | zoom in fast             |
-| `H`, `A`, `⇧←` | move cursor left fast    |   | `K`, `W`, `⇧↑` | zoom out fast            |
-| `L`, `D`, `⇧→` | move cursor right fast   |   | `n`            | next data row            |
-| `g`            | move cursor to start     |   | `p`            | previous data row        |
-| `G`            | move cursor to end       |   | `c`, `z`       | center view on cursor    |
+The shapes of `x` and `y` do not have to be the same, but they must be
+compatible. So, `x` could be a vector and `y` could be a matrix as long as the
+length of `x` equals the number of columns of `y`.
+
+If only `x` is given, it will be interpreted as the `y` values, and the `x`
+values will be the array of indices.
+
+When the plot is printed, the graph is rendered within a box and the ranges of
+`x` and `y` are listed in the bottom left corner. So,
+
+```
+(0:99, -1.5:1.5)
+```
+
+means that `x` ranges from `0` to `99` and `y` ranges from `-1.5` to `1.5`.
+
+If a `label` is given, this will be printed in the bottom right of the plot box.
+
+The `rows` and `cols` parameters let you specify the number of terminal text
+rows and columns to use for the plot, respectively. For each of these, if the
+value is less than or equal to 1, it represents a portion of the available space
+to use. For example, if `rows` is `0.5`, then half the number of rows of the
+current terminal window will be used for the plot. If the value is greater than
+1, it represents the absolute number of rows or columns to use. Also, if the
+size of the current terminal cannot be obtained, the available space will
+default to `20` rows and `60` columns. These defaults can be redefined by
+changing `itrm.config.rows` and `itrm.config.cols`, respectively.
+
+By default, this library will use Unicode symbols (specifically braille) for
+plotting. A recommended font is JuliaMono. However, if your font does not
+support the necessary Unicode symbols, you can tell the library to not use them
+by setting `itrm.config.uni` to `False` before calling the `itrm.plot` function.
+In that case, only ASCII characters will be used.
+
+To distinguish multiple curves from each other, colors will be used. The color
+map is blue, green, yellow, orange, magenta, and purple. If you have more than 6
+curves (This is just a terminal-based plot; why would you do that?), then the
+colors will recycle.
+
+If you want equal axis scaling, set `equal_axes` to `True`. However, since
+terminal fonts are not always the same aspect ratio and because the line spacing
+in your terminal might be adjustable, you can adjust the understood character
+aspect ratio with `itrm.config.ar`. The default value is `0.48`. This means the
+width of a character is understood to be about 0.48 of the height of a
+character. Making this value larger means the characters are interpreted to be
+wider, making the plot narrower horizontally. This is a feature the `iplot`
+function does not share. Because the `plot` supports equal axis scaling, it does
+not require that the `x` axis data monotonically increase.
+
+You can set the x or y axes to logarithmic scaling by setting the `lg` parameter
+to one of `"x"`, `"y"`, or `"xy"`. Note that the values reported for the view
+will also be logarithmic.
+
+To prevent your terminal history from extending each time a new plot is
+rendered, you can print a new plot over a previous plot by setting the `overlay`
+parameter to `True`. This can be especially useful when creating a live
+animation.
+
+| Single curve    | Multiple curves |
+| --------------- | --------------- |
+| ![](https://gitlab.com/davidwoodburn/itrm/-/raw/main/figures/fig_plot_1.png) | ![](https://gitlab.com/davidwoodburn/itrm/-/raw/main/figures/fig_plot_6.png) |
 
 ## Bars
 
 ```python
 itrm.bars(x, labels=None, cols=1, fat=False)
 ```
```

### Comparing `itrm-0.1.9/setup.cfg` & `itrm-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = itrm
-version = 0.1.9
+version = 0.2.0
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = Interactive Terminal Utilities
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/itrm
 classifiers =
```

### Comparing `itrm-0.1.9/src/itrm/itrm.py` & `itrm-0.2.0/src/itrm/itrm.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,127 +17,106 @@
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
 __author__ = "David Woodburn"
 __license__ = "MIT"
-__date__ = "2024-04-24"
+__date__ = "2024-05-13"
 __maintainer__ = "David Woodburn"
 __email__ = "david.woodburn@icloud.com"
 __status__ = "Development"
 
 import os
 import sys
 import signal
 import termios
 import time
 import math
 import numpy as np
 
 
 # Constants
-NORMAL_COLORS = [39, 40, 220, 202, 201] # blue, green, yellow, orange, magenta
-BRIGHT_COLORS = [87, 82, 228, 216, 213] # blue, green, yellow, orange, magenta
-COLOR_CNT = 5 # number of colors in the color map
+# (blue, green, yellow, orange, magenta, purple)
+DARK_COLORS = [33, 40, 220, 202, 201,  93]
+LITE_COLORS = [75, 82, 228, 214, 213, 135]
+DARK_GRAYS = [253, 250, 247, 244, 241, 238]
+LITE_GRAYS = [255, 252, 249, 246, 243, 240]
+DARK_REDS = [197, 196, 160, 124,  88, 52]
+LITE_REDS = [198, 197, 196, 160, 124, 88]
+DARK_GREENS = [47, 46, 40, 34, 28, 22]
+LITE_GREENS = [48, 47, 46, 40, 34, 28]
+DARK_BLUES = [27, 21, 20, 19, 18, 17]
+LITE_BLUES = [33, 27, 21, 20, 19, 18]
+COLOR_CNT = 6 # number of colors in the color map
+eps = 1e-32 # minimum magnitude
 
 
 class config: # configuration settings
     uni = True # flag to use Unicode characters
     cols = 60 # default column width
     rows = 20 # default row height
-    ar = 2.1 # aspect ratio of characters
+    ar = 0.48 # aspect ratio of characters
+    darks = DARK_COLORS # dark color map
+    lites = LITE_COLORS # light color map
+    
+    def cmap(cmap="colors"):
+        if not isinstance(cmap, str):
+            raise ValueError(f"cmap must be a string: {cmap}")
+        if cmap == "colors":
+            config.darks = DARK_COLORS
+            config.lites = LITE_COLORS
+        elif cmap == "grays":
+            config.darks = DARK_GRAYS
+            config.lites = LITE_GRAYS
+        elif cmap == "reds":
+            config.darks = DARK_REDS
+            config.lites = LITE_REDS
+        elif cmap == "greens":
+            config.darks = DARK_GREENS
+            config.lites = LITE_GREENS
+        elif cmap == "blues":
+            config.darks = DARK_BLUES
+            config.lites = LITE_BLUES
+        else:
+            raise ValueError("cmap must be one of "
+                    + "'colors', 'grays', 'reds', 'greens', or 'blues'")
 
 
 class persistent: # persistent, run-time values
     t_last = None # last time value
     orig_term_attr = None # original terminal attributes
     rows_last = None # last number of plot rows
 
 
 class limits: # x and y data limits
-    def __init__(self, x_min=None, x_max=None, y_min=None, y_max=None):
-        self.x_min = x_min
-        self.x_max = x_max
-        self.y_min = y_min
-        self.y_max = y_max
+    def __init__(self, x_min=None, x_max=None, y_min=None, y_max=None,
+            k_min=None, k_max=None, k_xc=None):
+        self.x_min = x_min # minimum x
+        self.x_max = x_max # maximum x
+        self.y_min = y_min # minimum y
+        self.y_max = y_max # maximum y
+        self.k_min = k_min # indices of minimum x
+        self.k_max = k_max # indices of maximum x
+        self.k_xc = k_xc   # indices of x near cursor
+        self.tmp = 0.0
 
 
 class term_ws: # terminal window size and sub-character resolution
     def __init__(self, rows, cols, subrows=None, subcols=None):
         self.rows = rows
         self.cols = cols
         self.subrows = subrows
         self.subcols = subcols
 
 # ------------------
 # Plotting functions
 # ------------------
 
-def plot(x, y=None, label=None, rows=1, cols=1, equal=0, overlay=False):
-    """
-    Create a text-based plot of the path defined by (`x`, `y`) using characters.
-    If the size of the terminal can be found, that will be used for sizing the
-    plot. Otherwise, the default dimensions (config.cols, config.rows) will be
-    used. Note that this function does not plot connecting lines, only the
-    points specified by the (`x`, `y`) pairs.
-
-    Parameters
-    ----------
-    x : (K,) or (J, K) np.ndarray
-        Array of x-axis values or matrix of rows of x-axis values.
-    y : (K,) or (J, K) np.ndarray, default None
-        Array of y-axis values or matrix of rows of y-axis values. If `y` is not
-        provided, `x` will be used as the `y` array and `x` will be defined to
-        be an array of indices (starting at zero).
-    label : str, default ''
-        Text to place at top of the plot, centered in the border.
-    rows : int, default 1
-        Desired number of rows if greater than 1 or fraction of existing rows if
-        less than 1.
-    cols : int, default 1
-        Desired number of columns if greater than 1 or fraction of window
-        columns if less than 1.
-    equal : float, default 0
-        Axis scaling, `y` to `x`. A value of 0 leaves the scaling alone. A value
-        of 1 would approximate equal axis scaling. However, because the aspect
-        ratio of characters in the terminal is not exactly 2 to 1, this value
-        can be adjusted to compensate.
-
-    Notes
-    -----
-    Non-finite values will be ignored.
-    """
-
-    # Check and (possibly) adjust the shapes of x and y.
-    x, y = shape_xy(x, y)
-
-    # Choose the canvas size.
-    tws = screen_size(rows, cols)
-    if overlay and (persistent.rows_last is not None):
-        print(f"\x1b[{persistent.rows_last + 2}A", end='', flush=True)
-
-    # Get the data limits, adjusting for the terminal window size.
-    lims, row_zero = limits_xy(x, y, tws, equal)
-
-    # Map x and y to the expanded canvas, M, and the foreground color matrix, F.
-    M, F = data_to_matrix(x, y, lims, tws)
-
-    # Convert the expanded matrix, M, to a matrix of character values, C.
-    C = matrix_to_braille(M) if config.uni else matrix_to_ascii(M)
-
-    # Get the ranges text.
-    ranges = f"({ftostr(lims.x_min)}:{ftostr(lims.x_max)}, " \
-            + f"{ftostr(lims.y_min)}:{ftostr(lims.y_max)})"
-
-    # Draw the plot.
-    draw_graph(C, ranges, label, F, row_zero)
-
-
-def iplot(x, y=None, label=None, rows=1, cols=1, overlay=False):
+def iplot(x, y=None, label=None, rows=1, cols=1, lg=None, overlay=False):
     """
     Create an interactive, text-based plot of the path defined by (`x`, `y`)
     using characters. If the size of the terminal can be found, that will be
     used for sizing the plot. Otherwise, the default dimensions (config.cols,
     config.rows) will be used. Note that this function does not plot connecting
     lines, only the points specified by the (`x`, `y`) pairs. Once the function
     has been called, the terminal will be in interactive mode. The user can then
@@ -147,410 +126,589 @@
     ----------
     x : (K,) or (J, K) np.ndarray
         Array of x-axis values or matrix of rows of x-axis values.
     y : (K,) or (J, K) np.ndarray, default None
         Array of y-axis values or matrix of rows of y-axis values. If `y` is not
         provided, `x` will be used as the `y` array and `x` will be defined to
         be an array of indices (starting at zero).
-    label : str, default ''
+    label : str, default ""
         Text to place at top of the plot, centered in the border.
     rows : int, default 1
         Desired number of rows if greater than 1 or fraction of existing rows if
         less than 1.
     cols : int, default 1
         Desired number of columns if greater than 1 or fraction of window
         columns if less than 1.
+    lg : str, default None
+        Logarithmic scaling of axes. If `None`, both axes will have linear
+        scaling. Otherwise, `lg` should be a string: "x", "y", or "xy".
+    overlay : bool, default False
+        Flag to print new plot on top of a previous plot.
 
     Shortcuts
     ---------
-    q, x, ⌫  : exit interactive plot
-    h, a, ←  : move cursor left
-    l, d, →  : move cursor right
-    H, A, ⇧← : move cursor left fast
-    L, D, ⇧→ : move cursor right fast
-    g        : move cursor to start
-    G        : move cursor to end
-    j, s, ↓  : zoom in
-    k, w, ↑  : zoom out
-    J, S, ⇧↓ : zoom in fast
-    K, W, ⇧↑ : zoom out fast
-    n        : next data row
-    p        : previous data row
-    c, z     : center view on cursor
+    q, x, ⌫, ↵ : exit interactive plot
+    h, a, ←    : move cursor left
+    l, d, →    : move cursor right
+    H, A, ⇧←   : move cursor left fast
+    L, D, ⇧→   : move cursor right fast
+    g          : move cursor to start
+    G          : move cursor to end
+    j, s, ↓    : zoom in
+    k, w, ↑    : zoom out
+    J, S, ⇧↓   : zoom in fast
+    K, W, ⇧↑   : zoom out fast
+    n          : next data row
+    p          : previous data row
+    c, z       : center view on cursor
+    i          : toggle individual view
 
     Notes
     -----
-    Non-finite values will be ignored.
+    Non-finite values (i.e., nan, inf, -inf) will be ignored.
     """
 
     # Check if this is a tty.
     if not istty():
-        print("The iplot function will not work in this terminal.")
+        print("Not a proper terminal. Passing to plot.", flush=True)
+        plot(x, y, label, rows, cols, False, lg, overlay)
         return
 
     # Set signal handler for Ctrl+C
     signal.signal(signal.SIGINT, signal_handler)
 
     # Set raw mode
     try:
         persistent.orig_term_attr = termios.tcgetattr(0)
         tty_mode = persistent.orig_term_attr.copy()
         tty_mode[3] &= ~termios.ICANON & ~termios.ECHO
         tty_mode[3] |= termios.ISIG  # Enable ISIG flag (Ctrl-c to exit)
         termios.tcsetattr(0, termios.TCSANOW, tty_mode)
     except termios.error:
-        print("The iplot function will not work in this terminal.")
+        print("Not a proper terminal. Passing to plot.", flush=True)
+        plot(x, y, label, rows, cols, False, lg, overlay)
         return
 
     # Hide the cursor.
-    sys.stdout.write("\033[?25l")
+    print("\x1b[?25l", end="", flush=True)
 
     # Check and (possibly) adjust the shapes of x and y.
     x, y = shape_xy(x, y)
     J, K = x.shape
 
     # Get the canvas size.
     tws = screen_size(rows, cols)
-    if overlay and (persistent.rows_last is not None):
-        print(f"\x1b[{persistent.rows_last + 1}A", end='', flush=True)
-
-    # Get the data limits, adjusting for the terminal window size.
-    lims, _ = limits_xy(x, y, tws, 0) # ignore row_zero
 
-    # --------------------
-    # Draw a blank canvas.
-    # --------------------
-
-    # Create a blank expanded canvas.
-    Rows = tws.subrows*tws.rows
-    Cols = tws.subcols*tws.cols
-    M = np.zeros((Rows, Cols), dtype=int)
-
-    # Convert the expanded canvas, M, to a matrix of character values, C.
-    C = matrix_to_braille(M) if config.uni else matrix_to_ascii(M)
+    # Move up if this is overlayed.
+    if overlay and (persistent.rows_last is not None):
+        print(f"\x1b[{persistent.rows_last + 2}A", end="", flush=True)
+    persistent.rows_last = tws.rows
 
-    # Draw the canvas.
-    draw_graph(C)
+    # Apply logarithmic scaling.
+    if lg is not None:
+        if not isinstance(lg, str):
+            raise ValueError(f"lg must be None or a string: {lg}")
+        lg = lg.lower()
+        if lg == "x":
+            # Scale x logarithmic.
+            x = x.copy()
+            is_non_pos = ~np.isfinite(x) | (x <= 0)
+            x[is_non_pos] = np.nan
+            x = np.log10(x)
+        elif lg == "y":
+            # Scale y logarithmic.
+            y = y.copy()
+            is_non_pos = ~np.isfinite(y) | (y <= 0)
+            y[is_non_pos] = np.nan
+            y = np.log10(y)
+        elif (lg == "xy") or (lg == "yx"):
+            # Scale x logarithmic.
+            x = x.copy()
+            is_non_pos = ~np.isfinite(x) | (x <= 0)
+            x[is_non_pos] = np.nan
+            x = np.log10(x)
+            # Scale y logarithmic.
+            y = y.copy()
+            is_non_pos = ~np.isfinite(y) | (y <= 0)
+            y[is_non_pos] = np.nan
+            y = np.log10(y)
+        else:
+            raise ValueError(f"lg should be 'x', 'y', or 'xy': {lg}")
 
-    # ----------------------------------
-    # Fill in the details on the canvas.
-    # ----------------------------------
+    # Get the data limits, adjusting for the terminal window size.
+    lims = limits_xy(x, y, tws, False)
+    view = limits(lims.x_min, lims.x_max,
+            lims.y_min, lims.y_max,
+            lims.k_min, lims.k_max) # k_xc not defined yet
 
-    # Define the current view rectangle.
-    view = limits(lims.x_min, lims.x_max, lims.y_min, lims.y_max)
+    # Set the deltas based on what is not a white-space character.
+    s = 0x2800 if config.uni else 0x20 # white-space character
+    D = np.ones((tws.rows, tws.cols), dtype=bool)
 
     # Define the cursor.
-    cstate = -1 # cursor state ("-1" means all data rows)
     xc = (view.x_max + view.x_min)/2 # cursor at mid-point
-    xc = move_cursor(xc, 0, x) # align xc with closest x values
-    ccol = get_column(xc, view, tws) # cursor column index
-    yc_min, yc_max = get_cursor_y(ccol, tws, x, y, view) # y range at cursor
-    if yc_min == yc_max:
-        cstr = f"({ftostr(xc)}, {ftostr(yc_max)})" # cursor readout
-    else:
-        cstr = f"({ftostr(xc)}, {ftostr(yc_min)}:{ftostr(yc_max)})"
-    cF = "\x1b[0m" # cursor foreground color
+    xc, k_xc = set_cursor(xc, x, view, tws) # align xc with closest x values
     dx = (view.x_max - view.x_min)/tws.cols # cursor jump size
+    dx_min = np.zeros(J)
+    for j in range(J):
+        is_valid = np.isfinite(x[j])
+        mm = (is_valid).nonzero()[0]
+        dx_min[j] = np.diff(x[j, mm]).min() # max zoom
+    dx_min = dx_min.min()
+
+    # Cursor color
+    cF = "\x1b[0m"
+
+    # States and flags
+    j_cursor = -1 # data rows the cursor should track (-1: all rows)
+    dj_cursor = 0 # change to j_cursor. not 0 is flag to change j_cursor
+    zoom_sf = 1.0 # scale factor. not 1.0 is flag to readjust view x axis
+    jump_sf = 0.0 # cursor jump scale factor. not 0.0 is flag to jump
+    recenter = False # flag to center the view on the cursor position
+    reclamp = True # flag to readjust view y axis
+    recursor = True # flag to update cursor column and data readout
+    remap = True # flag to remap the data to the canvas
+    invalid = False # flag that input was invalid
+    individual = False # flag to show an individual curve
+    first = True # flag that this is the first draw
+    tupdate = 0.0 # average time to update drawing
+    report = False # flag to display report data, like update time
+    redraw = False # flag to redraw the whole canvas
 
-    # Map x and y to the expanded canvas, M, and the color matrix, F.
-    M, F = data_to_matrix(x, y, view, tws)
+    while True:
+        # Skip if last input was invalid.
+        if invalid:
+            invalid = False
+            continue
 
-    # Convert the expanded canvas, M, to a matrix of character values, C.
-    C = matrix_to_braille(M) if config.uni else matrix_to_ascii(M)
+        # Start update timer.
+        tic = time.perf_counter()
 
-    # Set the deltas based on what is not a white-space character.
-    s = 0x2800 if config.uni else 0x20 # white-space character
-    D = (C != s) # wherever C is not a white space
-    D[:, ccol] = True # wherever the cursor is
+        # Cycle the cursor state.
+        if dj_cursor != 0:
+            # Cycle the j_cursor.
+            j_cursor += dj_cursor
+            if j_cursor < -1:
+                j_cursor = J - 1
+            elif j_cursor > J - 1:
+                j_cursor = -1
+            # Get the cursor color.
+            cF = "\x1b[0m" if j_cursor == -1 else \
+                    f"\x1b[38;5;{config.darks[j_cursor % COLOR_CNT]}m"
+            # Flags
+            reclamp = True # readjust the view y axis
+            recursor = True # update cursor column and data readout
+            dj_cursor = 0 # reset
+
+        # Readjust the view x axis. (Skip if already zoomed out.)
+        if (zoom_sf != 1.0):
+            x_span = view.x_max - view.x_min
+            if ((zoom_sf < 1) and (x_span > dx_min)) \
+                    or ((zoom_sf > 1) and ((view.x_min > lims.x_min)
+                    or (view.x_max < lims.x_max))):
+                # Adjust the x-axis of the view.
+                p = 0.75*(xc - view.x_min)/x_span + 0.25*(0.5)
+                x_span *= zoom_sf # change to the new span
+                if x_span < dx_min:
+                    x_span = dx_min
+                view.x_min = xc - p*x_span
+                view.x_max = view.x_min + x_span
+                # Limit the view x axis values.
+                limit_view_x(view, lims)
+                # Reposition the view indices.
+                if zoom_sf < 1:
+                    zoom_in_indices(x, view)
+                else:
+                    zoom_out_indices(x, view)
+                # Adjust the cursor jump size.
+                dx = (view.x_max - view.x_min)/tws.cols
+                # Flags
+                reclamp = True # trigger adjusting the view y axis
+                recursor = True # update cursor column and data readout
+                remap = True # trigger remapping of data to canvas
+            zoom_sf = 1.0 # reset
+
+        # Jump the cursor to the new x position.
+        if jump_sf != 0.0:
+            xc, k_xc = move_cursor(xc, jump_sf*dx, x, view, tws, j_cursor)
+            if (xc < view.x_min) or (xc > view.x_max): # if out of view
+                recenter = True # center the view on the cursor position
+            # Flags
+            recursor = True # update cursor column and data readout
+            jump_sf = 0.0 # reset
+
+        # Recenter the view on the cursor.
+        if recenter:
+            # Center the view.
+            center_view_x(xc, view) # center view on cursor
+            # Limit the view x axis values.
+            limit_view_x(view, lims) # limit the view x axis
+            # Reposition the view indices.
+            pan_indices(x, view)
+            # Flags
+            recursor = True # update cursor column and data readout
+            reclamp = True # readjust the view y axis
+            remap = True # remap data to canvas
+            recenter = False # reset
+
+        # Readjust the view y axis.
+        if reclamp:
+            # Set view y axis based on selected data sets.
+            view = get_view_y(x, y, view, j_cursor)
+            row_zero, view = get_row_zero(view, tws)
+            # Flags
+            remap = True # remap the data to the canvas
+            reclamp = False # reset
 
-    # Get the ranges text.
-    ranges = f"({ftostr(lims.x_min)}:{ftostr(lims.x_max)}, " \
-            + f"{ftostr(lims.y_min)}:{ftostr(lims.y_max)})"
+        # Redraw the canvas.
+        if redraw:
+            # Clear the screen
+            print("\x1b[2J")
+            # Get the current screen size.
+            tws = screen_size(rows, cols)
+            # Set all characters to refresh.
+            D = np.ones((tws.rows, tws.cols), dtype=bool)
+            # Redefine the cursor jump size.
+            dx = (view.x_max - view.x_min)/tws.cols
+            # Flags
+            recursor = True # reposition the cursor
+            remap = True # remap the data to the canvas
+            redraw = False # reset
 
-    # Draw the data to the canvas.
-    redraw_graph(C, D, ranges, label, F, ccol, cstr, cF, view, lims)
+        # Update cursor column and data readout.
+        if recursor:
+            # Get the cursor column.
+            ccol = get_column(xc, view, tws)
+            # Get the range of y values at the cursor.
+            yc_min, yc_max = get_cursor_y(x, y, view, tws, ccol, j_cursor)
+            cstr = ""
+            if (J == 1) or (j_cursor != -1):
+                cstr += f"[{k_xc}] "
+            if yc_min == yc_max:
+                cstr += f"({ftostr(xc)}, {ftostr(yc_max)})"
+            else:
+                cstr += f"({ftostr(xc)}, {ftostr(yc_min)}:{ftostr(yc_max)})"
+            # Mark the new cursor column for redraw.
+            D[:, ccol] = True # wherever the cursor is now
+            # Flags
+            recursor = False # reset
 
-    # --------------------------------
-    # Cycle through the state machine.
-    # --------------------------------
-
-    jump_sf = 0.0 # cursor jump scale factor
-    zoom_sf = 1.0 # scale factor
-    recursor = False
-    remap = False
+        # Remap the data to the canvas.
+        if remap:
+            # Map x and y to the expanded canvas, M, and the color matrix, F.
+            if individual:
+                M, F = data_to_matrix(x, y, view, tws, j_cursor)
+            else:
+                M, F = data_to_matrix(x, y, view, tws, -1)
+            # Convert expanded canvas, M, to a matrix of character values, C.
+            C = matrix_to_braille(M) if config.uni else matrix_to_ascii(M)
+            D = D | (C != s) # wherever C is not a white space
+            # Rebuild the view string.
+            view_str = f"({ftostr(view.x_min)}:{ftostr(view.x_max)}, " \
+                    + f"{ftostr(view.y_min)}:{ftostr(view.y_max)})"
+            # Flags
+            remap = False # reset
+
+        # Redraw the canvas.
+        if first:
+            redraw_graph(C, D, F, row_zero, view_str, label,
+                    -ccol, cstr, cF, view, lims)
+            first = False
+        else:
+            if report:
+                rstr = view_str + f" < t:{tupdate:4f} >"
+                #rstr = view_str + f" < {view.tmp}, {K} >"
+                redraw_graph(C, D, F, row_zero, rstr, label,
+                        ccol, cstr, cF, view, lims)
+            else:
+                redraw_graph(C, D, F, row_zero, view_str, label,
+                        ccol, cstr, cF, view, lims)
+        D = (C != s) # wherever C is not a white space
+        D[:, ccol] = True # wherever the cursor is
+
+        # Stop timer and average time to update.
+        tupdate = 0.99*tupdate + 0.01*(time.perf_counter() - tic)
 
-    while True:
         # Read a character. Wait for input.
         char = sys.stdin.read(1)
 
-        # Exit on 'q', 'x', delete, new line, or carriage return.
-        if (char == 'q') or (char == 'x') or \
-                (char == '\x7f') or (char == '\n') or (char == '\r'):
+        # Exit on "q", "x", backspace, new line, or carriage return.
+        if (char == "q") or (char == "x") or \
+                (char == "\x7f") or (char == "\n") or (char == "\r"):
             break
-        #else:
-        #    print(char)
-        #    continue
 
         # Interpret the shortcut keys pressed.
-        if char == '\x1b': # escape
+        if char == "\x1b": # escape
             char = sys.stdin.read(1)
-            if char == '[': # CSI
+            if char == "[": # CSI
                 char = sys.stdin.read(1)
-                if char == 'A': # slow zoom out
+                if char == "A": # slow zoom out
                     zoom_sf = 1.4142135623730950488
-                elif char == 'B': # slow zoom in
+                elif char == "B": # slow zoom in
                     zoom_sf = 0.70710678118654752440
-                elif char == 'C': # slow right
+                elif char == "C": # slow right
                     jump_sf = 1.0
-                    recursor = True
-                elif char == 'D': # slow left
+                elif char == "D": # slow left
                     jump_sf = -1.0
-                    recursor = True
-                elif char == '1': # possible shift arrow
+                elif char == "1": # possible shift arrow
                     chars = sys.stdin.read(3)
-                    if chars == ';2A': # fast zoom out
+                    if chars == ";2A": # fast zoom out
                         zoom_sf = 4.0
-                    elif chars == ';2B': # fast zoom in
+                    elif chars == ";2B": # fast zoom in
                         zoom_sf = 0.25
-                    elif chars == ';2C': # fast right
+                    elif chars == ";2C": # fast right
                         jump_sf = 10.0
-                        recursor = True
-                    elif chars == ';2D': # fast left
+                    elif chars == ";2D": # fast left
                         jump_sf = -10.0
-                        recursor = True
                     else: # unrecognized escape sequence
                         termios.tcflush(sys.stdin, termios.TCIFLUSH)
-                        continue
+                        invalid = True
                 else: # unrecognized escape sequence
                     termios.tcflush(sys.stdin, termios.TCIFLUSH)
-                    continue
+                    invalid = True
             else: # unrecognized escape sequence
                 termios.tcflush(sys.stdin, termios.TCIFLUSH)
-                continue
-        elif (char == 'l') or (char == 'd'): # slow right
+                invalid = True
+        elif (char == "l") or (char == "d"): # slow right
             jump_sf = 1.0
-            recursor = True
-        elif (char == 'h') or (char == 'a'): # slow left
+        elif (char == "h") or (char == "a"): # slow left
             jump_sf = -1.0
-            recursor = True
-        elif (char == 'L') or (char == 'D'): # fast right
+        elif (char == "L") or (char == "D"): # fast right
             jump_sf = 10.0
-            recursor = True
-        elif (char == 'H') or (char == 'A'): # fast left
+        elif (char == "H") or (char == "A"): # fast left
             jump_sf = -10.0
-            recursor = True
-        elif (char == 'k') or (char == 'w'): # slow zoom out
+        elif (char == "k") or (char == "w"): # slow zoom out
             zoom_sf = 1.4142135623730950488
-        elif (char == 'j') or (char == 's'): # slow zoom in
+        elif (char == "j") or (char == "s"): # slow zoom in
             zoom_sf = 0.70710678118654752440
-        elif (char == 'K') or (char == 'W'): # fast zoom out
+        elif (char == "K") or (char == "W"): # fast zoom out
             zoom_sf = 4.0
-        elif (char == 'J') or (char == 'S'): # fast zoom in
+        elif (char == "J") or (char == "S"): # fast zoom in
             zoom_sf = 0.25
-        elif char == 'n':
-            cstate = cstate + 1 if cstate < J - 1 else -1
-            recursor = True
-        elif char == 'p':
-            cstate = cstate - 1 if cstate > -1 else J - 1
-            recursor = True
-        elif (char == 'c') or (char == 'z'):
-            view = center_view(xc, view)
-            view = limit_view(view, lims)
-            recursor = True
-            remap = True
-        elif char == 'g':
+        elif char == "n":
+            dj_cursor = 1
+        elif char == "p":
+            dj_cursor = -1
+        elif (char == "c") or (char == "z"):
+            recenter = True
+        elif char == "g":
             jump_sf = (lims.x_min - xc)/dx
-            recursor = True
-        elif char == 'G':
+        elif char == "G":
             jump_sf = (lims.x_max - xc)/dx
+        elif char == "i":
+            individual = not individual
+            reclamp = True
             recursor = True
+            remap = True
+        elif char == "r":
+            redraw = True
+        elif char == "t":
+            report = not report
         else:
-            continue
-
-        # Process the zoom scaling factor.
-        if zoom_sf != 1.0:
-            if (zoom_sf > 1) and (view.x_min == lims.x_min) \
-                    and (view.x_max == lims.x_max): # skip if zoomed out
-                pass
-            else:
-                # Adjust the x-axis of the view.
-                x_span = view.x_max - view.x_min
-                p = 0.75*(xc - view.x_min)/x_span + 0.25*(0.5)
-                x_span *= zoom_sf # change to the new span
-                view.x_min = xc - p*x_span
-                view.x_max = view.x_min + x_span
-                # Adjust the y-axis of the view.
-                x_set = x if cstate == -1 else x[cstate:cstate+1]
-                y_set = y if cstate == -1 else y[cstate:cstate+1]
-                view = get_view_y(x_set, y_set, view)
-                # Limit the view and adjust the cursor jump size.
-                view = limit_view(view, lims)
-                dx = (view.x_max - view.x_min)/tws.cols
-                recursor = True # update the cursor
-                remap = True # remap the data to the canvas
-            zoom_sf = 1.0 # reset the zoom scale factor
-
-        # Update the cursor.
-        if recursor:
-            if cstate == -1:
-                x_set = x
-                y_set = y
-                cF = "\x1b[0m"
-            else:
-                x_set = x[cstate:cstate+1]
-                y_set = y[cstate:cstate+1]
-                cF = f"\x1b[38;5;{NORMAL_COLORS[cstate % COLOR_CNT]}m"
-            if jump_sf != 0.0:
-                xc = move_cursor(xc, jump_sf*dx, x_set)
-                jump_sf = 0.0 # reset the cursor jump scale factor
-            if (xc < view.x_min) or (xc > view.x_max):
-                # Adjust the view to center on xc.
-                view = center_view(xc, view)
-                # Adjust the y-axis of the view.
-                view = get_view_y(x_set, y_set, view)
-                # Limit the view and adjust the cursor jump size.
-                view = limit_view(view, lims)
-                remap = True
-            ccol = get_column(xc, view, tws)
-            yc_min, yc_max = get_cursor_y(ccol, tws, x_set, y_set, view)
-            if yc_min == yc_max:
-                cstr = f"({ftostr(xc)}, {ftostr(yc_max)})" # cursor readout
-            else:
-                cstr = f"({ftostr(xc)}, " \
-                        + f"{ftostr(yc_min)}:" \
-                        + f"{ftostr(yc_max)})" # cursor readout
-            D[:, ccol] = True # wherever the cursor is now
-            recursor = False
-
-        # Remap the data to the canvas.
-        if remap:
-            # Map x and y to the expanded canvas, M, and the color matrix, F.
-            M, F = data_to_matrix(x, y, view, tws)
-
-            # Convert expanded canvas, M, to a matrix of character values, C.
-            C = matrix_to_braille(M) if config.uni else matrix_to_ascii(M)
-            D = D | (C != s) # wherever C is not a white space
-
-            # Rebuild the ranges string.
-            ranges = f"({ftostr(view.x_min)}:{ftostr(view.x_max)}, " \
-                    + f"{ftostr(view.y_min)}:{ftostr(view.y_max)})"
-            remap = False
-
-        # Redraw the canvas.
-        redraw_graph(C, D, ranges, label, F, ccol, cstr, cF, view, lims)
-        D = (C != s) # wherever C is not a white space
-        D[:, ccol] = True # wherever the cursor is
+            invalid = True
 
     # Restore terminal settings
     termios.tcsetattr(0, termios.TCSADRAIN, persistent.orig_term_attr)
 
     # Newline and show the cursor.
-    sys.stdout.write("\r\033[?25h")
-    sys.stdout.flush()
+    print("\r\x1b[?25h", end="", flush=True)
 
 
-def bars(x, labels=None, cols=1, fat=False):
+def plot(x, y=None, label=None, rows=1, cols=1,
+        equal_axes=False, lg=None, overlay=False):
     """
-    Create a bar graph of the data in `x` using the `labels` for each element
-    of `x`.
+    Create a text-based plot of the path defined by (`x`, `y`) using characters.
+    If the size of the terminal can be found, that will be used for sizing the
+    plot. Otherwise, the default dimensions (config.cols, config.rows) will be
+    used. Note that this function does not plot connecting lines, only the
+    points specified by the (`x`, `y`) pairs.
 
     Parameters
     ----------
-    x : float array like
-        Set of values to plot as a bar graph.
-    labels : string list, default None
-        List of strings. This should be the same length as `x`.
+    x : (K,) or (J, K) np.ndarray
+        Array of x-axis values or matrix of rows of x-axis values.
+    y : (K,) or (J, K) np.ndarray, default None
+        Array of y-axis values or matrix of rows of y-axis values. If `y` is not
+        provided, `x` will be used as the `y` array and `x` will be defined to
+        be an array of indices (starting at zero).
+    label : str, default ""
+        Text to place at top of the plot, centered in the border.
+    rows : int, default 1
+        Desired number of rows if greater than 1 or fraction of existing rows if
+        less than 1.
     cols : int, default 1
         Desired number of columns if greater than 1 or fraction of window
         columns if less than 1.
-    fat : bool, default False
-        Use thicker characters for the progress bar.
+    equal_axes : bool, default False
+        Flag to apply equal axis scaling to the x and y axes. Because the
+        appearance of proportionality is affected by the particular font chosen
+        and the settings of the terminal emulator being used, the effective
+        aspect ratio of the characters can be set with `itrm.config.ar`.
+    lg : str, default None
+        Logarithmic scaling of axes. If `None`, both axes will have linear
+        scaling. Otherwise, `lg` should be a string: "x", "y", or "xy".
+    overlay : bool, default False
+        Flag to print new plot on top of a previous plot.
+
+    Notes
+    -----
+    Non-finite values will be ignored.
     """
 
-    # Get the terminal window size.
-    try: # Try to get the true size.
-        term_cols, _ = os.get_terminal_size()
-        term_cols -= 1
-        colorize = True
-    except: # If getting terminal size fails, use default values.
-        term_cols = config.cols
-        colorize = False
+    # Set signal handler for Ctrl+C
+    signal.signal(signal.SIGINT, signal_handler)
 
-    # Convert a fractional `cols` to columns.
-    if cols <= 1:
-        cols = max(round(term_cols * cols), 18)
+    # Check and (possibly) adjust the shapes of x and y.
+    x, y = shape_xy(x, y)
 
-    # Get the width of labels.
-    label_width = 0
-    if labels is not None:
-        label_width = max([len(l) for l in labels])
+    # Hide the cursor.
+    print("\x1b[?25l", end="", flush=True)
 
-    # Adjust the total width to make room for labels.
-    width = cols - label_width - 2
-    if width < 1:
-        width = 1
+    # Choose the canvas size.
+    tws = screen_size(rows, cols)
+    if overlay and (persistent.rows_last is not None):
+        print(f"\x1b[{persistent.rows_last + 2}A", end="", flush=True)
+    persistent.rows_last = tws.rows
 
-    # For each value of x, print the bar.
-    span = max(x) - 0
-    for n in range(len(x)):
-        if labels is None:
-            print(" |", end='')
+    # Apply logarithmic scaling.
+    if lg is not None:
+        if not isinstance(lg):
+            raise ValueError(f"lg must be None or a string: {lg}")
+        lg = lg.lower()
+        if lg == "x":
+            x = np.where(np.isfinite(x) & (x > 0), np.log10(x), np.nan)
+        elif lg == "y":
+            y = np.where(np.isfinite(y) & (y > 0), np.log10(y), np.nan)
+        elif (lg == "xy") or (lg == "yx"):
+            x = np.where(np.isfinite(x) & (x > 0), np.log10(x), np.nan)
+            y = np.where(np.isfinite(y) & (y > 0), np.log10(y), np.nan)
         else:
-            sstr = " " * (label_width - len(labels[n]))
-            print(f"{sstr}{labels[n]} |", end='')
-        ratio = x[n]/span
-        draw_bar(width*ratio, width, colorize, fat)
-        print("", flush=True)
+            raise ValueError(f"lg should be 'x', 'y', or 'xy': {lg}")
+
+    # Get the data limits, adjusting for the terminal window size.
+    lims = limits_xy(x, y, tws, equal_axes)
+    row_zero, lims = get_row_zero(lims, tws)
+
+    # Map x and y to the expanded canvas, M, and the foreground color matrix, F.
+    colorize = -1 if istty() else None
+    M, F = data_to_matrix(x, y, lims, tws, colorize)
+
+    # Convert the expanded matrix, M, to a matrix of character values, C.
+    C = matrix_to_braille(M) if config.uni else matrix_to_ascii(M)
+
+    # Get the view text.
+    view_str = f"({ftostr(lims.x_min)}:{ftostr(lims.x_max)}, " \
+            + f"{ftostr(lims.y_min)}:{ftostr(lims.y_max)})"
+
+    # Draw the plot.
+    draw_graph(C, view_str, label, F, row_zero)
+
+    # Show the cursor.
+    print("\x1b[?25h", end="", flush=True)
 
 
 def heat(matrix):
     """
     Create a surface plot using the input `matrix`. The rows are printed in
     reverse order.
+
+    Notes
+    -----
+    This function uses the 24 shades of gray at the end of the 8-bit color
+    table. Although there are 6 more "shades" of gray including true black and
+    true white between color codes 16 and 231, these do not fit into the
+    uniform spacing of the 24. True white makes a larger leap leap from the
+    rest of all the grays (17) than the usual interval (10) among the 24.
+    Therefore, given the slight benefit and the increased complexity, the 6
+    additional grays were not included.
     """
 
+    # Get the terminal window size.
+    try: # Try to get the true size.
+        term_cols, _ = os.get_terminal_size()
+        term_cols -= 1
+    except: # If getting terminal size fails, use default values.
+        term_cols = config.cols
+
     # Scale the matrix.
     m_min = np.min(matrix)
     m_max = np.max(matrix)
     M = np.round((matrix - m_min)/(m_max - m_min)*23).astype(int) + 232
     rows, cols = M.shape
 
+    # Stop if the terminal window is not wide enough.
+    if cols > term_cols:
+        raise ValueError("The terminal window is too small for "
+                + f"this heat map: {cols} > {term_cols}")
+
     # Print the matrix.
     if config.uni:
         for row in range(0, (rows - rows%2), 2):
             for col in range(cols):
                 print("\x1b[38;5;%dm\x1b[48;5;%dm\u2580" %
-                        (M[row, col], M[row + 1, col]), end='', flush=True)
+                        (M[row, col], M[row + 1, col]), end="", flush=True)
             print("\x1b[0m", flush=True)
         if rows % 2 == 1:
             for col in range(cols):
-                print("\x1b[38;5;%dm\u2580" % (M[-1, col]), end='', flush=True)
+                print("\x1b[38;5;%dm\u2580" % (M[-1, col]), end="", flush=True)
             print("\x1b[0m", flush=True)
     else:
         for row in range(rows):
             for col in range(cols):
-                print("\x1b[48;5;%dm  " % (M[row, col]), end='')
+                print("\x1b[48;5;%dm  " % (M[row, col]), end="")
             print("\x1b[0m")
 
 
-def table(matrix, head=None, left=None, width=10, sep='  '):
+def sparsity(matrix, label=None):
+    """
+    Print the sparsity of a matrix. Note, if you are using SciPy sparse arrays
+    or matrices, use the method `toarray()` on the input to this function.
+    """
+
+    # Get the terminal window size.
+    try: # Try to get the true size.
+        term_cols, _ = os.get_terminal_size()
+        term_cols -= 1
+    except: # If getting terminal size fails, use default values.
+        term_cols = config.cols
+
+    # Stop if the terminal window is not wide enough.
+    cols = matrix.shape[1]
+    if cols > term_cols:
+        raise ValueError("The terminal window is too small for "
+                + f"this sparsity map: {cols} > {term_cols}")
+
+    # Convert matrix to zeros and ones.
+    M = (np.abs(matrix) > eps).astype(int)
+
+    # Convert the large matrix to a smaller matrix of character values.
+    C = matrix_to_braille(M) if config.uni else matrix_to_stars(M)
+
+    # Create the shape string.
+    shape_str = f"{matrix.shape[0]}x{matrix.shape[1]}"
+
+    # Draw the plot.
+    draw_graph(C, shape_str, label)
+
+
+def table(matrix, head=None, left=None, width=10, sep="  "):
     """
     Print a table to the terminal.
 
     Parameters
     ----------
     matrix : list of lists of values
         Table of values.
     head : list of strings, default []
         List of header labels.
     left : list of strings, default []
         List of left-most column labels.
     width : int, default 10
         Width in characters of each cell.
-    sep : string, default '   '
+    sep : string, default "  "
         String separating columns.
     """
 
     # -----------------
     # Check the inputs.
     # -----------------
 
@@ -568,35 +726,35 @@
         if not is_2d:
             matrix = [matrix]
     elif isinstance(matrix, np.ndarray):
         matrix = matrix.tolist()
         if not isinstance(matrix[0], list):
             matrix = [matrix]
     else:
-        raise Exception('heat: matrix must be a list!')
+        raise Exception("heat: matrix must be a list!")
 
     # Check the type of head.
     if head is None:
         head = []
     elif isinstance(head, (str, float, int)):
         head = [head]
     elif isinstance(head, np.ndarray):
         head = head.tolist()
     elif not isinstance(head, list):
-        raise Exception('heat: head must be a list!')
+        raise Exception("heat: head must be a list!")
 
     # Check the type of left.
     if left is None:
         left = []
     elif isinstance(left, (str, float, int)):
         left = [left]
     elif isinstance(left, np.ndarray):
         left = left.tolist()
     elif not isinstance(left, list):
-        raise Exception('heat: left must be a list!')
+        raise Exception("heat: left must be a list!")
 
     # Check that width is within 3 to 30.
     if width < 6:
         width = 6
     elif width > 30:
         width = 30
 
@@ -669,19 +827,19 @@
         width in characters equal to `width`.
         """
 
         if isinstance(C, str):
             L = len(C)
             if L > width:
                 L = width - 3
-                return C[:L] + '...'
+                return C[:L] + "..."
             elif L == width:
                 return C
             else:
-                return ' '*(width-L) + C
+                return " "*(width-L) + C
         elif isinstance(C, float):
             return f2str(C, width)
         else:
             return f2str(float(C), width)
 
     if len(head) > 0:
         row_str = ""
@@ -715,31 +873,66 @@
         for n_col, val in enumerate(vals):
             if n_col > 0:
                 row_str += sep
             row_str += fixed_width_string(val, width)
         print(row_str)
 
 
-def sparsity(matrix, label=''):
+def bars(x, labels=None, cols=1, fat=False):
     """
-    Print the sparsity of a matrix. Note, if you are using SciPy sparse arrays
-    or matrices, use the method `toarray()` on the input to this function.
+    Create a bar graph of the data in `x` using the `labels` for each element
+    of `x`.
+
+    Parameters
+    ----------
+    x : float array like
+        Set of values to plot as a bar graph.
+    labels : string list, default None
+        List of strings. This should be the same length as `x`.
+    cols : int, default 1
+        Desired number of columns if greater than 1 or fraction of window
+        columns if less than 1.
+    fat : bool, default False
+        Use thicker characters for the progress bar.
     """
 
-    # Convert matrix to zeros and ones.
-    M = (np.abs(matrix) > 1e-30).astype(int)
+    # Get the terminal window size.
+    try: # Try to get the true size.
+        term_cols, _ = os.get_terminal_size()
+        term_cols -= 1
+        colorize = True
+    except: # If getting terminal size fails, use default values.
+        term_cols = config.cols
+        colorize = False
 
-    # Convert the large matrix to a smaller matrix of character values.
-    C = matrix_to_braille(M) if config.uni else matrix_to_stars(M)
+    # Convert a fractional `cols` to columns.
+    if cols <= 1:
+        cols = max(round(term_cols * cols), 18)
 
-    # Create the shape string.
-    shape_str = f"{matrix.shape[0]}x{matrix.shape[1]}"
+    # Get the width of labels.
+    label_width = 0
+    if labels is not None:
+        label_width = max([len(l) for l in labels])
 
-    # Draw the plot.
-    draw_graph(C, shape_str, label)
+    # Adjust the total width to make room for labels.
+    width = cols - label_width - 2
+    if width < 1:
+        width = 1
+
+    # For each value of x, print the bar.
+    span = max(x) - 0
+    for n in range(len(x)):
+        if labels is None:
+            print(" |", end="")
+        else:
+            sstr = " " * (label_width - len(labels[n]))
+            print(f"{sstr}{labels[n]} |", end="")
+        ratio = x[n]/span
+        draw_bar(width*ratio, width, colorize, fat)
+        print("", flush=True)
 
 
 def progress(k, K, t_init=None, cols=1, fat=False):
     """
     Output a simple progress bar with percent complete to the terminal. When `k`
     equals `K - 1`, the progress bar will complete and start a new line.
 
@@ -795,43 +988,44 @@
     else:
         clk_str = ""
 
     # Maximum length of bar
     N = cols - 5 - len(clk_str)
 
     # Build the progress bar.
-    print(f"\r{int(100*ratio):3d}% ", end='')
+    print(f"\r{int(100*ratio):3d}% ", end="")
     draw_bar(N*ratio, N, colorize, fat)
     if k + 1 >= K:
         print(f"{clk_str}", flush=True)
     else:
-        print(f"{clk_str}", end='', flush=True)
+        print(f"{clk_str}", end="", flush=True)
 
 # -----------------
 # Support functions
 # -----------------
 
 def signal_handler(sig, frame):
     # Restore terminal settings
-    termios.tcsetattr(0, termios.TCSADRAIN, persistent.orig_term_attr)
+    if persistent.orig_term_attr is not None:
+        termios.tcsetattr(0, termios.TCSADRAIN, persistent.orig_term_attr)
 
     # Newline and show the cursor.
-    sys.stdout.write("\r\033[?25h")
+    sys.stdout.write("\r\x1b[?25h")
     sys.stdout.flush()
 
     # Exit.
     sys.exit(0)
 
 
 def istty():
     """
     Try to determine if the current standard output is a teletype output. If it
     is we might assume it can handle ANSI escape codes.
     """
-    is_tty = hasattr(sys.stdout, 'isatty') and sys.stdout.isatty()
+    is_tty = hasattr(sys.stdout, "isatty") and sys.stdout.isatty()
     return is_tty
 
 
 def screen_size(rows, cols):
     # Get the terminal window size.
     try: # Try to get the true size.
         term_cols, term_rows = os.get_terminal_size()
@@ -860,15 +1054,14 @@
         subrows = 4
     else:
         subcols = 1
         subrows = 3
 
     # Load the dimensions into an object.
     tws = term_ws(rows, cols, subrows, subcols)
-    persistent.rows_last = rows
 
     return tws
 
 
 def shape_xy(x, y):
     # If only `x` is provided, copy to `y`
     # and make `x` an array of integers.
@@ -911,232 +1104,406 @@
             raise ValueError("x and y must have 1 or the same number of rows.")
     if Kx != Ky:
         raise ValueError("x and y must have the same number of columns.")
 
     return x, y
 
 
-def limits_xy(x, y, tws, equal):
+def limits_xy(x, y, tws, equal_axes):
     # Get the data shape and array of indices.
     J, K = x.shape
     nn = np.arange(K)
 
+    # Initialize the minimum and maximum index arrays.
+    k_min = np.zeros(J, dtype=int)
+    k_max = np.zeros(J, dtype=int)
+
     # Get the limits.
     x_min = np.inf; x_max = -np.inf
     y_min = np.inf; y_max = -np.inf
     # For each row of data,
     for j in range(J):
-        # Get this curve.
-        xj = x[j].copy()
-        yj = y[j].copy()
-
         # Find the valid points by index.
-        nn_valid = np.intersect1d(nn[np.isfinite(xj)], nn[np.isfinite(yj)])
+        nn_valid = np.intersect1d(nn[np.isfinite(x[j])], nn[np.isfinite(y[j])])
+
+        # Save the indices of the minimum and maximum.
+        k_min[j] = nn_valid[x[j, nn_valid].argmin()]
+        k_max[j] = nn_valid[x[j, nn_valid].argmax()]
 
         # Expand the limits.
-        x_min = min(x_min, np.min(xj[nn_valid]))
-        x_max = max(x_max, np.max(xj[nn_valid]))
-        y_min = min(y_min, np.min(yj[nn_valid]))
-        y_max = max(y_max, np.max(yj[nn_valid]))
+        x_min = min(x_min, x[j, k_min[j]])
+        x_max = max(x_max, x[j, k_max[j]])
+        y_min = min(y_min, np.min(y[j, nn_valid]))
+        y_max = max(y_max, np.max(y[j, nn_valid]))
 
     # Enforce differentiation.
-    eps = 1e-16
     if x_min == x_max:
         x_min -= eps
         x_max += eps
     if y_min == y_max:
         y_min -= eps
         y_max += eps
 
     # Apply axis scaling.
-    if equal != 0:
-        x_scale = (1/config.ar)*cols/(x_max - x_min)
+    if equal_axes:
+        x_scale = (tws.cols*config.ar)/(x_max - x_min)
         y_scale = tws.rows/(y_max - y_min)
-        if x_scale*equal < y_scale:
-            y_scale = x_scale*equal
+        if x_scale < y_scale:
+            y_scale = x_scale
             y_span = tws.rows/y_scale
             y_mid = (y_max + y_min)*0.5
             y_min = y_mid - y_span*0.5
             y_max = y_mid + y_span*0.5
-        elif y_scale < x_scale*equal:
-            x_scale = y_scale/equal
-            x_span = (1/config.ar)*cols/x_scale
+        elif y_scale < x_scale:
+            x_scale = y_scale
+            x_span = (tws.cols*config.ar)/x_scale
             x_mid = (x_max + x_min)*0.5
             x_min = x_mid - x_span*0.5
             x_max = x_mid + x_span*0.5
 
+    # Put limits into an object.
+    lims = limits(x_min, x_max, y_min, y_max, k_min, k_max)
+
+    return lims
+
+
+def get_row_zero(lims, tws):
     # Expand the limits to align zero with the nearest half row so that the zero
     # marker is true. FIXME This formula is likely wrong!
-    if (y_min < 0) and (y_max > 0):
+    if (lims.y_min < 0) and (lims.y_max > 0):
         idx_zero = round((tws.rows - 1.0/tws.subrows)
-            * y_max/(y_max - y_min) - 0.5)*tws.subrows + tws.subrows/2
-        slope = max((tws.subrows*tws.rows - 1 - idx_zero)/y_min,
-            -idx_zero/y_max)
-        y_min = (tws.subrows*tws.rows - 1 - idx_zero)/slope
-        y_max = -idx_zero/slope
+                * lims.y_max/(lims.y_max - lims.y_min)
+                - 0.5)*tws.subrows + tws.subrows/2
+        slope = max((tws.subrows*tws.rows - 1 - idx_zero)/lims.y_min,
+                -idx_zero/lims.y_max)
+        lims.y_min = (tws.subrows*tws.rows - 1 - idx_zero)/slope
+        lims.y_max = -idx_zero/slope
         row_zero = math.floor((tws.rows - 1/tws.subrows)*
-                (y_max)/(y_max - y_min))
+                (lims.y_max)/(lims.y_max - lims.y_min))
     else:
         row_zero = -1
+    return row_zero, lims
 
-    # Put limits into an object.
-    lims = limits(x_min, x_max, y_min, y_max)
-
-    return lims, row_zero
 
+def data_to_matrix(x, y, view, tws, j_cursor):
+    """
+    Parameters
+    ----------
+    x : (J, K) np.ndarray
+        Matrix of x-axis values.
+    y : (J, K) np.ndarray
+        Matrix of y-axis values.
+    view : limits
+        Object holding the current view.
+    tws : term_ws
+        Object holding the terminal window size.
+    j_cursor : int or None
+        Colorization flag. If `None`, do not color anything. If -1, color all
+        rows of data. If 0 or more, only plot the data row indexed with
+        `j_cursor` and use its corresponding color.
+    """
 
-def data_to_matrix(x, y, view, tws):
-    # Get the shape of the data.
-    J, K = x.shape
-    x_span = view.x_max - view.x_min
-    y_span = view.y_max - view.y_min
+    # Get the span of the view. Limit to non-zero values.
+    x_span = max(eps, view.x_max - view.x_min)
+    y_span = max(eps, view.y_max - view.y_min)
 
     # Get total numbers of subrows and subcolumns.
     Rows = tws.subrows*tws.rows
     Cols = tws.subcols*tws.cols
 
-    # Check if colors are likely supported.
-    colorize = istty()
-
     # Initialize the data and color matrices.
     M = np.zeros((Rows, Cols), dtype=int)
-    if (J > 1) and (colorize):
-        F = np.zeros((tws.rows, tws.cols), dtype=int)
-    else:
+    if j_cursor is None:
         F = None
+    else:
+        F = np.zeros((tws.rows, tws.cols), dtype=int)
 
     # For each curve, set the points and colors.
-    kk = np.arange(K)
-    for j in range(J):
+    J = x.shape[0]
+    if (j_cursor is None) or (j_cursor == -1):
+        jj = np.arange(J)
+    else:
+        jj = np.array([j_cursor])
+    for j in jj:
         # Find the valid points by index.
-        x_valid = np.isfinite(x[j]) & \
-                (x[j] >= view.x_min) & (x[j] <= view.x_max)
-        y_valid = np.isfinite(y[j]) & \
-                (y[j] >= view.y_min) & (y[j] <= view.y_max)
-        kk_valid = np.intersect1d(kk[x_valid], kk[y_valid])
+        is_valid_x = np.isfinite(x[j])
+        is_valid_y = np.isfinite(y[j])
+        is_vis_x = (x[j] >= view.x_min) & (x[j] <= view.x_max)
+        is_vis_y = (y[j] >= view.y_min) & (y[j] <= view.y_max)
+        mm = (is_valid_x & is_valid_y & is_vis_x & is_vis_y).nonzero()[0]
 
         # Scale the data to dots. First dot is 0; last dot is Cols - 1.
-        X_jk = Cols*(x[j, kk_valid] - view.x_min)/x_span - 0.5
-        Y_jk = Rows*(view.y_max - y[j, kk_valid])/y_span - 0.5
-        X = np.clip(np.round(X_jk).astype(int), 0, Cols - 1)
-        Y = np.clip(np.round(Y_jk).astype(int), 0, Rows - 1)
+        X = Cols*(x[j, mm] - view.x_min)/x_span - 0.5
+        Y = Rows*(view.y_max - y[j, mm])/y_span - 0.5
+        X = np.clip(np.round(X).astype(int), 0, Cols - 1)
+        Y = np.clip(np.round(Y).astype(int), 0, Rows - 1)
 
         # Map locations to a large matrix.
         M[Y, X] = 1 # Puts a 1 wherever the curve coordinates are.
 
         # Scale the data to dots.
-        if (J > 1) and (colorize):
+        if F is not None:
             u = X//tws.subcols
             v = Y//tws.subrows
-            F[v, u] = NORMAL_COLORS[j % COLOR_CNT]
+            F[v, u] = config.darks[j % COLOR_CNT]
 
     return M, F
 
 
-def move_cursor(xc, dx, x):
-    # Get the target x value.
-    xcp = xc + dx
+def set_cursor(xc, x, view, tws):
+    # Initialize the arrays of indices.
+    J = x.shape[0]
 
-    # For each row, get the best-fit index in `x`.
-    J, K = x.shape
-    kkc = np.zeros(J, dtype=int)
+    # Align target xc with column center.
+    x_span = view.x_max - view.x_min
+    ccol = round(tws.cols*(xc - view.x_min)/x_span - 0.5)
+    xc = (ccol + 0.5)*x_span/tws.cols + view.x_min
+
+    # Get the closest `x` to `xc`.
+    view.k_xc = np.zeros(J, dtype=int)
     for j in range(J):
-        if dx > 0:
-            if x[j, -1] <= xcp:
-                kkc[j] = K - 1
-            else:
-                kkc[j] = np.where(x[j] >= xcp, x, np.inf).argmin()
-        elif dx < 0:
-            if x[j, 0] >= xcp:
-                kkc[j] = 0
-            else:
-                kkc[j] = np.where(x[j] <= xcp, x, -np.inf).argmax()
+        ka = view.k_min[j]
+        kb = view.k_max[j]
+        xj_view = x[j, ka:kb+1]
+        is_valid = np.isfinite(xj_view)
+        mm = (is_valid).nonzero()[0]
+        if len(mm) > 0:
+            view.k_xc[j] = np.abs(xj_view[mm] - xc).argmin() + ka
         else:
-            kkc[j] = np.abs(x[j] - xcp).argmin()
+            mm = (np.isfinite(x[j])).nonzero()[0]
+            view.k_xc[j] = np.abs(x[j, mm] - xc).argmin()
+    jc = np.abs(x[:, view.k_xc] - xc).argmin()
+    xc = x[jc, view.k_xc[jc]]
 
-    # Find closest match in `x`.
-    jc = np.abs(x[:, kkc] - xcp).argmin()
-    kc = kkc[jc]
-    xc = x[jc, kc]
+    return xc, view.k_xc[jc]
 
-    return xc
 
+# FIXME Sometimes the cursor still jumps more than one column.
+def move_cursor(xc, dx, x, view, tws, j_cursor):
+    # Get the target `xc` value.
+    xc += dx
 
-def limit_view(view, lims):
+    # Align target xc with column center.
+    x_span = view.x_max - view.x_min
+    ccol = round(tws.cols*(xc - view.x_min)/x_span - 0.5)
+    xc = (ccol + 0.5)*x_span/tws.cols + view.x_min
+
+    # Get the closest `x` to `xc`.
+    J, K = x.shape
+    if dx > 0:
+        for j in range(J):
+            k_max = np.nanargmax(x[j])
+            if x[j, k_max] <= xc:
+                view.k_xc[j] = k_max
+            elif x[j, view.k_max[j]] >= xc:
+                ka = view.k_xc[j] # previous cursor index
+                kb = view.k_max[j]
+                xj_right = x[j, ka:kb+1]
+                mm_right = (xj_right >= xc).nonzero()[0]
+                n = xj_right[mm_right].argmin()
+                view.k_xc[j] = mm_right[n] + ka
+            else:
+                ka = view.k_xc[j] # previous cursor index
+                xj_right = x[j, ka:]
+                mm_right = (xj_right >= xc).nonzero()[0]
+                n = xj_right[mm_right].argmin()
+                view.k_xc[j] = mm_right[n] + ka
+    else:
+        for j in range(J):
+            k_min = np.nanargmin(x[j])
+            if x[j, k_min] >= xc:
+                view.k_xc[j] = k_min
+            elif x[j, view.k_min[j]] <= xc:
+                ka = view.k_min[j]
+                kb = view.k_xc[j] # previous cursor index
+                xj_left = x[j, ka:kb+1]
+                mm_left = (xj_left <= xc).nonzero()[0]
+                n = xj_left[mm_left].argmax()
+                view.k_xc[j] = mm_left[n] + ka
+            else:
+                kb = view.k_xc[j] # previous cursor index
+                xj_left = x[j, :kb+1]
+                mm_left = (xj_left <= xc).nonzero()[0]
+                if len(mm_left) == 0:
+                    print(f"x[k_min]: {x[j, k_min]}, xc: {xc}, xj_left: {xj_left}")
+                n = xj_left[mm_left].argmax()
+                view.k_xc[j] = mm_left[n]
+    if j_cursor == -1:
+        jc = np.abs(x[:, view.k_xc] - xc).argmin()
+    else:
+        jc = j_cursor
+    xc = x[jc, view.k_xc[jc]]
+
+    return xc, view.k_xc[jc]
+
+
+def limit_view_x(view, lims):
+    # Limit the x-axis values of the view.
     x_span = view.x_max - view.x_min
     if view.x_min < lims.x_min:
         view.x_min = lims.x_min
-        view.x_max = view.x_min + x_span
-    if view.x_max > lims.x_max:
-        view.x_max = lims.x_max
-        view.x_min = view.x_max - x_span
-    if view.x_min < lims.x_min:
-        view.x_min = lims.x_min
-    if view.x_max > lims.x_max:
+        view.x_max = min(view.x_min + x_span, lims.x_max)
+    elif view.x_max > lims.x_max:
         view.x_max = lims.x_max
-    if view.y_min < lims.y_min:
-        view.y_min = lims.y_min
-    if view.y_max > lims.y_max:
-        view.y_max = lims.y_max
-    return view
+        view.x_min = max(view.x_max - x_span, lims.x_min)
+
+
+def zoom_in_indices(x, view):
+    # Update the arrays of indices of the view's x min and max.
+    J = x.shape[0]
+    for j in range(J):
+        # Get subset of `x` within the old view.
+        ka = view.k_min[j]
+        kb = view.k_max[j]
+        xj_view = x[j, ka:kb + 1]
+
+        # Get the new index of minimum.
+        mm_min = (xj_view >= view.x_min).nonzero()[0]
+        n = xj_view[mm_min].argmin()
+        view.k_min[j] = mm_min[n] + ka
+
+        # Get the new index of maximum.
+        mm_max = (xj_view <= view.x_max).nonzero()[0]
+        n = xj_view[mm_max].argmax()
+        view.k_max[j] = mm_max[n] + ka
+
+
+def zoom_out_indices(x, view):
+    # Update the arrays of indices of the view's x min and max.
+    J = x.shape[0]
+    for j in range(J):
+        # Get subsets of `x` left or right of the old view.
+        kb = view.k_min[j]
+        ka = view.k_max[j]
+        xj_left = x[j, :kb + 1]
+        xj_right = x[j, ka:]
+
+        # Get the new index of minimum.
+        mm_min = (xj_left >= view.x_min).nonzero()[0]
+        n = xj_left[mm_min].argmin()
+        view.k_min[j] = mm_min[n]
+
+        # Get the new index of maximum.
+        mm_max = (xj_right <= view.x_max).nonzero()[0]
+        n = xj_right[mm_max].argmax()
+        view.k_max[j] = mm_max[n] + ka
+
+
+def pan_indices(x, view):
+    # Update the arrays of indices of the view's x min and max.
+    J = x.shape[0]
+    for j in range(J):
+        # Get subsets of `x` left or right of the old view.
+        ka = view.k_min[j]
+        kb = view.k_max[j]
+        if (x[j, ka] >= view.x_min) and (x[j, kb] >= view.x_max): # <--
+            xj_min = x[j, :ka + 1];     k_min_ref = 0
+            xj_max = x[j, :kb + 1];     k_max_ref = 0
+        elif (x[j, ka] < view.x_min) and (x[j, kb] < view.x_max): # -->
+            xj_min = x[j, ka:];         k_min_ref = ka
+            xj_max = x[j, kb:];         k_max_ref = kb
+        elif (x[j, ka] >= view.x_min) and (x[j, kb] < view.x_max): # <->
+            xj_min = x[j, :ka + 1];     k_min_ref = 0
+            xj_max = x[j, kb:];         k_max_ref = kb
+        elif (x[j, ka] < view.x_min) and (x[j, kb] >= view.x_max): # >-<
+            xj_min = x[j, ka:kb + 1];   k_min_ref = ka
+            xj_max = x[j, ka:kb + 1];   k_max_ref = ka
+
+        # Get the new index of minimum.
+        mm_min = (xj_min >= view.x_min).nonzero()[0]
+        n = xj_min[mm_min].argmin()
+        view.k_min[j] = mm_min[n] + k_min_ref
+
+        # Get the new index of maximum.
+        mm_max = (xj_max <= view.x_max).nonzero()[0]
+        n = xj_max[mm_max].argmax()
+        view.k_max[j] = mm_max[n] + k_max_ref
 
 
-def center_view(xc, view):
+def center_view_x(xc, view):
     x_span = view.x_max - view.x_min
     view.x_min = xc - x_span/2
     view.x_max = view.x_min + x_span
-    return view
 
 def get_column(xc, view, tws):
     x_span = view.x_max - view.x_min
     ccol = round(tws.cols*(xc - view.x_min)/x_span - 0.5)
     ccol = min(max(ccol, 0), tws.cols - 1)
     return ccol
 
 
-def get_cursor_y(ccol, tws, x, y, view):
+def get_cursor_y(x, y, view, tws, ccol, j_cursor):
     # Get range of x values from left to right of cursor.
     x_span = view.x_max - view.x_min
     xc_a = x_span*(ccol/tws.cols) + view.x_min
     xc_b = xc_a + x_span/tws.cols
 
     # Initialize the y limits.
-    yc_min = np.inf
-    yc_max = -np.inf
+    y_min = np.inf
+    y_max = -np.inf
 
     # Search each row of (x, y).
-    J, K = x.shape
-    for j in range(J):
-        kc_a = np.where(x[j] >= xc_a, x, np.inf).argmin()
-        kc_b = np.where(x[j] <= xc_b, x, -np.inf).argmax()
-        y_min = y[j, kc_a:kc_b + 1].min()
-        y_max = y[j, kc_a:kc_b + 1].max()
-        yc_min = min(yc_min, y_min)
-        yc_max = max(yc_max, y_max)
+    J = x.shape[0]
+    jj = np.arange(J) if j_cursor == -1 else np.array([j_cursor])
+    for j in jj:
+        ka = view.k_min[j]
+        kb = view.k_max[j]
+        xj_view = x[j, ka:kb + 1]
+        yj_view = y[j, ka:kb + 1]
+        is_valid_x = np.isfinite(xj_view)
+        is_valid_y = np.isfinite(yj_view)
+        is_in = (xj_view >= xc_a) & (xj_view <= xc_b)
+        mm = (is_valid_x & is_valid_y & is_in).nonzero()[0]
+        if len(mm) == 0:
+            continue
+        yj_min = y[j, mm + ka].min()
+        yj_max = y[j, mm + ka].max()
+        y_min = min(y_min, yj_min)
+        y_max = max(y_max, yj_max)
+
+    # Check for no valid values.
+    if y_min == np.inf:
+        y_min = np.nan
+        y_max = np.nan
 
-    return yc_min, yc_max
+    return y_min, y_max
 
 
-def get_view_y(x, y, view):
+def get_view_y(x, y, view, j_cursor):
     # Initialize the y limits.
-    yv_min = np.inf
-    yv_max = -np.inf
+    y_min = np.inf
+    y_max = -np.inf
 
     # Search each row of (x, y).
-    J, K = x.shape
-    for j in range(J):
-        kc_a = np.where(x[j] >= view.x_min, x, np.inf).argmin()
-        kc_b = np.where(x[j] <= view.x_max, x, -np.inf).argmax()
-        y_min = y[j, kc_a:kc_b + 1].min()
-        y_max = y[j, kc_a:kc_b + 1].max()
-        yv_min = min(yv_min, y_min)
-        yv_max = max(yv_max, y_max)
+    J = x.shape[0]
+    jj = np.arange(J) if j_cursor == -1 else np.array([j_cursor])
+    for j in jj:
+        ka = view.k_min[j]
+        kb = view.k_max[j]
+        xj_view = x[j, ka:kb + 1]
+        yj_view = y[j, ka:kb + 1]
+        is_valid_x = np.isfinite(xj_view)
+        is_valid_y = np.isfinite(yj_view)
+        mm = (is_valid_x & is_valid_y).nonzero()[0]
+        if len(mm) == 0:
+            continue
+        yj_min = y[j, mm + ka].min()
+        yj_max = y[j, mm + ka].max()
+        y_min = min(y_min, yj_min)
+        y_max = max(y_max, yj_max)
+
+    # Check for no valid values.
+    if (y_min == np.inf):
+        y_min = -eps
+        y_max = eps
+
+    # Save the view's y-axis minimum and maximum.
+    view.y_min = y_min
+    view.y_max = y_max
 
-    view.y_min = yv_min
-    view.y_max = yv_max
     return view
 
 
 def ftostr(f):
     """ Convert a floating-point value to a string, without the useless `+` sign
     or leading zeros in the exponent. """
     return f"{f:0.6g}".replace("e+0", "e").replace("e-0", "e-")
@@ -1218,17 +1585,17 @@
         s = 0x20 # ASCII space
 
     # Replace zeros with spaces.
     C = np.where(C == 0, s, C)
 
     # Draw the top edge of the box.
     rows, cols = C.shape
-    print(b[0], end='', flush=True)
+    print(b[0], end="", flush=True)
     for col in range(cols):
-        print(b[1], end='', flush=True)
+        print(b[1], end="", flush=True)
     print(b[2], flush=True)
 
     # For each row of the matrix, draw the contents and two sides of the box.
     for row in range(rows):
         # Get the side characters.
         if row != row_zero:
             l = b[3]
@@ -1238,107 +1605,113 @@
             r = b[6]
 
         # Get this row of data.
         F_row = 0 if F is None else F[row]
         C_row = C[row]
 
         # Draw this row.
-        print(l + "\x1b[1m", end='', flush=True)
+        print(l + "\x1b[1m", end="", flush=True)
         f_last = 0
         for col in range(cols):
             # Get this column color.
             f = 0 if F is None else F_row[col]
 
             if f_last != f:
                 if f == 0:
-                    print("\x1b[0;1m", end='')
+                    print("\x1b[0;1m", end="")
                 else:
-                    print(f"\x1b[38;5;{f}m", end='')
+                    print(f"\x1b[38;5;{f}m", end="")
                 f_last = f
-            print(chr(C_row[col]), end='', flush=True)
+            print(chr(C_row[col]), end="", flush=True)
         if f_last != 0:
-            print("\x1b[0;1m", end='')
+            print("\x1b[0;1m", end="")
         print(r, flush=True)
 
     # Get the number of middle dashes.
     mid_dashes = cols - 2
     if left is not None:
         mid_dashes -= len(left) + 2
     if right is not None:
         mid_dashes -= len(right) + 2
 
     # Draw the bottom of the box and the left and right strings.
     if mid_dashes >= 0:
-        print(f"{b[7]}{b[1]}", end='', flush=True)
+        print(b[7] + b[1], end="", flush=True)
         if left is not None:
-            print(f" {left} ", end='', flush=True)
+            print(" " + left + " ", end="", flush=True)
         for col in range(mid_dashes):
-            print(b[1], end='', flush=True)
+            print(b[1], end="", flush=True)
         if right is not None:
-            print(f" {right} ", end='', flush=True)
-        print(f"{b[1]}{b[8]}", flush=True)
+            print(" " + right + " ", end="", flush=True)
+        print(b[1] + b[8], flush=True)
     else:
-        print(f"{b[7]}", end='', flush=True)
+        print(b[7], end="", flush=True)
         for col in range(cols):
-            print(b[1], end='', flush=True)
-        print(f"{b[8]}", flush=True)
+            print(b[1], end="", flush=True)
+        print(b[8], flush=True)
         if left is not None:
-            print(left, end='', flush=True)
+            print(left, end="", flush=True)
         if right is not None:
             if left is not None:
-                print(", ", end='', flush=True)
-            print(right, end='', flush=True)
-        print('', flush=True)
+                print(", ", end="", flush=True)
+            print(right, end="", flush=True)
+        print("", flush=True)
 
 
-def redraw_graph(C, D, left=None, right=None,
-        F=None, ccol=None, cstr=None, cF=None, view=None, lims=None):
+def redraw_graph(C, D, F=None, row_zero=-1, view_str=None, label=None,
+        ccol=None, cstr=None, cF=None, view=None, lims=None):
     """
     Parameters
     ----------
     C : (I, J) int np.ndarray
         Matrix of character values.
     D : (I, J) int np.ndarray
         Matrix of boolean values marking changed characters.
-    left : string, default None
+    view_str : string, default None
         String to place on the left of the box.
-    right : string, default None
+    label : string, default None
         String to place on the right of the box.
     F : (I, J) int np.ndarray, default None
         Matrix of foreground 8-bit color values.
+    row_zero : int, default -1
+        Row index of y = 0.
     ccol : int, default None
-        Column index of cursor.
-
-    Notes
-    -----
-    0.022614872267481156 1.00 # baseline
-    0.007898384667653082 2.86 # skipping to deltas
-    0.007420537999439004 3.05 # removing the recalculation of C
+        Column index of cursor. A negative value signals to draw the graph
+        fresh.
+    cstr : str, default None
+        Cursor information string.
+    cF : str, default None
+        Cursor color command.
+    view : limits, default None
+        Object holding the x and y min and max values of the view.
+    lims : limits, default None
+        Object holding the x and y min and max values of the data.
     """
 
     # Define the box drawing characters.
     if config.uni:
         b = ["\u250F", "\u2501", "\u2513",  # . - .
                 "\u2503", "\u2503",         # |   |
                 "\u2523", "\u252B",         # +   +
                 "\u2517", "\u251B"]         # '   '
         s = 0x2800 # braille space
     else:
         b = [".", "-", ".", "|", "|", "+", "+", "'", "'"]
         s = 0x20 # ASCII space
 
-    # Replace zeros with spaces.
-    C = np.where(C == 0, s, C)
-
     # Move the cursor up to the top left corner of the border.
     rows, cols = C.shape
-    print(f"\x1b[{rows + 2}A", end='', flush=True)
+    if ccol >= 0:
+        print(f"\x1b[{rows + 2}A\x1b[1m", end="", flush=True)
+    else:
+        print(f"\x1b[1m", end="", flush=True)
+        ccol = -ccol
 
     # Draw the zoom bar.
-    print(b[0], end='', flush=True)
+    print(b[0], end="", flush=True)
     if (view.x_min > lims.x_min) or (view.x_max < lims.x_max):
         # Get the start and stop columns of the zoom bar.
         x_span = lims.x_max - lims.x_min
         bar_width = round(cols*(view.x_max - view.x_min)/x_span)
         bar_width = max(1, bar_width)
         if view.x_min == lims.x_min:
             col_a = 0
@@ -1354,144 +1727,156 @@
         # Draw the bar.
         print("\x1b[38;5;238m", end="", flush=True)
         for col in range(cols):
             if col == col_a:
                 print("\x1b[0m", end="", flush=True)
             if col == col_b:
                 print("\x1b[38;5;238m", end="", flush=True)
-            print(b[1], end='', flush=True)
+            print(b[1], end="", flush=True)
         print("\x1b[0m", end="", flush=True)
     else:
         for col in range(cols):
-            print(b[1], end='', flush=True)
-    print(f"{b[2]}", flush=True)
+            print(b[1], end="", flush=True)
+    print(b[2], flush=True)
 
     # For each row of the matrix, draw the contents.
     for row in range(rows):
+        # Get the side characters.
+        if row != row_zero:
+            l = b[3]
+            r = b[4]
+        else:
+            l = b[5]
+            r = b[6]
+
         # Get this row of data.
         F_row = 0 if F is None else F[row]
         C_row = C[row]
 
         # Draw this row.
-        print("\x1b[1C\x1b[1m", end='', flush=True) # Move past left border
-        f_last = 0
-        col_last = -1
+        print(l, end="", flush=True) # Move past left border
+        f_last = 0 # the last foreground color
+        col_last = -1 # column of the last edit
         for col in range(cols):
             # Skip where there is no delta.
             if not D[row, col]:
                 continue
+            D[row, col] = False
 
             # Jump to new character location.
             if col > col_last + 1:
-                print(f"\x1b[{col - col_last - 1}C", end='', flush=True)
+                print(f"\x1b[{col - col_last - 1}C", end="", flush=True)
             col_last = col
 
             # Get this column color.
             f = 0 if F is None else F_row[col]
             if F is None:
                 f = 0
             else:
                 f = F_row[col]
                 if (col == ccol) and (f != 0): # Switch to bright colors.
-                    f = BRIGHT_COLORS[NORMAL_COLORS.index(f)]
+                    f = config.lites[config.darks.index(f)]
 
             # Display the cursor.
             if (col == ccol) and (C_row[col] == s):
-                print(cF + b[3] + '\x1b[0;1m', end='', flush=True)
+                print(cF + b[3] + "\x1b[0;1m", end="", flush=True)
                 f_last = 0
             else:
                 if f_last != f:
                     if f == 0:
-                        print("\x1b[0;1m", end='')
+                        print("\x1b[0;1m", end="")
                     else:
-                        print(f"\x1b[38;5;{f}m", end='')
+                        print(f"\x1b[38;5;{f}m", end="")
                     f_last = f
-                print(chr(C_row[col]), end='', flush=True)
+                print(chr(C_row[col]), end="", flush=True)
         if f_last != 0:
-            print("\x1b[0;1m", end='', flush=True)
-        print('', flush=True)
+            print("\x1b[0;1m", end="", flush=True)
+        if cols > col_last + 1:
+            print(f"\x1b[{cols - col_last - 1}C", end="", flush=True)
+        print(r, flush=True)
 
     # Get the number of middle dashes.
-    mid_dashes = cols - 2
-    if left is not None:
-        mid_dashes -= len(left) + 2
-    if right is not None:
-        mid_dashes -= len(right) + 2
+    mid_dashes = cols - 2 # 2 off for corner dashes
     if cstr is not None:
-        mid_dashes -= len(cstr) + 2
+        if mid_dashes - len(cstr) - 2 >= 0:
+            mid_dashes -= len(cstr) + 2 # 2 spaces
+        else:
+            cstr = None
+    if label is not None:
+        if mid_dashes - len(label) - 2 >= 0:
+            mid_dashes -= len(label) + 2 # 2 spaces
+        else:
+            label = None
+    if view_str is not None:
+        if mid_dashes - len(view_str) - 2 >= 0:
+            mid_dashes -= len(view_str) + 2 # 2 spaces
+        else:
+            view_str = None
 
     # Draw the bottom of the box and the left and right strings.
-    if mid_dashes >= 0:
-        print(f"{b[7]}{b[1]}", end='', flush=True)
-        if left is not None:
-            print(f" {left} ", end='', flush=True)
-        if cstr is not None:
-            print(f" {cF}", end='', flush=True)
-            print(f"{cstr}", end='', flush=True)
-            print("\x1b[0m ", end='', flush=True)
-        for col in range(mid_dashes):
-            print(b[1], end='', flush=True)
-        if right is not None:
-            print(f" {right} ", end='', flush=True)
-        print(f"{b[1]}{b[8]}", flush=True)
-    else:
-        print(f"{b[7]}", end='', flush=True)
-        for col in range(cols):
-            print(b[1], end='', flush=True)
-        print(f"{b[8]}", flush=True)
-        if left is not None:
-            print(left, end='', flush=True)
-        if cstr is not None:
-            print(" " + cF, end='', flush=True)
-            print(cstr, end='', flush=True)
-            print("\x1b[0m", end='', flush=True)
-        if right is not None:
-            if (left is not None) or (cstr is not None):
-                print(", ", end='', flush=True)
-            print(right, end='', flush=True)
-        print('', flush=True)
+    print("\x1b[0m" + b[7] + b[1], end="", flush=True)
+    if view_str is not None:
+        print(" " + view_str + " ", end="", flush=True)
+    if cstr is not None:
+        print(" " + cF, end="", flush=True)
+        print(cstr, end="", flush=True)
+        print("\x1b[0m ", end="", flush=True)
+    for col in range(mid_dashes):
+        print(b[1], end="", flush=True)
+    if label is not None:
+        print(f" {label} ", end="", flush=True)
+    print(b[1] + b[8], flush=True)
 
 
 def draw_bar(n, N, colorize, fat):
     # Define the left, center, and right characters and color commands.
     if colorize:
-        grey = '\x1b[100m' if config.uni and fat else '\x1b[90m'
+        grey = "\x1b[100m" if config.uni and fat else "\x1b[90m"
     else:
-        grey = ''
+        grey = ""
     if config.uni:
         if fat:
             l = chr(0x2588)
             frac = int(n*8) % 8 # 0 to 7
-            c = ' ' if frac == 0 else chr(0x2588 + 8 - frac)
+            c = " " if frac == 0 else chr(0x2588 + 8 - frac)
             c = grey + c
-            r = ' '
+            r = " "
         else:
             l = chr(0x2501)
             if (n) % 1 < 0.5:
-                c = grey + chr(0x257A) if colorize else ' '
+                c = grey + chr(0x257A) if colorize else " "
             else:
                 c = chr(0x2578) + grey
-            r = chr(0x2501) if colorize else ' '
+            r = chr(0x2501) if colorize else " "
     else:
         if fat:
-            l = '/'
-            c = grey + '-' if (n % 1 < 0.5) else '/' + grey
-            r = '-'
+            l = "/"
+            c = grey + "-" if (n % 1 < 0.5) else "/" + grey
+            r = "-"
         else:
-            l = '='
-            c = grey + '-' if (n % 1 < 0.5) else '=' + grey
-            r = '-'
+            l = "="
+            c = grey + "-" if (n % 1 < 0.5) else "=" + grey
+            r = "-"
+
+    # Set signal handler for Ctrl+C
+    signal.signal(signal.SIGINT, signal_handler)
+
+    # Hide the cursor.
+    print("\x1b[?25l", end="", flush=True)
 
     # Build the progress bar.
     if n >= N:
         for j in range(N):
-            print(l, end='', flush=True)
+            print(l, end="", flush=True)
     else:
         bar_len = int(n)
         spc_len = N - 1 - bar_len
         for j in range(bar_len):
-            print(l, end='', flush=True)
-        print(c, end='', flush=True)
+            print(l, end="", flush=True)
+        print(c, end="", flush=True)
         for j in range(spc_len):
-            print(r, end='', flush=True)
+            print(r, end="", flush=True)
         if colorize:
-            print('\x1b[0m', end='', flush=True)
+            print("\x1b[0m", end="", flush=True)
+
+    # Show the cursor.
+    print("\x1b[?25h", end="", flush=True)
```

### Comparing `itrm-0.1.9/src/itrm.egg-info/PKG-INFO` & `itrm-0.2.0/src/itrm.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itrm
-Version: 0.1.9
+Version: 0.2.0
 Summary: Interactive Terminal Utilities
 Home-page: https://gitlab.com/davidwoodburn/itrm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,33 +22,64 @@
 This library provides several functions for nicely printing data to the
 terminal. MatPlotLib is a very nice library, but it can be a bit tedious at
 times when all you want is something quick and dirty.
 
 -   Every separate plot needs to be introduced with a `plt.figure()` statement.
 -   Large sets of data can be slow to render.
 -   If you are working in full screen on the terminal, plots can pull you to
-    another window.
+    another window which can be obnoxious.
 -   The entire python program and the terminal is locked up after any
     `plt.show()` command until you close all figure windows.
 -   Unless you save the figures to individual files, there is no buffer to show
     plots from past runs.
+-   Sometimes it it not available, such as when running code on a server through
+    SSH.
 
 These are all excuses to use this library. But, the biggest reason to use this
 library is that the terminal is cool, and the more you can do your work in the
 terminal the better!
 
-## Plots
+As a warning, the terminal emulator built into Neovim does seem to struggle to
+correctly handle string buffering of Unicode characters. Consequently, with
+`itrm.config.uni` set to `True` (the default) the plots can have garbled
+characters and not display correctly. Setting the `uni` property to `False` will
+remove that problem. Other terminal emulators tested do not have this problem.
+
+## Defaults
+
+While `itrm` does not use dotfiles, you can set some "defaults" with the
+`config` class. For example, by default Unicode characters are used throughout,
+but you can change this by setting `itrm.config.uni` to `False` before any other
+call to `itrm`. The following table lists the configuration options:
+
+| Setting       | Default       | Description                       |
+| ---------     | :-----------: | --------------------------------- |
+| `uni`         | `True`        | flag to use Unicode characters    |
+| `cols`        | `60`          | default column width              |
+| `rows`        | `20`          | default row height                |
+| `ar`          | `0.48`        | aspect ratio of characters        |
+
+There is also a method for changing the color map: `itrm.config.cmap()`. It
+takes a string: `"colors"`, `"grays"`, `"reds"`, `"greens"`, or `"blues"`.
+
+## Interactive Plots
 
 ```python
-itrm.plot(x, y=None, label='', rows=1, cols=1, equal=0)
+itrm.iplot(x, y=None, label=None, rows=1, cols=1,
+        lg=None, overlay=False):
 ```
 
-The plot function will render all the data points defined by `x` and `y` to the
-terminal. The inputs `x` and `y` can be vectors or matrices. If they are
-matrices, each row is treated as a separate curve.
+The `iplot` function will render all the data points defined by `x` and `y` to
+the terminal. The inputs `x` and `y` can be vectors or matrices. If they are
+matrices, each **row** is treated as a separate curve. Note, this is different
+from MatPlotLib, in which each *column* is treated as a separate row. (This
+difference is intentional, as in the author's opinion varying time along columns
+means each column in a matrix can be treated as a vector. This arrangement works
+very well with in linear algebra, especially matrix multiplication with a "set"
+of vectors over time.)
 
 The shapes of `x` and `y` do not have to be the same, but they must be
 compatible. So, `x` could be a vector and `y` could be a matrix as long as the
 length of `x` equals the number of columns of `y`.
 
 If only `x` is given, it will be interpreted as the `y` values, and the `x`
 values will be the array of indices.
@@ -65,61 +96,139 @@
 If a `label` is given, this will be printed in the bottom right of the plot box.
 
 The `rows` and `cols` parameters let you specify the number of terminal text
 rows and columns to use for the plot, respectively. For each of these, if the
 value is less than or equal to 1, it represents a portion of the available space
 to use. For example, if `rows` is `0.5`, then half the number of rows of the
 current terminal window will be used for the plot. If the value is greater than
-1, it represents the absolute number of columns or rows to use. Also, if the
+1, it represents the absolute number of rows or columns to use. Also, if the
 size of the current terminal cannot be obtained, the available space will
 default to `20` rows and `60` columns. These defaults can be redefined by
-changing `itrm.config.rows` and `itrm.config.cols`.
+changing `itrm.config.rows` and `itrm.config.cols`, respectively.
 
 By default, this library will use Unicode symbols (specifically braille) for
-plotting. A good font to use is JuliaMono. However, if your font does not
+plotting. A recommended font is JuliaMono. However, if your font does not
 support the necessary Unicode symbols, you can tell the library to not use them
 by setting `itrm.config.uni` to `False` before calling the `itrm.plot` function.
+In that case, only ASCII characters will be used.
 
-If only one curve is being plotted, the characters will be written in whatever
-the default font color is set to in your terminal. If more than one curve is
-plotted, color will be used. The color map is blue, green, yellow, orange, and
-magenta. If you have more than 5 curves (This is just a terminal-based plot; why
-would you do that?), then the colors will recycle.
-
-If you want equal axis scaling, set `equal` to `1`. However, since terminal
-fonts are not always the same aspect ratio and because the line spacing in your
-terminal might be adjustable, you can adjust this value to tune.
+To distinguish multiple curves from each other, colors will be used. The color
+map is blue, green, yellow, orange, magenta, and purple. If you have more than 6
+curves (This is just a terminal-based plot; why would you do that?), then the
+colors will recycle.
+
+You can set the x or y axes to logarithmic scaling by setting the `lg` parameter
+to one of `"x"`, `"y"`, or `"xy"`. Note that the values reported for the view
+and the cursor will also be logarithmic.
+
+To prevent your terminal history from extending each time a new plot is
+rendered, you can print a new plot over a previous plot by setting the `overlay`
+parameter to `True`. This can be especially useful when there a multiple plots
+to render but you do not want your terminal history to fill up quickly.
+
+The `iplot` function provides interactivity through a vertical cursor. You can
+move the cursor left and right, at normal speed or fast speed. You can zoom in
+and out. And, you can cycle through which rows of the `x` and `y` data to focus
+on. Note, `iplot` is designed for monotonically-increasing `x` values, and,
+consequently, does not support equal axis scaling.
 
-| Single curve    | Multiple curves |
-| --------------- | --------------- |
-| ![](https://gitlab.com/davidwoodburn/itrm/-/raw/main/figures/fig_plot_1.png) | ![](https://gitlab.com/davidwoodburn/itrm/-/raw/main/figures/fig_plot_5.png) |
+![](https://gitlab.com/davidwoodburn/itrm/-/raw/main/figures/fig_iplot.png)
 
-## Interactive Plots
+The following table details the shortcut keys:
+
+| Keys               | Function                 |   | Keys           | Function                 |
+| :----------------: | ------------------------ | - | :------------: | ------------------------ |
+| `q`, `x`, `⌫`, `↵` | exit interactive plot    |   | `j`, `s`, `↓`  | zoom in                  |
+| `h`, `a`, `←`      | move cursor left         |   | `k`, `w`, `↑`  | zoom out                 |
+| `l`, `d`, `→`      | move cursor right        |   | `J`, `S`, `⇧↓` | zoom in fast             |
+| `H`, `A`, `⇧←`     | move cursor left fast    |   | `K`, `W`, `⇧↑` | zoom out fast            |
+| `L`, `D`, `⇧→`     | move cursor right fast   |   | `n`            | next data row            |
+| `g`                | move cursor to start     |   | `p`            | previous data row        |
+| `G`                | move cursor to end       |   | `i`            | toggle individual view   |
+| `c`, `z`           | center view on cursor    |   | `r`            | redraw the whole plot    |
+
+## Plots
 
 ```python
-itrm.iplot(x, y=None, label='', rows=1, cols=1)
+itrm.plot(x, y=None, label=None, rows=1, cols=1,
+        equal_axes=0, lg=None, overlay=False):
 ```
 
-The `iplot` function is nearly identical to the `plot` function, except that the
-resulting plot will be interactive with a cursor you can move to inspect the
-values. You can move the cursor left and right, at normal speed or fast speed.
-You can zoom in and out. And, you can cycle through which rows of the `x` and
-`y` data to focus on.
+The `plot` function is a non-interactive version of the `iplot` function.
 
-The following table details the shortcut keys:
+The `plot` function will render all the data points defined by `x` and `y` to
+the terminal. The inputs `x` and `y` can be vectors or matrices. If they are
+matrices, each **row** is treated as a separate curve. Note, this is different
+from MatPlotLib, in which each *column* is treated as a separate row. (This
+difference is intentional, as in the author's opinion varying time along columns
+means each column in a matrix can be treated as a vector. This arrangement works
+very well with in linear algebra, especially matrix multiplication with a "set"
+of vectors over time.)
 
-| Keys           | Function                 |   | Keys           | Function                 |
-| :------------: | ------------------------ | - | :------------: | ------------------------ |
-| `q`, `x`, `⌫`  | exit interactive plot    |   | `j`, `s`, `↓`  | zoom in                  |
-| `h`, `a`, `←`  | move cursor left         |   | `k`, `w`, `↑`  | zoom out                 |
-| `l`, `d`, `→`  | move cursor right        |   | `J`, `S`, `⇧↓` | zoom in fast             |
-| `H`, `A`, `⇧←` | move cursor left fast    |   | `K`, `W`, `⇧↑` | zoom out fast            |
-| `L`, `D`, `⇧→` | move cursor right fast   |   | `n`            | next data row            |
-| `g`            | move cursor to start     |   | `p`            | previous data row        |
-| `G`            | move cursor to end       |   | `c`, `z`       | center view on cursor    |
+The shapes of `x` and `y` do not have to be the same, but they must be
+compatible. So, `x` could be a vector and `y` could be a matrix as long as the
+length of `x` equals the number of columns of `y`.
+
+If only `x` is given, it will be interpreted as the `y` values, and the `x`
+values will be the array of indices.
+
+When the plot is printed, the graph is rendered within a box and the ranges of
+`x` and `y` are listed in the bottom left corner. So,
+
+```
+(0:99, -1.5:1.5)
+```
+
+means that `x` ranges from `0` to `99` and `y` ranges from `-1.5` to `1.5`.
+
+If a `label` is given, this will be printed in the bottom right of the plot box.
+
+The `rows` and `cols` parameters let you specify the number of terminal text
+rows and columns to use for the plot, respectively. For each of these, if the
+value is less than or equal to 1, it represents a portion of the available space
+to use. For example, if `rows` is `0.5`, then half the number of rows of the
+current terminal window will be used for the plot. If the value is greater than
+1, it represents the absolute number of rows or columns to use. Also, if the
+size of the current terminal cannot be obtained, the available space will
+default to `20` rows and `60` columns. These defaults can be redefined by
+changing `itrm.config.rows` and `itrm.config.cols`, respectively.
+
+By default, this library will use Unicode symbols (specifically braille) for
+plotting. A recommended font is JuliaMono. However, if your font does not
+support the necessary Unicode symbols, you can tell the library to not use them
+by setting `itrm.config.uni` to `False` before calling the `itrm.plot` function.
+In that case, only ASCII characters will be used.
+
+To distinguish multiple curves from each other, colors will be used. The color
+map is blue, green, yellow, orange, magenta, and purple. If you have more than 6
+curves (This is just a terminal-based plot; why would you do that?), then the
+colors will recycle.
+
+If you want equal axis scaling, set `equal_axes` to `True`. However, since
+terminal fonts are not always the same aspect ratio and because the line spacing
+in your terminal might be adjustable, you can adjust the understood character
+aspect ratio with `itrm.config.ar`. The default value is `0.48`. This means the
+width of a character is understood to be about 0.48 of the height of a
+character. Making this value larger means the characters are interpreted to be
+wider, making the plot narrower horizontally. This is a feature the `iplot`
+function does not share. Because the `plot` supports equal axis scaling, it does
+not require that the `x` axis data monotonically increase.
+
+You can set the x or y axes to logarithmic scaling by setting the `lg` parameter
+to one of `"x"`, `"y"`, or `"xy"`. Note that the values reported for the view
+will also be logarithmic.
+
+To prevent your terminal history from extending each time a new plot is
+rendered, you can print a new plot over a previous plot by setting the `overlay`
+parameter to `True`. This can be especially useful when creating a live
+animation.
+
+| Single curve    | Multiple curves |
+| --------------- | --------------- |
+| ![](https://gitlab.com/davidwoodburn/itrm/-/raw/main/figures/fig_plot_1.png) | ![](https://gitlab.com/davidwoodburn/itrm/-/raw/main/figures/fig_plot_6.png) |
 
 ## Bars
 
 ```python
 itrm.bars(x, labels=None, cols=1, fat=False)
 ```
```

