# Comparing `tmp/ops_py_github_tools-1.1.3.tar.gz` & `tmp/ops_py_github_tools-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops_py_github_tools-1.1.3.tar", last modified: Tue May  7 09:23:40 2024, max compression
+gzip compressed data, was "ops_py_github_tools-1.1.4.tar", last modified: Mon May 13 13:04:32 2024, max compression
```

## Comparing `ops_py_github_tools-1.1.3.tar` & `ops_py_github_tools-1.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:40.711229 ops_py_github_tools-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-07 09:23:38.000000 ops_py_github_tools-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-07 09:23:40.707229 ops_py_github_tools-1.1.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:40.707229 ops_py_github_tools-1.1.3/github_tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)      124 2024-05-07 09:23:35.000000 ops_py_github_tools-1.1.3/github_tools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3570 2024-05-07 09:23:35.000000 ops_py_github_tools-1.1.3/github_tools/gh_create_milestone.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11170 2024-05-07 09:23:35.000000 ops_py_github_tools-1.1.3/github_tools/gh_issue_templates.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4956 2024-05-07 09:23:35.000000 ops_py_github_tools-1.1.3/github_tools/gh_repos.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4584 2024-05-07 09:23:35.000000 ops_py_github_tools-1.1.3/github_tools/github_issue_templates.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1092 2024-05-07 09:23:35.000000 ops_py_github_tools-1.1.3/github_tools/github_tools_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:40.707229 ops_py_github_tools-1.1.3/ops_py_github_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-07 09:23:40.000000 ops_py_github_tools-1.1.3/ops_py_github_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-07 09:23:40.000000 ops_py_github_tools-1.1.3/ops_py_github_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:23:40.000000 ops_py_github_tools-1.1.3/ops_py_github_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-07 09:23:40.000000 ops_py_github_tools-1.1.3/ops_py_github_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 09:23:40.000000 ops_py_github_tools-1.1.3/ops_py_github_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 09:23:38.000000 ops_py_github_tools-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-07 09:23:38.000000 ops_py_github_tools-1.1.3/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-07 09:23:35.000000 ops_py_github_tools-1.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 09:23:40.711229 ops_py_github_tools-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-07 09:23:38.000000 ops_py_github_tools-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:04:32.146597 ops_py_github_tools-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-13 13:04:30.000000 ops_py_github_tools-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-13 13:04:32.146597 ops_py_github_tools-1.1.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:04:32.142597 ops_py_github_tools-1.1.4/github_tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      124 2024-05-13 13:04:26.000000 ops_py_github_tools-1.1.4/github_tools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3570 2024-05-13 13:04:26.000000 ops_py_github_tools-1.1.4/github_tools/gh_create_milestone.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11203 2024-05-13 13:04:26.000000 ops_py_github_tools-1.1.4/github_tools/gh_issue_templates.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4956 2024-05-13 13:04:26.000000 ops_py_github_tools-1.1.4/github_tools/gh_repos.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4584 2024-05-13 13:04:26.000000 ops_py_github_tools-1.1.4/github_tools/github_issue_templates.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1092 2024-05-13 13:04:26.000000 ops_py_github_tools-1.1.4/github_tools/github_tools_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:04:32.146597 ops_py_github_tools-1.1.4/ops_py_github_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-13 13:04:32.000000 ops_py_github_tools-1.1.4/ops_py_github_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-13 13:04:32.000000 ops_py_github_tools-1.1.4/ops_py_github_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:04:32.000000 ops_py_github_tools-1.1.4/ops_py_github_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-13 13:04:32.000000 ops_py_github_tools-1.1.4/ops_py_github_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 13:04:32.000000 ops_py_github_tools-1.1.4/ops_py_github_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-13 13:04:30.000000 ops_py_github_tools-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-13 13:04:30.000000 ops_py_github_tools-1.1.4/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-13 13:04:26.000000 ops_py_github_tools-1.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:04:32.146597 ops_py_github_tools-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-13 13:04:30.000000 ops_py_github_tools-1.1.4/setup.py
```

### Comparing `ops_py_github_tools-1.1.3/LICENSE` & `ops_py_github_tools-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ops_py_github_tools-1.1.3/PKG-INFO` & `ops_py_github_tools-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-github-tools
-Version: 1.1.3
+Version: 1.1.4
 Summary: Selection of tools to use with GitHub
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `ops_py_github_tools-1.1.3/github_tools/gh_create_milestone.py` & `ops_py_github_tools-1.1.4/github_tools/gh_create_milestone.py`

 * *Files identical despite different names*

### Comparing `ops_py_github_tools-1.1.3/github_tools/gh_issue_templates.py` & `ops_py_github_tools-1.1.4/github_tools/gh_issue_templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,17 @@
     name: "\U0001f4c7 Collection"
     title: "\U0001f4c7 c-<team_alias>:"
 
     name: "\U0001f4c7 Collection Maintenance"
     title: "\U0001f4c7 mc-<team_alias>:"
     """
 
-    line_prefix = 'title: "'
+    line_prefix = 'title: '
     if string.startswith(line_prefix):
-        string = string.split(line_prefix)[-1]
+        string = string.split(line_prefix)[-1].replace("'", "").replace('"', '')
     title_parts = string.split()
 
     # When the issue title is only one character (should not happen)
     if len(title_parts) == 1:
         return title_parts[0][0]
 
     if len(title_parts) > 1:
```

### Comparing `ops_py_github_tools-1.1.3/github_tools/gh_repos.py` & `ops_py_github_tools-1.1.4/github_tools/gh_repos.py`

 * *Files identical despite different names*

### Comparing `ops_py_github_tools-1.1.3/github_tools/github_issue_templates.py` & `ops_py_github_tools-1.1.4/github_tools/github_issue_templates.py`

 * *Files identical despite different names*

### Comparing `ops_py_github_tools-1.1.3/github_tools/github_tools_examples.py` & `ops_py_github_tools-1.1.4/github_tools/github_tools_examples.py`

 * *Files identical despite different names*

### Comparing `ops_py_github_tools-1.1.3/ops_py_github_tools.egg-info/PKG-INFO` & `ops_py_github_tools-1.1.4/ops_py_github_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-github-tools
-Version: 1.1.3
+Version: 1.1.4
 Summary: Selection of tools to use with GitHub
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `ops_py_github_tools-1.1.3/readme.md` & `ops_py_github_tools-1.1.4/readme.md`

 * *Files identical despite different names*

