# Comparing `tmp/idzhiblavi_pydvim-0.1.2.tar.gz` & `tmp/idzhiblavi_pydvim-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idzhiblavi_pydvim-0.1.2.tar", last modified: Mon May 13 13:18:12 2024, max compression
+gzip compressed data, was "idzhiblavi_pydvim-0.2.0.tar", last modified: Mon May 13 13:21:18 2024, max compression
```

## Comparing `idzhiblavi_pydvim-0.1.2.tar` & `idzhiblavi_pydvim-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-13 13:18:12.252110 idzhiblavi_pydvim-0.1.2/
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)     1074 2024-05-13 06:05:12.000000 idzhiblavi_pydvim-0.1.2/LICENSE
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      395 2024-05-13 13:18:12.252055 idzhiblavi_pydvim-0.1.2/PKG-INFO
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)       63 2024-05-13 06:05:43.000000 idzhiblavi_pydvim-0.1.2/README.md
-drwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-13 13:18:12.251069 idzhiblavi_pydvim-0.1.2/dvim/
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-13 06:05:12.000000 idzhiblavi_pydvim-0.1.2/dvim/__init__.py
--rwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)      858 2024-05-13 13:14:42.000000 idzhiblavi_pydvim-0.1.2/dvim/__main__.py
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)     3237 2024-05-13 13:14:31.000000 idzhiblavi_pydvim-0.1.2/dvim/runner.py
-drwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-13 13:18:12.251886 idzhiblavi_pydvim-0.1.2/idzhiblavi_pydvim.egg-info/
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      395 2024-05-13 13:18:12.000000 idzhiblavi_pydvim-0.1.2/idzhiblavi_pydvim.egg-info/PKG-INFO
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      333 2024-05-13 13:18:12.000000 idzhiblavi_pydvim-0.1.2/idzhiblavi_pydvim.egg-info/SOURCES.txt
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)        1 2024-05-13 13:18:12.000000 idzhiblavi_pydvim-0.1.2/idzhiblavi_pydvim.egg-info/dependency_links.txt
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)       54 2024-05-13 13:18:12.000000 idzhiblavi_pydvim-0.1.2/idzhiblavi_pydvim.egg-info/entry_points.txt
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)       50 2024-05-13 13:18:12.000000 idzhiblavi_pydvim-0.1.2/idzhiblavi_pydvim.egg-info/requires.txt
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)        5 2024-05-13 13:18:12.000000 idzhiblavi_pydvim-0.1.2/idzhiblavi_pydvim.egg-info/top_level.txt
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      647 2024-05-13 13:18:12.252354 idzhiblavi_pydvim-0.1.2/setup.cfg
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)       38 2024-05-13 06:05:12.000000 idzhiblavi_pydvim-0.1.2/setup.py
+drwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-13 13:21:18.360339 idzhiblavi_pydvim-0.2.0/
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)     1074 2024-05-13 06:05:12.000000 idzhiblavi_pydvim-0.2.0/LICENSE
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      300 2024-05-13 13:21:18.360281 idzhiblavi_pydvim-0.2.0/PKG-INFO
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)       63 2024-05-13 06:05:43.000000 idzhiblavi_pydvim-0.2.0/README.md
+drwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-13 13:21:18.359398 idzhiblavi_pydvim-0.2.0/dvim/
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-13 06:05:12.000000 idzhiblavi_pydvim-0.2.0/dvim/__init__.py
+-rwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)      863 2024-05-13 13:20:48.000000 idzhiblavi_pydvim-0.2.0/dvim/__main__.py
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)     3237 2024-05-13 13:14:31.000000 idzhiblavi_pydvim-0.2.0/dvim/runner.py
+drwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-13 13:21:18.360126 idzhiblavi_pydvim-0.2.0/idzhiblavi_pydvim.egg-info/
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      300 2024-05-13 13:21:18.000000 idzhiblavi_pydvim-0.2.0/idzhiblavi_pydvim.egg-info/PKG-INFO
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      293 2024-05-13 13:21:18.000000 idzhiblavi_pydvim-0.2.0/idzhiblavi_pydvim.egg-info/SOURCES.txt
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)        1 2024-05-13 13:21:18.000000 idzhiblavi_pydvim-0.2.0/idzhiblavi_pydvim.egg-info/dependency_links.txt
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)       54 2024-05-13 13:21:18.000000 idzhiblavi_pydvim-0.2.0/idzhiblavi_pydvim.egg-info/entry_points.txt
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)        5 2024-05-13 13:21:18.000000 idzhiblavi_pydvim-0.2.0/idzhiblavi_pydvim.egg-info/top_level.txt
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      588 2024-05-13 13:21:18.360602 idzhiblavi_pydvim-0.2.0/setup.cfg
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)       38 2024-05-13 06:05:12.000000 idzhiblavi_pydvim-0.2.0/setup.py
```

### Comparing `idzhiblavi_pydvim-0.1.2/LICENSE` & `idzhiblavi_pydvim-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idzhiblavi_pydvim-0.1.2/dvim/__main__.py` & `idzhiblavi_pydvim-0.2.0/dvim/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 import click
-from runner import Runner
+from dvim.runner import Runner
 
 
 @click.group()
 @click.option("--debug/--no-debug", default=False)
 @click.option("--executable", default="nvim")
 @click.option("--workspace", default=None)
 @click.option("--session", default=None)
```

### Comparing `idzhiblavi_pydvim-0.1.2/dvim/runner.py` & `idzhiblavi_pydvim-0.2.0/dvim/runner.py`

 * *Files identical despite different names*

