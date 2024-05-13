# Comparing `tmp/wizlib-2.0.9.tar.gz` & `tmp/wizlib-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizlib-2.0.9.tar", max compression
+gzip compressed data, was "wizlib-3.0.0.tar", max compression
```

## Comparing `wizlib-2.0.9.tar` & `wizlib-3.0.0.tar`

### file list

```diff
@@ -1,14 +1,20 @@
--rw-r--r--   0        0        0     5320 2023-11-26 21:00:11.298215 wizlib-2.0.9/README.md
--rw-r--r--   0        0        0      696 2023-11-26 21:00:27.610307 wizlib-2.0.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-26 21:00:11.325215 wizlib-2.0.9/wizlib/__init__.py
--rw-r--r--   0        0        0     2794 2023-11-26 21:00:11.299215 wizlib-2.0.9/wizlib/app.py
--rw-r--r--   0        0        0     4424 2023-11-26 21:00:11.299215 wizlib-2.0.9/wizlib/class_family.py
--rw-r--r--   0        0        0     1304 2023-11-26 21:00:11.299215 wizlib-2.0.9/wizlib/command.py
--rw-r--r--   0        0        0     2639 2023-11-26 21:00:11.299215 wizlib-2.0.9/wizlib/config_handler.py
--rw-r--r--   0        0        0       46 2023-11-26 21:00:11.299215 wizlib-2.0.9/wizlib/error.py
--rw-r--r--   0        0        0      306 2023-11-26 21:00:11.299215 wizlib-2.0.9/wizlib/handler.py
--rw-r--r--   0        0        0      597 2023-11-26 21:00:11.299215 wizlib-2.0.9/wizlib/input_handler.py
--rw-r--r--   0        0        0     1505 2023-11-26 21:00:11.299215 wizlib-2.0.9/wizlib/parser.py
--rw-r--r--   0        0        0     1754 2023-11-26 21:00:11.299215 wizlib-2.0.9/wizlib/rlinput.py
--rw-r--r--   0        0        0      272 2023-11-26 21:00:11.299215 wizlib-2.0.9/wizlib/super_wrapper.py
--rw-r--r--   0        0        0     5921 1970-01-01 00:00:00.000000 wizlib-2.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-05-13 05:49:36.321921 wizlib-3.0.0/README.md
+-rw-r--r--   0        0        0      698 2024-05-13 05:49:48.180954 wizlib-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-13 05:49:36.413921 wizlib-3.0.0/wizlib/__init__.py
+-rw-r--r--   0        0        0     3263 2024-05-13 05:49:36.360921 wizlib-3.0.0/wizlib/app.py
+-rw-r--r--   0        0        0     4506 2024-05-13 05:49:36.360921 wizlib-3.0.0/wizlib/class_family.py
+-rw-r--r--   0        0        0     1686 2024-05-13 05:49:36.360921 wizlib-3.0.0/wizlib/command.py
+-rw-r--r--   0        0        0     2588 2024-05-13 05:49:36.360921 wizlib-3.0.0/wizlib/config_handler.py
+-rw-r--r--   0        0        0       46 2024-05-13 05:49:36.361921 wizlib-3.0.0/wizlib/error.py
+-rw-r--r--   0        0        0      446 2024-05-13 05:49:36.361921 wizlib-3.0.0/wizlib/handler.py
+-rw-r--r--   0        0        0     1505 2024-05-13 05:49:36.361921 wizlib-3.0.0/wizlib/parser.py
+-rw-r--r--   0        0        0     1754 2024-05-13 05:49:36.361921 wizlib-3.0.0/wizlib/rlinput.py
+-rw-r--r--   0        0        0      663 2024-05-13 05:49:36.361921 wizlib-3.0.0/wizlib/stream_handler.py
+-rw-r--r--   0        0        0      272 2024-05-13 05:49:36.361921 wizlib-3.0.0/wizlib/super_wrapper.py
+-rw-r--r--   0        0        0     4249 2024-05-13 05:49:36.361921 wizlib-3.0.0/wizlib/ui/__init__.py
+-rw-r--r--   0        0        0      943 2024-05-13 05:49:36.361921 wizlib-3.0.0/wizlib/ui/shell/__init__.py
+-rw-r--r--   0        0        0     7419 2024-05-13 05:49:36.361921 wizlib-3.0.0/wizlib/ui/shell/line_editor.py
+-rw-r--r--   0        0        0     2030 2024-05-13 05:49:36.361921 wizlib-3.0.0/wizlib/ui/shell_ui.py
+-rw-r--r--   0        0        0      634 2024-05-13 05:49:36.361921 wizlib-3.0.0/wizlib/ui_handler.py
+-rw-r--r--   0        0        0      156 2024-05-13 05:49:36.361921 wizlib-3.0.0/wizlib/util.py
+-rw-r--r--   0        0        0     1780 1970-01-01 00:00:00.000000 wizlib-3.0.0/PKG-INFO
```

### Comparing `wizlib-2.0.9/pyproject.toml` & `wizlib-3.0.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 [tool.poetry]
 name = "wizlib"
