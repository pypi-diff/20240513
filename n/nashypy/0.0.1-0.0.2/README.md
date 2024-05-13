# Comparing `tmp/nashypy-0.0.1.tar.gz` & `tmp/nashypy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nashypy-0.0.1.tar", last modified: Wed May  8 03:04:02 2024, max compression
+gzip compressed data, was "nashypy-0.0.2.tar", last modified: Mon May 13 12:42:30 2024, max compression
```

## Comparing `nashypy-0.0.1.tar` & `nashypy-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 son        (501) staff       (20)        0 2024-05-08 03:04:02.563332 nashypy-0.0.1/
--rw-r--r--   0 son        (501) staff       (20)    35149 2024-05-05 19:19:04.000000 nashypy-0.0.1/LICENSE
--rw-r--r--   0 son        (501) staff       (20)     2176 2024-05-08 03:04:02.563008 nashypy-0.0.1/PKG-INFO
--rw-r--r--   0 son        (501) staff       (20)     1749 2024-05-05 20:25:09.000000 nashypy-0.0.1/README.md
-drwxr-xr-x   0 son        (501) staff       (20)        0 2024-05-08 03:04:02.556759 nashypy-0.0.1/nashypy/
--rw-r--r--   0 son        (501) staff       (20)       24 2024-05-05 19:19:46.000000 nashypy-0.0.1/nashypy/__init__.py
-drwxr-xr-x   0 son        (501) staff       (20)        0 2024-05-08 03:04:02.561748 nashypy-0.0.1/nashypy/games/
--rw-r--r--   0 son        (501) staff       (20)       16 2024-05-05 19:46:44.000000 nashypy-0.0.1/nashypy/games/2x2_avis.txt
--rw-r--r--   0 son        (501) staff       (20)       16 2024-05-05 22:34:46.000000 nashypy-0.0.1/nashypy/games/2x2_battle.txt
--rw-r--r--   0 son        (501) staff       (20)       19 2024-05-05 20:45:55.000000 nashypy-0.0.1/nashypy/games/2x2_chicken.txt
--rw-r--r--   0 son        (501) staff       (20)       16 2024-05-05 20:39:23.000000 nashypy-0.0.1/nashypy/games/2x2_onemixed_nopure.txt
--rw-r--r--   0 son        (501) staff       (20)       16 2024-05-05 19:46:44.000000 nashypy-0.0.1/nashypy/games/2x2_onepurenash.txt
--rw-r--r--   0 son        (501) staff       (20)       18 2024-05-05 19:46:44.000000 nashypy-0.0.1/nashypy/games/2x2_stable_unstable_mixed.txt
--rw-r--r--   0 son        (501) staff       (20)       18 2024-05-05 19:46:44.000000 nashypy-0.0.1/nashypy/games/2x2_staghunt.txt
--rw-r--r--   0 son        (501) staff       (20)       16 2024-05-05 19:46:44.000000 nashypy-0.0.1/nashypy/games/2x2_twopurenash.txt
--rw-r--r--   0 son        (501) staff       (20)       20 2024-05-05 19:46:44.000000 nashypy-0.0.1/nashypy/games/2x2_zerosum.txt
--rw-r--r--   0 son        (501) staff       (20)       24 2024-05-05 19:46:44.000000 nashypy-0.0.1/nashypy/games/3x2_game1.txt
--rw-r--r--   0 son        (501) staff       (20)       26 2024-05-05 19:46:44.000000 nashypy-0.0.1/nashypy/games/3x2_game2.txt
--rw-r--r--   0 son        (501) staff       (20)       42 2024-05-05 23:12:30.000000 nashypy-0.0.1/nashypy/games/3x3_rockpaperscissor.txt
--rw-r--r--   0 son        (501) staff       (20)    29292 2024-05-08 02:54:46.000000 nashypy-0.0.1/nashypy/lrsnash.py
-drwxr-xr-x   0 son        (501) staff       (20)        0 2024-05-08 03:04:02.562654 nashypy-0.0.1/nashypy.egg-info/
--rw-r--r--   0 son        (501) staff       (20)     2176 2024-05-08 03:04:02.000000 nashypy-0.0.1/nashypy.egg-info/PKG-INFO
--rw-r--r--   0 son        (501) staff       (20)      650 2024-05-08 03:04:02.000000 nashypy-0.0.1/nashypy.egg-info/SOURCES.txt
--rw-r--r--   0 son        (501) staff       (20)        1 2024-05-08 03:04:02.000000 nashypy-0.0.1/nashypy.egg-info/dependency_links.txt
--rw-r--r--   0 son        (501) staff       (20)       13 2024-05-08 03:04:02.000000 nashypy-0.0.1/nashypy.egg-info/requires.txt
--rw-r--r--   0 son        (501) staff       (20)       14 2024-05-08 03:04:02.000000 nashypy-0.0.1/nashypy.egg-info/top_level.txt
--rw-r--r--   0 son        (501) staff       (20)       38 2024-05-08 03:04:02.563391 nashypy-0.0.1/setup.cfg
--rw-r--r--   0 son        (501) staff       (20)      650 2024-05-05 20:47:47.000000 nashypy-0.0.1/setup.py
-drwxr-xr-x   0 son        (501) staff       (20)        0 2024-05-08 03:04:02.562255 nashypy-0.0.1/tests/
--rw-r--r--   0 son        (501) staff       (20)        0 2024-05-05 20:27:23.000000 nashypy-0.0.1/tests/__init__.py
--rw-r--r--   0 son        (501) staff       (20)     2218 2024-05-05 20:49:56.000000 nashypy-0.0.1/tests/test_module.py
+drwxr-xr-x   0 son        (501) staff       (20)        0 2024-05-13 12:42:30.595420 nashypy-0.0.2/
+-rw-r--r--   0 son        (501) staff       (20)    35149 2024-05-05 19:19:04.000000 nashypy-0.0.2/LICENSE
+-rw-r--r--   0 son        (501) staff       (20)     2223 2024-05-13 12:42:30.595074 nashypy-0.0.2/PKG-INFO
+-rw-r--r--   0 son        (501) staff       (20)     1749 2024-05-05 20:25:09.000000 nashypy-0.0.2/README.md
+drwxr-xr-x   0 son        (501) staff       (20)        0 2024-05-13 12:42:30.591304 nashypy-0.0.2/nashypy/
+-rw-r--r--   0 son        (501) staff       (20)       24 2024-05-05 19:19:46.000000 nashypy-0.0.2/nashypy/__init__.py
+drwxr-xr-x   0 son        (501) staff       (20)        0 2024-05-13 12:42:30.594138 nashypy-0.0.2/nashypy/games/
+-rw-r--r--   0 son        (501) staff       (20)       16 2024-05-05 19:46:44.000000 nashypy-0.0.2/nashypy/games/2x2_avis.txt
+-rw-r--r--   0 son        (501) staff       (20)       16 2024-05-05 22:34:46.000000 nashypy-0.0.2/nashypy/games/2x2_battle.txt
+-rw-r--r--   0 son        (501) staff       (20)       19 2024-05-05 20:45:55.000000 nashypy-0.0.2/nashypy/games/2x2_chicken.txt
+-rw-r--r--   0 son        (501) staff       (20)       16 2024-05-05 20:39:23.000000 nashypy-0.0.2/nashypy/games/2x2_onemixed_nopure.txt
+-rw-r--r--   0 son        (501) staff       (20)       16 2024-05-05 19:46:44.000000 nashypy-0.0.2/nashypy/games/2x2_onepurenash.txt
+-rw-r--r--   0 son        (501) staff       (20)       18 2024-05-05 19:46:44.000000 nashypy-0.0.2/nashypy/games/2x2_stable_unstable_mixed.txt
+-rw-r--r--   0 son        (501) staff       (20)       18 2024-05-05 19:46:44.000000 nashypy-0.0.2/nashypy/games/2x2_staghunt.txt
+-rw-r--r--   0 son        (501) staff       (20)       16 2024-05-05 19:46:44.000000 nashypy-0.0.2/nashypy/games/2x2_twopurenash.txt
+-rw-r--r--   0 son        (501) staff       (20)       20 2024-05-05 19:46:44.000000 nashypy-0.0.2/nashypy/games/2x2_zerosum.txt
+-rw-r--r--   0 son        (501) staff       (20)       24 2024-05-05 19:46:44.000000 nashypy-0.0.2/nashypy/games/3x2_game1.txt
+-rw-r--r--   0 son        (501) staff       (20)       26 2024-05-05 19:46:44.000000 nashypy-0.0.2/nashypy/games/3x2_game2.txt
+-rw-r--r--   0 son        (501) staff       (20)       42 2024-05-05 23:12:30.000000 nashypy-0.0.2/nashypy/games/3x3_rockpaperscissor.txt
+-rw-r--r--   0 son        (501) staff       (20)    29292 2024-05-08 02:54:46.000000 nashypy-0.0.2/nashypy/lrsnash.py
+drwxr-xr-x   0 son        (501) staff       (20)        0 2024-05-13 12:42:30.594656 nashypy-0.0.2/nashypy.egg-info/
+-rw-r--r--   0 son        (501) staff       (20)     2223 2024-05-13 12:42:30.000000 nashypy-0.0.2/nashypy.egg-info/PKG-INFO
+-rw-r--r--   0 son        (501) staff       (20)      650 2024-05-13 12:42:30.000000 nashypy-0.0.2/nashypy.egg-info/SOURCES.txt
+-rw-r--r--   0 son        (501) staff       (20)        1 2024-05-13 12:42:30.000000 nashypy-0.0.2/nashypy.egg-info/dependency_links.txt
+-rw-r--r--   0 son        (501) staff       (20)       30 2024-05-13 12:42:30.000000 nashypy-0.0.2/nashypy.egg-info/requires.txt
+-rw-r--r--   0 son        (501) staff       (20)       14 2024-05-13 12:42:30.000000 nashypy-0.0.2/nashypy.egg-info/top_level.txt
+-rw-r--r--   0 son        (501) staff       (20)       38 2024-05-13 12:42:30.595479 nashypy-0.0.2/setup.cfg
+-rw-r--r--   0 son        (501) staff       (20)      673 2024-05-13 12:38:26.000000 nashypy-0.0.2/setup.py
+drwxr-xr-x   0 son        (501) staff       (20)        0 2024-05-13 12:42:30.594413 nashypy-0.0.2/tests/
+-rw-r--r--   0 son        (501) staff       (20)        0 2024-05-05 20:27:23.000000 nashypy-0.0.2/tests/__init__.py
+-rw-r--r--   0 son        (501) staff       (20)     2218 2024-05-05 20:49:56.000000 nashypy-0.0.2/tests/test_module.py
```

### Comparing `nashypy-0.0.1/LICENSE` & `nashypy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nashypy-0.0.1/PKG-INFO` & `nashypy-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: nashypy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Game Theory Library
 Home-page: https://github.com/snpham/nashypy
 Author: Son Pham
 Author-email: snpham02@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: plotly
 Requires-Dist: numpy
