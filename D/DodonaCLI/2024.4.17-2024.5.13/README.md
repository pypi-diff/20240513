# Comparing `tmp/dodonacli-2024.4.17.tar.gz` & `tmp/dodonacli-2024.5.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dodonacli-2024.4.17.tar", last modified: Wed Apr 17 20:28:39 2024, max compression
+gzip compressed data, was "dodonacli-2024.5.13.tar", last modified: Mon May 13 10:22:25 2024, max compression
```

## Comparing `dodonacli-2024.4.17.tar` & `dodonacli-2024.5.13.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:28:39.546408 dodonacli-2024.4.17/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:28:39.538407 dodonacli-2024.4.17/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:28:39.538407 dodonacli-2024.4.17/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/.github/workflows/prevent_outside_pr_master.yml
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/.github/workflows/publish_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:28:39.542407 dodonacli-2024.4.17/DodonaCLI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10034 2024-04-17 20:28:39.000000 dodonacli-2024.4.17/DodonaCLI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-17 20:28:39.000000 dodonacli-2024.4.17/DodonaCLI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 20:28:39.000000 dodonacli-2024.4.17/DodonaCLI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-17 20:28:39.000000 dodonacli-2024.4.17/DodonaCLI.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-17 20:28:39.000000 dodonacli-2024.4.17/DodonaCLI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 20:28:39.000000 dodonacli-2024.4.17/DodonaCLI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10034 2024-04-17 20:28:39.546408 dodonacli-2024.4.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8170 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:28:39.542407 dodonacli-2024.4.17/dodonacli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:28:39.542407 dodonacli-2024.4.17/dodonacli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/commands/cli_next.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/commands/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/commands/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/commands/select.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/commands/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/commands/submission.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/commands/tutorial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/commands/up.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      945 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:28:39.542407 dodonacli-2024.4.17/dodonacli/source/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/source/get_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11938 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/source/interactive_tutorial.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/source/pretty_console.py
--rw-r--r--   0 runner    (1001) docker     (127)    14473 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/source/pretty_print.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/source/set_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli/source/syntax_checker.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1465 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/dodonacli_completion_script.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:28:39.542407 dodonacli-2024.4.17/man-page/
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/man-page/dodonacli.1
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/man-page/dodonacli.1.gz
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-17 20:28:32.000000 dodonacli-2024.4.17/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 20:28:39.546408 dodonacli-2024.4.17/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:22:25.213991 dodonacli-2024.5.13/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:22:25.205991 dodonacli-2024.5.13/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:22:25.209991 dodonacli-2024.5.13/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/.github/workflows/publish_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/.github/workflows/set_version.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:22:25.213991 dodonacli-2024.5.13/DodonaCLI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-05-13 10:22:25.000000 dodonacli-2024.5.13/DodonaCLI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-13 10:22:25.000000 dodonacli-2024.5.13/DodonaCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 10:22:25.000000 dodonacli-2024.5.13/DodonaCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-13 10:22:25.000000 dodonacli-2024.5.13/DodonaCLI.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 10:22:25.000000 dodonacli-2024.5.13/DodonaCLI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-13 10:22:25.000000 dodonacli-2024.5.13/DodonaCLI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-05-13 10:22:25.213991 dodonacli-2024.5.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:22:25.209991 dodonacli-2024.5.13/dodonacli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:22:25.209991 dodonacli-2024.5.13/dodonacli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/commands/cli_next.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/commands/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/commands/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/commands/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/commands/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/commands/submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/commands/tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/commands/up.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      945 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:22:25.213991 dodonacli-2024.5.13/dodonacli/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/source/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11938 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/source/interactive_tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/source/pretty_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13709 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/source/pretty_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/source/set_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/source/submission_data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/source/syntax_checker.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1465 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli_completion_script.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:22:25.213991 dodonacli-2024.5.13/man-page/
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/man-page/dodonacli.1
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/man-page/dodonacli.1.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 10:22:25.213991 dodonacli-2024.5.13/setup.cfg
```

### Comparing `dodonacli-2024.4.17/.github/workflows/publish.yml` & `dodonacli-2024.5.13/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.4.17/.github/workflows/publish_test.yml` & `dodonacli-2024.5.13/.github/workflows/publish_test.yml`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.4.17/DodonaCLI.egg-info/PKG-INFO` & `dodonacli-2024.5.13/DodonaCLI.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DodonaCLI
-Version: 2024.4.17
+Version: 2024.5.13
 Summary: A CLI tool for Dodona
 Author-email: Bram Windey <windey.bram@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Bram Windey
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -184,7 +184,11 @@
 - add connection time-out to prevent long waiting when IPv6 doesn’t want to work along
 - add support for more languages syntax checkers
 - caching some info for faster navigation and/or autocompletion
 - add indicator to series to mark if all their exercises are completely solved (maybe fetch from html-version)
 - get exercise-names via html-parsing for a submission list to only need 1 API call (instead of 30). Am I salty about that not being just field in the API, yes I am! Glad you noticed. Html-parsing isn’t a hobby of mine after all
 - format weird markup in some feedback of submissions (like the Python and bash exercises)
 - add "completions_script" and "manpage" as subcommands to "info"
+
+Github stuff to figure out:
+- release by tag/release
+- action to check valid version before trying to push, if not valid, make it valid
```

