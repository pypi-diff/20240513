# Comparing `tmp/lib_version_group3-0.1.1.tar.gz` & `tmp/lib_version_group3-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_version_group3-0.1.1.tar", max compression
+gzip compressed data, was "lib_version_group3-0.1.2.tar", max compression
```

## Comparing `lib_version_group3-0.1.1.tar` & `lib_version_group3-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2024-05-12 19:07:45.839952 lib_version_group3-0.1.1/LICENSE
--rw-r--r--   0        0        0      431 2024-05-12 19:07:45.839952 lib_version_group3-0.1.1/README.md
--rw-r--r--   0        0        0      459 2024-05-12 19:07:45.839952 lib_version_group3-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      234 2024-05-12 19:07:45.839952 lib_version_group3-0.1.1/src/lib_version_group3/__init__.py
--rw-r--r--   0        0        0       23 2024-05-12 19:08:02.040108 lib_version_group3-0.1.1/src/lib_version_group3/version.py
--rw-r--r--   0        0        0     1062 1970-01-01 00:00:00.000000 lib_version_group3-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-10 15:23:27.917798 lib_version_group3-0.1.2/LICENSE
+-rw-r--r--   0        0        0      431 2024-05-12 06:35:19.316021 lib_version_group3-0.1.2/README.md
+-rw-r--r--   0        0        0      459 2024-05-13 07:31:03.044656 lib_version_group3-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      234 2024-05-12 06:35:19.317123 lib_version_group3-0.1.2/src/lib_version_group3/__init__.py
+-rw-r--r--   0        0        0      599 2024-05-12 06:35:19.317296 lib_version_group3-0.1.2/src/lib_version_group3/version.py
+-rw-r--r--   0        0        0     1062 1970-01-01 00:00:00.000000 lib_version_group3-0.1.2/PKG-INFO
```

### Comparing `lib_version_group3-0.1.1/LICENSE` & `lib_version_group3-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lib_version_group3-0.1.1/PKG-INFO` & `lib_version_group3-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib_version_group3
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library for managing and retrieving the software version.
 License: MIT
 Author: smtan
 Author-email: tan.stevenmitchell@gmail.com
 Requires-Python: >=3.8,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

