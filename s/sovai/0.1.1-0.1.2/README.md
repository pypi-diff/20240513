# Comparing `tmp/sovai-0.1.1.tar.gz` & `tmp/sovai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sovai-0.1.1.tar", last modified: Mon May 13 15:09:46 2024, max compression
+gzip compressed data, was "sovai-0.1.2.tar", last modified: Mon May 13 15:14:26 2024, max compression
```

## Comparing `sovai-0.1.1.tar` & `sovai-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 dereksnow   (501) staff       (20)        0 2024-05-13 15:09:46.896654 sovai-0.1.1/
--rw-r--r--   0 dereksnow   (501) staff       (20)      140 2024-05-13 15:09:46.896476 sovai-0.1.1/PKG-INFO
--rw-r--r--   0 dereksnow   (501) staff       (20)       17 2024-05-13 14:45:50.000000 sovai-0.1.1/README.md
--rw-r--r--   0 dereksnow   (501) staff       (20)       38 2024-05-13 15:09:46.896695 sovai-0.1.1/setup.cfg
--rw-r--r--   0 dereksnow   (501) staff       (20)      490 2024-05-13 14:49:31.000000 sovai-0.1.1/setup.py
-drwxr-xr-x   0 dereksnow   (501) staff       (20)        0 2024-05-13 15:09:46.895755 sovai-0.1.1/sovai/
--rw-r--r--   0 dereksnow   (501) staff       (20)        0 2024-05-13 14:46:44.000000 sovai-0.1.1/sovai/__init__.py
-drwxr-xr-x   0 dereksnow   (501) staff       (20)        0 2024-05-13 15:09:46.896303 sovai-0.1.1/sovai.egg-info/
--rw-r--r--   0 dereksnow   (501) staff       (20)      140 2024-05-13 15:09:46.000000 sovai-0.1.1/sovai.egg-info/PKG-INFO
--rw-r--r--   0 dereksnow   (501) staff       (20)      152 2024-05-13 15:09:46.000000 sovai-0.1.1/sovai.egg-info/SOURCES.txt
--rw-r--r--   0 dereksnow   (501) staff       (20)        1 2024-05-13 15:09:46.000000 sovai-0.1.1/sovai.egg-info/dependency_links.txt
--rw-r--r--   0 dereksnow   (501) staff       (20)        6 2024-05-13 15:09:46.000000 sovai-0.1.1/sovai.egg-info/top_level.txt
+drwxr-xr-x   0 dereksnow   (501) staff       (20)        0 2024-05-13 15:14:26.554284 sovai-0.1.2/
+-rw-r--r--   0 dereksnow   (501) staff       (20)      140 2024-05-13 15:14:26.554035 sovai-0.1.2/PKG-INFO
+-rw-r--r--   0 dereksnow   (501) staff       (20)       17 2024-05-13 14:45:50.000000 sovai-0.1.2/README.md
+-rw-r--r--   0 dereksnow   (501) staff       (20)       38 2024-05-13 15:14:26.554334 sovai-0.1.2/setup.cfg
+-rw-r--r--   0 dereksnow   (501) staff       (20)      489 2024-05-13 15:14:21.000000 sovai-0.1.2/setup.py
+drwxr-xr-x   0 dereksnow   (501) staff       (20)        0 2024-05-13 15:14:26.552946 sovai-0.1.2/sovai/
+-rw-r--r--   0 dereksnow   (501) staff       (20)        0 2024-05-13 14:46:44.000000 sovai-0.1.2/sovai/__init__.py
+drwxr-xr-x   0 dereksnow   (501) staff       (20)        0 2024-05-13 15:14:26.553629 sovai-0.1.2/sovai.egg-info/
+-rw-r--r--   0 dereksnow   (501) staff       (20)      140 2024-05-13 15:14:26.000000 sovai-0.1.2/sovai.egg-info/PKG-INFO
+-rw-r--r--   0 dereksnow   (501) staff       (20)      152 2024-05-13 15:14:26.000000 sovai-0.1.2/sovai.egg-info/SOURCES.txt
+-rw-r--r--   0 dereksnow   (501) staff       (20)        1 2024-05-13 15:14:26.000000 sovai-0.1.2/sovai.egg-info/dependency_links.txt
+-rw-r--r--   0 dereksnow   (501) staff       (20)        6 2024-05-13 15:14:26.000000 sovai-0.1.2/sovai.egg-info/top_level.txt
```

