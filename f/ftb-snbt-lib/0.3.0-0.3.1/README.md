# Comparing `tmp/ftb_snbt_lib-0.3.0.tar.gz` & `tmp/ftb_snbt_lib-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftb_snbt_lib-0.3.0.tar", last modified: Sun May 12 09:44:06 2024, max compression
+gzip compressed data, was "ftb_snbt_lib-0.3.1.tar", last modified: Mon May 13 10:21:50 2024, max compression
```

## Comparing `ftb_snbt_lib-0.3.0.tar` & `ftb_snbt_lib-0.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:44:06.081214 ftb_snbt_lib-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-12 09:44:06.081214 ftb_snbt_lib-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:44:06.077214 ftb_snbt_lib-0.3.0/ftb_snbt_lib/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib/parsetab.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:44:06.081214 ftb_snbt_lib-0.3.0/ftb_snbt_lib/ply/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib/ply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33639 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib/ply/cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib/ply/ctokens.py
--rw-r--r--   0 runner    (1001) docker     (127)    42905 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib/ply/lex.py
--rw-r--r--   0 runner    (1001) docker     (127)   137736 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib/ply/yacc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib/ply/ygen.py
--rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib/write.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:44:06.081214 ftb_snbt_lib-0.3.0/ftb_snbt_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-12 09:44:06.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-12 09:44:06.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 09:44:06.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-12 09:44:06.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-12 09:44:06.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 09:44:06.081214 ftb_snbt_lib-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:21:50.315832 ftb_snbt_lib-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-13 10:21:45.000000 ftb_snbt_lib-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-13 10:21:50.315832 ftb_snbt_lib-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-13 10:21:45.000000 ftb_snbt_lib-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:21:50.311832 ftb_snbt_lib-0.3.1/ftb_snbt_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-13 10:21:45.000000 ftb_snbt_lib-0.3.1/ftb_snbt_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-13 10:21:45.000000 ftb_snbt_lib-0.3.1/ftb_snbt_lib/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-05-13 10:21:45.000000 ftb_snbt_lib-0.3.1/ftb_snbt_lib/parsetab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:21:50.315832 ftb_snbt_lib-0.3.1/ftb_snbt_lib/ply/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-13 10:21:45.000000 ftb_snbt_lib-0.3.1/ftb_snbt_lib/ply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33639 2024-05-13 10:21:45.000000 ftb_snbt_lib-0.3.1/ftb_snbt_lib/ply/cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-13 10:21:45.000000 ftb_snbt_lib-0.3.1/ftb_snbt_lib/ply/ctokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42905 2024-05-13 10:21:45.000000 ftb_snbt_lib-0.3.1/ftb_snbt_lib/ply/lex.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137736 2024-05-13 10:21:45.000000 ftb_snbt_lib-0.3.1/ftb_snbt_lib/ply/yacc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-13 10:21:45.000000 ftb_snbt_lib-0.3.1/ftb_snbt_lib/ply/ygen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-05-13 10:21:45.000000 ftb_snbt_lib-0.3.1/ftb_snbt_lib/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-13 10:21:45.000000 ftb_snbt_lib-0.3.1/ftb_snbt_lib/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-05-13 10:21:45.000000 ftb_snbt_lib-0.3.1/ftb_snbt_lib/write.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:21:50.315832 ftb_snbt_lib-0.3.1/ftb_snbt_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-13 10:21:50.000000 ftb_snbt_lib-0.3.1/ftb_snbt_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-13 10:21:50.000000 ftb_snbt_lib-0.3.1/ftb_snbt_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 10:21:50.000000 ftb_snbt_lib-0.3.1/ftb_snbt_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 10:21:50.000000 ftb_snbt_lib-0.3.1/ftb_snbt_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 10:21:50.000000 ftb_snbt_lib-0.3.1/ftb_snbt_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-13 10:21:45.000000 ftb_snbt_lib-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 10:21:50.315832 ftb_snbt_lib-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-13 10:21:45.000000 ftb_snbt_lib-0.3.1/setup.py
```

### Comparing `ftb_snbt_lib-0.3.0/LICENSE` & `ftb_snbt_lib-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ftb_snbt_lib-0.3.0/PKG-INFO` & `ftb_snbt_lib-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftb-snbt-lib
-Version: 0.3.0
+Version: 0.3.1
 Summary: A python library to parse, edit, and save FTB snbt tag, which is a variant of the "vanilla" snbt tag.
 Author-email: peunsu <peunsu55@gmail.com>
 Project-URL: homepage, https://github.com/peunsu/ftb-snbt-lib
 Project-URL: repository, https://github.com/peunsu/ftb-snbt-lib
 Project-URL: documentation, https://github.com/peunsu/ftb-snbt-lib
 Keywords: minecraft,ftb,snbt,parser,library
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ftb_snbt_lib-0.3.0/README.md` & `ftb_snbt_lib-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ftb_snbt_lib-0.3.0/ftb_snbt_lib/parse.py` & `ftb_snbt_lib-0.3.1/ftb_snbt_lib/parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         p[0] = List()
     else:
         p[0] = List(p[2])
 
 def p_array(p):
     """array : LBRACKET TYPE SEMICOLON values RBRACKET
                 | LBRACKET TYPE SEMICOLON RBRACKET"""
