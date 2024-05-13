# Comparing `tmp/manage_requirements_files-0.1.2.tar.gz` & `tmp/manage_requirements_files-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manage_requirements_files-0.1.2.tar", last modified: Mon May  6 21:22:52 2024, max compression
+gzip compressed data, was "manage_requirements_files-0.1.3.tar", last modified: Mon May 13 13:04:35 2024, max compression
```

## Comparing `manage_requirements_files-0.1.2.tar` & `manage_requirements_files-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,15 @@
-drwxrwxr-x   0 guilhermegouw  (1000) guilhermegouw  (1000)        0 2024-05-06 21:22:52.490938 manage_requirements_files-0.1.2/
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)     1070 2024-05-05 10:03:57.000000 manage_requirements_files-0.1.2/LICENSE
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)     3255 2024-05-06 21:22:52.490938 manage_requirements_files-0.1.2/PKG-INFO
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)     2707 2024-05-06 21:08:20.000000 manage_requirements_files-0.1.2/README.md
-drwxrwxr-x   0 guilhermegouw  (1000) guilhermegouw  (1000)        0 2024-05-06 21:22:52.486938 manage_requirements_files-0.1.2/manage_requirements_files/
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)        0 2024-05-05 10:03:57.000000 manage_requirements_files-0.1.2/manage_requirements_files/__init__.py
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)     2055 2024-05-06 21:08:30.000000 manage_requirements_files-0.1.2/manage_requirements_files/cli.py
-drwxrwxr-x   0 guilhermegouw  (1000) guilhermegouw  (1000)        0 2024-05-06 21:22:52.490938 manage_requirements_files-0.1.2/manage_requirements_files.egg-info/
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)     3255 2024-05-06 21:22:52.000000 manage_requirements_files-0.1.2/manage_requirements_files.egg-info/PKG-INFO
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)      381 2024-05-06 21:22:52.000000 manage_requirements_files-0.1.2/manage_requirements_files.egg-info/SOURCES.txt
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)        1 2024-05-06 21:22:52.000000 manage_requirements_files-0.1.2/manage_requirements_files.egg-info/dependency_links.txt
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)       76 2024-05-06 21:22:52.000000 manage_requirements_files-0.1.2/manage_requirements_files.egg-info/entry_points.txt
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)       32 2024-05-06 21:22:52.000000 manage_requirements_files-0.1.2/manage_requirements_files.egg-info/top_level.txt
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)       38 2024-05-06 21:22:52.490938 manage_requirements_files-0.1.2/setup.cfg
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)      829 2024-05-06 21:22:04.000000 manage_requirements_files-0.1.2/setup.py
-drwxrwxr-x   0 guilhermegouw  (1000) guilhermegouw  (1000)        0 2024-05-06 21:22:52.490938 manage_requirements_files-0.1.2/tests/
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)        0 2024-05-06 21:08:30.000000 manage_requirements_files-0.1.2/tests/__init__.py
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)     7293 2024-05-06 21:08:30.000000 manage_requirements_files-0.1.2/tests/test_cli.py
+drwxr-xr-x   0 guilherme.gouw   (503) staff       (20)        0 2024-05-13 13:04:35.035626 manage_requirements_files-0.1.3/
+-rw-r--r--   0 guilherme.gouw   (503) staff       (20)     1070 2024-05-06 20:13:57.000000 manage_requirements_files-0.1.3/LICENSE
+-rw-r--r--   0 guilherme.gouw   (503) staff       (20)     3235 2024-05-13 13:04:35.035114 manage_requirements_files-0.1.3/PKG-INFO
+-rw-r--r--   0 guilherme.gouw   (503) staff       (20)     2707 2024-05-06 20:13:57.000000 manage_requirements_files-0.1.3/README.md
+drwxr-xr-x   0 guilherme.gouw   (503) staff       (20)        0 2024-05-13 13:04:35.030966 manage_requirements_files-0.1.3/manage_requirements_files/
+-rw-r--r--   0 guilherme.gouw   (503) staff       (20)        0 2024-05-06 20:13:57.000000 manage_requirements_files-0.1.3/manage_requirements_files/__init__.py
+-rw-r--r--   0 guilherme.gouw   (503) staff       (20)     2359 2024-05-13 12:31:43.000000 manage_requirements_files-0.1.3/manage_requirements_files/cli.py
+drwxr-xr-x   0 guilherme.gouw   (503) staff       (20)        0 2024-05-13 13:04:35.034332 manage_requirements_files-0.1.3/manage_requirements_files.egg-info/
+-rw-r--r--   0 guilherme.gouw   (503) staff       (20)     3235 2024-05-13 13:04:35.000000 manage_requirements_files-0.1.3/manage_requirements_files.egg-info/PKG-INFO
+-rw-r--r--   0 guilherme.gouw   (503) staff       (20)      345 2024-05-13 13:04:35.000000 manage_requirements_files-0.1.3/manage_requirements_files.egg-info/SOURCES.txt
+-rw-r--r--   0 guilherme.gouw   (503) staff       (20)        1 2024-05-13 13:04:35.000000 manage_requirements_files-0.1.3/manage_requirements_files.egg-info/dependency_links.txt
+-rw-r--r--   0 guilherme.gouw   (503) staff       (20)       75 2024-05-13 13:04:35.000000 manage_requirements_files-0.1.3/manage_requirements_files.egg-info/entry_points.txt
+-rw-r--r--   0 guilherme.gouw   (503) staff       (20)       26 2024-05-13 13:04:35.000000 manage_requirements_files-0.1.3/manage_requirements_files.egg-info/top_level.txt
+-rw-r--r--   0 guilherme.gouw   (503) staff       (20)       38 2024-05-13 13:04:35.035728 manage_requirements_files-0.1.3/setup.cfg
+-rw-r--r--   0 guilherme.gouw   (503) staff       (20)      829 2024-05-13 13:03:18.000000 manage_requirements_files-0.1.3/setup.py
```

### Comparing `manage_requirements_files-0.1.2/LICENSE` & `manage_requirements_files-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `manage_requirements_files-0.1.2/PKG-INFO` & `manage_requirements_files-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: manage_requirements_files
-Version: 0.1.2
+Version: 0.1.3
 Summary: A utility to manage project dependencies for development and production.
 Home-page: https://github.com/guilhermegouw/manage-requirements-files
 Author: Guilherme Gouw
 Author-email: guilherme.gouw@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -85,9 +84,7 @@
 ## License
 
 Distributed under the MIT License. See LICENSE for more information.
 
 ## Contact
 
 Guilherme Gouw - guilherme.gouw@gmail.com
-
-
```

