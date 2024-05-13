# Comparing `tmp/rs-booster-0.1.1.tar.gz` & `tmp/rs-booster-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rs-booster-0.1.1.tar", last modified: Mon Jul 31 20:51:43 2023, max compression
+gzip compressed data, was "rs-booster-0.1.2.tar", last modified: Mon May 13 18:28:40 2024, max compression
```

## Comparing `rs-booster-0.1.1.tar` & `rs-booster-0.1.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:43.283376 rs-booster-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-31 20:51:21.000000 rs-booster-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-31 20:51:21.000000 rs-booster-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-31 20:51:43.283376 rs-booster-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-31 20:51:21.000000 rs-booster-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:43.283376 rs-booster-0.1.1/rs_booster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-31 20:51:43.000000 rs-booster-0.1.1/rs_booster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-31 20:51:43.000000 rs-booster-0.1.1/rs_booster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 20:51:43.000000 rs-booster-0.1.1/rs_booster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-31 20:51:43.000000 rs-booster-0.1.1/rs_booster.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-31 20:51:43.000000 rs-booster-0.1.1/rs_booster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-31 20:51:43.000000 rs-booster-0.1.1/rs_booster.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:43.283376 rs-booster-0.1.1/rsbooster/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:43.283376 rs-booster-0.1.1/rsbooster/diffmaps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/diffmaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/diffmaps/diffmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/diffmaps/internaldiffmap.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/diffmaps/weights.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:43.283376 rs-booster-0.1.1/rsbooster/esf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/esf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/esf/extrapolate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:43.283376 rs-booster-0.1.1/rsbooster/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/io/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/io/precog2mtz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:43.283376 rs-booster-0.1.1/rsbooster/realspace/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/realspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/realspace/find_peaks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:43.283376 rs-booster-0.1.1/rsbooster/scaleit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/scaleit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/scaleit/scaleit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:43.283376 rs-booster-0.1.1/rsbooster/stats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/stats/ccanom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/stats/cchalf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/stats/ccpred.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/stats/ccsym.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/stats/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:43.283376 rs-booster-0.1.1/rsbooster/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/utils/rfree.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-31 20:51:43.287376 rs-booster-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-31 20:51:21.000000 rs-booster-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:43.283376 rs-booster-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:21.000000 rs-booster-0.1.1/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      977 2023-07-31 20:51:21.000000 rs-booster-0.1.1/tests/test_rfree.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-31 20:51:21.000000 rs-booster-0.1.1/tests/test_rsbooster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:28:40.718176 rs-booster-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-13 18:28:24.000000 rs-booster-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-13 18:28:24.000000 rs-booster-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-13 18:28:40.718176 rs-booster-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-13 18:28:24.000000 rs-booster-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:28:40.714176 rs-booster-0.1.2/rs_booster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-13 18:28:40.000000 rs-booster-0.1.2/rs_booster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-13 18:28:40.000000 rs-booster-0.1.2/rs_booster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 18:28:40.000000 rs-booster-0.1.2/rs_booster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-13 18:28:40.000000 rs-booster-0.1.2/rs_booster.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-13 18:28:40.000000 rs-booster-0.1.2/rs_booster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 18:28:40.000000 rs-booster-0.1.2/rs_booster.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:28:40.714176 rs-booster-0.1.2/rsbooster/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 18:28:24.000000 rs-booster-0.1.2/rsbooster/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-13 18:28:24.000000 rs-booster-0.1.2/rsbooster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:28:40.714176 rs-booster-0.1.2/rsbooster/diffmaps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:28:24.000000 rs-booster-0.1.2/rsbooster/diffmaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-13 18:28:24.000000 rs-booster-0.1.2/rsbooster/diffmaps/diffmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-13 18:28:24.000000 rs-booster-0.1.2/rsbooster/diffmaps/internaldiffmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-13 18:28:24.000000 rs-booster-0.1.2/rsbooster/diffmaps/weights.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:28:40.714176 rs-booster-0.1.2/rsbooster/esf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:28:24.000000 rs-booster-0.1.2/rsbooster/esf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-05-13 18:28:24.000000 rs-booster-0.1.2/rsbooster/esf/extrapolate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:28:40.714176 rs-booster-0.1.2/rsbooster/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:28:24.000000 rs-booster-0.1.2/rsbooster/io/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2936 2024-05-13 18:28:24.000000 rs-booster-0.1.2/rsbooster/io/precog2mtz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:28:40.714176 rs-booster-0.1.2/rsbooster/realspace/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:28:24.000000 rs-booster-0.1.2/rsbooster/realspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9940 2024-05-13 18:28:24.000000 rs-booster-0.1.2/rsbooster/realspace/find_peaks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:28:40.714176 rs-booster-0.1.2/rsbooster/scaleit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:28:24.000000 rs-booster-0.1.2/rsbooster/scaleit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-13 18:28:24.000000 rs-booster-0.1.2/rsbooster/scaleit/scaleit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:28:40.714176 rs-booster-0.1.2/rsbooster/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:28:24.000000 rs-booster-0.1.2/rsbooster/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-13 18:28:24.000000 rs-booster-0.1.2/rsbooster/stats/ccanom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-13 18:28:24.000000 rs-booster-0.1.2/rsbooster/stats/cchalf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-13 18:28:24.000000 rs-booster-0.1.2/rsbooster/stats/ccpred.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-13 18:28:24.000000 rs-booster-0.1.2/rsbooster/stats/ccsym.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-13 18:28:24.000000 rs-booster-0.1.2/rsbooster/stats/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:28:40.714176 rs-booster-0.1.2/rsbooster/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:28:24.000000 rs-booster-0.1.2/rsbooster/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-13 18:28:24.000000 rs-booster-0.1.2/rsbooster/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-13 18:28:24.000000 rs-booster-0.1.2/rsbooster/utils/rfree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-13 18:28:40.718176 rs-booster-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-13 18:28:24.000000 rs-booster-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:28:40.714176 rs-booster-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:28:24.000000 rs-booster-0.1.2/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      977 2024-05-13 18:28:24.000000 rs-booster-0.1.2/tests/test_rfree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-13 18:28:24.000000 rs-booster-0.1.2/tests/test_rsbooster.py
```

### Comparing `rs-booster-0.1.1/LICENSE` & `rs-booster-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rs-booster-0.1.1/PKG-INFO` & `rs-booster-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rs-booster
-Version: 0.1.1
+Version: 0.1.2
 Summary: Useful scripts for analyzing diffraction
 Home-page: https://github.com/rs-station/rs-booster
 Author: Jack B. Greisman
 Author-email: greisman@g.harvard.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rs-station/rs-booster/issues
 Project-URL: Source Code, https://github.com/rs-station/rs-booster
