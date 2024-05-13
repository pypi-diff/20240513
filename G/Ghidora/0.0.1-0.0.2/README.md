# Comparing `tmp/Ghidora-0.0.1.tar.gz` & `tmp/Ghidora-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Ghidora-0.0.1.tar", last modified: Sun Feb 21 15:51:24 2021, max compression
+gzip compressed data, was "Ghidora-0.0.2.tar", last modified: Mon May 13 15:33:50 2024, max compression
```

## Comparing `Ghidora-0.0.1.tar` & `Ghidora-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2021-02-21 15:51:24.182464 Ghidora-0.0.1/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2021-02-21 15:51:24.182464 Ghidora-0.0.1/Ghidora/
--rw-r--r--   0 runner    (1000) runner    (1000)     2433 2021-02-21 15:19:28.000000 Ghidora-0.0.1/Ghidora/Ghidora.py
--rw-r--r--   0 runner    (1000) runner    (1000)       21 2021-02-21 15:19:28.000000 Ghidora-0.0.1/Ghidora/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2021-02-21 15:51:24.182464 Ghidora-0.0.1/Ghidora.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      585 2021-02-21 15:51:23.000000 Ghidora-0.0.1/Ghidora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      181 2021-02-21 15:51:23.000000 Ghidora-0.0.1/Ghidora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2021-02-21 15:51:23.000000 Ghidora-0.0.1/Ghidora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2021-02-21 15:51:23.000000 Ghidora-0.0.1/Ghidora.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      585 2021-02-21 15:51:24.182464 Ghidora-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)       81 2021-02-21 15:23:49.000000 Ghidora-0.0.1/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2021-02-21 15:51:24.186465 Ghidora-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      722 2021-02-21 15:32:31.000000 Ghidora-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:33:50.648316 Ghidora-0.0.2/
+drwxrwxrwx   0        0        0        0 2024-05-13 15:33:50.641411 Ghidora-0.0.2/Ghidora/
+-rw-rw-rw-   0        0        0     2432 2024-05-13 15:23:06.000000 Ghidora-0.0.2/Ghidora/Ghidora.py
+-rw-rw-rw-   0        0        0       21 2024-05-13 15:22:55.000000 Ghidora-0.0.2/Ghidora/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:33:50.648316 Ghidora-0.0.2/Ghidora.egg-info/
+-rw-rw-rw-   0        0        0     2545 2024-05-13 15:33:50.000000 Ghidora-0.0.2/Ghidora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2024-05-13 15:33:50.000000 Ghidora-0.0.2/Ghidora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 15:33:50.000000 Ghidora-0.0.2/Ghidora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-13 15:33:50.000000 Ghidora-0.0.2/Ghidora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2024-05-13 15:22:55.000000 Ghidora-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2545 2024-05-13 15:33:50.648316 Ghidora-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2051 2024-05-13 15:22:55.000000 Ghidora-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-13 15:33:50.648316 Ghidora-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      722 2024-05-13 15:23:58.000000 Ghidora-0.0.2/setup.py
```

### Comparing `Ghidora-0.0.1/Ghidora/Ghidora.py` & `Ghidora-0.0.2/Ghidora/Ghidora.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,8 +69,8 @@
 new.factorial()
 
 new = NaturalLogarithm()
 new.natualLogarithm(1000)
 
 new = Logarithm(10)
 new.logarithm(1000)
-'''s
+'''
```

### Comparing `Ghidora-0.0.1/setup.py` & `Ghidora-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name = "Ghidora",
-    version = "0.0.1",
+    version = "0.0.2",
     author = "Jay Rank",
     author_email = "rank01jay01@gmail.com",
     description = "An abstract python library for calculating time complex math function.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/RankJay/Ghidora",
     packages = setuptools.find_packages(),
```

