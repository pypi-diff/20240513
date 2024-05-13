# Comparing `tmp/eQuimage-1.3.0.tar.gz` & `tmp/eQuimage-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eQuimage-1.3.0.tar", last modified: Sat Feb 17 14:12:12 2024, max compression
+gzip compressed data, was "eQuimage-1.4.0.tar", last modified: Sat Mar 30 07:28:13 2024, max compression
```

## Comparing `eQuimage-1.3.0.tar` & `eQuimage-1.4.0.tar`

### file list

```diff
@@ -1,61 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 14:12:12.668168 eQuimage-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-02-17 14:12:05.000000 eQuimage-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-02-17 14:12:12.668168 eQuimage-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-02-17 14:12:05.000000 eQuimage-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-02-17 14:12:05.000000 eQuimage-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-17 14:12:12.668168 eQuimage-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 14:12:12.660168 eQuimage-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 14:12:12.660168 eQuimage-1.3.0/src/eQuimage/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/eQuimage.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)    14727 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/eQuimage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 14:12:12.660168 eQuimage-1.3.0/src/eQuimage/icons/
--rw-r--r--   0 runner    (1001) docker     (127)    81116 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/icons/icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    81897 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/icons/icon.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 14:12:12.660168 eQuimage-1.3.0/src/eQuimage/imageprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/imageprocessing/Unistellar.py
--rw-r--r--   0 runner    (1001) docker     (127)    34847 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/imageprocessing/imageprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/imageprocessing/stretchfunctions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/imageprocessing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 14:12:12.660168 eQuimage-1.3.0/src/eQuimage/images/
--rw-r--r--   0 runner    (1001) docker     (127)   764153 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/images/splash.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 14:12:12.668168 eQuimage-1.3.0/src/eQuimage/windows/
--rw-r--r--   0 runner    (1001) docker     (127)    11821 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/addframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/arcsinh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/bilateral.py
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/blackpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/blend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/clahe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/colorbalance.py
--rw-r--r--   0 runner    (1001) docker     (127)     9115 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/colornoise.py
--rw-r--r--   0 runner    (1001) docker     (127)    10131 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/colorsaturation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9847 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/ghscolorsat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 14:12:12.668168 eQuimage-1.3.0/src/eQuimage/windows/gtk/
--rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/gtk/customwidgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/gtk/filechoosers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/gtk/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/gtk/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/hotpixels.py
--rw-r--r--   0 runner    (1001) docker     (127)     9929 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/hyperbolic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/luma.py
--rw-r--r--   0 runner    (1001) docker     (127)    19816 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/mainmenu.py
--rw-r--r--   0 runner    (1001) docker     (127)    24712 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/mainwindow.py
--rw-r--r--   0 runner    (1001) docker     (127)    10003 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/midtone.py
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/picker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    13789 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/stretch.py
--rw-r--r--   0 runner    (1001) docker     (127)    16860 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/totalvariation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/unsharp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-02-17 14:12:05.000000 eQuimage-1.3.0/src/eQuimage/windows/wavelets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 14:12:12.668168 eQuimage-1.3.0/src/eQuimage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-02-17 14:12:12.000000 eQuimage-1.3.0/src/eQuimage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-02-17 14:12:12.000000 eQuimage-1.3.0/src/eQuimage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-17 14:12:12.000000 eQuimage-1.3.0/src/eQuimage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-17 14:12:12.000000 eQuimage-1.3.0/src/eQuimage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-02-17 14:12:12.000000 eQuimage-1.3.0/src/eQuimage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-17 14:12:12.000000 eQuimage-1.3.0/src/eQuimage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 07:28:13.437389 eQuimage-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-30 07:28:08.000000 eQuimage-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-03-30 07:28:13.437389 eQuimage-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-03-30 07:28:08.000000 eQuimage-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-03-30 07:28:08.000000 eQuimage-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 07:28:13.437389 eQuimage-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 07:28:13.425389 eQuimage-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 07:28:13.429389 eQuimage-1.4.0/src/eQuimage/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 07:28:13.429389 eQuimage-1.4.0/src/eQuimage/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/config/eQuimage.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/config/eQuimage.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)    14871 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/eQuimage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 07:28:13.429389 eQuimage-1.4.0/src/eQuimage/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 07:28:13.433389 eQuimage-1.4.0/src/eQuimage/gui/gtk/
+-rw-r--r--   0 runner    (1001) docker     (127)    22933 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/gtk/customwidgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/gtk/filechoosers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/gtk/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/gtk/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/gtk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/luma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15506 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/mainmenu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25347 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/mainwindow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 07:28:13.433389 eQuimage-1.4.0/src/eQuimage/gui/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/misc/imagechooser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/misc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17171 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/toolmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 07:28:13.437389 eQuimage-1.4.0/src/eQuimage/gui/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    10915 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/tools/addframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/tools/arcsinh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/tools/bilateral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/tools/blackpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/tools/blend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/tools/butterworth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/tools/clahe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/tools/colorbalance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/tools/colornoise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8212 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/tools/colorsaturation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/tools/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9316 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/tools/ghscolorsat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/tools/grayscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/tools/hotpixels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9340 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/tools/hyperbolic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/tools/midtone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/tools/nlmeans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/tools/pixelmath.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12989 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/tools/stretch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/tools/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/tools/thresholdmask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/tools/totalvariation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/tools/unsharp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/gui/tools/wavelets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 07:28:13.437389 eQuimage-1.4.0/src/eQuimage/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)    81116 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/icons/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    81897 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/icons/icon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 07:28:13.437389 eQuimage-1.4.0/src/eQuimage/imageprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/imageprocessing/Unistellar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/imageprocessing/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/imageprocessing/defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34609 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/imageprocessing/imageprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/imageprocessing/pixelmath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/imageprocessing/stretchfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/imageprocessing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 07:28:13.437389 eQuimage-1.4.0/src/eQuimage/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   764153 2024-03-30 07:28:08.000000 eQuimage-1.4.0/src/eQuimage/images/splash.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 07:28:13.437389 eQuimage-1.4.0/src/eQuimage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-03-30 07:28:13.000000 eQuimage-1.4.0/src/eQuimage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-03-30 07:28:13.000000 eQuimage-1.4.0/src/eQuimage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 07:28:13.000000 eQuimage-1.4.0/src/eQuimage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-30 07:28:13.000000 eQuimage-1.4.0/src/eQuimage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-30 07:28:13.000000 eQuimage-1.4.0/src/eQuimage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-30 07:28:13.000000 eQuimage-1.4.0/src/eQuimage.egg-info/top_level.txt
```

### Comparing `eQuimage-1.3.0/LICENSE` & `eQuimage-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eQuimage-1.3.0/PKG-INFO` & `eQuimage-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eQuimage
-Version: 1.3.0
+Version: 1.4.0
 Summary: eQuimage is a tool to postprocess astronomical images from Unistellar telescopes.
 Author-email: Yann-Michel Niquet <contact@ymniquet.fr>
 Project-URL: homepage, https://astro.ymniquet.fr/
 Project-URL: repository, https://github.com/ymniquet/eQuimage
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -26,15 +26,15 @@
 
 ### eQuimage is a python tool to postprocess astronomical images from Unistellar telescopes
 
 Author: Yann-Michel Niquet (https://astro.ymniquet.fr)
 
 ### Installation
 
-eQuimage is developed in Python 3 with a GTK3 graphical interface. Python 3 and the GTK3 library are available in all Linux distributions; On Windows, follow https://www.gtk.org/docs/installations/windows/ for GTK3. To install the latest version of eQuimage, open a linux terminal/windows command prompt and run:
+eQuimage is developed in Python 3 with a GTK3 graphical user interface. Python 3 and the GTK3 library are available in all Linux distributions; on Windows, follow https://www.gtk.org/docs/installations/windows/ for GTK3. To install the latest version of eQuimage, open a linux terminal/windows command prompt and run:
 
   `pip install --user eQuimage`
 
 pip will automatically download eQuimage and the missing python modules if necessary (matplotlib, etc...). You can then launch eQuimage by typing:
 
   `eQuimage`
 
@@ -49,8 +49,7 @@
   - keep track (in a log file) of all operations applied to a given image.
 
 There is no documentation yet, but you should find your way around easily if you have used image processing software before. The python code itself is documented in English.
 
 ### Known bugs
 
   - On windows, the imageio/freeimage plugin can not read png's with accents (and likely other special characters) in the file name.
-
```

### Comparing `eQuimage-1.3.0/README.md` & `eQuimage-1.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ### eQuimage is a python tool to postprocess astronomical images from Unistellar telescopes
 
 Author: Yann-Michel Niquet (https://astro.ymniquet.fr)
 
 ### Installation
 
-eQuimage is developed in Python 3 with a GTK3 graphical interface. Python 3 and the GTK3 library are available in all Linux distributions; On Windows, follow https://www.gtk.org/docs/installations/windows/ for GTK3. To install the latest version of eQuimage, open a linux terminal/windows command prompt and run:
+eQuimage is developed in Python 3 with a GTK3 graphical user interface. Python 3 and the GTK3 library are available in all Linux distributions; on Windows, follow https://www.gtk.org/docs/installations/windows/ for GTK3. To install the latest version of eQuimage, open a linux terminal/windows command prompt and run:
 
   `pip install --user eQuimage`
 
 pip will automatically download eQuimage and the missing python modules if necessary (matplotlib, etc...). You can then launch eQuimage by typing:
 
   `eQuimage`
 
@@ -23,8 +23,7 @@
   - keep track (in a log file) of all operations applied to a given image.
 
 There is no documentation yet, but you should find your way around easily if you have used image processing software before. The python code itself is documented in English.
 
 ### Known bugs
 
   - On windows, the imageio/freeimage plugin can not read png's with accents (and likely other special characters) in the file name.
-
```

### Comparing `eQuimage-1.3.0/pyproject.toml` & `eQuimage-1.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eQuimage"
-version = "1.3.0"
+version = "1.4.0"
 authors = [
   { name = "Yann-Michel Niquet", email = "contact@ymniquet.fr" },
 ]
 description = "eQuimage is a tool to postprocess astronomical images from Unistellar telescopes."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -39,11 +39,11 @@
 eQuimage = "eQuimage.eQuimage:run"
 
 [tool.setuptools.packages.find]
 namespaces = true
 where = ["src"]
 
 [tool.setuptools.package-data]
-eQuimage = ["eQuimage.mplstyle", "splash.png", "icon.png", "icon.ico"]
-"eQuimage.icons" = ["icon.png", "icon.ico"]
+"eQuimage.config" = ["eQuimage.css", "eQuimage.mplstyle"]
 "eQuimage.images" = ["splash.png"]
+"eQuimage.icons" = ["icon.png", "icon.ico"]
```

### Comparing `eQuimage-1.3.0/src/eQuimage/__init__.py` & `eQuimage-1.4.0/src/eQuimage/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,5 +1,5 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
```

### Comparing `eQuimage-1.3.0/src/eQuimage/eQuimage.mplstyle` & `eQuimage-1.4.0/src/eQuimage/config/eQuimage.mplstyle`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
 
 ### LINES
 lines.linewidth       : 2.0
 lines.linestyle       : -
 lines.color           : black
 lines.marker          : None
 lines.markeredgewidth : 0.5
```

### Comparing `eQuimage-1.3.0/src/eQuimage/eQuimage.py` & `eQuimage-1.4.0/src/eQuimage/eQuimage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,53 +1,60 @@
 #!/usr/bin/python
 
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
 
 """eQuimage is a python tool to postprocess astronomical images from Unistellar telescopes."""
 
-__version__ = "1.3.0"
+__version__ = "1.4.0"
 
 import os
 os.environ["LANGUAGE"] = "en"
 import sys
 import ast
 import inspect
 packagepath = os.path.dirname(inspect.getabsfile(inspect.currentframe()))
 import gi
 gi.require_version("Gtk", "3.0")
-from gi.repository import Gtk, Gio
+from gi.repository import Gtk, Gdk, Gio
 import matplotlib.pyplot as plt
-plt.style.use(packagepath+"/eQuimage.mplstyle")
-from .windows.base import ErrorDialog
-from .windows.mainmenu import MainMenu
-from .windows.mainwindow import MainWindow
-from .windows.tools import BaseToolWindow
-from .windows.logs import LogWindow
+plt.style.use(os.path.join(packagepath, "config", "eQuimage.mplstyle"))
+from .gui.base import ErrorDialog
+from .gui.mainmenu import MainMenu
+from .gui.mainwindow import MainWindow
+from .gui.toolmanager import BaseToolWindow
+from .gui.logs import LogWindow
 from .imageprocessing import imageprocessing
-from .imageprocessing.Unistellar import UnistellarImage as Image
+from .imageprocessing.Unistellar import UnistellarImage
 
 class eQuimageApp(Gtk.Application):
   """The eQuimage application."""
 
   #######################
   # Gtk initialization. #
   #######################
 
   def __init__(self, *args, **kwargs):
     """Initialize the eQuimage application."""
     super().__init__(*args, flags = Gio.ApplicationFlags.HANDLES_OPEN, **kwargs)
     self.initialize()
 
   def do_startup(self):
-    """Prepare the main menu on startup."""
+    """Load CSS and prepare main menu on startup."""
     Gtk.Application.do_startup(self)
+    # Load CSS.
+    screen = Gdk.Screen.get_default()
+    provider = Gtk.CssProvider()
+    provider.load_from_path(os.path.join(self.packagepath, "config", "eQuimage.css"))
+    stylecontext = Gtk.StyleContext()
+    stylecontext.add_provider_for_screen(screen, provider, Gtk.STYLE_PROVIDER_PRIORITY_APPLICATION)
+    # Prepare main menu.
     self.mainmenu = MainMenu(self)
 
   def do_activate(self):
     """Open the main window on activation."""
     self.mainwindow.open()
     try: # Download freeimage plugin for imageio...
       import imageio
@@ -67,14 +74,16 @@
     except Exception as err:
       ErrorDialog(self.mainwindow.window, str(err))
 
   ###############################
   # Application data & methods. #
   ###############################
 
+  ImageClass = UnistellarImage # The base class used for images.
+
   # Initialization.
 
   def initialize(self):
     """Initialize the eQuimage object."""
     self.version = __version__
     self.packagepath = packagepath
     self.mainwindow = MainWindow(self)
@@ -110,20 +119,18 @@
     self.mainmenu.update()
 
   # Application context.
 
   def get_context(self, key = None):
     """Return the application context:
          - get_context("image") = True if an image is loaded.
-         - get_context("operations") = True if operations have been performed on the image.
          - get_context("activetool") = True if a tool is active.
-         - get_context("frame") = True if the image has a frame.
-         - get_context("cancelled") = True if there are cancelled operations available for restore.
+         - get_context("cancelled") = True if there are cancelled operations available for redo.
          - get_context() returns all above keys as a dictionnary."""
-    context = {"image": len(self.images) > 0, "operations": len(self.operations) > 0, "activetool": self.toolwindow.opened, "frame": self.frame is not None, "cancelled": len(self.cancelled) > 0}
+    context = {"image": len(self.images) > 0, "activetool": self.toolwindow.opened, "cancelled": len(self.cancelled) > 0}
     return context[key] if key is not None else context
 
   def get_image_size(self):
     """Return width and height of the *original* image."""
     return self.width, self.height
 
   def get_color_depth(self):
@@ -150,15 +157,15 @@
 
   def get_savename(self):
     """Return image save name."""
     return self.savename
 
   def load_file(self, filename):
     """Load image file 'filename'."""
-    image = Image()
+    image = self.ImageClass()
     meta = image.load(filename)
     if not image.is_valid(): return
     self.clear(mainwindow = False)
     self.meta = meta
     self.filename = filename
     self.pathname = os.path.dirname(filename)
     self.basename = os.path.basename(filename)
@@ -251,39 +258,39 @@
     if not self.toolwindow.open(self.images[-1]): return
     self.mainmenu.update()
     self.toolwindow.window.present()
 
   def finalize_tool(self, image, operation, frame = None):
     """Finalize tool: push ('operation', 'image', 'frame') on the operations and images stacks (if operation is not None)
        and refresh main menu, main window, and log window.
-       If 'frame' is None, the current self.frame is used as image frame."""
+       If 'frame' is None, the current self.frame is used as image frame from now on."""
     if operation is not None:
       image.meta["description"] = operation
       self.push_operation(operation, image, frame)
       self.cancelled = []
     self.mainwindow.reset_images()
     self.logwindow.update()
     self.mainmenu.update()
 
-  def cancel_last_operation(self):
+  def undo(self):
     """Cancel last operation."""
     if self.toolwindow.opened: return
     if not self.operations: return
     print("Cancelling last operation...")
     self.cancelled.append(self.pop_operation())
     if self.images: self.frame = self.images[-2] # Update current frame.
     self.mainwindow.reset_images()
     self.logwindow.update()
     self.mainmenu.update()
 
-  def redo_last_cancelled(self):
-    """Redo last cancelled operation."""
+  def redo(self):
+    """Redo last operation."""
     if self.toolwindow.opened: return
     if not self.cancelled: return
-    print("Redoing last cancelled operation...")
+    print("Redoing last operation...")
     self.push_operation(*self.cancelled.pop())
     self.mainwindow.reset_images()
     self.logwindow.update()
     self.mainmenu.update()
 
   # Simple tools.
 
@@ -295,36 +302,37 @@
 
   def negative(self):
     """Make a negative of the image."""
     if self.toolwindow.opened: return
     print("Converting to negative...")
     self.finalize_tool(self.images[-1].negative(inplace = False), f"Negative()")
 
-  def gray_scale(self):
-    """Convert image to gray scale."""
-    if self.toolwindow.opened: return
-    print("Converting to gray scale...")
-    self.mainwindow.lock_rgb_luma()
-    red, green, blue = imageprocessing.get_rgb_luma()
-    self.finalize_tool(self.images[-1].gray_scale(inplace = False), f"GrayScale({red:.2f}, {green:.2f}, {blue:.2f})")
-    self.mainwindow.unlock_rgb_luma()
-
   def remove_unistellar_frame(self):
     """Remove Unistellar frame."""
     if self.toolwindow.opened: return
-    if self.frame is None: return
+    frame = self.images[-1].get_frame()
+    if frame is None:
+      ErrorDialog(self.mainwindow.window, "This image has no frame.")
+      return
     print("Removing Unistellar frame...")
-    self.finalize_tool(self.images[-1].remove_frame(self.frame, inplace = False), "RemoveUnistellarFrame()")
+    self.finalize_tool(self.images[-1].remove_frame(frame, inplace = False), "RemoveUnistellarFrame()")
 
   def restore_unistellar_frame(self):
     """Restore Unistellar frame."""
     if self.toolwindow.opened: return
-    if self.frame is None: return
+    if self.frame is None:
+      ErrorDialog(self.mainwindow.window, "This is no registered frame.")
+      return
     print("Restoring Unistellar frame...")
-    self.finalize_tool(self.images[-1].add_frame(self.frame, inplace = False), "RestoreUnistellarFrame()")
+    try:
+      image = self.images[-1].add_frame(self.frame, inplace = False)
+    except:
+      ErrorDialog(self.mainwindow.window, "Operation failed.")
+      return
+    self.finalize_tool(image, "RestoreUnistellarFrame()")
 
   # Settings.
 
   def settings_from_dict(self, settings):
     """Set settings from dictionnary 'settings'.
        Return zero if successful, non-zero otherwise."""
     error = 0
@@ -362,34 +370,36 @@
   def default_settings(self):
     """Apply default settings."""
     self.settings_from_dict(self.get_default_settings())
 
   def load_settings(self):
     """Read settings in (system wide) file packagepath/eQuimagerc.
        Return zero if successful, non-zero otherwise."""
+    filename = os.path.join(self.packagepath, "config", "eQuimagerc")
     try:
-      with open(packagepath+"/eQuimagerc", "r") as f:
+      with open(filename, "r") as f:
         string = f.readline()
       settings = ast.literal_eval(string)
       if not isinstance(settings, dict): raise TypeError
     except:
-      print("Failed to read configuration file "+packagepath+"/eQuimagerc.")
+      print(f"Failed to read configuration file {filename}.")
       return -1
     return self.settings_from_dict(settings)
 
   def save_settings(self):
     """Save settings in (system wide) file packagepath/eQuimagerc.
        Return zero if successful, non-zero otherwise."""
     error = 0
     settings = {"remove_hot_pixels_on_the_fly": self.hotpixelsotf, "stretch_on_the_fly": self.stretchotf, "colors_on_the_fly": self.colorotf, "blend_on_the_fly": self.blendotf, "poll_time": self.polltime}
+    filename = os.path.join(self.packagepath, "config", "eQuimagerc")
     try:
-      with open(packagepath+"/eQuimagerc", "w") as f:
+      with open(filename, "w") as f:
         f.write(repr(settings))
     except:
-      print("Failed to write configuration file "+packagepath+"/eQuimagerc.")
+      print(f"Failed to write configuration file {filename}.")
       error = -1
     return error
 
 #
 
 def run():
   """Run eQuimage."""
```

### Comparing `eQuimage-1.3.0/src/eQuimage/icons/icon.ico` & `eQuimage-1.4.0/src/eQuimage/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `eQuimage-1.3.0/src/eQuimage/icons/icon.png` & `eQuimage-1.4.0/src/eQuimage/icons/icon.png`

 * *Files identical despite different names*

### Comparing `eQuimage-1.3.0/src/eQuimage/imageprocessing/Unistellar.py` & `eQuimage-1.4.0/src/eQuimage/imageprocessing/Unistellar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
 
 """Image processing tools for Unistellar frames."""
 
 import numpy as np
 from copy import deepcopy
 import matplotlib.pyplot as plt
 from .imageprocessing import Image
```

### Comparing `eQuimage-1.3.0/src/eQuimage/imageprocessing/imageprocessing.py` & `eQuimage-1.4.0/src/eQuimage/imageprocessing/imageprocessing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,79 +1,71 @@
 # This program is 0free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
 
 """Image processing tools."""
 
 import re
 import os
 import numpy as np
 import matplotlib.pyplot as plt
-import matplotlib.colors as colors
 import imageio.v3 as iio
 from copy import deepcopy
 from PIL import Image as PILImage
 from scipy.signal import convolve2d
-from .utils import scale_pixels, lookup
-
-IMGTYPE = np.float32 # Data type used for images (either np.float32 or np.float64).
-
-IMGTOL = 1.e-6 if IMGTYPE is np.float32 else 1.e-9 # Expected accuracy in np.float32/np.float64 calculations.
-
-NEAREST  = PILImage.Resampling.NEAREST # Resampling methods, imported from PIL.
-BILINEAR = PILImage.Resampling.BILINEAR
-BICUBIC  = PILImage.Resampling.BICUBIC
-LANCZOS  = PILImage.Resampling.LANCZOS
-BOX      = PILImage.Resampling.BOX
-HAMMING  = PILImage.Resampling.HAMMING
-
-rgbluma = IMGTYPE((0.3, 0.6, 0.1)) # Weight of the R, G, B channels in the luma.
-
-def get_rgb_luma():
-  """Return the RGB components of the luma channel."""
-  return tuple(rgbluma)
-
-def set_rgb_luma(rgb):
-  """Set the RGB components 'rgb' of the luma channel."""
-  global rgbluma
-  rgbluma = IMGTYPE(rgb)
+from .defs import *
+from . import utils
+from . import colors
+from .colors import rgbluma, get_rgb_luma, set_rgb_luma
 
 class Image:
-  """Image class. The RGB components are stored as floats in the range [0, 1].
-     Note: No particular color space is assumed. Practically, most RGB images
-     are encoded in the non-linear sRGB color space. It is the responsibility
-     of the user to make the color transformations appropriate to his needs."""
+  """Image class.
+     The RGB components are stored as (3, height, width) arrays of floats in the range [0, 1].
+     Note: No particular color space is assumed. Practically, most RGB images are encoded in
+     the non-linear sRGB color space. It is the responsibility of the user to make the color
+     space transformations appropriate to his needs."""
 
   # Object constructors, getters & setters.
 
-  def __init__(self, image = None, meta = {}):
-    """Initialize object with RGB image 'image' and meta-data 'meta'.
-       The meta-data is a dictionary (or any other container) of user-defined data."""
-    self.rgb = IMGTYPE(image) if image is not None else None
+  def __init__(self, image = None, meta = {}, channels = 0, copy = False):
+    """Initialize object with RGB image 'image' (with channel axis 'channels') and meta-data 'meta'.
+       The meta-data is a dictionary (or any other container) of user-defined data.
+       The image is copied if 'copy' is True, or referenced (if possible) if False."""
+    self.set_image(image, channels = channels, copy = copy)
     self.meta = meta
 
   @classmethod
-  def newImage(cls, self, image = None, meta = {}):
-    """Return a new instance with RGB image 'image' and meta-data 'meta'.
-       The meta-data is a dictionary (or any other container) of user-defined data."""
-    return cls(image = image, meta = meta)
-
-  def set_image(self, image, channel = 0, copy = False):
-    """Set RGB image 'image' with channel axis 'channel' and return the object.
-       The image is copied if 'copy' is True, or referenced if False."""
+  def newImage(cls, self, image = None, meta = {}, channels = 0, copy = False):
+    """Return a new instance with RGB image 'image' (with channel axis 'channels') and meta-data 'meta'.
+       The meta-data is a dictionary (or any other container) of user-defined data.
+       The image is copied if 'copy' is True, or referenced (if possible) if False."""
+    return cls(image = image, meta = meta, channels = channels, copy = copy)
+
+  def set_image(self, image, channels = 0, copy = False):
+    """Set RGB image 'image' (with channel axis 'channels') and return the object.
+       The image is copied if 'copy' is True, or referenced (if possible) if False."""
+    if image is None: # Short-circuit if image is None.
+      self.rgb = None
+      return self
+    if not isinstance(image, np.ndarray):
+      raise TypeError("Error, the image must be a numpy ndarray.")
+    if image.ndim != 3:
+      raise ValueError("Error, the image must be a 3D array.")
+    if image.shape[channels] != 3:
+      raise ValueError("Error, there must be exactly three (RGB) channels in the image.")
     if copy:
-      self.rgb = np.copy(np.moveaxis(image, channel, 0))
+      self.rgb = IMGTYPE(np.copy(np.moveaxis(image, channels, 0)))
     else:
-      self.rgb = np.moveaxis(image, channel, 0)
+      self.rgb = IMGTYPE(np.moveaxis(image, channels, 0))
     return self
 
   def get_image(self):
-    """Return (a reference to) the RGB image."""
+    """Return a reference to the RGB image."""
     return self.rgb
 
   def get_image_copy(self):
     """Return a copy of the RGB image."""
     return self.rgb.copy()
 
   def set_meta(self, meta):
@@ -84,24 +76,24 @@
   def update_meta(self, newmeta):
     """Update image meta-data with 'newmeta' and return the object.
        Meaningful only if the image meta-data is a dictionary or any other container with an 'update' method."""
     self.meta.update(newmeta)
     return self
 
   def get_meta(self):
-    """Return (a reference to) the image meta-data."""
+    """Return a reference to the image meta-data."""
     return self.meta
 
   # Object inquiries.
 
   def size(self):
     """Return the image width and height in pixels."""
     return self.rgb.shape[2], self.rgb.shape[1]
 
-  def rgbf(self):
+  def rgbf_view(self):
     """Return *a view* of the RGB components as a (height, width, 3) array of floats."""
     return np.moveaxis(self.rgb, 0, -1)
 
   def rgbf_copy(self):
     """Return *a copy* of the RGB components as a (height, width, 3) array of floats."""
     return np.moveaxis(self.rgb, 0, -1).copy()
 
@@ -113,83 +105,76 @@
   def rgb16(self):
     """Return the RGB components as a (height, width, 3) array of 16 bits integers in the range [0, 65535]."""
     data = np.clip(self.rgb*65535, 0, 65535)
     return np.moveaxis(np.rint(data).astype("uint16"), 0, -1)
 
   def value(self):
     """Return the HSV value = max(RGB)."""
-    return self.rgb.max(axis = 0)
+    return colors.hsv_value(self.rgb)
 
   def saturation(self):
     """Return the HSV saturation = 1-min(RGB)/max(RGB)."""
-    return 1.-self.rgb.min(axis = 0)/self.rgb.max(axis = 0, initial = IMGTOL) # Safe evaluation.
+    return colors.hsv_saturation(self.rgb)
 
   def luma(self):
-    """Return the (generalized) luma defined as the linear combination of the RGB components weighted by rgbluma."""
-    return rgbluma[0]*self.rgb[0]+rgbluma[1]*self.rgb[1]+rgbluma[2]*self.rgb[2]
+    """Return the luma."""
+    return colors.luma(self.rgb)
 
   def luma16(self):
-    """Return the luma as a (height, width) array of 16 bits integers in the range [0, 65535]."""
+    """Return the luma as 16 bits integers in the range [0, 65535]."""
     data = np.clip(self.luma()*65535, 0, 65535)
     return np.rint(data).astype("uint16")
 
   def rgb_to_hsv(self):
     """Return the hue/saturation/value (HSV) components as a (height, width, 3) array of floats."""
-    return IMGTYPE(colors.rgb_to_hsv(np.moveaxis(self.rgb, 0, -1)))
+    return colors.rgb_to_hsv(self.rgb)
 
   def set_hsv_image(self, hsv):
-    """Set RGB image from hue/saturation/value (HSV) data hsv(height, width, 3)."""
-    self.rgb = np.moveaxis(IMGTYPE(colors.hsv_to_rgb(hsv)), -1, 0)
+    """Set RGB image from the hue/saturation/value (HSV) data hsv(height, width, 3)."""
+    self.rgb = colors.hsv_to_rgb(hsv)
 
   def srgb_to_lrgb(self):
     """Return the linear RGB components of a sRGB image."""
-    srgb = np.clip(self.rgb, 0., 1.)
-    return np.where(srgb > 0.04045, ((srgb+0.055)/1.055)**2.4, srgb/12.92)
+    return colors.srgb_to_lrgb(self.rgb)
 
   def srgb_luminance(self):
     """Return the luminance Y of a sRGB image."""
-    lrgb = self.srgb_to_lrgb()
-    return 0.2126*lrgb[0]+0.7152*lrgb[1]+0.0722*lrgb[2]
+    return colors.srgb_luminance(self.rgb)
 
   def srgb_lightness(self):
     """Return the CIE lightness L* of a sRGB image."""
-    Y = self.srgb_luminance()
-    return np.where(Y > 0.008856, 116.*Y**(1./3.)-16., 903.3*Y)
+    return colors.srgb_lightness(self.rgb)
 
   def is_valid(self):
     """Return True if the object contains a valid RGB image, False otherwise."""
-    if not isinstance(self.rgb, np.ndarray): return False
-    if self.rgb.ndim != 3: return False
-    if self.rgb.shape[0] != 3: return False
-    if self.rgb.dtype != IMGTYPE: return False
-    return True
+    return utils.is_valid_rgb_image(self.rgb)
 
   def is_out_of_range(self):
     """Return True if the RGB image is out-of-range (data < 0 or > 1 in any channel), False otherwise."""
     return np.any(self.rgb < -IMGTOL) or np.any(self.rgb > 1.+IMGTOL)
 
   def is_gray_scale(self):
     """Return True if the image is a gray scale (same RGB channels), False otherwise."""
     return np.all(abs(self.rgb[1]-self.rgb[0]) < IMGTOL) and np.all(abs(self.rgb[2]-self.rgb[0]) < IMGTOL)
 
   # Object copies.
 
   def ref(self, meta = "self"):
     """Return a new Image object with a reference to the RGB image and new meta-data 'meta' (copy of the original if meta = "self")."""
     if meta == "self": meta = deepcopy(self.meta)
-    return self.newImage(self, self.rgb, meta)
+    return self.newImage(self, self.rgb, meta, copy = False)
 
   def clone(self, meta = "self"):
     """Return a new Image object with a copy of the RGB image and new meta-data 'meta' (copy of the original if meta = "self")."""
     if meta == "self": meta = deepcopy(self.meta)
-    return self.newImage(self, self.rgb.copy(), meta)
+    return self.newImage(self, self.rgb, meta, copy = True)
 
   def copy_image_from(self, source):
     """Copy the RGB image from 'source'."""
-    self.rgb = source.rgb.copy()
+    self.set_image(source.rgb, copy = True)
 
   def copy_meta_from(self, source):
     """Copy the meta-data from 'source'."""
     self.meta = deepcopy(source.meta)
 
   # Image load/save.
 
@@ -390,20 +375,20 @@
   ##########################
 
   # Image normalization.
 
   def scale_pixels(self, source, target):
     """Scale all pixels of the image by the ratio target/source.
        Wherever abs(source) < IMGTOL, set all channels to target."""
-    self.rgb = scale_pixels(self.rgb, source, target, cutoff = IMGTOL)
+    self.rgb = utils.scale_pixels(self.rgb, source, target)
 
   def protect_highlights(self, luma = None):
     """Normalize out-of-range pixels with HSV value > 1 by adjusting the saturation at constant luma.
        'luma' is the luma of the image, if available (if None, the luma is recomputed on the fly).
-       Warning: This method is aimed at protecting the highlights from overflowing when stretching the luma.
+       Warning: This method aims at protecting the highlights from overflowing when stretching the luma.
        It assumes that the luma remains <= 1 even though some pixels have HSV value > 1."""
     if luma is None: luma = self.luma() # Original luma.
     self.rgb /= np.maximum(self.rgb.max(axis = 0), 1.) # Rescale maximum HSV value to 1.
     newluma = self.luma() # Updated luma.
     # Scale the saturation.
     # Note: The following implementation is failsafe when newluma -> 1 (in which case luma is also 1 in principle),
     # at the cost of a small error.
@@ -421,15 +406,15 @@
        if 'inplace' is False."""
     if channels in ["V", "L"]:
       channel = self.value() if channels == "V" else self.luma()
       if shadow is None: shadow = max(channel.min(), 0.)
       if highlight is None: highlight = channel.max()
       clipped = np.clip(channel, shadow, highlight)
       interpd = np.interp(clipped, (shadow, highlight), (0., 1.))
-      image = scale_pixels(self.rgb, channel, interpd, cutoff = IMGTOL)
+      image = utils.scale_pixels(self.rgb, channel, interpd)
       if inplace: self.rgb = image
     else:
       image = self.rgb if inplace else self.rgb.copy()
       for ic, key in ((0, "R"), (1, "G"), (2, "B")):
         if key in channels:
           shadow_ = max(image[ic].min(), 0.) if shadow is None else shadow
           highlight_ = image[ic].max() if highlight is None else highlight
@@ -451,15 +436,15 @@
     if fr is not None:
       if fr[1] <= fr[0]: raise ValueError("Error, fr[1] must be > fr[0].")
     if to[1] <= to[0]: raise ValueError("Error, to[1] must be > to[0].")
     if channels in ["V", "L"]:
       channel = self.value() if channels == "V" else self.luma()
       fr_ = (channel.min(), channel.max()) if fr is None else fr
       interpd = np.maximum(np.interp(channel, fr_, to), 0.)
-      image = scale_pixels(self.rgb, channel, interpd, cutoff = IMGTOL)
+      image = utils.scale_pixels(self.rgb, channel, interpd)
       if inplace: self.rgb = image
     else:
       image = self.rgb if inplace else self.rgb.copy()
       for ic, key in ((0, "R"), (1, "G"), (2, "B")):
         if key in channels:
           fr_ = (image[ic].min(), image[ic].max()) if fr is None else fr
           image[ic] = np.maximum(np.interp(image[ic], fr_, to), 0.)
@@ -476,15 +461,15 @@
        Also set new meta-data 'meta' (same as the original if meta = "self"). Update the object if 'inplace'
        is True or return a new instance if 'inplace' is False."""
     if gamma <= 0.: raise ValueError("Error, gamma must be >= 0.")
     if channels in ["V", "L"]:
       channel = self.value() if channels == "V" else self.luma()
       clipped = np.clip(channel, 0., 1.)
       corrected = clipped**gamma
-      image = scale_pixels(self.rgb, channel, corrected, cutoff = IMGTOL)
+      image = utils.scale_pixels(self.rgb, channel, corrected)
       if inplace: self.rgb = image
     else:
       image = self.rgb if inplace else self.rgb.copy()
       for ic, key in ((0, "R"), (1, "G"), (2, "B")):
         if key in channels:
           clipped = np.clip(image[ic], 0., 1.)
           image[ic] = clipped**gamma
@@ -501,15 +486,15 @@
        Also set new meta-data 'meta' (same as the original if meta = "self"). Update the object if 'inplace'
        is True or return a new instance if 'inplace' is False."""
     if midtone <= 0.: raise ValueError("Error, midtone must be >= 0.")
     if channels in ["V", "L"]:
       channel = self.value() if channels == "V" else self.luma()
       clipped = np.clip(channel, 0., 1.)
       stretched = (midtone-1.)*clipped/((2.*midtone-1.)*clipped-midtone)
-      image = scale_pixels(self.rgb, channel, stretched, cutoff = IMGTOL)
+      image = utils.scale_pixels(self.rgb, channel, stretched)
       if inplace: self.rgb = image
     else:
       image = self.rgb if inplace else self.rgb.copy()
       for ic, key in ((0, "R"), (1, "G"), (2, "B")):
         if key in channels:
           clipped = np.clip(image[ic], 0., 1.)
           image[ic] = (midtone-1.)*clipped/((2.*midtone-1.)*clipped-midtone)
@@ -525,15 +510,15 @@
        by 'params'. The function stretch_function(input, params) shall return the output levels for an array of input
        levels 'input'. 'channels' can be "V" (value), "L" (luma) or any combination of "R" (red) "G" (green),
        and "B" (blue). Also set new meta-data 'meta' (same as the original if meta = "self"). Update the object
        if 'inplace' is True or return a new instance if 'inplace' is False."""
     if channels in ["V", "L"]:
       channel = self.value() if channels == "V" else self.luma()
       stretched = IMGTYPE(stretch_function(channel, params))
-      image = scale_pixels(self.rgb, channel, stretched, cutoff = IMGTOL)
+      image = utils.scale_pixels(self.rgb, channel, stretched)
       if inplace: self.rgb = image
     else:
       image = self.rgb if inplace else self.rgb.copy()
       for ic, key in ((0, "R"), (1, "G"), (2, "B")):
         if key in channels:
           image[ic] = IMGTYPE(stretch_function(image[ic], params))
     if inplace:
@@ -554,23 +539,23 @@
        The original image is clipped in the [0, 1] range before stretching."""
     xlut = np.linspace(0., 1., nlut, dtype = IMGTYPE) # Build the look-up table.
     ylut = IMGTYPE(stretch_function(xlut, params))
     slut = (ylut[1:]-ylut[:-1])/(xlut[1:]-xlut[:-1]) # Slopes.
     if channels in ["V", "L"]:
       channel = self.value() if channels == "V" else self.luma()
       clipped = np.clip(channel, 0., 1.)
-      stretched = lookup(clipped, xlut, ylut, slut, nlut)
-      image = scale_pixels(self.rgb, channel, stretched, cutoff = IMGTOL)
+      stretched = utils.lookup(clipped, xlut, ylut, slut, nlut)
+      image = utils.scale_pixels(self.rgb, channel, stretched)
       if inplace: self.rgb = image
     else:
       image = self.rgb if inplace else self.rgb.copy()
       for ic, key in ((0, "R"), (1, "G"), (2, "B")):
         if key in channels:
           clipped = np.clip(image[ic], 0., 1.)
-          image[ic] = lookup(clipped, xlut, ylut, slut, nlut)
+          image[ic] = utils.lookup(clipped, xlut, ylut, slut, nlut)
     if inplace:
       if meta != "self": self.meta = meta
       return None
     else:
       if meta == "self": meta = deepcopy(self.meta)
       return self.newImage(self, image, meta)
 
@@ -602,24 +587,32 @@
       self.rgb = image
       if meta != "self": self.meta = meta
       return None
     else:
       if meta == "self": meta = deepcopy(self.meta)
       return self.newImage(self, image, meta)
 
-  def gray_scale(self, inplace = True, meta = "self"):
-    """Convert to gray scale (using the luma) and set new meta-data 'meta' (same as the original if meta = "self").
+  def gray_scale(self, channel = "L", inplace = True, meta = "self"):
+    """Convert into a gray scale using channel = "V" (HSV value), "L" (luma) or "Y" (luminance),
+       and set new meta-data 'meta' (same as the original if meta = "self").
        Update the object if 'inplace' is True or return a new instance if False."""
     if inplace:
       if meta != "self": self.meta = meta
       image = self.rgb
     else:
       if meta == "self": meta = deepcopy(self.meta)
       image = np.empty_like(self.rgb)
-    image[:] = self.luma()
+    if channel == "V":
+      image[:] = self.value()
+    elif channel == "L":
+      image[:] = self.luma()
+    elif channel == "Y":
+      image[:] = colors.lrgb_to_srgb(self.srgb_luminance())
+    else:
+      raise ValueError(f"Error, invalid channel '{channel}'.")
     return None if inplace else self.newImage(self, image, meta)
 
   # Image enhancement.
 
   def sharpen(self, inplace = True, meta = "self"):
     """Apply a sharpening convolution filter and set new meta-data 'meta' (same
        as the original if meta = "self"). Update the object if 'inplace' is True or
```

### Comparing `eQuimage-1.3.0/src/eQuimage/imageprocessing/stretchfunctions.py` & `eQuimage-1.4.0/src/eQuimage/imageprocessing/stretchfunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
 
 """Histogram stretch functions."""
 
 import numpy as np
 
 def midtone_stretch_function(x_, params):
   """Return the midtone stretch function f(x_) for parameters 'params' = (shadow, midtone, highlight, low, high)."""
```

### Comparing `eQuimage-1.3.0/src/eQuimage/imageprocessing/utils.py` & `eQuimage-1.4.0/src/eQuimage/imageprocessing/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,42 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
 
 """Image processing utils."""
 
 import numpy as np
+from .defs import IMGTYPE, IMGTOL
+
+#############################
+# Generic image validation. #
+#############################
+
+def is_valid_rgb_image(image):
+  """Return True if 'image' is a valid RGB image, False otherwise."""
+  if not isinstance(image, np.ndarray): return False
+  if image.ndim != 3: return False
+  if image.shape[0] != 3: return False
+  if image.dtype != IMGTYPE: return False
+  return True
+
+###############################
+# Image manipulation helpers. #
+###############################
 
 def failsafe_divide(A, B):
   """Return A/B, ignoring errors (division by zero, ...)."""
   status = np.seterr(all = "ignore")
   C = np.divide(A, B)
   np.seterr(divide = status["divide"], over = status["over"], under = status["under"], invalid = status["invalid"])
   return C
 
-def scale_pixels(image, source, target, cutoff = 1.e-12):
+def scale_pixels(image, source, target, cutoff = IMGTOL):
   """Scale all pixels of the image 'image' by the ratio target/source.
      Wherever abs(source) < cutoff, set all channels to target."""
   return np.where(abs(source) > cutoff, failsafe_divide(image*target, source), target)
 
 def lookup(x, xlut, ylut, slut, nlut):
   """Return y = f(x) by linearly interpolating the values ylut = f(xlut) of an evenly spaced look-up table with nlut elements.
      slut = (ylut[1:]-ylut[:-1])/(xlut[1:]-xlut[:-1]) are the slopes used for linear interpolation between successive elements."""
```

### Comparing `eQuimage-1.3.0/src/eQuimage/images/splash.png` & `eQuimage-1.4.0/src/eQuimage/images/splash.png`

 * *Files identical despite different names*

### Comparing `eQuimage-1.3.0/src/eQuimage/windows/addframe.py` & `eQuimage-1.4.0/src/eQuimage/gui/tools/addframe.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
+# GUI updated.
 
 """Add Unistellar frame from an other image."""
 
 import os
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk
-from .gtk.customwidgets import Button, HoldButton, CheckButton, SpinButton
-from .gtk.filechoosers import ImageChooserDialog
-from .base import ErrorDialog
-from .tools import BaseToolWindow
-from ..imageprocessing import imageprocessing
-from ..imageprocessing.Unistellar import UnistellarImage as Image
+from ..gtk.customwidgets import Label, HBox, VBox, FramedHBox, Grid, Button, HoldButton, CheckButton, SpinButton
+from ..gtk.filechoosers import ImageFileChooserDialog
+from ..base import ErrorDialog
+from ..toolmanager import BaseToolWindow
+from ...imageprocessing import imageprocessing
 import matplotlib.pyplot as plt
 import numpy as np
 
 class AddUnistellarFrame(BaseToolWindow):
   """Add Unistellar frame tool class."""
 
-  __action__ = "Adding Unistellar frame..."
+  _action_ = "Adding Unistellar frame..."
 
   delay = 333 # Long press delay for "HoldButton".
   maxfade = 0.05 # Maximum fade.
 
   def open(self, image):
     """Open tool window for image 'image'."""
     if not super().open(image, "Add frame"): return False
-    filename = ImageChooserDialog(self.app.mainwindow.window, Gtk.FileChooserAction.OPEN, path = self.app.get_filename(), preview = True, title = "Open framed image")
+    filename = ImageFileChooserDialog(self.app.mainwindow.window, Gtk.FileChooserAction.OPEN, path = self.app.get_filename(), preview = True, title = "Open framed image")
     if filename is None:
       self.destroy()
       return False
     try:
-      image = Image()
+      image = self.app.ImageClass()
       image.load(filename)
     except Exception as err:
       ErrorDialog(self.window, str(err))
       self.destroy()
       return False
     framed = image.is_valid()
     if framed: framed = image.check_frame()
@@ -54,75 +54,58 @@
     self.fmargin = framed["margin"]
     self.fwidth, self.fheight = self.frame.size()
     self.xcenter = 0
     self.ycenter = 0
     self.currentscale = None
     self.currentmove = None
     self.currentfade = None
-    wbox = Gtk.VBox(spacing = 16)
+    wbox = VBox()
     self.window.add(wbox)
-    hbox = Gtk.HBox(spacing = 8)
-    wbox.pack_start(hbox, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = "Frame margin:"), False, False, 0)
     self.widgets.marginspin = SpinButton(self.fmargin, 0, self.fradius//4, 1, digits = 0)
     self.connect_update_request(self.widgets.marginspin, "value-changed")
-    hbox.pack_start(self.widgets.marginspin, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = "pixels"), False, False, 0)
-    hbox = Gtk.HBox(spacing = 8)
-    wbox.pack_start(hbox, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = "Fade length:"), False, False, 0)
+    wbox.pack(self.widgets.marginspin.hbox(prepend = "Frame margin:", append = "pixels"))
     self.widgets.fadespin = SpinButton(25, 0, 50, 1, digits = 1)
     self.connect_update_request(self.widgets.fadespin, "value-changed")