### Comparing `dodonacli-2024.4.17/DodonaCLI.egg-info/SOURCES.txt` & `dodonacli-2024.5.13/DodonaCLI.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 .gitignore
 LICENSE
 README.md
 dodonacli_completion_script.sh
 pyproject.toml
 .github/PULL_REQUEST_TEMPLATE.md
-.github/workflows/prevent_outside_pr_master.yml
 .github/workflows/publish.yml
 .github/workflows/publish_test.yml
+.github/workflows/set_version.yml
 DodonaCLI.egg-info/PKG-INFO
 DodonaCLI.egg-info/SOURCES.txt
 DodonaCLI.egg-info/dependency_links.txt
 DodonaCLI.egg-info/entry_points.txt
 DodonaCLI.egg-info/requires.txt
 DodonaCLI.egg-info/top_level.txt
 dodonacli/__init__.py
@@ -27,10 +27,11 @@
 dodonacli/commands/up.py
 dodonacli/source/__init__.py
 dodonacli/source/get_data.py
 dodonacli/source/interactive_tutorial.py
 dodonacli/source/pretty_console.py
 dodonacli/source/pretty_print.py
 dodonacli/source/set_data.py
+dodonacli/source/submission_data_handler.py
 dodonacli/source/syntax_checker.py
 man-page/dodonacli.1
 man-page/dodonacli.1.gz
```

### Comparing `dodonacli-2024.4.17/LICENSE` & `dodonacli-2024.5.13/LICENSE`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.4.17/PKG-INFO` & `dodonacli-2024.5.13/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DodonaCLI
-Version: 2024.4.17
+Version: 2024.5.13
 Summary: A CLI tool for Dodona
 Author-email: Bram Windey <windey.bram@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Bram Windey
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -184,7 +184,11 @@
 - add connection time-out to prevent long waiting when IPv6 doesn’t want to work along
 - add support for more languages syntax checkers
 - caching some info for faster navigation and/or autocompletion
 - add indicator to series to mark if all their exercises are completely solved (maybe fetch from html-version)
 - get exercise-names via html-parsing for a submission list to only need 1 API call (instead of 30). Am I salty about that not being just field in the API, yes I am! Glad you noticed. Html-parsing isn’t a hobby of mine after all
 - format weird markup in some feedback of submissions (like the Python and bash exercises)
 - add "completions_script" and "manpage" as subcommands to "info"
+
+Github stuff to figure out:
+- release by tag/release
+- action to check valid version before trying to push, if not valid, make it valid
```

### Comparing `dodonacli-2024.4.17/README.md` & `dodonacli-2024.5.13/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -141,7 +141,11 @@
 - add connection time-out to prevent long waiting when IPv6 doesn’t want to work along
 - add support for more languages syntax checkers
 - caching some info for faster navigation and/or autocompletion
 - add indicator to series to mark if all their exercises are completely solved (maybe fetch from html-version)
 - get exercise-names via html-parsing for a submission list to only need 1 API call (instead of 30). Am I salty about that not being just field in the API, yes I am! Glad you noticed. Html-parsing isn’t a hobby of mine after all
 - format weird markup in some feedback of submissions (like the Python and bash exercises)
 - add "completions_script" and "manpage" as subcommands to "info"
