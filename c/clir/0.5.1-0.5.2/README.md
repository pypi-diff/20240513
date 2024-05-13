# Comparing `tmp/clir-0.5.1.tar.gz` & `tmp/clir-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clir-0.5.1.tar", max compression
+gzip compressed data, was "clir-0.5.2.tar", max compression
```

## Comparing `clir-0.5.1.tar` & `clir-0.5.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2024-05-09 17:50:23.573456 clir-0.5.1/LICENSE
--rw-r--r--   0        0        0      751 2024-05-09 17:50:23.573456 clir-0.5.1/README.md
--rw-r--r--   0        0        0        0 2024-05-09 17:50:23.573456 clir-0.5.1/clir/__init__.py
--rw-r--r--   0        0        0     3145 2024-05-09 17:50:23.573456 clir-0.5.1/clir/cli.py
--rw-r--r--   0        0        0     9324 2024-05-09 17:50:23.573456 clir-0.5.1/clir/command.py
--rw-r--r--   0        0        0      668 2024-05-09 17:50:23.577456 clir-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1690 1970-01-01 00:00:00.000000 clir-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-13 16:03:02.901090 clir-0.5.2/LICENSE
+-rw-r--r--   0        0        0      751 2024-05-13 16:03:02.901090 clir-0.5.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-13 16:03:02.901090 clir-0.5.2/clir/__init__.py
+-rw-r--r--   0        0        0     3145 2024-05-13 16:03:02.901090 clir-0.5.2/clir/cli.py
+-rw-r--r--   0        0        0     9355 2024-05-13 16:03:02.901090 clir-0.5.2/clir/command.py
+-rw-r--r--   0        0        0      668 2024-05-13 16:03:02.905090 clir-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1690 1970-01-01 00:00:00.000000 clir-0.5.2/PKG-INFO
```

### Comparing `clir-0.5.1/LICENSE` & `clir-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clir-0.5.1/README.md` & `clir-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `clir-0.5.1/clir/cli.py` & `clir-0.5.2/clir/cli.py`

 * *Files identical despite different names*

### Comparing `clir-0.5.1/clir/command.py` & `clir-0.5.2/clir/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,15 @@
         for c in current_commands:
             if current_commands[c]["uid"] == uid:
                 command = c
         
         command = _replace_arguments(command)
         if uid and command:
             print(f'[bold green]Running command:[/bold green] {command}')
+            os.system(command)
             subprocess.Popen(['bash', '-ic', 'set -o history; history -s "$1"', '_', command])
     
     def copy_command(self):
         current_commands = self.commands
 
         uid = self.get_command_uid()
```

### Comparing `clir-0.5.1/pyproject.toml` & `clir-0.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clir"
-version = "0.5.1"
+version = "0.5.2"
 description = "A clear and fast way to store and recover your commands"
 authors = ["Elkin Aguas <elkinaguas@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/elkinaguas/clir"
 repository = "https://github.com/elkinaguas/clir"
```

### Comparing `clir-0.5.1/PKG-INFO` & `clir-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clir
-Version: 0.5.1
+Version: 0.5.2
 Summary: A clear and fast way to store and recover your commands
 Home-page: https://github.com/elkinaguas/clir
 License: MIT
 Author: Elkin Aguas
 Author-email: elkinaguas@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