-    hbox.pack_start(self.widgets.fadespin, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = "% frame radius"), False, False, 0)
-    hbox = Gtk.HBox(spacing = 8)
-    wbox.pack_start(hbox, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = "Image scale:"), False, False, 0)
+    wbox.pack(self.widgets.fadespin.hbox(prepend = "Fade length:", append = "% frame radius"))
     self.widgets.scalespin = SpinButton(1., .25, 4., .01, digits = 3)
     self.connect_update_request(self.widgets.scalespin, "value-changed")
-    hbox.pack_start(self.widgets.scalespin, False, False, 0)
-    self.widgets.sizelabel = Gtk.Label(label = f" (0x0) px)")
-    hbox.pack_start(self.widgets.sizelabel, False, False, 0)
-    frame = Gtk.Frame(label = " Position ")
-    frame.set_label_align(0.025, 0.5)
-    wbox.pack_start(frame, False, False, 0)
-    hbox = Gtk.HBox()
-    frame.add(hbox)
-    grid = Gtk.Grid(margin = 16)
-    grid.set_column_homogeneous(True)
-    grid.set_row_homogeneous(True)
-    hbox.pack_start(grid, True, False, 0)
+    self.widgets.sizelabel = Label(" (0x0) px")
+    wbox.pack(self.widgets.scalespin.hbox(prepend = "Image scale:", append = self.widgets.sizelabel))
+    frame, hbox = FramedHBox(" Position ", margin = 32)
+    wbox.pack(frame)
+    grid = Grid(column_spacing = 0, column_homogeneous = True, row_spacing = 0, row_homogeneous = True)
+    hbox.pack(grid, expand = True)
     self.widgets.cbutton = Button(label = "\u2022")
     self.widgets.cbutton.connect("clicked", lambda button: self.center_image())
-    grid.add(self.widgets.cbutton)
+    grid.attach(self.widgets.cbutton, 1, 1)
     self.widgets.ubutton = HoldButton(delay = self.delay)
     self.widgets.ubutton.add(Gtk.Arrow(arrow_type = Gtk.ArrowType.UP, shadow_type = Gtk.ShadowType.NONE))
     self.widgets.ubutton.connect("hold", lambda button: self.move_image(0, +10))
     self.widgets.ubutton.connect("clicked", lambda button: self.move_image(0, +1))
-    grid.attach_next_to(self.widgets.ubutton, self.widgets.cbutton, Gtk.PositionType.TOP, 1, 1)
+    grid.attach(self.widgets.ubutton, 1, 0)
     self.widgets.dbutton = HoldButton(delay = self.delay)
     self.widgets.dbutton.add(Gtk.Arrow(arrow_type = Gtk.ArrowType.DOWN, shadow_type = Gtk.ShadowType.NONE))
     self.widgets.dbutton.connect("hold", lambda button: self.move_image(0, -10))
     self.widgets.dbutton.connect("clicked", lambda button: self.move_image(0, -1))
-    grid.attach_next_to(self.widgets.dbutton, self.widgets.cbutton, Gtk.PositionType.BOTTOM, 1, 1)
+    grid.attach(self.widgets.dbutton, 1, 2)
     self.widgets.lbutton = HoldButton(delay = self.delay)
     self.widgets.lbutton.add(Gtk.Arrow(arrow_type = Gtk.ArrowType.LEFT, shadow_type = Gtk.ShadowType.NONE))
     self.widgets.lbutton.connect("hold", lambda button: self.move_image(-10, 0))
     self.widgets.lbutton.connect("clicked", lambda button: self.move_image(-1, 0))
-    grid.attach_next_to(self.widgets.lbutton, self.widgets.cbutton, Gtk.PositionType.LEFT, 1, 1)
+    grid.attach(self.widgets.lbutton, 0, 1)
     self.widgets.rbutton = HoldButton(delay = self.delay)
     self.widgets.rbutton.add(Gtk.Arrow(arrow_type = Gtk.ArrowType.RIGHT, shadow_type = Gtk.ShadowType.NONE))
     self.widgets.rbutton.connect("hold", lambda button: self.move_image(+10, 0))
     self.widgets.rbutton.connect("clicked", lambda button: self.move_image(+1, 0))
-    grid.attach_next_to(self.widgets.rbutton, self.widgets.cbutton, Gtk.PositionType.RIGHT, 1, 1)
+    grid.attach(self.widgets.rbutton, 2, 1)
     self.widgets.gbutton = CheckButton(label = "Show guide lines")
     self.widgets.gbutton.set_active(False)
     self.widgets.gbutton.connect("toggled", lambda button: self.update_guide_lines(self.get_params()))
-    wbox.pack_start(self.widgets.gbutton, False, False, 0)
-    wbox.pack_start(self.tool_control_buttons(model = "onthefly"), False, False, 0)
+    wbox.pack(self.widgets.gbutton)
+    wbox.pack(self.tool_control_buttons(model = "onthefly"))
     self.start(identity = False)
     return True
 
   def center_image(self):
     """Center image."""
     self.xcenter = 0
     self.ycenter = 0
```

### Comparing `eQuimage-1.3.0/src/eQuimage/windows/arcsinh.py` & `eQuimage-1.4.0/src/eQuimage/gui/tools/arcsinh.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,68 +1,65 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
+# GUI updated.
 
 """Arcsinh stretch tool."""
 
-import gi
-gi.require_version("Gtk", "3.0")
-from gi.repository import Gtk
-from .gtk.customwidgets import CheckButton, SpinButton
 from .stretch import StretchTool
-from ..imageprocessing import imageprocessing
-from ..imageprocessing.stretchfunctions import arcsinh_stretch_function
-import numpy as np
+from ..gtk.customwidgets import HBox, VBox, CheckButton, SpinButton
+from ...imageprocessing import imageprocessing
+from ...imageprocessing.stretchfunctions import arcsinh_stretch_function
 
 class ArcsinhStretchTool(StretchTool):
   """Arcsinh stretch tool class, derived from the StretchTool class."""
 
-  __action__ = "Stretching histograms (arcsinh stretch function)..."
+  _action_ = "Stretching histograms (arcsinh stretch function)..."
 
   # Build window.
 
-  __window_name__ = "Arcsinh stretch"
+  _window_name_ = "Arcsinh stretch"
 
   def options_widgets(self, widgets):
-    """Return a Gtk box with tool options widgets and store the reference to these widgets in container 'widgets'.
+    """Return a box with tool options widgets and store the reference to these widgets in container 'widgets'.
        Return None if there are no tool options widgets."""
-    hbox = Gtk.HBox(spacing = 8)
+    hbox = HBox()
     widgets.bindbutton = CheckButton(label = "Bind RGB channels")
     widgets.bindbutton.set_active(True)
     widgets.bindbutton.connect("toggled", lambda button: self.update("bindrgb"))
-    hbox.pack_start(widgets.bindbutton, True, True, 0)
+    hbox.pack(widgets.bindbutton, expand = True, fill = True)
     return hbox
 
   def tab_widgets(self, key, widgets):
-    """Return a Gtk box with tab widgets for channel 'key' in "R" (red), "G" (green), "B" (blue), "S" (saturation), "V" (value) or "L" (luma),
+    """Return a box with tab widgets for channel 'key' in "R" (red), "G" (green), "B" (blue), "S" (saturation), "V" (value) or "L" (luma),
        and store the reference to these widgets in container 'widgets'.
        Return None if there is no tab for this channel."""
     if not key in ["R", "G", "B", "V", "L"]: return None
     percentiles = self.reference.stats["L"].percentiles
     step = (percentiles[2]-percentiles[0])/20. if percentiles is not None else .01
     step = min(max(step, .0001), .01)
-    cbox = Gtk.VBox(margin = 16, spacing = 16)
-    hbox = Gtk.HBox(spacing = 8)
-    cbox.pack_start(hbox, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = "Shadow:"), False, False, 0)
+    cbox = VBox(margin = 16)
+    hbox = HBox()
+    cbox.pack(hbox)
     widgets.shadowspin = SpinButton(0., 0., .99, step, digits = 5)
     widgets.shadowspin.connect("value-changed", lambda button: self.update("shadow"))
-    hbox.pack_start(widgets.shadowspin, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = 8*" "+"Stretch factor:"), False, False, 0)
+    hbox.pack("Shadow:")
+    hbox.pack(widgets.shadowspin)
     widgets.stretchspin = SpinButton(0., 0., 1000., 1., digits = 1)
     widgets.stretchspin.connect("value-changed", lambda button: self.update("stretch"))
-    hbox.pack_start(widgets.stretchspin, False, False, 0)
+    hbox.pack(8*" "+"Stretch factor:")
+    hbox.pack(widgets.stretchspin)
     if key == "L":
-      hbox.pack_start(Gtk.Label(label = 8*" "), False, False, 0)
       widgets.highlightsbutton = CheckButton(label = "Protect highlights")
       widgets.highlightsbutton.set_active(False)
       widgets.highlightsbutton.connect("toggled", lambda button: self.update(None))
-      hbox.pack_start(widgets.highlightsbutton, False, False, 0)
+      hbox.pack(8*" ")
+      hbox.pack(widgets.highlightsbutton)
     return cbox
 
   # Tool methods.
 
   def get_params(self):
     """Return tool parameters."""
     params = {}
@@ -105,19 +102,19 @@
 
   def operation(self, params):
     """Return tool operation string for parameters 'params'."""
     operation = "ArcsinhStretch("
     separator = ""
     for key in self.channelkeys:
       shadow, stretch = params[key]
-      if key != "L":
-        operation += f"{separator}{key} : (shadow = {shadow:.5f}, stretch = {stretch:.1f})"
-      else:
+      if key == "L":
         red, green, blue = params["rgbluma"]
         operation += f"{separator}L({red:.2f}, {green:.2f}, {blue:.2f}) : (shadow = {shadow:.5f}, stretch = {stretch:.1f})"
+      else:
+        operation += f"{separator}{key} : (shadow = {shadow:.5f}, stretch = {stretch:.1f})"
       separator = ", "
     if params["highlights"]: operation += ", protect highlights"
     operation += ")"
     return operation
 
   # Plot histograms, stretch function, display stats...
```

### Comparing `eQuimage-1.3.0/src/eQuimage/windows/base.py` & `eQuimage-1.4.0/src/eQuimage/gui/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
+# GUI updated.
 
 """Base window classes and widgets."""
 
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk
+from .gtk.utils import Container
+from matplotlib.backends.backend_gtk3agg import FigureCanvasGTK3Agg as FigureCanvas
 from matplotlib.backends.backend_gtk3 import NavigationToolbar2GTK3 as NavigationToolbar
 
-class Container:
-  """Empty class as a container."""
-  pass
-
 class BaseWindow:
   """Generic application window."""
 
   def __init__(self, app):
     """Bind the window with application 'app'."""
     self.app = app
     self.opened = False
```

### Comparing `eQuimage-1.3.0/src/eQuimage/windows/bilateral.py` & `eQuimage-1.4.0/src/eQuimage/gui/tools/bilateral.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
+# GUI updated.
 
 """Bilateral filter tool."""
 
-import gi
-gi.require_version("Gtk", "3.0")
-from gi.repository import Gtk, Gdk
-from .gtk.customwidgets import HScaleSpinButton
-from .tools import BaseToolWindow
+from ..gtk.customwidgets import HBox, VBox, HScaleSpinButton
+from ..toolmanager import BaseToolWindow
 from skimage.restoration import denoise_bilateral
 
 class BilateralFilterTool(BaseToolWindow):
   """Bilateral filter tool class."""
 
-  __action__ = "Bilateral filtering..."
+  _action_ = "Applying bilateral filter..."
 
-  __onthefly__ = False # This transformation can not be applied on the fly.
+  _onthefly_ = False # This transformation can not be applied on the fly.
 
   def open(self, image):
     """Open tool window for image 'image'."""
     if not super().open(image, "Bilateral filter"): return False
-    wbox = Gtk.VBox(spacing = 16)
+    wbox = VBox()
     self.window.add(wbox)
-    self.widgets.colorscale = HScaleSpinButton(.05, 0., .2, .001, digits = 3, length = 320, expand = False)
-    wbox.pack_start(self.widgets.colorscale.layout2("\u03c3 color:"), False, False, 0)
+    self.widgets.colorscale = HScaleSpinButton(.1, 0., .5, .001, digits = 3, length = 320, expand = False)
+    wbox.pack(self.widgets.colorscale.layout2("\u03c3 color:"))
     self.widgets.spacescale = HScaleSpinButton(5., 0., 20., .01, digits = 2, length = 320, expand = False)
-    wbox.pack_start(self.widgets.spacescale.layout2("\u03c3 space (pixels):"), False, False, 0)
-    wbox.pack_start(self.tool_control_buttons(), False, False, 0)
+    wbox.pack(self.widgets.spacescale.layout2("\u03c3 space (pixels):"))
+    wbox.pack(self.tool_control_buttons())
     self.start(identity = False)
     return True
 
   def get_params(self):
     """Return tool parameters."""
     return self.widgets.colorscale.get_value(), self.widgets.spacescale.get_value()
```

### Comparing `eQuimage-1.3.0/src/eQuimage/windows/blackpoint.py` & `eQuimage-1.4.0/src/eQuimage/gui/tools/blackpoint.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,55 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
+# GUI updated.
 
 """Black point adjustment tool."""
 
-import gi
-gi.require_version("Gtk", "3.0")
-from gi.repository import Gtk
-from .gtk.customwidgets import CheckButton, SpinButton
 from .stretch import StretchTool
-from ..imageprocessing import imageprocessing
-from ..imageprocessing.stretchfunctions import blackpoint_stretch_function
-import numpy as np
+from ..gtk.customwidgets import HBox, VBox, CheckButton, SpinButton
+from ...imageprocessing import imageprocessing
+from ...imageprocessing.stretchfunctions import blackpoint_stretch_function
 
 class BlackPointTool(StretchTool):
   """Black point adjustment tool class, derived from the StretchTool class."""
 
-  __action__ = "Adjusting black point..."
+  _action_ = "Adjusting black point..."
 
   # Build window.
 
-  __window_name__ = "Black point"
+  _window_name_ = "Black point"
 
   def options_widgets(self, widgets):
-    """Return a Gtk box with tool options widgets and store the reference to these widgets in container 'widgets'.
+    """Return a box with tool options widgets and store the reference to these widgets in container 'widgets'.
        Return None if there are no tool options widgets."""
-    hbox = Gtk.HBox(spacing = 8)
+    hbox = HBox()
     widgets.bindbutton = CheckButton(label = "Bind RGB channels")
     widgets.bindbutton.set_active(True)
     widgets.bindbutton.connect("toggled", lambda button: self.update("bindrgb"))
-    hbox.pack_start(widgets.bindbutton, True, True, 0)
+    hbox.pack(widgets.bindbutton, expand = True, fill = True)
     return hbox
 
   def tab_widgets(self, key, widgets):
-    """Return a Gtk box with tab widgets for channel 'key' in "R" (red), "G" (green), "B" (blue), "S" (saturation), "V" (value) or "L" (luma),
+    """Return a box with tab widgets for channel 'key' in "R" (red), "G" (green), "B" (blue), "S" (saturation), "V" (value) or "L" (luma),
        and store the reference to these widgets in container 'widgets'.
        Return None if there is no tab for this channel."""
     if not key in ["R", "G", "B", "V", "L"]: return None
     percentiles = self.reference.stats["L"].percentiles
     step = (percentiles[2]-percentiles[0])/20. if percentiles is not None else .01
     step = min(max(step, .0001), .01)
-    cbox = Gtk.VBox(margin = 16, spacing = 16)
-    hbox = Gtk.HBox(spacing = 8)
-    cbox.pack_start(hbox, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = "Shadow:"), False, False, 0)
+    cbox = VBox(margin = 16)
+    hbox = HBox()
+    cbox.pack(hbox)
     widgets.shadowspin = SpinButton(0., 0., .99, step, digits = 5)
     widgets.shadowspin.connect("value-changed", lambda button: self.update("shadow"))
-    hbox.pack_start(widgets.shadowspin, False, False, 0)
+    hbox.pack("Shadow:")
+    hbox.pack(widgets.shadowspin)
     return cbox
 
   # Tool methods.
 
   def get_params(self):
     """Return tool parameters."""
     params = {}
@@ -90,19 +87,19 @@
 
   def operation(self, params):
     """Return tool operation string for parameters 'params'."""
     operation = "BlackPoint("
     separator = ""
     for key in self.channelkeys:
       shadow = params[key]
