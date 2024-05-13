# Comparing `tmp/ScopeSim_Templates-0.5.1.tar.gz` & `tmp/scopesim_templates-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ScopeSim_Templates-0.5.1.tar", last modified: Tue Feb  6 20:44:08 2024, max compression
+gzip compressed data, was "scopesim_templates-0.5.2.tar", last modified: Mon May 13 20:42:15 2024, max compression
```

## Comparing `ScopeSim_Templates-0.5.1.tar` & `scopesim_templates-0.5.2.tar`

### file list

```diff
@@ -1,68 +1,72 @@
-drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2024-02-06 20:44:08.664830 ScopeSim_Templates-0.5.1/
--rw-rw-r--   0 hugo      (1000) hugo      (1000)    35149 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/LICENSE
--rw-rw-r--   0 hugo      (1000) hugo      (1000)      256 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/MANIFEST.in
--rw-r--r--   0 hugo      (1000) hugo      (1000)     1889 2024-02-06 20:44:08.664830 ScopeSim_Templates-0.5.1/PKG-INFO
--rw-rw-r--   0 hugo      (1000) hugo      (1000)     4072 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/README.md
-drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2024-02-06 20:44:08.660830 ScopeSim_Templates-0.5.1/ScopeSim_Templates.egg-info/
--rw-r--r--   0 hugo      (1000) hugo      (1000)     1889 2024-02-06 20:44:08.000000 ScopeSim_Templates-0.5.1/ScopeSim_Templates.egg-info/PKG-INFO
--rw-rw-r--   0 hugo      (1000) hugo      (1000)     2215 2024-02-06 20:44:08.000000 ScopeSim_Templates-0.5.1/ScopeSim_Templates.egg-info/SOURCES.txt
--rw-rw-r--   0 hugo      (1000) hugo      (1000)        1 2024-02-06 20:44:08.000000 ScopeSim_Templates-0.5.1/ScopeSim_Templates.egg-info/dependency_links.txt
--rw-rw-r--   0 hugo      (1000) hugo      (1000)      371 2024-02-06 20:44:08.000000 ScopeSim_Templates-0.5.1/ScopeSim_Templates.egg-info/requires.txt
--rw-rw-r--   0 hugo      (1000) hugo      (1000)       29 2024-02-06 20:44:08.000000 ScopeSim_Templates-0.5.1/ScopeSim_Templates.egg-info/top_level.txt
-drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2024-02-06 20:44:08.648830 ScopeSim_Templates-0.5.1/docs/
--rw-rw-r--   0 hugo      (1000) hugo      (1000)     8582 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/docs/conf.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)     1682 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/pyproject.toml
-drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2024-02-06 20:44:08.652830 ScopeSim_Templates-0.5.1/scopesim_templates/
--rw-rw-r--   0 hugo      (1000) hugo      (1000)      918 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/__init__.py
-drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2024-02-06 20:44:08.652830 ScopeSim_Templates-0.5.1/scopesim_templates/calibration/
--rw-rw-r--   0 hugo      (1000) hugo      (1000)       27 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/calibration/__init__.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)     3989 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/calibration/calibration.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)      163 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/defaults.yaml
-drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2024-02-06 20:44:08.656830 ScopeSim_Templates-0.5.1/scopesim_templates/extragalactic/
--rw-rw-r--   0 hugo      (1000) hugo      (1000)       91 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/extragalactic/__init__.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)        0 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/extragalactic/agns.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)        0 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/extragalactic/clusters.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)    10178 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/extragalactic/exgal_models.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)    14899 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/extragalactic/galaxies.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)     3030 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/extragalactic/galaxy_utils.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)        0 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/extragalactic/quasars.py
-drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2024-02-06 20:44:08.656830 ScopeSim_Templates-0.5.1/scopesim_templates/micado/
--rw-rw-r--   0 hugo      (1000) hugo      (1000)      846 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/micado/__init__.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)      263 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/micado/cluster.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)      124 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/micado/darkness.py
-drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2024-02-06 20:44:08.656830 ScopeSim_Templates-0.5.1/scopesim_templates/micado/data/
--rw-rw-r--   0 hugo      (1000) hugo      (1000)    11438 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/micado/data/masterlinelist_2.1.txt
--rw-rw-r--   0 hugo      (1000) hugo      (1000)     2100 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/micado/flatlamp.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)     1799 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/micado/pinhole_masks.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)     3977 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/micado/spectral_calibrations.py
-drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2024-02-06 20:44:08.660830 ScopeSim_Templates-0.5.1/scopesim_templates/micado/viking_fields/
--rw-rw-r--   0 hugo      (1000) hugo      (1000)       27 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/micado/viking_fields/__init__.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)     1459 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/micado/viking_fields/cat_illum.dat
--rw-rw-r--   0 hugo      (1000) hugo      (1000)     1228 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/micado/viking_fields/cat_science.dat
--rw-rw-r--   0 hugo      (1000) hugo      (1000)     1195 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/micado/viking_fields/cat_stdstar.dat
--rw-rw-r--   0 hugo      (1000) hugo      (1000)    18130 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/micado/viking_fields/faintgal_1.dat
--rw-rw-r--   0 hugo      (1000) hugo      (1000)    18130 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/micado/viking_fields/faintgal_2.dat
--rw-rw-r--   0 hugo      (1000) hugo      (1000)    18130 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/micado/viking_fields/faintgal_3.dat
--rw-rw-r--   0 hugo      (1000) hugo      (1000)   606111 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/micado/viking_fields/field_illum.eps
--rw-rw-r--   0 hugo      (1000) hugo      (1000)   544241 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/micado/viking_fields/field_science.eps
--rw-rw-r--   0 hugo      (1000) hugo      (1000)   604612 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/micado/viking_fields/field_stdstar.eps
--rw-rw-r--   0 hugo      (1000) hugo      (1000)     8503 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/micado/viking_fields/readme.rst
--rw-rw-r--   0 hugo      (1000) hugo      (1000)     6587 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/micado/viking_fields/viking_fields.py
-drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2024-02-06 20:44:08.660830 ScopeSim_Templates-0.5.1/scopesim_templates/misc/
--rw-rw-r--   0 hugo      (1000) hugo      (1000)       20 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/misc/__init__.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)    14407 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/misc/misc.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)      597 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/rc.py
-drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2024-02-06 20:44:08.660830 ScopeSim_Templates-0.5.1/scopesim_templates/stellar/
--rw-rw-r--   0 hugo      (1000) hugo      (1000)       45 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/stellar/__init__.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)     3274 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/stellar/cluster_utils.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)     4474 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/stellar/clusters.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)    31038 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/stellar/imf.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)     3595 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/stellar/mamajek_alt.dat
--rw-rw-r--   0 hugo      (1000) hugo      (1000)     9371 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/stellar/stars.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)     1996 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/stellar/stars_utils.py
-drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2024-02-06 20:44:08.660830 ScopeSim_Templates-0.5.1/scopesim_templates/utils/
--rw-rw-r--   0 hugo      (1000) hugo      (1000)       51 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/utils/__init__.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)     3402 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/utils/general_utils.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)     3733 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/utils/samplers.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)     1032 2024-02-06 20:42:37.000000 ScopeSim_Templates-0.5.1/scopesim_templates/version.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)       38 2024-02-06 20:44:08.664830 ScopeSim_Templates-0.5.1/setup.cfg
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2024-05-13 20:42:15.501413 scopesim_templates-0.5.2/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    35149 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/LICENSE
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)      256 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/MANIFEST.in
+-rw-r--r--   0 hugo      (1000) hugo      (1000)     1891 2024-05-13 20:42:15.501413 scopesim_templates-0.5.2/PKG-INFO
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     4059 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/README.md
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2024-05-13 20:42:15.501413 scopesim_templates-0.5.2/ScopeSim_Templates.egg-info/
+-rw-r--r--   0 hugo      (1000) hugo      (1000)     1891 2024-05-13 20:42:15.000000 scopesim_templates-0.5.2/ScopeSim_Templates.egg-info/PKG-INFO
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     2327 2024-05-13 20:42:15.000000 scopesim_templates-0.5.2/ScopeSim_Templates.egg-info/SOURCES.txt
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)        1 2024-05-13 20:42:15.000000 scopesim_templates-0.5.2/ScopeSim_Templates.egg-info/dependency_links.txt
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)      373 2024-05-13 20:42:15.000000 scopesim_templates-0.5.2/ScopeSim_Templates.egg-info/requires.txt
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)       29 2024-05-13 20:42:15.000000 scopesim_templates-0.5.2/ScopeSim_Templates.egg-info/top_level.txt
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2024-05-13 20:42:15.493413 scopesim_templates-0.5.2/docs/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     8582 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/docs/conf.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     1684 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/pyproject.toml
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2024-05-13 20:42:15.493413 scopesim_templates-0.5.2/scopesim_templates/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)      938 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/__init__.py
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2024-05-13 20:42:15.493413 scopesim_templates-0.5.2/scopesim_templates/calibration/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)       27 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/calibration/__init__.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     3989 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/calibration/calibration.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)      163 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/defaults.yaml
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2024-05-13 20:42:15.497413 scopesim_templates-0.5.2/scopesim_templates/extragalactic/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)       91 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/extragalactic/__init__.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)        0 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/extragalactic/agns.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)        0 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/extragalactic/clusters.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    10178 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/extragalactic/exgal_models.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    14899 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/extragalactic/galaxies.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     3030 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/extragalactic/galaxy_utils.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)        0 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/extragalactic/quasars.py
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2024-05-13 20:42:15.497413 scopesim_templates-0.5.2/scopesim_templates/metis/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)      119 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/metis/__init__.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     5012 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/metis/laser.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     1361 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/metis/pinhole_mask.py
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2024-05-13 20:42:15.497413 scopesim_templates-0.5.2/scopesim_templates/micado/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)      846 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/micado/__init__.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)      263 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/micado/cluster.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)      124 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/micado/darkness.py
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2024-05-13 20:42:15.497413 scopesim_templates-0.5.2/scopesim_templates/micado/data/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    11438 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/micado/data/masterlinelist_2.1.txt
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     2100 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/micado/flatlamp.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     1799 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/micado/pinhole_masks.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     3977 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/micado/spectral_calibrations.py
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2024-05-13 20:42:15.501413 scopesim_templates-0.5.2/scopesim_templates/micado/viking_fields/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)       27 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/micado/viking_fields/__init__.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     1459 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/micado/viking_fields/cat_illum.dat
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     1228 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/micado/viking_fields/cat_science.dat
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     1195 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/micado/viking_fields/cat_stdstar.dat
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    18130 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/micado/viking_fields/faintgal_1.dat
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    18130 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/micado/viking_fields/faintgal_2.dat
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    18130 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/micado/viking_fields/faintgal_3.dat
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)   606111 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/micado/viking_fields/field_illum.eps
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)   544241 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/micado/viking_fields/field_science.eps
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)   604612 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/micado/viking_fields/field_stdstar.eps
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     8503 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/micado/viking_fields/readme.rst
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     6587 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/micado/viking_fields/viking_fields.py
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2024-05-13 20:42:15.501413 scopesim_templates-0.5.2/scopesim_templates/misc/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)       20 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/misc/__init__.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    14407 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/misc/misc.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)      597 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/rc.py
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2024-05-13 20:42:15.501413 scopesim_templates-0.5.2/scopesim_templates/stellar/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)       45 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/stellar/__init__.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     3274 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/stellar/cluster_utils.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     4474 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/stellar/clusters.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    31038 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/stellar/imf.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     3595 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/stellar/mamajek_alt.dat
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     9371 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/stellar/stars.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     1996 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/stellar/stars_utils.py
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2024-05-13 20:42:15.501413 scopesim_templates-0.5.2/scopesim_templates/utils/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)       51 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/utils/__init__.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     3402 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/utils/general_utils.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     3733 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/utils/samplers.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     1197 2024-05-13 20:40:14.000000 scopesim_templates-0.5.2/scopesim_templates/version.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)       38 2024-05-13 20:42:15.501413 scopesim_templates-0.5.2/setup.cfg
```

### Comparing `ScopeSim_Templates-0.5.1/LICENSE` & `scopesim_templates-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/PKG-INFO` & `scopesim_templates-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScopeSim_Templates
-Version: 0.5.1
+Version: 0.5.2
 Summary: On-sky source templates for ScopeSim
 Author-email: A* Vienna <astar.astro@univie.ac.at>
 Maintainer-email: Kieran Leschinski <kieran.leschinski@unive.ac.at>, Hugo Buddelmeijer <hugo@buddelmeijer.nl>
 License: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://scopesim_templates.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AstarVienna/ScopeSim_Templates
 Project-URL: Bug Reports, https://github.com/AstarVienna/ScopeSim_Templates/issues
