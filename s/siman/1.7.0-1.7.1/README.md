# Comparing `tmp/siman-1.7.0.tar.gz` & `tmp/siman-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/siman-1.7.0.tar", last modified: Mon Apr  1 11:29:22 2024, max compression
+gzip compressed data, was "dist/siman-1.7.1.tar", last modified: Mon May 13 19:13:10 2024, max compression
```

## Comparing `siman-1.7.0.tar` & `siman-1.7.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-04-01 11:29:22.738325 siman-1.7.0/
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18047 2021-02-17 13:28:25.000000 siman-1.7.0/LICENSE
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       98 2021-02-17 13:28:25.000000 siman-1.7.0/MANIFEST.in
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2024-04-01 11:29:22.738325 siman-1.7.0/PKG-INFO
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      409 2021-02-17 13:28:25.000000 siman-1.7.0/README.md
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       38 2024-04-01 11:29:22.738325 siman-1.7.0/setup.cfg
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      989 2024-04-01 11:29:18.000000 siman-1.7.0/setup.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-04-01 11:29:22.736325 siman-1.7.0/siman/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2473 2023-07-14 10:44:19.000000 siman-1.7.0/siman/3d_plot.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3215 2024-04-01 10:39:48.000000 siman-1.7.0/siman/SSHTools.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       32 2023-07-14 10:44:19.000000 siman-1.7.0/siman/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50716 2024-04-01 10:39:48.000000 siman-1.7.0/siman/analysis.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    26024 2023-07-14 10:44:19.000000 siman-1.7.0/siman/analysis_functions.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-04-01 11:29:22.736325 siman-1.7.0/siman/analyze/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.7.0/siman/analyze/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10970 2022-09-20 15:22:50.000000 siman-1.7.0/siman/analyze/segregation.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1160 2023-07-14 10:44:19.000000 siman-1.7.0/siman/approximation.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    16329 2023-07-14 10:44:19.000000 siman-1.7.0/siman/bands.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   121473 2024-04-01 10:39:48.000000 siman-1.7.0/siman/calc_manage (2).py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   122774 2024-04-01 10:39:48.000000 siman-1.7.0/siman/calc_manage.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1085 2023-07-14 10:44:19.000000 siman-1.7.0/siman/calcul.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-04-01 11:29:22.737325 siman-1.7.0/siman/calculators/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.7.0/siman/calculators/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3685 2022-09-20 15:22:50.000000 siman-1.7.0/siman/calculators/aims.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8718 2022-09-20 15:22:50.000000 siman-1.7.0/siman/calculators/gaussian.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3769 2022-09-20 15:22:50.000000 siman-1.7.0/siman/calculators/qe.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    57149 2024-04-01 10:39:48.000000 siman-1.7.0/siman/calculators/vasp.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    38832 2022-09-20 15:22:50.000000 siman-1.7.0/siman/calculators/vasp_old.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-04-01 11:29:22.737325 siman-1.7.0/siman/chg/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2021-02-17 13:28:25.000000 siman-1.7.0/siman/chg/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6771 2021-02-17 13:28:25.000000 siman-1.7.0/siman/chg/chg_func.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3718 2021-02-17 13:28:25.000000 siman-1.7.0/siman/chg/vasputil_chgarith_module.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    11041 2023-07-16 18:04:57.000000 siman-1.7.0/siman/classes.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-04-01 11:29:22.738325 siman-1.7.0/siman/core/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.7.0/siman/core/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    53522 2024-04-01 10:39:48.000000 siman-1.7.0/siman/core/calculation.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    45277 2022-09-20 15:22:50.000000 siman-1.7.0/siman/core/calculation_old.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    34063 2024-04-01 10:39:48.000000 siman-1.7.0/siman/core/cluster_batch_script.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3783 2023-07-26 16:52:32.000000 siman-1.7.0/siman/core/cluster_run_script.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2122 2023-07-16 18:04:57.000000 siman-1.7.0/siman/core/molecule.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   120871 2024-04-01 10:39:48.000000 siman-1.7.0/siman/core/structure.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    20407 2023-07-18 15:59:51.000000 siman-1.7.0/siman/database.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3192 2023-07-14 10:44:19.000000 siman-1.7.0/siman/default_project_conf.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10776 2023-07-14 10:44:19.000000 siman-1.7.0/siman/dev_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33350 2024-04-01 10:39:48.000000 siman-1.7.0/siman/dos_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     9424 2023-07-14 10:44:19.000000 siman-1.7.0/siman/fit_hex.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    28322 2024-04-01 10:39:48.000000 siman-1.7.0/siman/functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   115084 2024-04-01 10:39:48.000000 siman-1.7.0/siman/geo.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    16831 2024-04-01 10:39:48.000000 siman-1.7.0/siman/header.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      286 2023-07-14 10:44:19.000000 siman-1.7.0/siman/helper_for_writing_beatiful_code.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    40269 2023-07-14 10:44:19.000000 siman-1.7.0/siman/impurity.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    90186 2024-04-01 10:39:48.000000 siman-1.7.0/siman/inout.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     4642 2023-07-14 10:44:19.000000 siman-1.7.0/siman/kpoints_functions.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-04-01 11:29:22.738325 siman-1.7.0/siman/mat_prop/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.7.0/siman/mat_prop/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1574 2022-09-20 15:22:50.000000 siman-1.7.0/siman/mat_prop/mat_prop.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    46189 2023-07-14 10:44:19.000000 siman-1.7.0/siman/matproj_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    17009 2023-07-14 10:44:19.000000 siman-1.7.0/siman/monte.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      980 2023-07-14 10:44:19.000000 siman-1.7.0/siman/monte_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31738 2024-04-01 10:39:48.000000 siman-1.7.0/siman/neb.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    44420 2023-07-14 10:44:19.000000 siman-1.7.0/siman/pairs.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50674 2023-11-01 19:53:34.000000 siman-1.7.0/siman/picture_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    25262 2023-07-14 10:44:19.000000 siman-1.7.0/siman/plot_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     5224 2023-07-14 10:44:19.000000 siman-1.7.0/siman/polaron.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2406 2023-07-14 10:44:19.000000 siman-1.7.0/siman/polaron_hop.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3772 2023-07-14 10:44:19.000000 siman-1.7.0/siman/polaron_mod.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   194864 2024-04-01 10:39:48.000000 siman-1.7.0/siman/project_funcs.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    22880 2023-07-14 10:44:19.000000 siman-1.7.0/siman/properties_2d.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1114 2023-07-14 10:44:19.000000 siman-1.7.0/siman/properties_energy.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1091 2023-07-14 10:44:19.000000 siman-1.7.0/siman/properties_lattice.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31133 2024-04-01 10:39:48.000000 siman-1.7.0/siman/set_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1352 2023-07-14 10:44:19.000000 siman-1.7.0/siman/simanrc.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      174 2023-07-14 10:44:19.000000 siman-1.7.0/siman/small_classes.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6875 2023-11-01 20:00:05.000000 siman-1.7.0/siman/small_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8328 2023-07-14 10:44:19.000000 siman-1.7.0/siman/structure_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8854 2023-07-14 10:44:19.000000 siman-1.7.0/siman/table_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2780 2023-07-14 10:44:19.000000 siman-1.7.0/siman/thermo.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    18673 2023-07-14 10:44:19.000000 siman-1.7.0/siman/workflow_utilities.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-04-01 11:29:22.736325 siman-1.7.0/siman.egg-info/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2024-04-01 11:29:22.000000 siman-1.7.0/siman.egg-info/PKG-INFO
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1702 2024-04-01 11:29:22.000000 siman-1.7.0/siman.egg-info/SOURCES.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        1 2024-04-01 11:29:22.000000 siman-1.7.0/siman.egg-info/dependency_links.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       76 2024-04-01 11:29:22.000000 siman-1.7.0/siman.egg-info/requires.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        6 2024-04-01 11:29:22.000000 siman-1.7.0/siman.egg-info/top_level.txt
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-05-13 19:13:10.456055 siman-1.7.1/
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18047 2021-02-17 13:28:25.000000 siman-1.7.1/LICENSE
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       98 2021-02-17 13:28:25.000000 siman-1.7.1/MANIFEST.in
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2024-05-13 19:13:10.456055 siman-1.7.1/PKG-INFO
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      409 2021-02-17 13:28:25.000000 siman-1.7.1/README.md
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       38 2024-05-13 19:13:10.456055 siman-1.7.1/setup.cfg
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      989 2024-05-13 19:12:59.000000 siman-1.7.1/setup.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-05-13 19:13:10.452055 siman-1.7.1/siman/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2473 2023-07-14 10:44:19.000000 siman-1.7.1/siman/3d_plot.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3215 2024-04-01 10:39:48.000000 siman-1.7.1/siman/SSHTools.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       32 2023-07-14 10:44:19.000000 siman-1.7.1/siman/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50767 2024-05-13 16:42:27.000000 siman-1.7.1/siman/analysis.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    26024 2023-07-14 10:44:19.000000 siman-1.7.1/siman/analysis_functions.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-05-13 19:13:10.453055 siman-1.7.1/siman/analyze/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.7.1/siman/analyze/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10970 2022-09-20 15:22:50.000000 siman-1.7.1/siman/analyze/segregation.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1160 2023-07-14 10:44:19.000000 siman-1.7.1/siman/approximation.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    16329 2023-07-14 10:44:19.000000 siman-1.7.1/siman/bands.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   121473 2024-04-01 10:39:48.000000 siman-1.7.1/siman/calc_manage (2).py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   123358 2024-05-13 16:42:27.000000 siman-1.7.1/siman/calc_manage.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1085 2023-07-14 10:44:19.000000 siman-1.7.1/siman/calcul.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-05-13 19:13:10.454055 siman-1.7.1/siman/calculators/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.7.1/siman/calculators/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3685 2022-09-20 15:22:50.000000 siman-1.7.1/siman/calculators/aims.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     9011 2024-05-13 16:35:29.000000 siman-1.7.1/siman/calculators/gaussian.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3769 2022-09-20 15:22:50.000000 siman-1.7.1/siman/calculators/qe.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    57149 2024-04-01 10:39:48.000000 siman-1.7.1/siman/calculators/vasp.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    38832 2022-09-20 15:22:50.000000 siman-1.7.1/siman/calculators/vasp_old.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-05-13 19:13:10.454055 siman-1.7.1/siman/chg/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2021-02-17 13:28:25.000000 siman-1.7.1/siman/chg/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6771 2024-05-13 16:42:27.000000 siman-1.7.1/siman/chg/chg_func.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3718 2021-02-17 13:28:25.000000 siman-1.7.1/siman/chg/vasputil_chgarith_module.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    11041 2023-07-16 18:04:57.000000 siman-1.7.1/siman/classes.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-05-13 19:13:10.455055 siman-1.7.1/siman/core/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.7.1/siman/core/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    53942 2024-05-13 16:42:27.000000 siman-1.7.1/siman/core/calculation.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    45277 2022-09-20 15:22:50.000000 siman-1.7.1/siman/core/calculation_old.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    34063 2024-04-01 10:39:48.000000 siman-1.7.1/siman/core/cluster_batch_script.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3783 2023-07-26 16:52:32.000000 siman-1.7.1/siman/core/cluster_run_script.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2122 2023-07-16 18:04:57.000000 siman-1.7.1/siman/core/molecule.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   121776 2024-05-13 16:42:27.000000 siman-1.7.1/siman/core/structure.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    20407 2023-07-18 15:59:51.000000 siman-1.7.1/siman/database.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3192 2023-07-14 10:44:19.000000 siman-1.7.1/siman/default_project_conf.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10776 2023-07-14 10:44:19.000000 siman-1.7.1/siman/dev_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33350 2024-04-01 10:39:48.000000 siman-1.7.1/siman/dos_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     9424 2023-07-14 10:44:19.000000 siman-1.7.1/siman/fit_hex.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    28322 2024-04-01 10:39:48.000000 siman-1.7.1/siman/functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   115181 2024-05-13 16:42:27.000000 siman-1.7.1/siman/geo.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    16844 2024-05-13 16:46:33.000000 siman-1.7.1/siman/header.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      286 2023-07-14 10:44:19.000000 siman-1.7.1/siman/helper_for_writing_beatiful_code.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    40269 2023-07-14 10:44:19.000000 siman-1.7.1/siman/impurity.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    90259 2024-05-13 16:44:51.000000 siman-1.7.1/siman/inout.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     4642 2023-07-14 10:44:19.000000 siman-1.7.1/siman/kpoints_functions.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-05-13 19:13:10.455055 siman-1.7.1/siman/mat_prop/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.7.1/siman/mat_prop/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1574 2022-09-20 15:22:50.000000 siman-1.7.1/siman/mat_prop/mat_prop.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    46189 2023-07-14 10:44:19.000000 siman-1.7.1/siman/matproj_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    17009 2023-07-14 10:44:19.000000 siman-1.7.1/siman/monte.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      980 2023-07-14 10:44:19.000000 siman-1.7.1/siman/monte_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31738 2024-04-01 10:39:48.000000 siman-1.7.1/siman/neb.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    44420 2023-07-14 10:44:19.000000 siman-1.7.1/siman/pairs.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50674 2023-11-01 19:53:34.000000 siman-1.7.1/siman/picture_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    25262 2023-07-14 10:44:19.000000 siman-1.7.1/siman/plot_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     5224 2023-07-14 10:44:19.000000 siman-1.7.1/siman/polaron.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2406 2023-07-14 10:44:19.000000 siman-1.7.1/siman/polaron_hop.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3772 2023-07-14 10:44:19.000000 siman-1.7.1/siman/polaron_mod.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   194862 2024-05-13 16:42:27.000000 siman-1.7.1/siman/project_funcs.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    22880 2023-07-14 10:44:19.000000 siman-1.7.1/siman/properties_2d.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1114 2023-07-14 10:44:19.000000 siman-1.7.1/siman/properties_energy.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1091 2023-07-14 10:44:19.000000 siman-1.7.1/siman/properties_lattice.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31185 2024-05-13 16:42:27.000000 siman-1.7.1/siman/set_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1352 2023-07-14 10:44:19.000000 siman-1.7.1/siman/simanrc.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      174 2023-07-14 10:44:19.000000 siman-1.7.1/siman/small_classes.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6875 2023-11-01 20:00:05.000000 siman-1.7.1/siman/small_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8328 2023-07-14 10:44:19.000000 siman-1.7.1/siman/structure_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8854 2023-07-14 10:44:19.000000 siman-1.7.1/siman/table_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2780 2023-07-14 10:44:19.000000 siman-1.7.1/siman/thermo.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    18673 2023-07-14 10:44:19.000000 siman-1.7.1/siman/workflow_utilities.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-05-13 19:13:10.453055 siman-1.7.1/siman.egg-info/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2024-05-13 19:13:10.000000 siman-1.7.1/siman.egg-info/PKG-INFO
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1702 2024-05-13 19:13:10.000000 siman-1.7.1/siman.egg-info/SOURCES.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        1 2024-05-13 19:13:10.000000 siman-1.7.1/siman.egg-info/dependency_links.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       76 2024-05-13 19:13:10.000000 siman-1.7.1/siman.egg-info/requires.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        6 2024-05-13 19:13:10.000000 siman-1.7.1/siman.egg-info/top_level.txt
```

### Comparing `siman-1.7.0/LICENSE` & `siman-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/PKG-INFO` & `siman-1.7.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siman
-Version: 1.7.0
+Version: 1.7.1
 Summary: Manager for DFT calculations
 Home-page: https://github.com/dimonaks/siman
 Author: Dmitry Aksenov
 Author-email: dimonaks@gmail.com
 License: GPL
 Keywords: DFT VASP Density Functional Theory NEB DFT+U PAW GGA Monte-Carlo
 Platform: UNKNOWN
