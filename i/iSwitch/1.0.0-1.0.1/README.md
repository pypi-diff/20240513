# Comparing `tmp/iSwitch-1.0.0.tar.gz` & `tmp/iSwitch-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iSwitch-1.0.0.tar", last modified: Mon May 13 18:33:28 2024, max compression
+gzip compressed data, was "iSwitch-1.0.1.tar", last modified: Mon May 13 18:39:53 2024, max compression
```

## Comparing `iSwitch-1.0.0.tar` & `iSwitch-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-13 18:33:28.966774 iSwitch-1.0.0/
--rw-r--r--   0 mac        (501) staff       (20)     1057 2024-05-11 18:46:44.000000 iSwitch-1.0.0/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)      310 2024-05-13 18:33:28.965952 iSwitch-1.0.0/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     4528 2024-05-13 17:13:43.000000 iSwitch-1.0.0/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-13 18:33:28.965138 iSwitch-1.0.0/iSwitch.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      310 2024-05-13 18:33:28.000000 iSwitch-1.0.0/iSwitch.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      276 2024-05-13 18:33:28.000000 iSwitch-1.0.0/iSwitch.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2024-05-13 18:33:28.000000 iSwitch-1.0.0/iSwitch.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       26 2024-05-13 18:33:28.000000 iSwitch-1.0.0/iSwitch.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        8 2024-05-13 18:33:28.000000 iSwitch-1.0.0/iSwitch.egg-info/top_level.txt
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-13 18:33:28.964453 iSwitch-1.0.0/iswitch/
--rw-r--r--   0 mac        (501) staff       (20)      328 2024-05-12 10:01:33.000000 iSwitch-1.0.0/iswitch/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     6560 2024-05-13 16:12:36.000000 iSwitch-1.0.0/iswitch/_client.py
--rw-r--r--   0 mac        (501) staff       (20)     7677 2024-05-12 22:15:34.000000 iSwitch-1.0.0/iswitch/_services.py
--rw-r--r--   0 mac        (501) staff       (20)     7360 2024-05-13 16:09:25.000000 iSwitch-1.0.0/iswitch/_types.py
--rw-r--r--   0 mac        (501) staff       (20)     3247 2024-05-12 10:42:22.000000 iSwitch-1.0.0/iswitch/_utils.py
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-05-13 18:33:28.966943 iSwitch-1.0.0/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      416 2024-05-13 18:32:54.000000 iSwitch-1.0.0/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-13 18:39:53.434595 iSwitch-1.0.1/
+-rw-r--r--   0 mac        (501) staff       (20)     1057 2024-05-11 18:46:44.000000 iSwitch-1.0.1/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)     4880 2024-05-13 18:39:53.434070 iSwitch-1.0.1/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     4528 2024-05-13 17:13:43.000000 iSwitch-1.0.1/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-13 18:39:53.433508 iSwitch-1.0.1/iSwitch.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     4880 2024-05-13 18:39:53.000000 iSwitch-1.0.1/iSwitch.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      276 2024-05-13 18:39:53.000000 iSwitch-1.0.1/iSwitch.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2024-05-13 18:39:53.000000 iSwitch-1.0.1/iSwitch.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       26 2024-05-13 18:39:53.000000 iSwitch-1.0.1/iSwitch.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        8 2024-05-13 18:39:53.000000 iSwitch-1.0.1/iSwitch.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-13 18:39:53.432675 iSwitch-1.0.1/iswitch/
+-rw-r--r--   0 mac        (501) staff       (20)      328 2024-05-12 10:01:33.000000 iSwitch-1.0.1/iswitch/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     6560 2024-05-13 16:12:36.000000 iSwitch-1.0.1/iswitch/_client.py
+-rw-r--r--   0 mac        (501) staff       (20)     7677 2024-05-12 22:15:34.000000 iSwitch-1.0.1/iswitch/_services.py
+-rw-r--r--   0 mac        (501) staff       (20)     7360 2024-05-13 16:09:25.000000 iSwitch-1.0.1/iswitch/_types.py
+-rw-r--r--   0 mac        (501) staff       (20)     3247 2024-05-12 10:42:22.000000 iSwitch-1.0.1/iswitch/_utils.py
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-05-13 18:39:53.434706 iSwitch-1.0.1/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      617 2024-05-13 18:39:45.000000 iSwitch-1.0.1/setup.py
```

### Comparing `iSwitch-1.0.0/LICENSE` & `iSwitch-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iSwitch-1.0.0/README.md` & `iSwitch-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `iSwitch-1.0.0/iswitch/_client.py` & `iSwitch-1.0.1/iswitch/_client.py`

 * *Files identical despite different names*

### Comparing `iSwitch-1.0.0/iswitch/_services.py` & `iSwitch-1.0.1/iswitch/_services.py`

 * *Files identical despite different names*

### Comparing `iSwitch-1.0.0/iswitch/_types.py` & `iSwitch-1.0.1/iswitch/_types.py`

 * *Files identical despite different names*

### Comparing `iSwitch-1.0.0/iswitch/_utils.py` & `iSwitch-1.0.1/iswitch/_utils.py`

 * *Files identical despite different names*

