# Comparing `tmp/autopkg_wrapper-2024.3.1.tar.gz` & `tmp/autopkg_wrapper-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopkg_wrapper-2024.3.1.tar", max compression
+gzip compressed data, was "autopkg_wrapper-2024.5.1.tar", max compression
```

## Comparing `autopkg_wrapper-2024.3.1.tar` & `autopkg_wrapper-2024.5.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1602 2024-03-18 06:13:23.886052 autopkg_wrapper-2024.3.1/LICENSE
--rw-r--r--   0        0        0     1833 2024-03-18 06:13:23.886052 autopkg_wrapper-2024.3.1/README.md
--rw-r--r--   0        0        0       25 2024-03-18 06:13:50.662083 autopkg_wrapper-2024.3.1/autopkg_wrapper/__init__.py
--rwxr-xr-x   0        0        0    10387 2024-03-18 06:13:23.886052 autopkg_wrapper-2024.3.1/autopkg_wrapper/autopkg_wrapper.py
--rw-r--r--   0        0        0       22 2024-03-18 06:13:23.886052 autopkg_wrapper-2024.3.1/autopkg_wrapper/notifier/__init__.py
--rw-r--r--   0        0        0     1982 2024-03-18 06:13:23.886052 autopkg_wrapper-2024.3.1/autopkg_wrapper/notifier/slack.py
--rw-r--r--   0        0        0       22 2024-03-18 06:13:23.886052 autopkg_wrapper-2024.3.1/autopkg_wrapper/utils/__init__.py
--rw-r--r--   0        0        0     3934 2024-03-18 06:13:23.886052 autopkg_wrapper-2024.3.1/autopkg_wrapper/utils/args.py
--rw-r--r--   0        0        0     2975 2024-03-18 06:13:23.886052 autopkg_wrapper-2024.3.1/autopkg_wrapper/utils/git_functions.py
--rw-r--r--   0        0        0      324 2024-03-18 06:13:23.886052 autopkg_wrapper-2024.3.1/autopkg_wrapper/utils/logging.py
--rw-r--r--   0        0        0     1038 2024-03-18 06:13:50.658083 autopkg_wrapper-2024.3.1/pyproject.toml
--rw-r--r--   0        0        0     2659 1970-01-01 00:00:00.000000 autopkg_wrapper-2024.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1602 2024-05-13 03:58:20.101243 autopkg_wrapper-2024.5.1/LICENSE
+-rw-r--r--   0        0        0     1833 2024-05-13 03:58:20.101243 autopkg_wrapper-2024.5.1/README.md
+-rw-r--r--   0        0        0       25 2024-05-13 03:58:42.681450 autopkg_wrapper-2024.5.1/autopkg_wrapper/__init__.py
+-rwxr-xr-x   0        0        0    10410 2024-05-13 03:58:20.101243 autopkg_wrapper-2024.5.1/autopkg_wrapper/autopkg_wrapper.py
+-rw-r--r--   0        0        0       22 2024-05-13 03:58:20.101243 autopkg_wrapper-2024.5.1/autopkg_wrapper/notifier/__init__.py
+-rw-r--r--   0        0        0     1982 2024-05-13 03:58:20.101243 autopkg_wrapper-2024.5.1/autopkg_wrapper/notifier/slack.py
+-rw-r--r--   0        0        0       22 2024-05-13 03:58:20.101243 autopkg_wrapper-2024.5.1/autopkg_wrapper/utils/__init__.py
+-rw-r--r--   0        0        0     3934 2024-05-13 03:58:20.101243 autopkg_wrapper-2024.5.1/autopkg_wrapper/utils/args.py
+-rw-r--r--   0        0        0     2975 2024-05-13 03:58:20.101243 autopkg_wrapper-2024.5.1/autopkg_wrapper/utils/git_functions.py
+-rw-r--r--   0        0        0      324 2024-05-13 03:58:20.101243 autopkg_wrapper-2024.5.1/autopkg_wrapper/utils/logging.py
+-rw-r--r--   0        0        0     1038 2024-05-13 03:58:42.673450 autopkg_wrapper-2024.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2659 1970-01-01 00:00:00.000000 autopkg_wrapper-2024.5.1/PKG-INFO
```

### Comparing `autopkg_wrapper-2024.3.1/LICENSE` & `autopkg_wrapper-2024.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autopkg_wrapper-2024.3.1/README.md` & `autopkg_wrapper-2024.5.1/README.md`

 * *Files identical despite different names*

### Comparing `autopkg_wrapper-2024.3.1/autopkg_wrapper/autopkg_wrapper.py` & `autopkg_wrapper-2024.5.1/autopkg_wrapper/autopkg_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     @property
     def name(self):
         name = self.filename.split(".")[0]
 
         return name
 
     def verify_trust_info(self):