```

### Comparing `rs-booster-0.1.1/README.md` & `rs-booster-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `rs-booster-0.1.1/rs_booster.egg-info/PKG-INFO` & `rs-booster-0.1.2/rs_booster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rs-booster
-Version: 0.1.1
+Version: 0.1.2
 Summary: Useful scripts for analyzing diffraction
 Home-page: https://github.com/rs-station/rs-booster
 Author: Jack B. Greisman
 Author-email: greisman@g.harvard.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rs-station/rs-booster/issues
 Project-URL: Source Code, https://github.com/rs-station/rs-booster
```

### Comparing `rs-booster-0.1.1/rs_booster.egg-info/SOURCES.txt` & `rs-booster-0.1.2/rs_booster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rs-booster-0.1.1/rs_booster.egg-info/entry_points.txt` & `rs-booster-0.1.2/rs_booster.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `rs-booster-0.1.1/rsbooster/diffmaps/diffmap.py` & `rs-booster-0.1.2/rsbooster/diffmaps/diffmap.py`

 * *Files identical despite different names*

### Comparing `rs-booster-0.1.1/rsbooster/diffmaps/internaldiffmap.py` & `rs-booster-0.1.2/rsbooster/diffmaps/internaldiffmap.py`

 * *Files identical despite different names*