-      if key != "L":
-        operation += f"{separator}{key} = {shadow:.5f}"
-      else:
+      if key == "L":
         red, green, blue = params["rgbluma"]
         operation += f"{separator}L({red:.2f}, {green:.2f}, {blue:.2f}) = {shadow:.5f}"
+      else:
+        operation += f"{separator}{key} = {shadow:.5f}"
       separator = ", "
     operation += ")"
     return operation
 
   # Plot histograms, stretch function, display stats...
 
   def stretch_function(self, t, params):
```

### Comparing `eQuimage-1.3.0/src/eQuimage/windows/blend.py` & `eQuimage-1.4.0/src/eQuimage/gui/tools/blend.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,94 +1,84 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
+# GUI updated.
 
 """Blend tool."""
 
-import gi
-gi.require_version("Gtk", "3.0")
-from gi.repository import Gtk
-from .gtk.customwidgets import CheckButton, HScale
-from .gtk.filechoosers import ImageChooserDialog
-from .base import ErrorDialog
-from .tools import BaseToolWindow
-from .picker import ImagePicker
+from ..gtk.customwidgets import Align, Label, HBox, VBox, Grid, CheckButton, HScale
+from ..misc.imagechooser import ImageChooser
+from ..toolmanager import BaseToolWindow
 import numpy as np
 
 class BlendTool(BaseToolWindow):
   """Blend tool window class."""
 
-  __action__ = "Blending images..."
+  _action_ = "Blending images..."
 
   def open(self, image):
     """Open tool window for image 'image'."""
     if not super().open(image, "Blend images"): return False
-    wbox = Gtk.VBox(spacing = 16)
+    wbox = VBox()
     self.window.add(wbox)
-    wbox.pack_start(Gtk.Label("Choose image to blend with:", halign = Gtk.Align.START), False, False, 0)
-    self.widgets.picker = ImagePicker(self.app, self.window, wbox, lambda row, image: self.update("image"))
-    hbox = Gtk.HBox(spacing = 8)
-    wbox.pack_start(hbox, False, False, 0)
-    self.message = Gtk.Label(halign = Gtk.Align.START)
-    self.set_message()
-    hbox.pack_start(self.message, False, False, 0)
-    hbox = Gtk.HBox(spacing = 8)
-    wbox.pack_start(hbox, False, False, 0)
-    hbox.pack_start(Gtk.Label("Mixing factors:"), False, False, 0)
-    self.widgets.bindbutton = CheckButton(label = "Bind RGB channels", halign = Gtk.Align.END)
+    wbox.pack("Choose image to blend with:")
+    self.widgets.chooser = ImageChooser(self.app, self.window, wbox, callback = lambda row, image: self.update("image"))
+    self.message = Label(" ")
+    wbox.pack(self.message)
+    hbox = HBox()
+    wbox.pack(hbox)
+    hbox.pack("Mixing factors:")
+    self.widgets.bindbutton = CheckButton(label = "Bind RGB channels", halign = Align.END)
     self.widgets.bindbutton.set_active(True)
     self.widgets.bindbutton.connect("toggled", lambda button: self.update(0))
-    hbox.pack_start(self.widgets.bindbutton, True, True, 0)
-    grid = Gtk.Grid(column_spacing = 8)
-    wbox.pack_start(grid, False, False, 0)
+    hbox.pack(self.widgets.bindbutton, expand = True, fill = True)
+    grid = Grid()
+    wbox.pack(grid)
     self.widgets.mixingscales = []
     self.widgets.zerobuttons = []
     for channel, label in ((0, "Red:"), (1, "Green:"), (2, "Blue:")):
       mixingscale = HScale(.5, -1., 2., .01, digits = 2, marks = [-1., 0., 1., 2.], length = 320)
       mixingscale.channel = channel
       mixingscale.connect("value-changed", lambda scale: self.update(scale.channel))
-      if not self.widgets.mixingscales:
-        grid.add(mixingscale)
-      else:
-        grid.attach_next_to(mixingscale, self.widgets.mixingscales[-1], Gtk.PositionType.BOTTOM, 1, 1)
       self.widgets.mixingscales.append(mixingscale)
-      grid.attach_next_to(Gtk.Label(label = label, halign = Gtk.Align.END), mixingscale, Gtk.PositionType.LEFT, 1, 1)
-      zerobutton = CheckButton(label = "Zero is transparent", halign = Gtk.Align.START)
+      zerobutton = CheckButton(label = "Zero is transparent")
       zerobutton.channel = channel
       zerobutton.connect("toggled", lambda button: self.update(button.channel))
-      grid.attach_next_to(zerobutton, mixingscale, Gtk.PositionType.RIGHT, 1, 1)
       self.widgets.zerobuttons.append(zerobutton)
-    wbox.pack_start(self.tool_control_buttons(reset = False), False, False, 0)
+      grid.attach(Label(label, halign = Align.END), 0, channel)
+      grid.attach(mixingscale, 1, channel)
+      grid.attach(zerobutton, 2, channel)
+    wbox.pack(self.tool_control_buttons(reset = False))
     self.start(identity = True)
     return True
 
   def get_params(self):
     """Return tool parameters."""
-    row = self.widgets.picker.get_selected_row()
+    row = self.widgets.chooser.get_selected_row()
     mixings = tuple(self.widgets.mixingscales[channel].get_value() for channel in range(3))
     zeros = tuple(self.widgets.zerobuttons[channel].get_active() for channel in range(3))
     return row, mixings, zeros
 
   def set_params(self, params):
     """Set tool parameters 'params'."""
     row, mixings, zeros = params
-    self.widgets.picker.set_selected_row(row)
+    self.widgets.chooser.set_selected_row(row)
     for channel in range(3):
       self.widgets.mixingscales[channel].set_value(mixings[channel])
       self.widgets.zerobuttons[channel].set_active(zeros[channel])
     if mixings[1] != mixings[0] or mixings[2] != mixings[0]: self.widgets.bindbutton.set_active_block(False)
     if zeros[1] != zeros[0] or zeros[2] != zeros[0]: self.widgets.bindbutton.set_active_block(False)
 
   def run(self, params):
     """Run tool for parameters 'params'."""
     row, mixings, zeros = params
     if row < 0: return params, False
-    selection = self.widgets.picker.get_image(row)
+    selection = self.widgets.chooser.get_image(row)
     if selection.size() != self.reference.size():
       self.set_message("<span foreground='red'>Can not blend images with different sizes.</span>")
       return params, False
     self.set_message()
     for channel in range(3):
       mixing = mixings[channel]
       transparent = zeros[channel]
@@ -99,19 +89,19 @@
         self.image.rgb[channel] = blended
     return params, True
 
   def operation(self, params):
     """Return tool operation string for parameters 'params'."""
     row, mixings, zeros = params
     if row < 0: return None
-    operation = f"Blend({self.widgets.picker.get_image_tag(row)}"
+    operation = f"Blend({self.widgets.chooser.get_image_tag(row)}"
     for channel in range(3):
       key = ["R", "G", "B"][channel]
       decoration = "'" if zeros[channel] else ""
-      operation += f", {key}{decoration} = {mixings[channel]}"
+      operation += f", {key}{decoration} = {mixings[channel]:.2f}"
     operation += ")"
     return operation
 
   # Update widgets.
 
   def update(self, changed):
     """Update widgets on change of 'changed'."""
```

### Comparing `eQuimage-1.3.0/src/eQuimage/windows/clahe.py` & `eQuimage-1.4.0/src/eQuimage/gui/tools/clahe.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,87 +1,69 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
+# GUI updated.
 
 """Contrast Limited Adaptive Histogram Equalization (CLAHE) tool."""
 
-import gi
-gi.require_version("Gtk", "3.0")
-from gi.repository import Gtk, Gdk
-from .gtk.customwidgets import RadioButton, SpinButton, HScale
-from .tools import BaseToolWindow
-from ..imageprocessing import imageprocessing
+from ..gtk.customwidgets import HBox, VBox, RadioButtons, SpinButton, HScale
+from ..toolmanager import BaseToolWindow
+from ...imageprocessing import imageprocessing
 from skimage.exposure import equalize_adapthist
-import numpy as np
 
 class CLAHETool(BaseToolWindow):
   """Contrast Limited Adaptive Histogram Equalization (CLAHE) tool class."""
 
-  __action__ = "Running Contrast Limited Adaptive Histogram Equalization (CLAHE)..."
+  _action_ = "Running Contrast Limited Adaptive Histogram Equalization (CLAHE)..."
 
-  __onthefly__ = False # This transformation can not be applied on the fly.
+  _onthefly_ = False # This transformation can not be applied on the fly.
 
   def open(self, image):
     """Open tool window for image 'image'."""
     if not super().open(image, "Contrast Limited Adaptive Histogram Equalization (CLAHE)"): return False
-    wbox = Gtk.VBox(spacing = 16)
+    wbox = VBox()
     self.window.add(wbox)
-    hbox = Gtk.HBox(spacing = 8)
-    wbox.pack_start(hbox, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = "Channel(s):"), False, False, 0)
-    self.widgets.valuebutton = RadioButton.new_with_label_from_widget(None, "HSV value")
-    hbox.pack_start(self.widgets.valuebutton, False, False, 0)
-    self.widgets.lumabutton = RadioButton.new_with_label_from_widget(self.widgets.valuebutton, "Luma")
-    hbox.pack_start(self.widgets.lumabutton, False, False, 0)
-    hbox = Gtk.HBox(spacing = 8)
-    wbox.pack_start(hbox, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = "Kernel size: ", halign = Gtk.Align.START), False, False, 0)
+    self.widgets.channelbuttons = RadioButtons(("V", "HSV value"), ("L", "Luma"))
+    wbox.pack(self.widgets.channelbuttons.hbox(prepend = "Channel:"))
     self.widgets.sizebutton = SpinButton(15., 1., 100., 1., digits = 0)
-    hbox.pack_start(self.widgets.sizebutton, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = "% image width and height", halign = Gtk.Align.START), False, False, 0)
-    hbox = Gtk.HBox(spacing = 8)
-    wbox.pack_start(hbox, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = "Clip limit:"), False, False, 0)
+    wbox.pack(self.widgets.sizebutton.hbox(prepend = "Kernel size: ", append = "% image width and height"))
     self.widgets.clipscale = HScale(.5, 0., 1., 0.01, digits = 2, marks = [0., 1.], length = 320, expand = False)
-    hbox.pack_start(self.widgets.clipscale, False, False, 0)
-    wbox.pack_start(self.tool_control_buttons(), False, False, 0)
+    wbox.pack(self.widgets.clipscale.hbox(prepend = "Clip limit:"))
+    wbox.pack(self.tool_control_buttons())
     self.start(identity = False)
     return True
 
   def get_params(self):
     """Return tool parameters."""
-    channels = "V" if self.widgets.valuebutton.get_active() else "L"
-    return channels, self.widgets.sizebutton.get_value(), self.widgets.clipscale.get_value(), imageprocessing.get_rgb_luma()
+    return self.widgets.channelbuttons.get_selected(), self.widgets.sizebutton.get_value(), \
+           self.widgets.clipscale.get_value(), imageprocessing.get_rgb_luma()
 
   def set_params(self, params):
     """Set tool parameters 'params'."""
-    channels, size, clip, rgbluma = params
-    if channels == "V":
-      self.widgets.valuebutton.get_active(True)
-    else:
-      self.widgets.lumabutton.set_active(True)
+    channel, size, clip, rgbluma = params
+    self.widgets.channelbuttons.set_selected(channel)
     self.widgets.sizebutton.set_value(size)
     self.widgets.clipscale.set_value(clip)
 
   def run(self, params):
     """Run tool for parameters 'params'."""
-    channels, size, clip, rgbluma = params
+    channel, size, clip, rgbluma = params
     if size <= 0. or clip <= 0.: return params, False
     width, height = self.reference.size()
     kwidth = max(int(round(size*width/100.)), 3)
     kheight = max(int(round(size*height/100.)), 3)
-    if channels == "V":
-      self.image.set_image(equalize_adapthist(self.reference.rgbf(), kernel_size = (kheight, kwidth), clip_limit = clip), channel = -1, copy = True)
+    if channel == "V":
+      self.image.set_image(equalize_adapthist(self.reference.rgbf_view(), kernel_size = (kheight, kwidth), clip_limit = clip), channels = -1)
     else:
       ref = self.reference.luma()
       img = equalize_adapthist(ref, kernel_size = (kheight, kwidth), clip_limit = clip)
       self.image.copy_image_from(self.reference)
       self.image.scale_pixels(ref, img)
     return params, True
 
   def operation(self, params):
     """Return tool operation string for parameters 'params'."""
-    channels, size, clip, rgbluma = params
-    if channels == "L": channels = f"L({rgbluma[0]:.2f}, {rgbluma[1]:.2f}, {rgbluma[2]:.2f})"
-    return f"CLAHE({channels}, size = {size:.0f}%, clip = {clip:.2f})"
+    channel, size, clip, rgbluma = params
+    if channel == "L": channel = f"L({rgbluma[0]:.2f}, {rgbluma[1]:.2f}, {rgbluma[2]:.2f})"
+    return f"CLAHE(channel = {channel}, size = {size:.0f}%, clip = {clip:.2f})"
```

### Comparing `eQuimage-1.3.0/src/eQuimage/windows/colorbalance.py` & `eQuimage-1.4.0/src/eQuimage/gui/tools/colorbalance.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
+# GUI updated.
 
 """Color balance tool."""
 
-import gi
-gi.require_version("Gtk", "3.0")
-from gi.repository import Gtk
-from .gtk.customwidgets import SpinButton
-from .tools import BaseToolWindow
+from ..gtk.customwidgets import HBox, VBox, SpinButton
+from ..toolmanager import BaseToolWindow
 
 class ColorBalanceTool(BaseToolWindow):
   """Color balance tool class."""
 
-  __action__ = "Balancing colors..."
+  _action_ = "Balancing colors..."
 
   def open(self, image):
     """Open tool window for image 'image'."""
     if not super().open(image, "Color balance"): return False
-    wbox = Gtk.VBox(spacing = 16)
+    wbox = VBox()
     self.window.add(wbox)
-    hbox = Gtk.HBox(spacing = 8)
-    wbox.pack_start(hbox, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = "Red:"), False, False, 0)
+    hbox = HBox()
+    wbox.pack(hbox)
     self.widgets.redspin = SpinButton(1., 0., 2., 0.01)
-    hbox.pack_start(self.widgets.redspin, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = 8*" "+"Green:"), False, False, 0)
+    hbox.pack("Red:")
+    hbox.pack(self.widgets.redspin)
     self.widgets.greenspin = SpinButton(1., 0., 2., 0.01)
-    hbox.pack_start(self.widgets.greenspin, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = 8*" "+"Blue:"), False, False, 0)
+    hbox.pack(8*" "+"Green:")
+    hbox.pack(self.widgets.greenspin)
     self.widgets.bluespin = SpinButton(1., 0., 2., 0.01)
-    hbox.pack_start(self.widgets.bluespin, False, False, 0)
-    wbox.pack_start(self.tool_control_buttons(), False, False, 0)
+    hbox.pack(8*" "+"Blue:")
+    hbox.pack(self.widgets.bluespin)
+    wbox.pack(self.tool_control_buttons())
     if self.onthefly:
       self.connect_update_request(self.widgets.redspin  , "value-changed")
       self.connect_update_request(self.widgets.greenspin, "value-changed")
       self.connect_update_request(self.widgets.bluespin , "value-changed")
     self.start(identity = True)
     return True
```

### Comparing `eQuimage-1.3.0/src/eQuimage/windows/colorsaturation.py` & `eQuimage-1.4.0/src/eQuimage/gui/tools/ghscolorsat.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,227 +1,208 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
+# GUI updated.
 
-"""Color saturation tool."""
+"""Hyperbolic color saturation stretch tool."""
 
-import gi
-gi.require_version("Gtk", "3.0")
-from gi.repository import Gtk
-from .gtk.customwidgets import CheckButton, RadioButton, HScaleSpinButton
-from .tools import BaseToolWindow
-import numpy as np
-import matplotlib.colors as colors
-import matplotlib.ticker as ticker
-from matplotlib.backends.backend_gtk3agg import FigureCanvasGTK3Agg as FigureCanvas
-from matplotlib.figure import Figure
-from scipy.interpolate import interp1d, splrep, splev
-
-class ColorSaturationTool(BaseToolWindow):
-  """Color saturation tool class."""
-
-  __action__ = "Enhancing color saturation..."
-
-  def open(self, image):
-    """Open tool window for image 'image'."""
-    if not super().open(image, "Color saturation"): return False
+from .stretch import StretchTool
+from ..gtk.customwidgets import HBox, VBox, CheckButton, SpinButton
+from ...imageprocessing import imageprocessing
+from ...imageprocessing.stretchfunctions import ghyperbolic_stretch_function
+
+class GHSColorSaturationTool(StretchTool):
+  """Color saturation generalized hyperbolic stretch tool class, derived from the StretchTool class.
+     Adapted from hyperbolic.py/GeneralizedHyperbolicStretchTool."""
+
+  _action_ = "Stretching color saturation (generalized hyperbolic stretch function)..."
+
+  # Build window.
+
+  _window_name_ = "Color saturation generalized hyperbolic stretch"
+
+  def options_widgets(self, widgets):
+    """Return a box with tool options widgets and store the reference to these widgets in container 'widgets'.
+       Return None if there are no tool options widgets."""
+    hbox = HBox()
+    widgets.inversebutton = CheckButton(label = "Inverse transformation")
+    widgets.inversebutton.set_active(False)
+    widgets.inversebutton.connect("toggled", lambda button: self.update("inverse"))
+    hbox.pack(widgets.inversebutton)
+    return hbox
+
+  def tab_widgets(self, key, widgets):
+    """Return a box with tab widgets for channel 'key' in "R" (red), "G" (green), "B" (blue), "S" (saturation), "V" (value) or "L" (luma),
+       and store the reference to these widgets in container 'widgets'.
+       Return None if there is no tab for this channel."""
+    if key != "S": return None
+    cbox = VBox(margin = 16)
+    hbox = HBox()
+    cbox.pack(hbox)
+    widgets.logD1spin = SpinButton(0., 0., 10., .1, digits = 3)
+    widgets.logD1spin.connect("value-changed", lambda button: self.update("D"))
+    hbox.pack("Global log(D+1):")
+    hbox.pack(widgets.logD1spin)
+    widgets.Bspin = SpinButton(0, -5., 15., .1, digits = 3)
+    widgets.Bspin.connect("value-changed", lambda button: self.update("B"))
+    hbox.pack(5*" "+"Local B:")
+    hbox.pack(widgets.Bspin)
+    widgets.SYPspin = SpinButton(.5, 0., 1., .01, digits = 5)
+    widgets.SYPspin.connect("value-changed", lambda button: self.update("SYP"))
+    hbox.pack(5*" "+"Symmetry point:")
+    hbox.pack(widgets.SYPspin)
+    hbox = HBox()
+    cbox.pack(hbox)
+    widgets.SPPspin = SpinButton(0., 0., .99, .01, digits = 5)
+    widgets.SPPspin.connect("value-changed", lambda button: self.update("SPP"))
+    hbox.pack("Shadow protection point:")
+    hbox.pack(widgets.SPPspin)
+    widgets.HPPspin = SpinButton(1., .01, 1., .01, digits = 5)
+    widgets.HPPspin.connect("value-changed", lambda button: self.update("HPP"))
+    hbox.pack(5*" "+"Highlight protection point:")
+    hbox.pack(widgets.HPPspin)
+    return cbox
+
+  def start(self, *args, **kwargs):
+    """Compute the HSV components of the reference image before starting the tool."""
     self.reference.hsv = self.reference.rgb_to_hsv()
-    wbox = Gtk.VBox(spacing = 16)
-    self.window.add(wbox)
-    hbox = Gtk.HBox(spacing = 16)
-    wbox.pack_start(hbox, False, False, 0)
-    self.widgets.fig = Figure(figsize = (6., 6.))
-    canvas = FigureCanvas(self.widgets.fig)
-    canvas.set_size_request(300, 300)
-    hbox.pack_start(canvas, False, False, 0)
-    vbox = Gtk.VBox(spacing = 8)
-    hbox.pack_start(vbox, True, True, 0)
-    grid = Gtk.Grid(column_spacing = 8)
-    vbox.pack_start(grid, False, False, 0)
-    hbox = Gtk.HBox(spacing = 8)
-    grid.add(hbox)
-    self.widgets.deltasatbutton = RadioButton.new_with_label_from_widget(None, "\u0394Sat")
-    hbox.pack_start(self.widgets.deltasatbutton, False, False, 0)
-    self.widgets.msstretchbutton = RadioButton.new_with_label_from_widget(self.widgets.deltasatbutton, "MidSat stretch")
-    hbox.pack_start(self.widgets.msstretchbutton, False, False, 0)
-    self.widgets.deltasatbutton.connect("toggled", lambda button: self.update(-2))
-    self.widgets.msstretchbutton.connect("toggled", lambda button: self.update(-2))
-    self.widgets.bindbutton = CheckButton(label = "Bind hues", halign = Gtk.Align.END)
-    self.widgets.bindbutton.set_active(True)
-    self.widgets.bindbutton.connect("toggled", lambda button: self.update(0))
-    hbox.pack_start(self.widgets.bindbutton, True, True, 0)
-    grid.attach_next_to(Gtk.Label(label = "Model:", halign = Gtk.Align.END), hbox, Gtk.PositionType.LEFT, 1, 1)
-    anchor = hbox
-    self.widgets.satscales = []
-    for hid, label in ((0, "Red:"), (1, "Yellow:"), (2, "Green:"), (3, "Cyan:"), (4, "Blue:"), (5, "Magenta:")):
-      satscale = HScaleSpinButton(0., -1., 1., .001, digits = 3, length = 320)
-      satscale.hid = hid
-      satscale.connect("value-changed", lambda scale: self.update(scale.hid))
-      self.widgets.satscales.append(satscale)
-      satscalebox = satscale.layout1()
-      grid.attach_next_to(satscalebox, anchor, Gtk.PositionType.BOTTOM, 1, 1)
-      grid.attach_next_to(Gtk.Label(label = label, halign = Gtk.Align.END), satscalebox, Gtk.PositionType.LEFT, 1, 1)
-      anchor = satscalebox
-    hbox = Gtk.HBox(spacing = 8)
-    grid.attach_next_to(hbox, anchor, Gtk.PositionType.BOTTOM, 1, 1)
-    self.widgets.nearestbutton = RadioButton.new_with_label_from_widget(None, "Nearest")
-    hbox.pack_start(self.widgets.nearestbutton, False, False, 0)
-    self.widgets.linearbutton = RadioButton.new_with_label_from_widget(self.widgets.nearestbutton, "Linear")
-    hbox.pack_start(self.widgets.linearbutton, False, False, 0)
-    self.widgets.cubicbutton = RadioButton.new_with_label_from_widget(self.widgets.nearestbutton, "Cubic")
-    hbox.pack_start(self.widgets.cubicbutton, False, False, 0)
-    self.widgets.cubicbutton.set_active(True)
-    self.widgets.nearestbutton.connect("toggled", lambda button: self.update(-1))
-    self.widgets.linearbutton.connect("toggled", lambda button: self.update(-1))
-    self.widgets.cubicbutton.connect("toggled", lambda button: self.update(-1))
-    grid.attach_next_to(Gtk.Label(label = "Interpolation:", halign = Gtk.Align.END), hbox, Gtk.PositionType.LEFT, 1, 1)
-    vbox.pack_start(self.tool_control_buttons(), False, False, 8)
-    self.plot_hsv_wheel()
-    self.outofrange = self.reference.is_out_of_range() # Is the reference image out-of-range ?
-    if self.outofrange: print("Reference image is out-of-range...")
-    self.start(identity = not self.outofrange) # If so, the color saturation tool will clip the image whatever the parameters
-    return True
+    super().start(*args, **kwargs)
+
+  # Tool methods.
 
   def get_params(self):
     """Return tool parameters."""
-    model = "DeltaSat" if self.widgets.deltasatbutton.get_active() else "MidSatStretch"
-    psat = tuple(self.widgets.satscales[hid].get_value() for hid in range(6))
-    if self.widgets.nearestbutton.get_active():
-      interpolation = "nearest"
-    elif self.widgets.linearbutton.get_active():
-      interpolation = "linear"
-    else:
-      interpolation = "cubic"
-    return model, psat, interpolation
+    params = {}
+    for key in self.channelkeys:
+      channel = self.widgets.channels[key]
+      logD1 = channel.logD1spin.get_value()
+      B = channel.Bspin.get_value()
+      SYP = channel.SYPspin.get_value()
+      SPP = channel.SPPspin.get_value()
+      HPP = channel.HPPspin.get_value()
+      params[key] = (logD1, B, SYP, SPP, HPP)
+    #params["highlights"] = self.widgets.channels["L"].highlightsbutton.get_active()
+    params["inverse"] = self.widgets.inversebutton.get_active()
+    #params["rgbluma"] = imageprocessing.get_rgb_luma()
+    return params
 
   def set_params(self, params):
     """Set tool parameters 'params'."""
-    model, psat, interpolation = params
-    psat = np.array(psat)
-    if model == "DeltaSat":
-      self.widgets.deltasatbutton.set_active_block(True)
-    else:
-      self.widgets.msstretchbutton.set_active_block(True)
-    for hid in range(6): self.widgets.satscales[hid].set_value_block(psat[hid])
-    if np.any(psat != psat[0]): self.widgets.bindbutton.set_active_block(False)
-    if interpolation == "nearest":
-      self.widgets.nearestbutton.set_active_block(True)
-    elif interpolation == "linear":
-      self.widgets.linearbutton.set_active_block(True)
-    else:
-      self.widgets.cubicbutton.set_active_block(True)
-    self.update(0)
+    #unbindrgb = False
+    #redparams = params["R"]
+    for key in self.channelkeys:
+      channel = self.widgets.channels[key]
+      #if key in ("R", "G", "B"):
+        #unbindrgb = unbindrgb or (params[key] != redparams)
+      logD1, B, SYP, SPP, HPP = params[key]
+      channel.logD1spin.set_value_block(logD1)
+      channel.Bspin.set_value_block(B)
+      channel.SYPspin.set_value_block(SYP)
+      channel.SPPspin.set_value_block(SPP)
+      channel.HPPspin.set_value_block(HPP)
+    #self.widgets.channels["L"].highlightsbutton.set_active_block(params["highlights"])
+    self.widgets.inversebutton.set_active(params["inverse"])
+    #if unbindrgb: self.widgets.bindbutton.set_active_block(False)
+    self.update("all")
 
   def run(self, params):
     """Run tool for parameters 'params'."""
-    model, psat, interpolation = params
-    psat = np.array(psat)
-    if not self.outofrange and np.all(psat == 0.): return params, False
-    hsv = self.reference.hsv.copy()
-    sat = hsv[:, :, 1]
-    if np.all(psat == psat[0]):
-      if model == "DeltaSat":
-        sat += psat[0]
-      else:
-        midsat = min(max(.5*(1.-psat[0]), .005), .995)
-        sat = (midsat-1.)*sat/((2.*midsat-1.)*sat-midsat)
-    else:
-      hsat = np.linspace(0., 6., 7)/6.
-      psat = np.append(psat, psat[0])
-      if interpolation == "nearest":
-        fsat = interp1d(hsat, psat, kind = "nearest")
+    #self.image.copy_image_from(self.reference)
+    transformed = False
+    inverse = params["inverse"]
+    for key in self.channelkeys:
+      logD1, B, SYP, SPP, HPP = params[key]
+      if key == "S": # NOTE: MUST start with the "S" key !!
+        if not self.outofrange and logD1 == 0.:
+          self.image.copy_image_from(self.reference)
+        else: # Special transformation in the HSV color space.
+          transformed = True
+          hsv = self.reference.hsv.copy()
+          hsv[:, :, 1] = ghyperbolic_stretch_function(self.reference.hsv[:, :, 1], (logD1, B, SYP, SPP, HPP, inverse))
+          self.image.set_hsv_image(hsv)
       else:
-        k = 3 if interpolation == "cubic" else 1
-        tck = splrep(hsat, psat, k = k, per = True)
-        def fsat(x): return splev(x, tck)
-      hue = hsv[:, :, 0]
-      if model == "DeltaSat":
-        sat += fsat(hue)
-      else:
-        midsat = np.clip(.5*(1.-fsat(hue)), .005, .995)
-        sat = (midsat-1.)*sat/((2.*midsat-1.)*sat-midsat)
-    hsv[:, :, 1] = np.clip(sat, 0., 1.)
-    self.image.set_hsv_image(hsv)
-    return params, True
+        if logD1 != 0.:
+          transformed = True
+          self.image.generalized_stretch(ghyperbolic_stretch_function, (logD1, B, SYP, SPP, HPP, inverse), channels = key)
+    #if transformed and params["highlights"]: self.image.protect_highlights()
+    return params, transformed
 
   def operation(self, params):
     """Return tool operation string for parameters 'params'."""
-    model, psat, interpolation = params
-    tags = ["R", "Y", "G", "C", "B", "M"]
-    operation = f"ColorSaturation(model = {model}, "
-    for hid in range(6):
-      operation += f"{tags[hid]} = {psat[hid]:.3f}, "
-    operation += f" interpolation = {interpolation})"
+    operation = "GHStretch("
+    if params["inverse"]: operation = "Inverse"+operation
+    separator = ""
+    for key in self.channelkeys:
+      logD1, B, SYP, SPP, HPP = params[key]
+      if key == "L":
+        red, green, blue = params["rgbluma"]
+        operation += f"{separator}L({red:.2f}, {green:.2f}, {blue:.2f}) : (log(D+1) = {logD1:.3f}, B = {B:.3f}, SYP = {SYP:.5f}, SPP = {SPP:.5f}, HPP = {HPP:.5f})"
+      else:
+        operation += f"{separator}{key} : (log(D+1) = {logD1:.3f}, B = {B:.3f}, SYP = {SYP:.5f}, SPP = {SPP:.5f}, HPP = {HPP:.5f})"
+      separator = ", "
+    #if params["highlights"]: operation += ", protect highlights"
+    operation += ")"
     return operation
 
-  # Plot HSV wheel.
+  # Plot histograms, stretch function, display stats...
 