```

### Comparing `siman-1.7.0/setup.py` & `siman-1.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="siman",
-    version="1.7.0",
+    version="1.7.1",
     author="Dmitry Aksenov",
     author_email="dimonaks@gmail.com",
     description="Manager for DFT calculations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dimonaks/siman",
     license = 'GPL',
```

### Comparing `siman-1.7.0/siman/3d_plot.py` & `siman-1.7.1/siman/3d_plot.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/SSHTools.py` & `siman-1.7.1/siman/SSHTools.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/analysis.py` & `siman-1.7.1/siman/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1502,15 +1502,16 @@
     st1 = cl1.end
     st2 = cl2.end
     # pm = st1.convert2pymatgen(oxidation = {'Y':'Y3+', 'Ba':'Ba2+', 'Co':'Co2.25+', 'O':'O2-'})
     natom1 = st1.get_natom()
     natom2 = st2.get_natom()
 
     if natom1%natom2:
-        printlog('Warning! Non-stoichiometric slab, atom1/natom2 is', natom1/natom2)
+        printlog('Warning! Non-stoichiometric slab, natom1/natom2 is', natom1/natom2, 
+            imp = 'y')
 
 
     if normal == 0:
         A = np.linalg.norm( np.cross(st1.rprimd[1] , st1.rprimd[2]) )
 
     if normal == 1:
         A = np.linalg.norm( np.cross(st1.rprimd[0] , st1.rprimd[2]) )
