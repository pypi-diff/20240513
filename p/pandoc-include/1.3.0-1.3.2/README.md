# Comparing `tmp/pandoc-include-1.3.0.tar.gz` & `tmp/pandoc_include-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandoc-include-1.3.0.tar", last modified: Sat Feb 10 19:21:47 2024, max compression
+gzip compressed data, was "pandoc_include-1.3.2.tar", last modified: Mon May 13 21:31:58 2024, max compression
```

## Comparing `pandoc-include-1.3.0.tar` & `pandoc_include-1.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 19:21:47.111504 pandoc-include-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-10 19:21:35.000000 pandoc-include-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10677 2024-02-10 19:21:47.111504 pandoc-include-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10113 2024-02-10 19:21:35.000000 pandoc-include-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 19:21:47.111504 pandoc-include-1.3.0/pandoc_include/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-10 19:21:35.000000 pandoc-include-1.3.0/pandoc_include/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-02-10 19:21:35.000000 pandoc-include-1.3.0/pandoc_include/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-02-10 19:21:35.000000 pandoc-include-1.3.0/pandoc_include/format_heuristics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12743 2024-02-10 19:21:35.000000 pandoc-include-1.3.0/pandoc_include/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 19:21:47.111504 pandoc-include-1.3.0/pandoc_include.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10677 2024-02-10 19:21:47.000000 pandoc-include-1.3.0/pandoc_include.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-02-10 19:21:47.000000 pandoc-include-1.3.0/pandoc_include.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-10 19:21:47.000000 pandoc-include-1.3.0/pandoc_include.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-10 19:21:47.000000 pandoc-include-1.3.0/pandoc_include.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-10 19:21:47.000000 pandoc-include-1.3.0/pandoc_include.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-10 19:21:47.000000 pandoc-include-1.3.0/pandoc_include.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-10 19:21:47.111504 pandoc-include-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-10 19:21:35.000000 pandoc-include-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:31:58.228365 pandoc_include-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-13 21:31:51.000000 pandoc_include-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-05-13 21:31:58.228365 pandoc_include-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-05-13 21:31:51.000000 pandoc_include-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:31:58.228365 pandoc_include-1.3.2/pandoc_include/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:31:51.000000 pandoc_include-1.3.2/pandoc_include/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-13 21:31:51.000000 pandoc_include-1.3.2/pandoc_include/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-13 21:31:51.000000 pandoc_include-1.3.2/pandoc_include/format_heuristics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12847 2024-05-13 21:31:51.000000 pandoc_include-1.3.2/pandoc_include/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:31:58.228365 pandoc_include-1.3.2/pandoc_include.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-05-13 21:31:58.000000 pandoc_include-1.3.2/pandoc_include.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-13 21:31:58.000000 pandoc_include-1.3.2/pandoc_include.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 21:31:58.000000 pandoc_include-1.3.2/pandoc_include.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-13 21:31:58.000000 pandoc_include-1.3.2/pandoc_include.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-13 21:31:58.000000 pandoc_include-1.3.2/pandoc_include.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 21:31:58.000000 pandoc_include-1.3.2/pandoc_include.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 21:31:58.232365 pandoc_include-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-13 21:31:51.000000 pandoc_include-1.3.2/setup.py
```

### Comparing `pandoc-include-1.3.0/LICENSE` & `pandoc_include-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pandoc-include-1.3.0/PKG-INFO` & `pandoc_include-1.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandoc-include
-Version: 1.3.0
+Version: 1.3.2
 Summary: Pandoc filter to allow file and header includes
 Home-page: https://github.com/DCsunset/pandoc-include
 Author: DCsunset
 Author-email: DCsunset@protonmail.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -39,42 +39,52 @@
 * Yaml header Merging:
 When an included file has its header, it will be merged into the current header.
 If there's a conflict, the original header of the current file remains.
 * Header include: Use `!include-header file.yaml` to include Yaml header from file.
 
 ## TODO
 
-- [] Write options to a tmp file and pass the filename by environment variable
+- [ ] Write options to a tmp file and pass the filename by environment variable
 
 ## Installation
 