-  def plot_hsv_wheel(self):
-    """Plot HSV wheel."""
-    ax = self.widgets.fig.add_axes([.1, .1, .8, .8], projection = "polar")
-    self.widgets.fig.satax = ax
-    ax.patch.set_alpha(0.)
-    ax2 = ax.figure.add_axes(ax.get_position(), projection = "polar", zorder = -3)
-    ax2.axis("off")
-    ax2.set_ylim(0., 1.)
-    rho = np.linspace(1., 1.2, 32)
-    phi = np.linspace(0., 2.*np.pi, 256)
-    RHO, PHI = np.meshgrid(rho, phi)
-    h = np.ravel(PHI/(2.*np.pi))
-    s = np.ones_like(h)
-    v = s
-    hsv = np.column_stack((h, s, v))
-    rgb = colors.hsv_to_rgb(hsv)
-    ax2.scatter(PHI, RHO, c = rgb, clip_on = False)
-    hue = 2.*np.pi*np.linspace(0., 5., 6)/6.
-    ax.set_xticks(hue, labels = ["R", "Y", "G", "C", "B", "M"])
-    ax.set_ylim([-1., 1.])
-    ax.yaxis.set_major_locator(ticker.LinearLocator(5))
-    ax.yaxis.set_major_formatter(ticker.FormatStrFormatter("%.2f"))
-    ax.satpoints, = ax.plot(hue, np.zeros_like(hue), "ko", ms = 8)
-    hue = np.linspace(0., 2.*np.pi, 128)
-    ax.satcurve, = ax.plot(hue, np.zeros_like(hue), "k--")
-
-  # Update widgets.
-
-  def update(self, changed):
-    """Update widgets on change of 'changed'."""
-    if changed >= 0:
-      if self.widgets.bindbutton.get_active():
-        psat = self.widgets.satscales[changed].get_value()
-        for hid in range(6):
-          self.widgets.satscales[hid].set_value_block(psat)
-    if changed >= -1: self.update_hsv_wheel()
-    self.reset_polling(self.get_params()) # Expedite main window update.
-
-  def update_hsv_wheel(self):
-    """Update HSV wheel."""
-    model, psat, interpolation = self.get_params()
-    psat = np.array(psat)
-    pmin = psat.min()
-    pmax = psat.max()
-    ax = self.widgets.fig.satax
-    ax.satpoints.set_ydata(psat)
-    hsat = 2.*np.pi*np.linspace(0., 6., 7)/6.
-    psat = np.append(psat, psat[0])
-    if interpolation == "nearest":
-      fsat = interp1d(hsat, psat, kind = "nearest")
-    else:
-      k = 3 if interpolation == "cubic" else 1
-      tck = splrep(hsat, psat, k = k, per = True)
-      def fsat(x): return np.clip(splev(x, tck), -1., 1.)
-    ax.satcurve.set_ydata(fsat(ax.satcurve.get_xdata()))
-    if np.all(psat == psat[0]) or pmax-pmin > .25:
-      ymin = -1.
-      ymax =  1.
-    else:
-      ymin = max(pmin-.125, -1.)
-      ymax = min(pmax+.125,  1.)
-      if ymax-ymin < .2:
-        if ymax ==  1.:
-          ymin =  .8
-        elif ymin == -1.:
-          ymax = -.8
-    ax.set_ylim(ymin, ymax)
-    self.widgets.fig.canvas.draw_idle()
+  def stretch_function(self, t, params):
+    """Return the stretch function f(t) for parameters 'params'."""
+    return ghyperbolic_stretch_function(t, params)
+
+  def add_histogram_widgets(self, ax):
+    """Add histogram widgets (other than stretch function) in axes 'ax'."""
+    self.widgets.SPPline = ax.axvline(0., linestyle = "-.", zorder = -2)
+    self.widgets.SYPline = ax.axvline(.5, linestyle = "-.", zorder = -2)
+    self.widgets.HPPline = ax.axvline(1., linestyle = "-.", zorder = -2)
+
+  # Update histograms, stats... on widget or key_press events.
+
+  def update_widgets(self, key, changed):
+    """Update widgets (other than histograms and stats) on change of 'changed' in channel 'key'."""
+    channel = self.widgets.channels[key]
+    logD1 = channel.logD1spin.get_value()
+    B = channel.Bspin.get_value()
+    SYP = channel.SYPspin.get_value()
+    SPP = channel.SPPspin.get_value()
+    HPP = channel.HPPspin.get_value()
+    if changed == "SPP":
+      if SPP > HPP-0.005:
+        SPP = HPP-0.005
+        channel.SPPspin.set_value_block(SPP)
+      if SPP > SYP:
+        SYP = SPP
+        channel.SYPspin.set_value_block(SYP)
+    elif changed == "HPP":
+      if HPP < SPP+0.005:
+        HPP = SPP+0.005
+        channel.HPPspin.set_value_block(HPP)
+      if HPP < SYP:
+        SYP = HPP
+        channel.SYPspin.set_value_block(SYP)
+    elif changed == "SYP":
+      if SYP < SPP:
+        SPP = SYP
+        channel.SPPspin.set_value_block(SPP)
+      elif SYP > HPP:
+        HPP = SYP
+        channel.HPPspin.set_value_block(HPP)
+    color = channel.color
+    lcolor = channel.lcolor
+    self.widgets.SPPline.set_xdata([SPP, SPP])
+    self.widgets.SPPline.set_color(0.1*lcolor)
+    self.widgets.SYPline.set_xdata([SYP, SYP])
+    self.widgets.SYPline.set_color(0.5*lcolor)
+    self.widgets.HPPline.set_xdata([HPP, HPP])
+    self.widgets.HPPline.set_color(0.9*lcolor)
+    inverse = self.widgets.inversebutton.get_active()
+    self.plot_stretch_function(lambda t: self.stretch_function(t, (logD1, B, SYP, SPP, HPP, inverse)), color)
+    #if self.widgets.bindbutton.get_active() and key in ("R", "G", "B"):
+      #for rgbkey in ("R", "G", "B"):
+        #rgbchannel = self.widgets.channels[rgbkey]
+        #rgbchannel.logD1spin.set_value_block(logD1)
+        #rgbchannel.Bspin.set_value_block(B)
+        #rgbchannel.SYPspin.set_value_block(SYP)
+        #rgbchannel.SPPspin.set_value_block(SPP)
+        #rgbchannel.HPPspin.set_value_block(HPP)
```

### Comparing `eQuimage-1.3.0/src/eQuimage/windows/ghscolorsat.py` & `eQuimage-1.4.0/src/eQuimage/gui/tools/hyperbolic.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,154 +1,150 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
+# GUI updated.
 
-"""Hyperbolic color saturation stretch tool."""
+"""Hyperbolic stretch tool."""
 
-import gi
-gi.require_version("Gtk", "3.0")
-from gi.repository import Gtk
-from .gtk.customwidgets import CheckButton, SpinButton
 from .stretch import StretchTool
-from ..imageprocessing import imageprocessing
-from ..imageprocessing.stretchfunctions import ghyperbolic_stretch_function
-import numpy as np
-
-class GHSColorSaturationTool(StretchTool):
-  """Color saturation generalized hyperbolic stretch tool class, derived from the StretchTool class.
-     Adapted from hyperbolic.py/GeneralizedHyperbolicStretchTool."""
+from ..gtk.customwidgets import HBox, VBox, CheckButton, SpinButton
+from ...imageprocessing import imageprocessing
+from ...imageprocessing.stretchfunctions import ghyperbolic_stretch_function
 
-  __action__ = "Stretching color saturation (generalized hyperbolic stretch function)..."
+class GeneralizedHyperbolicStretchTool(StretchTool):
+  """Generalized hyperbolic stretch tool class, derived from the StretchTool class."""
+
+  _action_ = "Stretching histograms (generalized hyperbolic stretch function)..."
 
   # Build window.
 
-  __window_name__ = "Color saturation generalized hyperbolic stretch"
+  _window_name_ = "Generalized hyperbolic stretch"
 
   def options_widgets(self, widgets):
-    """Return a Gtk box with tool options widgets and store the reference to these widgets in container 'widgets'.
+    """Return a box with tool options widgets and store the reference to these widgets in container 'widgets'.
        Return None if there are no tool options widgets."""
-    hbox = Gtk.HBox(spacing = 8)
+    hbox = HBox()
+    widgets.bindbutton = CheckButton(label = "Bind RGB channels")
+    widgets.bindbutton.set_active(True)
+    widgets.bindbutton.connect("toggled", lambda button: self.update("bindrgb"))
+    hbox.pack(widgets.bindbutton, expand = True, fill = True)
     widgets.inversebutton = CheckButton(label = "Inverse transformation")
     widgets.inversebutton.set_active(False)
     widgets.inversebutton.connect("toggled", lambda button: self.update("inverse"))
-    hbox.pack_start(widgets.inversebutton, False, False, 0)
+    hbox.pack(widgets.inversebutton)
     return hbox
 
   def tab_widgets(self, key, widgets):
-    """Return a Gtk box with tab widgets for channel 'key' in "R" (red), "G" (green), "B" (blue), "S" (saturation), "V" (value) or "L" (luma),
+    """Return a box with tab widgets for channel 'key' in "R" (red), "G" (green), "B" (blue), "S" (saturation), "V" (value) or "L" (luma),
        and store the reference to these widgets in container 'widgets'.
        Return None if there is no tab for this channel."""
-    if key != "S": return None
-    cbox = Gtk.VBox(margin = 16, spacing = 16)
-    hbox = Gtk.HBox(spacing = 8)
-    cbox.pack_start(hbox, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = "Global log(D+1):"), False, False, 0)
+    if not key in ["R", "G", "B", "V", "L"]: return None
+    percentiles = self.reference.stats["L"].percentiles
+    step = (percentiles[2]-percentiles[0])/10. if percentiles is not None else .01
+    step = min(max(step, .0001), .01)
+    cbox = VBox(margin = 16)
+    hbox = HBox()
+    cbox.pack(hbox)
     widgets.logD1spin = SpinButton(0., 0., 10., .1, digits = 3)
     widgets.logD1spin.connect("value-changed", lambda button: self.update("D"))
-    hbox.pack_start(widgets.logD1spin, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = 5*" "+"Local B:"), False, False, 0)
+    hbox.pack("Global log(D+1):")
+    hbox.pack(widgets.logD1spin)
     widgets.Bspin = SpinButton(0, -5., 15., .1, digits = 3)
     widgets.Bspin.connect("value-changed", lambda button: self.update("B"))
-    hbox.pack_start(widgets.Bspin, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = 5*" "+"Symmetry point:"), False, False, 0)
-    widgets.SYPspin = SpinButton(.5, 0., 1., .01, digits = 5)
+    hbox.pack(5*" "+"Local B:")
+    hbox.pack(widgets.Bspin)
+    widgets.SYPspin = SpinButton(.5, 0., 1., step/2., digits = 5)
     widgets.SYPspin.connect("value-changed", lambda button: self.update("SYP"))
-    hbox.pack_start(widgets.SYPspin, False, False, 0)
-    hbox = Gtk.HBox(spacing = 8)
-    cbox.pack_start(hbox, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = "Shadow protection point:"), False, False, 0)
-    widgets.SPPspin = SpinButton(0., 0., .99, .01, digits = 5)
+    hbox.pack(5*" "+"Symmetry point:")
+    hbox.pack(widgets.SYPspin)
+    hbox = HBox()
+    cbox.pack(hbox)
+    widgets.SPPspin = SpinButton(0., 0., .99, step/2., digits = 5)
     widgets.SPPspin.connect("value-changed", lambda button: self.update("SPP"))
-    hbox.pack_start(widgets.SPPspin, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = 5*" "+"Highlight protection point:"), False, False, 0)
-    widgets.HPPspin = SpinButton(1., .01, 1., .01, digits = 5)
+    hbox.pack("Shadow protection point:")
+    hbox.pack(widgets.SPPspin)
+    widgets.HPPspin = SpinButton(1., .01, 1., step, digits = 5)
     widgets.HPPspin.connect("value-changed", lambda button: self.update("HPP"))
-    hbox.pack_start(widgets.HPPspin, False, False, 0)
+    hbox.pack(5*" "+"Highlight protection point:")
+    hbox.pack(widgets.HPPspin)
+    if key == "L":
+      widgets.highlightsbutton = CheckButton(label = "Protect highlights")
+      widgets.highlightsbutton.set_active(False)
+      widgets.highlightsbutton.connect("toggled", lambda button: self.update(None))
+      hbox.pack(5*" ")
+      hbox.pack(widgets.highlightsbutton)
     return cbox
 
-  def start(self, *args, **kwargs):
-    """Compute the HSV components of the reference image before starting the tool."""
-    self.reference.hsv = self.reference.rgb_to_hsv()
-    super().start(*args, **kwargs)
-
   # Tool methods.
 
   def get_params(self):
     """Return tool parameters."""
     params = {}
     for key in self.channelkeys:
       channel = self.widgets.channels[key]
       logD1 = channel.logD1spin.get_value()
       B = channel.Bspin.get_value()
       SYP = channel.SYPspin.get_value()
       SPP = channel.SPPspin.get_value()
       HPP = channel.HPPspin.get_value()
       params[key] = (logD1, B, SYP, SPP, HPP)
-    #params["highlights"] = self.widgets.channels["L"].highlightsbutton.get_active()
+    params["highlights"] = self.widgets.channels["L"].highlightsbutton.get_active()
     params["inverse"] = self.widgets.inversebutton.get_active()
-    #params["rgbluma"] = imageprocessing.get_rgb_luma()
+    params["rgbluma"] = imageprocessing.get_rgb_luma()
     return params
 
   def set_params(self, params):
     """Set tool parameters 'params'."""
-    #unbindrgb = False
-    #redparams = params["R"]
+    unbindrgb = False
+    redparams = params["R"]
     for key in self.channelkeys:
       channel = self.widgets.channels[key]
-      #if key in ("R", "G", "B"):
-        #unbindrgb = unbindrgb or (params[key] != redparams)
+      if key in ("R", "G", "B"):
+        unbindrgb = unbindrgb or (params[key] != redparams)
       logD1, B, SYP, SPP, HPP = params[key]
       channel.logD1spin.set_value_block(logD1)
       channel.Bspin.set_value_block(B)
       channel.SYPspin.set_value_block(SYP)
       channel.SPPspin.set_value_block(SPP)
       channel.HPPspin.set_value_block(HPP)
-    #self.widgets.channels["L"].highlightsbutton.set_active_block(params["highlights"])
+    self.widgets.channels["L"].highlightsbutton.set_active_block(params["highlights"])
     self.widgets.inversebutton.set_active(params["inverse"])
-    #if unbindrgb: self.widgets.bindbutton.set_active_block(False)
+    if unbindrgb: self.widgets.bindbutton.set_active_block(False)
     self.update("all")
 
   def run(self, params):
     """Run tool for parameters 'params'."""
-    #self.image.copy_image_from(self.reference)
+    self.image.copy_image_from(self.reference)
     transformed = False
     inverse = params["inverse"]
     for key in self.channelkeys:
       logD1, B, SYP, SPP, HPP = params[key]
-      if key == "S": # NOTE: MUST start with the "S" key !!
-        if not self.outofrange and logD1 == 0.:
-          self.image.copy_image_from(self.reference)
-        else: # Special transformation in the HSV color space.
-          transformed = True
-          hsv = self.reference.hsv.copy()
-          hsv[:, :, 1] = ghyperbolic_stretch_function(self.reference.hsv[:, :, 1], (logD1, B, SYP, SPP, HPP, inverse))
-          self.image.set_hsv_image(hsv)
-      else:
-        if logD1 != 0.:
-          transformed = True
-          self.image.generalized_stretch(ghyperbolic_stretch_function, (logD1, B, SYP, SPP, HPP, inverse), channels = key)
-    #if transformed and params["highlights"]: self.image.protect_highlights()
+      outofrange = self.outofrange and key in ["R", "G", "B"]
+      if not outofrange and logD1 == 0.: continue
+      transformed = True
+      self.image.generalized_stretch(ghyperbolic_stretch_function, (logD1, B, SYP, SPP, HPP, inverse), channels = key)
+    if transformed and params["highlights"]: self.image.protect_highlights()
     return params, transformed
 
   def operation(self, params):
     """Return tool operation string for parameters 'params'."""
     operation = "GHStretch("
     if params["inverse"]: operation = "Inverse"+operation
     separator = ""
     for key in self.channelkeys:
       logD1, B, SYP, SPP, HPP = params[key]
-      if key != "L":
-        operation += f"{separator}{key} : (log(D+1) = {logD1:.3f}, B = {B:.3f}, SYP = {SYP:.5f}, SPP = {SPP:.5f}, HPP = {HPP:.5f})"
-      else:
+      if key == "L":
         red, green, blue = params["rgbluma"]
         operation += f"{separator}L({red:.2f}, {green:.2f}, {blue:.2f}) : (log(D+1) = {logD1:.3f}, B = {B:.3f}, SYP = {SYP:.5f}, SPP = {SPP:.5f}, HPP = {HPP:.5f})"
+      else:
+        operation += f"{separator}{key} : (log(D+1) = {logD1:.3f}, B = {B:.3f}, SYP = {SYP:.5f}, SPP = {SPP:.5f}, HPP = {HPP:.5f})"
       separator = ", "
-    #if params["highlights"]: operation += ", protect highlights"
+    if params["highlights"]: operation += ", protect highlights"
     operation += ")"
     return operation
 
   # Plot histograms, stretch function, display stats...
 
   def stretch_function(self, t, params):
     """Return the stretch function f(t) for parameters 'params'."""
@@ -197,15 +193,15 @@
     self.widgets.SPPline.set_color(0.1*lcolor)
     self.widgets.SYPline.set_xdata([SYP, SYP])
     self.widgets.SYPline.set_color(0.5*lcolor)
     self.widgets.HPPline.set_xdata([HPP, HPP])
     self.widgets.HPPline.set_color(0.9*lcolor)
     inverse = self.widgets.inversebutton.get_active()
     self.plot_stretch_function(lambda t: self.stretch_function(t, (logD1, B, SYP, SPP, HPP, inverse)), color)
-    #if self.widgets.bindbutton.get_active() and key in ("R", "G", "B"):
-      #for rgbkey in ("R", "G", "B"):
-        #rgbchannel = self.widgets.channels[rgbkey]
-        #rgbchannel.logD1spin.set_value_block(logD1)
-        #rgbchannel.Bspin.set_value_block(B)
-        #rgbchannel.SYPspin.set_value_block(SYP)
-        #rgbchannel.SPPspin.set_value_block(SPP)
-        #rgbchannel.HPPspin.set_value_block(HPP)
+    if self.widgets.bindbutton.get_active() and key in ("R", "G", "B"):
+      for rgbkey in ("R", "G", "B"):
+        rgbchannel = self.widgets.channels[rgbkey]
+        rgbchannel.logD1spin.set_value_block(logD1)
+        rgbchannel.Bspin.set_value_block(B)
+        rgbchannel.SYPspin.set_value_block(SYP)
+        rgbchannel.SPPspin.set_value_block(SPP)
+        rgbchannel.HPPspin.set_value_block(HPP)
```

### Comparing `eQuimage-1.3.0/src/eQuimage/windows/gtk/filechoosers.py` & `eQuimage-1.4.0/src/eQuimage/gui/gtk/filechoosers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
 
 """Custom Gtk file choosers."""
 
 import os
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk, GdkPixbuf
 
-def ImageChooserDialog(window, action, path = None, preview = False, title = None, extra_widget = None):
+def ImageFileChooserDialog(window, action, path = None, preview = False, title = None, extra_widget = None):
   """Open file chooser dialog for an image, from window 'window' and for
      action 'action' (either Gtk.FileChooserAction.OPEN to open an image
      or Gtk.FileChooserAction.SAVE to save an image). Start with directory
      and file name 'path' (default if None), and preview selected image
      if 'preview' is True. If not None, 'title' overrides the default title
      of the dialog, and 'extra_widget' is a widget to provide, for example,
      additional options.
```

### Comparing `eQuimage-1.3.0/src/eQuimage/windows/gtk/signals.py` & `eQuimage-1.4.0/src/eQuimage/gui/gtk/signals.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
 
 """Signals management."""
 
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk
```

### Comparing `eQuimage-1.3.0/src/eQuimage/windows/gtk/utils.py` & `eQuimage-1.4.0/src/eQuimage/gui/gtk/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
 
 """Misc Gtk utilities."""
 
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk
 
+class Container:
+  """Empty class as a container."""
+  pass
+
 def get_work_area(window):
   """Return the width and height of the monitor displaying 'window'."""
   screen = window.get_screen()
   display = screen.get_display()
   monitor = display.get_monitor_at_window(screen.get_root_window())
   workarea = monitor.get_workarea()
   return workarea.width, workarea.height
```

### Comparing `eQuimage-1.3.0/src/eQuimage/windows/hyperbolic.py` & `eQuimage-1.4.0/src/eQuimage/gui/tools/midtone.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,210 +1,198 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
+# GUI updated.
 
-"""Hyperbolic stretch tool."""
+"""Midtone stretch tool."""
 
-import gi
-gi.require_version("Gtk", "3.0")
-from gi.repository import Gtk
-from .gtk.customwidgets import CheckButton, SpinButton
 from .stretch import StretchTool
-from ..imageprocessing import imageprocessing
-from ..imageprocessing.stretchfunctions import ghyperbolic_stretch_function
-import numpy as np
+from ..gtk.customwidgets import HBox, VBox, CheckButton, SpinButton
+from ...imageprocessing import imageprocessing
+from ...imageprocessing.stretchfunctions import midtone_stretch_function
 
-class GeneralizedHyperbolicStretchTool(StretchTool):
-  """Generalized hyperbolic stretch tool class, derived from the StretchTool class."""
+class MidtoneStretchTool(StretchTool):
+  """Midtone stretch tool class."""
 
-  __action__ = "Stretching histograms (generalized hyperbolic stretch function)..."
+  _action_ = "Stretching histograms (midtone stretch function)..."
 
   # Build window.
 
-  __window_name__ = "Generalized hyperbolic stretch"
+  _window_name_ = "Midtone stretch"
 
   def options_widgets(self, widgets):
-    """Return a Gtk box with tool options widgets and store the reference to these widgets in container 'widgets'.
+    """Return a box with tool options widgets and store the reference to these widgets in container 'widgets'.
        Return None if there are no tool options widgets."""
-    hbox = Gtk.HBox(spacing = 8)
+    hbox = HBox()
     widgets.bindbutton = CheckButton(label = "Bind RGB channels")
     widgets.bindbutton.set_active(True)
     widgets.bindbutton.connect("toggled", lambda button: self.update("bindrgb"))
-    hbox.pack_start(widgets.bindbutton, True, True, 0)
-    widgets.inversebutton = CheckButton(label = "Inverse transformation")
-    widgets.inversebutton.set_active(False)
-    widgets.inversebutton.connect("toggled", lambda button: self.update("inverse"))
-    hbox.pack_start(widgets.inversebutton, False, False, 0)
+    hbox.pack(widgets.bindbutton, expand = True, fill = True)
     return hbox
 
   def tab_widgets(self, key, widgets):
-    """Return a Gtk box with tab widgets for channel 'key' in "R" (red), "G" (green), "B" (blue), "S" (saturation), "V" (value) or "L" (luma),
+    """Return a box with tab widgets for channel 'key' in "R" (red), "G" (green), "B" (blue), "S" (saturation), "V" (value) or "L" (luma),
        and store the reference to these widgets in container 'widgets'.
        Return None if there is no tab for this channel."""
     if not key in ["R", "G", "B", "V", "L"]: return None
     percentiles = self.reference.stats["L"].percentiles
     step = (percentiles[2]-percentiles[0])/10. if percentiles is not None else .01
     step = min(max(step, .0001), .01)
-    cbox = Gtk.VBox(margin = 16, spacing = 16)
-    hbox = Gtk.HBox(spacing = 8)
-    cbox.pack_start(hbox, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = "Global log(D+1):"), False, False, 0)
-    widgets.logD1spin = SpinButton(0., 0., 10., .1, digits = 3)
-    widgets.logD1spin.connect("value-changed", lambda button: self.update("D"))
-    hbox.pack_start(widgets.logD1spin, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = 5*" "+"Local B:"), False, False, 0)
-    widgets.Bspin = SpinButton(0, -5., 15., .1, digits = 3)
-    widgets.Bspin.connect("value-changed", lambda button: self.update("B"))
-    hbox.pack_start(widgets.Bspin, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = 5*" "+"Symmetry point:"), False, False, 0)
-    widgets.SYPspin = SpinButton(.5, 0., 1., step/2., digits = 5)
-    widgets.SYPspin.connect("value-changed", lambda button: self.update("SYP"))
-    hbox.pack_start(widgets.SYPspin, False, False, 0)
-    hbox = Gtk.HBox(spacing = 8)
-    cbox.pack_start(hbox, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = "Shadow protection point:"), False, False, 0)
-    widgets.SPPspin = SpinButton(0., 0., .99, step/2., digits = 5)
-    widgets.SPPspin.connect("value-changed", lambda button: self.update("SPP"))
-    hbox.pack_start(widgets.SPPspin, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = 5*" "+"Highlight protection point:"), False, False, 0)
-    widgets.HPPspin = SpinButton(1., .01, 1., step, digits = 5)
-    widgets.HPPspin.connect("value-changed", lambda button: self.update("HPP"))
-    hbox.pack_start(widgets.HPPspin, False, False, 0)
+    cbox = VBox(margin = 16)
+    hbox = HBox()
+    cbox.pack(hbox)
+    widgets.shadowspin = SpinButton(0., 0., .99, step/2., digits = 5)
+    widgets.shadowspin.connect("value-changed", lambda button: self.update("shadow"))
+    hbox.pack("Shadow:")
+    hbox.pack(widgets.shadowspin)
+    widgets.midtonespin = SpinButton(.5, 0., 1., step, digits = 5)
+    widgets.midtonespin.connect("value-changed", lambda button: self.update("midtone"))
+    hbox.pack(8*" "+"Midtone:")
+    hbox.pack(widgets.midtonespin)
+    widgets.highlightspin = SpinButton(1., .01, 1., step, digits = 5)
+    widgets.highlightspin.connect("value-changed", lambda button: self.update("highlight"))
+    hbox.pack(8*" "+"Highlight:")
+    hbox.pack(widgets.highlightspin)
+    hbox = HBox()
+    cbox.pack(hbox)
+    widgets.lowspin = SpinButton(0., -10., 0., .01, digits = 3)
+    widgets.lowspin.connect("value-changed", lambda button: self.update("low"))
+    hbox.pack("Low range:")
+    hbox.pack(widgets.lowspin)
+    widgets.highspin = SpinButton(1., 1., 10., .01, digits = 3)
+    widgets.highspin.connect("value-changed", lambda button: self.update("high"))
+    hbox.pack(8*" "+"High range:")
+    hbox.pack(widgets.highspin)
     if key == "L":
-      hbox.pack_start(Gtk.Label(label = 5*" "), False, False, 0)
       widgets.highlightsbutton = CheckButton(label = "Protect highlights")
       widgets.highlightsbutton.set_active(False)
       widgets.highlightsbutton.connect("toggled", lambda button: self.update(None))
-      hbox.pack_start(widgets.highlightsbutton, False, False, 0)
+      hbox.pack(8*" ")
+      hbox.pack(widgets.highlightsbutton)
     return cbox
 
   # Tool methods.
 
   def get_params(self):
     """Return tool parameters."""
     params = {}
     for key in self.channelkeys:
       channel = self.widgets.channels[key]
-      logD1 = channel.logD1spin.get_value()
-      B = channel.Bspin.get_value()
-      SYP = channel.SYPspin.get_value()
-      SPP = channel.SPPspin.get_value()
-      HPP = channel.HPPspin.get_value()
-      params[key] = (logD1, B, SYP, SPP, HPP)
+      shadow = channel.shadowspin.get_value()
+      midtone = channel.midtonespin.get_value()
+      highlight = channel.highlightspin.get_value()
+      low = channel.lowspin.get_value()
+      high = channel.highspin.get_value()
+      params[key] = (shadow, midtone, highlight, low, high)
     params["highlights"] = self.widgets.channels["L"].highlightsbutton.get_active()
-    params["inverse"] = self.widgets.inversebutton.get_active()
     params["rgbluma"] = imageprocessing.get_rgb_luma()
     return params
 
   def set_params(self, params):
     """Set tool parameters 'params'."""
     unbindrgb = False
     redparams = params["R"]
     for key in self.channelkeys:
       channel = self.widgets.channels[key]
       if key in ("R", "G", "B"):
         unbindrgb = unbindrgb or (params[key] != redparams)
-      logD1, B, SYP, SPP, HPP = params[key]
-      channel.logD1spin.set_value_block(logD1)
-      channel.Bspin.set_value_block(B)
-      channel.SYPspin.set_value_block(SYP)
-      channel.SPPspin.set_value_block(SPP)
-      channel.HPPspin.set_value_block(HPP)
+      shadow, midtone, highlight, low, high = params[key]
+      channel.shadowspin.set_value_block(shadow)
+      channel.midtonespin.set_value_block(midtone)
+      channel.highlightspin.set_value_block(highlight)
+      channel.lowspin.set_value_block(low)
+      channel.highspin.set_value_block(high)
     self.widgets.channels["L"].highlightsbutton.set_active_block(params["highlights"])
-    self.widgets.inversebutton.set_active(params["inverse"])
     if unbindrgb: self.widgets.bindbutton.set_active_block(False)
     self.update("all")
 
   def run(self, params):
     """Run tool for parameters 'params'."""
     self.image.copy_image_from(self.reference)
     transformed = False
-    inverse = params["inverse"]
     for key in self.channelkeys:
-      logD1, B, SYP, SPP, HPP = params[key]
+      shadow, midtone, highlight, low, high = params[key]
       outofrange = self.outofrange and key in ["R", "G", "B"]
-      if not outofrange and logD1 == 0.: continue
+      if not outofrange and shadow == 0. and midtone == 0.5 and highlight == 1. and low == 0. and high == 1.: continue
       transformed = True
-      self.image.generalized_stretch(ghyperbolic_stretch_function, (logD1, B, SYP, SPP, HPP, inverse), channels = key)
+      self.image.generalized_stretch(midtone_stretch_function, (shadow, midtone, highlight, low, high), channels = key)
     if transformed and params["highlights"]: self.image.protect_highlights()
     return params, transformed
 
   def operation(self, params):
     """Return tool operation string for parameters 'params'."""
-    operation = "GHStretch("
-    if params["inverse"]: operation = "Inverse"+operation
+    operation = "MTStretch("
     separator = ""
     for key in self.channelkeys:
-      logD1, B, SYP, SPP, HPP = params[key]
-      if key != "L":
-        operation += f"{separator}{key} : (log(D+1) = {logD1:.3f}, B = {B:.3f}, SYP = {SYP:.5f}, SPP = {SPP:.5f}, HPP = {HPP:.5f})"
-      else:
+      shadow, midtone, highlight, low, high = params[key]
+      if key == "L":
         red, green, blue = params["rgbluma"]
-        operation += f"{separator}L({red:.2f}, {green:.2f}, {blue:.2f}) : (log(D+1) = {logD1:.3f}, B = {B:.3f}, SYP = {SYP:.5f}, SPP = {SPP:.5f}, HPP = {HPP:.5f})"
+        operation += f"{separator}L({red:.2f}, {green:.2f}, {blue:.2f}) : (shadow = {shadow:.5f}, midtone = {midtone:.5f}, highlight = {highlight:.5f}, low = {low:.3f}, high = {high:.3f})"
+      else:
+        operation += f"{separator}{key} : (shadow = {shadow:.5f}, midtone = {midtone:.5f}, highlight = {highlight:.5f}, low = {low:.3f}, high = {high:.3f})"
       separator = ", "
     if params["highlights"]: operation += ", protect highlights"
     operation += ")"
     return operation
 
   # Plot histograms, stretch function, display stats...
 
   def stretch_function(self, t, params):
     """Return the stretch function f(t) for parameters 'params'."""
-    return ghyperbolic_stretch_function(t, params)
+    return midtone_stretch_function(t, params)
 
   def add_histogram_widgets(self, ax):
     """Add histogram widgets (other than stretch function) in axes 'ax'."""
-    self.widgets.SPPline = ax.axvline(0., linestyle = "-.", zorder = -2)
-    self.widgets.SYPline = ax.axvline(.5, linestyle = "-.", zorder = -2)
-    self.widgets.HPPline = ax.axvline(1., linestyle = "-.", zorder = -2)
+    self.widgets.shadowline = ax.axvline(0., linestyle = "-.", zorder = -2)
+    self.widgets.midtoneline = ax.axvline(.5, linestyle = "-.", zorder = -2)
+    self.widgets.highlightline = ax.axvline(1., linestyle = "-.", zorder = -2)
 
   # Update histograms, stats... on widget or key_press events.
 
   def update_widgets(self, key, changed):
     """Update widgets (other than histograms and stats) on change of 'changed' in channel 'key'."""
     channel = self.widgets.channels[key]
-    logD1 = channel.logD1spin.get_value()
-    B = channel.Bspin.get_value()
-    SYP = channel.SYPspin.get_value()
-    SPP = channel.SPPspin.get_value()
-    HPP = channel.HPPspin.get_value()
-    if changed == "SPP":
-      if SPP > HPP-0.005:
-        SPP = HPP-0.005
-        channel.SPPspin.set_value_block(SPP)
-      if SPP > SYP:
-        SYP = SPP
-        channel.SYPspin.set_value_block(SYP)
-    elif changed == "HPP":
-      if HPP < SPP+0.005:
-        HPP = SPP+0.005
-        channel.HPPspin.set_value_block(HPP)
-      if HPP < SYP:
-        SYP = HPP
-        channel.SYPspin.set_value_block(SYP)
-    elif changed == "SYP":
-      if SYP < SPP:
-        SPP = SYP
-        channel.SPPspin.set_value_block(SPP)
-      elif SYP > HPP:
-        HPP = SYP
-        channel.HPPspin.set_value_block(HPP)
+    shadow = channel.shadowspin.get_value()
+    midtone = channel.midtonespin.get_value()
+    highlight = channel.highlightspin.get_value()
+    low = channel.lowspin.get_value()
+    high = channel.highspin.get_value()
+    if changed in ["shadow", "highlight"]:
+      if changed == "shadow":
+        if shadow > highlight-0.005:
+          shadow = highlight-0.005
+          channel.shadowspin.set_value_block(shadow)
+      else:
+        if highlight < shadow+0.005:
+          highlight = shadow+0.005
+          channel.highlightspin.set_value_block(highlight)
+      shadow_, midtone_, highlight_, low_, high_ = self.currentparams[key]
+      midtone_ = (midtone_-shadow_)/(highlight_-shadow_)
+      midtone = shadow+midtone_*(highlight-shadow)
+      channel.midtonespin.set_value_block(midtone)
+    if midtone <= shadow:
+      midtone = shadow+0.001
+      channel.midtonespin.set_value_block(midtone)
+    if midtone >= highlight:
+      midtone = highlight-0.001
+      channel.midtonespin.set_value_block(midtone)
+    self.currentparams[key] = (shadow, midtone, highlight, low, high)
     color = channel.color
     lcolor = channel.lcolor
-    self.widgets.SPPline.set_xdata([SPP, SPP])
-    self.widgets.SPPline.set_color(0.1*lcolor)
-    self.widgets.SYPline.set_xdata([SYP, SYP])
-    self.widgets.SYPline.set_color(0.5*lcolor)
-    self.widgets.HPPline.set_xdata([HPP, HPP])
-    self.widgets.HPPline.set_color(0.9*lcolor)
-    inverse = self.widgets.inversebutton.get_active()
-    self.plot_stretch_function(lambda t: self.stretch_function(t, (logD1, B, SYP, SPP, HPP, inverse)), color)
+    self.widgets.shadowline.set_xdata([shadow, shadow])
+    self.widgets.shadowline.set_color(0.1*lcolor)
+    self.widgets.midtoneline.set_xdata([midtone, midtone])
+    self.widgets.midtoneline.set_color(0.5*lcolor)
+    self.widgets.highlightline.set_xdata([highlight, highlight])
+    self.widgets.highlightline.set_color(0.9*lcolor)
+    self.plot_stretch_function(lambda t: self.stretch_function(t, (shadow, midtone, highlight, low, high)), color)
     if self.widgets.bindbutton.get_active() and key in ("R", "G", "B"):
       for rgbkey in ("R", "G", "B"):
         rgbchannel = self.widgets.channels[rgbkey]
-        rgbchannel.logD1spin.set_value_block(logD1)
-        rgbchannel.Bspin.set_value_block(B)
-        rgbchannel.SYPspin.set_value_block(SYP)
-        rgbchannel.SPPspin.set_value_block(SPP)
-        rgbchannel.HPPspin.set_value_block(HPP)
+        rgbchannel.shadowspin.set_value_block(shadow)
+        rgbchannel.midtonespin.set_value_block(midtone)
+        rgbchannel.highlightspin.set_value_block(highlight)
+        rgbchannel.lowspin.set_value_block(low)
+        rgbchannel.highspin.set_value_block(high)
+        self.currentparams[rgbkey] = (shadow, midtone, highlight, low, high)
```

### Comparing `eQuimage-1.3.0/src/eQuimage/windows/logs.py` & `eQuimage-1.4.0/src/eQuimage/gui/logs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,63 +1,53 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
+# GUI updated.
 
 """Log window."""
 
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk, Gdk
+from .gtk.customwidgets import HBox, VBox, HButtonBox, Button, TextView
 from .base import BaseWindow, Container
 
 class LogWindow(BaseWindow):
   """Log window class."""
 
   def open(self):
     """Open log window."""
     if self.opened: return
     if self.app.get_basename() is None: return
     self.opened = True
     self.window = Gtk.Window(title = f"Logs for {self.app.get_basename()}", border_width = 16)
     self.window.connect("delete-event", self.close)
     self.window.set_size_request(480, 360)
     self.widgets = Container()
-    wbox = Gtk.VBox(spacing = 16)
+    wbox = VBox()
     self.window.add(wbox)
-    self.widgets.textview = Gtk.TextView()
-    self.widgets.textview.set_editable(False)
-    self.widgets.textview.set_cursor_visible(False)
-    self.widgets.textview.set_wrap_mode(True)
-    self.widgets.textview.set_justification(Gtk.Justification.LEFT)
-    wbox.pack_start(self.widgets.textview, True, True, 0)
-    self.textbuffer = self.widgets.textview.get_buffer()
-    hbox = Gtk.HButtonBox(homogeneous = True, spacing = 16, halign = Gtk.Align.START)
-    wbox.pack_start(hbox, False, False, 0)
-    self.widgets.copybutton = Gtk.Button(label = "Copy")
-    self.widgets.copybutton.connect("clicked", self.copy_to_clipboard)
-    hbox.pack_start(self.widgets.copybutton, False, False, 0)
-    self.widgets.closebutton = Gtk.Button(label = "Close")
+    self.widgets.textview = TextView()
+    wbox.pack(self.widgets.textview, expand = True, fill = True)
+    hbox = HButtonBox()
+    wbox.pack(hbox)
+    self.widgets.copybutton = Button(label = "Copy")
+    self.widgets.copybutton.connect("clicked", self.widgets.textview.copy_to_clipboard)
+    hbox.pack(self.widgets.copybutton)
+    self.widgets.closebutton = Button(label = "Close")
     self.widgets.closebutton.connect("clicked", self.close)
-    hbox.pack_start(self.widgets.closebutton, False, False, 0)
+    hbox.pack(self.widgets.closebutton)
     self.update()
     self.window.show_all()
 
   def close(self, *args, **kwargs):
     """Close log window."""
     if not self.opened: return
     self.window.destroy()
     self.opened = False
-    del self.textbuffer
     del self.widgets
 
   def update(self):
     """Update log window."""
     if not self.opened: return
-    self.textbuffer.set_text(self.app.logs())
-
-  def copy_to_clipboard(self, *args, **kwargs):
-    """Copy the content of the log window to the clipboard."""
-    if not self.opened: return
-    clipboard = Gtk.Clipboard.get(Gdk.SELECTION_CLIPBOARD)
-    clipboard.set_text(self.textbuffer.get_text(self.textbuffer.get_start_iter(), self.textbuffer.get_end_iter(), False), -1)
+    self.widgets.textview.set_text(self.app.logs())
```

### Comparing `eQuimage-1.3.0/src/eQuimage/windows/luma.py` & `eQuimage-1.4.0/src/eQuimage/gui/luma.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
+# GUI updated.
 
 """Luma RGB dialog."""
 
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk
-from .gtk.customwidgets import Button, SpinButton
+from .gtk.customwidgets import HBox, VBox, HButtonBox, Button, SpinButton
 
 class LumaRGBDialog(Gtk.Window):
   """Luma RGB dialog class."""
 
   # Here we store the data, widgets & methods of this simple dialog directly in the window object.
 
   def __init__(self, parent, callback, rgbluma):
@@ -21,41 +22,41 @@
        RGB components 'rgbluma'. When the apply button is pressed, close the
        dialog and call 'callback(rgbluma)', where rgbluma are the updated RGB
        components of the luma."""
     super().__init__(title = "Luma RGB",
                      transient_for = parent,
                      modal = True,
                      border_width = 16)
