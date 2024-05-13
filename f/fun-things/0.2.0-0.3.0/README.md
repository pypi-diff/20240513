# Comparing `tmp/fun_things-0.2.0.tar.gz` & `tmp/fun_things-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fun_things-0.2.0.tar", max compression
+gzip compressed data, was "fun_things-0.3.0.tar", max compression
```

## Comparing `fun_things-0.2.0.tar` & `fun_things-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0        0 2024-04-15 03:49:51.312592 fun_things-0.2.0/README.md
--rw-r--r--   0        0        0       76 2024-04-30 06:37:52.226763 fun_things-0.2.0/fun_things/__init__.py
--rw-r--r--   0        0        0      330 2024-04-30 06:36:45.297965 fun_things-0.2.0/fun_things/generic_json_encoder.py
--rw-r--r--   0        0        0     1268 2024-04-17 08:24:16.933684 fun_things-0.2.0/fun_things/lazy.py
--rw-r--r--   0        0        0      277 2024-04-30 06:38:33.128287 fun_things-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 fun_things-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 03:49:51.312592 fun_things-0.3.0/README.md
+-rw-r--r--   0        0        0      108 2024-05-13 02:40:55.982879 fun_things-0.3.0/fun_things/__init__.py
+-rw-r--r--   0        0        0      330 2024-04-30 06:36:45.297965 fun_things-0.3.0/fun_things/generic_json_encoder.py
+-rw-r--r--   0        0        0     1268 2024-04-17 08:24:16.933684 fun_things-0.3.0/fun_things/lazy.py
+-rw-r--r--   0        0        0     1159 2024-05-13 02:40:34.766995 fun_things-0.3.0/fun_things/proxy_uri.py
+-rw-r--r--   0        0        0      277 2024-05-13 02:41:05.242829 fun_things-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 fun_things-0.3.0/PKG-INFO
```

### Comparing `fun_things-0.2.0/fun_things/lazy.py` & `fun_things-0.3.0/fun_things/lazy.py`

 * *Files identical despite different names*

