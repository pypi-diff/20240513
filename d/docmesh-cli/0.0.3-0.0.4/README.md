# Comparing `tmp/docmesh_cli-0.0.3.tar.gz` & `tmp/docmesh_cli-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmesh_cli-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "docmesh_cli-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `docmesh_cli-0.0.3.tar` & `docmesh_cli-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0       17 2024-05-09 08:25:56.000000 docmesh_cli-0.0.3/README.md
--rw-r--r--   0        0        0       83 2024-05-10 06:06:16.907319 docmesh_cli-0.0.3/docmesh_cli/__init__.py
--rw-r--r--   0        0        0     4064 2024-05-10 06:05:13.316314 docmesh_cli-0.0.3/docmesh_cli/client.py
--rw-r--r--   0        0        0      598 2024-05-09 05:29:56.000000 docmesh_cli-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 docmesh_cli-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-05-10 11:02:39.301355 docmesh_cli-0.0.4/README.md
+-rw-r--r--   0        0        0       83 2024-05-13 03:45:10.328509 docmesh_cli-0.0.4/docmesh_cli/__init__.py
+-rw-r--r--   0        0        0     2852 2024-05-11 02:11:13.130193 docmesh_cli-0.0.4/docmesh_cli/client.py
+-rw-r--r--   0        0        0     3896 2024-05-11 05:09:55.588764 docmesh_cli-0.0.4/docmesh_cli/logos.py
+-rw-r--r--   0        0        0      598 2024-05-10 11:02:39.301355 docmesh_cli-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 docmesh_cli-0.0.4/PKG-INFO
```

### Comparing `docmesh_cli-0.0.3/pyproject.toml` & `docmesh_cli-0.0.4/pyproject.toml`

 * *Files identical despite different names*

