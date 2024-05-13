# Comparing `tmp/onion_clustering-0.2.0.tar.gz` & `tmp/onion_clustering-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onion_clustering-0.2.0.tar", last modified: Thu May  2 13:06:17 2024, max compression
+gzip compressed data, was "onion_clustering-0.2.1.tar", last modified: Mon May 13 10:01:18 2024, max compression
```

## Comparing `onion_clustering-0.2.0.tar` & `onion_clustering-0.2.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-02 13:06:17.948502 onion_clustering-0.2.0/
--rw-r--r--   0 mattebecchi   (501) staff       (20)    53248 2024-05-02 13:04:24.000000 onion_clustering-0.2.0/.coverage
--rw-r--r--   0 mattebecchi   (501) staff       (20)       50 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/.gitignore
--rw-r--r--   0 mattebecchi   (501) staff       (20)     1068 2024-02-16 13:11:19.000000 onion_clustering-0.2.0/LICENSE
--rw-r--r--   0 mattebecchi   (501) staff       (20)     6088 2024-05-02 13:06:17.947605 onion_clustering-0.2.0/PKG-INFO
--rw-r--r--   0 mattebecchi   (501) staff       (20)     5652 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/README.md
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-02 13:06:17.932442 onion_clustering-0.2.0/examples/
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3664 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/examples/example_script.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3669 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/examples/example_script_2d.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)      641 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/justfile
--rw-r--r--   0 mattebecchi   (501) staff       (20)      947 2024-05-02 13:05:25.000000 onion_clustering-0.2.0/pyproject.toml
--rw-r--r--   0 mattebecchi   (501) staff       (20)       26 2024-02-21 15:08:50.000000 onion_clustering-0.2.0/pytest.ini
--rw-r--r--   0 mattebecchi   (501) staff       (20)       38 2024-05-02 13:06:17.948680 onion_clustering-0.2.0/setup.cfg
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-02 13:06:17.927333 onion_clustering-0.2.0/src/
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-02 13:06:17.936821 onion_clustering-0.2.0/src/onion_clustering/
--rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/src/onion_clustering/__init__.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    35963 2024-05-02 12:59:06.000000 onion_clustering-0.2.0/src/onion_clustering/classes.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    19800 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/src/onion_clustering/first_classes.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    22934 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/src/onion_clustering/functions.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    18526 2024-05-02 12:59:27.000000 onion_clustering-0.2.0/src/onion_clustering/main.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    23334 2024-05-02 13:01:37.000000 onion_clustering-0.2.0/src/onion_clustering/main_2d.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    15728 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/src/onion_clustering/utilities.py
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-02 13:06:17.946642 onion_clustering-0.2.0/src/onion_clustering.egg-info/
--rw-r--r--   0 mattebecchi   (501) staff       (20)     6088 2024-05-02 13:06:17.000000 onion_clustering-0.2.0/src/onion_clustering.egg-info/PKG-INFO
--rw-r--r--   0 mattebecchi   (501) staff       (20)      842 2024-05-02 13:06:17.000000 onion_clustering-0.2.0/src/onion_clustering.egg-info/SOURCES.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)        1 2024-05-02 13:06:17.000000 onion_clustering-0.2.0/src/onion_clustering.egg-info/dependency_links.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       30 2024-05-02 13:06:17.000000 onion_clustering-0.2.0/src/onion_clustering.egg-info/requires.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       17 2024-05-02 13:06:17.000000 onion_clustering-0.2.0/src/onion_clustering.egg-info/top_level.txt
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-02 13:06:17.941621 onion_clustering-0.2.0/test/
--rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-02-16 13:11:19.000000 onion_clustering-0.2.0/test/__init__.py
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-02 13:06:17.944046 onion_clustering-0.2.0/test/output_multi/
--rw-r--r--   0 mattebecchi   (501) staff       (20)      409 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/test/output_multi/final_states.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/test/output_multi/fraction_0.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/test/output_multi/number_of_states.txt
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-02 13:06:17.945993 onion_clustering-0.2.0/test/output_uni/
--rw-r--r--   0 mattebecchi   (501) staff       (20)     1668 2024-05-02 07:31:53.000000 onion_clustering-0.2.0/test/output_uni/final_states.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-05-02 07:28:27.000000 onion_clustering-0.2.0/test/output_uni/fraction_0.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/test/output_uni/number_of_states.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3375 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/test/test_multi.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3275 2024-05-02 08:15:07.000000 onion_clustering-0.2.0/test/test_uni.py
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-13 10:01:18.882819 onion_clustering-0.2.1/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    53248 2024-05-10 14:58:09.000000 onion_clustering-0.2.1/.coverage
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       81 2024-05-08 09:25:50.000000 onion_clustering-0.2.1/.gitignore
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     1068 2024-02-16 13:11:19.000000 onion_clustering-0.2.1/LICENSE
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     6088 2024-05-13 10:01:18.881807 onion_clustering-0.2.1/PKG-INFO
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     5652 2024-05-08 09:25:50.000000 onion_clustering-0.2.1/README.md
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-13 10:01:18.860596 onion_clustering-0.2.1/examples/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     3663 2024-05-08 09:25:50.000000 onion_clustering-0.2.1/examples/example_script.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     3669 2024-05-08 09:25:50.000000 onion_clustering-0.2.1/examples/example_script_2d.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      641 2024-05-08 09:25:50.000000 onion_clustering-0.2.1/justfile
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      947 2024-05-10 14:21:08.000000 onion_clustering-0.2.1/pyproject.toml
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       26 2024-02-21 15:08:50.000000 onion_clustering-0.2.1/pytest.ini
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       38 2024-05-13 10:01:18.883017 onion_clustering-0.2.1/setup.cfg
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-13 10:01:18.854860 onion_clustering-0.2.1/src/
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-13 10:01:18.868907 onion_clustering-0.2.1/src/onion_clustering/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-05-08 09:25:50.000000 onion_clustering-0.2.1/src/onion_clustering/__init__.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    36398 2024-05-10 14:39:49.000000 onion_clustering-0.2.1/src/onion_clustering/classes.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    19700 2024-05-10 14:05:21.000000 onion_clustering-0.2.1/src/onion_clustering/first_classes.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    23955 2024-05-10 14:53:43.000000 onion_clustering-0.2.1/src/onion_clustering/functions.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    25883 2024-05-10 14:03:06.000000 onion_clustering-0.2.1/src/onion_clustering/main.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    23334 2024-05-08 09:25:50.000000 onion_clustering-0.2.1/src/onion_clustering/main_2d.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    15728 2024-05-08 09:25:50.000000 onion_clustering-0.2.1/src/onion_clustering/utilities.py
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-13 10:01:18.880540 onion_clustering-0.2.1/src/onion_clustering.egg-info/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     6088 2024-05-13 10:01:18.000000 onion_clustering-0.2.1/src/onion_clustering.egg-info/PKG-INFO
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      842 2024-05-13 10:01:18.000000 onion_clustering-0.2.1/src/onion_clustering.egg-info/SOURCES.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)        1 2024-05-13 10:01:18.000000 onion_clustering-0.2.1/src/onion_clustering.egg-info/dependency_links.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       30 2024-05-13 10:01:18.000000 onion_clustering-0.2.1/src/onion_clustering.egg-info/requires.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       17 2024-05-13 10:01:18.000000 onion_clustering-0.2.1/src/onion_clustering.egg-info/top_level.txt
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-13 10:01:18.874029 onion_clustering-0.2.1/test/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-02-16 13:11:19.000000 onion_clustering-0.2.1/test/__init__.py
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-13 10:01:18.876595 onion_clustering-0.2.1/test/output_multi/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      409 2024-05-08 09:25:50.000000 onion_clustering-0.2.1/test/output_multi/final_states.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-05-08 09:25:50.000000 onion_clustering-0.2.1/test/output_multi/fraction_0.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-05-08 09:25:50.000000 onion_clustering-0.2.1/test/output_multi/number_of_states.txt
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-13 10:01:18.879266 onion_clustering-0.2.1/test/output_uni/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     1759 2024-05-10 14:20:03.000000 onion_clustering-0.2.1/test/output_uni/final_states.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-05-10 14:19:53.000000 onion_clustering-0.2.1/test/output_uni/fraction_0.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-05-10 14:19:46.000000 onion_clustering-0.2.1/test/output_uni/number_of_states.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     3375 2024-05-08 09:25:50.000000 onion_clustering-0.2.1/test/test_multi.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     2941 2024-05-10 14:20:36.000000 onion_clustering-0.2.1/test/test_uni.py
```

### Comparing `onion_clustering-0.2.0/.coverage` & `onion_clustering-0.2.1/.coverage`

 * *Files 14% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -46,18 +46,18 @@
     numbits blob,               -- see the numbits functions in coverage.numbits
     foreign key (file_id) references file (id),
     foreign key (context_id) references context (id),
     unique (file_id, context_id)
 );
 INSERT INTO line_bits VALUES(1,1,X'02');
 INSERT INTO line_bits VALUES(2,1,X'c27b074c70f30328ff000000c0d193270300dddeedbbcaefc000805dafb7caefc07243f8f3fbfadfef0d0000000000000000000000903f0020dd379fbcc7211f809ccf5f58dbd3e70700bb156c5a9e4602c6fff7fb2c07f02e01');
-INSERT INTO line_bits VALUES(3,1,X'627f81b2eebf882c797e6f57a0539c46c5f8f19b7c32cba78045040000000080700100000072f7fcbcfb046dbbee75c78a9f1ff9b86582bcdf3fc9f363fcbcfccfcff3eef7fbf12d4d4ab67fdcac00b7bbfefcf8fffbfb630000000b6041debfff89bf00000000000000000000000000f37bfffee7df7ffffee32f5b66f9d97fdc');
-INSERT INTO line_bits VALUES(4,1,X'625f0200c0f85dc08c5f40c66308c00b0858000080c0b74040003b0edbccf77bfcfcdf9f7fbe8c8701189f05082cf07b0200018130db4c7efef7653cf0ffbebfef4600aff8ff2f');
-INSERT INTO line_bits VALUES(5,1,X'a297302801001018400040fb6a0900800000b46fe500003cfe030000c03cd7bff8790200390000481e8b2500c0dff0077c00007ff9ef8ae77df3f371ecdef0ff910300108f1cfe27ff5d79fef98d8ff3dd02');
-INSERT INTO line_bits VALUES(6,1,X'c2bb03487086fc00ca0700c0febffc5f010000c01f00e6f3617e1e3f8f09cb0dfb5e0100c80f00e4eee693f738e40300679f5f58f7f4fc0080dd2698a7e5692601dbf3bffd3ee701bc4b');
+INSERT INTO line_bits VALUES(3,1,X'627f819075ff4564c9f37bbb029de2342ac68fdfe493593e052c220000000000840b00000090bbe7e7dd2768db75af3b56fc3e3ff271cb0479bf7f92f7f9317e5efee7e779f7fbfdf8962625db3f6e5680db5d7f7efcfffdfd3100008005b020efdfffc45f00000000000000000000000080f9bd7ffff3efbf7ffff1972db3fcec3f6e');
+INSERT INTO line_bits VALUES(4,1,X'625f0200c0f85dc08c5f40c66308c00b0858000080c0b74040003bc636f3fd1e3ffff7e79f2fe36100c66701020bfc9e00404020cc36939fff7d190ffcbfefefbb11c02bfeff0b');
+INSERT INTO line_bits VALUES(5,1,X'a297000cca0300e0001e0000edabe50100e00100a07d2b0700003cfe0300000000cc73fd8b9f270090070000248fc512000080bfe16ff90000fef2df15cffbe6e7e3d8bde1ff231f000000fefc000000f0d7e50000c42387ffc97f579e7f7ee3e37cb7');
+INSERT INTO line_bits VALUES(6,1,X'c2f70e400200e00cf901940f00000000fbffe5ff09f007007f000000309f0ff3737e1eff6dfb5e0100c80f0000007277f3c97b3cf20f00000072f9b07e79fc3cee60fa9b2f798f43f0010000c0d9e777c67feebbe7070000c06e05f3795a1e0000cd7c7200b03dffdbef731e0000807709');
 CREATE TABLE arc (
     -- If recording branches, a row per context per from/to line transition executed.
     file_id integer,            -- foreign key to `file`.
     context_id integer,         -- foreign key to `context`.
     fromno integer,             -- line number jumped from.
     tono integer,               -- line number jumped to.
     foreign key (file_id) references file (id),
```

