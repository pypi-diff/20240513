# Comparing `tmp/pycwr-0.3.6.tar.gz` & `tmp/pycwr-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycwr-0.3.6.tar", last modified: Wed Mar  1 12:33:11 2023, max compression
+gzip compressed data, was "pycwr-0.4.0.tar", last modified: Mon May 13 09:02:17 2024, max compression
```

## Comparing `pycwr-0.3.6.tar` & `pycwr-0.4.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 zhengyu    (501) staff       (20)        0 2023-03-01 12:33:11.658961 pycwr-0.3.6/
--rw-r--r--   0 zhengyu    (501) staff       (20)     1088 2023-03-01 09:05:21.000000 pycwr-0.3.6/LICENSE.txt
--rw-r--r--   0 zhengyu    (501) staff       (20)      125 2023-03-01 09:05:21.000000 pycwr-0.3.6/MANIFEST.in
--rw-r--r--   0 zhengyu    (501) staff       (20)      868 2023-03-01 12:33:11.658784 pycwr-0.3.6/PKG-INFO
--rw-r--r--   0 zhengyu    (501) staff       (20)     3917 2023-03-01 09:05:21.000000 pycwr-0.3.6/README.md
-drwxr-xr-x   0 zhengyu    (501) staff       (20)        0 2023-03-01 12:33:11.643175 pycwr-0.3.6/pycwr/
-drwxr-xr-x   0 zhengyu    (501) staff       (20)        0 2023-03-01 12:33:11.645877 pycwr-0.3.6/pycwr/GraphicalInterface/
--rw-r--r--   0 zhengyu    (501) staff       (20)    23249 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/GraphicalInterface/RadarInterface.py
--rw-r--r--   0 zhengyu    (501) staff       (20)    39034 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/GraphicalInterface/RadarUI.py
--rw-r--r--   0 zhengyu    (501) staff       (20)      125 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/GraphicalInterface/__init__.py
--rw-r--r--   0 zhengyu    (501) staff       (20)   301517 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/GraphicalInterface/icons.py
--rw-r--r--   0 zhengyu    (501) staff       (20)     9124 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/GraphicalInterface/station_info.py
--rw-r--r--   0 zhengyu    (501) staff       (20)      137 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/__init__.py
-drwxr-xr-x   0 zhengyu    (501) staff       (20)        0 2023-03-01 12:33:11.647280 pycwr-0.3.6/pycwr/configure/
--rw-r--r--   0 zhengyu    (501) staff       (20)      205 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/configure/__init__.py
--rw-r--r--   0 zhengyu    (501) staff       (20)      238 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/configure/config.py
--rw-r--r--   0 zhengyu    (501) staff       (20)    12953 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/configure/default_config.py
--rw-r--r--   0 zhengyu    (501) staff       (20)      535 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/configure/location_config.py
--rw-r--r--   0 zhengyu    (501) staff       (20)     9695 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/configure/pyart_config.py
--rw-r--r--   0 zhengyu    (501) staff       (20)    56920 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/configure/pyart_default_config.py
--rw-r--r--   0 zhengyu    (501) staff       (20)     4347 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/configure/pyart_lazydict.py
-drwxr-xr-x   0 zhengyu    (501) staff       (20)        0 2023-03-01 12:33:11.648467 pycwr-0.3.6/pycwr/core/
--rw-r--r--   0 zhengyu    (501) staff       (20)    21267 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/core/NRadar.py
--rw-r--r--   0 zhengyu    (501) staff       (20)    39903 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/core/PyartRadar.py
--rw-r--r--   0 zhengyu    (501) staff       (20)     9450 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/core/RadarGrid.py
--rw-r--r--   0 zhengyu    (501) staff       (20)   561785 2023-03-01 11:16:35.000000 pycwr-0.3.6/pycwr/core/RadarGridC.c
--rw-r--r--   0 zhengyu    (501) staff       (20)    12032 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/core/RadarGridC.pyx
--rw-r--r--   0 zhengyu    (501) staff       (20)      144 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/core/__init__.py
--rw-r--r--   0 zhengyu    (501) staff       (20)    29445 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/core/transforms.py
-drwxr-xr-x   0 zhengyu    (501) staff       (20)        0 2023-03-01 12:33:11.652557 pycwr-0.3.6/pycwr/data/
--rw-r--r--   0 zhengyu    (501) staff       (20)    86190 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/data/CHN_pronvices.dbf
--rw-r--r--   0 zhengyu    (501) staff       (20)      145 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/data/CHN_pronvices.prj
--rw-r--r--   0 zhengyu    (501) staff       (20)     8524 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/data/CHN_pronvices.sbn
--rw-r--r--   0 zhengyu    (501) staff       (20)      372 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/data/CHN_pronvices.sbx
--rw-r--r--   0 zhengyu    (501) staff       (20)  1490440 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/data/CHN_pronvices.shp
--rw-r--r--   0 zhengyu    (501) staff       (20)     7492 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/data/CHN_pronvices.shx
--rw-r--r--   0 zhengyu    (501) staff       (20)    12155 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/data/beta_function_parameters.nc
--rw-r--r--   0 zhengyu    (501) staff       (20)       38 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/data/default_opendir.json
--rw-r--r--   0 zhengyu    (501) staff       (20)    12622 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/data/radar_info.json
-drwxr-xr-x   0 zhengyu    (501) staff       (20)        0 2023-03-01 12:33:11.653388 pycwr-0.3.6/pycwr/draw/
--rw-r--r--   0 zhengyu    (501) staff       (20)    44117 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/draw/RadarPlot.py
--rw-r--r--   0 zhengyu    (501) staff       (20)    12015 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/draw/SingleRadarPlot.py
--rw-r--r--   0 zhengyu    (501) staff       (20)    11471 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/draw/SingleRadarPlotMap.py
--rw-r--r--   0 zhengyu    (501) staff       (20)    16573 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/draw/VerticalSectionPlot.py
--rw-r--r--   0 zhengyu    (501) staff       (20)      168 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/draw/__init__.py
-drwxr-xr-x   0 zhengyu    (501) staff       (20)        0 2023-03-01 12:33:11.654821 pycwr-0.3.6/pycwr/draw/colormap/
--rw-r--r--   0 zhengyu    (501) staff       (20)       65 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/draw/colormap/__init__.py
--rw-r--r--   0 zhengyu    (501) staff       (20)    96596 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/draw/colormap/_cm.py
--rw-r--r--   0 zhengyu    (501) staff       (20)     1685 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/draw/colormap/_cm_colorblind.py
--rw-r--r--   0 zhengyu    (501) staff       (20)    19200 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/draw/colormap/balance-rgb.txt
--rw-r--r--   0 zhengyu    (501) staff       (20)     4289 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/draw/colormap/cm.py
--rw-r--r--   0 zhengyu    (501) staff       (20)     1964 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/draw/colormap/cm_colorblind.py
-drwxr-xr-x   0 zhengyu    (501) staff       (20)        0 2023-03-01 12:33:11.655101 pycwr-0.3.6/pycwr/interp/
--rw-r--r--   0 zhengyu    (501) staff       (20)     4695 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/interp/RadarInterp.py
--rw-r--r--   0 zhengyu    (501) staff       (20)       52 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/interp/__init__.py
-drwxr-xr-x   0 zhengyu    (501) staff       (20)        0 2023-03-01 12:33:11.656305 pycwr-0.3.6/pycwr/io/
-drwxr-xr-x   0 zhengyu    (501) staff       (20)        0 2023-03-01 12:33:11.657207 pycwr-0.3.6/pycwr/io/BaseDataProtocol/
--rw-r--r--   0 zhengyu    (501) staff       (20)     8022 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/io/BaseDataProtocol/CCProtocol.py
--rw-r--r--   0 zhengyu    (501) staff       (20)     9442 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/io/BaseDataProtocol/PAProtocol.py
--rw-r--r--   0 zhengyu    (501) staff       (20)     2801 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/io/BaseDataProtocol/SABProtocol.py
--rw-r--r--   0 zhengyu    (501) staff       (20)     7678 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/io/BaseDataProtocol/SCProtocol.py
--rw-r--r--   0 zhengyu    (501) staff       (20)     8309 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/io/BaseDataProtocol/WSR98DProtocol.py
--rw-r--r--   0 zhengyu    (501) staff       (20)      137 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/io/BaseDataProtocol/__init__.py
--rw-r--r--   0 zhengyu    (501) staff       (20)    17825 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/io/CCFile.py
--rw-r--r--   0 zhengyu    (501) staff       (20)    19290 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/io/PAFile.py
--rw-r--r--   0 zhengyu    (501) staff       (20)    21161 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/io/SABFile.py
--rw-r--r--   0 zhengyu    (501) staff       (20)    18723 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/io/SCFile.py
--rw-r--r--   0 zhengyu    (501) staff       (20)    24443 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/io/WSR98DFile.py
--rw-r--r--   0 zhengyu    (501) staff       (20)     3573 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/io/__init__.py
--rw-r--r--   0 zhengyu    (501) staff       (20)     4889 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/io/util.py
-drwxr-xr-x   0 zhengyu    (501) staff       (20)        0 2023-03-01 12:33:11.657537 pycwr-0.3.6/pycwr/qc/
--rw-r--r--   0 zhengyu    (501) staff       (20)       82 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/qc/__init__.py
--rw-r--r--   0 zhengyu    (501) staff       (20)     3766 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/qc/attenuation.py
-drwxr-xr-x   0 zhengyu    (501) staff       (20)        0 2023-03-01 12:33:11.657974 pycwr-0.3.6/pycwr/retrieve/
--rw-r--r--   0 zhengyu    (501) staff       (20)     5518 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/retrieve/HID.py
--rw-r--r--   0 zhengyu    (501) staff       (20)     3689 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/retrieve/WindField.py
--rw-r--r--   0 zhengyu    (501) staff       (20)       75 2023-03-01 09:05:21.000000 pycwr-0.3.6/pycwr/retrieve/__init__.py
-drwxr-xr-x   0 zhengyu    (501) staff       (20)        0 2023-03-01 12:33:11.643898 pycwr-0.3.6/pycwr.egg-info/
--rw-r--r--   0 zhengyu    (501) staff       (20)      868 2023-03-01 12:33:11.000000 pycwr-0.3.6/pycwr.egg-info/PKG-INFO
--rw-r--r--   0 zhengyu    (501) staff       (20)     2012 2023-03-01 12:33:11.000000 pycwr-0.3.6/pycwr.egg-info/SOURCES.txt
--rw-r--r--   0 zhengyu    (501) staff       (20)        1 2023-03-01 12:33:11.000000 pycwr-0.3.6/pycwr.egg-info/dependency_links.txt
--rw-r--r--   0 zhengyu    (501) staff       (20)       76 2023-03-01 12:33:11.000000 pycwr-0.3.6/pycwr.egg-info/requires.txt
--rw-r--r--   0 zhengyu    (501) staff       (20)        6 2023-03-01 12:33:11.000000 pycwr-0.3.6/pycwr.egg-info/top_level.txt
--rw-r--r--   0 zhengyu    (501) staff       (20)       38 2023-03-01 12:33:11.659002 pycwr-0.3.6/setup.cfg
--rw-r--r--   0 zhengyu    (501) staff       (20)     1737 2023-03-01 12:29:53.000000 pycwr-0.3.6/setup.py
-drwxr-xr-x   0 zhengyu    (501) staff       (20)        0 2023-03-01 12:33:11.658425 pycwr-0.3.6/test/
--rw-r--r--   0 zhengyu    (501) staff       (20)     1681 2023-03-01 09:05:21.000000 pycwr-0.3.6/test/test.py
--rw-r--r--   0 zhengyu    (501) staff       (20)     1689 2023-03-01 09:05:21.000000 pycwr-0.3.6/test/test_0627.py
--rw-r--r--   0 zhengyu    (501) staff       (20)        0 2023-03-01 09:05:21.000000 pycwr-0.3.6/test/test_xband.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 09:02:17.508542 pycwr-0.4.0/
+-rwxrwxrwx   0 root         (0) root         (0)     1088 2024-05-13 08:13:33.000000 pycwr-0.4.0/LICENSE.txt
+-rwxrwxrwx   0 root         (0) root         (0)      125 2024-05-13 08:13:33.000000 pycwr-0.4.0/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)     1094 2024-05-13 09:02:17.506542 pycwr-0.4.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     3917 2024-05-13 08:13:33.000000 pycwr-0.4.0/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 09:02:17.383581 pycwr-0.4.0/pycwr/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 09:02:17.401543 pycwr-0.4.0/pycwr/GraphicalInterface/
+-rwxrwxrwx   0 root         (0) root         (0)    23249 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/GraphicalInterface/RadarInterface.py
+-rwxrwxrwx   0 root         (0) root         (0)    39034 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/GraphicalInterface/RadarUI.py
+-rwxrwxrwx   0 root         (0) root         (0)      125 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/GraphicalInterface/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)   301517 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/GraphicalInterface/icons.py
+-rwxrwxrwx   0 root         (0) root         (0)     9124 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/GraphicalInterface/station_info.py
+-rwxrwxrwx   0 root         (0) root         (0)      137 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 09:02:17.414578 pycwr-0.4.0/pycwr/configure/
+-rwxrwxrwx   0 root         (0) root         (0)      205 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/configure/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      238 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/configure/config.py
+-rwxrwxrwx   0 root         (0) root         (0)    12953 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/configure/default_config.py
+-rwxrwxrwx   0 root         (0) root         (0)      535 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/configure/location_config.py
+-rwxrwxrwx   0 root         (0) root         (0)     9695 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/configure/pyart_config.py
+-rwxrwxrwx   0 root         (0) root         (0)    56920 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/configure/pyart_default_config.py
+-rwxrwxrwx   0 root         (0) root         (0)     4347 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/configure/pyart_lazydict.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 09:02:17.427576 pycwr-0.4.0/pycwr/core/
+-rwxrwxrwx   0 root         (0) root         (0)    21319 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/core/NRadar.py
+-rwxrwxrwx   0 root         (0) root         (0)    39903 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/core/PyartRadar.py
+-rwxrwxrwx   0 root         (0) root         (0)     9639 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/core/RadarGrid.py
+-rwxrwxrwx   0 root         (0) root         (0)   723362 2024-05-13 08:15:58.000000 pycwr-0.4.0/pycwr/core/RadarGridC.c
+-rwxrwxrwx   0 root         (0) root         (0)    12753 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/core/RadarGridC.pyx
+-rwxrwxrwx   0 root         (0) root         (0)      144 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/core/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    29572 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/core/transforms.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 09:02:17.444574 pycwr-0.4.0/pycwr/data/
+-rwxrwxrwx   0 root         (0) root         (0)    86190 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/data/CHN_pronvices.dbf
+-rwxrwxrwx   0 root         (0) root         (0)      145 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/data/CHN_pronvices.prj
+-rwxrwxrwx   0 root         (0) root         (0)     8524 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/data/CHN_pronvices.sbn
+-rwxrwxrwx   0 root         (0) root         (0)      372 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/data/CHN_pronvices.sbx
+-rwxrwxrwx   0 root         (0) root         (0)  1490440 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/data/CHN_pronvices.shp
+-rwxrwxrwx   0 root         (0) root         (0)     7492 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/data/CHN_pronvices.shx
+-rwxrwxrwx   0 root         (0) root         (0)    12155 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/data/beta_function_parameters.nc
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/data/default_opendir.json
+-rwxrwxrwx   0 root         (0) root         (0)    12622 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/data/radar_info.json
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 09:02:17.453540 pycwr-0.4.0/pycwr/draw/
+-rwxrwxrwx   0 root         (0) root         (0)    44117 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/draw/RadarPlot.py
+-rwxrwxrwx   0 root         (0) root         (0)    12015 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/draw/SingleRadarPlot.py
+-rwxrwxrwx   0 root         (0) root         (0)    11471 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/draw/SingleRadarPlotMap.py
+-rwxrwxrwx   0 root         (0) root         (0)    16573 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/draw/VerticalSectionPlot.py
+-rwxrwxrwx   0 root         (0) root         (0)      168 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/draw/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 09:02:17.464541 pycwr-0.4.0/pycwr/draw/colormap/
+-rwxrwxrwx   0 root         (0) root         (0)       65 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/draw/colormap/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    96596 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/draw/colormap/_cm.py
+-rwxrwxrwx   0 root         (0) root         (0)     1685 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/draw/colormap/_cm_colorblind.py
+-rwxrwxrwx   0 root         (0) root         (0)    19200 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/draw/colormap/balance-rgb.txt
+-rwxrwxrwx   0 root         (0) root         (0)     4866 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/draw/colormap/cm.py
+-rwxrwxrwx   0 root         (0) root         (0)     1998 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/draw/colormap/cm_colorblind.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 09:02:17.467540 pycwr-0.4.0/pycwr/interp/
+-rwxrwxrwx   0 root         (0) root         (0)     4695 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/interp/RadarInterp.py
+-rwxrwxrwx   0 root         (0) root         (0)       52 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/interp/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 09:02:17.479540 pycwr-0.4.0/pycwr/io/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 09:02:17.491541 pycwr-0.4.0/pycwr/io/BaseDataProtocol/
+-rwxrwxrwx   0 root         (0) root         (0)     8022 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/io/BaseDataProtocol/CCProtocol.py
+-rwxrwxrwx   0 root         (0) root         (0)     9442 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/io/BaseDataProtocol/PAProtocol.py
+-rwxrwxrwx   0 root         (0) root         (0)     2801 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/io/BaseDataProtocol/SABProtocol.py
+-rwxrwxrwx   0 root         (0) root         (0)     7678 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/io/BaseDataProtocol/SCProtocol.py
+-rwxrwxrwx   0 root         (0) root         (0)     8309 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/io/BaseDataProtocol/WSR98DProtocol.py
+-rwxrwxrwx   0 root         (0) root         (0)      137 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/io/BaseDataProtocol/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    17825 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/io/CCFile.py
+-rwxrwxrwx   0 root         (0) root         (0)    19290 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/io/PAFile.py
+-rwxrwxrwx   0 root         (0) root         (0)    21161 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/io/SABFile.py
+-rwxrwxrwx   0 root         (0) root         (0)    18723 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/io/SCFile.py
+-rwxrwxrwx   0 root         (0) root         (0)    24443 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/io/WSR98DFile.py
+-rwxrwxrwx   0 root         (0) root         (0)     3573 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/io/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4889 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/io/util.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 09:02:17.494541 pycwr-0.4.0/pycwr/qc/
+-rwxrwxrwx   0 root         (0) root         (0)       82 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/qc/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3766 2024-05-13 08:13:33.000000 pycwr-0.4.0/pycwr/qc/attenuation.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 09:02:17.499542 pycwr-0.4.0/pycwr/retrieve/
+-rwxrwxrwx   0 root         (0) root         (0)     5518 2024-05-13 08:13:34.000000 pycwr-0.4.0/pycwr/retrieve/HID.py
+-rwxrwxrwx   0 root         (0) root         (0)     3689 2024-05-13 08:13:34.000000 pycwr-0.4.0/pycwr/retrieve/WindField.py
+-rwxrwxrwx   0 root         (0) root         (0)       75 2024-05-13 08:13:34.000000 pycwr-0.4.0/pycwr/retrieve/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 09:02:17.505542 pycwr-0.4.0/pycwr.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     1094 2024-05-13 09:02:17.000000 pycwr-0.4.0/pycwr.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2036 2024-05-13 09:02:17.000000 pycwr-0.4.0/pycwr.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-13 09:02:17.000000 pycwr-0.4.0/pycwr.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       76 2024-05-13 09:02:17.000000 pycwr-0.4.0/pycwr.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        6 2024-05-13 09:02:17.000000 pycwr-0.4.0/pycwr.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-13 09:02:17.508542 pycwr-0.4.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1737 2024-05-13 08:13:34.000000 pycwr-0.4.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 09:02:17.503541 pycwr-0.4.0/test/
+-rwxrwxrwx   0 root         (0) root         (0)     1681 2024-05-13 08:13:34.000000 pycwr-0.4.0/test/test.py
+-rwxrwxrwx   0 root         (0) root         (0)     1689 2024-05-13 08:13:34.000000 pycwr-0.4.0/test/test_0627.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 08:13:34.000000 pycwr-0.4.0/test/test_xband.py
```

### Comparing `pycwr-0.3.6/LICENSE.txt` & `pycwr-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/PKG-INFO` & `pycwr-0.4.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycwr
-Version: 0.3.6
+Version: 0.4.0
 Summary: China Weather Radar tools
 Home-page: https://github.com/YvZheng/pycwr
 Author: pycwr developers
 Author-email: YuZheng1206@outlook.com
 License: MIT
 Platform: Linux
 Platform: Mac OS-X
