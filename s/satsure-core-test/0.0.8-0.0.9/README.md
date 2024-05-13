# Comparing `tmp/satsure_core_test-0.0.8.tar.gz` & `tmp/satsure_core_test-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satsure_core_test-0.0.8.tar", last modified: Mon May 13 07:57:03 2024, max compression
+gzip compressed data, was "satsure_core_test-0.0.9.tar", last modified: Mon May 13 10:03:02 2024, max compression
```

## Comparing `satsure_core_test-0.0.8.tar` & `satsure_core_test-0.0.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:57:03.705594 satsure_core_test-0.0.8/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:02.000000 satsure_core_test-0.0.8/LICENCE.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      483 2024-05-13 07:57:03.705276 satsure_core_test-0.0.8/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:18.000000 satsure_core_test-0.0.8/README.md
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:57:03.689097 satsure_core_test-0.0.8/satelite/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-06 07:15:52.000000 satsure_core_test-0.0.8/satelite/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      974 2024-05-13 07:33:26.000000 satsure_core_test-0.0.8/satelite/config.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:57:03.689618 satsure_core_test-0.0.8/satelite/core/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.0.8/satelite/core/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2479 2024-05-13 07:33:26.000000 satsure_core_test-0.0.8/satelite/core/downloader.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:57:03.689886 satsure_core_test-0.0.8/satelite/gdal/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.0.8/satelite/gdal/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2539 2024-05-13 07:51:34.000000 satsure_core_test-0.0.8/satelite/gdal/gdal_commands.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:57:03.690359 satsure_core_test-0.0.8/satelite/models/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.0.8/satelite/models/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-13 07:33:26.000000 satsure_core_test-0.0.8/satelite/models/s2_enum.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:57:03.690695 satsure_core_test-0.0.8/satelite/raster/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.0.8/satelite/raster/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8913 2024-05-13 07:51:34.000000 satsure_core_test-0.0.8/satelite/raster/raster.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:57:03.695195 satsure_core_test-0.0.8/satelite/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      448 2024-05-13 07:57:00.000000 satsure_core_test-0.0.8/satelite/sentinel2/__init__.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:57:03.695604 satsure_core_test-0.0.8/satelite/sentinel2/band_stack/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.0.8/satelite/sentinel2/band_stack/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2829 2024-05-13 07:51:34.000000 satsure_core_test-0.0.8/satelite/sentinel2/band_stack/generate_band_stack.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-13 07:33:26.000000 satsure_core_test-0.0.8/satelite/sentinel2/fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-06 07:15:52.000000 satsure_core_test-0.0.8/satelite/sentinel2/fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3121 2024-05-13 07:33:26.000000 satsure_core_test-0.0.8/satelite/sentinel2/get_tiles.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:57:03.696049 satsure_core_test-0.0.8/satelite/sentinel2/indices/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.0.8/satelite/sentinel2/indices/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     4215 2024-05-13 07:51:34.000000 satsure_core_test-0.0.8/satelite/sentinel2/indices/general_indices.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2448 2024-05-13 07:51:34.000000 satsure_core_test-0.0.8/satelite/sentinel2/mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-13 07:51:34.000000 satsure_core_test-0.0.8/satelite/sentinel2/path_row_from_shp.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3250 2024-05-13 07:33:26.000000 satsure_core_test-0.0.8/satelite/sentinel2/s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2912 2024-05-13 07:33:26.000000 satsure_core_test-0.0.8/satelite/sentinel2/s2_l2a_urls.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:57:03.696568 satsure_core_test-0.0.8/satelite/tests/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure_core_test-0.0.8/satelite/tests/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      747 2024-05-06 07:43:01.000000 satsure_core_test-0.0.8/satelite/tests/conftest.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:57:03.701979 satsure_core_test-0.0.8/satelite/tests/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure_core_test-0.0.8/satelite/tests/sentinel2/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      384 2024-05-06 07:43:01.000000 satsure_core_test-0.0.8/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      430 2024-05-06 07:34:13.000000 satsure_core_test-0.0.8/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1322 2024-05-06 07:34:13.000000 satsure_core_test-0.0.8/satelite/tests/sentinel2/test_get_tile.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      322 2024-05-13 07:33:26.000000 satsure_core_test-0.0.8/satelite/tests/sentinel2/test_mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      871 2024-05-13 07:33:26.000000 satsure_core_test-0.0.8/satelite/tests/sentinel2/test_s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      898 2024-05-13 07:33:26.000000 satsure_core_test-0.0.8/satelite/tests/sentinel2/test_s2_l2a_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1543 2024-05-13 07:33:26.000000 satsure_core_test-0.0.8/satelite/tests/sentinel2/test_validate.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:57:03.703041 satsure_core_test-0.0.8/satelite/validators/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:51:34.000000 satsure_core_test-0.0.8/satelite/validators/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2381 2024-05-13 07:51:34.000000 satsure_core_test-0.0.8/satelite/validators/check_shape_of_rid.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:57:03.704892 satsure_core_test-0.0.8/satsure_core_test.egg-info/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      483 2024-05-13 07:57:03.000000 satsure_core_test-0.0.8/satsure_core_test.egg-info/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1491 2024-05-13 07:57:03.000000 satsure_core_test-0.0.8/satsure_core_test.egg-info/SOURCES.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-13 07:57:03.000000 satsure_core_test-0.0.8/satsure_core_test.egg-info/dependency_links.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      124 2024-05-13 07:57:03.000000 satsure_core_test-0.0.8/satsure_core_test.egg-info/requires.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        9 2024-05-13 07:57:03.000000 satsure_core_test-0.0.8/satsure_core_test.egg-info/top_level.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-13 07:57:03.706179 satsure_core_test-0.0.8/setup.cfg
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      507 2024-05-13 07:57:00.000000 satsure_core_test-0.0.8/setup.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 10:03:02.830765 satsure_core_test-0.0.9/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:02.000000 satsure_core_test-0.0.9/LICENCE.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      503 2024-05-13 10:03:02.830525 satsure_core_test-0.0.9/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:18.000000 satsure_core_test-0.0.9/README.md
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 10:03:02.823153 satsure_core_test-0.0.9/satelite/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-06 07:15:52.000000 satsure_core_test-0.0.9/satelite/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      974 2024-05-13 07:33:26.000000 satsure_core_test-0.0.9/satelite/config.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 10:03:02.823501 satsure_core_test-0.0.9/satelite/core/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.0.9/satelite/core/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2479 2024-05-13 07:33:26.000000 satsure_core_test-0.0.9/satelite/core/downloader.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 10:03:02.823796 satsure_core_test-0.0.9/satelite/gdal/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.0.9/satelite/gdal/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2539 2024-05-13 07:51:34.000000 satsure_core_test-0.0.9/satelite/gdal/gdal_commands.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 10:03:02.824418 satsure_core_test-0.0.9/satelite/models/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.0.9/satelite/models/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-13 07:33:26.000000 satsure_core_test-0.0.9/satelite/models/s2_enum.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 10:03:02.824739 satsure_core_test-0.0.9/satelite/raster/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.0.9/satelite/raster/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8913 2024-05-13 07:51:34.000000 satsure_core_test-0.0.9/satelite/raster/raster.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 10:03:02.826812 satsure_core_test-0.0.9/satelite/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      448 2024-05-13 08:48:32.000000 satsure_core_test-0.0.9/satelite/sentinel2/__init__.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 10:03:02.827106 satsure_core_test-0.0.9/satelite/sentinel2/band_stack/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.0.9/satelite/sentinel2/band_stack/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2829 2024-05-13 07:51:34.000000 satsure_core_test-0.0.9/satelite/sentinel2/band_stack/generate_band_stack.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-13 07:33:26.000000 satsure_core_test-0.0.9/satelite/sentinel2/fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-06 07:15:52.000000 satsure_core_test-0.0.9/satelite/sentinel2/fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3121 2024-05-13 07:33:26.000000 satsure_core_test-0.0.9/satelite/sentinel2/get_tiles.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 10:03:02.827677 satsure_core_test-0.0.9/satelite/sentinel2/indices/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.0.9/satelite/sentinel2/indices/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     4215 2024-05-13 07:51:34.000000 satsure_core_test-0.0.9/satelite/sentinel2/indices/general_indices.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2468 2024-05-13 10:01:38.000000 satsure_core_test-0.0.9/satelite/sentinel2/mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-13 07:51:34.000000 satsure_core_test-0.0.9/satelite/sentinel2/path_row_from_shp.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3250 2024-05-13 07:33:26.000000 satsure_core_test-0.0.9/satelite/sentinel2/s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2912 2024-05-13 07:33:26.000000 satsure_core_test-0.0.9/satelite/sentinel2/s2_l2a_urls.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 10:03:02.828027 satsure_core_test-0.0.9/satelite/tests/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure_core_test-0.0.9/satelite/tests/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      747 2024-05-06 07:43:01.000000 satsure_core_test-0.0.9/satelite/tests/conftest.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 10:03:02.829346 satsure_core_test-0.0.9/satelite/tests/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure_core_test-0.0.9/satelite/tests/sentinel2/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      384 2024-05-13 07:58:31.000000 satsure_core_test-0.0.9/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      430 2024-05-06 07:34:13.000000 satsure_core_test-0.0.9/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1322 2024-05-06 07:34:13.000000 satsure_core_test-0.0.9/satelite/tests/sentinel2/test_get_tile.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      322 2024-05-13 07:33:26.000000 satsure_core_test-0.0.9/satelite/tests/sentinel2/test_mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      871 2024-05-13 07:33:26.000000 satsure_core_test-0.0.9/satelite/tests/sentinel2/test_s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      898 2024-05-13 07:33:26.000000 satsure_core_test-0.0.9/satelite/tests/sentinel2/test_s2_l2a_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1543 2024-05-13 07:33:26.000000 satsure_core_test-0.0.9/satelite/tests/sentinel2/test_validate.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 10:03:02.829613 satsure_core_test-0.0.9/satelite/validators/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:51:34.000000 satsure_core_test-0.0.9/satelite/validators/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2381 2024-05-13 07:51:34.000000 satsure_core_test-0.0.9/satelite/validators/check_shape_of_rid.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 10:03:02.830323 satsure_core_test-0.0.9/satsure_core_test.egg-info/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      503 2024-05-13 10:03:02.000000 satsure_core_test-0.0.9/satsure_core_test.egg-info/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1491 2024-05-13 10:03:02.000000 satsure_core_test-0.0.9/satsure_core_test.egg-info/SOURCES.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-13 10:03:02.000000 satsure_core_test-0.0.9/satsure_core_test.egg-info/dependency_links.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      129 2024-05-13 10:03:02.000000 satsure_core_test-0.0.9/satsure_core_test.egg-info/requires.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        9 2024-05-13 10:03:02.000000 satsure_core_test-0.0.9/satsure_core_test.egg-info/top_level.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-13 10:03:02.830804 satsure_core_test-0.0.9/setup.cfg
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      514 2024-05-13 10:02:29.000000 satsure_core_test-0.0.9/setup.py
```

### Comparing `satsure_core_test-0.0.8/satelite/config.py` & `satsure_core_test-0.0.9/satelite/config.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.8/satelite/core/downloader.py` & `satsure_core_test-0.0.9/satelite/core/downloader.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.8/satelite/gdal/gdal_commands.py` & `satsure_core_test-0.0.9/satelite/gdal/gdal_commands.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.8/satelite/raster/raster.py` & `satsure_core_test-0.0.9/satelite/raster/raster.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.8/satelite/sentinel2/band_stack/generate_band_stack.py` & `satsure_core_test-0.0.9/satelite/sentinel2/band_stack/generate_band_stack.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.8/satelite/sentinel2/fetch_unique_tile_date.py` & `satsure_core_test-0.0.9/satelite/sentinel2/fetch_unique_tile_date.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.8/satelite/sentinel2/fetch_unique_tile_date_pystac.py` & `satsure_core_test-0.0.9/satelite/sentinel2/fetch_unique_tile_date_pystac.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.8/satelite/sentinel2/get_tiles.py` & `satsure_core_test-0.0.9/satelite/sentinel2/get_tiles.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.8/satelite/sentinel2/indices/general_indices.py` & `satsure_core_test-0.0.9/satelite/sentinel2/indices/general_indices.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.8/satelite/sentinel2/mosaic_same_bands.py` & `satsure_core_test-0.0.9/satelite/sentinel2/mosaic_same_bands.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from collections.abc import Iterable
 from pathlib import Path, PosixPath
 
 from satelite.raster.raster import merge
