# Comparing `tmp/hd2_macros-1.2.0.tar.gz` & `tmp/hd2_macros-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hd2_macros-1.2.0.tar", last modified: Fri Apr  5 08:07:44 2024, max compression
+gzip compressed data, was "hd2_macros-1.2.1.tar", last modified: Mon May 13 03:30:30 2024, max compression
```

## Comparing `hd2_macros-1.2.0.tar` & `hd2_macros-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 08:07:44.201389 hd2_macros-1.2.0/
--rw-rw-rw-   0        0        0     1099 2024-04-05 08:07:19.000000 hd2_macros-1.2.0/LICENSE
--rw-rw-rw-   0        0        0       91 2024-04-05 08:07:19.000000 hd2_macros-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6058 2024-04-05 08:07:44.201389 hd2_macros-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4972 2024-04-05 08:07:19.000000 hd2_macros-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 08:07:44.201389 hd2_macros-1.2.0/hd2_macros/
--rw-rw-rw-   0        0        0       23 2024-04-05 08:07:19.000000 hd2_macros-1.2.0/hd2_macros/__init__.py
--rw-rw-rw-   0        0        0       95 2024-04-05 08:07:19.000000 hd2_macros-1.2.0/hd2_macros/__main__.py
--rw-rw-rw-   0        0        0     2569 2024-04-05 08:07:19.000000 hd2_macros-1.2.0/hd2_macros/config.py
--rw-rw-rw-   0        0        0     1967 2024-04-05 08:07:19.000000 hd2_macros-1.2.0/hd2_macros/config.toml
--rw-rw-rw-   0        0        0     5355 2024-04-05 08:07:19.000000 hd2_macros-1.2.0/hd2_macros/constants.py
--rw-rw-rw-   0        0        0     6472 2024-04-05 08:07:19.000000 hd2_macros-1.2.0/hd2_macros/macro.py
--rw-rw-rw-   0        0        0        0 2024-04-05 08:07:19.000000 hd2_macros-1.2.0/hd2_macros/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-05 08:07:44.201389 hd2_macros-1.2.0/hd2_macros.egg-info/
--rw-rw-rw-   0        0        0     6058 2024-04-05 08:07:44.000000 hd2_macros-1.2.0/hd2_macros.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2024-04-05 08:07:44.000000 hd2_macros-1.2.0/hd2_macros.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 08:07:44.000000 hd2_macros-1.2.0/hd2_macros.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-04-05 08:07:44.000000 hd2_macros-1.2.0/hd2_macros.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-05 08:07:44.000000 hd2_macros-1.2.0/hd2_macros.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       48 2024-04-05 08:07:19.000000 hd2_macros-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0     1186 2024-04-05 08:07:44.201389 hd2_macros-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 03:30:30.027908 hd2_macros-1.2.1/
+-rw-rw-rw-   0        0        0     1099 2024-05-13 03:29:57.000000 hd2_macros-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0       91 2024-05-13 03:29:57.000000 hd2_macros-1.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6058 2024-05-13 03:30:30.027908 hd2_macros-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4972 2024-05-13 03:29:57.000000 hd2_macros-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 03:30:30.027908 hd2_macros-1.2.1/hd2_macros/
+-rw-rw-rw-   0        0        0       23 2024-05-13 03:29:57.000000 hd2_macros-1.2.1/hd2_macros/__init__.py
+-rw-rw-rw-   0        0        0       95 2024-05-13 03:29:57.000000 hd2_macros-1.2.1/hd2_macros/__main__.py
+-rw-rw-rw-   0        0        0     2569 2024-05-13 03:29:57.000000 hd2_macros-1.2.1/hd2_macros/config.py
+-rw-rw-rw-   0        0        0     1967 2024-05-13 03:29:57.000000 hd2_macros-1.2.1/hd2_macros/config.toml
+-rw-rw-rw-   0        0        0     5364 2024-05-13 03:29:57.000000 hd2_macros-1.2.1/hd2_macros/constants.py
+-rw-rw-rw-   0        0        0     6472 2024-05-13 03:29:57.000000 hd2_macros-1.2.1/hd2_macros/macro.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 03:29:57.000000 hd2_macros-1.2.1/hd2_macros/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-13 03:30:30.027908 hd2_macros-1.2.1/hd2_macros.egg-info/
+-rw-rw-rw-   0        0        0     6058 2024-05-13 03:30:30.000000 hd2_macros-1.2.1/hd2_macros.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2024-05-13 03:30:30.000000 hd2_macros-1.2.1/hd2_macros.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 03:30:30.000000 hd2_macros-1.2.1/hd2_macros.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-13 03:30:30.000000 hd2_macros-1.2.1/hd2_macros.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-13 03:30:30.000000 hd2_macros-1.2.1/hd2_macros.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       48 2024-05-13 03:29:57.000000 hd2_macros-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1186 2024-05-13 03:30:30.027908 hd2_macros-1.2.1/setup.cfg
```

### Comparing `hd2_macros-1.2.0/LICENSE` & `hd2_macros-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hd2_macros-1.2.0/PKG-INFO` & `hd2_macros-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hd2_macros
-Version: 1.2.0
+Version: 1.2.1
 Summary: Helldivers 2 macros
 Home-page: https://github.com/spyoungtech/helldivers2-macros
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Project-URL: Documentation, https://github.com/spyoungtech/helldivers2-macros
 Project-URL: Source, https://github.com/spyoungtech/helldivers2-macros
 Project-URL: Tracker, https://github.com/spyoungtech/helldivers2-macros/issues