@@ -23,15 +23,15 @@
 Requires-Dist: docutils>=0.19
 Requires-Dist: beautifulsoup4>=4.12.1
 Requires-Dist: lxml>=4.9.3
 Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: synphot>=1.2.1
 Requires-Dist: scopesim>=0.7.0
 Requires-Dist: pyckles>=0.2
-Requires-Dist: spextra>=0.33
+Requires-Dist: spextra>=0.40.0
 Requires-Dist: astar-utils>=0.2.1
 Provides-Extra: dev
 Requires-Dist: jupyter; extra == "dev"
 Requires-Dist: jupytext; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
```

### Comparing `ScopeSim_Templates-0.5.1/README.md` & `scopesim_templates-0.5.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # ScopeSim Templates
 
 [![Build Status](https://github.com/AstarVienna/ScopeSim_Templates/actions/workflows/tests.yml/badge.svg)](https://github.com/AstarVienna/ScopeSim_Templates/actions/workflows/tests.yml/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/scopesim-templates/badge/?version=latest)](https://scopesim-templates.readthedocs.io/en/latest)
-[![Codecov](https://img.shields.io/codecov/c/github/AstarVienna/ScopeSim_Templates/\branch/dev_master?logo=codecov)](https://app.codecov.io/gh/AstarVienna/ScopeSim_Templates/tree/dev_master)
+[![Codecov](https://img.shields.io/codecov/c/github/AstarVienna/ScopeSim_Templates/branch/main?logo=codecov)](https://app.codecov.io/gh/AstarVienna/ScopeSim_Templates/tree/main)
 [![PyPI - Version](https://img.shields.io/pypi/v/ScopeSim-Templates)](https://pypi.org/project/ScopeSim-Templates/)
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 This packages contain a number of templates to generate `Source` objects to be used in simulations with the [ScopeSim Simulator](https://scopesim.readthedocs.io/en/latest/)
 
 The Documentation can be found here: https://scopesim-templates.readthedocs.io/en/latest
```

### Comparing `ScopeSim_Templates-0.5.1/ScopeSim_Templates.egg-info/PKG-INFO` & `scopesim_templates-0.5.2/ScopeSim_Templates.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScopeSim_Templates
-Version: 0.5.1
+Version: 0.5.2
 Summary: On-sky source templates for ScopeSim
 Author-email: A* Vienna <astar.astro@univie.ac.at>
 Maintainer-email: Kieran Leschinski <kieran.leschinski@unive.ac.at>, Hugo Buddelmeijer <hugo@buddelmeijer.nl>
 License: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://scopesim_templates.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AstarVienna/ScopeSim_Templates
 Project-URL: Bug Reports, https://github.com/AstarVienna/ScopeSim_Templates/issues
@@ -23,15 +23,15 @@
 Requires-Dist: docutils>=0.19
 Requires-Dist: beautifulsoup4>=4.12.1
 Requires-Dist: lxml>=4.9.3
 Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: synphot>=1.2.1
 Requires-Dist: scopesim>=0.7.0
 Requires-Dist: pyckles>=0.2
-Requires-Dist: spextra>=0.33
+Requires-Dist: spextra>=0.40.0
 Requires-Dist: astar-utils>=0.2.1
 Provides-Extra: dev
 Requires-Dist: jupyter; extra == "dev"
 Requires-Dist: jupytext; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
```

### Comparing `ScopeSim_Templates-0.5.1/ScopeSim_Templates.egg-info/SOURCES.txt` & `scopesim_templates-0.5.2/ScopeSim_Templates.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 scopesim_templates/extragalactic/__init__.py
 scopesim_templates/extragalactic/agns.py
 scopesim_templates/extragalactic/clusters.py
 scopesim_templates/extragalactic/exgal_models.py
 scopesim_templates/extragalactic/galaxies.py
 scopesim_templates/extragalactic/galaxy_utils.py
 scopesim_templates/extragalactic/quasars.py
+scopesim_templates/metis/__init__.py
+scopesim_templates/metis/laser.py
+scopesim_templates/metis/pinhole_mask.py
 scopesim_templates/micado/__init__.py
 scopesim_templates/micado/cluster.py
 scopesim_templates/micado/darkness.py
 scopesim_templates/micado/flatlamp.py
 scopesim_templates/micado/pinhole_masks.py
 scopesim_templates/micado/spectral_calibrations.py
 scopesim_templates/micado/data/masterlinelist_2.1.txt
```

### Comparing `ScopeSim_Templates-0.5.1/docs/conf.py` & `scopesim_templates-0.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/pyproject.toml` & `scopesim_templates-0.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "ScopeSim_Templates"
 # When updating the version, also add a date and release notes to version.py
-version = "0.5.1"
+version = "0.5.2"
 description = "On-sky source templates for ScopeSim"
 readme = "README.rst"
 requires-python = ">=3.9"
 license = {text = "License :: OSI Approved :: GNU General Public License v3 (GPLv3)"}
 authors = [
     {name = "A* Vienna", email="astar.astro@univie.ac.at"},
 ]
@@ -31,15 +31,15 @@
     "lxml>=4.9.3",
     "pyyaml>=6.0.1",
 
     "synphot>=1.2.1",
 
     "scopesim>=0.7.0",
     "pyckles>=0.2",
-    "spextra>=0.33",
+    "spextra>=0.40.0",
     "astar-utils>=0.2.1",
 ]
 
 [project.optional-dependencies]
 dev = [
     "jupyter",
     "jupytext",
```

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/__init__.py` & `scopesim_templates-0.5.2/scopesim_templates/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import warnings
 
 from . import calibration
 from . import extragalactic
 from . import misc
 from . import stellar
 from . import utils
+from . import metis
 
 # This warning is emitted when just doing "import scopesim_templates", which
 # should be a normal non-warning thing to do.
 # TODO: Find a way to emit this warning only when the functions below are
 #       accessed directly.
 # warnings.warn("In a future version top level function calls will be removed. "
 #               "Always use this syntax: from module.submodule import function",
```

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/calibration/calibration.py` & `scopesim_templates-0.5.2/scopesim_templates/calibration/calibration.py`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/extragalactic/exgal_models.py` & `scopesim_templates-0.5.2/scopesim_templates/extragalactic/exgal_models.py`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/extragalactic/galaxies.py` & `scopesim_templates-0.5.2/scopesim_templates/extragalactic/galaxies.py`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/extragalactic/galaxy_utils.py` & `scopesim_templates-0.5.2/scopesim_templates/extragalactic/galaxy_utils.py`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/micado/__init__.py` & `scopesim_templates-0.5.2/scopesim_templates/micado/__init__.py`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/micado/data/masterlinelist_2.1.txt` & `scopesim_templates-0.5.2/scopesim_templates/micado/data/masterlinelist_2.1.txt`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/micado/flatlamp.py` & `scopesim_templates-0.5.2/scopesim_templates/micado/flatlamp.py`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/micado/pinhole_masks.py` & `scopesim_templates-0.5.2/scopesim_templates/micado/pinhole_masks.py`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/micado/spectral_calibrations.py` & `scopesim_templates-0.5.2/scopesim_templates/micado/spectral_calibrations.py`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/micado/viking_fields/cat_illum.dat` & `scopesim_templates-0.5.2/scopesim_templates/micado/viking_fields/cat_illum.dat`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/micado/viking_fields/cat_science.dat` & `scopesim_templates-0.5.2/scopesim_templates/micado/viking_fields/cat_science.dat`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/micado/viking_fields/cat_stdstar.dat` & `scopesim_templates-0.5.2/scopesim_templates/micado/viking_fields/cat_stdstar.dat`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/micado/viking_fields/faintgal_1.dat` & `scopesim_templates-0.5.2/scopesim_templates/micado/viking_fields/faintgal_1.dat`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/micado/viking_fields/faintgal_2.dat` & `scopesim_templates-0.5.2/scopesim_templates/micado/viking_fields/faintgal_2.dat`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/micado/viking_fields/faintgal_3.dat` & `scopesim_templates-0.5.2/scopesim_templates/micado/viking_fields/faintgal_3.dat`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/micado/viking_fields/field_illum.eps` & `scopesim_templates-0.5.2/scopesim_templates/micado/viking_fields/field_illum.eps`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/micado/viking_fields/field_science.eps` & `scopesim_templates-0.5.2/scopesim_templates/micado/viking_fields/field_science.eps`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/micado/viking_fields/field_stdstar.eps` & `scopesim_templates-0.5.2/scopesim_templates/micado/viking_fields/field_stdstar.eps`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/micado/viking_fields/readme.rst` & `scopesim_templates-0.5.2/scopesim_templates/micado/viking_fields/readme.rst`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/micado/viking_fields/viking_fields.py` & `scopesim_templates-0.5.2/scopesim_templates/micado/viking_fields/viking_fields.py`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/misc/misc.py` & `scopesim_templates-0.5.2/scopesim_templates/misc/misc.py`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/rc.py` & `scopesim_templates-0.5.2/scopesim_templates/rc.py`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/stellar/cluster_utils.py` & `scopesim_templates-0.5.2/scopesim_templates/stellar/cluster_utils.py`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/stellar/clusters.py` & `scopesim_templates-0.5.2/scopesim_templates/stellar/clusters.py`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/stellar/imf.py` & `scopesim_templates-0.5.2/scopesim_templates/stellar/imf.py`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/stellar/mamajek_alt.dat` & `scopesim_templates-0.5.2/scopesim_templates/stellar/mamajek_alt.dat`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/stellar/stars.py` & `scopesim_templates-0.5.2/scopesim_templates/stellar/stars.py`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/stellar/stars_utils.py` & `scopesim_templates-0.5.2/scopesim_templates/stellar/stars_utils.py`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/utils/general_utils.py` & `scopesim_templates-0.5.2/scopesim_templates/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/utils/samplers.py` & `scopesim_templates-0.5.2/scopesim_templates/utils/samplers.py`

 * *Files identical despite different names*

### Comparing `ScopeSim_Templates-0.5.1/scopesim_templates/version.py` & `scopesim_templates-0.5.2/scopesim_templates/version.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 from importlib import metadata
 version = metadata.version(__package__)
 date = '2024-02-06 18:00:00 GMT'
 yaml_descriptions = """
+- version : 0.5.2
+  date : 2024-05-13
+  comment : Patch to add METIS calibration sources.
+  changes :
+  - Add scopesim_templates/metis/laser.py and pinhole_mask.py
+
 - version : 0.5.1
   date : 2024-02-06
   comment : Patch to remove Python 3.8 and SystemDict.
   changes :
   - Drop support for Python 3.8 #77
   - Use astar_utils.NestedMapping instead of scopesim.system_dict.SystemDict #76
   - Fix scaling of spectrum #74
```