-
+from typing import  List
 
 class MosaicSameBands:
     """
     Stack similar bands on same date
     """
     BANDS = ("B02", "B03", "B04", "B05", "B08", "B12",)
 
     def __init__(self, input_folder: PosixPath,
                  output_folder: PosixPath,
-                 bands: Iterable[str] = None,
+                 bands: List[str] = None,
                  tile_identifier_position: int = 1):
 
         self.input_folder = input_folder
         self.output_folder = output_folder
         self.bands = bands or self.BANDS
         self.tile_identifier_position = tile_identifier_position
```

### Comparing `satsure_core_test-0.0.8/satelite/sentinel2/path_row_from_shp.py` & `satsure_core_test-0.0.9/satelite/sentinel2/path_row_from_shp.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.8/satelite/sentinel2/s2_l1c_urls.py` & `satsure_core_test-0.0.9/satelite/sentinel2/s2_l1c_urls.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.8/satelite/sentinel2/s2_l2a_urls.py` & `satsure_core_test-0.0.9/satelite/sentinel2/s2_l2a_urls.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.8/satelite/tests/conftest.py` & `satsure_core_test-0.0.9/satelite/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.8/satelite/tests/sentinel2/test_get_tile.py` & `satsure_core_test-0.0.9/satelite/tests/sentinel2/test_get_tile.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.8/satelite/tests/sentinel2/test_s2_l1c_urls.py` & `satsure_core_test-0.0.9/satelite/tests/sentinel2/test_s2_l1c_urls.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.8/satelite/tests/sentinel2/test_s2_l2a_urls.py` & `satsure_core_test-0.0.9/satelite/tests/sentinel2/test_s2_l2a_urls.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.8/satelite/tests/sentinel2/test_validate.py` & `satsure_core_test-0.0.9/satelite/tests/sentinel2/test_validate.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.8/satelite/validators/check_shape_of_rid.py` & `satsure_core_test-0.0.9/satelite/validators/check_shape_of_rid.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.8/satsure_core_test.egg-info/SOURCES.txt` & `satsure_core_test-0.0.9/satsure_core_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

