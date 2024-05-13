# Comparing `tmp/parse_llm_code-0.1.27.tar.gz` & `tmp/parse_llm_code-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parse_llm_code-0.1.27.tar", last modified: Mon May 13 07:06:50 2024, max compression
+gzip compressed data, was "parse_llm_code-0.1.5.tar", last modified: Sun May 12 12:03:20 2024, max compression
```

## Comparing `parse_llm_code-0.1.27.tar` & `parse_llm_code-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:06:50.523351 parse_llm_code-0.1.27/
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-13 07:06:50.523351 parse_llm_code-0.1.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-13 07:06:47.000000 parse_llm_code-0.1.27/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:06:50.519351 parse_llm_code-0.1.27/parse_llm_code/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-13 07:06:47.000000 parse_llm_code-0.1.27/parse_llm_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-13 07:06:47.000000 parse_llm_code-0.1.27/parse_llm_code/extract_code.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:06:50.523351 parse_llm_code-0.1.27/parse_llm_code.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-13 07:06:50.000000 parse_llm_code-0.1.27/parse_llm_code.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-13 07:06:50.000000 parse_llm_code-0.1.27/parse_llm_code.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 07:06:50.000000 parse_llm_code-0.1.27/parse_llm_code.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-13 07:06:50.000000 parse_llm_code-0.1.27/parse_llm_code.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 07:06:50.523351 parse_llm_code-0.1.27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-13 07:06:47.000000 parse_llm_code-0.1.27/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:06:50.523351 parse_llm_code-0.1.27/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:06:47.000000 parse_llm_code-0.1.27/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-13 07:06:47.000000 parse_llm_code-0.1.27/tests/test_extract_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-13 07:06:47.000000 parse_llm_code-0.1.27/tests/test_extract_first_code.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-12 12:03:20.383337 parse_llm_code-0.1.5/
+-rw-r--r--   0 apple      (501) staff       (20)     2566 2024-05-12 12:03:20.383116 parse_llm_code-0.1.5/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)     2170 2024-05-12 04:20:35.000000 parse_llm_code-0.1.5/README.md
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-12 12:03:20.381957 parse_llm_code-0.1.5/parse_llm_code/
+-rw-r--r--   0 apple      (501) staff       (20)      189 2024-05-12 03:59:03.000000 parse_llm_code-0.1.5/parse_llm_code/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     1945 2024-05-12 03:34:57.000000 parse_llm_code-0.1.5/parse_llm_code/extract_code.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-12 12:03:20.382910 parse_llm_code-0.1.5/parse_llm_code.egg-info/
+-rw-r--r--   0 apple      (501) staff       (20)     2566 2024-05-12 12:03:20.000000 parse_llm_code-0.1.5/parse_llm_code.egg-info/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)      307 2024-05-12 12:03:20.000000 parse_llm_code-0.1.5/parse_llm_code.egg-info/SOURCES.txt
+-rw-r--r--   0 apple      (501) staff       (20)        1 2024-05-12 12:03:20.000000 parse_llm_code-0.1.5/parse_llm_code.egg-info/dependency_links.txt
+-rw-r--r--   0 apple      (501) staff       (20)       21 2024-05-12 12:03:20.000000 parse_llm_code-0.1.5/parse_llm_code.egg-info/top_level.txt
+-rw-r--r--   0 apple      (501) staff       (20)       38 2024-05-12 12:03:20.383383 parse_llm_code-0.1.5/setup.cfg
+-rw-r--r--   0 apple      (501) staff       (20)      628 2024-05-12 12:03:16.000000 parse_llm_code-0.1.5/setup.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-12 12:03:20.382741 parse_llm_code-0.1.5/tests/
+-rw-r--r--   0 apple      (501) staff       (20)        0 2024-05-11 18:16:52.000000 parse_llm_code-0.1.5/tests/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     1719 2024-05-12 04:13:51.000000 parse_llm_code-0.1.5/tests/test_extract_codes.py
+-rw-r--r--   0 apple      (501) staff       (20)     1257 2024-05-12 04:11:36.000000 parse_llm_code-0.1.5/tests/test_extract_first_code.py
```

### Comparing `parse_llm_code-0.1.27/PKG-INFO` & `parse_llm_code-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: parse_llm_code
-Version: 0.1.27
+Version: 0.1.5
 Summary: a lib to parse llm answer to code
-Home-page: https://github.com/aboutmydreams/parse_llm_code
+Home-page: https://github.com/pypa/parse_llm_code
 Author: aboutmydreams
 Author-email: aboutmydreams@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `parse_llm_code-0.1.27/README.md` & `parse_llm_code-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `parse_llm_code-0.1.27/parse_llm_code/extract_code.py` & `parse_llm_code-0.1.5/parse_llm_code/extract_code.py`

 * *Files identical despite different names*

### Comparing `parse_llm_code-0.1.27/parse_llm_code.egg-info/PKG-INFO` & `parse_llm_code-0.1.5/parse_llm_code.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: parse_llm_code
-Version: 0.1.27
+Version: 0.1.5
 Summary: a lib to parse llm answer to code
-Home-page: https://github.com/aboutmydreams/parse_llm_code
+Home-page: https://github.com/pypa/parse_llm_code
 Author: aboutmydreams
 Author-email: aboutmydreams@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `parse_llm_code-0.1.27/tests/test_extract_codes.py` & `parse_llm_code-0.1.5/tests/test_extract_codes.py`

 * *Files identical despite different names*

### Comparing `parse_llm_code-0.1.27/tests/test_extract_first_code.py` & `parse_llm_code-0.1.5/tests/test_extract_first_code.py`

 * *Files identical despite different names*

