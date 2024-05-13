# Comparing `tmp/litellm_types-0.0.3.tar.gz` & `tmp/litellm_types-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm_types-0.0.3.tar", last modified: Fri May 10 08:30:58 2024, max compression
+gzip compressed data, was "litellm_types-0.0.4.tar", last modified: Mon May 13 12:28:24 2024, max compression
```

## Comparing `litellm_types-0.0.3.tar` & `litellm_types-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-10 08:30:58.542448 litellm_types-0.0.3/
--rw-r--r--   0 salamanderxing   (501) staff       (20)    11357 2024-05-06 12:34:17.000000 litellm_types-0.0.3/LICENSE
--rw-r--r--   0 salamanderxing   (501) staff       (20)      150 2024-05-10 08:30:58.542270 litellm_types-0.0.3/PKG-INFO
-drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-10 08:30:58.541430 litellm_types-0.0.3/litellm_types/
--rw-r--r--   0 salamanderxing   (501) staff       (20)        2 2024-05-05 16:42:41.000000 litellm_types-0.0.3/litellm_types/__init__.py
--rw-r--r--   0 salamanderxing   (501) staff       (20)     5030 2024-05-06 12:30:27.000000 litellm_types-0.0.3/litellm_types/completion.py
--rw-r--r--   0 salamanderxing   (501) staff       (20)      134 2024-05-05 16:26:12.000000 litellm_types-0.0.3/litellm_types/document.py
--rw-r--r--   0 salamanderxing   (501) staff       (20)     1341 2024-05-05 19:21:12.000000 litellm_types-0.0.3/litellm_types/messages.py
--rw-r--r--   0 salamanderxing   (501) staff       (20)      293 2024-05-05 16:23:45.000000 litellm_types-0.0.3/litellm_types/prompt.py
-drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-10 08:30:58.542085 litellm_types-0.0.3/litellm_types.egg-info/
--rw-r--r--   0 salamanderxing   (501) staff       (20)      150 2024-05-10 08:30:58.000000 litellm_types-0.0.3/litellm_types.egg-info/PKG-INFO
--rw-r--r--   0 salamanderxing   (501) staff       (20)      330 2024-05-10 08:30:58.000000 litellm_types-0.0.3/litellm_types.egg-info/SOURCES.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)        1 2024-05-10 08:30:58.000000 litellm_types-0.0.3/litellm_types.egg-info/dependency_links.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)       26 2024-05-10 08:30:58.000000 litellm_types-0.0.3/litellm_types.egg-info/requires.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)       14 2024-05-10 08:30:58.000000 litellm_types-0.0.3/litellm_types.egg-info/top_level.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)       38 2024-05-10 08:30:58.542484 litellm_types-0.0.3/setup.cfg
--rw-r--r--   0 salamanderxing   (501) staff       (20)      263 2024-05-10 08:30:52.000000 litellm_types-0.0.3/setup.py
+drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-13 12:28:24.133077 litellm_types-0.0.4/
+-rw-r--r--   0 salamanderxing   (501) staff       (20)    11357 2024-05-06 12:34:17.000000 litellm_types-0.0.4/LICENSE
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      150 2024-05-13 12:28:24.132890 litellm_types-0.0.4/PKG-INFO
+drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-13 12:28:24.132071 litellm_types-0.0.4/litellm_types/
+-rw-r--r--   0 salamanderxing   (501) staff       (20)        2 2024-05-05 16:42:41.000000 litellm_types-0.0.4/litellm_types/__init__.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)    11385 2024-05-13 11:48:57.000000 litellm_types-0.0.4/litellm_types/completion.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      134 2024-05-05 16:26:12.000000 litellm_types-0.0.4/litellm_types/document.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)     3875 2024-05-13 12:00:51.000000 litellm_types-0.0.4/litellm_types/messages.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      293 2024-05-05 16:23:45.000000 litellm_types-0.0.4/litellm_types/prompt.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)     1324 2024-05-13 11:50:02.000000 litellm_types-0.0.4/litellm_types/test.py
+drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-13 12:28:24.132710 litellm_types-0.0.4/litellm_types.egg-info/
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      150 2024-05-13 12:28:24.000000 litellm_types-0.0.4/litellm_types.egg-info/PKG-INFO
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      352 2024-05-13 12:28:24.000000 litellm_types-0.0.4/litellm_types.egg-info/SOURCES.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)        1 2024-05-13 12:28:24.000000 litellm_types-0.0.4/litellm_types.egg-info/dependency_links.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)       26 2024-05-13 12:28:24.000000 litellm_types-0.0.4/litellm_types.egg-info/requires.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)       14 2024-05-13 12:28:24.000000 litellm_types-0.0.4/litellm_types.egg-info/top_level.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)       38 2024-05-13 12:28:24.133110 litellm_types-0.0.4/setup.cfg
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      263 2024-05-13 12:28:16.000000 litellm_types-0.0.4/setup.py
```

### Comparing `litellm_types-0.0.3/LICENSE` & `litellm_types-0.0.4/LICENSE`

 * *Files identical despite different names*

