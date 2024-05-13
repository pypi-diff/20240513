# Comparing `tmp/movoid_function-1.5.4.tar.gz` & `tmp/movoid_function-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movoid_function-1.5.4.tar", last modified: Thu May  9 13:03:24 2024, max compression
+gzip compressed data, was "movoid_function-1.5.5.tar", last modified: Mon May 13 01:26:46 2024, max compression
```

## Comparing `movoid_function-1.5.4.tar` & `movoid_function-1.5.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 13:03:24.887946 movoid_function-1.5.4/
--rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_function-1.5.4/MANIFEST.in
--rw-rw-rw-   0        0        0      229 2024-05-09 13:03:24.886948 movoid_function-1.5.4/PKG-INFO
--rw-rw-rw-   0        0        0       60 2024-05-09 13:01:35.000000 movoid_function-1.5.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 13:03:24.873518 movoid_function-1.5.4/movoid_function/
--rw-rw-rw-   0        0        0      562 2024-04-13 09:15:08.000000 movoid_function-1.5.4/movoid_function/__init__.py
--rw-rw-rw-   0        0        0     9920 2024-05-08 14:50:45.000000 movoid_function-1.5.4/movoid_function/check.py
--rw-rw-rw-   0        0        0    16565 2024-02-20 11:49:02.000000 movoid_function-1.5.4/movoid_function/decorator.py
--rw-rw-rw-   0        0        0     1557 2024-04-14 08:03:48.000000 movoid_function-1.5.4/movoid_function/function.py
--rw-rw-rw-   0        0        0    16151 2024-05-09 13:01:35.000000 movoid_function-1.5.4/movoid_function/type.py
-drwxrwxrwx   0        0        0        0 2024-05-09 13:03:24.884831 movoid_function-1.5.4/movoid_function.egg-info/
--rw-rw-rw-   0        0        0      229 2024-05-09 13:03:24.000000 movoid_function-1.5.4/movoid_function.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2024-05-09 13:03:24.000000 movoid_function-1.5.4/movoid_function.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 13:03:24.000000 movoid_function-1.5.4/movoid_function.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-09 13:03:24.000000 movoid_function-1.5.4/movoid_function.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 13:03:24.889021 movoid_function-1.5.4/setup.cfg
--rw-rw-rw-   0        0        0      462 2024-05-09 13:02:55.000000 movoid_function-1.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 01:26:46.275056 movoid_function-1.5.5/
+-rw-rw-rw-   0        0        0       10 2024-05-08 05:39:36.000000 movoid_function-1.5.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      229 2024-05-13 01:26:46.273063 movoid_function-1.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2024-05-08 09:59:50.000000 movoid_function-1.5.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 01:26:46.244161 movoid_function-1.5.5/movoid_function/
+-rw-rw-rw-   0        0        0      562 2024-05-07 03:06:54.000000 movoid_function-1.5.5/movoid_function/__init__.py
+-rw-rw-rw-   0        0        0     9920 2024-05-08 07:30:51.000000 movoid_function-1.5.5/movoid_function/check.py
+-rw-rw-rw-   0        0        0    16565 2024-05-07 06:16:33.000000 movoid_function-1.5.5/movoid_function/decorator.py
+-rw-rw-rw-   0        0        0     1557 2024-05-07 03:06:54.000000 movoid_function-1.5.5/movoid_function/function.py
+-rw-rw-rw-   0        0        0    16159 2024-05-10 02:50:32.000000 movoid_function-1.5.5/movoid_function/type.py
+drwxrwxrwx   0        0        0        0 2024-05-13 01:26:46.261103 movoid_function-1.5.5/movoid_function.egg-info/
+-rw-rw-rw-   0        0        0      229 2024-05-13 01:26:46.000000 movoid_function-1.5.5/movoid_function.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-05-13 01:26:46.000000 movoid_function-1.5.5/movoid_function.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 01:26:46.000000 movoid_function-1.5.5/movoid_function.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-05-13 01:26:46.000000 movoid_function-1.5.5/movoid_function.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 01:26:46.276053 movoid_function-1.5.5/setup.cfg
+-rw-rw-rw-   0        0        0      462 2024-05-10 21:33:09.000000 movoid_function-1.5.5/setup.py
```

### Comparing `movoid_function-1.5.4/movoid_function/__init__.py` & `movoid_function-1.5.5/movoid_function/__init__.py`

 * *Files identical despite different names*

### Comparing `movoid_function-1.5.4/movoid_function/check.py` & `movoid_function-1.5.5/movoid_function/check.py`

 * *Files identical despite different names*

### Comparing `movoid_function-1.5.4/movoid_function/decorator.py` & `movoid_function-1.5.5/movoid_function/decorator.py`

 * *Files identical despite different names*

### Comparing `movoid_function-1.5.4/movoid_function/function.py` & `movoid_function-1.5.5/movoid_function/function.py`

 * *Files identical despite different names*

### Comparing `movoid_function-1.5.4/movoid_function/type.py` & `movoid_function-1.5.5/movoid_function/type.py`

 * *Files 0% similar despite different names*

```diff
@@ -424,15 +424,15 @@
         change_annotation = {}
         for _i, _v in func.__annotations__.items():
             _v_convert = convert_type(_v)
             if _v is None:
                 continue
             else:
                 real_annotation = _v_convert
-                change_annotation[_i] = _v.annotation
+                change_annotation[_i] = _v_convert.annotation
             if _i == 'return':
                 if check_return:
                     return_annotation[_i] = real_annotation
             else:
                 if check_arguments:
                     argument_annotation[_i] = real_annotation
         func.__annotations__ = change_annotation
```

