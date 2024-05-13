# Comparing `tmp/midas-mosaik-1.2.1.tar.gz` & `tmp/midas-mosaik-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midas-mosaik-1.2.1.tar", last modified: Tue Apr 16 06:54:14 2024, max compression
+gzip compressed data, was "midas-mosaik-1.2.2.tar", last modified: Mon May 13 13:38:32 2024, max compression
```

## Comparing `midas-mosaik-1.2.1.tar` & `midas-mosaik-1.2.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:54:14.720863 midas-mosaik-1.2.1/
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     7648 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/LICENSE
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      210 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/MANIFEST.in
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     6013 2024-04-16 06:54:14.720863 midas-mosaik-1.2.1/PKG-INFO
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     5034 2024-04-16 06:35:27.000000 midas-mosaik-1.2.1/README.md
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)        5 2024-04-16 06:53:07.000000 midas-mosaik-1.2.1/VERSION
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:54:14.714196 midas-mosaik-1.2.1/docs/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      634 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/docs/Makefile
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     2195 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/docs/conf.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)    10624 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/docs/configuration.rst
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     2009 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/docs/getting_started.rst
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      517 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/docs/index.rst
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     6504 2023-10-17 09:34:59.000000 midas-mosaik-1.2.1/docs/installation.rst
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      795 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/docs/make.bat
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:54:14.717530 midas-mosaik-1.2.1/docs/modules/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     8610 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/docs/modules/comdata.rst
--rw-r--r--   0 sbalduin  (1000) wheel      (998)  3895886 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/docs/modules/dlp_season.png
--rw-r--r--   0 sbalduin  (1000) wheel      (998)    10891 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/docs/modules/dlpdata.rst
--rw-r--r--   0 sbalduin  (1000) wheel      (998)   228112 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/docs/modules/facilitys.png
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      420 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/docs/modules/index.rst
--rw-r--r--   0 sbalduin  (1000) wheel      (998)    11576 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/docs/modules/powergrid.rst
--rw-r--r--   0 sbalduin  (1000) wheel      (998)   703409 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/docs/modules/smart_nord_lands.png
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     8750 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/docs/modules/sndata.rst
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     4868 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/docs/modules/store.rst
--rw-r--r--   0 sbalduin  (1000) wheel      (998)    86633 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/docs/modules/time_weather.png
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     6048 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/docs/modules/timesim.rst
--rw-r--r--   0 sbalduin  (1000) wheel      (998)   195881 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/docs/modules/two_grid_example-Powergrid__0_0-buses_vmpu.png
--rw-r--r--   0 sbalduin  (1000) wheel      (998)   213876 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/docs/modules/two_grid_example-Powergrid__1_0-buses_vmpu.png
--rw-r--r--   0 sbalduin  (1000) wheel      (998)   205192 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/docs/mymidasdb-Powergrid__0_0-buses_vmpu.png
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)    17182 2023-10-18 11:13:52.000000 midas-mosaik-1.2.1/docs/next_steps.rst
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:54:14.710863 midas-mosaik-1.2.1/midas/
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:54:14.717530 midas-mosaik-1.2.1/midas/api/
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      218 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/midas/api/__init__.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     5668 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/midas/api/fnc_analyze.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)    13756 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/midas/api/fnc_configure.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     4257 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/midas/api/fnc_download.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      470 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/midas/api/fnc_list.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     1873 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/midas/api/fnc_run.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     9478 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/midas/api/midasctl.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:54:14.717530 midas-mosaik-1.2.1/midas/scenario/
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)       50 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/midas/scenario/__init__.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:54:14.717530 midas-mosaik-1.2.1/midas/scenario/config/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     5701 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/midas/scenario/config/benchmark.yml
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     7730 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/midas/scenario/config/bremerhaven.yml
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1357 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/midas/scenario/config/constrainted_grids.yml
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     1739 2024-04-08 06:46:37.000000 midas-mosaik-1.2.1/midas/scenario/config/four_bus.yml
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1914 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/midas/scenario/config/grid_example.yml
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     3453 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/midas/scenario/config/midaslv.yml
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     3725 2024-03-19 15:44:34.000000 midas-mosaik-1.2.1/midas/scenario/config/midasmv.yml
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      874 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/midas/scenario/config/no_grid.yml
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      640 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/midas/scenario/config/sbrural3.yml
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     8865 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/midas/scenario/configurator.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)    13631 2023-07-14 11:51:02.000000 midas-mosaik-1.2.1/midas/scenario/scenario.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:54:14.717530 midas-mosaik-1.2.1/midas_mosaik.egg-info/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     6013 2024-04-16 06:54:14.000000 midas-mosaik-1.2.1/midas_mosaik.egg-info/PKG-INFO
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1516 2024-04-16 06:54:14.000000 midas-mosaik-1.2.1/midas_mosaik.egg-info/SOURCES.txt
--rw-r--r--   0 sbalduin  (1000) wheel      (998)        1 2024-04-16 06:54:14.000000 midas-mosaik-1.2.1/midas_mosaik.egg-info/dependency_links.txt
--rw-r--r--   0 sbalduin  (1000) wheel      (998)       53 2024-04-16 06:54:14.000000 midas-mosaik-1.2.1/midas_mosaik.egg-info/entry_points.txt
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      366 2024-04-16 06:54:14.000000 midas-mosaik-1.2.1/midas_mosaik.egg-info/requires.txt
--rw-r--r--   0 sbalduin  (1000) wheel      (998)        6 2024-04-16 06:54:14.000000 midas-mosaik-1.2.1/midas_mosaik.egg-info/top_level.txt
--rw-r--r--   0 sbalduin  (1000) wheel      (998)       38 2024-04-16 06:54:14.720863 midas-mosaik-1.2.1/setup.cfg
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     2161 2024-04-16 06:52:16.000000 midas-mosaik-1.2.1/setup.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:54:14.710863 midas-mosaik-1.2.1/tests/
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:54:14.717530 midas-mosaik-1.2.1/tests/system/
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      129 2023-09-22 07:38:16.000000 midas-mosaik-1.2.1/tests/system/debug_script.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:54:14.710863 midas-mosaik-1.2.1/tests/unit/
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:54:14.717530 midas-mosaik-1.2.1/tests/unit/scenario/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     2135 2023-07-12 12:35:52.000000 midas-mosaik-1.2.1/tests/unit/scenario/test_configurator.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-05-13 13:38:32.047852 midas-mosaik-1.2.2/
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     7648 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/LICENSE
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      210 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/MANIFEST.in
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     6013 2024-05-13 13:38:32.047852 midas-mosaik-1.2.2/PKG-INFO
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     5034 2024-04-16 06:35:27.000000 midas-mosaik-1.2.2/README.md
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)        5 2024-05-13 12:46:59.000000 midas-mosaik-1.2.2/VERSION
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-05-13 13:38:32.041185 midas-mosaik-1.2.2/docs/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      634 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/docs/Makefile
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     2195 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/docs/conf.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)    10624 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/docs/configuration.rst
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     2009 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/docs/getting_started.rst
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      517 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/docs/index.rst
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     6504 2023-10-17 09:34:59.000000 midas-mosaik-1.2.2/docs/installation.rst
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      795 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/docs/make.bat
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-05-13 13:38:32.044518 midas-mosaik-1.2.2/docs/modules/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     8610 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/docs/modules/comdata.rst
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)  3895886 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/docs/modules/dlp_season.png
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)    10891 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/docs/modules/dlpdata.rst
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)   228112 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/docs/modules/facilitys.png
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      420 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/docs/modules/index.rst
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)    11576 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/docs/modules/powergrid.rst
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)   703409 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/docs/modules/smart_nord_lands.png
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     8750 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/docs/modules/sndata.rst
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     4868 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/docs/modules/store.rst
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)    86633 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/docs/modules/time_weather.png
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     6048 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/docs/modules/timesim.rst
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)   195881 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/docs/modules/two_grid_example-Powergrid__0_0-buses_vmpu.png
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)   213876 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/docs/modules/two_grid_example-Powergrid__1_0-buses_vmpu.png
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)   205192 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/docs/mymidasdb-Powergrid__0_0-buses_vmpu.png
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)    17182 2023-10-18 11:13:52.000000 midas-mosaik-1.2.2/docs/next_steps.rst
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-05-13 13:38:32.041185 midas-mosaik-1.2.2/midas/
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-05-13 13:38:32.044518 midas-mosaik-1.2.2/midas/api/
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      218 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/midas/api/__init__.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     5668 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/midas/api/fnc_analyze.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)    13756 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/midas/api/fnc_configure.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     4257 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/midas/api/fnc_download.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      470 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/midas/api/fnc_list.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     1873 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/midas/api/fnc_run.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     9478 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/midas/api/midasctl.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-05-13 13:38:32.044518 midas-mosaik-1.2.2/midas/scenario/
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)       50 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/midas/scenario/__init__.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-05-13 13:38:32.044518 midas-mosaik-1.2.2/midas/scenario/config/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     5701 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/midas/scenario/config/benchmark.yml
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     7730 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/midas/scenario/config/bremerhaven.yml
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1357 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/midas/scenario/config/constrainted_grids.yml
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     1739 2024-04-08 06:46:37.000000 midas-mosaik-1.2.2/midas/scenario/config/four_bus.yml
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1914 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/midas/scenario/config/grid_example.yml
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     3453 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/midas/scenario/config/midaslv.yml
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     3725 2024-03-19 15:44:34.000000 midas-mosaik-1.2.2/midas/scenario/config/midasmv.yml
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      874 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/midas/scenario/config/no_grid.yml
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      640 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/midas/scenario/config/sbrural3.yml
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     8865 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/midas/scenario/configurator.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)    13638 2024-05-13 12:46:09.000000 midas-mosaik-1.2.2/midas/scenario/scenario.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-05-13 13:38:32.044518 midas-mosaik-1.2.2/midas_mosaik.egg-info/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     6013 2024-05-13 13:38:32.000000 midas-mosaik-1.2.2/midas_mosaik.egg-info/PKG-INFO
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1516 2024-05-13 13:38:32.000000 midas-mosaik-1.2.2/midas_mosaik.egg-info/SOURCES.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)        1 2024-05-13 13:38:32.000000 midas-mosaik-1.2.2/midas_mosaik.egg-info/dependency_links.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)       53 2024-05-13 13:38:32.000000 midas-mosaik-1.2.2/midas_mosaik.egg-info/entry_points.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      362 2024-05-13 13:38:32.000000 midas-mosaik-1.2.2/midas_mosaik.egg-info/requires.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)        6 2024-05-13 13:38:32.000000 midas-mosaik-1.2.2/midas_mosaik.egg-info/top_level.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)       38 2024-05-13 13:38:32.047852 midas-mosaik-1.2.2/setup.cfg
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     2157 2024-05-13 13:29:42.000000 midas-mosaik-1.2.2/setup.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-05-13 13:38:32.041185 midas-mosaik-1.2.2/tests/
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-05-13 13:38:32.044518 midas-mosaik-1.2.2/tests/system/
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      129 2023-09-22 07:38:16.000000 midas-mosaik-1.2.2/tests/system/debug_script.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-05-13 13:38:32.041185 midas-mosaik-1.2.2/tests/unit/
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-05-13 13:38:32.044518 midas-mosaik-1.2.2/tests/unit/scenario/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     2135 2023-07-12 12:35:52.000000 midas-mosaik-1.2.2/tests/unit/scenario/test_configurator.py
```

### Comparing `midas-mosaik-1.2.1/LICENSE` & `midas-mosaik-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/PKG-INFO` & `midas-mosaik-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas-mosaik
-Version: 1.2.1
+Version: 1.2.2
 Summary: MultI-DomAin test Scenario for smart grid co-simulation.
 Home-page: https://gitlab.com/midas-mosaik/midas
 Author: Stephan Balduin
 Author-email: stephan.balduin@offis.de
 License: LGPL
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `midas-mosaik-1.2.1/README.md` & `midas-mosaik-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/docs/Makefile` & `midas-mosaik-1.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/docs/conf.py` & `midas-mosaik-1.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/docs/configuration.rst` & `midas-mosaik-1.2.2/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/docs/getting_started.rst` & `midas-mosaik-1.2.2/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/docs/index.rst` & `midas-mosaik-1.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/docs/installation.rst` & `midas-mosaik-1.2.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/docs/make.bat` & `midas-mosaik-1.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/docs/modules/comdata.rst` & `midas-mosaik-1.2.2/docs/modules/comdata.rst`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/docs/modules/dlp_season.png` & `midas-mosaik-1.2.2/docs/modules/dlp_season.png`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/docs/modules/dlpdata.rst` & `midas-mosaik-1.2.2/docs/modules/dlpdata.rst`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/docs/modules/facilitys.png` & `midas-mosaik-1.2.2/docs/modules/facilitys.png`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/docs/modules/powergrid.rst` & `midas-mosaik-1.2.2/docs/modules/powergrid.rst`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/docs/modules/smart_nord_lands.png` & `midas-mosaik-1.2.2/docs/modules/smart_nord_lands.png`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/docs/modules/sndata.rst` & `midas-mosaik-1.2.2/docs/modules/sndata.rst`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/docs/modules/store.rst` & `midas-mosaik-1.2.2/docs/modules/store.rst`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/docs/modules/time_weather.png` & `midas-mosaik-1.2.2/docs/modules/time_weather.png`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/docs/modules/timesim.rst` & `midas-mosaik-1.2.2/docs/modules/timesim.rst`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/docs/modules/two_grid_example-Powergrid__0_0-buses_vmpu.png` & `midas-mosaik-1.2.2/docs/modules/two_grid_example-Powergrid__0_0-buses_vmpu.png`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/docs/modules/two_grid_example-Powergrid__1_0-buses_vmpu.png` & `midas-mosaik-1.2.2/docs/modules/two_grid_example-Powergrid__1_0-buses_vmpu.png`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/docs/mymidasdb-Powergrid__0_0-buses_vmpu.png` & `midas-mosaik-1.2.2/docs/mymidasdb-Powergrid__0_0-buses_vmpu.png`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/docs/next_steps.rst` & `midas-mosaik-1.2.2/docs/next_steps.rst`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/midas/api/fnc_analyze.py` & `midas-mosaik-1.2.2/midas/api/fnc_analyze.py`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/midas/api/fnc_configure.py` & `midas-mosaik-1.2.2/midas/api/fnc_configure.py`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/midas/api/fnc_download.py` & `midas-mosaik-1.2.2/midas/api/fnc_download.py`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/midas/api/fnc_run.py` & `midas-mosaik-1.2.2/midas/api/fnc_run.py`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/midas/api/midasctl.py` & `midas-mosaik-1.2.2/midas/api/midasctl.py`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/midas/scenario/config/benchmark.yml` & `midas-mosaik-1.2.2/midas/scenario/config/benchmark.yml`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/midas/scenario/config/bremerhaven.yml` & `midas-mosaik-1.2.2/midas/scenario/config/bremerhaven.yml`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/midas/scenario/config/constrainted_grids.yml` & `midas-mosaik-1.2.2/midas/scenario/config/constrainted_grids.yml`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/midas/scenario/config/four_bus.yml` & `midas-mosaik-1.2.2/midas/scenario/config/four_bus.yml`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/midas/scenario/config/grid_example.yml` & `midas-mosaik-1.2.2/midas/scenario/config/grid_example.yml`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/midas/scenario/config/midaslv.yml` & `midas-mosaik-1.2.2/midas/scenario/config/midaslv.yml`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/midas/scenario/config/midasmv.yml` & `midas-mosaik-1.2.2/midas/scenario/config/midasmv.yml`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/midas/scenario/config/no_grid.yml` & `midas-mosaik-1.2.2/midas/scenario/config/no_grid.yml`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/midas/scenario/config/sbrural3.yml` & `midas-mosaik-1.2.2/midas/scenario/config/sbrural3.yml`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/midas/scenario/configurator.py` & `midas-mosaik-1.2.2/midas/scenario/configurator.py`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/midas/scenario/scenario.py` & `midas-mosaik-1.2.2/midas/scenario/scenario.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
 import logging
 import os
 import pickle
 from dataclasses import dataclass, field
