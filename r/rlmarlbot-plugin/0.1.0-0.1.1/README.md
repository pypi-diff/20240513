# Comparing `tmp/rlmarlbot_plugin-0.1.0.tar.gz` & `tmp/rlmarlbot_plugin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlmarlbot_plugin-0.1.0.tar", max compression
+gzip compressed data, was "rlmarlbot_plugin-0.1.1.tar", max compression
```

## Comparing `rlmarlbot_plugin-0.1.0.tar` & `rlmarlbot_plugin-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      290 2024-05-13 00:22:21.067015 rlmarlbot_plugin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-13 00:20:02.783433 rlmarlbot_plugin-0.1.0/README.md
--rw-r--r--   0        0        0       34 2024-05-13 00:21:17.003894 rlmarlbot_plugin-0.1.0/rlmarlbot_plugin/__init__.py
--rw-r--r--   0        0        0     1129 2024-05-13 00:10:16.122495 rlmarlbot_plugin-0.1.0/rlmarlbot_plugin/base_plugin.py
--rw-r--r--   0        0        0      334 1970-01-01 00:00:00.000000 rlmarlbot_plugin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      334 2024-05-13 00:39:02.529875 rlmarlbot_plugin-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-13 00:20:02.783433 rlmarlbot_plugin-0.1.1/README.md
+-rw-r--r--   0        0        0       34 2024-05-13 00:21:17.003894 rlmarlbot_plugin-0.1.1/rlmarlbot_plugin/__init__.py
+-rw-r--r--   0        0        0     1129 2024-05-13 00:26:48.171097 rlmarlbot_plugin-0.1.1/rlmarlbot_plugin/base_plugin.py
+-rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 rlmarlbot_plugin-0.1.1/PKG-INFO
```

### Comparing `rlmarlbot_plugin-0.1.0/rlmarlbot_plugin/base_plugin.py` & `rlmarlbot_plugin-0.1.1/rlmarlbot_plugin/base_plugin.py`

 * *Files identical despite different names*

