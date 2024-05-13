# Comparing `tmp/idzhiblavi_pydvim-0.2.1.tar.gz` & `tmp/idzhiblavi_pydvim-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idzhiblavi_pydvim-0.2.1.tar", last modified: Mon May 13 13:23:23 2024, max compression
+gzip compressed data, was "idzhiblavi_pydvim-0.2.2.tar", last modified: Mon May 13 13:32:06 2024, max compression
```

## Comparing `idzhiblavi_pydvim-0.2.1.tar` & `idzhiblavi_pydvim-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-13 13:23:23.138434 idzhiblavi_pydvim-0.2.1/
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)     1074 2024-05-13 06:05:12.000000 idzhiblavi_pydvim-0.2.1/LICENSE
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      300 2024-05-13 13:23:23.138376 idzhiblavi_pydvim-0.2.1/PKG-INFO
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)       63 2024-05-13 06:05:43.000000 idzhiblavi_pydvim-0.2.1/README.md
-drwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-13 13:23:23.137408 idzhiblavi_pydvim-0.2.1/dvim/
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-13 06:05:12.000000 idzhiblavi_pydvim-0.2.1/dvim/__init__.py
--rwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)      863 2024-05-13 13:20:48.000000 idzhiblavi_pydvim-0.2.1/dvim/__main__.py
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)     3237 2024-05-13 13:14:31.000000 idzhiblavi_pydvim-0.2.1/dvim/runner.py
-drwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-13 13:23:23.138203 idzhiblavi_pydvim-0.2.1/idzhiblavi_pydvim.egg-info/
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      300 2024-05-13 13:23:23.000000 idzhiblavi_pydvim-0.2.1/idzhiblavi_pydvim.egg-info/PKG-INFO
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      293 2024-05-13 13:23:23.000000 idzhiblavi_pydvim-0.2.1/idzhiblavi_pydvim.egg-info/SOURCES.txt
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)        1 2024-05-13 13:23:23.000000 idzhiblavi_pydvim-0.2.1/idzhiblavi_pydvim.egg-info/dependency_links.txt
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)       55 2024-05-13 13:23:23.000000 idzhiblavi_pydvim-0.2.1/idzhiblavi_pydvim.egg-info/entry_points.txt
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)        5 2024-05-13 13:23:23.000000 idzhiblavi_pydvim-0.2.1/idzhiblavi_pydvim.egg-info/top_level.txt
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      589 2024-05-13 13:23:23.138692 idzhiblavi_pydvim-0.2.1/setup.cfg
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)       38 2024-05-13 06:05:12.000000 idzhiblavi_pydvim-0.2.1/setup.py
+drwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-13 13:32:06.691355 idzhiblavi_pydvim-0.2.2/
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)     1074 2024-05-13 06:05:12.000000 idzhiblavi_pydvim-0.2.2/LICENSE
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      300 2024-05-13 13:32:06.691286 idzhiblavi_pydvim-0.2.2/PKG-INFO
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)       63 2024-05-13 06:05:43.000000 idzhiblavi_pydvim-0.2.2/README.md
+drwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-13 13:32:06.690253 idzhiblavi_pydvim-0.2.2/dvim/
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-13 06:05:12.000000 idzhiblavi_pydvim-0.2.2/dvim/__init__.py
+-rwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)      863 2024-05-13 13:20:48.000000 idzhiblavi_pydvim-0.2.2/dvim/__main__.py
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)     3261 2024-05-13 13:31:41.000000 idzhiblavi_pydvim-0.2.2/dvim/runner.py
+drwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-13 13:32:06.691044 idzhiblavi_pydvim-0.2.2/idzhiblavi_pydvim.egg-info/
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      300 2024-05-13 13:32:06.000000 idzhiblavi_pydvim-0.2.2/idzhiblavi_pydvim.egg-info/PKG-INFO
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      293 2024-05-13 13:32:06.000000 idzhiblavi_pydvim-0.2.2/idzhiblavi_pydvim.egg-info/SOURCES.txt
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)        1 2024-05-13 13:32:06.000000 idzhiblavi_pydvim-0.2.2/idzhiblavi_pydvim.egg-info/dependency_links.txt
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)       55 2024-05-13 13:32:06.000000 idzhiblavi_pydvim-0.2.2/idzhiblavi_pydvim.egg-info/entry_points.txt
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)        5 2024-05-13 13:32:06.000000 idzhiblavi_pydvim-0.2.2/idzhiblavi_pydvim.egg-info/top_level.txt
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      589 2024-05-13 13:32:06.691628 idzhiblavi_pydvim-0.2.2/setup.cfg
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)       38 2024-05-13 06:05:12.000000 idzhiblavi_pydvim-0.2.2/setup.py
```

### Comparing `idzhiblavi_pydvim-0.2.1/LICENSE` & `idzhiblavi_pydvim-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `idzhiblavi_pydvim-0.2.1/dvim/__main__.py` & `idzhiblavi_pydvim-0.2.2/dvim/__main__.py`

 * *Files identical despite different names*

### Comparing `idzhiblavi_pydvim-0.2.1/dvim/runner.py` & `idzhiblavi_pydvim-0.2.2/dvim/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,16 @@
         os.remove(socket_path)
 
 
 def run(cmd, extra_env, debug):
     if debug:
         print(extra_env, cmd)
     else:
-        subprocess.run(cmd, env=dict(os.environ) | extra_env)
+        extra_env.update(dict(os.environ))
+        subprocess.run(cmd, env=extra_env)
 
 
 def find_running_instance_socket_path(socket_prefix):
     print(f"prefix: {socket_prefix}")
     sockets = [
         os.path.join(SOCKETS_DIR, path)
         for path in os.listdir(SOCKETS_DIR)
```

### Comparing `idzhiblavi_pydvim-0.2.1/setup.cfg` & `idzhiblavi_pydvim-0.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = idzhiblavi_pydvim
-version = 0.2.1
+version = 0.2.2
 license_files = LICENSE
 author = Ibragim Dzhiblavi
 author_email = dzhiblavi@gmail.com
 description = Lightweight neovim wrapper
 long_description = file:README.md
 project_urls = 
 	Source = https://github.com/dzhiblavi/pydvim
```