-from distutils.util import strtobool
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import mosaik
 import numpy as np
+
+from midas.util.dict_util import strtobool
 from midas.util.runtime_config import RuntimeConfig
 from midas.util.upgrade_module import UpgradeModule
 
 LOG = logging.getLogger(__name__)
 
 
 class Scenario:
```

### Comparing `midas-mosaik-1.2.1/midas_mosaik.egg-info/PKG-INFO` & `midas-mosaik-1.2.2/midas_mosaik.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas-mosaik
-Version: 1.2.1
+Version: 1.2.2
 Summary: MultI-DomAin test Scenario for smart grid co-simulation.
 Home-page: https://gitlab.com/midas-mosaik/midas
 Author: Stephan Balduin
 Author-email: stephan.balduin@offis.de
 License: LGPL
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `midas-mosaik-1.2.1/midas_mosaik.egg-info/SOURCES.txt` & `midas-mosaik-1.2.2/midas_mosaik.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.2.1/setup.py` & `midas-mosaik-1.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 install_requirements = [
     "click",
     "mosaik",
     "mosaik-api",
     "midas-util>=1.1.2",
     "midas-comdata>=1.0.0rc5",
     "midas-dlpdata>=1.0.0rc6",
-    "midas-goa>=1.0.0rc6",
-    "midas-powergrid>=1.0.10",
+    "midas-goa>=1.0.0",
+    "midas-powergrid>=1.1.0",
     "midas-pwdata>=1.0.0",
     "midas-sbdata>=1.0.1",
     "midas-sndata>=1.0.2",
-    "midas-store>=1.0.0",
+    "midas-store>=1.0.1",
     "midas-timesim>=1.0.0rc5",
     "midas-weather>=1.1.4",
     "pysimmods>=0.11.2",
     "ruamel.yaml",
 ]
 
 development_requirements = [
```

### Comparing `midas-mosaik-1.2.1/tests/unit/scenario/test_configurator.py` & `midas-mosaik-1.2.2/tests/unit/scenario/test_configurator.py`

 * *Files identical despite different names*

