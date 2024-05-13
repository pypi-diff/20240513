# Comparing `tmp/trapezoidal_fuzzy_number-1.1.tar.gz` & `tmp/trapezoidal_fuzzy_number-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trapezoidal_fuzzy_number-1.1.tar", last modified: Sat May 11 03:46:18 2024, max compression
+gzip compressed data, was "trapezoidal_fuzzy_number-1.2.tar", last modified: Mon May 13 06:55:24 2024, max compression
```

## Comparing `trapezoidal_fuzzy_number-1.1.tar` & `trapezoidal_fuzzy_number-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 03:46:18.278924 trapezoidal_fuzzy_number-1.1/
--rw-rw-rw-   0        0        0     1073 2024-05-11 01:40:35.000000 trapezoidal_fuzzy_number-1.1/LICENSE
--rw-rw-rw-   0        0        0      328 2024-05-11 03:46:18.278924 trapezoidal_fuzzy_number-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       48 2024-05-11 01:41:42.000000 trapezoidal_fuzzy_number-1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 03:46:18.263301 trapezoidal_fuzzy_number-1.1/Trapezoidal_Fuzzy_Number/
--rw-rw-rw-   0        0        0     1541 2024-05-11 03:40:18.000000 trapezoidal_fuzzy_number-1.1/Trapezoidal_Fuzzy_Number/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 03:46:18.278924 trapezoidal_fuzzy_number-1.1/Trapezoidal_Fuzzy_Number.egg-info/
--rw-rw-rw-   0        0        0      328 2024-05-11 03:46:18.000000 trapezoidal_fuzzy_number-1.1/Trapezoidal_Fuzzy_Number.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2024-05-11 03:46:18.000000 trapezoidal_fuzzy_number-1.1/Trapezoidal_Fuzzy_Number.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 03:46:18.000000 trapezoidal_fuzzy_number-1.1/Trapezoidal_Fuzzy_Number.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-11 03:46:18.000000 trapezoidal_fuzzy_number-1.1/Trapezoidal_Fuzzy_Number.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 03:46:18.278924 trapezoidal_fuzzy_number-1.1/setup.cfg
--rw-rw-rw-   0        0        0      453 2024-05-11 03:46:07.000000 trapezoidal_fuzzy_number-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 06:55:24.760461 trapezoidal_fuzzy_number-1.2/
+-rw-rw-rw-   0        0        0     1073 2024-05-11 01:40:35.000000 trapezoidal_fuzzy_number-1.2/LICENSE
+-rw-rw-rw-   0        0        0      263 2024-05-13 06:55:24.760461 trapezoidal_fuzzy_number-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       48 2024-05-11 01:41:42.000000 trapezoidal_fuzzy_number-1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 06:55:24.744840 trapezoidal_fuzzy_number-1.2/Trapezoidal_Fuzzy_Number/
+-rw-rw-rw-   0        0        0     1541 2024-05-13 06:50:57.000000 trapezoidal_fuzzy_number-1.2/Trapezoidal_Fuzzy_Number/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 06:55:24.760461 trapezoidal_fuzzy_number-1.2/Trapezoidal_Fuzzy_Number.egg-info/
+-rw-rw-rw-   0        0        0      263 2024-05-13 06:55:24.000000 trapezoidal_fuzzy_number-1.2/Trapezoidal_Fuzzy_Number.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-05-13 06:55:24.000000 trapezoidal_fuzzy_number-1.2/Trapezoidal_Fuzzy_Number.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 06:55:24.000000 trapezoidal_fuzzy_number-1.2/Trapezoidal_Fuzzy_Number.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-13 06:55:24.000000 trapezoidal_fuzzy_number-1.2/Trapezoidal_Fuzzy_Number.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 06:55:24.760461 trapezoidal_fuzzy_number-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      368 2024-05-13 06:46:52.000000 trapezoidal_fuzzy_number-1.2/setup.py
```

### Comparing `trapezoidal_fuzzy_number-1.1/LICENSE` & `trapezoidal_fuzzy_number-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trapezoidal_fuzzy_number-1.1/Trapezoidal_Fuzzy_Number/__init__.py` & `trapezoidal_fuzzy_number-1.2/Trapezoidal_Fuzzy_Number/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,12 +26,12 @@
 
     def __truediv__(self, other):
         # Division of two trapezoidal fuzzy numbers
         return [self.a / other.d, self.b / other.c, self.c / other.b, self.d / other.a]
 
     def __rtruediv__(self, scalar):
         # Division of a real number and a fuzzy number
-        return [scalar / self.a, scalar / self.b, scalar / self.c, scalar / self.d]
+        return [scalar / self.d, scalar / self.c, scalar / self.b, scalar / self.a]
 
     def __floordiv__(self, scalar):
         # Division of a trapezoidal fuzzy number and a real number
         return [self.a // scalar, self.b // scalar, self.c // scalar, self.d // scalar]
```