### Comparing `manage_requirements_files-0.1.2/README.md` & `manage_requirements_files-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `manage_requirements_files-0.1.2/manage_requirements_files/cli.py` & `manage_requirements_files-0.1.3/manage_requirements_files/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #!/usr/bin/env python
 import argparse
 import subprocess
 import sys
+import os
 
 
 def main():
-    parser = argparse.ArgumentParser(
-        description="Manage Python project dependencies."
-    )
+    parser = argparse.ArgumentParser(description="Manage Python project dependencies.")
     parser.add_argument(
         "mode",
         choices=["prod", "dev"],
         help="Update production or development dependencies.",
     )
 
     args = parser.parse_args()
@@ -20,19 +19,27 @@
         update_requirements("requirements.txt", "requirements-dev.txt")
     else:  # dev
         update_requirements("requirements-dev.txt", "requirements.txt")
 
 
 def pip_freeze():
     """Get the output of pip freeze as a set of package=version strings."""
-    return set(
-        subprocess.check_output(
-            [sys.executable, "-m", "pip", "freeze"], text=True
-        ).splitlines()
-    )
+    venv_path = os.environ.get("VIRTUAL_ENV")
+    if not venv_path:
+        print("No active virtual environment found.\nDid you forget to activate it?")
+        sys.exit(1)
+
+    pip_path = os.path.join(venv_path, "bin", "pip")
+
+    try:
+        output = subprocess.check_output([pip_path, "freeze"], text=True)
+        return set(output.splitlines())
+    except subprocess.CalledProcessError as e:
+        print("An error occurred while running pip freeze: ", e)
+        return set()
 
 
 def read_requirements(filename):
     """Read a requirements file and return its contents as a set,\
         automatically create if not exist."""
     try:
         with open(filename, "r") as file:
@@ -49,24 +56,20 @@
             file.write(f"{line}\n")
 
 
 def update_requirements(target_file, other_file):
     """Update the target requirements file with new dependencies,\
         automatically creating files if they don't exist."""
     current_packages = pip_freeze()
-    existing_deps = read_requirements(target_file) | read_requirements(
-        other_file
-    )
+    existing_deps = read_requirements(target_file) | read_requirements(other_file)
 
     new_dependencies = current_packages - existing_deps
 
     if new_dependencies:
         write_requirements(target_file, new_dependencies)
-        print(
-            f"Updated {target_file} with new dependencies: {new_dependencies}"
-        )
+        print(f"Updated {target_file} with new dependencies: {new_dependencies}")
     else:
         print(f"No new dependencies to add to {target_file}.")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `manage_requirements_files-0.1.2/manage_requirements_files.egg-info/PKG-INFO` & `manage_requirements_files-0.1.3/manage_requirements_files.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
-Name: manage-requirements-files
-Version: 0.1.2
+Name: manage_requirements_files
+Version: 0.1.3
 Summary: A utility to manage project dependencies for development and production.
 Home-page: https://github.com/guilhermegouw/manage-requirements-files
 Author: Guilherme Gouw
 Author-email: guilherme.gouw@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -85,9 +84,7 @@
 ## License
 
 Distributed under the MIT License. See LICENSE for more information.
 
 ## Contact
 
 Guilherme Gouw - guilherme.gouw@gmail.com
-
-
```

### Comparing `manage_requirements_files-0.1.2/setup.py` & `manage_requirements_files-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="manage_requirements_files",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "manage-dependencies=manage_requirements_files.cli:main",
         ],
     },
     author="Guilherme Gouw",
```

