# Comparing `tmp/cs2solutions-0.8.0.tar.gz` & `tmp/cs2solutions-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs2solutions-0.8.0.tar", last modified: Mon Apr 29 19:48:34 2024, max compression
+gzip compressed data, was "cs2solutions-0.8.1.tar", last modified: Sun May 12 18:10:21 2024, max compression
```

## Comparing `cs2solutions-0.8.0.tar` & `cs2solutions-0.8.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 19:48:34.784990 cs2solutions-0.8.0/
--rw-rw-rw-   0        0        0    35823 2024-02-17 10:04:18.000000 cs2solutions-0.8.0/LICENSE
--rw-rw-rw-   0        0        0    43040 2024-04-29 19:48:34.780651 cs2solutions-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0      727 2024-02-21 18:21:30.000000 cs2solutions-0.8.0/README.md
--rw-rw-rw-   0        0        0     1294 2024-04-29 19:47:44.000000 cs2solutions-0.8.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-29 19:48:34.784990 cs2solutions-0.8.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-29 19:48:34.701973 cs2solutions-0.8.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 19:48:34.751672 cs2solutions-0.8.0/src/cs2solutions/
--rw-rw-rw-   0        0        0      163 2024-04-29 19:47:44.000000 cs2solutions-0.8.0/src/cs2solutions/__init__.py
--rw-rw-rw-   0        0        0     7065 2024-04-29 19:47:44.000000 cs2solutions-0.8.0/src/cs2solutions/aircraft.py
--rw-rw-rw-   0        0        0        0 2024-04-29 19:47:44.000000 cs2solutions-0.8.0/src/cs2solutions/cs.py
--rw-rw-rw-   0        0        0     6142 2024-02-21 18:21:30.000000 cs2solutions-0.8.0/src/cs2solutions/cs2bot.py
--rw-rw-rw-   0        0        0    11149 2024-04-29 19:47:44.000000 cs2solutions-0.8.0/src/cs2solutions/decomp.py
--rw-rw-rw-   0        0        0    21713 2024-02-21 18:21:30.000000 cs2solutions-0.8.0/src/cs2solutions/discretization.py
--rw-rw-rw-   0        0        0    11230 2024-04-29 19:47:44.000000 cs2solutions-0.8.0/src/cs2solutions/duckiebot.py
--rw-rw-rw-   0        0        0     3480 2024-04-29 19:47:44.000000 cs2solutions-0.8.0/src/cs2solutions/inf_pkg.py
--rw-rw-rw-   0        0        0     7967 2024-02-21 18:21:30.000000 cs2solutions-0.8.0/src/cs2solutions/intro.py
--rw-rw-rw-   0        0        0    15791 2024-04-29 19:47:44.000000 cs2solutions-0.8.0/src/cs2solutions/intromimo.py
--rw-rw-rw-   0        0        0    13575 2024-04-29 19:47:44.000000 cs2solutions-0.8.0/src/cs2solutions/lqg.py
--rw-rw-rw-   0        0        0    11049 2024-04-29 19:47:44.000000 cs2solutions-0.8.0/src/cs2solutions/lqrfeedback.py
--rw-rw-rw-   0        0        0    13739 2024-02-21 18:21:30.000000 cs2solutions-0.8.0/src/cs2solutions/morse.py
--rw-rw-rw-   0        0        0    16030 2024-04-29 19:47:44.000000 cs2solutions-0.8.0/src/cs2solutions/norms.py
--rw-rw-rw-   0        0        0       93 2024-02-21 18:21:30.000000 cs2solutions-0.8.0/src/cs2solutions/plot.py
--rw-rw-rw-   0        0        0       68 2024-02-21 18:21:30.000000 cs2solutions-0.8.0/src/cs2solutions/test.py
-drwxrwxrwx   0        0        0        0 2024-04-29 19:48:34.768512 cs2solutions-0.8.0/src/cs2solutions.egg-info/
--rw-rw-rw-   0        0        0    43040 2024-04-29 19:48:34.000000 cs2solutions-0.8.0/src/cs2solutions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      673 2024-04-29 19:48:34.000000 cs2solutions-0.8.0/src/cs2solutions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 19:48:34.000000 cs2solutions-0.8.0/src/cs2solutions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-04-29 19:48:34.000000 cs2solutions-0.8.0/src/cs2solutions.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-29 19:48:34.000000 cs2solutions-0.8.0/src/cs2solutions.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 18:10:21.630238 cs2solutions-0.8.1/
+-rw-rw-rw-   0        0        0    35823 2024-02-17 10:04:18.000000 cs2solutions-0.8.1/LICENSE
+-rw-rw-rw-   0        0        0    43040 2024-05-12 18:10:21.630238 cs2solutions-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0      727 2024-02-21 18:21:30.000000 cs2solutions-0.8.1/README.md
+-rw-rw-rw-   0        0        0     1294 2024-05-12 16:53:49.000000 cs2solutions-0.8.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-12 18:10:21.630238 cs2solutions-0.8.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-12 18:10:21.605173 cs2solutions-0.8.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-12 18:10:21.616498 cs2solutions-0.8.1/src/cs2solutions/
+-rw-rw-rw-   0        0        0    12143 2024-05-12 17:53:10.000000 cs2solutions-0.8.1/src/cs2solutions/Qparam.py
+-rw-rw-rw-   0        0        0      173 2024-05-06 16:24:59.000000 cs2solutions-0.8.1/src/cs2solutions/__init__.py
+-rw-rw-rw-   0        0        0     7065 2024-04-29 19:47:44.000000 cs2solutions-0.8.1/src/cs2solutions/aircraft.py
+-rw-rw-rw-   0        0        0        0 2024-04-29 19:47:44.000000 cs2solutions-0.8.1/src/cs2solutions/cs.py
+-rw-rw-rw-   0        0        0     6142 2024-02-21 18:21:30.000000 cs2solutions-0.8.1/src/cs2solutions/cs2bot.py
+-rw-rw-rw-   0        0        0    11149 2024-04-29 19:47:44.000000 cs2solutions-0.8.1/src/cs2solutions/decomp.py
+-rw-rw-rw-   0        0        0    21713 2024-02-21 18:21:30.000000 cs2solutions-0.8.1/src/cs2solutions/discretization.py
+-rw-rw-rw-   0        0        0    11230 2024-04-29 19:47:44.000000 cs2solutions-0.8.1/src/cs2solutions/duckiebot.py
+-rw-rw-rw-   0        0        0     3480 2024-04-29 19:47:44.000000 cs2solutions-0.8.1/src/cs2solutions/inf_pkg.py
+-rw-rw-rw-   0        0        0     7967 2024-02-21 18:21:30.000000 cs2solutions-0.8.1/src/cs2solutions/intro.py
+-rw-rw-rw-   0        0        0    15791 2024-04-29 19:47:44.000000 cs2solutions-0.8.1/src/cs2solutions/intromimo.py
+-rw-rw-rw-   0        0        0    13575 2024-04-29 19:47:44.000000 cs2solutions-0.8.1/src/cs2solutions/lqg.py
+-rw-rw-rw-   0        0        0    11049 2024-04-29 19:47:44.000000 cs2solutions-0.8.1/src/cs2solutions/lqrfeedback.py
+-rw-rw-rw-   0        0        0    13739 2024-02-21 18:21:30.000000 cs2solutions-0.8.1/src/cs2solutions/morse.py
+-rw-rw-rw-   0        0        0    16030 2024-04-29 19:47:44.000000 cs2solutions-0.8.1/src/cs2solutions/norms.py
+-rw-rw-rw-   0        0        0       93 2024-02-21 18:21:30.000000 cs2solutions-0.8.1/src/cs2solutions/plot.py
+-rw-rw-rw-   0        0        0       68 2024-02-21 18:21:30.000000 cs2solutions-0.8.1/src/cs2solutions/test.py
+drwxrwxrwx   0        0        0        0 2024-05-12 18:10:21.628569 cs2solutions-0.8.1/src/cs2solutions.egg-info/
+-rw-rw-rw-   0        0        0    43040 2024-05-12 18:10:21.000000 cs2solutions-0.8.1/src/cs2solutions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      700 2024-05-12 18:10:21.000000 cs2solutions-0.8.1/src/cs2solutions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 18:10:21.000000 cs2solutions-0.8.1/src/cs2solutions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-05-12 18:10:21.000000 cs2solutions-0.8.1/src/cs2solutions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-12 18:10:21.000000 cs2solutions-0.8.1/src/cs2solutions.egg-info/top_level.txt
```

### Comparing `cs2solutions-0.8.0/LICENSE` & `cs2solutions-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.8.0/PKG-INFO` & `cs2solutions-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs2solutions
-Version: 0.8.0
+Version: 0.8.1
 Summary: A package containing solutions for the CS2 lecture at ETH Zürich
 Author-email: Kalle Laitinen <klaitinen@ethz.ch>, Dejan Milojevic <dejanmi@ethz.ch>, Niclas Scheuer <nscheuer@ethz.ch>
 Maintainer-email: Kalle Laitinen <klaitinen@ethz.ch>, Niclas Scheuer <nscheuer@ethz.ch>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `cs2solutions-0.8.0/README.md` & `cs2solutions-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.8.0/pyproject.toml` & `cs2solutions-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/solutions"]
 
 [project]
 name = "cs2solutions"
-version = "0.8.0"
+version = "0.8.1"
 dependencies =[
     "control",
     "matplotlib",
     "numpy",
     "scipy",
     "sympy",
     "pandas"
```

