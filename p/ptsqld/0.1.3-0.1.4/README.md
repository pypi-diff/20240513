# Comparing `tmp/ptsqld-0.1.3.tar.gz` & `tmp/ptsqld-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptsqld-0.1.3.tar", max compression
+gzip compressed data, was "ptsqld-0.1.4.tar", max compression
```

## Comparing `ptsqld-0.1.3.tar` & `ptsqld-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,10 @@
--rw-r--r--   0        0        0      810 2024-04-26 05:49:16.395339 ptsqld-0.1.3/README.md
--rw-r--r--   0        0        0     7281 2024-05-11 19:44:00.963863 ptsqld-0.1.3/ptsqld/__init__.py
--rw-r--r--   0        0        0     1462 2024-03-12 09:17:42.025413 ptsqld-0.1.3/ptsqld/__init__.py~
--rw-r--r--   0        0        0      487 2024-03-13 20:19:06.329725 ptsqld-0.1.3/ptsqld/__main__.py~
--rw-r--r--   0        0        0      488 2024-05-11 19:47:19.018537 ptsqld-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1354 1970-01-01 00:00:00.000000 ptsqld-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      810 2024-04-26 05:49:16.395339 ptsqld-0.1.4/README.md
+-rw-r--r--   0        0        0     3212 2024-05-13 19:09:31.555950 ptsqld-0.1.4/ptsqld/__init__.py
+-rw-r--r--   0        0        0     1462 2024-03-12 09:17:42.025413 ptsqld-0.1.4/ptsqld/__init__.py~
+-rw-r--r--   0        0        0      487 2024-03-13 20:19:06.329725 ptsqld-0.1.4/ptsqld/__main__.py~
+-rw-r--r--   0        0        0      663 2024-05-13 19:10:01.542954 ptsqld-0.1.4/ptsqld/structured_engine.py
+-rw-r--r--   0        0        0      625 2024-05-13 19:02:02.734253 ptsqld-0.1.4/ptsqld/structured_engine.py~
+-rw-r--r--   0        0        0     3263 2024-05-13 19:02:12.891033 ptsqld-0.1.4/ptsqld/structured_vault.py
+-rw-r--r--   0        0        0     3263 2024-05-13 19:01:01.096900 ptsqld-0.1.4/ptsqld/structuredvault.py~
+-rw-r--r--   0        0        0      488 2024-05-13 20:03:02.372428 ptsqld-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1354 1970-01-01 00:00:00.000000 ptsqld-0.1.4/PKG-INFO
```

### Comparing `ptsqld-0.1.3/README.md` & `ptsqld-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ptsqld-0.1.3/ptsqld/__init__.py~` & `ptsqld-0.1.4/ptsqld/__init__.py~`

 * *Files identical despite different names*

### Comparing `ptsqld-0.1.3/PKG-INFO` & `ptsqld-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptsqld
-Version: 0.1.3
+Version: 0.1.4
 Summary: An SQL Database which shall avoid any further PTSD associated to other SQL Database setup (understand flexible, simple)
 Author: Charles Bajeux
 Author-email: charles.bajeux@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

