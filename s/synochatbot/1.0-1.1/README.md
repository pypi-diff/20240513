# Comparing `tmp/synochatbot-1.0.tar.gz` & `tmp/synochatbot-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synochatbot-1.0.tar", last modified: Mon May 13 15:38:27 2024, max compression
+gzip compressed data, was "synochatbot-1.1.tar", last modified: Mon May 13 15:49:56 2024, max compression
```

## Comparing `synochatbot-1.0.tar` & `synochatbot-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 15:38:27.586420 synochatbot-1.0/
--rw-r--r--   0 ct         (502) staff       (20)      138 2024-05-13 15:38:27.586220 synochatbot-1.0/PKG-INFO
--rw-r--r--   0 ct         (502) staff       (20)       38 2024-05-13 15:38:27.586461 synochatbot-1.0/setup.cfg
--rw-r--r--   0 ct         (502) staff       (20)      239 2024-05-13 15:09:13.000000 synochatbot-1.0/setup.py
-drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 15:38:27.584826 synochatbot-1.0/synochatbot/
--rw-r--r--   0 ct         (502) staff       (20)      573 2024-05-13 04:29:50.000000 synochatbot-1.0/synochatbot/__init__.py
--rw-r--r--   0 ct         (502) staff       (20)     3372 2024-05-13 15:08:15.000000 synochatbot-1.0/synochatbot/bot.py
-drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 15:38:27.585983 synochatbot-1.0/synochatbot.egg-info/
--rw-r--r--   0 ct         (502) staff       (20)      138 2024-05-13 15:38:27.000000 synochatbot-1.0/synochatbot.egg-info/PKG-INFO
--rw-r--r--   0 ct         (502) staff       (20)      225 2024-05-13 15:38:27.000000 synochatbot-1.0/synochatbot.egg-info/SOURCES.txt
--rw-r--r--   0 ct         (502) staff       (20)        1 2024-05-13 15:38:27.000000 synochatbot-1.0/synochatbot.egg-info/dependency_links.txt
--rw-r--r--   0 ct         (502) staff       (20)       30 2024-05-13 15:38:27.000000 synochatbot-1.0/synochatbot.egg-info/requires.txt
--rw-r--r--   0 ct         (502) staff       (20)       12 2024-05-13 15:38:27.000000 synochatbot-1.0/synochatbot.egg-info/top_level.txt
+drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 15:49:56.032652 synochatbot-1.1/
+-rw-r--r--   0 ct         (502) staff       (20)     1036 2024-05-13 15:49:56.032447 synochatbot-1.1/PKG-INFO
+-rw-r--r--   0 ct         (502) staff       (20)       38 2024-05-13 15:49:56.032692 synochatbot-1.1/setup.cfg
+-rw-r--r--   0 ct         (502) staff       (20)     1185 2024-05-13 15:49:03.000000 synochatbot-1.1/setup.py
+drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 15:49:56.031329 synochatbot-1.1/synochatbot/
+-rw-r--r--   0 ct         (502) staff       (20)      573 2024-05-13 04:29:50.000000 synochatbot-1.1/synochatbot/__init__.py
+-rw-r--r--   0 ct         (502) staff       (20)     3372 2024-05-13 15:08:15.000000 synochatbot-1.1/synochatbot/bot.py
+drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 15:49:56.032221 synochatbot-1.1/synochatbot.egg-info/
+-rw-r--r--   0 ct         (502) staff       (20)     1036 2024-05-13 15:49:56.000000 synochatbot-1.1/synochatbot.egg-info/PKG-INFO
+-rw-r--r--   0 ct         (502) staff       (20)      225 2024-05-13 15:49:56.000000 synochatbot-1.1/synochatbot.egg-info/SOURCES.txt
+-rw-r--r--   0 ct         (502) staff       (20)        1 2024-05-13 15:49:56.000000 synochatbot-1.1/synochatbot.egg-info/dependency_links.txt
+-rw-r--r--   0 ct         (502) staff       (20)       30 2024-05-13 15:49:56.000000 synochatbot-1.1/synochatbot.egg-info/requires.txt
+-rw-r--r--   0 ct         (502) staff       (20)       12 2024-05-13 15:49:56.000000 synochatbot-1.1/synochatbot.egg-info/top_level.txt
```

### Comparing `synochatbot-1.0/synochatbot/__init__.py` & `synochatbot-1.1/synochatbot/__init__.py`

 * *Files identical despite different names*

### Comparing `synochatbot-1.0/synochatbot/bot.py` & `synochatbot-1.1/synochatbot/bot.py`

 * *Files identical despite different names*