### Comparing `rs-booster-0.1.1/rsbooster/esf/extrapolate.py` & `rs-booster-0.1.2/rsbooster/esf/extrapolate.py`

 * *Files identical despite different names*

### Comparing `rs-booster-0.1.1/rsbooster/io/precog2mtz.py` & `rs-booster-0.1.2/rsbooster/io/precog2mtz.py`

 * *Files identical despite different names*

### Comparing `rs-booster-0.1.1/rsbooster/realspace/find_peaks.py` & `rs-booster-0.1.2/rsbooster/realspace/find_peaks.py`

 * *Files identical despite different names*

### Comparing `rs-booster-0.1.1/rsbooster/scaleit/scaleit.py` & `rs-booster-0.1.2/rsbooster/scaleit/scaleit.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,22 @@
     )
     parser.add_argument(
         "-o",
         "--outfile",
         default="scaled.mtz",
         help="MTZ file to which scaleit output will be written",
     )
+    
+    parser.add_argument(
+        "--ignore-isomorphism",
+        action="store_true",
+        help=(
+            "Allow poorly isomorphous inputs to be scaled. "
+            "By default (no flag) poorly isomorphous inputs will raise an error.")
+    )
 
     return parser#.parse_args()
 
 
 def load_mtz(mtzpath, data_col, sig_col):
     """Load mtz and do French-Wilson scaling, if necessary"""
     mtz = rs.read_mtz(mtzpath)
@@ -135,15 +143,16 @@
             common = ref.index.intersection(mtz.index)
         else:
             common = common.intersection(mtz.index)
     common = common.sort_values()
 
     print(f"Number of common reflections: {len(common)}")
     mtzs = [mtz.loc[common] for mtz in mtzs]
-    joined = rs.concat([ref.loc[common]] + mtzs, axis=1)
+    
+    joined = rs.concat([ref.loc[common]] + mtzs, axis=1, check_isomorphous=(not args.ignore_isomorphism))
 
     # Run scaleit
     run_scaleit(joined, args.outfile, len(mtzs))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `rs-booster-0.1.1/rsbooster/stats/ccanom.py` & `rs-booster-0.1.2/rsbooster/stats/ccanom.py`

 * *Files identical despite different names*

### Comparing `rs-booster-0.1.1/rsbooster/stats/cchalf.py` & `rs-booster-0.1.2/rsbooster/stats/cchalf.py`

 * *Files identical despite different names*

### Comparing `rs-booster-0.1.1/rsbooster/stats/ccpred.py` & `rs-booster-0.1.2/rsbooster/stats/ccpred.py`

 * *Files identical despite different names*

### Comparing `rs-booster-0.1.1/rsbooster/stats/ccsym.py` & `rs-booster-0.1.2/rsbooster/stats/ccsym.py`

 * *Files identical despite different names*

### Comparing `rs-booster-0.1.1/rsbooster/stats/parser.py` & `rs-booster-0.1.2/rsbooster/stats/parser.py`

 * *Files identical despite different names*

### Comparing `rs-booster-0.1.1/rsbooster/utils/io.py` & `rs-booster-0.1.2/rsbooster/utils/io.py`

 * *Files identical despite different names*

### Comparing `rs-booster-0.1.1/rsbooster/utils/rfree.py` & `rs-booster-0.1.2/rsbooster/utils/rfree.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         ),
     )
 
     parser.add_argument(
         "-sg",
         "--spacegroup",
         required=True,
-        type=int,
+        type=str,
         help=("Spacegroup for output mtz file containing rfree flags"),
     )
 
     parser.add_argument(
         "-d",
         "--dmin",
         required=True,
```

### Comparing `rs-booster-0.1.1/setup.py` & `rs-booster-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `rs-booster-0.1.1/tests/test_rfree.py` & `rs-booster-0.1.2/tests/test_rfree.py`

 * *Files identical despite different names*