@@ -16,10 +16,20 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 License-File: LICENSE.txt
+Requires-Dist: matplotlib
+Requires-Dist: cython
+Requires-Dist: pyproj
+Requires-Dist: Cartopy
+Requires-Dist: xarray
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: pandas
+Requires-Dist: netCDF4
+Requires-Dist: easydict
 
 The Weather Radar Toolkit, support most of China's radar formats
 (WSR98D, CINRAD/SA/SB/CB, CINRAD/CC/CCJ, CINRAD/SC/CD)
```

### Comparing `pycwr-0.3.6/README.md` & `pycwr-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -131,11 +131,11 @@
 - [x] Interpolation algorithm support
 - [x] PPI drawing support, overlay map support
 - [ ] RHI drawing support
 - [ ] Multi-radar inversion algorithm support
 - [x] Radar product algorithm support
 - [ ] Doppler Radar/Dual polarization radar quality control algorithm
 - [ ] DSD Algorithm Support for Dual Polarization Radar
-- [x] Doppler radar wind field retrieve support
+- [ ] Doppler radar wind field retrieve support
 - [ ] Radar quantitative precipitation estimation algorithm support
 - [ ] Radar extrapolation algorithm support
 - [ ] Radar quantitative precipitation forecast  algorithm support
```

### Comparing `pycwr-0.3.6/pycwr/GraphicalInterface/RadarInterface.py` & `pycwr-0.4.0/pycwr/GraphicalInterface/RadarInterface.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/GraphicalInterface/RadarUI.py` & `pycwr-0.4.0/pycwr/GraphicalInterface/RadarUI.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/GraphicalInterface/icons.py` & `pycwr-0.4.0/pycwr/GraphicalInterface/icons.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/GraphicalInterface/station_info.py` & `pycwr-0.4.0/pycwr/GraphicalInterface/station_info.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/configure/default_config.py` & `pycwr-0.4.0/pycwr/configure/default_config.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/configure/location_config.py` & `pycwr-0.4.0/pycwr/configure/location_config.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/configure/pyart_config.py` & `pycwr-0.4.0/pycwr/configure/pyart_config.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/configure/pyart_default_config.py` & `pycwr-0.4.0/pycwr/configure/pyart_default_config.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/configure/pyart_lazydict.py` & `pycwr-0.4.0/pycwr/configure/pyart_lazydict.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/core/NRadar.py` & `pycwr-0.4.0/pycwr/core/NRadar.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,19 +103,19 @@
             for ikey in keys:
                 isweep_data[ikey] = (['time','range'], fields[ikey][istart:iend+1, :bins_per_sweep[idx]])
                 isweep_data[ikey].attrs = DEFAULT_METADATA[CINRAD_field_mapping[ikey]]
             self.fields.append(isweep_data)
         self.scan_info = xr.Dataset(data_vars={"latitude":latitude,"longitude":longitude,
                         "altitude":altitude,"scan_type":scan_type,  "frequency":frequency,
                         "start_time":time[0], "end_time":time[-1],
-                         "nyquist_velocity":(['sweep',], nyquist_velocity),
-                        "unambiguous_range":(['sweep',], unambiguous_range),
-                        "rays_per_sweep": (['sweep',], sweep_end_ray_index-sweep_start_ray_index+1),
-                        "fixed_angle": (["sweep",], fixed_angle),
-                        "beam_width":(["sweep",], 360./(sweep_end_ray_index-sweep_start_ray_index+1))},
+                         "nyquist_velocity":(['sweep',], nyquist_velocity[:nsweeps]),
+                        "unambiguous_range":(['sweep',], unambiguous_range[:nsweeps]),
+                        "rays_per_sweep": (['sweep',], (sweep_end_ray_index-sweep_start_ray_index+1)[:nsweeps]),
+                        "fixed_angle": (["sweep",], fixed_angle[:nsweeps]),
+                        "beam_width":(["sweep",], 360./(sweep_end_ray_index-sweep_start_ray_index+1)[:nsweeps])},
                         coords={"sweep": np.arange(nsweeps, dtype=int)})
         self.scan_info['latitude'].attrs = DEFAULT_METADATA['latitude']
         self.scan_info['longitude'].attrs = DEFAULT_METADATA['longitude']
         self.scan_info['altitude'].attrs = DEFAULT_METADATA['altitude']
         self.scan_info['scan_type'].attrs = DEFAULT_METADATA['scan_type']
         self.scan_info['frequency'].attrs = DEFAULT_METADATA['frequency']
         self.scan_info['nyquist_velocity'].attrs = DEFAULT_METADATA['nyquist_velocity']
