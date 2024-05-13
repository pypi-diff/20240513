# Comparing `tmp/mergefast1-0.1.3.tar.gz` & `tmp/mergefast1-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mergefast1-0.1.3.tar", last modified: Mon May 13 11:08:25 2024, max compression
+gzip compressed data, was "mergefast1-0.1.4.tar", last modified: Mon May 13 11:23:56 2024, max compression
```

## Comparing `mergefast1-0.1.3.tar` & `mergefast1-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 11:08:25.199128 mergefast1-0.1.3/
--rw-rw-rw-   0        0        0       57 2024-05-13 11:08:25.196063 mergefast1-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-13 11:08:25.165387 mergefast1-0.1.3/mergefast/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:53:09.000000 mergefast1-0.1.3/mergefast/__init__.py
--rw-rw-rw-   0        0        0      549 2024-05-13 09:43:57.000000 mergefast1-0.1.3/mergefast/core.py
-drwxrwxrwx   0        0        0        0 2024-05-13 11:08:25.181182 mergefast1-0.1.3/mergefast1.egg-info/
--rw-rw-rw-   0        0        0       57 2024-05-13 11:08:25.000000 mergefast1-0.1.3/mergefast1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-05-13 11:08:25.000000 mergefast1-0.1.3/mergefast1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 11:08:25.000000 mergefast1-0.1.3/mergefast1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-13 11:08:25.000000 mergefast1-0.1.3/mergefast1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      625 2024-05-13 10:17:11.000000 mergefast1-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-13 11:08:25.199654 mergefast1-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      203 2024-05-13 11:08:08.000000 mergefast1-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 11:08:25.191841 mergefast1-0.1.3/tests/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:57:12.000000 mergefast1-0.1.3/tests/__init__.py
--rw-rw-rw-   0        0        0     1408 2024-05-13 09:57:15.000000 mergefast1-0.1.3/tests/perf.py
--rw-rw-rw-   0        0        0      711 2024-05-13 09:55:21.000000 mergefast1-0.1.3/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-05-13 11:23:56.813275 mergefast1-0.1.4/
+-rw-rw-rw-   0        0        0       57 2024-05-13 11:23:56.810274 mergefast1-0.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-13 11:23:56.775224 mergefast1-0.1.4/mergefast/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:53:09.000000 mergefast1-0.1.4/mergefast/__init__.py
+-rw-rw-rw-   0        0        0      549 2024-05-13 09:43:57.000000 mergefast1-0.1.4/mergefast/core.py
+drwxrwxrwx   0        0        0        0 2024-05-13 11:23:56.792763 mergefast1-0.1.4/mergefast1.egg-info/
+-rw-rw-rw-   0        0        0       57 2024-05-13 11:23:56.000000 mergefast1-0.1.4/mergefast1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-05-13 11:23:56.000000 mergefast1-0.1.4/mergefast1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 11:23:56.000000 mergefast1-0.1.4/mergefast1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-13 11:23:56.000000 mergefast1-0.1.4/mergefast1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      625 2024-05-13 10:17:11.000000 mergefast1-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 11:23:56.814281 mergefast1-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      203 2024-05-13 11:22:41.000000 mergefast1-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 11:23:56.805278 mergefast1-0.1.4/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:57:12.000000 mergefast1-0.1.4/tests/__init__.py
+-rw-rw-rw-   0        0        0     1408 2024-05-13 09:57:15.000000 mergefast1-0.1.4/tests/perf.py
+-rw-rw-rw-   0        0        0      711 2024-05-13 09:55:21.000000 mergefast1-0.1.4/tests/test.py
```

### Comparing `mergefast1-0.1.3/mergefast/core.py` & `mergefast1-0.1.4/mergefast/core.py`

 * *Files identical despite different names*

### Comparing `mergefast1-0.1.3/pyproject.toml` & `mergefast1-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mergefast1-0.1.3/tests/perf.py` & `mergefast1-0.1.4/tests/perf.py`

 * *Files identical despite different names*

### Comparing `mergefast1-0.1.3/tests/test.py` & `mergefast1-0.1.4/tests/test.py`

 * *Files identical despite different names*