@@ -1570,15 +1571,16 @@
         for el in uniqe_elements:
             dif = els1.count(el) - mul * els2.count(el)
             if not float(dif).is_integer():
                 printlog('Error! difference of atom numbers is not integer for element ', el, 'something is wrong')
             if abs(dif) > 0:
                 el_dif[el] = int(dif) 
 
-        print('The following elements are off-stoichiometry in the slab', el_dif, 'please provide corresponding chemical potentials')
+        if not silent:
+            print('The following elements are off-stoichiometry in the slab', el_dif, 'please provide corresponding chemical potentials')
         
         E_nonst = 0
         for key in el_dif:
             if key not in chem_pot:
                 printlog('Warning! no chemical potential for ', key, 'in chem_pot, return')
                 return
 
@@ -1702,15 +1704,14 @@
     st2 = cl_bulk.end
 
     e1 = cl_gb.e0
     n1 = st1.natom
     e2 = cl_bulk.e0
     n2 = st2.natom
 
-
     A = st1.get_surface_area()
 
 
     e_gb = (e1 - e2*n1/n2)/2/A * header.eV_A_to_J_m
     print('E_gb = {} J/m2; Check manually that stoichiometry is the same in cl_gb and cl_bulk'.format(round(e_gb, 2)))
     return e_gb
