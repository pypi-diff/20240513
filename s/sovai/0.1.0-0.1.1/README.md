# Comparing `tmp/sovai-0.1.0.tar.gz` & `tmp/sovai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sovai-0.1.0.tar", max compression
+gzip compressed data, was "sovai-0.1.1.tar", last modified: Mon May 13 15:09:46 2024, max compression
```

## Comparing `sovai-0.1.0.tar` & `sovai-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,12 @@
--rwxr-xr-x   0        0        0        0 2022-09-25 17:29:23.127944 sovai-0.1.0/README.md
--rwxr-xr-x   0        0        0      274 2022-09-25 18:25:14.458679 sovai-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0       46 2022-09-25 17:28:35.544161 sovai-0.1.0/src/sovai/__init__.py
--rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 sovai-0.1.0/setup.py
--rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 sovai-0.1.0/PKG-INFO
+drwxr-xr-x   0 dereksnow   (501) staff       (20)        0 2024-05-13 15:09:46.896654 sovai-0.1.1/
+-rw-r--r--   0 dereksnow   (501) staff       (20)      140 2024-05-13 15:09:46.896476 sovai-0.1.1/PKG-INFO
+-rw-r--r--   0 dereksnow   (501) staff       (20)       17 2024-05-13 14:45:50.000000 sovai-0.1.1/README.md
+-rw-r--r--   0 dereksnow   (501) staff       (20)       38 2024-05-13 15:09:46.896695 sovai-0.1.1/setup.cfg
+-rw-r--r--   0 dereksnow   (501) staff       (20)      490 2024-05-13 14:49:31.000000 sovai-0.1.1/setup.py
+drwxr-xr-x   0 dereksnow   (501) staff       (20)        0 2024-05-13 15:09:46.895755 sovai-0.1.1/sovai/
+-rw-r--r--   0 dereksnow   (501) staff       (20)        0 2024-05-13 14:46:44.000000 sovai-0.1.1/sovai/__init__.py
+drwxr-xr-x   0 dereksnow   (501) staff       (20)        0 2024-05-13 15:09:46.896303 sovai-0.1.1/sovai.egg-info/
+-rw-r--r--   0 dereksnow   (501) staff       (20)      140 2024-05-13 15:09:46.000000 sovai-0.1.1/sovai.egg-info/PKG-INFO
+-rw-r--r--   0 dereksnow   (501) staff       (20)      152 2024-05-13 15:09:46.000000 sovai-0.1.1/sovai.egg-info/SOURCES.txt
+-rw-r--r--   0 dereksnow   (501) staff       (20)        1 2024-05-13 15:09:46.000000 sovai-0.1.1/sovai.egg-info/dependency_links.txt
+-rw-r--r--   0 dereksnow   (501) staff       (20)        6 2024-05-13 15:09:46.000000 sovai-0.1.1/sovai.egg-info/top_level.txt
```