+
+Github stuff to figure out:
+- release by tag/release
+- action to check valid version before trying to push, if not valid, make it valid
```

### Comparing `dodonacli-2024.4.17/dodonacli/commands/cli_next.py` & `dodonacli-2024.5.13/dodonacli/commands/cli_next.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.4.17/dodonacli/commands/display.py` & `dodonacli-2024.5.13/dodonacli/commands/display.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.4.17/dodonacli/commands/info.py` & `dodonacli-2024.5.13/dodonacli/commands/info.py`

 * *Files 7% similar despite different names*

```diff
@@ -102,22 +102,17 @@
 
 @click.command(help='Changelog for the latest version.')
 def changelog():
     from rich.markdown import Markdown
     from dodonacli.source import pretty_console
 
     changelog_raw = """
-- Fixed inconsistent aligning on 'dodona sub view'
-- Improved the syntax-checker for:
-    - Java, now supports multiple classes by compiling all .java-files in the current directory
-    - JavaScript, switched from jshint to node to check syntax, which most JS-devs will have installed already
-- Fixed a wrong link that prevented you from using 'dodona next' inside a hidden series
-- Added check to prevent you from going to a 'next' course when you're in a hidden one, I feel this is a good change, if you disagree, let me know on GitHub
-- Fixed the bash completion script to correctly complete after 'dodona info'
-- Improved the sentence under this one to be more friendly.
+- Working on rendering feedback. Please report any troubles you have. 
+I may not be able to solve them, but I can definitly hide them =D
+This is not a full implementation, you should only be able to see which tabs were wrong and wich were correct.
 
 As always, you can use the "--help" flag after every command and sub-command to learn more.
 Happy coding!
     """
     md = Markdown(changelog_raw)
     pretty_console.console.print(md)