-    wbox = Gtk.VBox(spacing = 16)
+    wbox = VBox()
     self.add(wbox)
-    hbox = Gtk.HBox(spacing = 8)
-    wbox.pack_start(hbox, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = "Red:"), False, False, 0)
+    hbox = HBox()
+    wbox.pack(hbox)
     self.redspin = SpinButton(rgbluma[0], 0., 1., 0.01)
-    hbox.pack_start(self.redspin, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = 8*" "+"Green:"), False, False, 0)
+    hbox.pack("Red:")
+    hbox.pack(self.redspin)
     self.greenspin = SpinButton(rgbluma[1], 0., 1., 0.01)
-    hbox.pack_start(self.greenspin, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = 8*" "+"Blue:"), False, False, 0)
+    hbox.pack(8*" "+"Green:")
+    hbox.pack(self.greenspin)
     self.bluespin = SpinButton(rgbluma[2], 0., 1., 0.01)
-    hbox.pack_start(self.bluespin, False, False, 0)
-    hbox = Gtk.HButtonBox(homogeneous = True, spacing = 16, halign = Gtk.Align.START)
-    wbox.pack_start(hbox, False, False, 0)
+    hbox.pack(8*" "+"Blue:")
+    hbox.pack(self.bluespin)
+    hbox = HButtonBox()
+    wbox.pack(hbox)
     applybutton = Button(label = "OK")
     applybutton.connect("clicked", self.apply)
-    hbox.pack_start(applybutton, False, False, 0)
+    hbox.pack(applybutton)
     humanbutton = Button(label = "Human")
     humanbutton.connect("clicked", self.set_human_vision)
-    hbox.pack_start(humanbutton, False, False, 0)
+    hbox.pack(humanbutton)
     uniformbutton = Button(label = "Uniform")
     uniformbutton.connect("clicked", self.set_uniform_rgb)
-    hbox.pack_start(uniformbutton, False, False, 0)
+    hbox.pack(uniformbutton)
     cancelbutton = Button(label = "Cancel")
     cancelbutton.connect("clicked", lambda button: self.destroy())
-    hbox.pack_start(cancelbutton, False, False, 0)
+    hbox.pack(cancelbutton)
     self.callback = callback
     self.show_all()
 
   def apply(self, *args, **kwargs):
     """Apply luma RGB settings."""
     red = self.redspin.get_value()
     green = self.greenspin.get_value()
```

### Comparing `eQuimage-1.3.0/src/eQuimage/windows/mainmenu.py` & `eQuimage-1.4.0/src/eQuimage/gui/mainmenu.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
+# GUI updated.
 
 """Main menu."""
 
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk, Gio
-from .gtk.customwidgets import CheckButton
-from .gtk.filechoosers import ImageChooserDialog
+from .gtk.customwidgets import HBox, VBox, CheckButton
+from .gtk.filechoosers import ImageFileChooserDialog
 from .base import ErrorDialog
 from .settings import SettingsWindow
-from .blackpoint import BlackPointTool
-from .arcsinh import ArcsinhStretchTool
-from .hyperbolic import GeneralizedHyperbolicStretchTool
-from .midtone import MidtoneStretchTool
-from .clahe import CLAHETool
-from .colorbalance import ColorBalanceTool
-from .colorsaturation import ColorSaturationTool
-from .ghscolorsat import GHSColorSaturationTool
-from .colornoise import ColorNoiseReductionTool
-from .hotpixels import RemoveHotPixelsTool
-from .wavelets import WaveletsFilterTool
-from .totalvariation import TotalVariationFilterTool
-from .bilateral import BilateralFilterTool
-from .unsharp import UnsharpMaskTool
-from .blend import BlendTool
-from .addframe import AddUnistellarFrame
+from .tools.blackpoint import BlackPointTool
+from .tools.arcsinh import ArcsinhStretchTool
+from .tools.hyperbolic import GeneralizedHyperbolicStretchTool
+from .tools.midtone import MidtoneStretchTool
+from .tools.clahe import CLAHETool
+from .tools.colorbalance import ColorBalanceTool
+from .tools.colorsaturation import ColorSaturationTool
+from .tools.ghscolorsat import GHSColorSaturationTool
+from .tools.colornoise import ColorNoiseReductionTool
+from .tools.grayscale import GrayScaleConversionTool
+from .tools.hotpixels import RemoveHotPixelsTool
+from .tools.gaussian import GaussianFilterTool
+from .tools.butterworth import ButterworthFilterTool
+from .tools.wavelets import WaveletsFilterTool
+from .tools.bilateral import BilateralFilterTool
+from .tools.nlmeans import NonLocalMeansFilterTool
+from .tools.totalvariation import TotalVariationFilterTool
+from .tools.unsharp import UnsharpMaskTool
+from .tools.thresholdmask import ThresholdMaskTool
+from .tools.blend import BlendTool
+from .tools.pixelmath import PixelMathTool
+from .tools.addframe import AddUnistellarFrame
+from .tools.switch import SwitchTool
 
 class MainMenu:
   """Main menu class."""
 
-  __XMLMENU__ = """
+  _XMLMENU_ = """
 <?xml version="1.0" encoding="UTF-8"?>
 <interface>
   <menu id="MainMenu">
     <submenu>
       <attribute name="label">File</attribute>
       <section>
         <item>
@@ -76,15 +84,15 @@
           <attribute name="label">Black point</attribute>
           <attribute name="action">app.blackpoint</attribute>
         </item>
       </section>
       <section>
         <item>
           <attribute name="label">Arcsinh stretch</attribute>
-          <attribute name="action">app.arcsinhstretch</attribute>
+          <attribute name="action">app.asinhstretch</attribute>
         </item>
         <item>
           <attribute name="label">Generalized hyperbolic stretch</attribute>
           <attribute name="action">app.GHstretch</attribute>
         </item>
         <item>
           <attribute name="label">Midtone stretch</attribute>
@@ -132,46 +140,75 @@
     <submenu>
       <attribute name="label">Filters</attribute>
       <section>
         <item>
           <attribute name="label">Remove hot pixels</attribute>
           <attribute name="action">app.hotpixels</attribute>
         </item>
+      </section>
+      <section>
         <item>
-          <attribute name="label">Wavelets filter</attribute>
-          <attribute name="action">app.wavelets</attribute>
+          <attribute name="label">Gaussian filter</attribute>
+          <attribute name="action">app.gaussian</attribute>
         </item>
         <item>
-          <attribute name="label">Total variation filter</attribute>
-          <attribute name="action">app.totalvariation</attribute>
+          <attribute name="label">Butterworth filter</attribute>
+          <attribute name="action">app.butterworth</attribute>
+        </item>
+        <item>
+          <attribute name="label">Wavelets filter</attribute>
+          <attribute name="action">app.wavelets</attribute>
         </item>
         <item>
           <attribute name="label">Bilateral filter</attribute>
           <attribute name="action">app.bilateral</attribute>
         </item>
+        <item>
+          <attribute name="label">Non-local means filter</attribute>
+          <attribute name="action">app.nlmeans</attribute>
+        </item>
+        <item>
+          <attribute name="label">Total variation filter</attribute>
+          <attribute name="action">app.totalvariation</attribute>
+        </item>
       </section>
       <section>
         <item>
           <attribute name="label">Sharpen (Laplacian)</attribute>
           <attribute name="action">app.sharpen</attribute>
         </item>
         <item>
           <attribute name="label">Unsharp mask</attribute>
           <attribute name="action">app.unsharp</attribute>
         </item>
       </section>
     </submenu>
     <submenu>
+      <attribute name="label">Masks</attribute>
+      <section>
+        <item>
+          <attribute name="label">Threshold mask</attribute>
+          <attribute name="action">app.thresholdmask</attribute>
+        </item>
+      </section>
+    </submenu>
+    <submenu>
       <attribute name="label">Operations</attribute>
       <section>
         <item>
           <attribute name="label">Blend</attribute>
           <attribute name="action">app.blend</attribute>
         </item>
       </section>
+      <section>
+        <item>
+          <attribute name="label">Pixel math</attribute>
+          <attribute name="action">app.pixelmath</attribute>
+        </item>
+      </section>
     </submenu>
     <submenu>
       <attribute name="label">Frames</attribute>
       <section>
         <item>
           <attribute name="label">Remove frame</attribute>
           <attribute name="action">app.removeframe</attribute>
@@ -188,249 +225,165 @@
         </item>
       </section>
     </submenu>
     <submenu>
       <attribute name="label">Logs</attribute>
       <section>
         <item>
-          <attribute name="label">Cancel last operation</attribute>
-          <attribute name="action">app.cancel</attribute>
+          <attribute name="label">Undo last operation</attribute>
+          <attribute name="action">app.undo</attribute>
           <attribute name="accel">&lt;Primary&gt;z</attribute>
         </item>
         <item>
-          <attribute name="label">Redo last cancelled operation</attribute>
+          <attribute name="label">Redo last operation</attribute>
           <attribute name="action">app.redo</attribute>
           <attribute name="accel">&lt;Primary&gt;r</attribute>
         </item>
       </section>
       <section>
         <item>
+          <attribute name="label">Switch to an other image</attribute>
+          <attribute name="action">app.switch</attribute>
+        </item>
+      </section>
+      <section>
+        <item>
           <attribute name="label">View logs</attribute>
           <attribute name="action">app.viewlogs</attribute>
           <attribute name="accel">&lt;Primary&gt;l</attribute>
         </item>
       </section>
     </submenu>
   </menu>
 </interface>
 """
 
   def __init__(self, app):
     """Build the main menu for app 'app'."""
+
+    def add_action(name, callback, context = {}):
+      """Add action with name 'name', callback 'callback', and context modifiers 'context'
+         (with respect to the default context {"noimage": False, "activetool": False, "nocancelled": True})."""
+      action = Gio.SimpleAction.new(name, None)
+      action.connect("activate", callback)
+      app.add_action(action)
+      actioncontext = {"noimage": False, "activetool": False, "nocancelled": True}
+      actioncontext.update(context)
+      self.actions.append((action, actioncontext))
+
     self.app = app
     self.actions = []
     #
     ### File.
     #
-    action = Gio.SimpleAction.new("open", None)
-    action.connect("activate", self.load_file)
-    app.add_action(action)
-    self.actions.append((action, {"noimage": True, "nooperations": True, "activetool": False, "noframe": True, "nocancelled": True}))
-    #
-    action = Gio.SimpleAction.new("save", None)
-    action.connect("activate", self.save_file)
-    app.add_action(action)
-    self.actions.append((action, {"noimage": False, "nooperations": False, "activetool": False, "noframe": True, "nocancelled": True}))
-    #
-    action = Gio.SimpleAction.new("close", None)
-    action.connect("activate", self.close)
-    app.add_action(action)
-    self.actions.append((action, {"noimage": False, "nooperations": True, "activetool": False, "noframe": True, "nocancelled": True}))
-    #
-    action = Gio.SimpleAction.new("settings", None)
-    action.connect("activate", lambda action, parameter: SettingsWindow(app).open())
-    app.add_action(action)
-    self.actions.append((action, {"noimage": True, "nooperations": True, "activetool": False, "noframe": True, "nocancelled": True}))
-    #
-    action = Gio.SimpleAction.new("quit", None)
-    action.connect("activate", lambda action, parameter: app.mainwindow.close())
-    app.add_action(action)
-    self.actions.append((action, {"noimage": True, "nooperations": True, "activetool": True, "noframe": True, "nocancelled": True}))
+    add_action("open", self.load_file, {"noimage": True})
+    add_action("save", self.save_file)
+    add_action("close", self.close)
+    #
+    add_action("settings", lambda action, parameter: SettingsWindow(app).open(), {"noimage": True})
+    #
+    add_action("quit", lambda action, parameter: app.mainwindow.close(), {"noimage": True, "activetool": True})
     #
     ### Stretch.
     #
-    action = Gio.SimpleAction.new("blackpoint", None)
-    action.connect("activate", lambda action, parameter: app.run_tool(BlackPointTool, app.stretchotf))
-    app.add_action(action)
-    self.actions.append((action, {"noimage": False, "nooperations": True, "activetool": False, "noframe": True, "nocancelled": True}))
-    #
-    action = Gio.SimpleAction.new("arcsinhstretch", None)
-    action.connect("activate", lambda action, parameter: app.run_tool(ArcsinhStretchTool, app.stretchotf))
-    app.add_action(action)
-    self.actions.append((action, {"noimage": False, "nooperations": True, "activetool": False, "noframe": True, "nocancelled": True}))
-    #
-    action = Gio.SimpleAction.new("GHstretch", None)
-    action.connect("activate", lambda action, parameter: app.run_tool(GeneralizedHyperbolicStretchTool, app.stretchotf))
-    app.add_action(action)
-    self.actions.append((action, {"noimage": False, "nooperations": True, "activetool": False, "noframe": True, "nocancelled": True}))
-    #
-    action = Gio.SimpleAction.new("MTstretch", None)
-    action.connect("activate", lambda action, parameter: app.run_tool(MidtoneStretchTool, app.stretchotf))
-    app.add_action(action)
-    self.actions.append((action, {"noimage": False, "nooperations": True, "activetool": False, "noframe": True, "nocancelled": True}))
-    #
-    action = Gio.SimpleAction.new("CLAHE", None)
-    action.connect("activate", lambda action, parameter: app.run_tool(CLAHETool))
-    app.add_action(action)
-    self.actions.append((action, {"noimage": False, "nooperations": True, "activetool": False, "noframe": True, "nocancelled": True}))
+    add_action("blackpoint", lambda action, parameter: app.run_tool(BlackPointTool, app.stretchotf))
+    #
+    add_action("asinhstretch", lambda action, parameter: app.run_tool(ArcsinhStretchTool, app.stretchotf))
+    add_action("GHstretch", lambda action, parameter: app.run_tool(GeneralizedHyperbolicStretchTool, app.stretchotf))
+    add_action("MTstretch", lambda action, parameter: app.run_tool(MidtoneStretchTool, app.stretchotf))
+    #
+    add_action("CLAHE", lambda action, parameter: app.run_tool(CLAHETool))
     #
     ### Colors.
     #
-    action = Gio.SimpleAction.new("colorbalance", None)
-    action.connect("activate", lambda action, parameter: app.run_tool(ColorBalanceTool, app.colorotf))
-    app.add_action(action)
-    self.actions.append((action, {"noimage": False, "nooperations": True, "activetool": False, "noframe": True, "nocancelled": True}))
-    #
-    action = Gio.SimpleAction.new("colorsaturation", None)
-    action.connect("activate", lambda action, parameter: app.run_tool(ColorSaturationTool, app.colorotf))
-    app.add_action(action)
-    self.actions.append((action, {"noimage": False, "nooperations": True, "activetool": False, "noframe": True, "nocancelled": True}))
-    #
-    action = Gio.SimpleAction.new("GHScolorsat", None)
-    action.connect("activate", lambda action, parameter: app.run_tool(GHSColorSaturationTool, app.stretchotf))
-    app.add_action(action)
-    self.actions.append((action, {"noimage": False, "nooperations": True, "activetool": False, "noframe": True, "nocancelled": True}))
-    #
-    action = Gio.SimpleAction.new("colornoise", None)
-    action.connect("activate", lambda action, parameter: app.run_tool(ColorNoiseReductionTool, app.colorotf))
-    app.add_action(action)
-    self.actions.append((action, {"noimage": False, "nooperations": True, "activetool": False, "noframe": True, "nocancelled": True}))
-    #
-    action = Gio.SimpleAction.new("negative", None)
-    action.connect("activate", lambda action, parameter: app.negative())
-    app.add_action(action)
-    self.actions.append((action, {"noimage": False, "nooperations": True, "activetool": False, "noframe": True, "nocancelled": True}))
-    #
-    action = Gio.SimpleAction.new("grayscale", None)
-    action.connect("activate", lambda action, parameter: app.gray_scale())
-    app.add_action(action)
-    self.actions.append((action, {"noimage": False, "nooperations": True, "activetool": False, "noframe": True, "nocancelled": True}))
+    add_action("colorbalance", lambda action, parameter: app.run_tool(ColorBalanceTool, app.colorotf))
+    add_action("colorsaturation", lambda action, parameter: app.run_tool(ColorSaturationTool, app.colorotf))
+    add_action("GHScolorsat", lambda action, parameter: app.run_tool(GHSColorSaturationTool, app.stretchotf))
+    add_action("colornoise", lambda action, parameter: app.run_tool(ColorNoiseReductionTool, app.colorotf))
+    #
+    add_action("negative", lambda action, parameter: app.negative())
+    add_action("grayscale", lambda action, parameter: app.run_tool(GrayScaleConversionTool, app.colorotf))
     #
     ### Filters.
     #
-    action = Gio.SimpleAction.new("hotpixels", None)
-    action.connect("activate", lambda action, parameter: app.run_tool(RemoveHotPixelsTool, app.hotpixelsotf))
-    app.add_action(action)
-    self.actions.append((action, {"noimage": False, "nooperations": True, "activetool": False, "noframe": True, "nocancelled": True}))
-    #
-    action = Gio.SimpleAction.new("sharpen", None)
-    action.connect("activate", lambda action, parameter: app.sharpen())
-    app.add_action(action)
-    self.actions.append((action, {"noimage": False, "nooperations": True, "activetool": False, "noframe": True, "nocancelled": True}))
-    #
-    action = Gio.SimpleAction.new("wavelets", None)
-    action.connect("activate", lambda action, parameter: app.run_tool(WaveletsFilterTool))
-    app.add_action(action)
-    self.actions.append((action, {"noimage": False, "nooperations": True, "activetool": False, "noframe": True, "nocancelled": True}))
-    #
-    action = Gio.SimpleAction.new("totalvariation", None)
-    action.connect("activate", lambda action, parameter: app.run_tool(TotalVariationFilterTool))
-    app.add_action(action)
-    self.actions.append((action, {"noimage": False, "nooperations": True, "activetool": False, "noframe": True, "nocancelled": True}))
-    #
-    action = Gio.SimpleAction.new("bilateral", None)
-    action.connect("activate", lambda action, parameter: app.run_tool(BilateralFilterTool))
-    app.add_action(action)
-    self.actions.append((action, {"noimage": False, "nooperations": True, "activetool": False, "noframe": True, "nocancelled": True}))
-    #
-    action = Gio.SimpleAction.new("unsharp", None)
-    action.connect("activate", lambda action, parameter: app.run_tool(UnsharpMaskTool))
-    app.add_action(action)
-    self.actions.append((action, {"noimage": False, "nooperations": True, "activetool": False, "noframe": True, "nocancelled": True}))
+    add_action("hotpixels", lambda action, parameter: app.run_tool(RemoveHotPixelsTool, app.hotpixelsotf))
+    #
+    add_action("gaussian", lambda action, parameter: app.run_tool(GaussianFilterTool))
+    add_action("butterworth", lambda action, parameter: app.run_tool(ButterworthFilterTool))
+    add_action("wavelets", lambda action, parameter: app.run_tool(WaveletsFilterTool))
+    add_action("bilateral", lambda action, parameter: app.run_tool(BilateralFilterTool))
+    add_action("nlmeans", lambda action, parameter: app.run_tool(NonLocalMeansFilterTool))
+    add_action("totalvariation", lambda action, parameter: app.run_tool(TotalVariationFilterTool))
+    #
+    add_action("sharpen", lambda action, parameter: app.sharpen())
+    add_action("unsharp", lambda action, parameter: app.run_tool(UnsharpMaskTool))
+    #
+    ### Masks.
+    #
+    add_action("thresholdmask", lambda action, parameter: app.run_tool(ThresholdMaskTool))
     #
     ### Operations.
     #
-    action = Gio.SimpleAction.new("blend", None)
-    action.connect("activate", lambda action, parameter: app.run_tool(BlendTool, app.blendotf))
-    app.add_action(action)
-    self.actions.append((action, {"noimage": False, "nooperations": True, "activetool": False, "noframe": True, "nocancelled": True}))
+    add_action("blend", lambda action, parameter: app.run_tool(BlendTool, app.blendotf))
+    #
+    add_action("pixelmath", lambda action, parameter: app.run_tool(PixelMathTool))
     #
     ### Frames.
     #
-    action = Gio.SimpleAction.new("removeframe", None)
-    action.connect("activate", lambda action, parameter: app.remove_unistellar_frame())
-    app.add_action(action)
-    self.actions.append((action, {"noimage": False, "nooperations": True, "activetool": False, "noframe": False, "nocancelled": True}))
-    #
-    action = Gio.SimpleAction.new("restoreframe", None)
-    action.connect("activate", lambda action, parameter: app.restore_unistellar_frame())
-    app.add_action(action)
-    self.actions.append((action, {"noimage": False, "nooperations": True, "activetool": False, "noframe": False, "nocancelled": True}))
-    #
-    action = Gio.SimpleAction.new("addframe", None)
-    action.connect("activate", lambda action, parameter: app.run_tool(AddUnistellarFrame))
-    app.add_action(action)
-    self.actions.append((action, {"noimage": False, "nooperations": True, "activetool": False, "noframe": True, "nocancelled": True}))
+    add_action("removeframe", lambda action, parameter: app.remove_unistellar_frame())
+    add_action("restoreframe", lambda action, parameter: app.restore_unistellar_frame())
+    #
+    add_action("addframe", lambda action, parameter: app.run_tool(AddUnistellarFrame))
     #
     ### Logs.
     #
-    action = Gio.SimpleAction.new("cancel", None)
-    action.connect("activate", lambda action, parameter: app.cancel_last_operation())
-    app.add_action(action)
-    self.actions.append((action, {"noimage": False, "nooperations": False, "activetool": False, "noframe": True, "nocancelled": True}))
-    #
-    action = Gio.SimpleAction.new("redo", None)
-    action.connect("activate", lambda action, parameter: app.redo_last_cancelled())
-    app.add_action(action)
-    self.actions.append((action, {"noimage": True, "nooperations": True, "activetool": False, "noframe": True, "nocancelled": False}))
-    #
-    action = Gio.SimpleAction.new("viewlogs", None)
-    action.connect("activate", lambda action, parameter: app.logwindow.open())
-    app.add_action(action)
-    self.actions.append((action, {"noimage": False, "nooperations": True, "activetool": True, "noframe": True, "nocancelled": True}))
+    add_action("undo", lambda action, parameter: app.undo())
+    add_action("redo", lambda action, parameter: app.redo(), {"noimage": True, "nocancelled": False})
+    #
+    add_action("switch", lambda action, parameter: app.run_tool(SwitchTool))
+    #
+    add_action("viewlogs", lambda action, parameter: app.logwindow.open(), {"activetool": True})
     #
     ###
     #
-    builder = Gtk.Builder.new_from_string(self.__XMLMENU__, -1)
+    builder = Gtk.Builder.new_from_string(self._XMLMENU_, -1)
     app.set_menubar(builder.get_object("MainMenu"))
     self.update()
 
-  def update(self, present = True):
-    """Update main menu."""
+  def update(self):
+    """Update main menu according to the application context."""
     context = self.app.get_context()
     for action, enable in self.actions:
       if not context["image"]:
         enabled = enable["noimage"]
       elif context["activetool"]:
         enabled = enable["activetool"]
       else:
         enabled = True
-      if not context["frame"]:
-        enabled = enabled and enable["noframe"]
-      if not context["operations"]:
-        enabled = enabled and enable["nooperations"]
       if not context["cancelled"]:
         enabled = enabled and enable["nocancelled"]
       action.set_enabled(enabled)
 
   def load_file(self, *args, **kwargs):
     """Open file dialog and load image file."""
-    filename = ImageChooserDialog(self.app.mainwindow.window, Gtk.FileChooserAction.OPEN, preview = True)
+    filename = ImageFileChooserDialog(self.app.mainwindow.window, Gtk.FileChooserAction.OPEN, preview = True)
     if filename is None: return
     try:
       self.app.load_file(filename)
     except Exception as err:
       ErrorDialog(self.app.mainwindow.window, str(err))
 
   def save_file(self, *args, **kwargs):
     """Open file dialog and save image file."""
     if not self.app.get_context("image"): return
     # Add extra widget to choose the color depth of png and tiff files.
-    #widget = Gtk.HBox(spacing = 8)
-    #widget.pack_start(Gtk.Label(label = "Color depth (for png and tiff files):"), False, False, 0)
-    #button8 = RadioButton.new_with_label_from_widget(None, "8 bits")
-    #widget.pack_start(button8, False, False, 0)
-    #button16 = RadioButton.new_with_label_from_widget(button8, "16 bits")
-    #widget.pack_start(button16, False, False, 0)
     depthbutton = CheckButton(label = "16 bits color depth (for png and tiff files)")
-    #filename = ImageChooserDialog(self.app.mainwindow.window, Gtk.FileChooserAction.SAVE, path = self.app.get_savename(), extra_widget = widget)
-    filename = ImageChooserDialog(self.app.mainwindow.window, Gtk.FileChooserAction.SAVE, path = self.app.get_savename(), extra_widget = depthbutton)
+    filename = ImageFileChooserDialog(self.app.mainwindow.window, Gtk.FileChooserAction.SAVE, path = self.app.get_savename(), extra_widget = depthbutton)
     if filename is None: return
     try:
-      #self.app.save_file(filename, depth = 8 if button8.get_active() else 16)
       self.app.save_file(filename, depth = 16 if depthbutton.get_active() else 8)
     except Exception as err:
       ErrorDialog(self.app.mainwindow.window, str(err))
 
   def close(self, *args, **kwargs):
     """Close current image."""
     if not self.app.get_context("image"): return
```

### Comparing `eQuimage-1.3.0/src/eQuimage/windows/mainwindow.py` & `eQuimage-1.4.0/src/eQuimage/gui/mainwindow.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
+# GUI updated.
 
 """Main window."""
 
+import os
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk, Gdk, GObject
 from .gtk.utils import get_work_area
-from .gtk.signals import Signals
-from .gtk.customwidgets import CheckButton, HScale, Notebook
-from .base import BaseWindow, BaseToolbar, Container
+from .gtk.customwidgets import Align, Label, HBox, VBox, Button, CheckButton, HScale, Notebook
+from .gtk.keyboard import decode_key
+from .base import BaseWindow, FigureCanvas, BaseToolbar, Container
 from .luma import LumaRGBDialog
 from .statistics import StatsWindow
 from ..imageprocessing import imageprocessing
 import numpy as np
-from matplotlib.backends.backend_gtk3agg import FigureCanvasGTK3Agg as FigureCanvas
 from matplotlib.figure import Figure
 from collections import OrderedDict as OD
 
 class MainWindow:
   """Main window class."""
 
   MAXIMGSIZE = 0.75 # Maximal width/height of the image (as a fraction of the screen resolution).
 
   SHADOWCOLOR = np.array([[1.], [.5], [0.]], dtype = imageprocessing.IMGTYPE)
   HIGHLIGHTCOLOR = np.array([[1.], [1.], [0.]], dtype = imageprocessing.IMGTYPE)
   DIFFCOLOR = np.array([[1.], [1.], [0.]], dtype = imageprocessing.IMGTYPE)
 
-  __help__ = """[PAGE DOWN]: Next image tab
+  _help_ = """[PAGE DOWN]: Next image tab
 [PAGE UP]: Previous image tab
 [D] : Show image description (if available)
 [S]: Statistics (of the zoomed area)
 [CTRL+C]: Copy image in a new tab
 [CTRL+V]: Paste tab parameters to the tool
 [CTRL+X]: Close image tab (if possible)
 [CTRL+TAB]: Toggle between main and tool windows""" # Help tootip.