```

### Comparing `hd2_macros-1.2.0/README.md` & `hd2_macros-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `hd2_macros-1.2.0/hd2_macros/config.py` & `hd2_macros-1.2.1/hd2_macros/config.py`

 * *Files identical despite different names*

### Comparing `hd2_macros-1.2.0/hd2_macros/config.toml` & `hd2_macros-1.2.1/hd2_macros/config.toml`

 * *Files identical despite different names*

### Comparing `hd2_macros-1.2.0/hd2_macros/constants.py` & `hd2_macros-1.2.1/hd2_macros/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,14 @@
     'anti-personnel minefield': ['Down', 'Left', 'Up', 'Right'],
     'supply pack': ['Down', 'Left', 'Down', 'Up', 'Up', 'Down'],
     'grenade launcher': ['Down', 'Left', 'Up', 'Left', 'Down'],
     'quasar cannon': ['Down', 'Down', 'Up', 'Left', 'Right'],
     'laser cannon': ['Down', 'Left', 'Down', 'Up', 'Left'],
     'incendiary mines': ['Down', 'Left', 'Left', 'Down'],
     'guard dog rover': ['Down', 'Up', 'Left', 'Up', 'Right', 'Right'],
-    'ballistic shield backpack': ['Down', 'Left', 'Up', 'Up', 'Right'],
+    'ballistic shield backpack': ['Down', 'Left', 'Down', 'Down', 'Up', 'Left'],
     'arc thrower': ['Down', 'Right', 'Down', 'Up', 'Left', 'Left'],
     'shield generator pack': ['Down', 'Up', 'Left', 'Right', 'Left', 'Right'],
     'patriot exosuit': ['Left', 'Down', 'Right', 'Up', 'Left', 'Down', 'Down'],
 }
 
 INPUT_MAPPING: Final[dict[str, str]] = {'Down': 'S', 'Up': 'W', 'Left': 'A', 'Right': 'D'}
```

### Comparing `hd2_macros-1.2.0/hd2_macros/macro.py` & `hd2_macros-1.2.1/hd2_macros/macro.py`

 * *Files identical despite different names*

### Comparing `hd2_macros-1.2.0/hd2_macros.egg-info/PKG-INFO` & `hd2_macros-1.2.1/hd2_macros.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hd2_macros
-Version: 1.2.0
+Version: 1.2.1
 Summary: Helldivers 2 macros
 Home-page: https://github.com/spyoungtech/helldivers2-macros
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Project-URL: Documentation, https://github.com/spyoungtech/helldivers2-macros
 Project-URL: Source, https://github.com/spyoungtech/helldivers2-macros
 Project-URL: Tracker, https://github.com/spyoungtech/helldivers2-macros/issues
```

### Comparing `hd2_macros-1.2.0/setup.cfg` & `hd2_macros-1.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2068 6432 5f6d 6163 726f 730d 0a76   = hd2_macros..v
-00000020: 6572 7369 6f6e 203d 2031 2e32 2e30 0d0a  ersion = 1.2.0..
+00000020: 6572 7369 6f6e 203d 2031 2e32 2e31 0d0a  ersion = 1.2.1..
 00000030: 6175 7468 6f72 5f65 6d61 696c 203d 2073  author_email = s
 00000040: 7065 6e63 6572 2e79 6f75 6e67 4073 7079  pencer.young@spy
 00000050: 6f75 6e67 2e63 6f6d 0d0a 6175 7468 6f72  oung.com..author
 00000060: 203d 2053 7065 6e63 6572 2059 6f75 6e67   = Spencer Young
 00000070: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000080: 4865 6c6c 6469 7665 7273 2032 206d 6163  Helldivers 2 mac
 00000090: 726f 730d 0a6c 6f6e 675f 6465 7363 7269  ros..long_descri
```

