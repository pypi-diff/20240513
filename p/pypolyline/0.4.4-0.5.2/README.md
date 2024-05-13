# Comparing `tmp/pypolyline-0.4.4.tar.gz` & `tmp/pypolyline-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypolyline-0.4.4.tar", last modified: Fri May  3 17:17:56 2024, max compression
+gzip compressed data, was "pypolyline-0.5.2.tar", last modified: Mon May 13 21:26:23 2024, max compression
```

## Comparing `pypolyline-0.4.4.tar` & `pypolyline-0.5.2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:56.122171 pypolyline-0.4.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:56.118171 pypolyline-0.4.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-03 17:17:48.000000 pypolyline-0.4.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:56.118171 pypolyline-0.4.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-05-03 17:17:48.000000 pypolyline-0.4.4/.github/workflows/wheels.yml
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-03 17:17:48.000000 pypolyline-0.4.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-03 17:17:48.000000 pypolyline-0.4.4/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-05-03 17:17:56.122171 pypolyline-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-03 17:17:48.000000 pypolyline-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:56.122171 pypolyline-0.4.4/benches/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-03 17:17:48.000000 pypolyline-0.4.4/benches/benchmark_cgg.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-03 17:17:48.000000 pypolyline-0.4.4/benches/benchmark_python.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-03 17:17:48.000000 pypolyline-0.4.4/benches/benchmark_rust.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-03 17:17:48.000000 pypolyline-0.4.4/benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-03 17:17:48.000000 pypolyline-0.4.4/license.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-03 17:17:48.000000 pypolyline-0.4.4/pypolyline_p.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-03 17:17:48.000000 pypolyline-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 17:17:56.122171 pypolyline-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-03 17:17:48.000000 pypolyline-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:56.122171 pypolyline-0.4.4/src/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-03 17:17:56.000000 pypolyline-0.4.4/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:56.122171 pypolyline-0.4.4/src/pypolyline/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-03 17:17:48.000000 pypolyline-0.4.4/src/pypolyline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-03 17:17:48.000000 pypolyline-0.4.4/src/pypolyline/cutil.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-03 17:17:48.000000 pypolyline-0.4.4/src/pypolyline/pypolyline_p.pxd
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-03 17:17:48.000000 pypolyline-0.4.4/src/pypolyline/stdbool.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:56.122171 pypolyline-0.4.4/src/pypolyline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-05-03 17:17:56.000000 pypolyline-0.4.4/src/pypolyline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-03 17:17:56.000000 pypolyline-0.4.4/src/pypolyline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:17:56.000000 pypolyline-0.4.4/src/pypolyline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-03 17:17:56.000000 pypolyline-0.4.4/src/pypolyline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-03 17:17:56.000000 pypolyline-0.4.4/src/pypolyline.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:56.122171 pypolyline-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-05-03 17:17:48.000000 pypolyline-0.4.4/tests/test_pypolyline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:26:23.148559 pypolyline-0.5.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:26:23.144559 pypolyline-0.5.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-13 21:26:14.000000 pypolyline-0.5.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:26:23.144559 pypolyline-0.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-05-13 21:26:14.000000 pypolyline-0.5.2/.github/workflows/wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-13 21:26:14.000000 pypolyline-0.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-13 21:26:14.000000 pypolyline-0.5.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-05-13 21:26:23.148559 pypolyline-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-13 21:26:14.000000 pypolyline-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:26:23.144559 pypolyline-0.5.2/benches/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-13 21:26:14.000000 pypolyline-0.5.2/benches/benchmark_cgg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-13 21:26:14.000000 pypolyline-0.5.2/benches/benchmark_flexpolyline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-13 21:26:14.000000 pypolyline-0.5.2/benches/benchmark_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-13 21:26:14.000000 pypolyline-0.5.2/benches/benchmark_rust.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-13 21:26:14.000000 pypolyline-0.5.2/benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-13 21:26:14.000000 pypolyline-0.5.2/license.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-13 21:26:14.000000 pypolyline-0.5.2/pypolyline_p.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-13 21:26:14.000000 pypolyline-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 21:26:23.148559 pypolyline-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-13 21:26:14.000000 pypolyline-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:26:23.144559 pypolyline-0.5.2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-13 21:26:23.000000 pypolyline-0.5.2/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:26:23.144559 pypolyline-0.5.2/src/pypolyline/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-13 21:26:14.000000 pypolyline-0.5.2/src/pypolyline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-13 21:26:14.000000 pypolyline-0.5.2/src/pypolyline/cutil.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-13 21:26:14.000000 pypolyline-0.5.2/src/pypolyline/pypolyline_p.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-13 21:26:14.000000 pypolyline-0.5.2/src/pypolyline/stdbool.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:26:23.148559 pypolyline-0.5.2/src/pypolyline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-05-13 21:26:23.000000 pypolyline-0.5.2/src/pypolyline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-13 21:26:23.000000 pypolyline-0.5.2/src/pypolyline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 21:26:23.000000 pypolyline-0.5.2/src/pypolyline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-13 21:26:23.000000 pypolyline-0.5.2/src/pypolyline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-13 21:26:23.000000 pypolyline-0.5.2/src/pypolyline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:26:23.148559 pypolyline-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6288 2024-05-13 21:26:14.000000 pypolyline-0.5.2/tests/test_pypolyline.py
```

### Comparing `pypolyline-0.4.4/.github/workflows/wheels.yml` & `pypolyline-0.5.2/.github/workflows/wheels.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 name: Build and test wheels, release on new tag
+
+permissions:
+  id-token: write
+  attestations: write
+  contents: read
+
 env:
   librepo: polyline-ffi
   rustlib: polylineffi
   wheelname: pypolyline
 
 on: [push, pull_request]
 