@@ -46,83 +47,82 @@
   def open(self):
     """Open main window."""
     self.window = Gtk.ApplicationWindow(application = self.app, title = "eQuimage v"+self.app.version)
     self.window.connect("delete-event", self.close)
     self.window.connect("key-press-event", self.key_press)
     self.window.connect("key-release-event", self.key_release)
     self.widgets = Container()
-    wbox = Gtk.VBox()
+    wbox = VBox(spacing = 0)
     self.window.add(wbox)
     fig = Figure()
     ax = fig.add_axes([0., 0., 1., 1.])
     self.canvas = FigureCanvas(fig)
-    wbox.pack_start(self.canvas, True, True, 0)
     self.canvas.size = (-1, -1)
-    hbox = Gtk.HBox()
-    wbox.pack_start(hbox, False, False, 0)
-    self.tabs = Notebook()
-    self.tabs.set_tab_pos(Gtk.PositionType.BOTTOM)
+    wbox.pack(self.canvas, expand = True, fill = True)
+    hbox = HBox(spacing = 0)
+    wbox.pack(hbox)
+    self.tabs = Notebook(pos = Gtk.PositionType.BOTTOM)
     self.tabs.set_scrollable(True)
     self.tabs.set_show_border(False)
     self.tabs.connect("switch-page", lambda tabs, tab, itab: self.display_tab(itab))
-    hbox.pack_start(self.tabs, True, True, 0)
-    label = Gtk.Label("?", halign = Gtk.Align.END)
-    label.set_tooltip_text(self.__help__)
-    hbox.pack_start(label, False, False, 8)
-    hbox = Gtk.HBox()
-    wbox.pack_start(hbox, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = "Output range Min:"), False, False, 4)
+    hbox.pack(self.tabs, expand = True, fill = True)
+    label = Label("?")
+    label.set_tooltip_text(self._help_)
+    hbox.pack(label, padding = 8)
+    hbox = HBox(spacing = 0)
+    wbox.pack(hbox)
+    hbox.pack("Output range Min:", padding = 4)
     self.widgets.minscale = HScale(0., 0., 1., 0.01, length = 128)
     self.widgets.minscale.connect("value-changed", lambda scale: self.update_output_range("Min"))
-    hbox.pack_start(self.widgets.minscale, True, True, 4)
+    hbox.pack(self.widgets.minscale, expand = True, fill = True, padding = 4)
     self.widgets.spinner = Gtk.Spinner()
-    hbox.pack_start(self.widgets.spinner, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = "Max:"), False, False, 4)
+    hbox.pack(self.widgets.spinner, padding = 4)
+    hbox.pack("Max:", padding = 4)
     self.widgets.maxscale = HScale(1., 0., 1., 0.01, length = 128)
     self.widgets.maxscale.connect("value-changed", lambda scale: self.update_output_range("Max"))
-    hbox.pack_start(self.widgets.maxscale, True, True, 4)
-    hbox = Gtk.HBox()
-    wbox.pack_start(hbox, False, False, 0)
+    hbox.pack(self.widgets.maxscale, expand = True, fill = True, padding = 4)
+    hbox = HBox(spacing = 0)
+    wbox.pack(hbox)
     self.widgets.redbutton = CheckButton(label = "Red")
     self.widgets.redbutton.set_active(True)
     self.widgets.redbutton.connect("toggled", lambda button: self.update_channels("R"))
-    hbox.pack_start(self.widgets.redbutton, False, False, 0)
+    hbox.pack(self.widgets.redbutton)
     self.widgets.greenbutton = CheckButton(label = "Green")
     self.widgets.greenbutton.set_active(True)
     self.widgets.greenbutton.connect("toggled", lambda button: self.update_channels("G"))
-    hbox.pack_start(self.widgets.greenbutton, False, False, 0)
+    hbox.pack(self.widgets.greenbutton)
     self.widgets.bluebutton = CheckButton(label = "Blue")
     self.widgets.bluebutton.set_active(True)
     self.widgets.bluebutton.connect("toggled", lambda button: self.update_channels("B"))
-    hbox.pack_start(self.widgets.bluebutton, False, False, 0)
+    hbox.pack(self.widgets.bluebutton)
     self.widgets.lumabutton = CheckButton(label = self.rgb_luma_string())
     self.widgets.lumabutton.set_active(False)
     self.widgets.lumabutton.connect("toggled", lambda button: self.update_channels("L"))
-    hbox.pack_start(self.widgets.lumabutton, False, False, 0)
-    self.widgets.rgblumabutton = Gtk.Button(label = "Set", halign = Gtk.Align.START)
+    hbox.pack(self.widgets.lumabutton)
+    self.widgets.rgblumabutton = Button(label = "Set", halign = Align.START)
     self.widgets.rgblumabutton.connect("clicked", lambda button: LumaRGBDialog(self.window, self.set_rgb_luma, self.get_rgb_luma()))
-    hbox.pack_start(self.widgets.rgblumabutton, True, True, 0)
+    hbox.pack(self.widgets.rgblumabutton, expand = True, fill = True)
     self.widgets.shadowbutton = CheckButton(label = "Shadowed")
     self.widgets.shadowbutton.set_active(False)
     self.widgets.shadowbutton.connect("toggled", lambda button: self.update_modifiers("S"))
-    hbox.pack_start(self.widgets.shadowbutton, False, False, 0)
+    hbox.pack(self.widgets.shadowbutton)
     self.widgets.highlightbutton = CheckButton(label = "Highlighted")
     self.widgets.highlightbutton.set_active(False)
     self.widgets.highlightbutton.connect("toggled", lambda button: self.update_modifiers("H"))
-    hbox.pack_start(self.widgets.highlightbutton, False, False, 0)
+    hbox.pack(self.widgets.highlightbutton)
     self.widgets.diffbutton = CheckButton(label = "Differences")
     self.widgets.diffbutton.set_active(False)
     self.widgets.diffbutton.connect("toggled", lambda button: self.update_modifiers("D"))
-    hbox.pack_start(self.widgets.diffbutton, False, False, 0)
+    hbox.pack(self.widgets.diffbutton)
     self.widgets.toolbar = BaseToolbar(self.canvas, fig)
-    wbox.pack_start(self.widgets.toolbar, False, False, 0)
+    wbox.pack(self.widgets.toolbar)
     self.set_copy_paste_callbacks(None, None)
     self.set_rgb_luma_callback(None)
     self.set_guide_lines(None)