```

### Comparing `siman-1.7.0/siman/analysis_functions.py` & `siman-1.7.1/siman/analysis_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/analyze/segregation.py` & `siman-1.7.1/siman/analyze/segregation.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/approximation.py` & `siman-1.7.1/siman/approximation.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/bands.py` & `siman-1.7.1/siman/bands.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/calc_manage (2).py` & `siman-1.7.1/siman/calc_manage (2).py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/calc_manage.py` & `siman-1.7.1/siman/calc_manage.py`

 * *Files 1% similar despite different names*

```diff
@@ -564,15 +564,15 @@
         full_chg - including chg file
         """
         nonlocal  it, setlist, id_base, it_suffix
         struct_des = header.struct_des
 
         printlog('add_loop: starting add_loop_inherit ...', imp ='n')
         #inherit option
-        inh_opt_ngkpt = ['full', 'full_chg', 'full_nomag', 'occ', 'r1r2r3', 'remove_imp', 'replace_atoms', 'make_vacancy', 'antisite'] #inherit also ngkpt
+        inh_opt_ngkpt = ['full', 'full_chg', 'full_nomag', 'occ', 'r1r2r3', 'remove_imp', 'replace_atoms', 'make_vacancy', 'antisite', 'full_wave'] #inherit also ngkpt
         inh_opt_other = ['supercell', 'r2r3'] # do not inherit ngkpt
         # if inherit_option in inh_opt_ngkpt+inh_opt_other:
         omit_inh_opt = ['inherit_xred', 'continue']
         if inherit_option and inherit_option not in omit_inh_opt:
             
             if 'id_base_st_type' in inherit_args and inherit_args['id_base_st_type'] == 'init':
                 iti = it+'.init'
@@ -602,15 +602,16 @@
                 it_new = iti+'.'+suf
                 # print (it_new)
                 # sys.exit()
 
             elif inherit_option == 'make_vacancy':
                 it_new = iti+'.vac'
 
-
+            elif inherit_option == 'full_wave':
+                it_new = iti+'.ifw'
 
             if it_suffix: # add to default behaviour; make additional key, which can allow to override default behavior
                 it_new = it_new+'.'+it_suffix
                 it_suffix = None
 
 
 
@@ -1280,14 +1281,21 @@
                 pass
         if inherit_option  == 'optic':
             printlog('Copying WAVECAR ...', imp = 'y')
             if copy_to_server:
                 wrapper_cp_on_server(calc[id_base].path["output"].replace('WAVECAR'), header.project_path_cluster + '/' + calc[id].dir + '/', new_filename = 'WAVECAR')
             else:
                 pass
+        
+        if inherit_option  == 'full_wave':
+            printlog('Copying WAVECAR ...', imp = 'y')
+            if copy_to_server:
+                wrapper_cp_on_server(calc[id_base].path["output"].replace('OUTCAR','WAVECAR'), header.project_path_cluster + '/' + calc[id].dir + '/', new_filename = 'WAVECAR')
+            else:
+                pass
 
         if inherit_option  == 'band_hse':
             printlog('Copying WAVECAR ...', imp = 'y')
             if copy_to_server:
                 wrapper_cp_on_server(calc[id_base].path["output"].replace('WAVECAR'), header.project_path_cluster + '/' + calc[id].dir + '/', new_filename = 'WAVECAR')
             else:
                 pass
@@ -2226,14 +2234,18 @@
         # The file is copied in add_loop_finalize !!!
 
     elif inherit_type == "full_nomag":
         # printlog("Warning! final xred and xcart was used from OUTCAR and have low precision. Please use CONTCAR file \n");
         des = 'Fully inherited from the final state of '+cl_base.name+'; "magmom" set to [None]'
         st.magmom = [None]
 
+    elif inherit_type  == 'full_wave':
+
+        des = 'Fully inherited (including Wave file ) from the final state of '+cl_base.name
+
     elif inherit_type == "occ":
         des = 'Fully inherited from the final state of '+cl_base.name+'; occupation matrix is taken from '+calc_from_name
 
         printlog('Inherit option: "occ", reading occupation matrices from',calc_from_name)
         
         if not calc_from.occ_matrices:
             printlog('Error! calc_from.occ_matrices is empty')
```

### Comparing `siman-1.7.0/siman/calcul.py` & `siman-1.7.1/siman/calcul.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/calculators/aims.py` & `siman-1.7.1/siman/calculators/aims.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/calculators/gaussian.py` & `siman-1.7.1/siman/calculators/gaussian.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,24 +92,33 @@
 
         basis_set  = sp.get('basis_set')
         functional = sp.get('functional')
         job_type = sp.get('job_type')
         spin_multiplicity = sp.get('multiplicity')
         charge = sp.get('charge')
         SCRF = sp.get('SCRF')
+        chk = sp.get('chk')
         # route_parameters = None#{"SCF":"Tight"}
+        print(sp)
+        print('job_type', job_type)
         route_parameters = {job_type:''}
         if SCRF:
             route_parameters[SCRF] = ''
         mem = self.cluster.get('memory')
         if not mem:
             printlog('Warning! no memory limit in cluster description, I set default of 24GB')
             mem = 24
 
         link0_parameters = {'%NProcShared':self.cluster['corenum'], '%mem':str(mem)+'GB'}
+        if chk:
+            link0_parameters['%chk'] = str(chk)
+        
+        # print(functional)
+        # if not functional:
+            # printlog('Error! The set contains no functional, please provide!')
 
         inp = GaussianInput(self.init, basis_set = basis_set, charge = charge, spin_multiplicity = spin_multiplicity,
             functional = functional, route_parameters = route_parameters, 
             input_parameters = sp.get('optional'), link0_parameters = link0_parameters )
 
         inp.write_file(incar, cart_coords=True)
         # sys.exit()
```

### Comparing `siman-1.7.0/siman/calculators/qe.py` & `siman-1.7.1/siman/calculators/qe.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/calculators/vasp.py` & `siman-1.7.1/siman/calculators/vasp.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/calculators/vasp_old.py` & `siman-1.7.1/siman/calculators/vasp_old.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/chg/chg_func.py` & `siman-1.7.1/siman/chg/chg_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,10 +219,10 @@
         elst.append(dens/k_p**2 * st.vol)
         z_coord.append(n3/10)
 
 
     if plot:
         # print(z_coord, elst)
         fit_and_plot(a=(z_coord, elst, '-b'), xlabel = 'Z coordinate, $\AA$', 
-            ylabel = 'Potential, eV', filename = 'figs/'+st.id[0]+'_pot')
+            ylabel = 'Potential, eV', filename = 'figs/'+cl.id[0]+'_pot')
 
     return z_coord, elst
```

### Comparing `siman-1.7.0/siman/chg/vasputil_chgarith_module.py` & `siman-1.7.1/siman/chg/vasputil_chgarith_module.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/classes.py` & `siman-1.7.1/siman/classes.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/core/calculation.py` & `siman-1.7.1/siman/core/calculation.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 if header.pymatgen_flag:
     from pymatgen.io.cif import CifWriter
     from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
     from pymatgen.core.surface import Slab
     from pymatgen.core.composition import Composition
 
 
-from siman.header import printlog
+from siman.header import printlog,runBash
 
 from siman import set_functions
 # from siman.small_functions import return_xred, makedir, angle, is_string_like, cat_files, grep_file, red_prec, list2string, is_list_like, b2s, calc_ngkpt, setting_sshpass
 from siman.small_functions import return_xred, makedir, angle, is_string_like, cat_files, grep_file, red_prec, list2string, is_list_like, b2s, calc_ngkpt, setting_sshpass
 from siman.functions import (read_vectors, read_list, words, read_string,
      element_name_inv, invert, calculate_voronoi, 
     get_from_server, push_to_server, run_on_server, smoother, file_exists_on_server, check_output)
@@ -539,16 +539,21 @@
         # make entry with new id
         clcopy = copy.deepcopy(self)
         if id is not None:
             header.db[id] = clcopy
             header.db[id].id = id
         return clcopy
 
-    def jmol(self, *args, **kwargs):
-        self.end.jmol(*args, **kwargs)
+    def jmol(self, r = 0, *args, **kwargs):
+        if r == 5:
+            self.get_file('*XDATCAR')
+            filename = self.path['xdatcar']
+            runBash(header.PATH2OVITO+' '+filename, detached = True)
+        else:
+            self.end.jmol(r=r,*args, **kwargs)
     def poscar(self):
         self.end.write_poscar()
 
     def me(self):
         self.end.printme()
     def gmt(self, *args, **kwargs):
         return self.end.get_mag_tran(*args, **kwargs)
@@ -1254,14 +1259,17 @@
                 path_to_file = os.path.dirname(self.path['output']) +'/'+ filetype
         if 'CHGCAR' in filetype:
             self.path['chgcar'] = path_to_file
             self.path['charge'] = path_to_file
         elif 'xml' in filetype:
             self.path['xml'] = path_to_file
 
+        elif 'XDATCAR' in filetype:
+            self.path['xdatcar'] = path_to_file
+
 
         # print(self.cluster_address)
         # print(self.project_path_cluster+'/')
         # sys.exit()
         if hasattr(self, 'cluster'):
             address = self.cluster['address']
         if header.override_cluster_address:
@@ -1364,14 +1372,15 @@
         INPUT:
             ise (str) - name of new set available in header.varset
 
             iopt (str) - inherit_option
                 'full_nomag' - full without magmom
                 'full' - full with magmom
                 'full_chg' - full with magmom and including chg file
+                'full_wave' - full with magmom and including wavecar
             
             up (str) - update key transferred to add_loop and res_loop;
                 'up1' - create new calculation if not exist
                 'up2' - recreate new calculation overwriting old; for reading results redownload output files
 
             vers (list of int) - list of version for which the inheritance is done
 
@@ -1404,15 +1413,16 @@
 
         if iopt == 'full_nomag':
             suffix = '.ifn'
         if iopt == 'full':
             suffix = '.if'
         if iopt == 'full_chg':
             suffix = '.ifc'
-
+        if iopt == 'full_wave':
+            suffix = '.ifw'
 
 
 
         if 'it_suffix' in kwargs:
             it_suffix = '.'+kwargs['it_suffix']
             it_suffix_del = False
         else:
```

### Comparing `siman-1.7.0/siman/core/calculation_old.py` & `siman-1.7.1/siman/core/calculation_old.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/core/cluster_batch_script.py` & `siman-1.7.1/siman/core/cluster_batch_script.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/core/cluster_run_script.py` & `siman-1.7.1/siman/core/cluster_run_script.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/core/molecule.py` & `siman-1.7.1/siman/core/molecule.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/core/structure.py` & `siman-1.7.1/siman/core/structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,20 +270,38 @@
         
         """
         st = copy.deepcopy(self)
         r = copy.deepcopy(st.rprimd)
 
         st.rprimd[i1_r] = r[i2_r]
         st.rprimd[i2_r] = r[i1_r]