```

### Comparing `pycwr-0.3.6/pycwr/core/PyartRadar.py` & `pycwr-0.4.0/pycwr/core/PyartRadar.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/core/RadarGrid.py` & `pycwr-0.4.0/pycwr/core/RadarGrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,49 +129,54 @@
         for iy in range(Ny):
             if (Grid_el[ix, iy] >= fix_elevation[0]) and (Grid_el[ix, iy] <= fix_elevation[-1]):
                 for ie in range(Ne):
                     if Grid_el[ix, iy] < fix_elevation[ie]:
                         break
                 for iaz_0, temp_az in enumerate(vol_azimuth[ie - 1]):
                     if Grid_az[ix, iy] < temp_az:
+                        Grid_az_0 = Grid_az[ix, iy]
                         break
                 else:
                     iaz_0 = 0
+                    Grid_az_0 = Grid_az[ix, iy] - 360
 
                 for range_0, temp_range in enumerate(vol_range[ie - 1]):
                     if Grid_range[ix, iy] < temp_range:
                         break
 
                 if iaz_0 == 0:
                     az_last_0 = vol_azimuth[ie - 1][iaz_0 - 1] - 360.
                 else:
                     az_last_0 = vol_azimuth[ie - 1][iaz_0 - 1]
 
                 for iaz_1, temp_az in enumerate(vol_azimuth[ie]):
                     if Grid_az[ix, iy] < temp_az:
+                        Grid_az_1 = Grid_az[ix, iy]
                         break
                 else:
                     iaz_1 = 0
+                    Grid_az_1 = Grid_az[ix, iy] - 360
 
                 for range_1, temp_range in enumerate(vol_range[ie]):
                     if Grid_range[ix, iy] < temp_range:
                         break
 
                 if iaz_1 == 0:
                     az_last_1 = vol_azimuth[ie][iaz_1 - 1] - 360.
                 else:
                     az_last_1 = vol_azimuth[ie][iaz_1 - 1]
                 if (Grid_range[ix, iy] <= vol_range[ie][-1]) and (Grid_range[ix, iy] <= vol_range[ie - 1][-1]):
-                    ER00 = interp_azimuth(Grid_az[ix, iy], az_last_0, vol_azimuth[ie - 1][iaz_0],
+                    ER00 = interp_azimuth(Grid_az_0, az_last_0, vol_azimuth[ie - 1][iaz_0],
                                           vol_value[ie - 1][iaz_0 - 1, range_0 - 1],
                                           vol_value[ie - 1][iaz_0, range_0 - 1], fillvalue)
-                    ER01 = interp_azimuth(Grid_az[ix, iy], az_last_0, vol_azimuth[ie - 1][iaz_0],
+                    ER01 = interp_azimuth(Grid_az_0, az_last_0, vol_azimuth[ie - 1][iaz_0],
                                           vol_value[ie - 1][iaz_0 - 1, range_0], vol_value[ie - 1][iaz_0, range_0], fillvalue)
-                    ER10 = interp_azimuth(Grid_az[ix, iy], az_last_1, vol_azimuth[ie][iaz_1], vol_value[ie][iaz_1 - 1, range_1 - 1],
+                    ER10 = interp_azimuth(Grid_az_1, az_last_1, vol_azimuth[ie][iaz_1], vol_value[ie][iaz_1 - 1, range_1 - 1],
                                           vol_value[ie][iaz_1, range_1 - 1], fillvalue)
-                    ER11 = interp_azimuth(Grid_az[ix, iy], az_last_1, vol_azimuth[ie][iaz_1], vol_value[ie][iaz_1 - 1, range_1],
+                    ER11 = interp_azimuth(Grid_az_1, az_last_1, vol_azimuth[ie][iaz_1], vol_value[ie][iaz_1 - 1, range_1],
                                           vol_value[ie][iaz_1, range_1], fillvalue)
                     IER0 = interp_azimuth(Grid_range[ix, iy], vol_range[ie - 1][range_0 - 1], vol_range[ie - 1][range_0], ER00, ER01,
                                           fillvalue)
                     IER1 = interp_azimuth(Grid_range[ix, iy], vol_range[ie][range_1 - 1], vol_range[ie][range_1], ER10, ER11, fillvalue)
                     GridValue[ix, iy] = interp_azimuth(Grid_el[ix, iy], fix_elevation[ie - 1], fix_elevation[ie], IER0, IER1, fillvalue)
+
     return GridValue
```

### Comparing `pycwr-0.3.6/pycwr/core/RadarGridC.pyx` & `pycwr-0.4.0/pycwr/core/RadarGridC.pyx`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,17 @@
     直角坐标系转换为天线坐标系
     ranges: 天线坐标系距离雷达天线的距离
     """
     cdef double PI = 3.141592653589793
     cdef double R = 8494666.6666666661
     cdef double elevation, ranges, azimuth
     ranges = ((R+h)**2 + (R+z)**2 - 2*(R+h)*(R+z)*cos((x**2 + y**2)**0.5/R))**0.5
-    elevation = acos((R+z)*sin((x**2 + y**2)**0.5/R)/ranges) * 180./PI
+    # elevation = acos((R+z)*sin((x**2 + y**2)**0.5/R)/ranges) * 180./PI
+    elevation = (acos(
+        ((R + h) ** 2 + ranges ** 2 - (R + z) ** 2) / (2 * (R + h) * ranges)) - PI / 2) * 180. / PI
     azimuth = xy_to_azimuth(x, y)
     return azimuth, ranges, elevation
 
 @cython.cdivision(True)
 def xy_to_azimuth(double x, double y):
     """
     using x and y to cal azimuth
@@ -164,77 +166,91 @@
     :return:
     """
     cdef int Ne = fix_elevation.shape[0]
     cdef int Nx = GridX.shape[0]
     cdef int Ny = GridX.shape[1]
     cdef cnp.ndarray GridValue = np.full([Nx, Ny], fillvalue, dtype=np.float64)
     cdef int ix, iy, ie, iaz_0, iaz_1, range_0, range_1
-    cdef double az, el, r, temp_az, temp_range, az_last_0, az_last_1
+    cdef double az, el, r, temp_az, temp_range, az_last_0, az_last_1, az_values_0, az_values_1
     cdef double ER00, ER01, ER10, ER11, IER0, IER1
     for ix in range(Nx):
         for iy in range(Ny):
             az, r, el = cartesian_to_antenna(GridX[ix, iy], GridY[ix, iy], level_height, radar_height)
             if (el <= fix_elevation[-1]) and (el >= fix_elevation[0]):
+                # Check elevation bounds
                 for ie in range(Ne):
                     if el < fix_elevation[ie]:
                         break
+                # Check azimuth bounds
                 for iaz_0, temp_az in enumerate(vol_azimuth[ie-1]):
                     if az < temp_az:
+                        az_values_0 = az #第一层仰角
                         break
                 else:
                     iaz_0 = 0
-                    az = az - 360.
-
+                    az_values_0 = az - 360.
+                # Check range bounds
                 for range_0, temp_range in enumerate(vol_range[ie-1]):
                     if r < temp_range:
                         break
 
                 if iaz_0 == 0:
                     az_last_0 = vol_azimuth[ie-1][iaz_0-1] - 360.
                 else:
                     az_last_0 = vol_azimuth[ie-1][iaz_0-1]
 
                 for iaz_1, temp_az in enumerate(vol_azimuth[ie]):
                     if az < temp_az:
-                        break
+                        az_values_1 = az
+                        break #第一层仰角
                 else:
                     iaz_1 = 0
+                    az_values_1 = az - 360.
+
                 for range_1, temp_range in enumerate(vol_range[ie]):
                     if r < temp_range:
                         break
                 if iaz_1 == 0:
                     az_last_1 = vol_azimuth[ie][iaz_1-1] - 360.
                 else:
                     az_last_1 = vol_azimuth[ie][iaz_1-1]
 
                 if (r <= vol_range[ie][-1]) and (r <= vol_range[ie-1][-1]):
-                    ER00 = interp_azimuth(az, az_last_0, vol_azimuth[ie-1][iaz_0], vol_value[ie-1][iaz_0-1, range_0-1],
+                    ER00 = interp_azimuth(az_values_0, az_last_0, vol_azimuth[ie-1][iaz_0], vol_value[ie-1][iaz_0-1, range_0-1],
                                           vol_value[ie-1][iaz_0, range_0-1], fillvalue)
-                    ER01 = interp_azimuth(az, az_last_0, vol_azimuth[ie-1][iaz_0], vol_value[ie-1][iaz_0-1, range_0],
+                    ER01 = interp_azimuth(az_values_0, az_last_0, vol_azimuth[ie-1][iaz_0], vol_value[ie-1][iaz_0-1, range_0],
                                           vol_value[ie-1][iaz_0, range_0], fillvalue)
-                    ER10 = interp_azimuth(az, az_last_1, vol_azimuth[ie][iaz_1], vol_value[ie][iaz_1-1, range_1-1],
+                    ER10 = interp_azimuth(az_values_1, az_last_1, vol_azimuth[ie][iaz_1], vol_value[ie][iaz_1-1, range_1-1],
                                           vol_value[ie][iaz_1, range_1-1], fillvalue)
-                    ER11 = interp_azimuth(az, az_last_1, vol_azimuth[ie][iaz_1], vol_value[ie][iaz_1-1, range_1],
+                    ER11 = interp_azimuth(az_values_1, az_last_1, vol_azimuth[ie][iaz_1], vol_value[ie][iaz_1-1, range_1],
                                           vol_value[ie][iaz_1, range_1], fillvalue)
                     IER0 = interp_azimuth(r, vol_range[ie-1][range_0-1], vol_range[ie-1][range_0], ER00, ER01, fillvalue)
                     IER1 = interp_azimuth(r, vol_range[ie][range_1-1], vol_range[ie][range_1], ER10, ER11, fillvalue)
                     GridValue[ix, iy] = interp_azimuth(el, fix_elevation[ie-1], fix_elevation[ie], IER0, IER1, fillvalue)
     return GridValue
 
 def interp_azimuth(double az, double az_0, double az_1, double dat_0, double dat_1, double fillvalue):
     """
     在两个方位角或者距离之间进行插值
     """
-    if (dat_0 != fillvalue) and (dat_1 != fillvalue):
-        return ((az_1 - az)*dat_0 + (az - az_0) * dat_1)/(az_1 - az_0)
+    # Check for division by zero
+    if az_1 == az_0:
+        return fillvalue  # or some other value that makes sense in your context
+
+    # Check for missing values
+    if (dat_0 == fillvalue) and (dat_1 == fillvalue):
+        return fillvalue
     elif dat_0 == fillvalue:
         return dat_1
-    else:
+    elif dat_1 == fillvalue:
         return dat_0
 
+    # Perform linear interpolation
+    return ((az_1 - az) * dat_0 + (az - az_0) * dat_1) / (az_1 - az_0)
+
 @cython.boundscheck(False)  # Deactivate bounds checking
 def get_CR_xy(vol_azimuth, vol_range, cnp.ndarray[cnp.float64_t, ndim=1] fix_elevation, vol_value, double radar_height,
               cnp.ndarray[cnp.float64_t, ndim=2] GridX, cnp.ndarray[cnp.float64_t, ndim=2] GridY, double fillvalue):
     """
     计算组合反射率，利用雷达体扫的数据
     :param vol_azimuth:存放多个仰角体扫方位角的列表, list, units:degree
     :param vol_range:存放多个仰角体扫距离的列表, list, units:meters
@@ -254,8 +270,8 @@
     for ie in range(Ne):
         GridValue[ie,:,:] = ppi_to_grid(vol_azimuth[ie], vol_range[ie], fix_elevation[ie],
                                        vol_value[ie], radar_height, GridX, GridY, fillvalue)
 
     GridValue = np.where(GridValue == fillvalue, np.nan, GridValue)
     GridValue = np.nanmax(GridValue, axis=0)
     GridValue = np.where(np.isnan(GridValue), fillvalue, GridValue)
-    return GridValue
+    return GridValue
```

### Comparing `pycwr-0.3.6/pycwr/core/transforms.py` & `pycwr-0.4.0/pycwr/core/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,17 @@
     y, units:meters
     z, units:meters
     h, units:meters
     return ranges, azimuth, elevation
     """
     R = 8494666.6666666661 #等效地球半径
     ranges = ((R + h) ** 2 + (R + z) ** 2 - 2 * (R + h) * (R + z) * np.cos((x ** 2 + y ** 2) ** 0.5 / R)) ** 0.5
-    elevation = np.arccos((R + z) * np.sin((x ** 2 + y ** 2) ** 0.5 / R) / ranges) * 180. / np.pi
+    #elevation = np.arccos((R + z) * np.sin((x ** 2 + y ** 2) ** 0.5 / R) / ranges) * 180. / np.pi
+    elevation = (np.arccos(((R + h) ** 2 + ranges ** 2 - (R + z) ** 2) / (2 * (R + h) * ranges)) - np.pi / 2) * 180. / np.pi
+
     azimuth = _azimuth(x, y)
     return azimuth, ranges, elevation
 
 def cartesian_to_antenna_cwr(x, y, elevation , h):
     """根据采样点距离雷达的x,y的水平距离,以及雷达仰角
     return x, y, z
     和高度,计算该点雷达的斜距
```

### Comparing `pycwr-0.3.6/pycwr/data/CHN_pronvices.dbf` & `pycwr-0.4.0/pycwr/data/CHN_pronvices.dbf`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/data/CHN_pronvices.sbn` & `pycwr-0.4.0/pycwr/data/CHN_pronvices.sbn`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/data/CHN_pronvices.shp` & `pycwr-0.4.0/pycwr/data/CHN_pronvices.shp`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/data/CHN_pronvices.shx` & `pycwr-0.4.0/pycwr/data/CHN_pronvices.shx`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/data/beta_function_parameters.nc` & `pycwr-0.4.0/pycwr/data/beta_function_parameters.nc`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/data/radar_info.json` & `pycwr-0.4.0/pycwr/data/radar_info.json`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/draw/RadarPlot.py` & `pycwr-0.4.0/pycwr/draw/RadarPlot.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/draw/SingleRadarPlot.py` & `pycwr-0.4.0/pycwr/draw/SingleRadarPlot.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/draw/SingleRadarPlotMap.py` & `pycwr-0.4.0/pycwr/draw/SingleRadarPlotMap.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/draw/VerticalSectionPlot.py` & `pycwr-0.4.0/pycwr/draw/VerticalSectionPlot.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/draw/colormap/_cm.py` & `pycwr-0.4.0/pycwr/draw/colormap/_cm.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/draw/colormap/_cm_colorblind.py` & `pycwr-0.4.0/pycwr/draw/colormap/_cm_colorblind.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/draw/colormap/balance-rgb.txt` & `pycwr-0.4.0/pycwr/draw/colormap/balance-rgb.txt`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/draw/colormap/cm.py` & `pycwr-0.4.0/pycwr/draw/colormap/cm.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,37 +100,48 @@
             # and the result is shades of gray.
         else:
             # Flip x and exchange the y values facing x = 0 and x = 1.
             valnew = [(1.0 - x, y1, y0) for x, y0, y1 in reversed(val)]
         data_r[key] = valnew
     return data_r
 
-
+#
+# def _reverse_cmap_spec(spec):
+#     """Reverses cmap specification *spec*, can handle both dict and tuple
+#     type specs."""
+#     with warnings.catch_warnings():
+#         warnings.simplefilter("ignore", FutureWarning)
+#         if 'red' in spec:
+#             return revcmap(spec)
+#         else:
+#             revspec = list(reversed(spec))
+#             if len(revspec[0]) == 2:    # e.g., (1, (1.0, 0.0, 1.0))
+#                 revspec = [(1.0 - a, b) for a, b in revspec]
+#             return revspec
 def _reverse_cmap_spec(spec):
     """Reverses cmap specification *spec*, can handle both dict and tuple
     type specs."""
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", FutureWarning)
-        if 'red' in spec:
+        if isinstance(spec, dict) and "red" in spec.keys():
             return revcmap(spec)
         else:
             revspec = list(reversed(spec))
-            if len(revspec[0]) == 2:    # e.g., (1, (1.0, 0.0, 1.0))
+            if len(revspec[0]) == 2:  # e.g., (1, (1.0, 0.0, 1.0))
                 revspec = [(1.0 - a, b) for a, b in revspec]
             return revspec
 
-
 def _generate_cmap(name, lutsize):
     """Generates the requested cmap from it's name *name*.  The lut size is
     *lutsize*."""
 
     spec = datad[name]
 
     # Generate the colormap object.
-    if 'red' in spec:
+    if isinstance(spec, dict) and "red" in spec.keys():
         return colors.LinearSegmentedColormap(name, spec, lutsize)
     else:
         return colors.LinearSegmentedColormap.from_list(name, spec, lutsize)
 
 LUTSIZE = mpl.rcParams['image.lut']
 
 # need this list because datad is changed in loop
```

### Comparing `pycwr-0.3.6/pycwr/draw/colormap/cm_colorblind.py` & `pycwr-0.4.0/pycwr/draw/colormap/cm_colorblind.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     """Generates the requested cmap from it's name *name*. The lut size is
     *lutsize*."""
 
     spec = datad[name]
     # Generate the colormap object.
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", FutureWarning)
-        if 'red' in spec:
+        if isinstance(spec, dict) and "red" in spec.keys():
             return colors.LinearSegmentedColormap(name, spec, lutsize)
         else:
             return colors.LinearSegmentedColormap.from_list(name, spec, lutsize)
 
 cmap_d = dict()
 
 # reverse all the colormaps.
```

### Comparing `pycwr-0.3.6/pycwr/interp/RadarInterp.py` & `pycwr-0.4.0/pycwr/interp/RadarInterp.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/io/BaseDataProtocol/CCProtocol.py` & `pycwr-0.4.0/pycwr/io/BaseDataProtocol/CCProtocol.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/io/BaseDataProtocol/PAProtocol.py` & `pycwr-0.4.0/pycwr/io/BaseDataProtocol/PAProtocol.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/io/BaseDataProtocol/SABProtocol.py` & `pycwr-0.4.0/pycwr/io/BaseDataProtocol/SABProtocol.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/io/BaseDataProtocol/SCProtocol.py` & `pycwr-0.4.0/pycwr/io/BaseDataProtocol/SCProtocol.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/io/BaseDataProtocol/WSR98DProtocol.py` & `pycwr-0.4.0/pycwr/io/BaseDataProtocol/WSR98DProtocol.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/io/CCFile.py` & `pycwr-0.4.0/pycwr/io/CCFile.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/io/PAFile.py` & `pycwr-0.4.0/pycwr/io/PAFile.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/io/SABFile.py` & `pycwr-0.4.0/pycwr/io/SABFile.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/io/SCFile.py` & `pycwr-0.4.0/pycwr/io/SCFile.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/io/WSR98DFile.py` & `pycwr-0.4.0/pycwr/io/WSR98DFile.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/io/__init__.py` & `pycwr-0.4.0/pycwr/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/io/util.py` & `pycwr-0.4.0/pycwr/io/util.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/qc/attenuation.py` & `pycwr-0.4.0/pycwr/qc/attenuation.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/retrieve/HID.py` & `pycwr-0.4.0/pycwr/retrieve/HID.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr/retrieve/WindField.py` & `pycwr-0.4.0/pycwr/retrieve/WindField.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/pycwr.egg-info/PKG-INFO` & `pycwr-0.4.0/pycwr.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycwr
-Version: 0.3.6
+Version: 0.4.0
 Summary: China Weather Radar tools
 Home-page: https://github.com/YvZheng/pycwr
 Author: pycwr developers
 Author-email: YuZheng1206@outlook.com
 License: MIT
 Platform: Linux
 Platform: Mac OS-X
@@ -16,10 +16,20 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 License-File: LICENSE.txt
+Requires-Dist: matplotlib
+Requires-Dist: cython
+Requires-Dist: pyproj
+Requires-Dist: Cartopy
+Requires-Dist: xarray
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: pandas
+Requires-Dist: netCDF4
+Requires-Dist: easydict
 
 The Weather Radar Toolkit, support most of China's radar formats
 (WSR98D, CINRAD/SA/SB/CB, CINRAD/CC/CCJ, CINRAD/SC/CD)
```

### Comparing `pycwr-0.3.6/pycwr.egg-info/SOURCES.txt` & `pycwr-0.4.0/pycwr.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 pycwr/configure/location_config.py
 pycwr/configure/pyart_config.py
 pycwr/configure/pyart_default_config.py
 pycwr/configure/pyart_lazydict.py
 pycwr/core/NRadar.py
 pycwr/core/PyartRadar.py
 pycwr/core/RadarGrid.py
+pycwr/core/RadarGridC.c
 pycwr/core/RadarGridC.pyx
 pycwr/core/__init__.py
 pycwr/core/transforms.py
 pycwr/data/CHN_pronvices.dbf
 pycwr/data/CHN_pronvices.prj
 pycwr/data/CHN_pronvices.sbn
 pycwr/data/CHN_pronvices.sbx
```

### Comparing `pycwr-0.3.6/setup.py` & `pycwr-0.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
     'Topic :: Scientific/Engineering',
     'Topic :: Scientific/Engineering :: Atmospheric Science',
     "Operating System :: OS Independent",]
 setup(
     name=DISTNAME,
-    version="0.3.6",
+    version="0.4.0",
     author=AUTHOR,
     license=LICENSE,
     author_email=AUTHOR_EMAIL,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     python_requires=PYTHON_REQUIRES,
     install_requires=INSTALL_REQUIRES,
```

### Comparing `pycwr-0.3.6/test/test.py` & `pycwr-0.4.0/test/test.py`

 * *Files identical despite different names*

### Comparing `pycwr-0.3.6/test/test_0627.py` & `pycwr-0.4.0/test/test_0627.py`

 * *Files identical despite different names*