### Comparing `onion_clustering-0.2.0/LICENSE` & `onion_clustering-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.0/PKG-INFO` & `onion_clustering-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onion_clustering
-Version: 0.2.0
+Version: 0.2.1
 Summary: Code for unsupervised clustering of time-correlated data.
 Maintainer-email: Matteo Becchi <bechmath@gmail.com>
 Project-URL: github, https://github.com/matteobecchi/timeseries_analysis/
 Requires-Python: <3.11,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
```

### Comparing `onion_clustering-0.2.0/README.md` & `onion_clustering-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.0/examples/example_script.py` & `onion_clustering-0.2.1/examples/example_script.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 from onion_clustering import main
 
 ##############################################################################
 ### Set all the analysis parameters ###
 # Use git clone git@github.com:matteobecchi/onion_example_files.git
 # to download example datasets
 PATH_TO_INPUT_DATA = "../onion_example_files/data/univariate_time-series.npy"
-TAU_WINDOW = 10  # time resolution of the analysis
+TAU_WINDOW = 4  # time resolution of the analysis
 
 ### Optional parametrers ###
 T_SMOOTH = 1  # window for moving average (default 1)
 T_DELAY = 1  # remove the first t_delay frames (default 0)
 T_CONV = 1.0  # convert frames in time units (default 1)
 TIME_UNITS = "frames"  # the time units (default 'frames')
 EXAMPLE_ID = 0  # particle plotted as example (default 0)
-NUM_TAU_W = 10  # number of values of tau_window tested (default 20)
+NUM_TAU_W = 20  # number of values of tau_window tested (default 20)
 MIN_TAU_W = 2  # min number of tau_window tested (default 2)
 MIN_T_SMOOTH = 1  # min value of t_smooth tested (default 1)
 MAX_T_SMOOTH = 2  # max value of t_smooth tested (default 5)
 STEP_T_SMOOTH = 1  # increment in value of t_smooth tested (default 1)
 MAX_TAU_W = "auto"  # max number of tau_window tested (default is auto)
 BINS = "auto"  # number of histogram bins (default is auto)
 ##############################################################################
```

### Comparing `onion_clustering-0.2.0/examples/example_script_2d.py` & `onion_clustering-0.2.1/examples/example_script_2d.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.0/justfile` & `onion_clustering-0.2.1/justfile`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.0/pyproject.toml` & `onion_clustering-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "onion_clustering"
-version = "0.2.0"
+version = "0.2.1"
 description = "Code for unsupervised clustering of time-correlated data."
 # license = "MIT"
 maintainers = [
   { name = "Matteo Becchi", email = "bechmath@gmail.com" },
 ]
 dependencies = [
   "matplotlib",
```

### Comparing `onion_clustering-0.2.0/src/onion_clustering/classes.py` & `onion_clustering-0.2.1/src/onion_clustering/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,18 @@
 from onion_clustering.first_classes import (
     MultiData,
     Parameters,
     StateMulti,
     StateUni,
     UniData,
 )
-from onion_clustering.functions import gaussian
+from onion_clustering.functions import (
+    gaussian,
+    moving_average,
+)
 
 COLORMAP = "viridis"
 
 
 class ClusteringObject:
     """This class contains input, output and methods for plotting."""
 
@@ -348,26 +351,26 @@
 
         for i, t_smooth in enumerate(self.t_smooth_list):
             pop_array = self.list_of_pop[i]
 
             max_num_of_states = np.max(
                 [len(pop_list) for pop_list in pop_array]
             )
-            for j, pop_list in enumerate(pop_array):
+            for _, pop_list in enumerate(pop_array):
                 while len(pop_list) < max_num_of_states:
-                    pop_array[j].append(0.0)
+                    pop_list.append(0.0)
 
             pop_array = np.array(pop_array)
 
             fig, axes = plt.subplots()
             width = time[1:] - time[:-1]
             width = np.insert(width, 0, width[0] / 2)
 
             bottom = np.zeros(len(pop_array))
-            for j, state in enumerate(pop_array.T):
+            for _, state in enumerate(pop_array.T):
                 _ = axes.bar(
                     time, state, width, bottom=bottom, edgecolor="black"
                 )
                 bottom += state
 
             axes.set_xlabel(rf"Time resolution $\Delta t$ {units}")
             axes.set_ylabel(r"Population's fractions")
@@ -391,14 +394,20 @@
         m_clean = self.data.matrix
         flat_m = m_clean.flatten()
         binning = self.par.bins
         counts, bins = np.histogram(flat_m, bins=binning, density=True)
         bins -= (bins[1] - bins[0]) / 2
         counts *= flat_m.size
 