-
+        
         st.update_xred()
 
         return st
 
+    def exchange_axes_with_atoms(self, i1_r, i2_r):
+        """
+        
+        """
+        st = copy.deepcopy(self)
+        xc = copy.deepcopy(self.xcart)
+        xr = copy.deepcopy(self.xred)
+        r = copy.deepcopy(self.rprimd)
+
+        for i in range(0,st.natom):
+            st.xcart[i][i1_r] = xc[i][i2_r] 
+            st.xcart[i][i2_r] = xc[i][i1_r] 
 
+            st.xred[i][i1_r] = xr[i][i2_r] 
+            st.xred[i][i2_r] = xr[i][i1_r] 
+
+        # st.update_xred()
+
+        return st
 
 
     def get_volume(self):
         self.vol = np.dot( self.rprimd[0], np.cross(self.rprimd[1], self.rprimd[2])  ); #volume
         return self.vol
 
     def get_recip(self):
@@ -740,15 +758,15 @@
                 st.znucl.append(z)
                 # nznucl.append(0)
                 unique.append(el)
             st.typat.append(types[el])
         
         st.get_nznucl()
 
-        # print(st.ntypat, st.typat, st.nznucl, st.znucl)
+        print(st.ntypat, st.typat, st.nznucl, st.znucl)
 
         return st
 
     def update_from_pymatgen(self, stpm):
         """
         stpm - pymatgen structure
         update the current structure from pymatgen structure
@@ -1714,16 +1732,17 @@
                     printlog('Error! Check *order* list')
 
                 if el_i == el:
                     # print(el)
                     typat.append(t)
                     xcart.append(st.xcart[i])
                     old_numbers.append(i)
-                    if None not in st.magmom:
-                        magmom.append(st.magmom[i])
+                    if st.magmom != []:
+                        if None not in st.magmom:
+                            magmom.append(st.magmom[i])
             t+=1
 
         if len(magmom) == 0:
             magmom = [None]
 
         st.old_numbers = old_numbers
         st.xcart = xcart
@@ -3905,14 +3924,15 @@
         shift (list) - shift vector  in reduced coordinates
         r (int ) - parameter
             0 - open POSCAR
             1 - open OUTCAR to see optimization steps
             2 - open mcif to see magnetic moments
             3 - xyz
             4 - open mcif to see magnetic moments only on oxygen, other magmoms are set as zero
+            5 - open XDATCAR
         show_voids (bool) - replace voids (z = 300) with Po to visualize them
         rep  (list 3*int) - replicate along vectors
         program - 
             'jmol'
             'vesta'
         
         """