+Requires-Dist: sympy
+Requires-Dist: matplotlib
 
 # NashyPy
 
 `nashypy` is a Python package designed for the analysis of Nash equilibria in game theory. It offers tools to read game data, visualize best response polyhedra and polytopes, and find Nash equilibria.
 
 Note: this package is in development and currently can only run 2x2 games, 3x2 games are WIP.
```

### Comparing `nashypy-0.0.1/README.md` & `nashypy-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nashypy-0.0.1/nashypy/lrsnash.py` & `nashypy-0.0.2/nashypy/lrsnash.py`

 * *Files identical despite different names*

### Comparing `nashypy-0.0.1/nashypy.egg-info/PKG-INFO` & `nashypy-0.0.2/nashypy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: nashypy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Game Theory Library
 Home-page: https://github.com/snpham/nashypy
 Author: Son Pham
 Author-email: snpham02@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: plotly
 Requires-Dist: numpy
+Requires-Dist: sympy
+Requires-Dist: matplotlib
 
 # NashyPy
 
 `nashypy` is a Python package designed for the analysis of Nash equilibria in game theory. It offers tools to read game data, visualize best response polyhedra and polytopes, and find Nash equilibria.
 
 Note: this package is in development and currently can only run 2x2 games, 3x2 games are WIP.
```

### Comparing `nashypy-0.0.1/nashypy.egg-info/SOURCES.txt` & `nashypy-0.0.2/nashypy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nashypy-0.0.1/tests/test_module.py` & `nashypy-0.0.2/tests/test_module.py`

 * *Files identical despite different names*

