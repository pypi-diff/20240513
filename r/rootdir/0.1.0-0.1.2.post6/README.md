# Comparing `tmp/rootdir-0.1.0.tar.gz` & `tmp/rootdir-0.1.2.post6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rootdir-0.1.0.tar", last modified: Sun May 12 15:53:57 2024, max compression
+gzip compressed data, was "rootdir-0.1.2.post6.tar", last modified: Mon May 13 15:01:40 2024, max compression
```

## Comparing `rootdir-0.1.0.tar` & `rootdir-0.1.2.post6.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 15:53:57.020949 rootdir-0.1.0/
--rw-rw-rw-   0        0        0      351 2024-05-12 15:53:57.019949 rootdir-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      112 2024-05-11 07:40:55.000000 rootdir-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 15:53:57.011951 rootdir-0.1.0/rootdir.egg-info/
--rw-rw-rw-   0        0        0      351 2024-05-12 15:53:56.000000 rootdir-0.1.0/rootdir.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2024-05-12 15:53:56.000000 rootdir-0.1.0/rootdir.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 15:53:56.000000 rootdir-0.1.0/rootdir.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-05-12 15:53:56.000000 rootdir-0.1.0/rootdir.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 15:53:57.020949 rootdir-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      479 2024-05-12 15:53:47.000000 rootdir-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:53:57.016959 rootdir-0.1.0/src/
--rw-rw-rw-   0        0        0      503 2024-05-12 15:53:29.000000 rootdir-0.1.0/src/RootDir.py
--rw-rw-rw-   0        0        0        0 2024-05-11 07:37:50.000000 rootdir-0.1.0/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:01:40.840359 rootdir-0.1.2.post6/
+-rw-rw-rw-   0        0        0      666 2024-05-13 15:01:40.839353 rootdir-0.1.2.post6/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2024-05-12 16:03:46.000000 rootdir-0.1.2.post6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 15:01:40.814358 rootdir-0.1.2.post6/rootdir/
+-rw-rw-rw-   0        0        0      659 2024-05-13 15:01:11.000000 rootdir-0.1.2.post6/rootdir/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:01:40.836349 rootdir-0.1.2.post6/rootdir.egg-info/
+-rw-rw-rw-   0        0        0      666 2024-05-13 15:01:40.000000 rootdir-0.1.2.post6/rootdir.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2024-05-13 15:01:40.000000 rootdir-0.1.2.post6/rootdir.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 15:01:40.000000 rootdir-0.1.2.post6/rootdir.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-13 15:01:40.000000 rootdir-0.1.2.post6/rootdir.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 15:01:40.841358 rootdir-0.1.2.post6/setup.cfg
+-rw-rw-rw-   0        0        0      520 2024-05-13 15:01:37.000000 rootdir-0.1.2.post6/setup.py
```