@@ -3938,31 +3958,42 @@
         elif r == 4:
             for i in range(0, len(st.xcart)):
                 if st.get_el_name(i) != 'O':
                     st.magmom[i] = 0
                 else:
                     st.magmom[i] *= 5
             filename = st.write_cif(mcif = 1)
+        elif r == 5:
+            filename = None
+            ''
         else:
             filename = st.write_poscar(vasp5 = 1)
         
         # print(r, filename)
         # sys.exit()
-        if 'jmol' in program :
-            # runBash(header.PATH2JMOL+' -j \"background white\" '+filename, detached = True)
-            runBash(header.PATH2JMOL+' '+filename, detached = True)
-        elif 'vesta' in program:
-            runBash(header.PATH2VESTA+' '+filename, detached = True)
+        if filename:
+            if 'jmol' in program :
+                runBash(header.PATH2JMOL+' -j \"background white\" '+filename, detached = True)
+                # runBash(header.PATH2JMOL+' '+filename, detached = True)
+            elif 'vesta' in program:
+                runBash(header.PATH2VESTA+' '+filename, detached = True)
+            elif 'ovito' in program:
+                runBash(header.PATH2VESTA+' '+filename, detached = True)
 
         return
 
     def vesta(self, *args, **kwargs):
         kwargs['program'] = 'vesta'
         self.jmol(*args, **kwargs)
 