@@ -93,30 +99,35 @@
         run:   |
                tar -xvf "rustlib/${{ env.filename }}" -C src/${{ env.wheelname }}
                mkdir wheelhouse
                git status
         shell: bash
 
       - name: Build and Test Wheels
-        uses: pypa/cibuildwheel@v2.17.0
+        uses: pypa/cibuildwheel@v2.18.0
         env:
-          CIBW_BEFORE_BUILD_MACOS: pip install numpy cython
-          CIBW_BEFORE_BUILD: pip install numpy cython
-          CIBW_TEST_REQUIRES: setuptools pytest numpy cython
+          CIBW_TEST_REQUIRES: pytest
           CIBW_TEST_COMMAND: 'pytest {package}'
           CIBW_BUILD: ${{ matrix.pybuilds }}
           CIBW_ARCHS_MACOS: ${{ matrix.arch }}
           CIBW_ARCHS_LINUX: "auto aarch64"
           CIBW_TEST_SKIP: "*:arm64"
 
+      - id: attest
+        name: Attest Build Provenance
+        uses: actions/attest-build-provenance@v1
+        with:
+          subject-path: "./wheelhouse/*.whl"
+
       - uses: actions/upload-artifact@v4
         name: Upload repaired wheels as artifact
         with:
-          name: wheels-${{ matrix.os }}-${{ matrix.arch }}
+          name: cibw-wheels-${{ matrix.os }}-${{ strategy.job-index }}
           path: |
