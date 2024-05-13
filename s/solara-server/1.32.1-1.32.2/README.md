# Comparing `tmp/solara_server-1.32.1.tar.gz` & `tmp/solara_server-1.32.2.tar.gz`

## Comparing `solara_server-1.32.1.tar` & `solara_server-1.32.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 solara_server-1.32.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 solara_server-1.32.1/LICENSE
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 solara_server-1.32.1/README.md
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 solara_server-1.32.1/pyproject.toml
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 solara_server-1.32.1/PKG-INFO
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 solara_server-1.32.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 solara_server-1.32.2/LICENSE
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 solara_server-1.32.2/README.md
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 solara_server-1.32.2/pyproject.toml
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 solara_server-1.32.2/PKG-INFO
```

### Comparing `solara_server-1.32.1/.gitignore` & `solara_server-1.32.2/.gitignore`

 * *Files identical despite different names*

### Comparing `solara_server-1.32.1/LICENSE` & `solara_server-1.32.2/LICENSE`

 * *Files identical despite different names*

### Comparing `solara_server-1.32.1/pyproject.toml` & `solara_server-1.32.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [project]
 name = "solara-server"
 readme = "README.md"
 authors = [{name = "Maarten A. Breddels", email = "maartenbreddels@gmail.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
-version = "1.32.1"
+version = "1.32.2"
 dynamic = ["description"]
 dependencies = [
     "solara-ui",
     "jinja2",
     "click>=7.1.0",
     "rich_click",
     "filelock",
```

### Comparing `solara_server-1.32.1/PKG-INFO` & `solara_server-1.32.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: solara-server
-Version: 1.32.1
+Version: 1.32.2
 Dynamic: Summary
 Project-URL: Home, https://www.github.com/widgetti/solara
 Project-URL: Documentation, https://solara.dev
 Author-email: "Maarten A. Breddels" <maartenbreddels@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2022 Maarten A. Breddels
```