-version = "2.0.9"
+version = "3.0.0"
 description = "Framework for flexible and powerful command-line applications"
 authors = ["Steampunk Wizard <wizlib@steampunkwizard.ca>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 PyYAML = "^6.0.1"
 pyreadline3 = { version="^3.4.1", markers="sys_platform=='win32'" }
 gnureadline = { version="^8.1.2", markers="sys_platform=='darwin'" }
+myst-parser = "^2.0.0"
+readchar = "^4.0.5"
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.3.1"
 pycodestyle = "^2.11.0"
 autopep8 = "^2.0.4"
+pelican = "^4.9.1"
+markdown = "^3.5.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
-
-[tool.poetry-dynamic-versioning]
-enable = false
-vcs = "git"
-format = "{base}"
-
```

### Comparing `wizlib-2.0.9/wizlib/app.py` & `wizlib-3.0.0/wizlib/app.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,82 +3,96 @@
 import os
 from pathlib import Path
 
 from wizlib.class_family import ClassFamily
 from wizlib.command import WizHelpCommand
 from wizlib.super_wrapper import SuperWrapper
 from wizlib.parser import WizParser
+from wizlib.ui import UI
 
 
 RED = '\033[91m'
 RESET = '\033[0m'
 
 
+class AppCancellation(BaseException):
+    pass
+
+
 class WizApp:
     """Root of all WizLib-based CLI applications. Subclass it. Can be
     instantiated and then run multiple commands."""
 
     base_command = None
     name = ''
 
+    # Set some default types so linting works
+    ui: UI
+
     @classmethod
     def main(cls):  # pragma: nocover
         """Call this from a __main__ entrypoint"""
-        cls.run(*sys.argv[1:], debug=os.getenv('DEBUG'))
+        cls.start(*sys.argv[1:], debug=os.getenv('DEBUG'))
 
     @classmethod
-    def run(cls, *args, debug=False):
+    def start(cls, *args, debug=False):
         """Call this from a Python entrypoint"""
         try:
-            cls.initialize()
-            app = cls(*args)
-            # if app.ready:
-            command = app.first_command
-            result = command.execute()
-            if result:
-                print(result, file=sys.stdout, end='')
-                if sys.stdout.isatty():  # pragma: nocover
-                    print()
-            if command.status:
-                print(command.status, file=sys.stderr)
-        except Exception as error:
+            parser = WizParser(prog=cls.name)
+            for handler in cls.base_command.handlers:
+                handler.add_args(parser)
+            ns, more = parser.parse_known_args(args)
+            app = cls.initialize(**vars(ns))
+            more = more if more else [cls.base_command.default]
+            app.run(*more)
+        except AppCancellation as cancellation:
+            if str(cancellation):
+                print(str(cancellation), file=sys.stderr)
+        except BaseException as error:
             if debug:
                 raise error
             else:
-                print(f"\n{RED}{type(error).__name__}: " +
-                      f"{error}{RESET}\n", file=sys.stderr)
+                name = type(error).__name__
+                print(f"\n{RED}{name}{': ' if str(error) else ''}" +
+                      f"{error}{RESET}", file=sys.stderr)
+                sys.exit(1)
 
     @classmethod
-    def initialize(cls):
-        """Set up the app class to parse arguments"""
-        cls.parser = WizParser(
-            prog=cls.name,
-            exit_on_error=False)
+    def initialize(cls, **vals):
+        """Converts argparse values (strings) into actual handlers and
+        instantiates the app"""
+        handlers = {}
         for handler in cls.base_command.handlers:
-            cls.parser.add_argument(
-                f"--{handler.name}",
-                f"-{handler.name[0]}",
-                type=handler.named(cls.name),
-                default='')
-        subparsers = cls.parser.add_subparsers(dest='command')
-        for command in cls.base_command.family_members('name'):
+            val = vals[handler.name] if (
+                handler.name in vals) else handler.default
+            handlers[handler.name] = handler.setup(val)
+        return cls(**handlers)
+
+    def __init__(self, **handlers):
+        for name, handler in handlers.items():
+            handler.app = self
+            setattr(self, name, handler)
+        self.parser = WizParser()
+        subparsers = self.parser.add_subparsers(dest='command')
+        for command in self.base_command.family_members('name'):
             key = command.get_member_attr('key')
             aliases = [key] if key else []
             subparser = subparsers.add_parser(command.name, aliases=aliases)
             command.add_args(subparser)
 
-    def __init__(self, *args):
-        args = args if args else [self.base_command.default]
-        self.vals = vars(self.parser.parse_args(args))
-        self.first_command = self.get_command(**self.vals)
-
-    def get_command(self, **vals):
-        """Run a single command"""
+    def run(self, *args):
+        vals = vars(self.parser.parse_args(args))
         if 'help' in vals:
             return WizHelpCommand(**vals)
-        else:
-            command_name = vals.pop('command')
-            command_class = self.base_command.family_member(
-                'name', command_name)
-            if not command_class:
-                raise Exception(f"Unknown command {command_name}")
-            return command_class(**vals)
+        command_name = vals.pop('command')
+        command_class = self.base_command.family_member(
+            'name', command_name)
+        if not command_class:
+            raise Exception(f"Unknown command {command_name}")
+        command = command_class(self, **vals)
+        result = command.execute()
+        if result:
+            print(result, end='')
+            if sys.stdout.isatty():  # pragma: nocover
+                print()
+        if command.status:
+            print(command.status, file=sys.stderr)
```

### Comparing `wizlib-2.0.9/wizlib/class_family.py` & `wizlib-3.0.0/wizlib/class_family.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,18 +44,19 @@
             # Call the same function on each subclass
             hits |= kid.family_members(*attributes)
 
         # Send it back
         return hits
 
     @classmethod
-    def family_attrs(self, attribute):
+    def family_attrs(self, attribute):  # pragma: nocover
         """
         Return a set of all the values of a specific attribute that exist in
-        the family. The set avoids repetition of values in the result.
+        the family. The set avoids repetition of values in the result. This is
+        a legacy method, not currently tested or used.
         """
         # Put myself into a set if I qualify
         if self.has_member_attrs(attribute):
             values = {self.get_member_attr(attribute)}
         else:
             values = set()
```

### Comparing `wizlib-2.0.9/wizlib/config_handler.py` & `wizlib-3.0.0/wizlib/config_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,43 +5,44 @@
 from unittest.mock import patch
 
 from yaml import load
 from yaml import Loader
 from wizlib.handler import Handler
 
 from wizlib.error import ConfigHandlerError
+from wizlib.parser import WizParser
 
 
 class ConfigHandler(Handler):
     """
     Handle app-level configuration, where settings could come from specific
     settings (such as from argparse), environment variables, or a YAML file.
     Within the Python code, config keys are underscore-separated all-lower.
 
     A ConfigHandler returns null in the case of a missing value, assuming that
     commands can handle their own null cases.
     """
 
     name = 'config'
 
-    def __init__(self, value=None):
-        self.file = value
+    def __init__(self, file=None):
+        self.file = file
         self.cache = {}
 
     @property
     def yaml(self):
         if hasattr(self, '_yaml'):
             return self._yaml
         path = None
         if self.file:
             path = Path(self.file)
-        elif self.appname:
-            localpath = Path.cwd() / f".{self.appname}.yml"
-            homepath = Path.home() / f".{self.appname}.yml"
-            if (envvar := self.env(self.appname + '-config')):
+        elif self.app and self.app.name:
+            localpath = Path.cwd() / f".{self.app.name}.yml"
+            homepath = Path.home() / f".{self.app.name}.yml"
+            if (envvar := self.env(self.app.name + '-config')):
                 path = Path(envvar)
             elif (localpath.is_file()):
                 path = localpath
             elif (homepath.is_file()):
                 path = homepath
         if path:
             with open(path) as file:
@@ -73,15 +74,10 @@
                 if not split:
                     self.cache[key] = yaml
                     return yaml
 
     @classmethod
     def fake(cls, **vals):
         """Return a fake ConfigHandler with forced values, for testing"""
-        handler = cls()
-
-        def fake_env(name):
-            key = name.replace('-', '_')
-            if key in vals:
-                return vals[key]
-        handler.env = fake_env
-        return handler
+        self = cls()
+        self.cache = {k.replace('_', '-'): vals[k] for k in vals}
+        return self
```

### Comparing `wizlib-2.0.9/wizlib/parser.py` & `wizlib-3.0.0/wizlib/parser.py`

 * *Files identical despite different names*

### Comparing `wizlib-2.0.9/wizlib/rlinput.py` & `wizlib-3.0.0/wizlib/rlinput.py`

 * *Files identical despite different names*