-pandoc-include requires [python](https://www.python.org/) and [pip](https://pip.pypa.io/en/stable/installing/).
+### Using pip
 
-Then, use pip to install:
+To install the latest published version:
 
 ```
 pip install --user pandoc-include
 ```
 
-After installation,
-make sure that the `pandoc-include` executable is put in the directory which is in **the PATH environment**.
 
 To install the current (development) version hosted on the repository, use
 
 ```
 pip install --upgrade --force --no-cache git+https://github.com/DCsunset/pandoc-include
 ```
 
-You can use
+To check the version currently installed:
 
 ```
 pip show pandoc-include
 ```
 
-to check the version currently installed.
+### Using Nix
+
+`pandoc-include` is included in the Nixpkgs.
+Simply add the package to your NixOS config or use the following command:
+
+```sh
+# install in your profile
+nix-env -iA nixpkgs.pandoc-include
+
+# Or use it temporarily in a shell
+nix-shell -p pandoc-include
+```
+
 
 ## Usage
 
 **Note**: you should use `pandoc` with version greater than or equal to `2.17`,
 which is the minimum version that is tested.
 
 ### Command
@@ -386,22 +396,38 @@
 ## Development
 
 To setup local dev environment, you can use python `venv` to create a virtual environment from `requirements.txt`.
 
 Or if you use Nix, you can simply run `nix develop`.
 
 
+## Contributing
+
+Contributions are welcome if you find any bugs or want to add some features.
+Please open an issue for discussion first if it's a big change (e.g. a new feature) or if you are uncertain about it.
+
+Please follow [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)
+for your commit messages so that the changelog can be generated automatically.
+
+
 ## Trouble Shooting
 
+### Command-line options
+
 The pandoc command-line options are processed in order.
 If you want some options to be applied in included files,
 make sure the `--filter pandoc-include` option is specified before those options.
 
 For example, use bibliography in the included files:
 
 ```
 pandoc main.md --filter pandoc-include --citeproc --bibliography=ref.bib -o main.pdf
 ```
 
+### Executable not found
+
+For some operating systems, the path may not be set correctly after installation.
+Make sure that the `pandoc-include` executable is put in the directory which is in **the PATH environment**.
+
 ## License
 
 MIT License
```

### Comparing `pandoc-include-1.3.0/README.md` & `pandoc_include-1.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -21,42 +21,52 @@
 * Yaml header Merging:
 When an included file has its header, it will be merged into the current header.
 If there's a conflict, the original header of the current file remains.
 * Header include: Use `!include-header file.yaml` to include Yaml header from file.
 
 ## TODO
 
-- [] Write options to a tmp file and pass the filename by environment variable
+- [ ] Write options to a tmp file and pass the filename by environment variable
 
 ## Installation
 
-pandoc-include requires [python](https://www.python.org/) and [pip](https://pip.pypa.io/en/stable/installing/).
+### Using pip
 
-Then, use pip to install:
+To install the latest published version:
 
 ```
 pip install --user pandoc-include
 ```
 
-After installation,
-make sure that the `pandoc-include` executable is put in the directory which is in **the PATH environment**.
 
 To install the current (development) version hosted on the repository, use
 
 ```
 pip install --upgrade --force --no-cache git+https://github.com/DCsunset/pandoc-include
 ```
 
-You can use
+To check the version currently installed:
 
 ```
 pip show pandoc-include
 ```
 
-to check the version currently installed.
+### Using Nix
+
+`pandoc-include` is included in the Nixpkgs.
+Simply add the package to your NixOS config or use the following command:
+
+```sh
+# install in your profile
+nix-env -iA nixpkgs.pandoc-include
+
+# Or use it temporarily in a shell
+nix-shell -p pandoc-include
+```
+
 
 ## Usage
 
 **Note**: you should use `pandoc` with version greater than or equal to `2.17`,
 which is the minimum version that is tested.
 
 ### Command
@@ -368,22 +378,38 @@
 ## Development
 
 To setup local dev environment, you can use python `venv` to create a virtual environment from `requirements.txt`.
 
 Or if you use Nix, you can simply run `nix develop`.
 
 
+## Contributing
+
+Contributions are welcome if you find any bugs or want to add some features.
+Please open an issue for discussion first if it's a big change (e.g. a new feature) or if you are uncertain about it.
+
+Please follow [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)
+for your commit messages so that the changelog can be generated automatically.
+
+
 ## Trouble Shooting
 
+### Command-line options
+
 The pandoc command-line options are processed in order.
 If you want some options to be applied in included files,
 make sure the `--filter pandoc-include` option is specified before those options.
 
 For example, use bibliography in the included files:
 
 ```
 pandoc main.md --filter pandoc-include --citeproc --bibliography=ref.bib -o main.pdf
 ```
 
+### Executable not found
+
+For some operating systems, the path may not be set correctly after installation.
+Make sure that the `pandoc-include` executable is put in the directory which is in **the PATH environment**.
+
 ## License
 
 MIT License
```

### Comparing `pandoc-include-1.3.0/pandoc_include/config.py` & `pandoc_include-1.3.2/pandoc_include/config.py`

 * *Files identical despite different names*

### Comparing `pandoc-include-1.3.0/pandoc_include/format_heuristics.py` & `pandoc_include-1.3.2/pandoc_include/format_heuristics.py`

 * *Files identical despite different names*

### Comparing `pandoc-include-1.3.0/pandoc_include/main.py` & `pandoc_include-1.3.2/pandoc_include/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 
     includeType = INCLUDE_INVALID
     config = {}
     filename = None
 
     # wildcards '*' are escaped which needs to be undone because of path globing
     # convert_text has a tendency to produce multiline text which can not be matched correctly
-    rawString = rawString.replace('\\*', '*').replace('\n', ' ')
+    # Also here we should unescape underscores from markdown_strict.
+    rawString = rawString.replace('\\*', '*').replace('\n', ' ').replace('\\_', '_')
 
     if re.match(RE_IS_INCLUDE_HEADER, rawString):
         includeType = INCLUDE_HEADER
     else:
         includeType = INCLUDE_FILE
 
     matches = re.match(RE_INCLUDE_PATTERN, rawString)
@@ -125,36 +126,49 @@
         return s[min(pos, num):]
 
 def dedent(content: str, num):
     lines = content.split("\n")
     return list(map(lambda s: removeLeadingWhitespaces(s, num), lines))
 
 
+def findFile(filename: str):
+    resource_paths = options['include-resources'].split(':')
+
+    files = glob.glob(filename, recursive=True)
+    if len(files) == 0 and resource_paths:
+        for resource_path in resource_paths:
+            if os.path.isabs(resource_path):
+                files += glob.glob(os.path.normpath(os.path.join(resource_path, filename)), recursive=True)
+            else:
+                files += glob.glob(os.path.normpath(os.path.join(options['process-path'], resource_path, filename)), recursive=True)
+
+    return files
+
+
 def read_file(filename, config: dict):
     with open(filename, encoding="utf-8") as f:
         content = f.read()
 
     if "xslt" in config:
         xsltParam = config.get("xslt", None)
 
         if not xsltParam:
             raise ValueError(f"Invalid value for xsl file: '{xsltParam}'")
 
-        xslTransformerFile = glob.glob(xsltParam, recursive=True)
-
+        xslTransformerFile = findFile(xsltParam)
         if len(xslTransformerFile) == 0:
             raise ValueError(f"xsl transformer file not found: '{xsltParam}'")
         elif len(xslTransformerFile) > 1:
             raise ValueError(f"Ambiguous xsl transformer file: '{xsltParam}'")
         else:
             xslTransformerFile = xslTransformerFile[0]
 
         pf.debug(f"[INFO] xslt transform {filename} with {xslTransformerFile}")
 
-        dom = xml.parse(filename)
+        dom = xml.parse(filename, xml.XMLParser(recover=True))
 
         xslt = xml.parse(xslTransformerFile)
         if not xslt:
             raise IOError("Unable to read XSLT file '{xslt}'")
         transform = xml.XSLT(xslt)
         transformedDom = transform(dom)
 
@@ -245,24 +259,15 @@
     # --- Include statement ---
     if isinstance(elem, pf.Para):
         includeType, name, config = is_include_line(elem)
 
         if includeType == INCLUDE_INVALID:
             return
 
-        resource_paths = options['include-resources'].split(':')
-
-        # Enable shell-style wildcards
-        files = glob.glob(name, recursive=True)
-        if len(files) == 0 and resource_paths:
-            for resource_path in resource_paths:
-                if os.path.isabs(resource_path):
-                    files += glob.glob(os.path.normpath(os.path.join(resource_path, name)), recursive=True)
-                else:
-                    files += glob.glob(os.path.normpath(os.path.join(options['process-path'], resource_path, name)), recursive=True)
+        files = findFile(name)
         if len(files) == 0:
             msg = f"Included file not found: {name}"
             if Env.NotFoundError:
                 raise IOError(msg)
             else:
                 pf.debug(f"[WARNING] {msg}")
                 return
@@ -369,15 +374,15 @@
     # --- Code Blocks ---
     elif isinstance(elem, pf.CodeBlock):
         includeType, name, config = is_code_include(elem)
         if includeType == 0:
             return
 
         # Enable shell-style wildcards
-        files = glob.glob(name, recursive=True)
+        files = findFile(name)
         if len(files) == 0:
             msg = f"Included file not found: {name}"
             if Env.NotFoundError:
                 raise IOError(msg)
             else:
                 pf.debug(f"[WARNING] {msg}")
                 return
```

### Comparing `pandoc-include-1.3.0/pandoc_include.egg-info/PKG-INFO` & `pandoc_include-1.3.2/pandoc_include.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandoc-include
-Version: 1.3.0
+Version: 1.3.2
 Summary: Pandoc filter to allow file and header includes
 Home-page: https://github.com/DCsunset/pandoc-include
 Author: DCsunset
 Author-email: DCsunset@protonmail.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -39,42 +39,52 @@
 * Yaml header Merging:
 When an included file has its header, it will be merged into the current header.
 If there's a conflict, the original header of the current file remains.
 * Header include: Use `!include-header file.yaml` to include Yaml header from file.
 
 ## TODO
 
-- [] Write options to a tmp file and pass the filename by environment variable
+- [ ] Write options to a tmp file and pass the filename by environment variable
 
 ## Installation
 
-pandoc-include requires [python](https://www.python.org/) and [pip](https://pip.pypa.io/en/stable/installing/).
+### Using pip
 
-Then, use pip to install:
+To install the latest published version:
 
 ```
 pip install --user pandoc-include
 ```
 
-After installation,
-make sure that the `pandoc-include` executable is put in the directory which is in **the PATH environment**.
 
 To install the current (development) version hosted on the repository, use
 
 ```
 pip install --upgrade --force --no-cache git+https://github.com/DCsunset/pandoc-include
 ```
 
-You can use
+To check the version currently installed:
 
 ```
 pip show pandoc-include
 ```
 
-to check the version currently installed.
+### Using Nix
+
+`pandoc-include` is included in the Nixpkgs.
+Simply add the package to your NixOS config or use the following command:
+
+```sh
+# install in your profile
+nix-env -iA nixpkgs.pandoc-include
+
+# Or use it temporarily in a shell
+nix-shell -p pandoc-include
+```
+
 
 ## Usage
 
 **Note**: you should use `pandoc` with version greater than or equal to `2.17`,
 which is the minimum version that is tested.
 
 ### Command
@@ -386,22 +396,38 @@
 ## Development
 
 To setup local dev environment, you can use python `venv` to create a virtual environment from `requirements.txt`.
 
 Or if you use Nix, you can simply run `nix develop`.
 
 
+## Contributing
+
+Contributions are welcome if you find any bugs or want to add some features.
+Please open an issue for discussion first if it's a big change (e.g. a new feature) or if you are uncertain about it.
+
+Please follow [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)
+for your commit messages so that the changelog can be generated automatically.
+
+
 ## Trouble Shooting
 
+### Command-line options
+
 The pandoc command-line options are processed in order.
 If you want some options to be applied in included files,
 make sure the `--filter pandoc-include` option is specified before those options.
 
 For example, use bibliography in the included files:
 
 ```
 pandoc main.md --filter pandoc-include --citeproc --bibliography=ref.bib -o main.pdf
 ```
 
+### Executable not found
+
+For some operating systems, the path may not be set correctly after installation.
+Make sure that the `pandoc-include` executable is put in the directory which is in **the PATH environment**.
+
 ## License
 
 MIT License
```

### Comparing `pandoc-include-1.3.0/setup.py` & `pandoc_include-1.3.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 from os import path
 
-version = '1.3.0'
+version = '1.3.2'
 
 repo_base_dir = path.abspath(path.dirname(__file__))
 
 # Long description
 readme = path.join(repo_base_dir, 'README.md')
 with open(readme) as f:
     long_description = f.read()
```