### Comparing `cs2solutions-0.8.0/src/cs2solutions/aircraft.py` & `cs2solutions-0.8.1/src/cs2solutions/aircraft.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.8.0/src/cs2solutions/cs2bot.py` & `cs2solutions-0.8.1/src/cs2solutions/cs2bot.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.8.0/src/cs2solutions/decomp.py` & `cs2solutions-0.8.1/src/cs2solutions/decomp.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.8.0/src/cs2solutions/discretization.py` & `cs2solutions-0.8.1/src/cs2solutions/discretization.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.8.0/src/cs2solutions/duckiebot.py` & `cs2solutions-0.8.1/src/cs2solutions/duckiebot.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.8.0/src/cs2solutions/inf_pkg.py` & `cs2solutions-0.8.1/src/cs2solutions/inf_pkg.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.8.0/src/cs2solutions/intro.py` & `cs2solutions-0.8.1/src/cs2solutions/intro.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.8.0/src/cs2solutions/intromimo.py` & `cs2solutions-0.8.1/src/cs2solutions/intromimo.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.8.0/src/cs2solutions/lqg.py` & `cs2solutions-0.8.1/src/cs2solutions/lqg.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.8.0/src/cs2solutions/lqrfeedback.py` & `cs2solutions-0.8.1/src/cs2solutions/lqrfeedback.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.8.0/src/cs2solutions/morse.py` & `cs2solutions-0.8.1/src/cs2solutions/morse.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.8.0/src/cs2solutions/norms.py` & `cs2solutions-0.8.1/src/cs2solutions/norms.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.8.0/src/cs2solutions.egg-info/PKG-INFO` & `cs2solutions-0.8.1/src/cs2solutions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs2solutions
-Version: 0.8.0
+Version: 0.8.1
 Summary: A package containing solutions for the CS2 lecture at ETH Zürich
 Author-email: Kalle Laitinen <klaitinen@ethz.ch>, Dejan Milojevic <dejanmi@ethz.ch>, Niclas Scheuer <nscheuer@ethz.ch>
 Maintainer-email: Kalle Laitinen <klaitinen@ethz.ch>, Niclas Scheuer <nscheuer@ethz.ch>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `cs2solutions-0.8.0/src/cs2solutions.egg-info/SOURCES.txt` & `cs2solutions-0.8.1/src/cs2solutions.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
+src/cs2solutions/Qparam.py
 src/cs2solutions/__init__.py
 src/cs2solutions/aircraft.py
 src/cs2solutions/cs.py
 src/cs2solutions/cs2bot.py
 src/cs2solutions/decomp.py
 src/cs2solutions/discretization.py
 src/cs2solutions/duckiebot.py
```