-    if len(p) == 4:
+    if len(p) == 5:
         p[0] = Array(p[2], [])
     else:
         p[0] = Array(p[2], p[4])
 
 def p_values(p):
     """values : values value
               | values COMMA value
```

### Comparing `ftb_snbt_lib-0.3.0/ftb_snbt_lib/parsetab.py` & `ftb_snbt_lib-0.3.1/ftb_snbt_lib/parsetab.py`

 * *Files identical despite different names*

### Comparing `ftb_snbt_lib-0.3.0/ftb_snbt_lib/ply/cpp.py` & `ftb_snbt_lib-0.3.1/ftb_snbt_lib/ply/cpp.py`

 * *Files identical despite different names*

### Comparing `ftb_snbt_lib-0.3.0/ftb_snbt_lib/ply/ctokens.py` & `ftb_snbt_lib-0.3.1/ftb_snbt_lib/ply/ctokens.py`

 * *Files identical despite different names*

### Comparing `ftb_snbt_lib-0.3.0/ftb_snbt_lib/ply/lex.py` & `ftb_snbt_lib-0.3.1/ftb_snbt_lib/ply/lex.py`

 * *Files identical despite different names*

### Comparing `ftb_snbt_lib-0.3.0/ftb_snbt_lib/ply/yacc.py` & `ftb_snbt_lib-0.3.1/ftb_snbt_lib/ply/yacc.py`

 * *Files identical despite different names*

### Comparing `ftb_snbt_lib-0.3.0/ftb_snbt_lib/ply/ygen.py` & `ftb_snbt_lib-0.3.1/ftb_snbt_lib/ply/ygen.py`

 * *Files identical despite different names*

### Comparing `ftb_snbt_lib-0.3.0/ftb_snbt_lib/tag.py` & `ftb_snbt_lib-0.3.1/ftb_snbt_lib/tag.py`

 * *Files identical despite different names*

### Comparing `ftb_snbt_lib-0.3.0/ftb_snbt_lib/token.py` & `ftb_snbt_lib-0.3.1/ftb_snbt_lib/token.py`

 * *Files identical despite different names*

### Comparing `ftb_snbt_lib-0.3.0/ftb_snbt_lib/write.py` & `ftb_snbt_lib-0.3.1/ftb_snbt_lib/write.py`

 * *Files identical despite different names*

### Comparing `ftb_snbt_lib-0.3.0/ftb_snbt_lib.egg-info/PKG-INFO` & `ftb_snbt_lib-0.3.1/ftb_snbt_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftb-snbt-lib
-Version: 0.3.0
+Version: 0.3.1
 Summary: A python library to parse, edit, and save FTB snbt tag, which is a variant of the "vanilla" snbt tag.
 Author-email: peunsu <peunsu55@gmail.com>
 Project-URL: homepage, https://github.com/peunsu/ftb-snbt-lib
 Project-URL: repository, https://github.com/peunsu/ftb-snbt-lib
 Project-URL: documentation, https://github.com/peunsu/ftb-snbt-lib
 Keywords: minecraft,ftb,snbt,parser,library
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ftb_snbt_lib-0.3.0/pyproject.toml` & `ftb_snbt_lib-0.3.1/pyproject.toml`

 * *Files identical despite different names*

