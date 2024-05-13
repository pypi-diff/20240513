# Comparing `tmp/rlmarlbot_plugin-0.1.4.tar.gz` & `tmp/rlmarlbot_plugin-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlmarlbot_plugin-0.1.4.tar", max compression
+gzip compressed data, was "rlmarlbot_plugin-0.1.5.tar", max compression
```

## Comparing `rlmarlbot_plugin-0.1.4.tar` & `rlmarlbot_plugin-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      334 2024-05-13 00:58:01.153386 rlmarlbot_plugin-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-13 00:20:02.783433 rlmarlbot_plugin-0.1.4/README.md
--rw-r--r--   0        0        0       51 2024-05-13 00:47:16.864668 rlmarlbot_plugin-0.1.4/rlmarlbot_plugin/__init__.py
--rw-r--r--   0        0        0      972 2024-05-13 00:57:38.139149 rlmarlbot_plugin-0.1.4/rlmarlbot_plugin/base_plugin.py
--rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 rlmarlbot_plugin-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      334 2024-05-13 07:08:48.054815 rlmarlbot_plugin-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-13 00:20:02.783433 rlmarlbot_plugin-0.1.5/README.md
+-rw-r--r--   0        0        0       51 2024-05-13 00:47:16.864668 rlmarlbot_plugin-0.1.5/rlmarlbot_plugin/__init__.py
+-rw-r--r--   0        0        0     1804 2024-05-13 07:00:56.558306 rlmarlbot_plugin-0.1.5/rlmarlbot_plugin/base_plugin.py
+-rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 rlmarlbot_plugin-0.1.5/PKG-INFO
```