+    def ovito(self, *args, **kwargs):
+        kwargs['program'] = 'ovito'
+        self.jmol(*args, **kwargs)
+
+
 
 
     @property
     def vlen(self):
         #return vector lengths
         r = self.rprimd
         n = np.linalg.norm
```

### Comparing `siman-1.7.0/siman/database.py` & `siman-1.7.1/siman/database.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/default_project_conf.py` & `siman-1.7.1/siman/default_project_conf.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/dev_functions.py` & `siman-1.7.1/siman/dev_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/dos_functions.py` & `siman-1.7.1/siman/dos_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/fit_hex.py` & `siman-1.7.1/siman/fit_hex.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/functions.py` & `siman-1.7.1/siman/functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/geo.py` & `siman-1.7.1/siman/geo.py`

 * *Files 1% similar despite different names*

```diff
@@ -542,15 +542,15 @@
     # print 'Structure is replicated; now', st.natom,'atoms' 
     return st
 
 
 
 def local_surrounding(x_central, st, n_neighbours, control = 'sum', periodic = False, only_elements = None, only_numbers = None, round_flag = 1):
     """
-    Return list of distances to n closest atoms around central atom. (By defauld sum of distances)
+    Return list of distances to n closest atoms around central atom. (By default sum of distances)
     
     Input:
     - x_central - cartesian coordinates of central atom; vector
     - st - structure with xcart list of coordinates of all atoms in system
     - n_neighbours - number of needed closest neighbours
 
     - control - type of output; 
@@ -1009,15 +1009,15 @@
 
 
 
 def create_supercell(st, mul_matrix, test_overlap = False, mp = 4, bound = 0.01, mul = (1,1,1), silent = 0, test_natom = 1): 
 
     """ 
     st (Structure) -  
-    mul_matrix (3x3 ndarray of int) - for example created by *ortho_    vec()* 
+    mul_matrix (3x3 ndarray of int) - for example created by *ortho_vec()* 
 
     mul - multiply mul matrix - allows to choose fractions of new vectors
 
     bound (float) - shift (A) allows to correctly account atoms on boundaries
     mp    (int)  include additionall atoms before cutting supecell
     test_natom (bool) - test if the number of atoms is correct after transformation
     test_overlap (bool) - check if atoms are overlapping -  quite slow
