# Comparing `tmp/py_tools_ds-0.9.3.tar.gz` & `tmp/py_tools_ds-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py_tools_ds-0.9.3.tar", last modified: Thu Oct 12 21:43:50 2017, max compression
+gzip compressed data, was "dist/py_tools_ds-0.9.4.tar", last modified: Thu Nov  2 20:49:24 2017, max compression
```

## Comparing `py_tools_ds-0.9.3.tar` & `py_tools_ds-0.9.4.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/
--rw-rw-rw-   0 root         (0) root         (0)     1581 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/py_tools_ds/
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/py_tools_ds/similarity/
--rw-rw-rw-   0 root         (0) root         (0)      657 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/similarity/raster.py
--rw-rw-rw-   0 root         (0) root         (0)      100 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/similarity/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/py_tools_ds/dtypes/
--rw-rw-rw-   0 root         (0) root         (0)     2189 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/dtypes/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)      108 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/dtypes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/py_tools_ds/geo/
--rwxrwxrwx   0 root         (0) root         (0)    14528 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/geo/coord_trafo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/py_tools_ds/geo/vector/
--rw-rw-rw-   0 root         (0) root         (0)     8737 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/geo/vector/geometry.py
--rw-rw-rw-   0 root         (0) root         (0)     4948 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/geo/vector/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)     6710 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/geo/vector/topology.py
--rw-rw-rw-   0 root         (0) root         (0)      200 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/geo/vector/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8867 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/geo/coord_calc.py
--rw-rw-rw-   0 root         (0) root         (0)     4327 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/geo/coord_grid.py
--rw-rw-rw-   0 root         (0) root         (0)     7441 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/geo/projection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/py_tools_ds/geo/raster/
--rw-rw-rw-   0 root         (0) root         (0)     4596 2017-10-12 21:25:45.000000 py_tools_ds-0.9.3/py_tools_ds/geo/raster/conversion.py
--rwxrwxrwx   0 root         (0) root         (0)    24914 2017-10-12 21:25:45.000000 py_tools_ds-0.9.3/py_tools_ds/geo/raster/reproject.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/geo/raster/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      366 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/geo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4284 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/geo/map_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/py_tools_ds/web/
--rw-rw-rw-   0 root         (0) root         (0)     1252 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/web/network.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/web/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/py_tools_ds/processing/
--rwxrwxrwx   0 root         (0) root         (0)      611 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/processing/shell.py
--rw-rw-rw-   0 root         (0) root         (0)       98 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/processing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5618 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/processing/progress_mon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/py_tools_ds/environment/
--rw-rw-rw-   0 root         (0) root         (0)     1847 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/environment/gdal_env.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/environment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/py_tools_ds/compatibility/
--rwxrwxrwx   0 root         (0) root         (0)    16693 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/compatibility/gdal.py
--rwxrwxrwx   0 root         (0) root         (0)     1771 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/compatibility/gdalnumeric.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/py_tools_ds/compatibility/python/
--rw-rw-rw-   0 root         (0) root         (0)      180 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/compatibility/python/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/compatibility/python/os.py
--rw-rw-rw-   0 root         (0) root         (0)      108 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/compatibility/python/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       56 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/compatibility/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/py_tools_ds/io/
--rw-rw-rw-   0 root         (0) root         (0)     1887 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/io/pathgen.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/py_tools_ds/io/raster/
--rwxrwxrwx   0 root         (0) root         (0)     2586 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/io/raster/gdal.py
--rw-rw-rw-   0 root         (0) root         (0)       56 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/io/raster/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      144 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/io/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/py_tools_ds/compression/
--rw-rw-rw-   0 root         (0) root         (0)     3340 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/compression/decompress.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/compression/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/py_tools_ds/convenience/
--rw-rw-rw-   0 root         (0) root         (0)      237 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/convenience/object_oriented.py
--rw-rw-rw-   0 root         (0) root         (0)      118 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/convenience/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/py_tools_ds/numeric/
--rw-rw-rw-   0 root         (0) root         (0)      847 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/numeric/array.py
--rw-rw-rw-   0 root         (0) root         (0)      171 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/numeric/numbers.py
--rw-rw-rw-   0 root         (0) root         (0)     1892 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/numeric/vector.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/py_tools_ds/numeric/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      670 2017-10-12 21:31:14.000000 py_tools_ds-0.9.3/py_tools_ds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1896 2017-10-12 21:31:14.000000 py_tools_ds-0.9.3/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      262 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/tests/CI_docker/
--rw-rw-rw-   0 root         (0) root         (0)     1208 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/tests/CI_docker/build_testsuite_image.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/tests/CI_docker/context/
--rw-rw-rw-   0 root         (0) root         (0)     2005 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/tests/CI_docker/context/py_tools_ds_ci.docker
--rw-rw-rw-   0 root         (0) root         (0)     3149 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/tests/test_map_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/tests/linting/
--rw-rw-rw-   0 root         (0) root         (0)        0 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/tests/linting/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)      788 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/tests/test_coord_grid.py
--rw-rw-rw-   0 root         (0) root         (0)     1820 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/tests/test_projection.py
--rw-rw-rw-   0 root         (0) root         (0)       24 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      383 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      173 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)     4172 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2493 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/py_tools_ds.egg-info/
--rw-r--r--   0 root         (0) root         (0)       18 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/py_tools_ds.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       69 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/py_tools_ds.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     2532 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/py_tools_ds.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     4172 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/py_tools_ds.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/py_tools_ds.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/py_tools_ds.egg-info/not-zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/docs/
--rw-rw-rw-   0 root         (0) root         (0)     6785 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)       77 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/docs/usage.rst
--rw-rw-rw-   0 root         (0) root         (0)       33 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/docs/contributing.rst
--rw-rw-rw-   0 root         (0) root         (0)       27 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/docs/readme.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/docs/_build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/docs/_build/html/
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-12 21:43:50.000000 py_tools_ds-0.9.3/docs/_build/html/_static/
--rw-r--r--   0 root         (0) root         (0)      829 2017-07-02 09:28:03.000000 py_tools_ds-0.9.3/docs/_build/html/_static/comment-close.png
--rw-r--r--   0 root         (0) root         (0)      286 2017-07-02 09:28:03.000000 py_tools_ds-0.9.3/docs/_build/html/_static/file.png
--rw-r--r--   0 root         (0) root         (0)      673 2017-07-02 09:28:03.000000 py_tools_ds-0.9.3/docs/_build/html/_static/ajax-loader.gif
--rw-r--r--   0 root         (0) root         (0)       90 2017-07-02 09:28:03.000000 py_tools_ds-0.9.3/docs/_build/html/_static/minus.png
--rw-r--r--   0 root         (0) root         (0)      214 2017-07-02 09:28:03.000000 py_tools_ds-0.9.3/docs/_build/html/_static/up-pressed.png
--rw-r--r--   0 root         (0) root         (0)       90 2017-07-02 09:28:03.000000 py_tools_ds-0.9.3/docs/_build/html/_static/plus.png
--rw-r--r--   0 root         (0) root         (0)      202 2017-07-02 09:28:03.000000 py_tools_ds-0.9.3/docs/_build/html/_static/down.png
--rw-r--r--   0 root         (0) root         (0)      203 2017-07-02 09:28:03.000000 py_tools_ds-0.9.3/docs/_build/html/_static/up.png
--rw-r--r--   0 root         (0) root         (0)      222 2017-07-02 09:28:03.000000 py_tools_ds-0.9.3/docs/_build/html/_static/down-pressed.png
--rw-r--r--   0 root         (0) root         (0)      641 2017-07-02 09:28:03.000000 py_tools_ds-0.9.3/docs/_build/html/_static/comment.png
--rw-r--r--   0 root         (0) root         (0)      756 2017-07-02 09:28:03.000000 py_tools_ds-0.9.3/docs/_build/html/_static/comment-bright.png
--rwxrwxrwx   0 root         (0) root         (0)     8455 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       28 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/docs/authors.rst
--rw-rw-rw-   0 root         (0) root         (0)     6469 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)      287 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1223 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/docs/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)       28 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/docs/history.rst
--rw-rw-rw-   0 root         (0) root         (0)       89 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     3314 2017-10-10 22:39:20.000000 py_tools_ds-0.9.3/CONTRIBUTING.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/py_tools_ds/
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/py_tools_ds/similarity/
+-rw-rw-rw-   0 root         (0) root         (0)      657 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/similarity/raster.py
+-rw-rw-rw-   0 root         (0) root         (0)      100 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/similarity/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/py_tools_ds/dtypes/
+-rw-rw-rw-   0 root         (0) root         (0)     2189 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/dtypes/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)      108 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/dtypes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/py_tools_ds/geo/
+-rwxrwxrwx   0 root         (0) root         (0)    14528 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/geo/coord_trafo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/py_tools_ds/geo/vector/
+-rw-rw-rw-   0 root         (0) root         (0)     8737 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/geo/vector/geometry.py
+-rw-rw-rw-   0 root         (0) root         (0)     4948 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/geo/vector/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)     6710 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/geo/vector/topology.py
+-rw-rw-rw-   0 root         (0) root         (0)      200 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/geo/vector/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8867 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/geo/coord_calc.py
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/geo/coord_grid.py
+-rw-rw-rw-   0 root         (0) root         (0)     7441 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/geo/projection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/py_tools_ds/geo/raster/
+-rw-rw-rw-   0 root         (0) root         (0)     4596 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/geo/raster/conversion.py
+-rwxrwxrwx   0 root         (0) root         (0)    25816 2017-11-02 20:43:28.000000 py_tools_ds-0.9.4/py_tools_ds/geo/raster/reproject.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/geo/raster/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      366 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/geo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4284 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/geo/map_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/py_tools_ds/web/
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/web/network.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/web/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/py_tools_ds/processing/
+-rwxrwxrwx   0 root         (0) root         (0)      611 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/processing/shell.py
+-rw-rw-rw-   0 root         (0) root         (0)       98 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/processing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5618 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/processing/progress_mon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/py_tools_ds/environment/
+-rw-rw-rw-   0 root         (0) root         (0)     1847 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/environment/gdal_env.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/environment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/py_tools_ds/compatibility/
+-rwxrwxrwx   0 root         (0) root         (0)    16693 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/compatibility/gdal.py
+-rwxrwxrwx   0 root         (0) root         (0)     1771 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/compatibility/gdalnumeric.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/py_tools_ds/compatibility/python/
+-rw-rw-rw-   0 root         (0) root         (0)      180 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/compatibility/python/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/compatibility/python/os.py
+-rw-rw-rw-   0 root         (0) root         (0)      108 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/compatibility/python/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       56 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/compatibility/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/py_tools_ds/io/
+-rw-rw-rw-   0 root         (0) root         (0)     1887 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/io/pathgen.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/py_tools_ds/io/raster/
+-rwxrwxrwx   0 root         (0) root         (0)     2586 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/io/raster/gdal.py
+-rw-rw-rw-   0 root         (0) root         (0)       56 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/io/raster/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      144 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/py_tools_ds/compression/
+-rw-rw-rw-   0 root         (0) root         (0)     3340 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/compression/decompress.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/compression/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/py_tools_ds/convenience/
+-rw-rw-rw-   0 root         (0) root         (0)      237 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/convenience/object_oriented.py
+-rw-rw-rw-   0 root         (0) root         (0)      118 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/convenience/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/py_tools_ds/numeric/
+-rw-rw-rw-   0 root         (0) root         (0)      847 2017-11-02 20:48:30.000000 py_tools_ds-0.9.4/py_tools_ds/numeric/array.py
+-rw-rw-rw-   0 root         (0) root         (0)      171 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/numeric/numbers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1892 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/numeric/vector.py
+-rw-rw-rw-   0 root         (0) root         (0)      140 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/py_tools_ds/numeric/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      670 2017-11-02 20:48:30.000000 py_tools_ds-0.9.4/py_tools_ds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1896 2017-11-02 20:48:30.000000 py_tools_ds-0.9.4/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      262 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/tests/CI_docker/
+-rw-rw-rw-   0 root         (0) root         (0)     1208 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/tests/CI_docker/build_testsuite_image.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/tests/CI_docker/context/
+-rw-rw-rw-   0 root         (0) root         (0)     2005 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/tests/CI_docker/context/py_tools_ds_ci.docker
+-rw-rw-rw-   0 root         (0) root         (0)     3149 2017-11-02 20:48:30.000000 py_tools_ds-0.9.4/tests/test_map_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/tests/linting/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/tests/linting/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)      788 2017-11-02 20:48:30.000000 py_tools_ds-0.9.4/tests/test_coord_grid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1820 2017-11-02 20:48:30.000000 py_tools_ds-0.9.4/tests/test_projection.py
+-rw-rw-rw-   0 root         (0) root         (0)       24 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      383 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      173 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)     4179 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2500 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/py_tools_ds.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       18 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/py_tools_ds.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/py_tools_ds.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     2532 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/py_tools_ds.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     4179 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/py_tools_ds.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/py_tools_ds.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/py_tools_ds.egg-info/not-zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     6785 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)       77 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/docs/usage.rst
+-rw-rw-rw-   0 root         (0) root         (0)       33 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/docs/contributing.rst
+-rw-rw-rw-   0 root         (0) root         (0)       27 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/docs/readme.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/docs/_build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/docs/_build/html/
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-11-02 20:49:24.000000 py_tools_ds-0.9.4/docs/_build/html/_static/
+-rw-r--r--   0 root         (0) root         (0)      829 2017-07-02 09:28:03.000000 py_tools_ds-0.9.4/docs/_build/html/_static/comment-close.png
+-rw-r--r--   0 root         (0) root         (0)      286 2017-07-02 09:28:03.000000 py_tools_ds-0.9.4/docs/_build/html/_static/file.png
+-rw-r--r--   0 root         (0) root         (0)      673 2017-07-02 09:28:03.000000 py_tools_ds-0.9.4/docs/_build/html/_static/ajax-loader.gif
+-rw-r--r--   0 root         (0) root         (0)       90 2017-07-02 09:28:03.000000 py_tools_ds-0.9.4/docs/_build/html/_static/minus.png
+-rw-r--r--   0 root         (0) root         (0)      214 2017-07-02 09:28:03.000000 py_tools_ds-0.9.4/docs/_build/html/_static/up-pressed.png
+-rw-r--r--   0 root         (0) root         (0)       90 2017-07-02 09:28:03.000000 py_tools_ds-0.9.4/docs/_build/html/_static/plus.png
+-rw-r--r--   0 root         (0) root         (0)      202 2017-07-02 09:28:03.000000 py_tools_ds-0.9.4/docs/_build/html/_static/down.png
+-rw-r--r--   0 root         (0) root         (0)      203 2017-07-02 09:28:03.000000 py_tools_ds-0.9.4/docs/_build/html/_static/up.png
+-rw-r--r--   0 root         (0) root         (0)      222 2017-07-02 09:28:03.000000 py_tools_ds-0.9.4/docs/_build/html/_static/down-pressed.png
+-rw-r--r--   0 root         (0) root         (0)      641 2017-07-02 09:28:03.000000 py_tools_ds-0.9.4/docs/_build/html/_static/comment.png
+-rw-r--r--   0 root         (0) root         (0)      756 2017-07-02 09:28:03.000000 py_tools_ds-0.9.4/docs/_build/html/_static/comment-bright.png
+-rwxrwxrwx   0 root         (0) root         (0)     8455 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       28 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/docs/authors.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6469 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)      287 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1223 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/docs/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)       28 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/docs/history.rst
+-rw-rw-rw-   0 root         (0) root         (0)       89 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3314 2017-10-25 13:25:33.000000 py_tools_ds-0.9.4/CONTRIBUTING.rst
```

### Comparing `py_tools_ds-0.9.3/LICENSE` & `py_tools_ds-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/py_tools_ds/similarity/raster.py` & `py_tools_ds-0.9.4/py_tools_ds/similarity/raster.py`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/py_tools_ds/dtypes/conversion.py` & `py_tools_ds-0.9.4/py_tools_ds/dtypes/conversion.py`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/py_tools_ds/geo/coord_trafo.py` & `py_tools_ds-0.9.4/py_tools_ds/geo/coord_trafo.py`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/py_tools_ds/geo/vector/geometry.py` & `py_tools_ds-0.9.4/py_tools_ds/geo/vector/geometry.py`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/py_tools_ds/geo/vector/conversion.py` & `py_tools_ds-0.9.4/py_tools_ds/geo/vector/conversion.py`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/py_tools_ds/geo/vector/topology.py` & `py_tools_ds-0.9.4/py_tools_ds/geo/vector/topology.py`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/py_tools_ds/geo/coord_calc.py` & `py_tools_ds-0.9.4/py_tools_ds/geo/coord_calc.py`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/py_tools_ds/geo/coord_grid.py` & `py_tools_ds-0.9.4/py_tools_ds/geo/coord_grid.py`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/py_tools_ds/geo/projection.py` & `py_tools_ds-0.9.4/py_tools_ds/geo/projection.py`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/py_tools_ds/geo/raster/conversion.py` & `py_tools_ds-0.9.4/py_tools_ds/geo/raster/conversion.py`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/py_tools_ds/geo/raster/reproject.py` & `py_tools_ds-0.9.4/py_tools_ds/geo/raster/reproject.py`

 * *Files 4% similar despite different names*

```diff
@@ -236,17 +236,17 @@
                  out_gsd=(None, None), out_bounds=None, out_bounds_prj=None, out_XYdims=(None, None),
                  rspAlg='near', in_nodata=None, out_nodata=None, in_alpha=False,
                  out_alpha=False, targetAlignedPixels=False, gcpList=None, polynomialOrder=None, options=None,
                  transformerOptions=None, warpOptions=None, CPUs=1, warpMemoryLimit=0, progress=True, q=False):
     # type: () -> (np.ndarray, tuple, str)
     """
 
-    :param ndarray:             the numpy array to be warped
-    :param in_gt:               input GDAL geotransform
-    :param in_prj:              input GDAL projection (WKT string, 'EPSG:1234', <EPSG_int>),
+    :param ndarray:             numpy array to be warped (or a list of numpy arrays (requires lists for in_gt/in_prj))
+    :param in_gt:               input GDAL geotransform (or a list of GDAL geotransforms)
+    :param in_prj:              input GDAL projection or list of projections (WKT string, 'EPSG:1234', <EPSG_int>),
                                 default: "LOCAL_CS[\"MAP\"]"
     :param out_prj:             output GDAL projection (WKT string, 'EPSG:1234', <EPSG_int>),
                                 default: "LOCAL_CS[\"MAP\"]"
     :param out_dtype:           gdal.DataType
     :param out_gsd:
     :param out_bounds:          [xmin,ymin,xmax,ymax] set georeferenced extents of output file to be created,
                                 e.g. [440720, 3750120, 441920, 3751320])
@@ -284,28 +284,37 @@
     # assume local coordinates if no projections are given
     if not in_prj and not out_prj:
         if out_bounds_prj and not out_bounds_prj.startswith('LOCAL_CS'):
             raise ValueError("'out_bounds_prj' cannot have a projection if 'in_prj' and 'out_prj' are not given.")
         in_prj = out_prj = out_bounds_prj = "LOCAL_CS[\"MAP\"]"
 
     # assertions
-    assert str(np.dtype(ndarray.dtype)) in dTypeDic_NumPy2GDAL, "Unknown target datatype '%s'." % ndarray.dtype
     if rspAlg == 'average':
         is_avail_rsp_average = int(gdal.VersionInfo()[0]) >= 2
         if not is_avail_rsp_average:
             warnings.warn("The GDAL version on this machine does not yet support the resampling algorithm 'average'. "
                           "'cubic' is used instead. To avoid this please update GDAL to a version above 2.0.0!")
             rspAlg = 'cubic'
 
+    if not isinstance(ndarray, (list, tuple)):
+        assert str(np.dtype(ndarray.dtype)) in dTypeDic_NumPy2GDAL, "Unknown target datatype '%s'." % ndarray.dtype
+    else:
+        assert str(np.dtype(ndarray[0].dtype)) in dTypeDic_NumPy2GDAL, "Unknown target datatype '%s'." % ndarray.dtype
+        assert isinstance(in_gt, (list, tuple)), "If 'ndarray' is a list, 'in_gt' must also be a list!"
+        assert isinstance(in_prj, (list, tuple)), "If 'ndarray' is a list, 'in_prj' must also be a list!"
+        assert len(list(set([arr.dtype for arr in ndarray]))) == 1,  "Data types of input ndarray list must be equal."
+
     def get_SRS(prjArg):
         return prjArg if isinstance(prjArg, str) and prjArg.startswith('EPSG:') else \
             'EPSG:%s' % prjArg if isinstance(prjArg, int) else prjArg
 
     def get_GDT(DT): return dTypeDic_NumPy2GDAL[str(np.dtype(DT))]
 
+    in_dtype_np = ndarray.dtype if not isinstance(ndarray, (list, tuple)) else ndarray[0].dtype
+
     # # not yet implemented
     # # TODO cutline from OGR datasource. => implement input shapefile or Geopandas dataframe
     # cutlineDSName = 'data/cutline.vrt'  # '/vsimem/cutline.shp'
     # cutlineLayer = 'cutline'
     # cropToCutline = False
     # cutlineSQL = 'SELECT * FROM cutline'
     # cutlineWhere = '1 = 1'
@@ -381,15 +390,19 @@
           metadataConflictValue --- metadata data conflict value
           setColorInterpretation --- whether to force color interpretation of input bands to output bands
           callback --- callback method
           callback_data --- user data for callback  # value for last parameter of progress callback
     """
 
     # get input dataset (in-MEM)
