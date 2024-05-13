# Comparing `tmp/vsmetaEncoder-0.9.tar.gz` & `tmp/vsmetaencoder-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsmetaEncoder-0.9.tar", last modified: Wed Mar 17 07:12:38 2021, max compression
+gzip compressed data, was "vsmetaencoder-1.1.1.tar", last modified: Mon May 13 06:12:03 2024, max compression
```

## Comparing `vsmetaEncoder-0.9.tar` & `vsmetaencoder-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxrwxrwx   0        0        0        0 2021-03-17 07:12:29.651775 vsmetaEncoder-0.9/
--rw-rw-rw-   0        0        0     6225 2021-03-17 07:12:29.633112 vsmetaEncoder-0.9/PKG-INFO
--rw-rw-rw-   0        0        0     4833 2021-03-17 07:08:17.000000 vsmetaEncoder-0.9/README.md
--rw-rw-rw-   0        0        0       42 2021-03-17 07:12:29.665713 vsmetaEncoder-0.9/setup.cfg
--rw-rw-rw-   0        0        0      895 2021-03-17 07:10:59.000000 vsmetaEncoder-0.9/setup.py
-drwxrwxrwx   0        0        0        0 2021-03-17 07:12:28.878763 vsmetaEncoder-0.9/vsmetaEncoder/
--rw-rw-rw-   0        0        0      237 2021-03-17 06:55:59.000000 vsmetaEncoder-0.9/vsmetaEncoder/__init__.py
--rw-rw-rw-   0        0        0     7815 2021-02-28 21:08:33.000000 vsmetaEncoder-0.9/vsmetaEncoder/vsmetaBase.py
--rw-rw-rw-   0        0        0      190 2021-01-21 06:36:50.000000 vsmetaEncoder-0.9/vsmetaEncoder/vsmetaImageInfo.py
--rw-rw-rw-   0        0        0     1160 2021-03-02 21:52:53.000000 vsmetaEncoder-0.9/vsmetaEncoder/vsmetaInfo.py
--rw-rw-rw-   0        0        0      155 2021-02-03 19:02:10.000000 vsmetaEncoder-0.9/vsmetaEncoder/vsmetaListInfo.py
--rw-rw-rw-   0        0        0     1054 2021-02-28 10:26:14.000000 vsmetaEncoder-0.9/vsmetaEncoder/vsmetaMovieEncoder.py
--rw-rw-rw-   0        0        0     1448 2021-02-28 21:04:53.000000 vsmetaEncoder-0.9/vsmetaEncoder/vsmetaSeriesEncoder.py
-drwxrwxrwx   0        0        0        0 2021-03-17 07:12:29.451772 vsmetaEncoder-0.9/vsmetaEncoder.egg-info/
--rw-rw-rw-   0        0        0     6225 2021-03-17 07:12:28.000000 vsmetaEncoder-0.9/vsmetaEncoder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      458 2021-03-17 07:12:28.000000 vsmetaEncoder-0.9/vsmetaEncoder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-03-17 07:12:28.000000 vsmetaEncoder-0.9/vsmetaEncoder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-01-22 15:37:57.000000 vsmetaEncoder-0.9/vsmetaEncoder.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2021-03-17 07:12:28.000000 vsmetaEncoder-0.9/vsmetaEncoder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2021-03-17 07:12:28.000000 vsmetaEncoder-0.9/vsmetaEncoder.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-13 06:12:03.883813 vsmetaencoder-1.1.1/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35129 2024-05-13 06:03:51.000000 vsmetaencoder-1.1.1/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)    10304 2024-05-13 06:12:03.883813 vsmetaencoder-1.1.1/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9676 2024-05-13 06:06:31.000000 vsmetaencoder-1.1.1/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      704 2024-05-13 06:08:40.000000 vsmetaencoder-1.1.1/pyproject.toml
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-13 06:12:03.883813 vsmetaencoder-1.1.1/setup.cfg
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-13 06:12:03.875813 vsmetaencoder-1.1.1/src/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      885 2024-05-13 06:10:01.000000 vsmetaencoder-1.1.1/src/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-13 06:12:03.879813 vsmetaencoder-1.1.1/src/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2950 2024-05-13 06:03:51.000000 vsmetaencoder-1.1.1/src/tests/testHelpers.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2947 2024-05-13 06:03:51.000000 vsmetaencoder-1.1.1/src/tests/testVsMetaBase.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4315 2024-05-13 06:03:51.000000 vsmetaencoder-1.1.1/src/tests/testVsMetaMovieEncoder.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2323 2024-05-13 06:03:51.000000 vsmetaencoder-1.1.1/src/tests/testvsmetaDecoder.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3222 2024-05-13 06:03:51.000000 vsmetaencoder-1.1.1/src/tests/testvsmetaSeriesEncoder.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-13 06:12:03.879813 vsmetaencoder-1.1.1/src/vsmetaCodec/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      318 2024-05-13 06:03:51.000000 vsmetaencoder-1.1.1/src/vsmetaCodec/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9558 2024-05-13 06:03:51.000000 vsmetaencoder-1.1.1/src/vsmetaCodec/vsmetaBase.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5051 2024-05-13 06:03:51.000000 vsmetaencoder-1.1.1/src/vsmetaCodec/vsmetaCode.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7298 2024-05-13 06:03:51.000000 vsmetaencoder-1.1.1/src/vsmetaCodec/vsmetaDecoder.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1729 2024-05-13 06:03:51.000000 vsmetaencoder-1.1.1/src/vsmetaCodec/vsmetaEncoder.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6392 2024-05-13 06:03:51.000000 vsmetaencoder-1.1.1/src/vsmetaCodec/vsmetaInfo.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-13 06:12:03.879813 vsmetaencoder-1.1.1/src/vsmetaEncoder.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)    10304 2024-05-13 06:12:03.000000 vsmetaencoder-1.1.1/src/vsmetaEncoder.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      550 2024-05-13 06:12:03.000000 vsmetaencoder-1.1.1/src/vsmetaEncoder.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-13 06:12:03.000000 vsmetaencoder-1.1.1/src/vsmetaEncoder.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       24 2024-05-13 06:12:03.000000 vsmetaencoder-1.1.1/src/vsmetaEncoder.egg-info/top_level.txt
```