@@ -2785,15 +2785,18 @@
     conf_i - [0,1,2] - list of ads configuration numbers
             key 'all' means all constructed configurations
     under_atom return configuration with ads atom strongly under me and neme atoms in surface
     """
 
 
 
-    from pymatgen import Structure, Lattice, Molecule
+    # from pymatgen import Structure, Lattice, Molecule
+    from pymatgen.core import Lattice, Structure
+    from pymatgen.core.structure import Molecule
+
     from pymatgen.analysis.adsorption import AdsorbateSiteFinder
     from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
     from pymatgen.io.vasp.inputs import Poscar
 
     pm = st.convert2pymatgen()
     # pm = st
     asf_pm = AdsorbateSiteFinder(pm)
```

### Comparing `siman-1.7.0/siman/header.py` & `siman-1.7.1/siman/header.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,16 +201,17 @@
 
     import importlib.util, sys
     spec = importlib.util.spec_from_file_location('project_conf', filename)
     project_conf = importlib.util.module_from_spec(spec)
 
     spec.loader.exec_module(project_conf)
     # print(dir(project_conf))
+
     config_vars = ['MEM_CPU','CIF2CELL', 'DEFAULT_CLUSTER', 'EXCLUDE_NODES', 
-    'NEW_BATCH', 'PATH2ARCHIVE', 'PATH2DATABASE', 'PATH2JMOL', 'PATH2VESTA', 'PATH2NEBMAKE', 
+    'NEW_BATCH', 'PATH2ARCHIVE', 'PATH2DATABASE', 'PATH2JMOL', 'PATH2VESTA','PATH2OVITO','PATH2NEBMAKE', 
     'PATH2PHONOPY', 'PATH2POTENTIALS', 'PATH2PROJECT', 'PBS_PROCS', 
     'RAMDISK', 'SIMAN_WEB', 'WALLTIME_LIMIT', 
     'geo_folder', 'path_to_images', 'path_to_paper', 
     'path_to_wrapper', 'pmgkey', 'reorganize', 'CLUSTERS', 
     'PATH2SHELVE_DBSUP', 'PATH2SHELVE_DB', 'PATH2HISTORYFILE', 'AUTO_UPDATE_DB', 'warnings', ]
 
     for var in config_vars:
```

### Comparing `siman-1.7.0/siman/impurity.py` & `siman-1.7.1/siman/impurity.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/inout.py` & `siman-1.7.1/siman/inout.py`

 * *Files 0% similar despite different names*

```diff
@@ -1418,14 +1418,15 @@
         self.potcar_lines = []
         self.stress = None
         self.extpress = 0
 
         self.intstress = None
         spin_polarized = None
         ifmaglist = None
+        self.mags_step = []
         for line in outcarlines:
 
 
             #Check bands
 
             # if 'band No.' in line:
             #     kpoint = float(outcarlines[i_line-1].split()[1])
@@ -1841,14 +1842,15 @@
                     tot_mag_by_atoms.append(np.array(mags))#[ifmaglist])
                     # print(ifmaglist)
                     tot_mag_by_mag_atoms.append(np.array(mags)[ifmaglist])
                 # print tot_mag_by_atoms
                 # magnetic_elements
                 # ifmaglist
                 # self.tot_mag_by_atoms = tot_mag_by_atoms
+                self.mags_step.append(mags)
 
 
 
             if 'LDAUU' in line:
                 ldauu = line
 
 
@@ -1890,14 +1892,15 @@
                         i+=1
                         try:
                             line = outcarlines[i_line+i]
                         except:
                             break
                         if 'f  =' in line:
                             freq.append(float(line.split()[3]) ) #THz
+
                         elif 'f/i=' in line:
                             freq.append(-float(line.split()[2]) ) #THz
                             # print(line)
 
                     self.freq = freq
```

### Comparing `siman-1.7.0/siman/kpoints_functions.py` & `siman-1.7.1/siman/kpoints_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/mat_prop/mat_prop.py` & `siman-1.7.1/siman/mat_prop/mat_prop.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/matproj_functions.py` & `siman-1.7.1/siman/matproj_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/monte.py` & `siman-1.7.1/siman/monte.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/monte_functions.py` & `siman-1.7.1/siman/monte_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/neb.py` & `siman-1.7.1/siman/neb.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/pairs.py` & `siman-1.7.1/siman/pairs.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/picture_functions.py` & `siman-1.7.1/siman/picture_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/plot_functions.py` & `siman-1.7.1/siman/plot_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/polaron.py` & `siman-1.7.1/siman/polaron.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/polaron_hop.py` & `siman-1.7.1/siman/polaron_hop.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/polaron_mod.py` & `siman-1.7.1/siman/polaron_mod.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/project_funcs.py` & `siman-1.7.1/siman/project_funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4712,15 +4712,15 @@
 
     return
 
 
 
 
 def run_OMC_sol(cl_defect, cl_ideal, defect_atoms = None, defect_occ = None, ise = None, suf = '', up = 0, gmt = 0, soluted_atom = None, e_s = None, 
-    add_loop_dic = None, cluster = 'cee-omc'):
+    add_loop_dic = {}, cluster = 'cee-omc'):
     """
     
     Optionally for each defect atom an occupation matrix can be provided
 
     cl_defect - calculation for cell with defect
     cl_ideal - calculation for commensurate reference cell
     defect_atoms - list of atoms in cl_defect which are considered defective
```

### Comparing `siman-1.7.0/siman/properties_2d.py` & `siman-1.7.1/siman/properties_2d.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/properties_energy.py` & `siman-1.7.1/siman/properties_energy.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/properties_lattice.py` & `siman-1.7.1/siman/properties_lattice.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/set_functions.py` & `siman-1.7.1/siman/set_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,17 @@
 'VDW_C6',
 'VDW_R0',
 'NWRITE',
 'MAGATOM',
 'DOSTATIC',
 'IWAVPRE',
 'MIXPRE',
-
+'LANGEVIN_GAMMA_L',
+'LANGEVIN_GAMMA',
+'PMASS'
 ]
 vasp_keys = vasp_electronic_keys+vasp_ionic_keys+vasp_other_keys
 
 siman_keys = [
 'universal', # universal paramater with any content
 'u_ramping_region', #deprecated
 'u_ramping_nstep', #number of u ramping steps
@@ -221,14 +223,15 @@
 'functional',
 'basis_set',
 'job_type',
 'optional',
 'multiplicity',
 'charge',
 'SCRF',
+'chk',
 ]
 
 
 def read_vasp_sets(user_vasp_sets, override_global = False):
     """
     Read user sets for different calculators and add them to project database
     Works not only for VASP but other codes as well, such as Gaussian
```

### Comparing `siman-1.7.0/siman/simanrc.py` & `siman-1.7.1/siman/simanrc.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/small_functions.py` & `siman-1.7.1/siman/small_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/structure_functions.py` & `siman-1.7.1/siman/structure_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/table_functions.py` & `siman-1.7.1/siman/table_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/thermo.py` & `siman-1.7.1/siman/thermo.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman/workflow_utilities.py` & `siman-1.7.1/siman/workflow_utilities.py`

 * *Files identical despite different names*

### Comparing `siman-1.7.0/siman.egg-info/PKG-INFO` & `siman-1.7.1/siman.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siman
-Version: 1.7.0
+Version: 1.7.1
 Summary: Manager for DFT calculations
 Home-page: https://github.com/dimonaks/siman
 Author: Dmitry Aksenov
 Author-email: dimonaks@gmail.com
 License: GPL
 Keywords: DFT VASP Density Functional Theory NEB DFT+U PAW GGA Monte-Carlo
 Platform: UNKNOWN
```

### Comparing `siman-1.7.0/siman.egg-info/SOURCES.txt` & `siman-1.7.1/siman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