+            ${{ steps.attest.outputs.bundle-path }}
             ./wheelhouse/*.whl
             ./wheelhouse/*.so
             ./wheelhouse/*.dylib
             ./wheelhouse/*.lib
             ./wheelhouse/*.dll
 
   make_sdist:
@@ -155,14 +166,21 @@
     - name: Download compressed artifacts
       id: download
       uses: actions/download-artifact@v4
       with:
         path: ./artifacts
         merge-multiple: true
 
+    - name: Remove attestation dir, copy wheels into main dir, remove subdirs
+      run:   |
+             rm -rf "${{ steps.download.outputs.download-path }}"/_temp
+             cp "${{ steps.download.outputs.download-path }}"/"${{ env.wheelname }}"/"${{ env.wheelname }}"/wheelhouse/*.whl ${{ steps.download.outputs.download-path }}
+             rm -rf "${{ steps.download.outputs.download-path }}"/"${{ env.wheelname }}"
+      shell: bash
+
     - name: Display structure of downloaded files
       run: ls -R ./artifacts
 
     - name: Create release and upload wheels
       uses: ncipollo/release-action@v1
       with:
         allowUpdates: true
```

### Comparing `pypolyline-0.4.4/PKG-INFO` & `pypolyline-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypolyline
-Version: 0.4.4
+Version: 0.5.2
 Summary: Fast Google Polyline encoding and decoding using Rust FFI
 Author-email: Stephan Hügel <urschrei@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 Stephan Hügel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -50,15 +50,14 @@
 
 ![example workflow](https://github.com/urschrei/pypolyline/actions/workflows/wheels.yml/badge.svg) [![Coverage Status](https://coveralls.io/repos/github/urschrei/pypolyline/badge.svg?branch=master)](https://coveralls.io/github/urschrei/pypolyline?branch=master) [![Downloads](https://pepy.tech/badge/pypolyline)](https://pepy.tech/project/pypolyline)[![DOI](https://zenodo.org/badge/63355673.svg)](https://zenodo.org/badge/latestdoi/63355673)
 
 # Fast Google [Polyline](https://developers.google.com/maps/documentation/utilities/polylinealgorithm) Encoding and Decoding
 
 ## Installation
 `pip install pypolyline`  
-Please use a recent (>= 8.1.2) version of `pip`.
 
 ### Supported Python Versions
 - Python 3.8
 - Python 3.9
 - Python 3.10
 - Python 3.11
 - Python 3.12
@@ -85,24 +84,24 @@
 # precision is 5 for Google Polyline, 6 for OSRM / Valhalla
 polyline = encode_coordinates(coords, 5)
 # polyline is 'ynh`IcftoCyq@Ne@ncBds@EEycB'
 decoded_coords = decode_polyline(polyline, 5)
 ```
 
 ## Error Handling
-Failure to encode coordinates, or to decode a supplied Polyline, will raise a `RuntimeError` which can be caught.
+Failure to encode coordinates, or to decode a supplied Polyline, will raise a `RuntimeError` containing information about the invalid input.
 
 
 ## How it Works
 FFI and a [Rust binary](https://github.com/urschrei/polyline-ffi)
 
 ## Is It Fast
 …Yes.  
 You can verify this by installing the `polyline` package, then running [`benchmarks.py`](benchmarks.py), a calibrated benchmark using `cProfile`.  
-On a 1.8 GHz Intel Core i7, The pure-Python test runs in ~5000 ms and The Rust + Cython benchmark runs in around 300 ms (177 % faster).
+On an M2 MBP, The [pure-Python](https://pypi.org/project/polyline/) test runs in ~2500 ms, the [Flexpolyline](https://pypi.org/project/flexpolyline/) benchmark runs in ~1500 ms and The Rust + Cython benchmark runs in around 80 ms (30 x and 17.5 x faster, respectively).
 
 ## License
 [MIT](license.txt)
 
 ## Citing `Pypolyline`
 If Pypolyline has been significant in your research, and you would like to acknowledge the project in your academic publication, we suggest citing it as follows (example in APA style, 7th edition):
```

### Comparing `pypolyline-0.4.4/README.md` & `pypolyline-0.5.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 ![example workflow](https://github.com/urschrei/pypolyline/actions/workflows/wheels.yml/badge.svg) [![Coverage Status](https://coveralls.io/repos/github/urschrei/pypolyline/badge.svg?branch=master)](https://coveralls.io/github/urschrei/pypolyline?branch=master) [![Downloads](https://pepy.tech/badge/pypolyline)](https://pepy.tech/project/pypolyline)[![DOI](https://zenodo.org/badge/63355673.svg)](https://zenodo.org/badge/latestdoi/63355673)
 
 # Fast Google [Polyline](https://developers.google.com/maps/documentation/utilities/polylinealgorithm) Encoding and Decoding
 
 ## Installation
 `pip install pypolyline`  
-Please use a recent (>= 8.1.2) version of `pip`.
 
 ### Supported Python Versions
 - Python 3.8
 - Python 3.9
 - Python 3.10
 - Python 3.11
 - Python 3.12
@@ -35,24 +34,24 @@
 # precision is 5 for Google Polyline, 6 for OSRM / Valhalla
 polyline = encode_coordinates(coords, 5)
 # polyline is 'ynh`IcftoCyq@Ne@ncBds@EEycB'
 decoded_coords = decode_polyline(polyline, 5)
 ```
 
 ## Error Handling
-Failure to encode coordinates, or to decode a supplied Polyline, will raise a `RuntimeError` which can be caught.
+Failure to encode coordinates, or to decode a supplied Polyline, will raise a `RuntimeError` containing information about the invalid input.
 
 
 ## How it Works
 FFI and a [Rust binary](https://github.com/urschrei/polyline-ffi)
 
 ## Is It Fast
 …Yes.  
 You can verify this by installing the `polyline` package, then running [`benchmarks.py`](benchmarks.py), a calibrated benchmark using `cProfile`.  
-On a 1.8 GHz Intel Core i7, The pure-Python test runs in ~5000 ms and The Rust + Cython benchmark runs in around 300 ms (177 % faster).
+On an M2 MBP, The [pure-Python](https://pypi.org/project/polyline/) test runs in ~2500 ms, the [Flexpolyline](https://pypi.org/project/flexpolyline/) benchmark runs in ~1500 ms and The Rust + Cython benchmark runs in around 80 ms (30 x and 17.5 x faster, respectively).
 
 ## License
 [MIT](license.txt)
 
 ## Citing `Pypolyline`
 If Pypolyline has been significant in your research, and you would like to acknowledge the project in your academic publication, we suggest citing it as follows (example in APA style, 7th edition):
```

### Comparing `pypolyline-0.4.4/license.txt` & `pypolyline-0.5.2/license.txt`

 * *Files identical despite different names*

### Comparing `pypolyline-0.4.4/pyproject.toml` & `pypolyline-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pypolyline-0.4.4/setup.py` & `pypolyline-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `pypolyline-0.4.4/src/pypolyline/cutil.pyx` & `pypolyline-0.5.2/src/pypolyline/cutil.pyx`

 * *Files 10% similar despite different names*

```diff
@@ -55,16 +55,21 @@
     cdef double[:,::1] ncoords = np.array(coords, dtype=np.float64)
     cdef ExternalArray coords_ffi
     coords_ffi.data = <void*>&ncoords[0, 0]
     coords_ffi.len = ncoords.shape[0]
     cdef char* result = encode_coordinates_ffi(coords_ffi, precision)
     cdef bytes polyline = result
     drop_cstring(result)
-    if np.char.startswith(polyline, b"Latitude") or np.char.startswith(polyline, b"Longitude"):
-        raise RuntimeError("The input coordinates could not be encoded")
+    if (
+        np.char.startswith(polyline, b"latitude") or
+        np.char.startswith(polyline, b"longitude") or
+        np.char.startswith(polyline, b"no longitude") or
+        np.char.startswith(polyline, b"couldn't")
+    ):
+        raise RuntimeError(polyline)
     return polyline
 
 def decode_polyline(bytes polyline, int precision):
     """
     Decode an encoded Polyline to coordinates.
     Input: a Polyline string, and a precision int (5 for Google, 6 for OSM-derived).
     Output: a list of lat, lon coordinates.
```

### Comparing `pypolyline-0.4.4/src/pypolyline.egg-info/PKG-INFO` & `pypolyline-0.5.2/src/pypolyline.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypolyline
-Version: 0.4.4
+Version: 0.5.2
 Summary: Fast Google Polyline encoding and decoding using Rust FFI
 Author-email: Stephan Hügel <urschrei@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 Stephan Hügel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -50,15 +50,14 @@
 
 ![example workflow](https://github.com/urschrei/pypolyline/actions/workflows/wheels.yml/badge.svg) [![Coverage Status](https://coveralls.io/repos/github/urschrei/pypolyline/badge.svg?branch=master)](https://coveralls.io/github/urschrei/pypolyline?branch=master) [![Downloads](https://pepy.tech/badge/pypolyline)](https://pepy.tech/project/pypolyline)[![DOI](https://zenodo.org/badge/63355673.svg)](https://zenodo.org/badge/latestdoi/63355673)
 
 # Fast Google [Polyline](https://developers.google.com/maps/documentation/utilities/polylinealgorithm) Encoding and Decoding
 
 ## Installation
 `pip install pypolyline`  
-Please use a recent (>= 8.1.2) version of `pip`.
 
 ### Supported Python Versions
 - Python 3.8
 - Python 3.9
 - Python 3.10
 - Python 3.11
 - Python 3.12
@@ -85,24 +84,24 @@
 # precision is 5 for Google Polyline, 6 for OSRM / Valhalla
 polyline = encode_coordinates(coords, 5)
 # polyline is 'ynh`IcftoCyq@Ne@ncBds@EEycB'
 decoded_coords = decode_polyline(polyline, 5)
 ```
 
 ## Error Handling
-Failure to encode coordinates, or to decode a supplied Polyline, will raise a `RuntimeError` which can be caught.
+Failure to encode coordinates, or to decode a supplied Polyline, will raise a `RuntimeError` containing information about the invalid input.
 
 
 ## How it Works
 FFI and a [Rust binary](https://github.com/urschrei/polyline-ffi)
 
 ## Is It Fast
 …Yes.  
 You can verify this by installing the `polyline` package, then running [`benchmarks.py`](benchmarks.py), a calibrated benchmark using `cProfile`.  
-On a 1.8 GHz Intel Core i7, The pure-Python test runs in ~5000 ms and The Rust + Cython benchmark runs in around 300 ms (177 % faster).
+On an M2 MBP, The [pure-Python](https://pypi.org/project/polyline/) test runs in ~2500 ms, the [Flexpolyline](https://pypi.org/project/flexpolyline/) benchmark runs in ~1500 ms and The Rust + Cython benchmark runs in around 80 ms (30 x and 17.5 x faster, respectively).
 
 ## License
 [MIT](license.txt)
 
 ## Citing `Pypolyline`
 If Pypolyline has been significant in your research, and you would like to acknowledge the project in your academic publication, we suggest citing it as follows (example in APA style, 7th edition):
```

### Comparing `pypolyline-0.4.4/src/pypolyline.egg-info/SOURCES.txt` & `pypolyline-0.5.2/src/pypolyline.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 license.txt
 pypolyline_p.pxd
 pyproject.toml
 setup.py
 .github/dependabot.yml
 .github/workflows/wheels.yml
 benches/benchmark_cgg.py
+benches/benchmark_flexpolyline.py
 benches/benchmark_python.py
 benches/benchmark_rust.py
 src/_version.py
 src/pypolyline/__init__.py
 src/pypolyline/cutil.pyx
 src/pypolyline/pypolyline_p.pxd
 src/pypolyline/stdbool.h
```

### Comparing `pypolyline-0.4.4/tests/test_pypolyline.py` & `pypolyline-0.5.2/tests/test_pypolyline.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,16 @@
         """Test that bad Polylines throw the correct error"""
         with pytest.raises(RuntimeError) as exc_info:
             cdecode_polyline(self.bad_polyline, 6)
         assert str(exc_info.value) == "Polyline could not be decoded. Is it valid?"
 
     def testEncodeBadCoordinates(self):
         """Test that bad Polylines throw the correct error"""
-        with pytest.raises(RuntimeError) as exc_info:
+        with pytest.raises(RuntimeError) as _:
             cencode_coordinates(self.bad_coordinates, 6)
-        assert str(exc_info.value) == "The input coordinates could not be encoded"
 
     # def testEncodeBadCoordinatesB(self):
     #     """Test that bad Polylines throw the correct error"""
     #     # with pytest.raises(RuntimeError) as exc_info:
     #     res = cencode_coordinates(self.bad_coordinates, 6)
     #     self.assertEqual(res, "ug")
     #     # assert str(exc_info.value) == "The input coordinates could not be encoded"
```