+        gap = 1
+        if bins.size > 49:
+            gap = int(bins.size * 0.02) * 2
+        counts = moving_average(counts, gap)
+        bins = moving_average(bins, gap)
+
         # Create a plot with two subplots (side-by-side)
         fig, axes = plt.subplots(
             1,
             2,
             sharey=True,
             gridspec_kw={"width_ratios": [3, 1]},
             figsize=(9, 4.8),
@@ -468,14 +477,20 @@
 
         # Compute histogram of flattened self.data.matrix
         flat_m = self.data.matrix.flatten()
         counts, bins = np.histogram(flat_m, bins=self.par.bins, density=True)
         bins -= (bins[1] - bins[0]) / 2
         counts *= flat_m.size
 
+        gap = 1
+        if bins.size > 49:
+            gap = int(bins.size * 0.02) * 2
+        counts = moving_average(counts, gap)
+        bins = moving_average(bins, gap)
+
         # Create a 1x2 subplots with shared y-axis
         fig, axes = plt.subplots(
             1,
             2,
             sharey=True,
             gridspec_kw={"width_ratios": [3, 1]},
             figsize=(9, 4.8),
@@ -699,35 +714,35 @@
 
                 # Set labels and titles for the plots
                 ax2.set_ylabel("Signal 1")
                 ax2.set_xlabel("Signal 2")
 
             elif self.data.dims == 3:
                 fig = plt.figure(figsize=(6, 6))
-                ax: Axes3D = fig.add_subplot(111, projection="3d")
+                axes: Axes3D = fig.add_subplot(111, projection="3d")
 
                 # Plot the individual trajectories
                 step = 1 if m_clean.size > 1000000 else 1
                 for idx, mol in enumerate(m_clean[::step]):
-                    ax.plot(
+                    axes.plot(
                         mol[:, 0],
                         mol[:, 1],
                         mol[:, 2],
                         color="black",
                         marker="o",
                         ms=0.5,
                         lw=0.2,
                         alpha=1.0,
                         rasterized=True,
                     )
 
                 # Set labels and titles for the plots
-                ax.set_xlabel("Signal 1")
-                ax.set_ylabel("Signal 2")
-                ax.set_zlabel("Signal 3")
+                axes.set_xlabel("Signal 1")
+                axes.set_ylabel("Signal 2")
+                axes.set_zlabel("Signal 3")
 
             fig.savefig("output_figures/" + filename + ".png", dpi=600)
             plt.close(fig)
 
     def preparing_the_data(self):
         """
         Prepare the raw data for analysis.
@@ -785,15 +800,15 @@
         tmp = plt.get_cmap(COLORMAP, n_states)
         colors_from_cmap = tmp(np.arange(0, 1, 1 / n_states))
         colors_from_cmap[-1] = tmp(1.0)
         m_clean = self.data.matrix
         all_the_labels = self.create_all_the_labels()
 
         if m_clean.shape[2] == 3:
-            fig, ax = plt.subplots(2, 2, figsize=(6, 6))
+            fig, axes = plt.subplots(2, 2, figsize=(6, 6))
             dir0 = [0, 0, 1]
             dir1 = [1, 2, 2]
             ax0 = [0, 0, 1]
             ax1 = [0, 1, 0]
 
             for k in range(3):
                 d_0 = dir0[k]
@@ -810,63 +825,63 @@
 
                 line_w = 0.05
                 max_t = all_the_labels.shape[1]
                 m_resized = m_clean[:, :max_t:, :]
                 step = 5 if m_resized.size > 1000000 else 1
 
                 for i, mol in enumerate(m_resized[::step]):
-                    ax[a_0][a_1].plot(
+                    axes[a_0][a_1].plot(
                         mol.T[d_0],
                         mol.T[d_1],
                         c="black",
                         lw=line_w,
                         rasterized=True,
                         zorder=0,
                     )
                     color_list = all_the_labels[i * step]
-                    ax[a_0][a_1].scatter(
+                    axes[a_0][a_1].scatter(
                         mol.T[d_0],
                         mol.T[d_1],
                         c=color_list,
                         cmap=COLORMAP,
                         vmin=0,
                         vmax=n_states - 1,
                         s=0.5,
                         rasterized=True,
                     )
 
                     color_list = all_the_labels[id_min]
-                    ax[a_0][a_1].plot(
+                    axes[a_0][a_1].plot(
                         m_resized[id_min].T[d_0],
                         m_resized[id_min].T[d_1],
                         c="black",
                         lw=line_w,
                         rasterized=True,
                         zorder=0,
                     )
-                    ax[a_0][a_1].scatter(
+                    axes[a_0][a_1].scatter(
                         m_resized[id_min].T[d_0],
                         m_resized[id_min].T[d_1],
                         c=color_list,
                         cmap=COLORMAP,
                         vmin=0,
                         vmax=n_states - 1,
                         s=0.5,
                         rasterized=True,
                     )
                     color_list = all_the_labels[id_max]
-                    ax[a_0][a_1].plot(
+                    axes[a_0][a_1].plot(
                         m_resized[id_max].T[d_0],
                         m_resized[id_max].T[d_1],
                         c="black",
                         lw=line_w,
                         rasterized=True,
                         zorder=0,
                     )
-                    ax[a_0][a_1].scatter(
+                    axes[a_0][a_1].scatter(
                         m_resized[id_max].T[d_0],
                         m_resized[id_max].T[d_1],
                         c=color_list,
                         cmap=COLORMAP,
                         vmin=0,
                         vmax=n_states - 1,
                         s=0.5,
@@ -879,26 +894,26 @@
                             ellipse = Ellipse(
                                 tuple(state.mean),
                                 state.axis[d_0],
                                 state.axis[d_1],
                                 color="black",
                                 fill=False,
                             )
-                            ax[a_0][a_1].add_patch(ellipse)
+                            axes[a_0][a_1].add_patch(ellipse)
 
                 # Set plot titles and axis labels
-                ax[a_0][a_1].set_xlabel(r"Signal " + str(d_0))
-                ax[a_0][a_1].set_ylabel(r"Signal " + str(d_1))
+                axes[a_0][a_1].set_xlabel(r"Signal " + str(d_0))
+                axes[a_0][a_1].set_ylabel(r"Signal " + str(d_1))
 
-            ax[1][1].axis("off")
+            axes[1][1].axis("off")
             fig.savefig("output_figures/Fig2.png", dpi=600)
             plt.close(fig)
 
         elif m_clean.shape[2] == 2:
-            fig, ax = plt.subplots(figsize=(6, 6))
+            fig, axes = plt.subplots(figsize=(6, 6))
 
             # Plot the individual trajectories
             id_max, id_min = 0, 0
             for idx, mol in enumerate(m_clean):
                 if np.max(mol) == np.max(m_clean):
                     id_max = idx
                 if np.min(mol) == np.min(m_clean):
@@ -906,63 +921,63 @@
 
             line_w = 0.05
             max_t = all_the_labels.shape[1]
             m_resized = m_clean[:, :max_t:, :]
             step = 5 if m_resized.size > 1000000 else 1
 
             for i, mol in enumerate(m_resized[::step]):
-                ax.plot(
+                axes.plot(
                     mol.T[0],
                     mol.T[1],
                     c="black",
                     lw=line_w,
                     rasterized=True,
                     zorder=0,
                 )
                 color_list = all_the_labels[i * step]
-                ax.scatter(
+                axes.scatter(
                     mol.T[0],
                     mol.T[1],
                     c=color_list,
                     cmap=COLORMAP,
                     vmin=0,
                     vmax=n_states - 1,
                     s=0.5,
                     rasterized=True,
                 )
 
             color_list = all_the_labels[id_min]
-            ax.plot(
+            axes.plot(
                 m_resized[id_min].T[0],
                 m_resized[id_min].T[1],
                 c="black",
                 lw=line_w,
                 rasterized=True,
                 zorder=0,
             )
-            ax.scatter(
+            axes.scatter(
                 m_resized[id_min].T[0],
                 m_resized[id_min].T[1],
                 c=color_list,
                 cmap=COLORMAP,
                 vmin=0,
                 vmax=n_states - 1,
                 s=0.5,
                 rasterized=True,
             )
             color_list = all_the_labels[id_max]
-            ax.plot(
+            axes.plot(
                 m_resized[id_max].T[0],
                 m_resized[id_max].T[1],
                 c="black",
                 lw=line_w,
                 rasterized=True,
                 zorder=0,
             )
-            ax.scatter(
+            axes.scatter(
                 m_resized[id_max].T[0],
                 m_resized[id_max].T[1],
                 c=color_list,
                 cmap=COLORMAP,
                 vmin=0,
                 vmax=n_states - 1,
                 s=0.5,
@@ -974,58 +989,58 @@
                 ellipse = Ellipse(
                     tuple(state.mean),
                     state.axis[0],
                     state.axis[1],
                     color="black",
                     fill=False,
                 )
-                ax.add_patch(ellipse)
+                axes.add_patch(ellipse)
 
             # Set plot titles and axis labels
-            ax.set_xlabel(r"$x$")
-            ax.set_ylabel(r"$y$")
+            axes.set_xlabel(r"$x$")
+            axes.set_ylabel(r"$y$")
 
             fig.savefig("output_figures/Fig2.png", dpi=600)
             plt.close(fig)
 
     def plot_one_trajectory(self):
         """Plots the colored trajectory of an example particle."""
 
         m_clean = self.data.matrix
         all_the_labels = self.create_all_the_labels()
 
         # Get the signal of the example particle
         signal_x = m_clean[self.par.example_id].T[0][: all_the_labels.shape[1]]
         signal_y = m_clean[self.par.example_id].T[1][: all_the_labels.shape[1]]
 
-        fig, ax = plt.subplots(figsize=(6, 6))
+        fig, axes = plt.subplots(figsize=(6, 6))
 
         # Create a colormap to map colors to the labels
         cmap = plt.get_cmap(
             COLORMAP,
             int(
                 np.max(np.unique(all_the_labels))
                 - np.min(np.unique(all_the_labels))
                 + 1
             ),
         )
         color = all_the_labels[self.par.example_id]
-        ax.plot(signal_x, signal_y, c="black", lw=0.1)
+        axes.plot(signal_x, signal_y, c="black", lw=0.1)
 
-        ax.scatter(
+        axes.scatter(
             signal_x,
             signal_y,
             c=color,
             cmap=cmap,
             vmin=np.min(np.unique(all_the_labels)),
             vmax=np.max(np.unique(all_the_labels)),
             s=1.0,
             zorder=10,
         )
 
         # Set plot titles and axis labels
         fig.suptitle("Example particle: ID = " + str(self.par.example_id))
-        ax.set_xlabel(r"$x$")
-        ax.set_ylabel(r"$y$")
+        axes.set_xlabel(r"$x$")
+        axes.set_ylabel(r"$y$")
 
         fig.savefig("output_figures/Fig3.png", dpi=600)
         plt.close(fig)
```

### Comparing `onion_clustering-0.2.0/src/onion_clustering/first_classes.py` & `onion_clustering-0.2.1/src/onion_clustering/first_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,19 +210,17 @@
         # Initialize lists to store cluster means and standard deviations
         center_list = []
         std_list = []
         env0 = []
 
         # If there are no assigned window, we still need the "0" state
         # for consistency:
-        missing_zero = 0
         list_of_labels = np.unique(all_the_labels)
         if 0 not in list_of_labels:
             list_of_labels = np.insert(list_of_labels, 0, 0)
-            missing_zero = 1
 
         # Loop through unique labels (clusters)
         for ref_label in list_of_labels:
             tmp = []
             # Iterate through molecules and their labels
             for i, mol in enumerate(all_the_labels):
                 for window, label in enumerate(mol):
@@ -269,22 +267,22 @@
             err_inf = center - std_list[center_id]
             err_sup = center + std_list[center_id]
             axes.fill_between(
                 time_seq,
                 err_inf,
                 err_sup,
                 alpha=0.25,
-                color=palette[center_id + missing_zero + 1],
+                color=palette[center_id + 1],
             )
             axes.plot(
                 time_seq,
                 center,
-                label="ENV" + str(center_id + missing_zero),
+                label=f"ENV{center_id + 1}",
                 marker="o",
-                c=palette[center_id + missing_zero + 1],
+                c=palette[center_id + 1],
                 zorder=1,
             )
 
         for window in env0:
             axes.plot(
                 time_seq,
                 window,
```

### Comparing `onion_clustering-0.2.0/src/onion_clustering/functions.py` & `onion_clustering-0.2.1/src/onion_clustering/functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,82 +11,92 @@
 
 from onion_clustering.first_classes import Parameters, StateMulti, StateUni
 
 
 def read_input_data() -> str:
     """
     Attempt to read the content of 'data_directory.txt' file
-    and load it into a NumPy array as strings.
+    and load it into a string.
+
+    Returns
+    -------
+
+    data_dir : str
+        The path to the input file.
     """
     try:
         data_dir = np.loadtxt("data_directory.txt", dtype=str)
     except OSError as msg_exc:
         print(f"\t Reading data_directory.txt: {msg_exc}")
     except ValueError as msg_exc:
         print(f"\t Reading data_directory.txt: {msg_exc}")
 
     print("* Reading data from", data_dir)
 
     return str(data_dir)
 
 
-def moving_average(data: np.ndarray, window: int) -> np.ndarray:
-    """Applies a moving average filter to a 1D or 2D NumPy array.
+def moving_average(
+    data: np.ndarray,
+    window: int,
+) -> np.ndarray:
+    """
+    Applies a moving average filter to a 1D or 2D NumPy array.
 
-    Args:
-    - data (np.ndarray): The input array to be smoothed.
-    - window (int): The size of the moving average window.
+    Parameters
+    ----------
 
-    Returns:
-    - np.ndarray: The smoothed array obtained after applying
-    the moving average filter.
+    data : np.ndarray
+        The input array to be smoothed.
 
-    Raises:
-    - ValueError: If the input array dimension is not supported
-    (only 1D and 2D arrays are supported).
-    """
+    window : int
+        The size of the moving average window.
 
-    # Step 1: Create a NumPy array 'weights' with the values 1.0
-    # repeated 'window' times.
-    # Then, divide each element of 'weights' by the 'window' value
-    # to get the average weights.
-    weights = np.ones(window) / window
+    Returns
+    -------
 
-    # Step 2: Apply the moving average filter to the 'data' array using
-    # the 'weights' array. The 'np.convolve' function performs a linear
-    # convolution between 'data' and 'weights'. The result is a smoothed
-    # version of the 'data', where each point represents the weighted
-    # average of its neighbors.
+    np.ndarray
+        The smoothed array obtained after applying
+        the moving average filter.
+    """
+    weights = np.ones(window) / window
     if data.ndim == 1:
         return np.convolve(data, weights, mode="valid")
     if data.ndim >= 2:
         return np.apply_along_axis(
             lambda x: np.convolve(x, weights, mode="valid"), axis=1, arr=data
         )
     raise ValueError(
         "Invalid array dimension. Only 1D and 2D arrays are supported."
     )
 
 
-def moving_average_2d(data: np.ndarray, side: int) -> np.ndarray:
+def moving_average_2d(
+    data: np.ndarray,
+    side: int,
+) -> np.ndarray:
     """Applies a 2D moving average filter to a NumPy array.
 
-    Args:
-    - data (np.ndarray): The 2D input array to be smoothed.
-    - side (int): The side length of the square moving average window
+    Parameters
+    ----------
+
+    data : np.ndarray
+        The 2D input array to be smoothed.
+
+    side : int
+        The side length of the square moving average window
         (must be an odd number).
 
-    Returns:
-    - np.ndarray: The smoothed array obtained after applying the 2D
-        moving average filter.
+    Returns
+    -------
 
-    Raises:
-    - ValueError: If the side length 'side' is not an odd number.
+    np.ndarray
+        The smoothed array obtained after applying the 2D
+        moving average filter.
     """
-
     if side % 2 == 0:  # Check if side is an odd number
         raise ValueError("L must be an odd number.")
     half_width = (side - 1) // 2
     result = np.zeros_like(data, dtype=float)
 
     for index in np.ndindex(*data.shape):
         slices = tuple(
@@ -100,53 +110,62 @@
         # Calculate the average if the subarray is not empty
         if subarray.size > 0:
             result[index] = subarray.mean()
 
     return result
 
 
-def plot_histo(ax: plt.Axes, counts: np.ndarray, bins: np.ndarray):
+def plot_histo(
+    axes: plt.Axes,
+    counts: np.ndarray,
+    bins: np.ndarray,
+):
     """Plots a histogram on the specified axes.
 
-    Args:
-    - ax: The matplotlib axes to plot on.
-    - counts (np.ndarray): The count or frequency of occurrences.
-    - bins (np.ndarray): The bin edges defining the intervals.
+    Parameters
+    ----------
 
-    Returns:
-    - None
+    axes
+        The matplotlib axes to plot on.
 
-    The function plots a histogram with the provided count and bin information
-    on the specified axes 'ax' and labels the x and y axes accordingly.
-    """
+    counts : np.ndarray
+        The count or frequency of occurrences.
 
-    ax.stairs(counts, bins, fill=True)
-    ax.set_xlabel(r"Normalized signal")
-    ax.set_ylabel(r"Probability distribution")
+    bins : np.ndarray
+        The bin edges defining the intervals.
+    """
+    axes.stairs(counts, bins, fill=True)
+    axes.set_xlabel(r"Normalized signal")
+    axes.set_ylabel(r"Probability distribution")
 
 
-def param_grid(par: Parameters, trj_len: int) -> Tuple[List, List]:
+def param_grid(
+    par: Parameters,
+    trj_len: int,
+) -> Tuple[List, List]:
     """Generates parameter grids for tau_window and t_smooth.
 
-    Args:
-    - par (Parameters): An instance of the Parameters class containing
-        parameter details.
-    - trj_len (int): Length of the trajectory data.
+    Parameters
+    ----------
 
-    Returns:
-    - tau_window (List[int]): A list of tau_window values.
-    - t_smooth (List[int]): A list of t_smooth values.
+    par : Parameters
+        An instance of the Parameters class containing parameter details.
 
-    This function generates grids of values for 'tau_window' and 't_smooth'
-    based on the provided 'Parameters' instance and the length of the
-    trajectory. It calculates the values for 'tau_window' within the range
-    defined in 'Parameters' and generates 't_smooth' values within the
-    specified range.
-    """
+    trj_len : int
+        Length of the trajectory data.
+
+    Returns
+    -------
 
+    tau_window : List[int]
+        A list of tau_window values.
+
+    t_smooth : List[int]
+        A list of t_smooth values.
+    """
     if par.max_tau_w == -1:
         par.max_tau_w = trj_len - par.max_t_smooth
     tmp = np.geomspace(
         par.min_tau_w, par.max_tau_w, num=par.num_tau_w, dtype=int
     )
     tau_window = []
     for tau_w in tmp:
@@ -163,30 +182,35 @@
 
 
 def gaussian(
     x_points: np.ndarray, x_mean: float, sigma: float, area: float
 ) -> np.ndarray:
     """Compute the Gaussian function values at given points 'x'.
 
-    Args:
-    - x_points (np.ndarray): Array of input values.
-    - x_mean (float): Mean value of the Gaussian function.
-    - sigma (float): Standard deviation of the Gaussian function.
-    - area (float): Area under the Gaussian curve.
+    Parameters
+    ----------
 
-    Returns:
-    - np.ndarray: Gaussian function values computed at the input points.
+    x_points : np.ndarray
+        Array of input values.
 
-    This function calculates the values of a Gaussian function at the given
-    array of points 'x_points' using the provided 'x_mean', 'sigma'
-    (standard deviation), and 'area' (area under the curve) parameters.
-    It returns an array of Gaussian function values corresponding to the
-    input 'x_points'.
-    """
+    x_mean : float
+        Mean value of the Gaussian function.
+
+    sigma : float
+        Standard deviation of the Gaussian function.
 
+    area : float
+        Area under the Gaussian curve.
+
+    Returns
+    -------
+
+    np.ndarray
+        Gaussian function values computed at the input points.
+    """
     return (
         np.exp(-(((x_points - x_mean) / sigma) ** 2))
         * area
         / (np.sqrt(np.pi) * sigma)
     )
 
 
@@ -197,39 +221,51 @@
     edges: np.ndarray,
     counts: np.ndarray,
     gap: int,
     m_limits: np.ndarray,
 ) -> Tuple[int, int, np.ndarray]:
     """Fit a Gaussian curve to selected data based on provided parameters.
 
-    Args:
-    - dim (int): The dimension of the data.
-    - max_ind (int): Index of the maximum value in the histogram.
-    - minima (list[int]): List of indices representing the minimum points.
-    - edges (np.ndarray): Array containing the bin edges of the histogram.
-    - counts (np.ndarray): Array containing histogram counts.
-    - gap (int): Minimum allowed gap size for fitting intervals.
-    - m_limits (list[list[int]]): List of min and max limits for each
-        dimension.
+    Parameters
+    ----------
 
-    Returns:
-    - tuple[int, int, list[float]]: A tuple containing:
-        - flag (int): Flag indicating the success (1) or failure (0) of
-            the fitting process.
-        - goodness (int): Goodness value representing the fitting quality
-            (higher is better).
-        - popt (list[float]): Optimal values for the parameters
-            (mu, sigma, area) of the fitted Gaussian.
-
-    This function attempts to fit a Gaussian curve to selected data within the
-    specified dimension 'dim' based on provided histogram data ('edges' and
-    'counts'). It uses 'max_ind' to initialize parameters and 'minima' to
-    define the fitting interval.
-    """
+    dim : int
+        The dimension of the data.
+
+    max_ind : int
+        Index of the maximum value in the histogram.
+
+    minima : list[int]
+        List of indices representing the minimum points.
+
+    edges : np.ndarray
+        Array containing the bin edges of the histogram.
+
+    counts : np.ndarray
+        Array containing histogram counts.
+
+    gap : int
+        Minimum allowed gap size for fitting intervals.
+
+    m_limits : list[list[int]]
+        List of min and max limits for each dimension.
+
+    Returns
+    -------
+
+    flag : int
+        Flag indicating the success (1) or failure (0) of the fitting process.
 
+    goodness : int
+        Goodness value representing the fitting quality (higher is better).
+
+    popt : list[float]
+        Optimal values for the parameters (mu, sigma, area) of the
+        fitted Gaussian.
+    """
     # Initialize flag and goodness variables
     flag = 1
     goodness = 5
 
     # Extract relevant data within the specified minima
     edges_selection = edges[minima[2 * dim] : minima[2 * dim + 1]]
     all_axes = tuple(i for i in range(counts.ndim) if i != dim)
@@ -285,35 +321,38 @@
         print("\tFit: ValueError.")
         flag = 0
         popt = np.empty((3,))
     return flag, goodness, popt
 
 
 def relabel_states(
-    all_the_labels: np.ndarray, states_list: list[StateUni]
+    all_the_labels: np.ndarray,
+    states_list: list[StateUni],
 ) -> Tuple[np.ndarray, list[StateUni]]:
-    """Relabel states and update the state list based on occurrence in
-        'all_the_labels'.
+    """
+    Relabel states and update the state list based on occurrence in
+    'all_the_labels'.
 
-    Args:
-    - all_the_labels (np.ndarray): Array containing labels assigned
-        to each window in the trajectory.
-    - states_list (list[StateUni]): List of StateUni objects representing
-        different states.
+    Parameters
+    ----------
 
-    Returns:
-    - tuple[np.ndarray, list[StateUni]]: A tuple containing:
-        - all_the_labels (np.ndarray): Updated labels array with relabeled
-            states.
-        - relevant_states (list[StateUni]): Updated list of non-empty states,
-        ordered by mean values.
-
-    This function performs several operations to relabel the states and update
-    the state list. It removes empty states, reorders them based on the mean
-    values and relabels the labels in 'all_the_labels'.
+    all_the_labels : np.ndarray
+        Array containing labels assigned to each window in the trajectory.
+
+    states_list : list[StateUni]
+        List of StateUni objects representing different states.
+
+    Returns
+    -------
+
+    all_the_labels : np.ndarray
+        Updated labels array with relabeled states.
+
+    relevant_states : list[StateUni]
+        Updated list of non-empty states, ordered by mean values.
     """
     # Step 1: Remove states with zero relevance
     relevant_states = [state for state in states_list if state.perc != 0.0]
 
     # Step 2: Sort states according to their mean value
     relevant_states.sort(key=lambda x: x.mean)
 
@@ -338,21 +377,31 @@
     return all_the_labels, relevant_states
 
 
 def find_intersection(st_0: StateUni, st_1: StateUni) -> Tuple[float, int]:
     """
     Finds the intersection between two Gaussians.
 
-    Args:
-    - st_0, st_1 (StateUni): the two states we are computing the threshold
-        between
+    Parameters
+    ----------
 
-    Returns:
-    - th_val (float): the value of the threshold
-    - th_type (int): the type of the threshold (1 or 2)
+    st_0, st_1 : StateUni
+        The two states we are computing the threshold between.
+
+    Returns
+    -------
+
+    th_val : float
+        The value of the threshold.
+
+    th_type : int
+        The type of the threshold (1 or 2).
+
+    Notes
+    -----
 
     If the intersection exists, the threshold is type 1. If there are 2
     intersections, the one with higher value is chosen.
     If no intersection exists, the threshold is type 2. Its value will be
     the average between the two means, weighted with the two sigmas.
     """
     coeff_a = st_1.sigma**2 - st_0.sigma**2
@@ -454,19 +503,19 @@
         relabel_map[key + 1] = value + 1
 
     all_the_labels = relabel_map[all_the_labels.flatten()].reshape(
         all_the_labels.shape
     )
 
     final_map = np.zeros(max(np.unique(all_the_labels)) + 1, dtype=int)
-    for i, el in enumerate(np.unique(all_the_labels)):
-        final_map[el] = i + 1 * (1 - if_env0)
+    for i, elem in enumerate(np.unique(all_the_labels)):
+        final_map[elem] = i + 1 * (1 - if_env0)
     for i, particle in enumerate(all_the_labels):
-        for j, el in enumerate(particle):
-            all_the_labels[i][j] = final_map[el]
+        for j, elem in enumerate(particle):
+            all_the_labels[i][j] = final_map[elem]
 
     # Remove merged states from the state list
     states_to_remove = set(s0 for s0, s1 in best_merge)
     updated_states = [
         state
         for i, state in enumerate(list_of_states)
         if i not in states_to_remove
@@ -512,14 +561,107 @@
             file=file,
         )
 
     # Step 5: Return the 'updated_states' as the output of the function.
     return updated_states, all_the_labels
 
 
+def find_max_prob_state(
+    window: np.ndarray,
+    old_label: int,
+    list_of_states: List[StateUni],
+) -> int:
+    """
+    Assign a singla window to the state for which the belonging
+    is the most probable.
+
+    Parameters
+    ----------
+
+    window : np.ndarray of shape (tau_window,)
+        The signal window to assign to a state.
+
+    old_label : int
+        The temporary label for the considered signal window.
+
+    list_of_states : List[StateUni]
+        List of the identified states.
+
+    Returns
+    -------
+
+    new_label : int
+        The label for the considered signal window.
+
+    Notes
+    -----
+
+    I am using the meadian here, instead of the mean, because it's more
+    robust against outliers. Not sure if this is the best chioce.
+    """
+    median_x = np.median(window)
+    new_label = old_label
+    if median_x < list_of_states[old_label - 1].th_inf[0]:
+        new_label -= 1
+    elif median_x > list_of_states[old_label - 1].th_sup[0]:
+        new_label += 1
+    return new_label
+
+
+def max_prob_assignment(
+    list_of_states: List[StateUni],
+    matrix: np.ndarray,
+    all_the_labels: np.ndarray,
+    tau_window: int,
+) -> Tuple[np.ndarray, List[StateUni]]:
+    """
+    After all the states have been identified, assign each window.
+    Each signal window is assignet to the most probable state.
+
+    Parameters
+    ----------
+
+    list_of_states : List[StateUni]
+        List of the identified states.
+
+    matrix : np.ndarray of shape (num_of_particles, num_of_timesteps)
+        The data to cluster.
+
+    all_the_labels : np.ndarray of shape (num_of_particles, num_of_windows)
+        The temporary labels assigned to the signal windows.
+
+    tau_window : int
+        The time resolution of the analysis.
+
+    Returns
+    -------
+
+    final_labels : np.ndarray of shape (num_of_particles, num_of_windows)
+        The definitive labels for all the signal windows.
+
+    list_of_states : List[StateUni]
+        List of the identified states, with updated percetages.
+    """
+    final_labels = np.zeros(all_the_labels.shape, dtype=int)
+    for i, mol in enumerate(all_the_labels):
+        for j, old_label in enumerate(mol):
+            if old_label > 0:
+                window = matrix[i][tau_window * j : tau_window * (j + 1)]
+                new_label = find_max_prob_state(
+                    window, old_label, list_of_states
+                )
+                final_labels[i][j] = new_label
+
+    for i, state in enumerate(list_of_states):
+        num_of_points = np.sum(final_labels == i + 1)
+        state.perc = num_of_points / final_labels.size
+
+    return final_labels, list_of_states
+
+
 def relabel_states_2d(
     all_the_labels: np.ndarray, states_list: list[StateMulti]
 ) -> Tuple[np.ndarray, List[StateMulti]]:
     """
     Reorders labels and merges strongly overlapping states in a
     multidimensional space.
```

### Comparing `onion_clustering-0.2.0/src/onion_clustering/main.py` & `onion_clustering-0.2.1/src/onion_clustering/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,24 +2,27 @@
 Code for clustering of univariate time-series data.
 See the documentation for all the details.
 """
 
 import copy
 import os
 import shutil
+import warnings
 from typing import List, Tuple, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy.signal
+from scipy.optimize import OptimizeWarning
 
 from onion_clustering.classes import ClusteringObject1D
 from onion_clustering.first_classes import Parameters, StateUni, UniData
 from onion_clustering.functions import (
     gaussian,
+    max_prob_assignment,
     moving_average,
     param_grid,
     plot_histo,
     read_input_data,
     relabel_states,
     set_final_states,
 )
@@ -27,14 +30,28 @@
 OUTPUT_FILE = "states_output.txt"
 
 
 def all_the_input_stuff(number_of_sigmas: float) -> ClusteringObject1D:
     """
     Reads input parameters and raw data from specified files and directories,
     processes the raw data, and creates output files.
+
+    Parameters
+    ----------
+
+    number_of_sigmas : float
+        The signal windos are classified inside a state with a certain mean
+        and std_dev if all the points differ from the mean less than
+        std_dev * number_of_sigmas.
+
+    Returns
+    -------
+
+    clustering_object : ClusteringObject1D
+        The object containing all the information and data for the analysis.
     """
     # Read input parameters from files.
     data_directory = read_input_data()
     par = Parameters("input_parameters.txt")
     par.print_to_screen()
 
     # Read raw data from the specified directory/files.
@@ -67,92 +84,109 @@
     return clustering_object
 
 
 def perform_gauss_fit(
     param: List[int],
     data: List[np.ndarray],
     int_type: str,
-) -> Tuple[bool, int, np.ndarray]:
+) -> Tuple[bool, float, np.ndarray]:
     """
     Perform Gaussian fit on given data.
 
-    Args:
-    - id0 (int): Index representing the lower limit for data selection.
-    - id1 (int): Index representing the upper limit for data selection.
-    - bins (np.ndarray): Array containing bin values.
-    - counts (np.ndarray): Array containing counts corresponding to bins.
-    - n_data (int): Number of data points.
-    - gap (int): Gap value for the fit.
-    - interval_type (str): Type of interval.
-
-    Returns:
-    - tuple: A tuple containing:
-        - bool: True if the fit is successful, False otherwise.
-        - int: Goodness value calculated based on fit quality.
-        - array or None: Parameters of the Gaussian fit if successful,
-            None otherwise.
+    Parameters
+    ----------
+
+    id0 : int
+        Index representing the lower limit for data selection.
+
+    id1 : int
+        Index representing the upper limit for data selection.
+
+    bins : np.ndarray
+        Array containing bin values.
+
+    counts : np.ndarray
+        Array containing counts corresponding to bins.
+
+    n_data : int
+        Number of data points.
+
+    interval_type : str
+        Type of interval ("min" of "half").
+
+    Returns
+    -------
+
+    bool
+        True if the fit is successful, False otherwise.
+
+    coeff_det_r2 : float
+        Coefficient of determination of the fit. Zero if the fit fails.
+
+    popt : np.ndarray or None
+        Parameters of the Gaussian fit if successful, None otherwise.
     """
-    id0, id1, max_ind, n_data, gap = param
+    id0, id1, max_ind, n_data = param
     bins, counts = data
 
-    goodness = 5
     selected_bins = bins[id0:id1]
     selected_counts = counts[id0:id1]
     mu0 = bins[max_ind]
     sigma0 = (bins[id1] - bins[id0]) / 6
     area0 = counts[max_ind] * np.sqrt(np.pi) * sigma0
     try:
-        popt, pcov, _, _, _ = scipy.optimize.curve_fit(
-            gaussian,
-            selected_bins,
-            selected_counts,
-            p0=[mu0, sigma0, area0],
-            full_output=True,
-        )
-        if popt[1] < 0:
-            popt[1] *= -1
-            popt[2] *= -1
-        gauss_max = popt[2] * np.sqrt(np.pi) * popt[1]
-        if gauss_max < area0 / 2:
-            goodness -= 1
-        popt[2] *= n_data
-        if popt[0] < selected_bins[0] or popt[0] > selected_bins[-1]:
-            goodness -= 1
-        if popt[1] > selected_bins[-1] - selected_bins[0]:
-            goodness -= 1
-        perr = np.sqrt(np.diag(pcov))
-        for j, par_err in enumerate(perr):
-            if par_err / popt[j] > 0.5:
-                goodness -= 1
-        if id1 - id0 <= gap:
-            goodness -= 1
-        return True, goodness, popt
+        with warnings.catch_warnings():
+            warnings.filterwarnings("error")
+            popt, _, infodict, _, _ = scipy.optimize.curve_fit(
+                gaussian,
+                selected_bins,
+                selected_counts,
+                p0=[mu0, sigma0, area0],
+                full_output=True,
+            )
+            if popt[1] < 0:
+                popt[1] *= -1
+                popt[2] *= -1
+            popt[2] *= n_data
+            ss_res = np.sum(infodict["fvec"] ** 2)
+            ss_tot = np.sum((selected_counts - np.mean(selected_counts)) ** 2)
+            coeff_det_r2 = 1 - ss_res / ss_tot
+            return True, coeff_det_r2, popt
+    except OptimizeWarning:
+        print(f"\t{int_type} fit: Optimize warning. ")
+        return (
+            False,
+            0,
+            np.empty(
+                3,
+            ),
+        )
     except RuntimeError:
-        print("\t" + int_type + " fit: Runtime error. ")
+        print(f"\t{int_type} fit: Runtime error. ")
         return (
             False,
-            goodness,
+            0,
             np.empty(
                 3,
             ),
         )
     except TypeError:
-        print("\t" + int_type + " fit: TypeError.")
+        print(f"\t{int_type} fit: TypeError.")
         return (
             False,
-            goodness,
+            0,
             np.empty(
                 3,
             ),
         )
     except ValueError:
-        print("\t" + int_type + " fit: ValueError.")
+        print(f"\t{int_type} fit: ValueError.")
         return (
             False,
-            goodness,
+            0,
             np.empty(
                 3,
             ),
         )
 
 
 def gauss_fit_max(
@@ -161,31 +195,48 @@
     number_of_sigmas: float,
     filename: str,
     full_out: bool,
 ) -> Union[StateUni, None]:
     """
     Performs Gaussian fitting on input data.
 
-    Args:
-    - m_clean (np.ndarray): Input data for Gaussian fitting.
-    - par (Parameters): Object containing parameters for fitting.
-    - filename (str): Name of the output plot file.
-
-    Returns:
-    - state (StateUni): Object containing Gaussian fit parameters
-        (mu, sigma, area) or None if the fit fails.
+    Parameters
+    ----------
+
+    m_clean : np.ndarray
+        Input data for Gaussian fitting.
+
+    par : Parameters
+        Object containing parameters for fitting.
+
+    number_of_sigmas : float
+        To set the thresholds for assigning windows to the state.
+
+    filename : str
+        Name of the output plot file.
+
+    full_output : bool
+        If True, plot all the intermediate histograms with the best fit.
+        Useful for debugging.
+
+    Returns
+    -------
+
+    state : StateUni
+        Object containing Gaussian fit parameters (mu, sigma, area)
+        or None if the fit fails.
     """
     print("* Gaussian fit...")
     flat_m = m_clean.flatten()
 
     ### 1. Histogram ###
     counts, bins = np.histogram(flat_m, bins=par.bins, density=True)
     gap = 1
-    if bins.size > 99:
-        gap = int(bins.size * 0.02)
+    if bins.size > 49:
+        gap = int(bins.size * 0.02) * 2
     print(f"\tNumber of bins = {bins.size}, gap = {gap}")
 
     ### 2. Smoothing with tau = 3 ###
     counts = moving_average(counts, gap)
     bins = moving_average(bins, gap)
     if (counts == 0.0).any():
         print(
@@ -202,57 +253,46 @@
     min_id1 = np.min([max_ind + gap, counts.size - 1])
     while min_id0 > 0 and counts[min_id0] > counts[min_id0 - 1]:
         min_id0 -= 1
     while min_id1 < counts.size - 1 and counts[min_id1] > counts[min_id1 + 1]:
         min_id1 += 1
 
     ### 5. Try the fit between the minima and check its goodness ###
-    fit_param = [min_id0, min_id1, max_ind, flat_m.size, gap]
+    fit_param = [min_id0, min_id1, max_ind, flat_m.size]
     fit_data = [bins, counts]
-    flag_min, goodness_min, popt_min = perform_gauss_fit(
-        fit_param, fit_data, "Min"
-    )
+    flag_min, r_2_min, popt_min = perform_gauss_fit(fit_param, fit_data, "Min")
 
     ### 6. Find the inrterval of half height ###
     half_id0 = np.max([max_ind - gap, 0])
     half_id1 = np.min([max_ind + gap, counts.size - 1])
     while half_id0 > 0 and counts[half_id0] > max_val / 2:
         half_id0 -= 1
     while half_id1 < counts.size - 1 and counts[half_id1] > max_val / 2:
         half_id1 += 1
 
     ### 7. Try the fit between the minima and check its goodness ###
-    fit_param = [half_id0, half_id1, max_ind, flat_m.size, gap]
+    fit_param = [half_id0, half_id1, max_ind, flat_m.size]
     fit_data = [bins, counts]
-    flag_half, goodness_half, popt_half = perform_gauss_fit(
+    flag_half, r_2_half, popt_half = perform_gauss_fit(
         fit_param, fit_data, "Half"
     )
 
-    ### 7.bis Avoid that the ENV0 is hidden in a very large Gaussian ###
-    data_range = np.max(m_clean) - np.min(m_clean)
-    if popt_min[1] > data_range / 4:
-        print("\tWARNING: sigma is too large, fit discarded.")
-        flag_min = False
-    if popt_half[1] > data_range / 4:
-        print("\tWARNING: sigma is too large, fit discarded.")
-        flag_half = False
-
     ### 8. Choose the best fit ###
-    goodness = goodness_min
+    r_2 = r_2_min
     if flag_min == 1 and flag_half == 0:
         popt = popt_min
     elif flag_min == 0 and flag_half == 1:
         popt = popt_half
-        goodness = goodness_half
+        r_2 = r_2_half
     elif flag_min * flag_half == 1:
-        if goodness_min >= goodness_half:
+        if r_2_min >= r_2_half:
             popt = popt_min
         else:
             popt = popt_half
-            goodness = goodness_half
+            r_2 = r_2_half
     else:
         print("\tWARNING: this fit is not converging.")
         return None
 
     state = StateUni(popt[0], popt[1], popt[2])
     state.build_boundaries(number_of_sigmas)
 
@@ -263,15 +303,15 @@
             f" area = {state.area:.4f}"
         )
         print(
             f"\tmu = {state.mean:.4f}, sigma = {state.sigma:.4f},"
             f" area = {state.area:.4f}",
             file=file,
         )
-        print("\tFit goodness = " + str(goodness), file=file)
+        print(f"\tFit r2 = {r_2}", file=file)
 
     if full_out:
         ### Plot the distribution and the fitted gaussians
         y_spread = np.max(m_clean) - np.min(m_clean)
         y_lim = [
             np.min(m_clean) - 0.025 * y_spread,
             np.max(m_clean) + 0.025 * y_spread,
@@ -294,26 +334,41 @@
 def find_stable_trj(
     cl_ob: ClusteringObject1D,
     state: StateUni,
     tmp_labels: np.ndarray,
     lim: int,
 ) -> Tuple[np.ndarray, float, bool]:
     """
-    Identifies stable windows in a trajectory.
+    Identifies stable windows within a state.
+
+    Parameters
+    ----------
 
-    Args:
-    - cl_ob (ClusteringObject1D): the clustering object
-    - state (StateUni): Object containing stable state parameters.
-    - all_the_labels (np.ndarray): Labels indicating window classifications.
-    - offset (int): Offset value for classifying stable windows.
-
-    Returns:
-    - m2_array (np.ndarray): Array of non-stable windows.
-    - fw (float): Fraction of windows classified as stable.
-    - one_last_state (bool): Indicates if there's one last state remaining.
+    cl_ob : ClusteringObject1D
+
+    state : StateUni
+        Object containing stable state parameters.
+
+    all_the_labels : np.ndarray
+        Labels indicating window classifications.
+
+    offset : int
+        Offset value for classifying stable windows.
+
+    Returns
+    -------
+
+    m2_array : np.ndarray
+        Array of non-stable windows.
+
+    fw : float
+        Fraction of windows classified as stable.
+
+    one_last_state : bool
+        Indicates if there's one last state remaining.
     """
     print("* Finding stable windows...")
 
     # Calculate the number of windows in the trajectory
     number_of_windows = tmp_labels.shape[1]
     m_clean = cl_ob.data.matrix
     tau_window = cl_ob.par.tau_w
@@ -350,38 +405,213 @@
             f" = {window_fraction:.3}",
             file=file,
         )
 
     # Convert the list of non-stable windows to a NumPy array
     m2_array = np.array(remaning_data)
     one_last_state = True
-    if len(m2_array) == 0:
+    if m2_array.size == 0:
         one_last_state = False
 
     # Return the array of non-stable windows, the fraction of stable windows,
     # and the updated list_of_states
     return m2_array, window_fraction, one_last_state
 
 
+def solve_batman(
+    cl_ob: ClusteringObject1D,
+    m_clean: np.ndarray,
+    par: Parameters,
+    number_of_sigmas: float,
+    tmp_labels: np.ndarray,
+    tau_window: int,
+    lim: int,
+):
+    """
+    This functions takes care of particular cases where the
+    data points on the tails of a Gaussian are not correctly assigned,
+    creating weird sharp peaks in the hsistogram.
+
+    Parameters
+    ----------
+
+    cl_ob : ClusteringObject1D
+
+    m_clean : np.ndarray
+        Input data for Gaussian fitting.
+
+    par : Parameters
+        Object containing parameters for fitting.
+
+    number_of_sigmas : float
+        To set the thresholds for assigning windows to the state.
+
+    tmp_labels : np.ndarray
+        Labels indicating window classifications.
+
+    tau_windw : int
+        The time resolution of the analysis.
+
+    lim : int
+        Offset value for classifying stable windows.
+    """
+    flat_m = m_clean.flatten()
+
+    ### 1. Histogram ###
+    counts, bins = np.histogram(flat_m, bins=par.bins, density=True)
+    gap = 1
+    if bins.size > 99:
+        gap = int(bins.size * 0.02)
+    print(f"\tNumber of bins = {bins.size}, gap = {gap}")
+
+    ### 2. Smoothing with tau = 3 ###
+    counts = moving_average(counts, gap)
+    bins = moving_average(bins, gap)
+    if (counts == 0.0).any():
+        print(
+            "\tWARNING: there are empty bins. "
+            "Consider reducing the number of bins."
+        )
+
+    ### 3. Find the maxima ###
+    max_ind, _ = scipy.signal.find_peaks(counts)
+    max_val = np.array([counts[i] for i in max_ind])
+
+    for i, m_ind in enumerate(max_ind[:1]):
+        ### 4. Find the minima surrounding it ###
+        min_id0 = np.max([m_ind - gap, 0])
+        min_id1 = np.min([m_ind + gap, counts.size - 1])
+        while min_id0 > 0 and counts[min_id0] > counts[min_id0 - 1]:
+            min_id0 -= 1
+        while (
+            min_id1 < counts.size - 1 and counts[min_id1] > counts[min_id1 + 1]
+        ):
+            min_id1 += 1
+
+        ### 5. Try the fit between the minima and check its goodness ###
+        fit_param = [min_id0, min_id1, m_ind, flat_m.size]
+        fit_data = [bins, counts]
+        flag_min, r_2_min, popt_min = perform_gauss_fit(
+            fit_param, fit_data, "Min"
+        )
+
+        ### 6. Find the inrterval of half height ###
+        half_id0 = np.max([m_ind - gap, 0])
+        half_id1 = np.min([m_ind + gap, counts.size - 1])
+        while half_id0 > 0 and counts[half_id0] > max_val[i] / 2:
+            half_id0 -= 1
+        while half_id1 < counts.size - 1 and counts[half_id1] > max_val[i] / 2:
+            half_id1 += 1
+
+        ### 7. Try the fit between the minima and check its goodness ###
+        fit_param = [half_id0, half_id1, m_ind, flat_m.size]
+        fit_data = [bins, counts]
+        flag_half, r_2_half, popt_half = perform_gauss_fit(
+            fit_param, fit_data, "Half"
+        )
+
+        ### 8. Choose the best fit ###
+        if flag_min == 1 and flag_half == 0:
+            popt = popt_min
+        elif flag_min == 0 and flag_half == 1:
+            popt = popt_half
+        elif flag_min * flag_half == 1:
+            if r_2_min >= r_2_half:
+                popt = popt_min
+            else:
+                popt = popt_half
+        else:
+            continue
+
+        state = StateUni(popt[0], popt[1], popt[2])
+        state.build_boundaries(number_of_sigmas)
+
+        # Calculate the number of windows in the trajectory
+        number_of_windows = tmp_labels.shape[1]
+
+        mask_unclassified = tmp_labels < 0.5
+        m_reshaped = cl_ob.data.matrix[
+            :, : number_of_windows * tau_window
+        ].reshape(cl_ob.data.matrix.shape[0], number_of_windows, tau_window)
+        mask_inf = np.min(m_reshaped, axis=2) >= state.th_inf[0]
+        mask_sup = np.max(m_reshaped, axis=2) <= state.th_sup[0]
+        mask = mask_unclassified & mask_inf & mask_sup
+
+        tmp_labels[mask] = lim + 1
+        counter = np.sum(mask)
+
+        # Initialize an empty list to store non-stable windows
+        remaning_data = []
+        mask_remaining = mask_unclassified & ~mask
+        for i, window in np.argwhere(mask_remaining):
+            r_w = cl_ob.data.matrix[
+                i, window * tau_window : (window + 1) * tau_window
+            ]
+            remaning_data.append(r_w)
+
+        # Calculate the fraction of stable windows found
+        window_fraction = counter / (tmp_labels.size)
+
+        # Print the fraction of stable windows
+        with open(OUTPUT_FILE, "a", encoding="utf-8") as file:
+            print(
+                f"\tFraction of windows in state {lim + 1}"
+                f" = {window_fraction:.3}"
+            )
+            print(
+                f"\tFraction of windows in state {lim + 1}"
+                f" = {window_fraction:.3}",
+                file=file,
+            )
+
+        # Convert the list of non-stable windows to a NumPy array
+        m2_array = np.array(remaning_data)
+        one_last_state = True
+        if len(m2_array) == 0:
+            one_last_state = False
+
+        # Return the array of non-stable windows, the fraction of stable windows,
+        # and the updated list_of_states
+        return state, m2_array, window_fraction, one_last_state
+
+    # If event trying all the maxima does not work, surrend
+    return None, None, None, None
+
+
 def iterative_search(
     cl_ob: ClusteringObject1D,
     name: str,
     full_out: bool,
 ) -> Tuple[ClusteringObject1D, np.ndarray, bool]:
     """
     Performs an iterative search for stable states in a trajectory.
 
-    Args:
-    - cl_ob (ClusteringObject1D).
-    - name (str): Name for identifying output figures.
-
-    Returns:
-    - cl_ob (ClusteringObject1D): updated with the clustering results.
-    - atl (np.ndarray): temporary array of labels
-    - one_last_state (bool): Indicates if there's one last state remaining.
+    Parameters
+    ----------
+
+    cl_ob : ClusteringObject1D
+
+    name : str
+        Name for identifying output figures.
+
+    full_output : bool
+        If True, plot all the intermediate histograms with the best fit.
+        Useful for debugging.
+
+    Returns
+    -------
+
+    cl_ob : ClusteringObject1D
+        Updated with the clustering results.
+
+    atl : np.ndarray of shape (n_particles, n_windows)
+        Temporary array of labels.
+
+    one_last_state : bool
+        Indicates if there's one last state remaining.
     """
 
     # Initialize an array to store labels for each window.
     num_windows = int(cl_ob.data.num_of_steps / cl_ob.par.tau_w)
     tmp_labels = np.zeros((cl_ob.data.num_of_particles, num_windows)).astype(
         int
     )
@@ -396,38 +626,51 @@
     one_last_state = False
     while True:
         ### Locate and fit maximum in the signal distribution
         state = gauss_fit_max(
             m_copy,
             cl_ob.par,
             cl_ob.number_of_sigmas,
-            "output_figures/" + name + "Fig1_" + str(iteration_id),
+            f"output_figures/{name}Fig1_{iteration_id}",
             full_out,
         )
         if state is None:
             print("Iterations interrupted because fit does not converge. ")
             break
 
         ### Find the windows in which the trajectories are stable
         m_next, counter, one_last_state = find_stable_trj(
             cl_ob, state, tmp_labels, states_counter
         )
-        state.perc = counter
 
+        ### Exit the loop if no new stable windows are found
+        if counter <= 0.0:
+            state, m_next, counter, one_last_state = solve_batman(
+                cl_ob,
+                m_copy,
+                cl_ob.par,
+                cl_ob.number_of_sigmas,
+                tmp_labels,
+                cl_ob.par.tau_w,
+                states_counter,
+            )
+
+            if counter == 0 or state is None:
+                print("Iterations interrupted because last state is empty. ")
+                break
+
+        state.perc = counter
         states_list.append(state)
         states_counter += 1
         iteration_id += 1
-        ### Exit the loop if no new stable windows are found
-        if counter <= 0.0:
-            print("Iterations interrupted because last state is empty. ")
-            break
+        m_copy = m_next
+
         if m_next.size == 0:
             print("Iterations interrupted because all points are classififed.")
             break
-        m_copy = m_next
 
     cl_ob.iterations = len(states_list)
     atl, lis = relabel_states(tmp_labels, states_list)
     cl_ob.states = lis
     return cl_ob, atl, one_last_state
 
 
@@ -436,50 +679,67 @@
     tau_w: int,
     t_smooth: int,
     full_out: bool,
 ) -> Tuple[int, float, List[float]]:
     """
     Performs an analysis pipeline on time series data.
 
-    Args:
-    - cl_ob (ClusteringObject1D)
-    - tau_w (int): the time window for the analysis
-    - t_smooth (int): the width of the moving average for the analysis
-
-    Returns:
-    - num_states (int): Number of identified states.
-    - fraction_0 (float): Fraction of unclassified data points.
-    - list_of_pop (List[float]): List of the populations of the different
-        states.
+    Parameters
+    ----------
+
+    cl_ob : ClusteringObject1D
+
+    tau_w : int
+        The time resolution for the analysis.
+
+    t_smooth : int
+        The width of the moving average for the analysis.
+
+    Returns
+    -------
+
+    num_states : int
+        Number of identified states.
+
+    fraction_0 : float
+        Fraction of unclassified data points. Between 0 and 1.
+
+    list_of_pop : List[float]
+        List of the populations of the different states.
     """
 
     print("* New analysis: ", tau_w, t_smooth)
     name = str(t_smooth) + "_" + str(tau_w) + "_"
 
     tmp_cl_ob = copy.deepcopy(cl_ob)
     tmp_cl_ob.par.tau_w = tau_w
     tmp_cl_ob.par.t_smooth = t_smooth
 
     tmp_cl_ob.preparing_the_data()
     tmp_cl_ob.plot_input_data(name + "Fig0")
 
-    tmp_cl_ob, tmp_labels, one_last_state = iterative_search(
-        tmp_cl_ob, name, full_out
-    )
+    tmp_cl_ob, tmp_labels, _ = iterative_search(tmp_cl_ob, name, full_out)
 
     if len(tmp_cl_ob.states) == 0:
         print("* No possible classification was found. ")
         # We need to free the memory otherwise it accumulates
         del tmp_cl_ob
         return 0, 1.0, [1.0]
 
-    tmp_cl_ob.states, tmp_cl_ob.data.labels = set_final_states(
+    list_of_states, tmp_labels = set_final_states(
         tmp_cl_ob.states, tmp_labels, tmp_cl_ob.data.range
     )
 
+    tmp_cl_ob.data.labels, tmp_cl_ob.states = max_prob_assignment(
+        list_of_states,
+        tmp_cl_ob.data.matrix,
+        tmp_labels,
+        tau_w,
+    )
+
     list_of_pop = [state.perc for state in tmp_cl_ob.states]
     fraction_0 = 1 - np.sum(list_of_pop)
     list_of_pop.insert(0, fraction_0)
     n_states = len(tmp_cl_ob.states)
 
     # We need to free the memory otherwise it accumulates
     del tmp_cl_ob
@@ -490,36 +750,68 @@
     return n_states, fraction_0, list_of_pop
 
 
 def full_output_analysis(
     cl_ob: ClusteringObject1D,
     full_out: bool,
 ) -> ClusteringObject1D:
-    """Perform a comprehensive analysis on the input data."""
+    """
+    Perform a comprehensive analysis on the input data.
+
+    Parameters
+    ----------
+
+    cl_ob : ClusteringObject1D
+
+    full_out : bool
+        If True, plot all the intermediate histograms with the best fit.
+        Useful for debugging.
+
+    Returns
+    -------
+
+    cl_ob : ClusteringObject1D
+        Updated with the clustering results.
+    """
 
     cl_ob.preparing_the_data()
 
     cl_ob, tmp_labels, _ = iterative_search(cl_ob, "", full_out)
     if len(cl_ob.states) == 0:
         print("* No possible classification was found. ")
         return cl_ob
-    cl_ob.states, cl_ob.data.labels = set_final_states(
+    list_of_states, tmp_labels = set_final_states(
         cl_ob.states, tmp_labels, cl_ob.data.range
     )
 
+    cl_ob.data.labels, cl_ob.states = max_prob_assignment(
+        list_of_states,
+        cl_ob.data.matrix,
+        tmp_labels,
+        cl_ob.par.tau_w,
+    )
+
     return cl_ob
 
 
-def time_resolution_analysis(cl_ob: ClusteringObject1D, full_out: bool):
+def time_resolution_analysis(
+    cl_ob: ClusteringObject1D,
+    full_out: bool,
+):
     """
     Performs Temporal Resolution Analysis (TRA) to explore parameter
     space and analyze the dataset.
 
-    Args:
-    - cl_ob (ClusteringObject1D): Conteining now only the raw input data.
+    Parameters
+    ----------
+    cl_ob : ClusteringObject1D
+
+    full_out : bool
+        If True, plot all the intermediate histograms with the best fit.
+        Useful for debugging.
     """
     tau_window_list, t_smooth_list = param_grid(
         cl_ob.par, cl_ob.data.num_of_steps
     )
     cl_ob.tau_window_list = np.array(tau_window_list)
     cl_ob.t_smooth_list = np.array(t_smooth_list)
 
@@ -560,22 +852,39 @@
     cl_ob.number_of_states = number_of_states_arr
     cl_ob.fraction_0 = fraction_0_arr
     cl_ob.list_of_pop = list_of_pop
 
 
 def main(
     full_output: bool = True,
-    number_of_sigmas: float = 1.5,
+    number_of_sigmas: float = 2.0,
 ) -> ClusteringObject1D:
     """
     Returns the clustering object with the analysi.
 
+    Parameters
+    ----------
+
+    full_output : bool
+        If True, plot all the intermediate histograms with the best fit.
+        Useful for debugging.
+
+    number_of_sigmas : float
+        The signal windos are classified inside a state with a certain mean
+        and std_dev if all the points differ from the mean less than
+        std_dev * number_of_sigmas.
+
+    Notes
+    -----
+
     all_the_input_stuff() reads the data and the parameters
+
     time_resolution_analysis() explore the parameter
         (tau_window, t_smooth) space.
+
     full_output_analysis() performs a detailed analysis
         with the chosen parameters.
     """
     print("##############################################################")
     print("# If you publish results using onion-clustering, please cite #")
     print("# this work: https://doi.org/10.48550/arXiv.2402.07786.      #")
     print("##############################################################")
```

### Comparing `onion_clustering-0.2.0/src/onion_clustering/main_2d.py` & `onion_clustering-0.2.1/src/onion_clustering/main_2d.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.0/src/onion_clustering/utilities.py` & `onion_clustering-0.2.1/src/onion_clustering/utilities.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.0/src/onion_clustering.egg-info/PKG-INFO` & `onion_clustering-0.2.1/src/onion_clustering.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onion_clustering
-Version: 0.2.0
+Version: 0.2.1
 Summary: Code for unsupervised clustering of time-correlated data.
 Maintainer-email: Matteo Becchi <bechmath@gmail.com>
 Project-URL: github, https://github.com/matteobecchi/timeseries_analysis/
 Requires-Python: <3.11,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
```

### Comparing `onion_clustering-0.2.0/src/onion_clustering.egg-info/SOURCES.txt` & `onion_clustering-0.2.1/src/onion_clustering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.0/test/test_multi.py` & `onion_clustering-0.2.1/test/test_multi.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.0/test/test_uni.py` & `onion_clustering-0.2.1/test/test_uni.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 
 import pytest
 from onion_clustering import main as onion
 
 ### Set all the analysis parameters ###
 FILE = "water_coex_100ps_1nm_LENS.npy"
 PATH_TO_INPUT_DATA = "/Users/mattebecchi/00_signal_analysis/data/" + FILE
-TAU_WINDOW = 10  # time resolution of the analysis
-T_DELAY = 1  # remove the first t_delay frames (default 0)
-T_CONV = 0.1  # convert frames in time units (default 1)
-T_UNITS = "ns"  # the time units (default 'frames')
+TAU_WINDOW = 10
+T_DELAY = 1
 NUM_TAU_W = 2
 MAX_TAU_W = 10
-MAX_T_SMOOTH = 2  # max value of t_smooth tested (default 5)
+MAX_T_SMOOTH = 2
 
 
 # Define a fixture to set up the test environment
 @pytest.fixture
 def setup_test_environment(tmpdir):
     # tmpdir is a built-in pytest fixture providing a temporary directory
     original_dir = os.getcwd()  # Save the current working directory
@@ -33,16 +31,14 @@
     with open("data_directory.txt", "w+", encoding="utf-8") as file:
         print(PATH_TO_INPUT_DATA, file=file)
 
     ### Create the 'input_parameter.txt' file ###
     with open("input_parameters.txt", "w+", encoding="utf-8") as file:
         print("tau_window\t" + str(TAU_WINDOW), file=file)
         print("t_delay\t" + str(T_DELAY), file=file)
-        print("t_conv\t" + str(T_CONV), file=file)
-        print("t_units\t" + T_UNITS, file=file)
         print("num_tau_w\t" + str(NUM_TAU_W), file=file)
         print("max_tau_w\t" + str(MAX_TAU_W), file=file)
         print("max_t_smooth\t" + str(MAX_T_SMOOTH), file=file)
 
     # Call your code to generate the output files
     tmp = onion.main(False)
```

