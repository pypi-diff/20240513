# Comparing `tmp/ctm-cli-0.1.0.tar.gz` & `tmp/ctm-cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctm-cli-0.1.0.tar", last modified: Mon May 13 19:23:12 2024, max compression
+gzip compressed data, was "ctm-cli-0.2.0.tar", last modified: Mon May 13 19:33:01 2024, max compression
```

## Comparing `ctm-cli-0.1.0.tar` & `ctm-cli-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-13 19:23:12.870916 ctm-cli-0.1.0/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      674 2024-05-13 19:23:12.870720 ctm-cli-0.1.0/PKG-INFO
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      235 2024-05-13 19:16:25.000000 ctm-cli-0.1.0/README.md
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-13 19:23:12.868264 ctm-cli-0.1.0/ctm_cli/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       21 2024-05-13 19:16:59.000000 ctm-cli-0.1.0/ctm_cli/__init__.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      907 2024-05-13 19:21:39.000000 ctm-cli-0.1.0/ctm_cli/main.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-13 19:23:12.870378 ctm-cli-0.1.0/ctm_cli.egg-info/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      674 2024-05-13 19:23:12.000000 ctm-cli-0.1.0/ctm_cli.egg-info/PKG-INFO
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      242 2024-05-13 19:23:12.000000 ctm-cli-0.1.0/ctm_cli.egg-info/SOURCES.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2024-05-13 19:23:12.000000 ctm-cli-0.1.0/ctm_cli.egg-info/dependency_links.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       41 2024-05-13 19:23:12.000000 ctm-cli-0.1.0/ctm_cli.egg-info/entry_points.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       46 2024-05-13 19:23:12.000000 ctm-cli-0.1.0/ctm_cli.egg-info/requires.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        8 2024-05-13 19:23:12.000000 ctm-cli-0.1.0/ctm_cli.egg-info/top_level.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2024-05-13 19:23:12.870962 ctm-cli-0.1.0/setup.cfg
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      906 2024-05-13 19:17:57.000000 ctm-cli-0.1.0/setup.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-13 19:33:01.720265 ctm-cli-0.2.0/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      674 2024-05-13 19:33:01.720082 ctm-cli-0.2.0/PKG-INFO
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      235 2024-05-13 19:16:25.000000 ctm-cli-0.2.0/README.md
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-13 19:33:01.717202 ctm-cli-0.2.0/ctm_cli/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       21 2024-05-13 19:32:55.000000 ctm-cli-0.2.0/ctm_cli/__init__.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1018 2024-05-13 19:28:34.000000 ctm-cli-0.2.0/ctm_cli/main.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-13 19:33:01.719213 ctm-cli-0.2.0/ctm_cli.egg-info/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      674 2024-05-13 19:33:01.000000 ctm-cli-0.2.0/ctm_cli.egg-info/PKG-INFO
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      270 2024-05-13 19:33:01.000000 ctm-cli-0.2.0/ctm_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2024-05-13 19:33:01.000000 ctm-cli-0.2.0/ctm_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       41 2024-05-13 19:33:01.000000 ctm-cli-0.2.0/ctm_cli.egg-info/entry_points.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       46 2024-05-13 19:33:01.000000 ctm-cli-0.2.0/ctm_cli.egg-info/requires.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       12 2024-05-13 19:33:01.000000 ctm-cli-0.2.0/ctm_cli.egg-info/top_level.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2024-05-13 19:33:01.720309 ctm-cli-0.2.0/setup.cfg
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      960 2024-05-13 19:31:54.000000 ctm-cli-0.2.0/setup.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-13 19:33:01.719702 ctm-cli-0.2.0/src/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       21 2024-05-13 19:32:55.000000 ctm-cli-0.2.0/src/__init__.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1018 2024-05-13 19:28:34.000000 ctm-cli-0.2.0/src/main.py
```

### Comparing `ctm-cli-0.1.0/PKG-INFO` & `ctm-cli-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctm-cli
-Version: 0.1.0
+Version: 0.2.0
 Summary: A command-line tool for managing configurations, tasks, and schedules
 Home-page: https://github.com/gomleksiz/ctm-cli
 Author: Huseyin G.
 Author-email: huseyim@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ctm-cli-0.1.0/ctm_cli/main.py` & `ctm-cli-0.2.0/ctm_cli/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,8 +25,15 @@
 @click.option('--debug', '-d', is_flag=True, default=False, help='Enable debug mode')
 @click.pass_context
 def main(ctx, log_level, debug):
     if debug:
         log_level = 'DEBUG'
 
     cli = CtmCli(log_level=log_level)
-    ctx.obj = cli.main()
+    ctx.obj = cli.main()
+
+
+def run():
+    main(auto_envvar_prefix='CTM')
+
+if __name__ == '__main__':
+    main(auto_envvar_prefix='CTM')
```

### Comparing `ctm-cli-0.1.0/ctm_cli.egg-info/PKG-INFO` & `ctm-cli-0.2.0/ctm_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctm-cli
-Version: 0.1.0
+Version: 0.2.0
 Summary: A command-line tool for managing configurations, tasks, and schedules
 Home-page: https://github.com/gomleksiz/ctm-cli
 Author: Huseyin G.
 Author-email: huseyim@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ctm-cli-0.1.0/setup.py` & `ctm-cli-0.2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import setuptools
+from ctm_cli import __version__
+version = __version__
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ctm-cli",
-    version="0.1.0",
+    version=version,
     author="Huseyin G.",
     author_email="huseyim@gmail.com",
     description="A command-line tool for managing configurations, tasks, and schedules",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gomleksiz/ctm-cli",
     packages=setuptools.find_packages(),
```