-        cmd = ["/usr/local/bin/autopkg", "verify-trust-info", self.filename, "-vv"]
+        cmd = ["/usr/local/bin/autopkg", "verify-trust-info", self.filename, "-v"]
         cmd = " ".join(cmd)
         logging.debug(f"cmd: {str(cmd)}")
 
         p = subprocess.Popen(
             cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True
         )
         (output, err) = p.communicate()
@@ -88,15 +88,15 @@
 
             try:
                 post_processor_cmd = list(chain.from_iterable([("--post", processor) for processor in self.post_processors])) if self.post_processors else None
                 initial_cmd = [
                     "/usr/local/bin/autopkg",
                     "run",
                     self.filename,
-                    "-vv",
+                    "-v",
                     "--report-plist",
                     str(report),
                 ]
                 cmd = initial_cmd + post_processor_cmd if post_processor_cmd else initial_cmd
                 cmd = " ".join(cmd)
 
                 logging.debug(f"cmd: {str(cmd)}")
@@ -263,14 +263,15 @@
         case False:
             recipe.update_trust_info()
 
     return recipe
 
 
 def main():
+    print("Hello World")
     args = setup_args()
     setup_logger(args.debug if args.debug else False)
     logging.info("Running autopkg_wrapper")
 
     override_repo_info = get_override_repo_info(args)
 
     post_processors_list = parse_post_processors(post_processors=args.post_processors)
```

### Comparing `autopkg_wrapper-2024.3.1/autopkg_wrapper/notifier/slack.py` & `autopkg_wrapper-2024.5.1/autopkg_wrapper/notifier/slack.py`

 * *Files identical despite different names*

### Comparing `autopkg_wrapper-2024.3.1/autopkg_wrapper/utils/args.py` & `autopkg_wrapper-2024.5.1/autopkg_wrapper/utils/args.py`

 * *Files identical despite different names*

### Comparing `autopkg_wrapper-2024.3.1/autopkg_wrapper/utils/git_functions.py` & `autopkg_wrapper-2024.5.1/autopkg_wrapper/utils/git_functions.py`

 * *Files identical despite different names*

### Comparing `autopkg_wrapper-2024.3.1/pyproject.toml` & `autopkg_wrapper-2024.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
     authors = ["James Smith <james@smithjw.me>"]
     description = "A package used to execute some autopkg functions, primarily within the context of a GitHub Actions runner."
     license = "BSD-3-Clause"
     name = "autopkg-wrapper"
     readme = "README.md"
     repository = "https://github.com/smithjw/autopkg-wrapper"
-    version = "2024.3.1"
+    version = "2024.5.1"
 
     [tool.poetry.scripts]
         # When built and installed by pip, the command autopkg_wrapper will be availble in to run within that environment
         autopkg-wrapper = "autopkg_wrapper.autopkg_wrapper:main"
         autopkg_wrapper = "autopkg_wrapper.autopkg_wrapper:main"
 
     [tool.poetry.dependencies]
         chardet = "5.2.0"
-        idna = "3.6"
-        pygithub = "2.2.0"
+        idna = "3.7"
+        pygithub = "2.3.0"
         python = "^3.12"
         requests = "2.31.0"
         ruamel-yaml = "0.18.6"
         toml = "0.10.2"
         urllib3 = "2.2.1"
 
     [tool.poetry_bumpversion.file."autopkg_wrapper/__init__.py"]
```

### Comparing `autopkg_wrapper-2024.3.1/PKG-INFO` & `autopkg_wrapper-2024.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: autopkg-wrapper
-Version: 2024.3.1
+Version: 2024.5.1
 Summary: A package used to execute some autopkg functions, primarily within the context of a GitHub Actions runner.
 Home-page: https://github.com/smithjw/autopkg-wrapper
 License: BSD-3-Clause
 Author: James Smith
 Author-email: james@smithjw.me
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: chardet (==5.2.0)
-Requires-Dist: idna (==3.6)
-Requires-Dist: pygithub (==2.2.0)
+Requires-Dist: idna (==3.7)
+Requires-Dist: pygithub (==2.3.0)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: ruamel-yaml (==0.18.6)
 Requires-Dist: toml (==0.10.2)
 Requires-Dist: urllib3 (==2.2.1)
 Project-URL: Repository, https://github.com/smithjw/autopkg-wrapper
 Description-Content-Type: text/markdown
```