```

### Comparing `dodonacli-2024.4.17/dodonacli/commands/post.py` & `dodonacli-2024.5.13/dodonacli/commands/post.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import click
 
 
 @click.command(help="Post a solution-file to Dodona. "
                     "The file has to be in your current working directory, and this only works "
-                    "if there is a selected exercise.")
+                    "if there is a selected exercise. "
+                    "DodonaCLI will give a try at rendering a small part of the feedback-table so you can continue "
+                    "working from the terminal, this isn't guarenteed to provide enough info, but it's doing its best.")
 @click.option("-l", "--use-link",
               help="Post your solutionfile to the link at the first line of your solutionfile. "
                    "This is inspired by plugins for editors as VSCode for Dodona.",
               is_flag=True, default=False)
 @click.option("-c", "--check",
               help="Check the file you provided if the syntax is valid for the programming language "
                    "associated with the exercise. Currently supported languages: bash, python, java, "
```

### Comparing `dodonacli-2024.4.17/dodonacli/commands/select.py` & `dodonacli-2024.5.13/dodonacli/commands/select.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.4.17/dodonacli/commands/submission.py` & `dodonacli-2024.5.13/dodonacli/commands/submission.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.4.17/dodonacli/commands/up.py` & `dodonacli-2024.5.13/dodonacli/commands/up.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.4.17/dodonacli/main.py` & `dodonacli-2024.5.13/dodonacli/main.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.4.17/dodonacli/source/get_data.py` & `dodonacli-2024.5.13/dodonacli/source/get_data.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.4.17/dodonacli/source/interactive_tutorial.py` & `dodonacli-2024.5.13/dodonacli/source/interactive_tutorial.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.4.17/dodonacli/source/pretty_print.py` & `dodonacli-2024.5.13/dodonacli/source/pretty_print.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import shutil
 import textwrap
 
 from bs4 import BeautifulSoup
 from rich.markdown import Markdown
 from rich.padding import Padding
 
-from . import get_data, pretty_console
+from . import get_data, pretty_console, submission_data_handler
 
 
 def print_courses_data(json_data: dict, title: str = "Your courses:", prefixes: dict = None):
     """
     Print out the courses in json_data in a neat way
     :param json_data: json object with data about Dodona courses
     :param title: title to display above the courses-list
@@ -111,16 +111,17 @@
             new_description = textwrap.indent(new_description, '\t')
             pretty_console.console.print(
                 f"\t{series[0].ljust(max_series_id_length)}: "
                 f"[bold]{series[1].ljust(max_series_name_length)}[/]"
                 f"\n{new_description}")
         else:
             pretty_console.console.print(
-                (prefixes.get(series[0]) or "\t") + f"{series[0].ljust(max_series_id_length)}: "
-                f"[bold]{series[1].ljust(max_series_name_length)}[/]"
+                (prefixes.get(series[0]) or "\t")
+                + f"{series[0].ljust(max_series_id_length)}: "
+                + f"[bold]{series[1].ljust(max_series_name_length)}[/]"
             )
     # Newline for clarity
     print()
 
 
 def print_exercise_data(json_data: dict, prefixes: dict = None):
     """
@@ -183,16 +184,17 @@
             else:
                 solve_status = "[bold]NOT YET READ[/]"
 
         else:
             solve_status = "[bold]SOLVE STATUS UNKNOWN"
 
         pretty_console.console.print(
-            (prefixes.get(exercise['id']) or "\t") + f"{exercise['id'].ljust(max_exercise_id_length)}: "
-            f"[bold]{exercise['name'].ljust(max_exercise_name_length)}[/]\t"
+            (prefixes.get(exercise['id']) or "\t")
+            + f"{exercise['id'].ljust(max_exercise_id_length)}: "
+            + f"[bold]{exercise['name'].ljust(max_exercise_name_length)}[/]\t"
             + solve_status
         )
     print()
 
 
 def print_exercise(json_data: dict, token: str, force: bool = False):
     """
@@ -211,17 +213,17 @@
 
     elif not force:
         pretty_console.console.print("\nYou can find the description at \n" + json_data['description_url'] + '\n')
 
     else:
         # Print the HTML with warnings
         warning = (
-            "\n[u bold bright_red]WARNING:[/] the description may be incorrect, "
-            "DO NOT rely on this for exams and tests!\n"
-            "View in browser: " + json_data['description_url'] + '\n'
+                "\n[u bold bright_red]WARNING:[/] the description may be incorrect, "
+                "DO NOT rely on this for exams and tests!\n"
+                "View in browser: " + json_data['description_url'] + '\n'
         )
         pretty_console.console.print(warning)
 
         pretty_console.console.print(
             '\n'
             "Expected programming language: " + json_data['programming_language']['name'] +
             '\n'
@@ -255,32 +257,15 @@
     :param json_results: json object with data about a submission
     """
     if json_results['accepted']:
         # Everything passed, well done!
         pretty_console.console.print("[bold bright_green]All tests passed![/] You can continue to next exercise.")
     else:
         pretty_console.console.print("[bold bright_red]Some tests faild.[/]")
-        # try:
-        #     if json_results['status'] in ("memory limit exceeded", "test"):
-        #         print("\t" + json_results['description'])
-        #         return
-        #
-        #     # There were some problems, list them here
-        #     for group in json_results['groups']:
-        #         print(group['description'] + ": " + str(group['badgeCount']) + " tests failed.")
-        #
-        #         if group['badgeCount'] > 0:
-        #             print("Failed exercises:")
-        #             for test in group['groups']:
-        #                 if not test['accepted']:
-        #                     pass
-        #                     print("\t- " + test['groups'][0]['description'] + "\n\t\t" +
-        #                           test['groups'][0]['description']['description'])
-        # except Exception as e:
-        #     print("\tSomething went wrong trying to display the results: " + str(e))
+        pretty_console.console.print(submission_data_handler.submission_data_handler(json_results))
 
 
 def print_status(config: dict):
     """
     Print out the current selection of course, exercise-series and exercise.
     :param config: Dictionary with the configs
     """
```

### Comparing `dodonacli-2024.4.17/dodonacli/source/set_data.py` & `dodonacli-2024.5.13/dodonacli/source/set_data.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.4.17/dodonacli/source/syntax_checker.py` & `dodonacli-2024.5.13/dodonacli/source/syntax_checker.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.4.17/dodonacli_completion_script.sh` & `dodonacli-2024.5.13/dodonacli_completion_script.sh`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.4.17/man-page/dodonacli.1` & `dodonacli-2024.5.13/man-page/dodonacli.1`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.4.17/man-page/dodonacli.1.gz` & `dodonacli-2024.5.13/man-page/dodonacli.1.gz`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.4.17/pyproject.toml` & `dodonacli-2024.5.13/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "DodonaCLI"
-version = "2024.4.17"
+version = "2024.5.13"
 authors = [
     { name = "Bram Windey", email = "windey.bram@gmail.com" },
 ]
 description = "A CLI tool for Dodona"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
```