-    self.descpopup = None
+    self.popup = None
     self.statswindow = StatsWindow(self.app)
     self.reset_images()
     self.window.show_all()
 
   def close(self, *args, **kwargs):
     """Quit application."""
     dialog = Gtk.MessageDialog(transient_for = self.window,
@@ -132,48 +132,62 @@
     dialog.set_markup("Are you sure you want to quit ?")
     response = dialog.run()
     dialog.destroy()
     if response != Gtk.ResponseType.OK: return True
     print("Exiting eQuimage...")
     self.app.quit()
 
-  # Update tabs.
+  # Images/tabs associations.
 
   def get_current_tab(self):
     """Return current tab."""
     return self.tabs.get_current_page()
 
   def set_current_tab(self, tab):
     """Set current tab 'tab'."""
     if self.get_current_tab() != tab: self.tabs.set_current_page(tab)
 
   def display_tab(self, tab):
     """Display image of tab 'tab'."""
     keys = list(self.images.keys())
     self.draw_image(keys[tab])
 
+  def update_tab_label(self, tab, label):
+    """Update the label 'label' of tab 'tab'."""
+    self.tabs.set_tab_label(self.tabs.get_nth_page(tab), Label(label))
+
   def get_keys(self):
     """Return the list of image keys."""
     return list(self.images.keys())
 
+  def get_key_tab(self, tab):
+    """Return the image key of tab 'tab'."""
+    return list(self.images.keys())[tab]
+
+  def get_tab_key(self, key):
+    """Return the tab of image 'key'."""
+    try:
+      return list(self.images.keys()).index(key)
+    except KeyError:
+      raise KeyError(f"There is no image with key '{key}'.")
+
   def get_current_key(self):
-    """Return the key associated to the current tab."""
+    """Return the image key of the current tab."""
     tab = self.get_current_tab()
-    if tab < 0: return None
-    keys = list(self.images.keys())
-    return keys[tab]
+    return self.get_key_tab(tab) if tab >= 0 else None
 
   def set_current_key(self, key):
-    """Set current key 'key'."""
-    try:
-      tab = list(self.images.keys()).index(key)
-    except KeyError:
-      raise KeyError("There is no image with key '{key}'.")
-      return
-    self.set_current_tab(tab)
+    """Set current tab with image 'key'."""
+    tab = self.get_tab_key(key)
+    if tab is not None: self.set_current_tab(tab)
+
+  def update_key_label(self, key, label):
+    """Update the tab label 'label' of image 'key'."""
+    tab = self.get_tab_key(key)
+    if tab is not None: self.update_tab_label(tab, label)
 
   # Update displayed channels.
 
   def update_channels(self, toggled):
     """Update channels buttons."""
     if toggled == "L":
       luma = self.widgets.lumabutton.get_active()
@@ -218,50 +232,48 @@
       self.widgets.minscale.set_value_block(vmin)
       self.widgets.maxscale.set_value_block(vmax)
     self.refresh_image()
 
   # Image modifiers (shadow, highlight, difference).
 
   def difference(self, image, reference, channels):
-    """Highlight differences between 'image' and 'reference' with DIFFCOLOR color."""
-    diff = image.copy()
+    """Highlight differences between 'image' and 'reference' with color DIFFCOLOR."""
+    if reference is None: return
+    if reference.shape != image.shape: return
     mask = np.any(image[channels] != reference[channels], axis = 0)
-    diff[:, mask] = self.DIFFCOLOR
-    return diff
+    image[:, mask] = self.DIFFCOLOR
 
   def shadow_highlight(self, image, reference, channels, shadow = True, highlight = True):
     """If shadow is True,
          show pixels black on 'image' and     on 'reference' with color 0.5*SHADOWCOLOR,
          and  pixels black on 'image' but not on 'reference' with color     SHADOWCOLOR,
        If higlight is True,
          show pixels with at least one channel >= 1 on 'image' and     on  'reference' with color 0.5*HIGHLIGHTCOLOR,
          and  pixels with at least one channel >= 1 on 'image' but not on  'reference' with color     HIGHLIGHTCOLOR."""
-    swhl = image.copy()
     if shadow:
-      imgmask = np.all(image[channels] < imageprocessing.IMGTOL, axis = 0)
-      if image.shape == reference.shape:
-        refmask = np.all(reference[channels] < imageprocessing.IMGTOL, axis = 0)
-        swhl[:, imgmask &  refmask] = 0.5*self.SHADOWCOLOR
-        swhl[:, imgmask & ~refmask] =     self.SHADOWCOLOR
-      else:
-        swhl[:, imgmask] = self.SHADOWCOLOR
+      shadowmask = np.all(image[channels] < imageprocessing.IMGTOL, axis = 0)
     if highlight:
-      imgmask = np.any(image[channels] > 1.-imageprocessing.IMGTOL, axis = 0)
-      if image.shape == reference.shape:
-        refmask = np.any(reference[channels] > 1.-imageprocessing.IMGTOL, axis = 0)
-        swhl[:, imgmask &  refmask] = 0.5*self.HIGHLIGHTCOLOR
-        swhl[:, imgmask & ~refmask] =     self.HIGHLIGHTCOLOR
-      else:
-        swhl[:, imgmask] = self.HIGHLIGHTCOLOR
-    return swhl
+      hlightmask = np.any(image[channels] > 1.-imageprocessing.IMGTOL, axis = 0)
+    if shadow:
+      image[:, shadowmask] = self.SHADOWCOLOR
+      if reference is not None:
+        if reference.shape == image.shape:
+          refmask = np.all(reference[channels] < imageprocessing.IMGTOL, axis = 0)
+          image[:, shadowmask & refmask] = 0.5*self.SHADOWCOLOR
+    if highlight:
+      image[:, hlightmask] = self.HIGHLIGHTCOLOR
+      if reference is not None:
+        if reference.shape == image.shape:
+          refmask = np.any(reference[channels] > 1.-imageprocessing.IMGTOL, axis = 0)
+          image[:, hlightmask & refmask] = 0.5*self.HIGHLIGHTCOLOR
 
   # Draw or refresh the image displayed in the main window.
 
   def set_canvas_size(self, width, height):
-    """Set canvas size for a target figure width 'width' and height 'height'."""
+    """Set canvas size for a figure width 'width' and height 'height'."""
     swidth, sheight = get_work_area(self.window)
     cwidth, cheight = self.MAXIMGSIZE*swidth, self.MAXIMGSIZE*swidth*height/width
     if cheight > self.MAXIMGSIZE*sheight:
       cwidth, cheight = self.MAXIMGSIZE*sheight*width/height, self.MAXIMGSIZE*sheight
     if self.canvas.size != (cwidth, cheight):
       self.canvas.size = (cwidth, cheight)
       self.canvas.set_size_request(cwidth, cheight)
@@ -269,40 +281,42 @@
 
   def draw_image(self, key):
     """Apply modifiers and draw image with key 'key'."""
     if key is None: return
     try:
       image = self.images[key]
     except KeyError:
-      raise KeyError("There is no image with key '{key}'.")
-      return
+      raise KeyError(f"There is no image with key '{key}'.")
+    reference = None
     shadow = self.widgets.shadowbutton.get_active()
     highlight = self.widgets.highlightbutton.get_active()
     diff = self.widgets.diffbutton.get_active()
     modifiers = shadow or highlight or diff
     luma = self.widgets.lumabutton.get_active()
     if luma:
-      image = np.repeat(image.lum[np.newaxis], 3, axis = 0)
+      image = np.repeat(image._luma_[np.newaxis], 3, axis = 0)
       channels = np.array([True, False, False])
-      if modifiers: reference = np.repeat(self.reference.lum[np.newaxis], 3, axis = 0)
+      if modifiers and self.refkey is not None:
+        reference = np.repeat(self.images[self.refkey]._luma_[np.newaxis], 3, axis = 0)
     else:
-      image = image.get_image().copy()
+      image = image.get_image_copy()
       channels = np.array([self.widgets.redbutton.get_active(), self.widgets.greenbutton.get_active(), self.widgets.bluebutton.get_active()])
       image[~channels] = 0.
-      if modifiers: reference = self.reference.get_image()
+      if modifiers and self.refkey is not None:
+        reference = self.images[self.refkey].get_image()
     if modifiers:
       if diff:
-        if image.shape == reference.shape: image = self.difference(image, reference, channels)
-      elif shadow or highlight:
-        image = self.shadow_highlight(image, reference, channels, shadow, highlight)
+        self.difference(image, reference, channels)
+      else:
+        self.shadow_highlight(image, reference, channels, shadow, highlight)
     self.refresh_image(image)
 
   def refresh_image(self, image = None):
-    """Draw (if 'image' is not None) or refresh the current image."""
-    update = self.currentimage is not None # Is this an update or fresh draw ?
+    """Draw 'image' (if not None) or refresh the current image."""
+    update = self.currentimage is not None # Is this an update or fresh plot ?
     if image is not None:
       currentshape = self.currentimage.shape if update else None
       self.currentimage = np.clip(np.moveaxis(image, 0, -1), 0., 1.)
       update = update and self.currentimage.shape == currentshape
     if self.currentimage is None: return # Nothing to draw !
     vmin = self.widgets.minscale.get_value() if self.widgets.minscale.get_sensitive() else 0.
     vmax = self.widgets.maxscale.get_value() if self.widgets.maxscale.get_sensitive() else 1.
@@ -334,100 +348,106 @@
       if nimages > 3:
         self.set_images(OD(Image = self.app.get_image(-1), Original = self.app.get_image(1)), reference = "Original")
       elif nimages > 0:
         self.set_images(OD(Original = self.app.get_image(1)), reference = "Original")
     else:
       self.set_canvas_size(800, 600)
       try:
-        splash = imageprocessing.load_image(self.app.get_packagepath()+"/images/splash.png", {"tag": "Welcome"})
+        splash = imageprocessing.load_image(os.path.join(self.app.get_packagepath(), "images", "splash.png"), {"tag": "Welcome"})
       except:
         splash = imageprocessing.black_image(800, 600, {"tag": "Welcome"})
       self.set_images(OD(Splash = splash))
 
   def set_images(self, images, reference = None):
     """Set main window images and reference."""
     self.tabs.block_all_signals()
     for tab in range(self.tabs.get_n_pages()): self.tabs.remove_page(-1)
     self.images = OD()
     for key, image in images.items():
-      #self.images[key] = image.clone()
       self.images[key] = image.ref()
-      self.images[key].lum = self.images[key].luma()
-    if reference is None:
-      self.reference = self.images[key]
-    else:
-      try:
-        self.reference = self.images[reference]
-      except KeyError:
-        raise KeyError("There is no image with key '{reference}'.")
-        self.reference = self.images[key]
-    self.reference.meta["deletable"] = False # Can't delete the reference image.
+      self.images[key]._luma_ = self.images[key].luma()
+    self.refkey = None
+    if reference is not None:
+      if reference not in self.images.keys():
+        raise KeyError(f"There is no image with key '{reference}'.")
+      self.refkey = reference
     for key, image in self.images.items():
       label = self.images[key].meta.get("tag", key)
-      if key == reference: label += " (\u2022)"
-      self.tabs.append_page(Gtk.Alignment(), Gtk.Label(label = label)) # Append a zero size dummy child.
+      if key == self.refkey: label += " (\u2022)"
+      self.tabs.append_page(Gtk.Alignment(), Label(label)) # Append a zero size dummy child.
     self.widgets.redbutton.set_active_block(True)
     self.widgets.greenbutton.set_active_block(True)
     self.widgets.bluebutton.set_active_block(True)
     self.widgets.lumabutton.set_active_block(False)
     self.widgets.shadowbutton.set_active_block(False)
     self.widgets.highlightbutton.set_active_block(False)
     self.widgets.diffbutton.set_active_block(False)
     self.widgets.minscale.set_sensitive(True)
     self.widgets.maxscale.set_sensitive(True)
-    self.widgets.shadowbutton.set_sensitive(True)
-    self.widgets.highlightbutton.set_sensitive(True)
-    self.widgets.diffbutton.set_sensitive(len(self.images) > 1)
+    self.widgets.diffbutton.set_sensitive(self.refkey is not None and len(self.images) > 1)
     self.tabs.unblock_all_signals()
     self.tabs.set_current_page(0)
     self.window.show_all()
 
   def append_image(self, key, image):
     """Append a new tab for image 'image' with key 'key'.
        This can be done only once set_images has been called."""
     if self.images is None:
       raise RuntimeError("The method 'set_images' must be called before 'append_image'.")
-      return
     if key in self.images.keys():
-      raise ValueError("The key '{key}' is already registered.")
-      return
+      raise KeyError(f"The key '{key}' is already registered.")
     self.tabs.block_all_signals()
-    #self.images[key] = image.clone()
     self.images[key] = image.ref()
-    self.images[key].lum = self.images[key].luma()
+    self.images[key]._luma_ = self.images[key].luma()
     label = self.images[key].meta.get("tag", key)
-    self.tabs.append_page(Gtk.Alignment(), Gtk.Label(label = label)) # Append a zero size dummy child.
+    self.tabs.append_page(Gtk.Alignment(), Label(label)) # Append a zero size dummy child.
     self.tabs.unblock_all_signals()
+    self.widgets.diffbutton.set_sensitive(self.refkey is not None)
     self.window.show_all()
 
-  def update_image(self, key, image):
-    """Update main window image with key 'key'."""
-    try:
-      #self.images[key] = image.clone()
+  def update_image(self, key, image, create = False):
+    """Update image with key 'key'.
+       A new tab is appended if 'key' does not exist and 'create' is True. Otherwise, a KeyError exception is raised."""
+    if key in self.images.keys():
       self.images[key] = image.ref()
-      self.images[key].lum = self.images[key].luma()
-      if self.get_current_key() == key: self.draw_image(key)
-    except KeyError:
-      raise KeyError("There is no image with key '{key}'.")
+      self.images[key]._luma_ = self.images[key].luma()
+      currentkey = self.get_current_key()
+      redraw = (currentkey == key)
+      if self.refkey == key:
+        shadow = self.widgets.shadowbutton.get_active()
+        highlight = self.widgets.highlightbutton.get_active()
+        diff = self.widgets.diffbutton.get_active()
+        redraw = redraw or shadow or highlight or diff
+      if redraw: self.draw_image(currentkey)
+    else:
+      if create:
+        self.append_image(key, image)
+      else:
+        raise KeyError(f"There is no image with key '{key}'.")
 
-  def delete_image(self, key, force = False):
-    """Delete image with key 'key' if image.meta["deletable"] is False or 'force' is True."""
+  def delete_image(self, key, force = False, failsafe = False):
+    """Delete image with key 'key' if image.meta["deletable"] is False or 'force' is True.
+       A KeyError exception is raised if image 'key' does not exist unless 'failsafe' is True."""
     try:
       image = self.images[key]
     except KeyError:
-      raise KeyError("There is no image with key '{key}'.")
+      if not failsafe: raise KeyError(f"There is no image with key '{key}'.")
       return
     deletable = image.meta.get("deletable", False)
     if not deletable and not force: return
+    if self.refkey == key:
+      self.widgets.diffbutton.set_active_block(False)
+      self.refkey = None
     self.tabs.block_all_signals()
     tab = list(self.images.keys()).index(key)
-    del image
+    del self.images[key]
     self.tabs.remove_page(tab)
     self.draw_image(self.get_current_key())
     self.tabs.unblock_all_signals()
+    self.widgets.diffbutton.set_sensitive(self.refkey is not None and len(self.images) > 1)
     self.window.show_all()
 
   def get_nbr_images(self):
     """Return the number of image tabs."""
     return self.tabs.get_n_pages()
 
   def next_image(self, *args, **kwargs):
@@ -442,34 +462,34 @@
     tab = (self.tabs.get_current_page()-1)%self.tabs.get_n_pages()
     self.tabs.set_current_page(tab)
 
   # Show image description.
 
   def show_description(self):
     """Open image description popup."""
-    if self.descpopup is not None: return
+    if self.popup is not None: return
     key = self.get_current_key()
     description = self.images[key].meta.get("description", None)
     if description is None: return
-    self.descpopup = Gtk.Window(Gtk.WindowType.POPUP, transient_for = self.window)
-    self.descpopup.set_position(Gtk.WindowPosition.CENTER_ON_PARENT)
-    self.descpopup.set_size_request(480, -1)
-    label = Gtk.Label(label = description, margin = 8)
+    self.popup = Gtk.Window(Gtk.WindowType.POPUP, transient_for = self.window)
+    self.popup.set_position(Gtk.WindowPosition.CENTER_ON_PARENT)
+    self.popup.set_size_request(480, -1)
+    label = Label(description, margin = 8)
     label.set_line_wrap(True)
-    self.descpopup.add(label)
-    self.descpopup.resize(1, 1)
-    self.descpopup.show_all()
+    self.popup.add(label)
+    self.popup.resize(1, 1)
+    self.popup.show_all()
 
   def hide_description(self):
     """Close image description popup."""
     try:
-      self.descpopup.destroy()
+      self.popup.destroy()
     except:
       pass
-    self.descpopup = None
+    self.popup = None
 
   # Show image statistics.
 
   def show_statistics(self):
     """Open image statistics window."""
     key = self.get_current_key()
     if key is None: return
@@ -488,44 +508,41 @@
     self.copy_callback = copy
     self.paste_callback = paste
 
   # Manage key press/release events.
 
   def key_press(self, widget, event):
     """Callback for key press in the main window."""
-    ctrl = event.state & Gdk.ModifierType.CONTROL_MASK
-    alt = event.state & Gdk.ModifierType.MOD1_MASK
-    if alt: return
-    keyname = Gdk.keyval_name(event.keyval).upper()
-    #print(keyname)
-    if ctrl:
+    kbrd = decode_key(event)
+    if kbrd.alt: return
+    if kbrd.ctrl:
       key = self.get_current_key()
       if key is None: return
-      if keyname == "C" and self.copy_callback is not None:
+      if kbrd.uname == "C" and self.copy_callback is not None:
         self.copy_callback(key, self.images[key])
-      elif keyname == "V" and self.paste_callback is not None:
+      elif kbrd.uname == "V" and self.paste_callback is not None:
         self.paste_callback(key, self.images[key])
-      elif keyname == "X":
+      elif kbrd.uname == "X":
         self.delete_image(key)
-      elif keyname == "TAB":
+      elif kbrd.uname == "TAB":
         if self.app.toolwindow.opened: self.app.toolwindow.window.present()
     else:
-      if keyname == "PAGE_UP":
+      if kbrd.uname == "PAGE_UP":
         self.previous_image()
-      elif keyname == "PAGE_DOWN":
+      elif kbrd.uname == "PAGE_DOWN":
         self.next_image()
-      elif keyname == "D":
+      elif kbrd.uname == "D":
         self.show_description()
-      elif keyname == "S":
+      elif kbrd.uname == "S":
         self.show_statistics()
 
   def key_release(self, widget, event):
     """Callback for key release in the main window."""
-    keyname = Gdk.keyval_name(event.keyval).upper()
-    if keyname == "D":
+    kbrd = decode_key(event)
+    if kbrd.uname == "D":
       self.hide_description()
 
   # Update luma RGB components.
 
   def get_rgb_luma(self):
     """Get luma RGB components."""
     return imageprocessing.get_rgb_luma()
@@ -541,30 +558,30 @@
     self.rgb_luma_callback = callback
 
   def set_rgb_luma(self, rgbluma):
     """Set luma RGB components 'rgbluma'."""
     imageprocessing.set_rgb_luma(rgbluma)
     self.widgets.lumabutton.set_label(self.rgb_luma_string(rgbluma))
     for key in self.images.keys():
-      self.images[key].lum = self.images[key].luma()
+      self.images[key]._luma_ = self.images[key].luma()
     if self.widgets.lumabutton.get_active(): self.draw_image(self.get_current_key())
     if self.rgb_luma_callback is not None: self.rgb_luma_callback(rgbluma)
 
   def lock_rgb_luma(self):
     """Lock luma RGB components (disable Set button)."""
     self.widgets.rgblumabutton.set_sensitive(False)
 
   def unlock_rgb_luma(self):
     """Unlock luma RGB components (enable Set button)."""
     self.widgets.rgblumabutton.set_sensitive(True)
 
   # Guide lines.
 
   def set_guide_lines(self, plot_guide_lines, redraw = True):
-    """Remove any existing guidelines and set new ones defined by the method 'plot_guide_lines'.
+    """Remove any existing guidelines and plot new ones with the method 'plot_guide_lines'.
        If not None, plot_guide_lines(ax) shall plot the guidelines in axes 'ax' and collect them in ax.guidelines.
        The main window canvas is redrawn if 'redraw' if True."""
     ax = self.canvas.figure.axes[0]
     try:
       for guideline in ax.guidelines: guideline.remove()
       del(ax.guidelines)
     except:
```

### Comparing `eQuimage-1.3.0/src/eQuimage/windows/picker.py` & `eQuimage-1.4.0/src/eQuimage/gui/misc/imagechooser.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,123 +1,126 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
+# GUI updated.
 
-"""Image picker widget."""
+"""Image chooser widget."""
 
 import os
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk, GObject
-from .gtk.customwidgets import Button
-from .gtk.filechoosers import ImageChooserDialog
-from .base import ErrorDialog
-from ..imageprocessing.imageprocessing import Image
-
-class ImagePicker():
-  """Image picker widget class."""
-
-  def __init__(self, app, window, vbox, callback = None):
-    """Add an image picker treeview in Gtk.VBox 'vbox' of window 'window' of app 'app'.
-       'callback(row, image)' is an optional method called upon image selection change, with 'image' the selected image on row 'row' of the treeview."""
+from ..gtk.customwidgets import HBox, VBox, HButtonBox, ScrolledBox, Button
+from ..gtk.filechoosers import ImageFileChooserDialog
+from ..base import ErrorDialog
+
+class ImageChooser():
+  """Image chooser widget class."""
+
+  def __init__(self, app, window, vbox, tabkey = "Selection", callback = None, last = False):
+    """Add an image chooser treeview in VBox 'vbox' of window 'window' of app 'app'. Display the selected image in tab 'tabkey' of the main
+       window (if not None). 'callback(row, image)' is an optional method called upon selection change, with 'image' the selected
+       image on row 'row' of the treeview. If 'last' is False, the last image/operation (the current image) is not included in the treeview."""
     self.app = app
     self.window = window
+    self.tabkey = tabkey
+    self.newtab = tabkey not in self.app.mainwindow.get_keys() # Is this a new tab ?
     self.callback = callback
     self.nfiles = 0
     self.nimages = 0
-    self.opentab = False
     self.imagestore = Gtk.ListStore(int, str, GObject.TYPE_PYOBJECT)
-    for operation, image, frame in self.app.operations[:-1]:
+    for operation, image, frame in self.app.operations[:None if last else -1]:
       self.nimages += 1
       self.imagestore.append([self.nimages, operation, image])
-    scrolled = Gtk.ScrolledWindow(vexpand = True, hexpand = True)
-    scrolled.set_min_content_width(480)
-    scrolled.set_min_content_height(200)
-    vbox.pack_start(scrolled, True, True, 0)
+    scrolled = ScrolledBox(480, 200)
+    vbox.pack(scrolled, expand = True, fill = True)
     self.treeview = Gtk.TreeView(model = self.imagestore, search_column = -1)
     scrolled.add(self.treeview)
     renderer = Gtk.CellRendererText()
-    renderer.set_property("xalign", 0.)
+    renderer.set_property("xalign", 1.)
     column = Gtk.TreeViewColumn("#", renderer, text = 0)
-    column.set_alignment(0.)
+    column.set_alignment(.5)
     column.set_expand(False)
     self.treeview.append_column(column)
     renderer = Gtk.CellRendererText()
     renderer.set_property("xalign", 0.)
     column = Gtk.TreeViewColumn("Operation", renderer, text = 1)
     column.set_alignment(0.)
     column.set_expand(True)
     self.treeview.append_column(column)
     self.selection = self.treeview.get_selection()
     self.selection.set_mode(Gtk.SelectionMode.SINGLE)
     self.selection.connect("changed", lambda selection: self.update())
-    hbox = Gtk.HBox(spacing = 8)
-    vbox.pack_start(hbox, False, False, 0)
+    hbox = HButtonBox()
+    vbox.pack(hbox)
     self.filebutton = Button(label = "Add file")
     self.filebutton.connect("clicked", self.load_file)
-    hbox.pack_start(self.filebutton, False, False, 0)
+    hbox.pack(self.filebutton)
 
   def load_file(self, *args, **kwargs):
     """Open file dialog and load an extra image file."""
-    filename = ImageChooserDialog(self.window, Gtk.FileChooserAction.OPEN, preview = True)
+    filename = ImageFileChooserDialog(self.window, Gtk.FileChooserAction.OPEN, preview = True)
     if filename is None: return
     try:
-      image = Image()
+      image = self.app.ImageClass()
       image.load(filename)
     except Exception as err:
       ErrorDialog(self.window, str(err))
       return
-    basename = os.path.basename(filename)
-    image.meta["pickertag"] = f"file = '{basename}'"
-    image.meta["description"] = basename
     self.nfiles += 1
     self.nimages += 1
+    basename = os.path.basename(filename)
+    image.meta["imchooser.row"] = self.nimages
+    image.meta["imchooser.file"] = basename
+    image.meta["imchooser.tag"] = f"file = '{basename}'"
+    image.meta["description"] = basename
     self.imagestore.append([self.nimages, f"Load('{basename}')", image])
 
   def get_image(self, row):
     """Get image on row 'row'."""
     return self.imagestore[row][2] if row >= 0 and row < self.nimages else None
 
   def get_image_tag(self, row):
     """Get tag of image on row 'row'."""
-    return self.imagestore[row][2].meta.get("pickertag", f"image = #{row+1}") if row >= 0 and row < self.nimages else ""
+    return self.imagestore[row][2].meta.get("imchooser.tag", f"image = #{row+1}") if row >= 0 and row < self.nimages else ""
 
   def get_selected_row(self):
     """Return selected row."""
     model, list_iter = self.selection.get_selected()
     return model[list_iter][0]-1 if list_iter is not None else -1
 
   def set_selected_row(self, row):
     """Set selected row 'row'."""
+    if row < 0: row = self.nimages+row
     if row >= 0 and row < self.nimages: self.treeview.set_cursor(row)
 
   def get_selected_image(self):
     """Return selected image."""
     model, list_iter = self.selection.get_selected()
     return model[list_iter][2] if list_iter is not None else None
 
   def get_selected_row_and_image(self):
     """Return selected row and image."""
     model, list_iter = self.selection.get_selected()
     return (model[list_iter][0]-1, model[list_iter][2]) if list_iter is not None else (None, None)
 
+  def get_images_list(self):
+    """Return the list of images in the treeview."""
+    return [image for n, operation, image in self.imagestore]
+
   def update(self):
     """Update main window selection tab."""
     row, image = self.get_selected_row_and_image()
-    if image is None:
-      if self.opentab:
-        self.app.mainwindow.delete_image("Selection")
-        self.opentab = False
-    if self.opentab:
-      self.app.mainwindow.update_image("Selection", image)
-    else:
-      self.app.mainwindow.append_image("Selection", image)
-      self.opentab = True
+    if self.tabkey is not None:
+      if image is None:
+        self.app.mainwindow.delete_image(self.tabkey, force = self.newtab, failsafe = True)
+      else:
+        self.app.mainwindow.update_image(self.tabkey, image, create = self.newtab)
     if self.callback is not None: self.callback(row, image)
 
   def lock(self):
     """Lock treeview."""
     self.filebutton.set_sensitive(False)
 
   def unlock(self):
```

### Comparing `eQuimage-1.3.0/src/eQuimage/windows/settings.py` & `eQuimage-1.4.0/src/eQuimage/gui/settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
+# GUI updated.
 
 """Settings window."""
 
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk
-from .gtk.customwidgets import Button, CheckButton, SpinButton
+from .gtk.customwidgets import Align, HBox, VBox, FramedHBox, HButtonBox, Button, CheckButton, SpinButton
 from .base import BaseWindow, Container
 
 class SettingsWindow(BaseWindow):
   """Settings window class."""
 
   def open(self):
     """Open tool window with title 'title' for image 'image'."""
@@ -21,54 +22,47 @@
     self.opened = True
     self.window = Gtk.Window(title = "Settings",
                              transient_for = self.app.mainwindow.window,
                              border_width = 16,
                              modal = True)
     self.window.connect("delete-event", self.close)
     self.widgets = Container()
-    wbox = Gtk.VBox(spacing = 16)
+    wbox = VBox()
     self.window.add(wbox)
-    frame = Gtk.Frame(label = " Apply operations on the fly (disable if not responsive) ")
-    frame.set_label_align(0.2, 0.5)
-    wbox.pack_start(frame, False, False, 0)
-    hbox = Gtk.HBox()
-    frame.add(hbox)
-    vbox = Gtk.VBox(homogeneous = True, margin = 8)
-    hbox.pack_start(vbox, False, False, 0)
+    frame, hbox = FramedHBox(" Apply operations on the fly (disable if not responsive) ", spacing = 16)
+    wbox.pack(frame)
+    vbox = VBox(spacing = 0, homogeneous = True)
+    hbox.pack(vbox)
     self.widgets.hotpixelsbutton = CheckButton(label = "Hot pixels")
     self.widgets.hotpixelsbutton.set_active(self.app.hotpixelsotf)
-    vbox.pack_start(self.widgets.hotpixelsbutton, False, False, 0)
+    vbox.pack(self.widgets.hotpixelsbutton)
     self.widgets.stretchbutton = CheckButton(label = "Stretch tools")
     self.widgets.stretchbutton.set_active(self.app.stretchotf)
-    vbox.pack_start(self.widgets.stretchbutton, False, False, 0)
+    vbox.pack(self.widgets.stretchbutton)
     self.widgets.colorbutton = CheckButton(label = "Color balance/saturation/noise")
     self.widgets.colorbutton.set_active(self.app.colorotf)
-    vbox.pack_start(self.widgets.colorbutton, False, False, 0)
+    vbox.pack(self.widgets.colorbutton)
     self.widgets.blendbutton = CheckButton(label = "Blend images")
     self.widgets.blendbutton.set_active(self.app.blendotf)
-    vbox.pack_start(self.widgets.blendbutton, False, False, 0)
-    vbox = Gtk.VBox(margin = 8, valign = Gtk.Align.CENTER)
-    hbox.pack_start(vbox, False, False, 0)
-    tbox = Gtk.HBox()
-    vbox.pack_start(tbox, False, False, 0)
-    tbox.pack_start(Gtk.Label(label = "Poll time: "), False, False, 0)
+    vbox.pack(self.widgets.blendbutton)
+    vbox = VBox(spacing = 0, valign = Align.CENTER)
+    hbox.pack(vbox)
     self.widgets.timespin = SpinButton(self.app.polltime, 100, 1000, 10, digits = 0)
-    tbox.pack_start(self.widgets.timespin, False, False, 0)
-    tbox.pack_start(Gtk.Label(label = " ms"), False, False, 0)
-    hbox = Gtk.HButtonBox(homogeneous = True, spacing = 16, halign = Gtk.Align.START)
-    wbox.pack_start(hbox, False, False, 0)
+    vbox.pack(self.widgets.timespin.hbox(prepend = "Poll time:", append = "ms"))
+    hbox = HButtonBox()
+    wbox.pack(hbox)
     self.widgets.applybutton = Button(label = "OK")
     self.widgets.applybutton.connect("clicked", self.apply)
-    hbox.pack_start(self.widgets.applybutton, False, False, 0)
+    hbox.pack(self.widgets.applybutton)
     self.widgets.applybutton = Button(label = "Reset")
     self.widgets.applybutton.connect("clicked", self.reset)
-    hbox.pack_start(self.widgets.applybutton, False, False, 0)
+    hbox.pack(self.widgets.applybutton)
     self.widgets.cancelbutton = Button(label = "Cancel")
     self.widgets.cancelbutton.connect("clicked", self.close)
-    hbox.pack_start(self.widgets.cancelbutton, False, False, 0)
+    hbox.pack(self.widgets.cancelbutton)
     self.window.show_all()
 
   def reset(self, *args, **kwargs):
     """Reset settings."""
     if not self.opened: return
     settings = self.app.get_default_settings()
     self.widgets.hotpixelsbutton.set_active(settings["remove_hot_pixels_on_the_fly"])
```

### Comparing `eQuimage-1.3.0/src/eQuimage/windows/statistics.py` & `eQuimage-1.4.0/src/eQuimage/gui/statistics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,73 +1,75 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
+# GUI updated.
 
 """Image statistics window."""
 
 import gi
 gi.require_version("Gtk", "3.0")
-from gi.repository import Gtk, Gdk
-from .base import BaseWindow, BaseToolbar, Container
-from .utils import histogram_bins, plot_histograms, highlight_histogram
-from matplotlib.backends.backend_gtk3agg import FigureCanvasGTK3Agg as FigureCanvas
+from gi.repository import Gtk
+from .gtk.customwidgets import HBox, VBox, HButtonBox, Button
+from .gtk.keyboard import decode_key
+from .base import BaseWindow, FigureCanvas, BaseToolbar, Container
+from .misc.utils import histogram_bins, plot_histograms, highlight_histogram
 from matplotlib.figure import Figure
 
 class StatsWindow(BaseWindow):
   """Image statistics window class."""
 
   def open(self, image):
     """Open statistics window for image 'image'."""
     if self.opened: self.close()
     self.opened = True
     self.window = Gtk.Window(title = "Image histograms & statistics", transient_for = self.app.mainwindow.window, destroy_with_parent = True, border_width = 16)
     self.window.connect("delete-event", self.close)
     self.window.connect("key-press-event", self.key_press)
     self.widgets = Container()
-    wbox = Gtk.VBox(spacing = 16)
+    wbox = VBox()
     self.window.add(wbox)
-    fbox = Gtk.VBox(spacing = 0)
-    wbox.pack_start(fbox, True, True, 0)
+    fbox = VBox(spacing = 0)
+    wbox.pack(fbox, expand = True, fill = True)
     self.widgets.fig = Figure(figsize = (10., 3.), layout = "constrained")
     canvas = FigureCanvas(self.widgets.fig)
     canvas.set_size_request(600, 180)
-    fbox.pack_start(canvas, True, True, 0)
+    fbox.pack(canvas, expand = True, fill = True)
     toolbar = BaseToolbar(canvas, self.widgets.fig)
-    fbox.pack_start(toolbar, False, False, 0)
-    wbox.pack_start(Gtk.Label("Press [L] to toggle lin/log scale", halign = Gtk.Align.START), False, False, 0)
+    fbox.pack(toolbar)
+    wbox.pack("Press [L] to toggle lin/log scale")
     stats = image.statistics()
     self.widgets.selection = self.pack_image_statistics_treeview(stats, wbox)
-    hbox = Gtk.HButtonBox(homogeneous = True, spacing = 16, halign = Gtk.Align.START)
-    wbox.pack_start(hbox, False, False, 0)
-    self.widgets.closebutton = Gtk.Button(label = "Close")
+    hbox = HButtonBox()
+    wbox.pack(hbox)
+    self.widgets.closebutton = Button(label = "Close")
     self.widgets.closebutton.connect("clicked", self.close)
-    hbox.pack_start(self.widgets.closebutton, False, False, 0)
+    hbox.pack(self.widgets.closebutton)
     self.widgets.fig.histax = self.widgets.fig.add_subplot(111)
     self.histlogscale = False
     self.histcolors = ((1., 0., 0.), (0., 1., 0.), (0., 0., 1.), (0., 0., 0.), (0.5, 0.5, 0.5))
     self.histograms = image.histograms(nbins = histogram_bins(stats["L"], self.app.get_color_depth()))
-    self.plot_image_histograms()
-    self.widgets.selection.connect("changed", lambda selection: self.highlight_image_histogram())
+    self.plot_histograms()
+    self.widgets.selection.connect("changed", lambda selection: self.highlight_histogram())
     self.window.show_all()
 
   def close(self, *args, **kwargs):
     """Close statistics window."""
     if not self.opened: return
     self.window.destroy()
     self.opened = False
     del self.widgets
     del self.histograms
 
   def pack_image_statistics_treeview(self, stats, box):
     """Pack image statistics 'stats' (see imageprocessing.Image.statistics) as a TreeView in box 'box'.
        Return a TreeView selection object to get the selected channel with self.get_selected_channel()."""
     width, height, npixels = stats["L"].width, stats["L"].height, stats["L"].npixels
-    box.pack_start(Gtk.Label(f"Image size = {width}x{height} pixels = {npixels} pixels", halign = Gtk.Align.START), False, False, 0)
+    box.pack(f"Image size = {width}x{height} pixels = {npixels} pixels")
     store = Gtk.ListStore(int, str, str, str, str, str, str, str, str, str, str)
     idx = 0
     for key in ("R", "G", "B", "V", "L"):
       channel = stats[key]
       if channel.median is None:
         perc25 = "-"
         median = "-"
@@ -76,15 +78,15 @@
         perc25 = f"{channel.percentiles[0]:.5f}"
         median = f"{channel.median:.5f}"
         perc75 = f"{channel.percentiles[2]:.5f}"
       store.append([idx, channel.name, f"{channel.minimum:.5f}", perc25, median, perc75, f"{channel.maximum:.5f}",
                     f"{channel.zerocount:d}", f"({100.*channel.zerocount/npixels:6.3f}%)", f"{channel.outcount:d}", f"({100.*channel.outcount/npixels:6.3f}%)"])
       idx += 1
     treeview = Gtk.TreeView(model = store, search_column = -1)
-    box.pack_start(treeview, False, False, 0)
+    box.pack(treeview)
     renderer = Gtk.CellRendererText()
     renderer.set_property("xalign", 0.)
     column = Gtk.TreeViewColumn("Channel", renderer, text = 1)
     column.set_alignment(0.)
     column.set_expand(True)
     treeview.append_column(column)
     renderer = Gtk.CellRendererText()
@@ -137,39 +139,37 @@
     column.pack_start(count, True)
     column.add_attribute(count, "text", 9)
     percent = Gtk.CellRendererText()
     percent.set_property("xalign", 1.)
     column.pack_start(percent, False)
     column.add_attribute(percent, "text", 10)
     treeview.append_column(column)
-    box.pack_start(Gtk.Label("The medians and percentiles (%) above exclude pixels <= 0 and >= 1", halign = Gtk.Align.START), False, False, 0)
+    box.pack("The medians and percentiles (%) above exclude pixels &lt;= 0 and &gt;= 1")
     selection = treeview.get_selection()
     selection.set_mode(Gtk.SelectionMode.SINGLE)
     return selection
 
   def get_selected_channel(self):
     """Return selected channel (-1 if None)."""
     model, list_iter = self.widgets.selection.get_selected()
     return model[list_iter][0] if list_iter is not None else -1
 
-  def plot_image_histograms(self):
-    """Plot image histograms."""
+  def plot_histograms(self):
+    """Plot histograms."""
     ax = self.widgets.fig.histax
     ax.histlines = plot_histograms(ax, *self.histograms, colors = self.histcolors, ylogscale = self.histlogscale)
     highlight_histogram(ax.histlines, self.get_selected_channel())
 
-  def highlight_image_histogram(self):
-    """Highlight image histogram line."""
+  def highlight_histogram(self):
+    """Highlight histogram line."""
     highlight_histogram(self.widgets.fig.histax.histlines, self.get_selected_channel())
     self.widgets.fig.canvas.draw_idle()
 
   def key_press(self, widget, event):
     """Callback for key press in the statistics window."""
-    ctrl = event.state & Gdk.ModifierType.CONTROL_MASK
-    alt = event.state & Gdk.ModifierType.MOD1_MASK
-    if ctrl or alt: return
-    keyname = Gdk.keyval_name(event.keyval).upper()
-    if keyname == "L": # Toggle log scale.
+    key = decode_key(event)
+    if key.ctrl or key.alt: return
+    if key.uname == "L": # Toggle log scale.
       self.histlogscale = not self.histlogscale
-      self.plot_image_histograms()
+      self.plot_histograms()
       self.widgets.fig.canvas.draw_idle()
       self.window.queue_draw()
```

### Comparing `eQuimage-1.3.0/src/eQuimage/windows/stretch.py` & `eQuimage-1.4.0/src/eQuimage/gui/tools/stretch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,72 +1,65 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
+# GUI updated.
 
 """Template for histogram stretch tools."""
 
-import gi
-gi.require_version("Gtk", "3.0")
-from gi.repository import Gtk, Gdk
-from .gtk.customwidgets import Notebook
-from .base import  BaseToolbar, Container
-from .tools import BaseToolWindow
-from .utils import histogram_bins, plot_histograms, update_histograms, highlight_histogram, stats_string
+from ..gtk.customwidgets import Label, HBox, VBox, Grid, Notebook
+from ..gtk.keyboard import decode_key
+from ..base import FigureCanvas, BaseToolbar, Container
+from ..toolmanager import BaseToolWindow
+from ..misc.utils import histogram_bins, plot_histograms, update_histograms, highlight_histogram, stats_string
 import numpy as np
-from matplotlib.backends.backend_gtk3agg import FigureCanvasGTK3Agg as FigureCanvas
 from matplotlib.figure import Figure
 import matplotlib.ticker as ticker
 
 class StretchTool(BaseToolWindow):
   """Histogram stretch tool class."""
 
   # Build window.
 
-  __window_name__ = "" # Window name.
+  _window_name_ = "" # Window name.
 
   def open(self, image):
     """Open tool window for image 'image'."""
-    if not super().open(image, self.__window_name__): return False
-    wbox = Gtk.VBox(spacing = 16)
+    if not super().open(image, self._window_name_): return False
+    wbox = VBox()
     self.window.add(wbox)
-    fbox = Gtk.VBox(spacing = 0)
-    wbox.pack_start(fbox, True, True, 0)
+    fbox = VBox(spacing = 0)
+    wbox.pack(fbox, expand = True, fill = True)
     self.widgets.fig = Figure(figsize = (10., 6.), layout = "constrained")
     canvas = FigureCanvas(self.widgets.fig)
     canvas.set_size_request(800, 480)
-    fbox.pack_start(canvas, True, True, 0)
+    fbox.pack(canvas, expand = True, fill = True)
     toolbar = BaseToolbar(canvas, self.widgets.fig)
-    fbox.pack_start(toolbar, False, False, 0)
-    wbox.pack_start(Gtk.Label("Press [L] to toggle lin/log scale, [C] to plot the contrast enhancement function log(f')", halign = Gtk.Align.START), False, False, 0)
-    grid = Gtk.Grid(column_spacing = 8)
-    wbox.pack_start(grid, True, True, 0)
-    reflabel = Gtk.Label(halign = Gtk.Align.START)
-    reflabel.set_markup("<b>Reference</b>")
-    grid.add(reflabel)
-    self.widgets.refstats = Gtk.Label(label = "", halign = Gtk.Align.START)
-    grid.attach_next_to(self.widgets.refstats, reflabel, Gtk.PositionType.RIGHT, 1, 1)
-    imglabel = Gtk.Label(halign = Gtk.Align.START)
-    imglabel.set_markup("<b>Image</b>")
-    grid.attach_next_to(imglabel, reflabel, Gtk.PositionType.BOTTOM, 1, 1)
-    self.widgets.imgstats = Gtk.Label(label = "", halign = Gtk.Align.START)
-    grid.attach_next_to(self.widgets.imgstats, imglabel, Gtk.PositionType.RIGHT, 1, 1)
+    fbox.pack(toolbar)
+    wbox.pack("Press [L] to toggle lin/log scale, [C] to plot the contrast enhancement function log(f')")
+    grid = Grid()
+    wbox.pack(grid, expand = True, fill = True)
+    self.widgets.refstats = Label()
+    grid.attach("<b>Reference</b>", 0, 0)
+    grid.attach(self.widgets.refstats, 1, 0)
+    self.widgets.imgstats = Label()
+    grid.attach("<b>Image</b>", 0, 1)
+    grid.attach(self.widgets.imgstats, 1, 1)
     options = self.options_widgets(self.widgets)
-    if options is not None: wbox.pack_start(options, False, False, 0)
+    if options is not None: wbox.pack(options)
     self.reference.stats = self.reference.statistics(channels = "RGBSVL")
     self.image.stats = self.reference.stats.copy()
     self.statchannels = ""     # Keys for the image statistics.
     self.histchannels = ""     # Keys for the image histograms.
     self.histcolors = []       # Colors of the image histograms.
     self.channelkeys = []      # Keys of the different channels/tabs.
     self.widgets.channels = {} # Widgets of the different channels/tabs.
     self.widgets.rgbtabs = Notebook()
-    self.widgets.rgbtabs.set_tab_pos(Gtk.PositionType.TOP)
-    wbox.pack_start(self.widgets.rgbtabs, False, False, 0)
+    wbox.pack(self.widgets.rgbtabs)
     for key, name, color, lcolor in (("R", "Red", (1., 0., 0.), (1., 0., 0.)),
                                      ("G", "Green", (0., 1., 0.), (0., 1., 0.)),
                                      ("B", "Blue", (0., 0., 1.), (0., 0., 1.)),
                                      ("S", "HSV saturation", (1., .5, 0.), (1., .5, 0.)),
                                      ("V", "HSV value = max(RGB)", (0., 0., 0.), (1., 1., 1.)),
                                      ("L", "Luma", (.5, .5, .5), (1., 1., 1.))):
       channel = Container()
@@ -75,17 +68,17 @@
         channel.color = np.array(color)
         channel.lcolor = np.array(lcolor)
         self.statchannels += key
         self.histchannels += key
         self.histcolors.append(channel.color)
         self.channelkeys.append(key)
         self.widgets.channels[key] = channel
-        self.widgets.rgbtabs.append_page(tab, Gtk.Label(label = name))
+        self.widgets.rgbtabs.append_page(tab, Label(name))
     self.widgets.rgbtabs.connect("switch-page", lambda tabs, tab, itab: self.update("tab", tab = itab))
-    wbox.pack_start(self.tool_control_buttons(), False, False, 0)
+    wbox.pack(self.tool_control_buttons())
     if "R" not in self.histchannels: # Always include red, blue, green...
       self.histchannels += "R"
       self.histcolors.append(np.array((1., 0., 0.)))
     if "G" not in self.histchannels: # ...in the histograms even though...
       self.histchannels += "G"
       self.histcolors.append(np.array((0., 1., 0.)))
     if "B" not in self.histchannels: # ...there are no tabs for these channels.
@@ -101,21 +94,21 @@
     if self.outofrange: print("Reference image is out-of-range...")
     self.currentparams = self.get_params()
     self.app.mainwindow.set_rgb_luma_callback(self.update_rgb_luma)
     self.start(identity = not self.outofrange) # If so, the stretch tool may clip the image whatever the parameters.
     return True
 
   def options_widgets(self, widgets):
-    """Return a Gtk box with tool options widgets and store the reference to these widgets in container 'widgets'.
+    """Return a box with tool options widgets and store the reference to these widgets in container 'widgets'.
        Return None if there are no tool options widgets.
        Must be defined (if needed) in each subclass."""
     return None
 
   def tab_widgets(self, key, widgets):
-    """Return a Gtk box with tab widgets for channel 'key' in "R" (red), "G" (green), "B" (blue), "S" (saturation), "V" (value) or "L" (luma),
+    """Return a box with tab widgets for channel 'key' in "R" (red), "G" (green), "B" (blue), "S" (saturation), "V" (value) or "L" (luma),
        and store the reference to these widgets in container 'widgets'.
        Return None if there is no tab for this channel.
        Must be defined (if needed) in each subclass."""
     return None
 
   # Tool methods.
 
@@ -257,26 +250,24 @@
   def update_widgets(self, key, changed):
     """Update widgets (other than histograms and stats) on change of 'changed' in channel 'key'.
        Must be defined (if needed) in each subclass."""
     return
 
   def key_press(self, widget, event):
     """Callback for key press in the stretch tool window."""
-    ctrl = event.state & Gdk.ModifierType.CONTROL_MASK
-    alt = event.state & Gdk.ModifierType.MOD1_MASK
-    if not ctrl and not alt:
-      keyname = Gdk.keyval_name(event.keyval).upper()
-      if keyname == "L": # Toggle log scale.
+    key = decode_key(event)
+    if not key.ctrl and not key.alt:
+      if key.uname == "L": # Toggle log scale.
         self.histlogscale = not self.histlogscale
         self.update_reference_histograms()
         self.update_image_histograms()
         self.widgets.fig.canvas.draw_idle()
         self.window.queue_draw()
         return
-      elif keyname == "C": # Toggle stretch function/contrast enhancement function.
+      elif key.uname == "C": # Toggle stretch function/contrast enhancement function.
         self.plotcontrast = not self.plotcontrast
         tab = self.widgets.rgbtabs.get_current_page()
         key = self.channelkeys[tab]
         self.update_stretch_function_axes()
         self.update_widgets(key, "sfplot")
         self.widgets.fig.canvas.draw_idle()
         self.window.queue_draw()
```

### Comparing `eQuimage-1.3.0/src/eQuimage/windows/tools.py` & `eQuimage-1.4.0/src/eQuimage/gui/toolmanager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,81 +1,88 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
+# GUI updated.
 
 """Base tool window class."""
 
 import gi
 gi.require_version("Gtk", "3.0")
-from gi.repository import Gtk, Gdk, GObject
-from .gtk.customwidgets import Button
+from gi.repository import Gtk, GObject
+from .gtk.customwidgets import HBox, VBox, HButtonBox, Button
+from .gtk.keyboard import decode_key
 from .base import BaseWindow, Container
 import threading
 from collections import OrderedDict as OD
 
 class BaseToolWindow(BaseWindow):
   """Base tool window class."""
 
-  __action__ = None # Message printed when the tool is applied.
+  _action_ = None # Message printed when the tool is applied.
 
-  __onthefly__ = True # True if the transformations can be applied on the fly.
+  _onthefly_ = True # True if the transformations can be applied on the fly.
+
+  _referencetab_ = True # Show the reference image tab.
 
   def __init__(self, app, polltime = -1):
     """Bind window with application 'app'.
        If polltime > 0, run the tool on the fly by polling for
        tool parameters change every 'polltime' ms.
        If polltime <= 0, run the tool on demand when the
        user clicks the "Apply" button."""
     super().__init__(app)
-    self.polltime = polltime if self.__onthefly__ else -1
+    self.polltime = polltime if self._onthefly_ else -1
     self.onthefly = (self.polltime > 0)
 
   def open(self, image, title):
     """Open tool window with title 'title' for image 'image'.
        Return True if successful, False otherwise."""
     if self.opened: return False
-    if self.__action__ is not None: print(self.__action__)
+    if self._action_ is not None: print(self._action_)
     self.opened = True
     self.image = image.clone()
     self.image.meta["params"] = None
     self.image.meta["description"] = "[No transformations]"
     self.image.stats = None # Image statistics.
     self.reference = image.ref()
     self.reference.meta["description"] = "Reference image"
     self.reference.stats = None # Reference image statistics.
-    self.app.mainwindow.set_images(OD(Image = self.image, Reference = self.reference), reference = "Reference")
-    self.app.mainwindow.set_copy_paste_callbacks(self.copy, self.paste)
     self.window = Gtk.Window(title = title, border_width = 16)
     self.window.connect("delete-event", self.quit)
     self.window.connect("key-press-event", self.key_press)
     self.widgets = Container()
+    if self._referencetab_:
+      self.app.mainwindow.set_images(OD(Image = self.image, Reference = self.reference), reference = "Reference")
+    else:
+      self.app.mainwindow.set_images(OD(Image = self.image))
+    self.app.mainwindow.set_copy_paste_callbacks(self.copy, self.paste)
     self.polltimer = None # Polling/update threads data.
     self.lock = threading.Lock()
     self.thread = threading.Thread(target = None)
     self.toolparams = None # Tool parameters of the last transformation.
     self.transformed = False # True if the image has been transformed.
     self.defaultparams = None # Default tool parameters.
-    self.defaultparams_identity = True # True if default tool parameters are the identity operation.
+    self.defaultparams_are_identity = True # True if default tool parameters are the identity operation.
     self.frame = None # New frame if modified by the tool.
     return True
 
   # Start tool.
 
   def start(self, identity = True):
     """Start tool.
-       Set the present tool parameters (drawn from self.get_params()) as default parameters, show the tool window and start polling
-       for tool parameters change.
+       Set the present tool parameters (drawn from self.get_params()) as default parameters, update the
+       main window tabs, show the tool window and start polling for tool parameters change.
        If 'identity' is True, the default parameters are the identity operation (no image transformation)."""
     self.defaultparams = self.get_params()
     self.toolparams = self.get_params()
-    self.defaultparams_identity = identity
-    if not identity:
-      if self.onthefly: self.apply(cancellable = False)
+    self.defaultparams_are_identity = identity
+
+    if self.onthefly and not identity: self.apply(cancellable = False)
     self.window.show_all()
     self.start_polling()
 
   # Finalize tool.
 
   def finalize(self, image, operation, frame = None):
     """Finalize tool.
@@ -87,15 +94,15 @@
     self.opened = False
     if image is not None:
       image.meta.pop("params", None) # Clean-up the image meta-data.
       self.app.finalize_tool(image, operation, frame)
     del self.widgets
     del self.image
     del self.reference
-    self.cleanup()
+    self.cleanup() # Additional cleanup.
 
   def destroy(self):
     """Destroy tool (without returning any image and operation to the application)."""
     if not self.opened: return
     self.stop_polling() # Stop polling.
     if self.thread.is_alive(): self.thread.join() # Wait for the current thread to finish.
     self.finalize(None, None)
@@ -112,63 +119,63 @@
     if not self.opened: return
     polling = self.stop_polling() # Stop polling.
     if self.thread.is_alive(): self.thread.join() # Wait for the current thread to finish.
     if polling:
       params = self.get_params()
       if params != self.toolparams: # Make sure that the last changes have been applied.
         self.start_run_thread(params)
-        if self.thread.is_alive(): self.thread.join()
+        if self.thread.is_alive(): self.thread.join() # Shall be alive, actually.
     self.finalize(self.image, self.image.meta["description"] if self.transformed else None, self.frame)
 
   def cleanup(self):
     """Free memory on exit.
        Must be defined (if needed) in each subclass."""
     return
 
   # Tool control buttons.
 
   def tool_control_buttons(self, model = None, reset = True):
-    """Return a Gtk HButtonBox with tool control buttons.
+    """Return a HButtonBox with tool control buttons.
        If None, 'model' is set to "ondemand" if self.onthefly is False, and to "onthefly" if self.onthefly is True.
        If 'model' is "ondemand", the transformations are applied on demand and the control buttons are
          Apply, Cancel, Reset and Close
        connected to the self.apply, self.cancel, self.reset and self.close methods.
        If 'model' is "onthefly", the transformations are applied on the fly and the control buttons are
          OK, Reset, and Cancel
        connected to the self.close, self.cancel and self.quit methods.
        The Reset button is not displayed if 'reset' is False."""
     if model is None:
       model = "onthefly" if self.onthefly else "ondemand"
-    hbox = Gtk.HButtonBox(homogeneous = True, spacing = 16, halign = Gtk.Align.START)
+    hbox = HButtonBox()
     if model == "ondemand":
       self.widgets.applybutton = Button(label = "Apply") # Apply transformation on demand.
       self.widgets.applybutton.connect("clicked", self.apply)
-      hbox.pack_start(self.widgets.applybutton, False, False, 0)
-      self.widgets.cancelbutton = Button(label = "Cancel") # Cancel all transformations (restore the reference image).
+      hbox.pack(self.widgets.applybutton)
+      self.widgets.cancelbutton = Button(label = "Cancel") # Cancel transformation (restore the reference image).
       self.widgets.cancelbutton.connect("clicked", self.cancel)
       self.widgets.cancelbutton.set_sensitive(False)
-      hbox.pack_start(self.widgets.cancelbutton, False, False, 0)
-      self.widgets.resetbutton = Button(label = "Reset") # Cancel last transformation.
+      hbox.pack(self.widgets.cancelbutton)
+      self.widgets.resetbutton = Button(label = "Reset") # Reset parameters to the last applied transformation.
       self.widgets.resetbutton.connect("clicked", self.reset)
-      if reset: hbox.pack_start(self.widgets.resetbutton, False, False, 0)
+      if reset: hbox.pack(self.widgets.resetbutton)
       self.widgets.closebutton = Button(label = "Close") # Close tool and return the transformed image to the application.
       self.widgets.closebutton.connect("clicked", self.close)
-      hbox.pack_start(self.widgets.closebutton, False, False, 0)
+      hbox.pack(self.widgets.closebutton)
     elif model == "onthefly":
       self.widgets.applybutton = None
       self.widgets.closebutton = Button(label = "OK") # Close tool and return the transformed image to the application.
       self.widgets.closebutton.connect("clicked", self.close)
-      hbox.pack_start(self.widgets.closebutton, False, False, 0)
-      self.widgets.cancelbutton = Button(label = "Reset") # Cancel all transformations (restore the reference image).
+      hbox.pack(self.widgets.closebutton)
+      self.widgets.cancelbutton = Button(label = "Reset") # Cancel transformation (restore the reference image).
       self.widgets.cancelbutton.connect("clicked", self.cancel)
       self.widgets.cancelbutton.set_sensitive(False)
-      if reset: hbox.pack_start(self.widgets.cancelbutton, False, False, 0)
-      self.widgets.quitbutton = Button(label = "Cancel") # Cancel all transformations and close tool (return the reference image to the application).
+      if reset: hbox.pack(self.widgets.cancelbutton)
+      self.widgets.quitbutton = Button(label = "Cancel") # Cancel transformation and close tool (return the reference image to the application).
       self.widgets.quitbutton.connect("clicked", self.quit)
-      hbox.pack_start(self.widgets.quitbutton, False, False, 0)
+      hbox.pack(self.widgets.quitbutton)
     else:
       raise ValueError("Model must be 'onthefly' or 'ondemand'.")
     return hbox
 
   # Apply tool.
 
   def get_params(self):
@@ -180,28 +187,44 @@
     """Set tool parameters 'params'.
        Must be defined in each subclass."""
     return
 
   def run(self, params):
     """Run tool for parameters 'params'.
        Return (toolparams, transformed), where toolparams are the tool parameters
-       actually applied (that might differ from params if the latter are, e.g., out
+       actually applied (that may differ from params if the latter are, e.g., out
        of range), and transformed is True if self.image has indeed been transformed
        (with respect to self.reference), False otherwise.
        Must be defined in each subclass."""
     print("Doing nothing !...")
     return None, False
 
   def operation(self, params):
     """Return tool operation string for parameters 'params'.
        Must be defined in each subclass."""
     return None
 
   #
 
+  def queue_gui_mainloop(self, function, *args):
+    """Enqueue a thread-safe call to 'function(*args)' in the GUI mainloop.
+       This is a wrapper to GObject.idle_add(function, *args, priority = GObject.PRIORITY_DEFAULT)."""
+    GObject.idle_add(function, *args, priority = GObject.PRIORITY_DEFAULT)
+
+  def update_gui(self):
+    """Update main and tool windows after tool run."""
+    if not self.opened: return
+    self.app.mainwindow.update_image("Image", self.image)
+    self.app.mainwindow.update_key_label("Image", "Image (*)" if self.transformed else "Image")
+    if not self.thread.is_alive():
+      self.app.mainwindow.set_idle()
+      self.app.mainwindow.unlock_rgb_luma()
+      if self.widgets.applybutton is not None: self.widgets.applybutton.set_sensitive(True)
+    return False
+
   def start_run_thread(self, params):
     """Run tool for params 'params' and update main and tool windows in a separate thread to keep the GUI responsive."""
     if self.thread.is_alive(): self.thread.join() # Wait for the current thread to finish.
     self.app.mainwindow.lock_rgb_luma()
     self.app.mainwindow.set_busy()
     self.thread = threading.Thread(target = self.run_thread, args = (params,), daemon = False)
     self.thread.start()
@@ -210,37 +233,27 @@
     """Run tool for params 'params' and update main and tool windows."""
     with self.lock: # Make sure no other thread is running concurrently.
       toolparams, self.transformed = self.run(params) # Must be defined in each subclass.
       if not self.transformed: self.image.copy_image_from(self.reference)
       self.image.meta["params"] = toolparams
       self.image.meta["description"] = self.operation(toolparams)
       self.toolparams = params
-      GObject.idle_add(self.update_gui, priority = GObject.PRIORITY_DEFAULT) # Thread-safe.
-
-  def update_gui(self):
-    """Update main and tool windows."""
-    if not self.opened: return
-    self.app.mainwindow.update_image("Image", self.image)
-    if not self.thread.is_alive():
-      self.app.mainwindow.set_idle()
-      self.app.mainwindow.unlock_rgb_luma()
-      if self.widgets.applybutton is not None: self.widgets.applybutton.set_sensitive(True)
-    return False
+      self.queue_gui_mainloop(self.update_gui) # Thread-safe.
 
   def apply(self, *args, **kwargs):
     """Get tool parameters, run tool and update main and tool windows.
        If the keyword argument 'cancellable' is False (default True), this run can not be cancelled,
        so that the "Cancel" button is made insensitive."""
     params = self.get_params()
     if params is None: return # Do nothing is params is None.
     if self.widgets.applybutton is not None: self.widgets.applybutton.set_sensitive(False)
     self.start_run_thread(params)
-    cancellable = kwargs["cancellable"] if "cancellable" in kwargs.keys() else True
+    cancellable = kwargs.get("cancellable", True)
     self.widgets.cancelbutton.set_sensitive(cancellable)
-    self.app.mainwindow.set_current_tab(0)
+    #self.app.mainwindow.set_current_tab(0)
 
   def apply_idle(self):
     """Get tool parameters, run tool and update main and tool windows if no other thread is already running.
        Return True if new thread successfully started, False otherwise."""
     if self.thread.is_alive(): return False
     params = self.get_params()
     if params is None: return False # Do nothing is params is None.
@@ -255,15 +268,15 @@
     self.set_params(self.toolparams)
 
   def cancel(self, *args, **kwargs):
     """Cancel tool."""
     self.stop_polling() # Stop polling while restoring reference image.
     if self.thread.is_alive(): self.thread.join() # Wait for the current thread to finish.
     self.set_params(self.defaultparams)
-    if self.onthefly and not self.defaultparams_identity:
+    if self.onthefly and not self.defaultparams_are_identity:
       self.apply(cancellable = False)
     else:
       self.image.copy_image_from(self.reference)
       self.image.meta["params"] = None
       self.image.meta["description"] = "[No transformations]"
       self.toolparams = self.get_params()
       self.transformed = False
@@ -275,15 +288,15 @@
 
   def start_polling(self, lastparams = None):
     """Start polling for tool parameter changes every self.polltime ms.
        At each poll, get the tool parameters from self.get_params(); then
        call self.apply_idle() if the tool parameters are the same *twice* in a row,
        but are different from the self.toolparams registered at the last update.
        'lastparams' is the assumptive outcome of the last poll (defaults to self.toolparams if None);
-       set to self.get_params() to attempt calling self.apply_idle() as soon as the first poll.
+       set to self.get_params() to expedite call to self.apply_idle() as soon as the first poll.
        Return true if successfully polling, False otherwise (self.polltime < 0)."""
     if self.polltime <= 0: return False # No poll time defined.
     self.pollparams = self.toolparams if lastparams is None else lastparams
     self.polltimer = GObject.timeout_add(self.polltime, self.poll)
     return True
 
   def poll(self, *args, **kwargs):
@@ -322,19 +335,16 @@
        order to request tool update on next poll. This enhances responsivity to tool parameters changes."""
     widget.connect(signames, lambda *args: self.reset_polling(self.get_params()))
 
   # Manage key press/release events.
 
   def key_press(self, widget, event):
     """Callback for key press in the tool window."""
-    ctrl = event.state & Gdk.ModifierType.CONTROL_MASK
-    alt = event.state & Gdk.ModifierType.MOD1_MASK
-    if ctrl and not alt:
-      keyname = Gdk.keyval_name(event.keyval).upper()
-      if keyname == "TAB":
+    key = decode_key(event)
+    if key.ctrl and not key.alt and key.uname == "TAB":
         self.app.mainwindow.set_current_tab(0)
         self.app.mainwindow.window.present()
 
   # Ctrl-C/Ctrl-V callbacks.
 
   def copy(self, key, image):
     """Copy image 'image' with key 'key' in a new tab."""
```

### Comparing `eQuimage-1.3.0/src/eQuimage/windows/unsharp.py` & `eQuimage-1.4.0/src/eQuimage/gui/tools/unsharp.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,52 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
+# GUI updated.
 
 """Unsharp mask tool."""
 
-import gi
-gi.require_version("Gtk", "3.0")
-from gi.repository import Gtk, Gdk
-from .gtk.customwidgets import RadioButton, HScaleSpinButton
-from .tools import BaseToolWindow
-from ..imageprocessing import imageprocessing
+from ..gtk.customwidgets import HBox, VBox, RadioButtons, HScaleSpinButton
+from ..toolmanager import BaseToolWindow
+from ...imageprocessing import imageprocessing
 from skimage.filters import unsharp_mask
-import numpy as np
 
 class UnsharpMaskTool(BaseToolWindow):
   """Unsharp mask tool class."""
 
-  __action__ = "Unsharp masking..."
+  _action_ = "Unsharp masking..."
 
-  __onthefly__ = False # This transformation can not be applied on the fly.
+  _onthefly_ = False # This transformation can not be applied on the fly.
 
   def open(self, image):
     """Open tool window for image 'image'."""
     if not super().open(image, "Unsharp mask"): return False
-    wbox = Gtk.VBox(spacing = 16)
+    wbox = VBox()
     self.window.add(wbox)
-    hbox = Gtk.HBox(spacing = 8)
-    wbox.pack_start(hbox, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = "Channel(s):"), False, False, 0)
-    self.widgets.rgbbutton = RadioButton.new_with_label_from_widget(None, "RGB")
-    hbox.pack_start(self.widgets.rgbbutton, False, False, 0)
-    self.widgets.valuebutton = RadioButton.new_with_label_from_widget(self.widgets.rgbbutton, "HSV value")
-    hbox.pack_start(self.widgets.valuebutton, False, False, 0)
-    self.widgets.lumabutton = RadioButton.new_with_label_from_widget(self.widgets.rgbbutton, "Luma")
-    hbox.pack_start(self.widgets.lumabutton, False, False, 0)
-    self.widgets.radiusscale = HScaleSpinButton(5., 0., 20., .01, digits = 2, length = 320, expand = False)
-    wbox.pack_start(self.widgets.radiusscale.layout2("Radius (pixels):"), False, False, 0)
+    self.widgets.channelbuttons = RadioButtons(("RGB", "RGB"), ("V", "HSV value"), ("L", "Luma"))
+    wbox.pack(self.widgets.channelbuttons.hbox(prepend = "Channel(s):"))
+    self.widgets.radiusscale = HScaleSpinButton(5., 0., 25., .01, digits = 2, length = 320, expand = False)
+    wbox.pack(self.widgets.radiusscale.layout2("Radius (pixels):"))
     self.widgets.amountscale = HScaleSpinButton(1., 0., 10., .01, digits = 2, length = 320, expand = False)
-    wbox.pack_start(self.widgets.amountscale.layout2("Amount:"), False, False, 0)
-    wbox.pack_start(self.tool_control_buttons(), False, False, 0)
+    wbox.pack(self.widgets.amountscale.layout2("Amount:"))
+    wbox.pack(self.tool_control_buttons())
     self.start(identity = False)
     return True
 
   def get_params(self):
     """Return tool parameters."""
-    if self.widgets.rgbbutton.get_active():
-      channels = "RGB"
-    elif self.widgets.valuebutton.get_active():
-      channels = "V"
-    else:
-      channels = "L"
-    return channels, self.widgets.radiusscale.get_value(), self.widgets.amountscale.get_value(), imageprocessing.get_rgb_luma()
+    return self.widgets.channelbuttons.get_selected(), self.widgets.radiusscale.get_value(), \
+           self.widgets.amountscale.get_value(), imageprocessing.get_rgb_luma()
 
   def set_params(self, params):
     """Set tool parameters 'params'."""
     channels, radius, amount, rgbluma = params
-    if channels == "RGB":
-      self.widgets.rgbbutton.set_active(True)
-    elif channels == "V":
-      self.widgets.valuebutton.get_active(True)
-    else:
-      self.widgets.lumabutton.set_active(True)
+    self.widgets.channelbuttons.get_selected(channels)
     self.widgets.radiusscale.set_value(radius)
     self.widgets.amountscale.set_value(amount)
 
   def run(self, params):
     """Run tool for parameters 'params'."""
     channels, radius, amount, rgbluma = params
     if amount <= 0. or radius <= 0.: return params, False
```

### Comparing `eQuimage-1.3.0/src/eQuimage/windows/utils.py` & `eQuimage-1.4.0/src/eQuimage/gui/misc/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
+# GUI updated.
 
 """Tool utils."""
 
 import numpy as np
 import matplotlib as mpl
 import matplotlib.colors as colors
 import matplotlib.ticker as ticker
```

### Comparing `eQuimage-1.3.0/src/eQuimage/windows/wavelets.py` & `eQuimage-1.4.0/src/eQuimage/gui/tools/wavelets.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,101 +1,111 @@
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 # Author: Yann-Michel Niquet (contact@ymniquet.fr).
-# Version: 1.3.0 / 2024.02.17
+# Version: 1.4.0 / 2024.03.30
+# GUI updated.
 
 """Wavelets filter tool."""
 
-import gi
-gi.require_version("Gtk", "3.0")
-from gi.repository import Gtk, Gdk
-from .gtk.customwidgets import CheckButton, SpinButton, Entry
-from .tools import BaseToolWindow
+from ..gtk.customwidgets import Align, HBox, VBox, CheckButton, RadioButtons, SpinButton, ComboBoxText, Entry
+from ..toolmanager import BaseToolWindow
 from skimage.restoration import estimate_sigma, denoise_wavelet, cycle_spin
 
 class WaveletsFilterTool(BaseToolWindow):
   """Wavelets filter tool class."""
 
-  __action__ = "Filtering wavelets..."
+  _action_ = "Applying wavelets filter..."
 
-  __onthefly__ = False # This transformation can not be applied on the fly.
+  _onthefly_ = False # This transformation can not be applied on the fly.
 
   def open(self, image):
     """Open tool window for image 'image'."""
     if not super().open(image, "Wavelets filter"): return False
-    self.update_css()
     sigma = estimate_sigma(self.reference.rgb, channel_axis = 0, average_sigmas = False)
-    wbox = Gtk.VBox(spacing = 16)
+    wbox = VBox()
     self.window.add(wbox)
-    hbox = Gtk.HBox(spacing = 8)
-    wbox.pack_start(hbox, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = "Estimated noise level in each channel:", halign = Gtk.Align.START), False, False, 0)
-    self.widgets.bindbutton = CheckButton(label = "Bind RGB channels", halign = Gtk.Align.END)
+    hbox = HBox()
+    wbox.pack(hbox)
+    hbox.pack("Estimated noise level in each channel:")
+    self.widgets.bindbutton = CheckButton(label = "Bind RGB channels", halign = Align.END)
     self.widgets.bindbutton.connect("toggled", lambda button: self.update(0))
