# Comparing `tmp/idzhiblavi_pydvim-0.2.0.tar.gz` & `tmp/idzhiblavi_pydvim-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idzhiblavi_pydvim-0.2.0.tar", last modified: Mon May 13 13:21:18 2024, max compression
+gzip compressed data, was "idzhiblavi_pydvim-0.2.1.tar", last modified: Mon May 13 13:23:23 2024, max compression
```

## Comparing `idzhiblavi_pydvim-0.2.0.tar` & `idzhiblavi_pydvim-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-13 13:21:18.360339 idzhiblavi_pydvim-0.2.0/
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)     1074 2024-05-13 06:05:12.000000 idzhiblavi_pydvim-0.2.0/LICENSE
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      300 2024-05-13 13:21:18.360281 idzhiblavi_pydvim-0.2.0/PKG-INFO
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)       63 2024-05-13 06:05:43.000000 idzhiblavi_pydvim-0.2.0/README.md
-drwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-13 13:21:18.359398 idzhiblavi_pydvim-0.2.0/dvim/
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-13 06:05:12.000000 idzhiblavi_pydvim-0.2.0/dvim/__init__.py
--rwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)      863 2024-05-13 13:20:48.000000 idzhiblavi_pydvim-0.2.0/dvim/__main__.py
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)     3237 2024-05-13 13:14:31.000000 idzhiblavi_pydvim-0.2.0/dvim/runner.py
-drwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-13 13:21:18.360126 idzhiblavi_pydvim-0.2.0/idzhiblavi_pydvim.egg-info/
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      300 2024-05-13 13:21:18.000000 idzhiblavi_pydvim-0.2.0/idzhiblavi_pydvim.egg-info/PKG-INFO
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      293 2024-05-13 13:21:18.000000 idzhiblavi_pydvim-0.2.0/idzhiblavi_pydvim.egg-info/SOURCES.txt
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)        1 2024-05-13 13:21:18.000000 idzhiblavi_pydvim-0.2.0/idzhiblavi_pydvim.egg-info/dependency_links.txt
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)       54 2024-05-13 13:21:18.000000 idzhiblavi_pydvim-0.2.0/idzhiblavi_pydvim.egg-info/entry_points.txt
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)        5 2024-05-13 13:21:18.000000 idzhiblavi_pydvim-0.2.0/idzhiblavi_pydvim.egg-info/top_level.txt
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      588 2024-05-13 13:21:18.360602 idzhiblavi_pydvim-0.2.0/setup.cfg
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)       38 2024-05-13 06:05:12.000000 idzhiblavi_pydvim-0.2.0/setup.py
+drwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-13 13:23:23.138434 idzhiblavi_pydvim-0.2.1/
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)     1074 2024-05-13 06:05:12.000000 idzhiblavi_pydvim-0.2.1/LICENSE
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      300 2024-05-13 13:23:23.138376 idzhiblavi_pydvim-0.2.1/PKG-INFO
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)       63 2024-05-13 06:05:43.000000 idzhiblavi_pydvim-0.2.1/README.md
+drwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-13 13:23:23.137408 idzhiblavi_pydvim-0.2.1/dvim/
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-13 06:05:12.000000 idzhiblavi_pydvim-0.2.1/dvim/__init__.py
+-rwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)      863 2024-05-13 13:20:48.000000 idzhiblavi_pydvim-0.2.1/dvim/__main__.py
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)     3237 2024-05-13 13:14:31.000000 idzhiblavi_pydvim-0.2.1/dvim/runner.py
+drwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-13 13:23:23.138203 idzhiblavi_pydvim-0.2.1/idzhiblavi_pydvim.egg-info/
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      300 2024-05-13 13:23:23.000000 idzhiblavi_pydvim-0.2.1/idzhiblavi_pydvim.egg-info/PKG-INFO
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      293 2024-05-13 13:23:23.000000 idzhiblavi_pydvim-0.2.1/idzhiblavi_pydvim.egg-info/SOURCES.txt
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)        1 2024-05-13 13:23:23.000000 idzhiblavi_pydvim-0.2.1/idzhiblavi_pydvim.egg-info/dependency_links.txt
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)       55 2024-05-13 13:23:23.000000 idzhiblavi_pydvim-0.2.1/idzhiblavi_pydvim.egg-info/entry_points.txt
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)        5 2024-05-13 13:23:23.000000 idzhiblavi_pydvim-0.2.1/idzhiblavi_pydvim.egg-info/top_level.txt
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      589 2024-05-13 13:23:23.138692 idzhiblavi_pydvim-0.2.1/setup.cfg
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)       38 2024-05-13 06:05:12.000000 idzhiblavi_pydvim-0.2.1/setup.py
```

### Comparing `idzhiblavi_pydvim-0.2.0/LICENSE` & `idzhiblavi_pydvim-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `idzhiblavi_pydvim-0.2.0/dvim/__main__.py` & `idzhiblavi_pydvim-0.2.1/dvim/__main__.py`

 * *Files identical despite different names*

### Comparing `idzhiblavi_pydvim-0.2.0/dvim/runner.py` & `idzhiblavi_pydvim-0.2.1/dvim/runner.py`

 * *Files identical despite different names*

### Comparing `idzhiblavi_pydvim-0.2.0/setup.cfg` & `idzhiblavi_pydvim-0.2.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = idzhiblavi_pydvim
-version = 0.2.0
+version = 0.2.1
 license_files = LICENSE
 author = Ibragim Dzhiblavi
 author_email = dzhiblavi@gmail.com
 description = Lightweight neovim wrapper
 long_description = file:README.md
 project_urls = 
 	Source = https://github.com/dzhiblavi/pydvim
@@ -12,15 +12,15 @@
 [options]
 packages = 
 	dvim
 install_requires = 
 
 [options.entry_points]
 console_scripts = 
-	dvim = dvim.__main__:cli_entrypoint
+	pdvim = dvim.__main__:cli_entrypoint
 
 [flake8]
 max-line-length = 100
 max-complexity = 10
 
 [pycodestyle]
 max-line-length = 100
```