-    in_ds = get_GDAL_ds_inmem(ndarray, in_gt, in_prj)
+    if not isinstance(ndarray, (list, tuple)):
+        in_ds = get_GDAL_ds_inmem(ndarray, in_gt, in_prj)
+    else:
+        # list of ndarrays
+        in_ds = [get_GDAL_ds_inmem(arr, gt, prj) for arr, gt, prj in zip(ndarray, in_gt, in_prj)]
 
     # set RPCs
     # if rpcList:
     #    in_ds.SetMetadata(rpc, "RPC")
     #    transformerOptions = ['RPC_DEM=data/warp_52_dem.tif']
 
     if CPUs is None or CPUs > 1:
@@ -412,15 +425,15 @@
         # NOTE: options = ['SPARSE_OK=YES'] ## => what is that for?
 
     # GDAL Warp
     gdal_Warp = get_gdal_func('Warp')
     res_ds = gdal_Warp(
         '', in_ds, format='MEM',
         dstSRS=get_SRS(out_prj),
-        outputType=get_GDT(out_dtype) if out_dtype else get_GDT(ndarray.dtype),
+        outputType=get_GDT(out_dtype) if out_dtype else get_GDT(in_dtype_np),
         xRes=out_gsd[0],
         yRes=out_gsd[1],
         outputBounds=out_bounds,
         outputBoundsSRS=get_SRS(out_bounds_prj),
         width=out_XYdims[0],
         height=out_XYdims[1],
         resampleAlg=rspAlg,
@@ -453,16 +466,16 @@
     res_gt = res_ds.GetGeoTransform()
     res_prj = res_ds.GetProjection()
 
     # cleanup
     del in_ds, res_ds
 
     # dtype check -> possibly dtype had to be changed for GDAL compatibility
-    if ndarray.dtype != res_arr.dtype:
-        res_arr = res_arr.astype(ndarray.dtype)
+    if in_dtype_np != res_arr.dtype:
+        res_arr = res_arr.astype(in_dtype_np)
 
     # test output
     if out_prj and prj_equal(out_prj, 4626):
         assert -180 < res_gt[0] < 180 and -90 < res_gt[3] < 90, 'Testing of gdal_warp output failed.'
 
     # output bounds verification
     if out_bounds:
```

### Comparing `py_tools_ds-0.9.3/py_tools_ds/geo/map_info.py` & `py_tools_ds-0.9.4/py_tools_ds/geo/map_info.py`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/py_tools_ds/web/network.py` & `py_tools_ds-0.9.4/py_tools_ds/web/network.py`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/py_tools_ds/processing/shell.py` & `py_tools_ds-0.9.4/py_tools_ds/processing/shell.py`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/py_tools_ds/processing/progress_mon.py` & `py_tools_ds-0.9.4/py_tools_ds/processing/progress_mon.py`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/py_tools_ds/environment/gdal_env.py` & `py_tools_ds-0.9.4/py_tools_ds/environment/gdal_env.py`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/py_tools_ds/compatibility/gdal.py` & `py_tools_ds-0.9.4/py_tools_ds/compatibility/gdal.py`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/py_tools_ds/compatibility/gdalnumeric.py` & `py_tools_ds-0.9.4/py_tools_ds/compatibility/gdalnumeric.py`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/py_tools_ds/io/pathgen.py` & `py_tools_ds-0.9.4/py_tools_ds/io/pathgen.py`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/py_tools_ds/io/raster/gdal.py` & `py_tools_ds-0.9.4/py_tools_ds/io/raster/gdal.py`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/py_tools_ds/compression/decompress.py` & `py_tools_ds-0.9.4/py_tools_ds/compression/decompress.py`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/py_tools_ds/numeric/array.py` & `py_tools_ds-0.9.4/py_tools_ds/numeric/array.py`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/py_tools_ds/numeric/vector.py` & `py_tools_ds-0.9.4/py_tools_ds/numeric/vector.py`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/py_tools_ds/__init__.py` & `py_tools_ds-0.9.4/py_tools_ds/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from __future__ import (division, print_function, absolute_import, unicode_literals)
 
-__version__ = '0.9.3'
-__versionalias__ = '20171012_02'
+__version__ = '0.9.4'
+__versionalias__ = '20171102_01'
 __author__ = 'Daniel Scheffler'
 
 # Validate GDAL version
 try:
     import gdal
     import gdalnumeric
 except ImportError:
```

### Comparing `py_tools_ds-0.9.3/setup.py` & `py_tools_ds-0.9.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 requirements = ['gdal', 'numpy', 'shapely', 'six', 'rasterio', 'pandas', 'geopandas',
                 'scikit-image', 'pyproj']
 setup_requirements = []  # TODO(danschef): put setup requirements (distutils extensions, etc.) here
 test_requirements = requirements + ["coverage", "nose", "nose2", "nose-htmloutput", "rednose"]
 
 setup(
     name='py_tools_ds',
-    version='0.9.3',
+    version='0.9.4',
     description="A collection of Python tools by Daniel Scheffler.",
     long_description=readme + '\n\n' + history,
     author="Daniel Scheffler",
     author_email='daniel.scheffler@gfz-potsdam.de',
     url='https://gitext.gfz-potsdam.de/danschef/py_tools_ds',
     packages=find_packages(),  # searches for packages with an __init__.py and returns them as properly formatted list
     package_dir={'py_tools_ds': 'py_tools_ds'},
```

### Comparing `py_tools_ds-0.9.3/tests/CI_docker/build_testsuite_image.sh` & `py_tools_ds-0.9.4/tests/CI_docker/build_testsuite_image.sh`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/tests/CI_docker/context/py_tools_ds_ci.docker` & `py_tools_ds-0.9.4/tests/CI_docker/context/py_tools_ds_ci.docker`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/tests/test_map_info.py` & `py_tools_ds-0.9.4/tests/test_map_info.py`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/tests/test_coord_grid.py` & `py_tools_ds-0.9.4/tests/test_coord_grid.py`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/tests/test_projection.py` & `py_tools_ds-0.9.4/tests/test_projection.py`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/PKG-INFO` & `py_tools_ds-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: py_tools_ds
-Version: 0.9.3
+Version: 0.9.4
 Summary: A collection of Python tools by Daniel Scheffler.
 Home-page: https://gitext.gfz-potsdam.de/danschef/py_tools_ds
 Author: Daniel Scheffler
 Author-email: daniel.scheffler@gfz-potsdam.de
 License: GNU General Public License v3
 Description-Content-Type: UNKNOWN
 Description: ===========
@@ -57,15 +57,15 @@
         Using conda_, the recommended approach is:
         
          .. code-block:: console
         
             # create virtual environment for py_tools_ds, this is optional
             conda create -y -q --name py_tools_ds python=3
             source activate py_tools_ds
-            conda install -y -q -c conda-forge numpy gdal scikit-image pyproj rasterio shapely
+            conda install -y -q -c conda-forge numpy gdal scikit-image pyproj rasterio shapely pandas
         
         * To install py_tools_ds, use the pip installer:
         
          .. code-block:: console
         
             pip install py_tools_ds
```

### Comparing `py_tools_ds-0.9.3/README.rst` & `py_tools_ds-0.9.4/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 Using conda_, the recommended approach is:
 
  .. code-block:: console
 
     # create virtual environment for py_tools_ds, this is optional
     conda create -y -q --name py_tools_ds python=3
     source activate py_tools_ds
-    conda install -y -q -c conda-forge numpy gdal scikit-image pyproj rasterio shapely
+    conda install -y -q -c conda-forge numpy gdal scikit-image pyproj rasterio shapely pandas
 
 * To install py_tools_ds, use the pip installer:
 
  .. code-block:: console
 
     pip install py_tools_ds
```

### Comparing `py_tools_ds-0.9.3/py_tools_ds.egg-info/SOURCES.txt` & `py_tools_ds-0.9.4/py_tools_ds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/py_tools_ds.egg-info/PKG-INFO` & `py_tools_ds-0.9.4/py_tools_ds.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: py-tools-ds
-Version: 0.9.3
+Version: 0.9.4
 Summary: A collection of Python tools by Daniel Scheffler.
 Home-page: https://gitext.gfz-potsdam.de/danschef/py_tools_ds
 Author: Daniel Scheffler
 Author-email: daniel.scheffler@gfz-potsdam.de
 License: GNU General Public License v3
 Description-Content-Type: UNKNOWN
 Description: ===========
@@ -57,15 +57,15 @@
         Using conda_, the recommended approach is:
         
          .. code-block:: console
         
             # create virtual environment for py_tools_ds, this is optional
             conda create -y -q --name py_tools_ds python=3
             source activate py_tools_ds
-            conda install -y -q -c conda-forge numpy gdal scikit-image pyproj rasterio shapely
+            conda install -y -q -c conda-forge numpy gdal scikit-image pyproj rasterio shapely pandas
         
         * To install py_tools_ds, use the pip installer:
         
          .. code-block:: console
         
             pip install py_tools_ds
```

### Comparing `py_tools_ds-0.9.3/docs/Makefile` & `py_tools_ds-0.9.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/docs/_build/html/_static/comment-close.png` & `py_tools_ds-0.9.4/docs/_build/html/_static/comment-close.png`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/docs/_build/html/_static/ajax-loader.gif` & `py_tools_ds-0.9.4/docs/_build/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/docs/_build/html/_static/comment.png` & `py_tools_ds-0.9.4/docs/_build/html/_static/comment.png`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/docs/_build/html/_static/comment-bright.png` & `py_tools_ds-0.9.4/docs/_build/html/_static/comment-bright.png`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/docs/conf.py` & `py_tools_ds-0.9.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/docs/make.bat` & `py_tools_ds-0.9.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/docs/installation.rst` & `py_tools_ds-0.9.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `py_tools_ds-0.9.3/CONTRIBUTING.rst` & `py_tools_ds-0.9.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