-    hbox.pack_start(self.widgets.bindbutton, True, True, 0)
-    hbox = Gtk.HBox(spacing = 8)
-    wbox.pack_start(hbox, False, False, 0)
+    hbox.pack(self.widgets.bindbutton, expand = True, fill = True)
+    hbox = HBox()
+    wbox.pack(hbox)
     self.widgets.entries = []
     for channel, label in ((0, "Red:"), (1, 8*" "+"Green:"), (2, 8*" "+"Blue:")):
       entry = Entry(text = f"{sigma[channel]:.5e}", width = 12)
       entry.channel = channel
       entry.connect("changed", lambda entry: self.update(entry.channel))
       self.widgets.entries.append(entry)
-      hbox.pack_start(Gtk.Label(label = label), False, False, 0)
-      hbox.pack_start(entry, False, False, 0)
-    hbox = Gtk.HBox(spacing = 8)
-    wbox.pack_start(hbox, False, False, 0)
-    hbox.pack_start(Gtk.Label(label = "Maximum shift for cycle spinning:"), False, False, 0)
+      hbox.pack(label)
+      hbox.pack(entry)
+    self.widgets.ycbcrbutton = CheckButton(label = "Apply transformation in the YCbCr color space")
+    self.widgets.ycbcrbutton.set_active(True)
+    wbox.pack(self.widgets.ycbcrbutton)
+    wavelets = [] # Set-up the list of wavelets.
+    for i in range(8):
+      wavelets.append((f"db{i+1}", f"Daubechies {i+1}"))
+    for i in range(7):
+      wavelets.append((f"sym{i+2}", f"Symlets {i+2}"))
+    for i in range(8):
+      wavelets.append((f"coif{i+1}", f"Coiflets {i+1}"))
+    self.widgets.waveletcombo = ComboBoxText(*wavelets)
+    self.widgets.waveletcombo.set_selected("coif4")
+    wbox.pack(self.widgets.waveletcombo.hbox(prepend = "Wavelets:"))
+    hbox = HBox()
+    wbox.pack(hbox)
+    self.widgets.methodbuttons = RadioButtons(("BayesShrink", "Bayes Shrink"), ("VisuShrink", "Visu Shrink"))
+    hbox.pack(self.widgets.methodbuttons.hbox(prepend = "Method:"))
+    self.widgets.modebuttons = RadioButtons(("Soft", "Soft"), ("Hard", "Hard"))
+    hbox.pack(self.widgets.modebuttons.hbox(prepend = "        Mode:"))
     self.widgets.shiftsbutton = SpinButton(0., 0., 8., 1., page = 1., digits = 0)
-    hbox.pack_start(self.widgets.shiftsbutton, False, False, 0)
-    wbox.pack_start(self.tool_control_buttons(), False, False, 0)
+    wbox.pack(self.widgets.shiftsbutton.hbox(prepend = "Maximum shift for cycle spinning:"))
+    wbox.pack(self.tool_control_buttons())
     self.start(identity = False)
     return True
 
   def get_params(self):
     """Return tool parameters."""
     try:
       sigma = tuple(float(self.widgets.entries[channel].get_text()) for channel in range(3))
     except:
       return None
-    return sigma, int(self.widgets.shiftsbutton.get_value())
+    return sigma, self.widgets.ycbcrbutton.get_active(), self.widgets.waveletcombo.get_selected(), self.widgets.methodbuttons.get_selected(), \
+           self.widgets.modebuttons.get_selected(), int(self.widgets.shiftsbutton.get_value())
 
   def set_params(self, params):
     """Set tool parameters 'params'."""
-    sigma, shifts = params
+    sigma, ycbcr, wavelet, method, mode, shifts = params
     for channel in range(3):
       self.widgets.entries[channel].set_name("")
       self.widgets.entries[channel].set_text_block(f"{sigma[channel]:.5e}")
     if sigma[1] != sigma[0] or sigma[2] != sigma[0]: self.widgets.bindbutton.set_active_block(False)
+    self.widgets.ycbcrbutton.set_active(ycbcr)
+    self.widgets.waveletcombo.set_selected(wavelet)
+    self.widgets.methodbuttons.set_selected(method)
+    self.widgets.modebuttons.set_selected(mode)
     self.widgets.shiftsbutton.set_value(shifts)
 
   def run(self, params):
     """Run tool for parameters 'params'."""
-    sigma, shifts = params
-    kwargs = dict(channel_axis = -1, sigma = sigma, wavelet = "db1", mode = "soft", wavelet_levels = None,
-                  convert2ycbcr = True, method = "BayesShrink", rescale_sigma = True)
+    sigma, ycbcr, wavelet, method, mode, shifts = params
+    kwargs = dict(channel_axis = -1, sigma = sigma, wavelet = wavelet, mode = mode.lower(), wavelet_levels = None,
+                  convert2ycbcr = ycbcr, method = method, rescale_sigma = True)
     self.image.rgb = cycle_spin(self.reference.rgb, channel_axis = 0, max_shifts = shifts, func = denoise_wavelet, func_kw = kwargs, num_workers = None)
     return params, True
 
   def operation(self, params):
     """Return tool operation string for parameters 'params'."""
-    sigma, shifts = params
-    return f"WaveletsFilter(R = {sigma[0]:.5e}, G = {sigma[1]:.5e}, B = {sigma[2]:.5e}, shifts = {shifts})"
-
- # Update CSS.
-
-  def update_css(self):
-    """Update CSS for Gtk.Entry."""
-    screen = Gdk.Screen.get_default()
-    provider = Gtk.CssProvider()
-    stylecontext = Gtk.StyleContext()
-    stylecontext.add_provider_for_screen(screen, provider, Gtk.STYLE_PROVIDER_PRIORITY_APPLICATION)
-    css = b"""#red-entry {color: red}"""
-    provider.load_from_data(css)
+    sigma, ycbcr, wavelet, method, mode, shifts = params
+    operation = f"WaveletsFilter(R = {sigma[0]:.5e}, G = {sigma[1]:.5e}, B = {sigma[2]:.5e}, "
+    if ycbcr: operation += " YCbCr,"
+    operation += f" wavelets = {wavelet}, method = {method}, mode = {mode}, shifts = {shifts})"
+    return operation
 
  # Update widgets.
 
   def update(self, changed):
     """Update widgets on change of 'changed'."""
     text = self.widgets.entries[changed].get_text()
     try:
```

### Comparing `eQuimage-1.3.0/src/eQuimage.egg-info/PKG-INFO` & `eQuimage-1.4.0/src/eQuimage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eQuimage
-Version: 1.3.0
+Version: 1.4.0
 Summary: eQuimage is a tool to postprocess astronomical images from Unistellar telescopes.
 Author-email: Yann-Michel Niquet <contact@ymniquet.fr>
 Project-URL: homepage, https://astro.ymniquet.fr/
 Project-URL: repository, https://github.com/ymniquet/eQuimage
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -26,15 +26,15 @@
 
 ### eQuimage is a python tool to postprocess astronomical images from Unistellar telescopes
 
 Author: Yann-Michel Niquet (https://astro.ymniquet.fr)
 
 ### Installation
 
-eQuimage is developed in Python 3 with a GTK3 graphical interface. Python 3 and the GTK3 library are available in all Linux distributions; On Windows, follow https://www.gtk.org/docs/installations/windows/ for GTK3. To install the latest version of eQuimage, open a linux terminal/windows command prompt and run:
+eQuimage is developed in Python 3 with a GTK3 graphical user interface. Python 3 and the GTK3 library are available in all Linux distributions; on Windows, follow https://www.gtk.org/docs/installations/windows/ for GTK3. To install the latest version of eQuimage, open a linux terminal/windows command prompt and run:
 
   `pip install --user eQuimage`
 
 pip will automatically download eQuimage and the missing python modules if necessary (matplotlib, etc...). You can then launch eQuimage by typing:
 
   `eQuimage`
 
@@ -49,8 +49,7 @@
   - keep track (in a log file) of all operations applied to a given image.
 
 There is no documentation yet, but you should find your way around easily if you have used image processing software before. The python code itself is documented in English.
 
 ### Known bugs
 
   - On windows, the imageio/freeimage plugin can not read png's with accents (and likely other special characters) in the file name.
-
```

### Comparing `eQuimage-1.3.0/src/eQuimage.egg-info/SOURCES.txt` & `eQuimage-1.4.0/src/eQuimage.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,62 @@
 LICENSE
 README.md
 pyproject.toml
 src/eQuimage/__init__.py
-src/eQuimage/eQuimage.mplstyle
 src/eQuimage/eQuimage.py
 src/eQuimage.egg-info/PKG-INFO
 src/eQuimage.egg-info/SOURCES.txt
 src/eQuimage.egg-info/dependency_links.txt
 src/eQuimage.egg-info/entry_points.txt
 src/eQuimage.egg-info/requires.txt
 src/eQuimage.egg-info/top_level.txt
+src/eQuimage/config/eQuimage.css
+src/eQuimage/config/eQuimage.mplstyle
+src/eQuimage/gui/base.py
+src/eQuimage/gui/logs.py
+src/eQuimage/gui/luma.py
+src/eQuimage/gui/mainmenu.py
+src/eQuimage/gui/mainwindow.py
+src/eQuimage/gui/settings.py
+src/eQuimage/gui/statistics.py
+src/eQuimage/gui/toolmanager.py
+src/eQuimage/gui/gtk/customwidgets.py
+src/eQuimage/gui/gtk/filechoosers.py
+src/eQuimage/gui/gtk/keyboard.py
+src/eQuimage/gui/gtk/signals.py
+src/eQuimage/gui/gtk/utils.py
+src/eQuimage/gui/misc/imagechooser.py
+src/eQuimage/gui/misc/utils.py
+src/eQuimage/gui/tools/addframe.py
+src/eQuimage/gui/tools/arcsinh.py
+src/eQuimage/gui/tools/bilateral.py
+src/eQuimage/gui/tools/blackpoint.py
+src/eQuimage/gui/tools/blend.py
+src/eQuimage/gui/tools/butterworth.py
+src/eQuimage/gui/tools/clahe.py
+src/eQuimage/gui/tools/colorbalance.py
+src/eQuimage/gui/tools/colornoise.py
+src/eQuimage/gui/tools/colorsaturation.py
+src/eQuimage/gui/tools/gaussian.py
+src/eQuimage/gui/tools/ghscolorsat.py
+src/eQuimage/gui/tools/grayscale.py
+src/eQuimage/gui/tools/hotpixels.py
+src/eQuimage/gui/tools/hyperbolic.py
+src/eQuimage/gui/tools/midtone.py
+src/eQuimage/gui/tools/nlmeans.py
+src/eQuimage/gui/tools/pixelmath.py
+src/eQuimage/gui/tools/stretch.py
+src/eQuimage/gui/tools/switch.py
+src/eQuimage/gui/tools/thresholdmask.py
+src/eQuimage/gui/tools/totalvariation.py
+src/eQuimage/gui/tools/unsharp.py
+src/eQuimage/gui/tools/wavelets.py
 src/eQuimage/icons/icon.ico
 src/eQuimage/icons/icon.png
 src/eQuimage/imageprocessing/Unistellar.py
+src/eQuimage/imageprocessing/colors.py
+src/eQuimage/imageprocessing/defs.py
 src/eQuimage/imageprocessing/imageprocessing.py
+src/eQuimage/imageprocessing/pixelmath.py
 src/eQuimage/imageprocessing/stretchfunctions.py
 src/eQuimage/imageprocessing/utils.py
-src/eQuimage/images/splash.png
-src/eQuimage/windows/addframe.py
-src/eQuimage/windows/arcsinh.py
-src/eQuimage/windows/base.py
-src/eQuimage/windows/bilateral.py
-src/eQuimage/windows/blackpoint.py
-src/eQuimage/windows/blend.py
-src/eQuimage/windows/clahe.py
-src/eQuimage/windows/colorbalance.py
-src/eQuimage/windows/colornoise.py
-src/eQuimage/windows/colorsaturation.py
-src/eQuimage/windows/ghscolorsat.py
-src/eQuimage/windows/hotpixels.py
-src/eQuimage/windows/hyperbolic.py
-src/eQuimage/windows/logs.py
-src/eQuimage/windows/luma.py
-src/eQuimage/windows/mainmenu.py
-src/eQuimage/windows/mainwindow.py
-src/eQuimage/windows/midtone.py
-src/eQuimage/windows/picker.py
-src/eQuimage/windows/settings.py
-src/eQuimage/windows/statistics.py
-src/eQuimage/windows/stretch.py
-src/eQuimage/windows/tools.py
-src/eQuimage/windows/totalvariation.py
-src/eQuimage/windows/unsharp.py
-src/eQuimage/windows/utils.py
-src/eQuimage/windows/wavelets.py
-src/eQuimage/windows/gtk/customwidgets.py
-src/eQuimage/windows/gtk/filechoosers.py
-src/eQuimage/windows/gtk/signals.py
-src/eQuimage/windows/gtk/utils.py
+src/eQuimage/images/splash.png
```

