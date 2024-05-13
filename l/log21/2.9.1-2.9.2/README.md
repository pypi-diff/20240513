# Comparing `tmp/log21-2.9.1.tar.gz` & `tmp/log21-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log21-2.9.1.tar", last modified: Fri Apr  5 21:28:25 2024, max compression
+gzip compressed data, was "log21-2.9.2.tar", last modified: Fri Apr 12 08:21:14 2024, max compression
```

## Comparing `log21-2.9.1.tar` & `log21-2.9.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:28:25.657975 log21-2.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-04-05 21:28:15.000000 log21-2.9.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-04-05 21:28:25.657975 log21-2.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-05 21:28:15.000000 log21-2.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-05 21:28:15.000000 log21-2.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 21:28:25.657975 log21-2.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:28:25.649975 log21-2.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:28:25.653975 log21-2.9.1/src/log21/
--rw-r--r--   0 runner    (1001) docker     (127)    47574 2024-04-05 21:28:15.000000 log21-2.9.1/src/log21/Argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    15229 2024-04-05 21:28:15.000000 log21-2.9.1/src/log21/Argumentify.py
--rw-r--r--   0 runner    (1001) docker     (127)    11796 2024-04-05 21:28:15.000000 log21-2.9.1/src/log21/Colors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:28:25.657975 log21-2.9.1/src/log21/CrashReporter/
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-05 21:28:15.000000 log21-2.9.1/src/log21/CrashReporter/Formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)    14913 2024-04-05 21:28:15.000000 log21-2.9.1/src/log21/CrashReporter/Reporters.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-05 21:28:15.000000 log21-2.9.1/src/log21/CrashReporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-05 21:28:15.000000 log21-2.9.1/src/log21/FileHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11632 2024-04-05 21:28:15.000000 log21-2.9.1/src/log21/Formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-05 21:28:15.000000 log21-2.9.1/src/log21/Levels.py
--rw-r--r--   0 runner    (1001) docker     (127)    14968 2024-04-05 21:28:15.000000 log21-2.9.1/src/log21/Logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    34385 2024-04-05 21:28:15.000000 log21-2.9.1/src/log21/LoggingWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-05 21:28:15.000000 log21-2.9.1/src/log21/Manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    28854 2024-04-05 21:28:15.000000 log21-2.9.1/src/log21/PPrint.py
--rw-r--r--   0 runner    (1001) docker     (127)    15154 2024-04-05 21:28:15.000000 log21-2.9.1/src/log21/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-04-05 21:28:15.000000 log21-2.9.1/src/log21/StreamHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9470 2024-04-05 21:28:15.000000 log21-2.9.1/src/log21/TreePrint.py
--rw-r--r--   0 runner    (1001) docker     (127)    24029 2024-04-05 21:28:15.000000 log21-2.9.1/src/log21/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:28:25.657975 log21-2.9.1/src/log21.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-04-05 21:28:25.000000 log21-2.9.1/src/log21.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-05 21:28:25.000000 log21-2.9.1/src/log21.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 21:28:25.000000 log21-2.9.1/src/log21.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-05 21:28:25.000000 log21-2.9.1/src/log21.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 21:28:25.000000 log21-2.9.1/src/log21.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:21:14.147370 log21-2.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-04-12 08:21:08.000000 log21-2.9.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-04-12 08:21:14.147370 log21-2.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-12 08:21:08.000000 log21-2.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-12 08:21:08.000000 log21-2.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 08:21:14.147370 log21-2.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:21:14.143370 log21-2.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:21:14.147370 log21-2.9.2/src/log21/
+-rw-r--r--   0 runner    (1001) docker     (127)    48386 2024-04-12 08:21:08.000000 log21-2.9.2/src/log21/Argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15182 2024-04-12 08:21:08.000000 log21-2.9.2/src/log21/Argumentify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11796 2024-04-12 08:21:08.000000 log21-2.9.2/src/log21/Colors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:21:14.147370 log21-2.9.2/src/log21/CrashReporter/
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-12 08:21:08.000000 log21-2.9.2/src/log21/CrashReporter/Formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14913 2024-04-12 08:21:08.000000 log21-2.9.2/src/log21/CrashReporter/Reporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-12 08:21:08.000000 log21-2.9.2/src/log21/CrashReporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-12 08:21:08.000000 log21-2.9.2/src/log21/FileHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11632 2024-04-12 08:21:08.000000 log21-2.9.2/src/log21/Formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-12 08:21:08.000000 log21-2.9.2/src/log21/Levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14968 2024-04-12 08:21:08.000000 log21-2.9.2/src/log21/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34385 2024-04-12 08:21:08.000000 log21-2.9.2/src/log21/LoggingWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-12 08:21:08.000000 log21-2.9.2/src/log21/Manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28854 2024-04-12 08:21:08.000000 log21-2.9.2/src/log21/PPrint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15154 2024-04-12 08:21:08.000000 log21-2.9.2/src/log21/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-04-12 08:21:08.000000 log21-2.9.2/src/log21/StreamHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9470 2024-04-12 08:21:08.000000 log21-2.9.2/src/log21/TreePrint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24029 2024-04-12 08:21:08.000000 log21-2.9.2/src/log21/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:21:14.147370 log21-2.9.2/src/log21.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-04-12 08:21:14.000000 log21-2.9.2/src/log21.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-12 08:21:14.000000 log21-2.9.2/src/log21.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 08:21:14.000000 log21-2.9.2/src/log21.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-12 08:21:14.000000 log21-2.9.2/src/log21.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 08:21:14.000000 log21-2.9.2/src/log21.egg-info/top_level.txt
```

### Comparing `log21-2.9.1/LICENSE.txt` & `log21-2.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `log21-2.9.1/PKG-INFO` & `log21-2.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log21
-Version: 2.9.1
+Version: 2.9.2
 Summary: A simple logging package that helps you log colorized messages in Windows console.
 Author-email: "CodeWriter21(Mehrad Pooryoussof)" <CodeWriter21@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/MPCodeWriter21/log21
 Project-URL: Donations, https://github.com/MPCodeWriter21/log21/blob/master/DONATE.md
 Project-URL: Source, https://github.com/MPCodeWriter21/log21
 Keywords: python,log,colorize,color,logging,Python3,CodeWriter21
@@ -88,17 +88,18 @@
 ```bash
 pip install git+https://github.com/MPCodeWriter21/log21
 ```
 
 Changes
 -------
 
-### 2.9.1
+### 2.9.2
 
-+ Update `README.md`.
++ Added `Sequence[T]` as a supported type to the ColorizingArgumentParser.
++ Bug fixes.
 
 [Full CHANGELOG](https://github.com/MPCodeWriter21/log21/blob/master/CHANGELOG.md)
 
 
 Usage Examples:
 ---------------
```

### Comparing `log21-2.9.1/README.md` & `log21-2.9.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,17 +57,18 @@
 ```bash
 pip install git+https://github.com/MPCodeWriter21/log21
 ```
 
 Changes
 -------
 
-### 2.9.1
+### 2.9.2
 
-+ Update `README.md`.
++ Added `Sequence[T]` as a supported type to the ColorizingArgumentParser.
++ Bug fixes.
 
 [Full CHANGELOG](https://github.com/MPCodeWriter21/log21/blob/master/CHANGELOG.md)
 
 
 Usage Examples:
 ---------------
```

### Comparing `log21-2.9.1/pyproject.toml` & `log21-2.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   "Operating System :: Microsoft :: Windows",
   "Operating System :: MacOS :: MacOS X"
 ]
 dependencies = [
   "webcolors",
   "docstring-parser"
 ]
-version = "2.9.1"
+version = "2.9.2"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project.urls]
 Homepage = "https://github.com/MPCodeWriter21/log21"
 Donations = "https://github.com/MPCodeWriter21/log21/blob/master/DONATE.md"
```

### Comparing `log21-2.9.1/src/log21/Argparse.py` & `log21-2.9.2/src/log21/Argparse.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 from __future__ import annotations
 
 import re as _re
 import sys as _sys
 import types as _types
 import typing as _typing
 import argparse as _argparse
+import collections.abc
 from enum import Enum as _Enum
-from typing import (Tuple as _Tuple, Mapping as _Mapping, Optional as _Optional,
-                    Sequence as _Sequence)
+from typing import (Tuple as _Tuple, Mapping as _Mapping, NoReturn,
+                    Optional as _Optional, Sequence as _Sequence)
 from gettext import gettext as _gettext
 from textwrap import TextWrapper as _TextWrapper
 from collections import OrderedDict as _OrderedDict
 
 import log21 as _log21
 from log21.Colors import get_colors as _gc
 from log21.Formatters import DecolorizingFormatter as _Formatter
@@ -74,15 +75,15 @@
         }
 
         if colors:
             for key, value in colors.items():
                 if key in self.colors:
                     self.colors[key] = value
 
-    class _Section(object):
+    class _Section:
 
         def __init__(self, formatter, parent, heading=None):
             self.formatter = formatter
             self.parent = parent
             self.heading = heading
             self.items = []
 
@@ -557,44 +558,51 @@
             func_type = func_type.__args__  # type: ignore
 
         # Handle `Literal` as a type (e.g. `Literal[1, 2, 3]`)
         elif (hasattr(_typing, '_LiteralGenericAlias')
               and isinstance(func_type, _typing._LiteralGenericAlias)):  # type: ignore
             func_type = Literal(func_type)
 
+        # Handle `Union` and `Optional` as a type (e.g. `Union[int, str]` and
+        # `Optional[int]`)
+        elif (hasattr(_typing, '_UnionGenericAlias')
+              and isinstance(func_type, _typing._UnionGenericAlias)):  # type: ignore
+            # Optional[T] is just Union[T, NoneType]
+            # Optional
+            if (hasattr(_types, 'NoneType') and len(func_type.__args__) == 2
+                    and func_type.__args__[1] is _types.NoneType):
+                action.required = False
+                func_type = func_type.__args__[0]
+            # Union
+            else:
+                func_type = func_type.__args__  # type: ignore
+
         # Handle `List` as a type (e.g. `List[int]`)
         elif (hasattr(_typing, '_GenericAlias')
               and isinstance(func_type, _typing._GenericAlias)  # type: ignore
-              and func_type.__origin__ is list):
+              and getattr(func_type, '__origin__') is list):
+            func_type = func_type.__args__[0]
+            if kwargs.get('nargs') is None:
+                action.nargs = '+'
+
+        # Handle `Sequence` as a type (e.g. `Sequence[int]`)
+        elif (hasattr(_typing, '_GenericAlias')
+              and isinstance(func_type, _typing._GenericAlias)  # type: ignore
+              and getattr(func_type, '__origin__') is collections.abc.Sequence):
             func_type = func_type.__args__[0]
             if kwargs.get('nargs') is None:
                 action.nargs = '+'
 
         # Handle `Required` as a type (e.g. `Required[int]`)
         elif (hasattr(_typing, 'Required') and hasattr(_typing, '_GenericAlias')
               and isinstance(func_type, _typing._GenericAlias)  # type: ignore
-              and func_type.__origin__ is _typing.Required
-              ):
+              and getattr(func_type, '__origin__') is _typing.Required):
             func_type = func_type.__args__[0]
             action.required = True
 
-        # Handle `Union` and `Optional` as a type (e.g. `Union[int, str]` and
-        # `Optional[int]`)
-        elif (hasattr(_types, 'NoneType') and hasattr(_typing, '_UnionGenericAlias')
-              and isinstance(func_type, _typing._UnionGenericAlias)):  # type: ignore
-            # Optional[T] is just Union[T, NoneType]
-            # Optional
-            if (len(func_type.__args__) == 2
-                    and func_type.__args__[1] is _types.NoneType):
-                action.required = False
-                func_type = func_type.__args__[0]
-            # Union
-            else:
-                func_type = func_type.__args__  # type: ignore
-
         # Handle Enum as a type
         elif callable(func_type) and isinstance(func_type, type) and issubclass(
                 func_type, _Enum) and action.choices is None and level == 0:
             action.choices = tuple(
                 map(lambda x: x.value, func_type.__members__.values())
             )
 
@@ -743,24 +751,23 @@
         args = {'prog': self.prog, 'message': message}
         self.exit(
             2,
             _gettext(
                 f'%(prog)s: {_gc("r")}error{_gc("lr")}:{_gc("rst")} %(message)s\n'
             ) % args
         )
+        return NoReturn
 
     def _get_formatter(self):
         if hasattr(self.formatter_class, 'colors'):
             return self.formatter_class(prog=self.prog, colors=self.colors)
-        else:
-            return self.formatter_class(prog=self.prog)
+        return self.formatter_class(prog=self.prog)
 
     def _get_value(self, action, arg_string):
-        """Override _get_value to add support for types such as Union and
-        Literal."""
+        """Override _get_value to add support for types such as Union and Literal."""
 
         func_type = self._registry_get('type', action.type, action.type)
         if not callable(func_type) and not isinstance(func_type, tuple):
             raise _argparse.ArgumentError(
                 action, _gettext(f'{func_type!r} is not callable')
             )
 
@@ -838,21 +845,22 @@
 
     def _read_args_from_files(self, arg_strings):
         # expand arguments referencing files
         new_arg_strings = []
         for arg_string in arg_strings:
 
             # for regular arguments, just add them back into the list
-            if not arg_string or arg_string[0] not in self.fromfile_prefix_chars:
+            if not arg_string or arg_string[0] not in (self.fromfile_prefix_chars
+                                                       or ''):
                 new_arg_strings.append(arg_string)
 
             # replace arguments referencing files with the file content
             else:
                 try:
-                    with open(arg_string[1:]) as args_file:
+                    with open(arg_string[1:], encoding='utf-8') as args_file:
                         arg_strings = []
                         for arg_line in args_file.read().splitlines():
                             for arg in self.convert_arg_line_to_args(arg_line):
                                 arg_strings.append(arg)
                         arg_strings = self._read_args_from_files(arg_strings)
                         new_arg_strings.extend(arg_strings)
                 except OSError as err:
@@ -1106,15 +1114,19 @@
                 else:
                     names = [
                         _argparse._get_action_name(action)
                         for action in group._group_actions
                         if action.help is not _argparse.SUPPRESS
                     ]
                     self.error(
-                        _gettext(f'one of the arguments {" ".join(names)} is required')
+                        _gettext(
+                            'one of the arguments ' +
+                            ' '.join(name for name in names if name is not None) +
+                            ' is required'
+                        )
                     )
 
         for group in self._action_groups:
             if isinstance(group, _ArgumentGroup) and group.required:
                 for action in group._group_actions:
                     if action in seen_non_default_actions:
                         break
@@ -1123,15 +1135,19 @@
                 else:
                     names = [
                         _argparse._get_action_name(action)
                         for action in group._group_actions
                         if action.help is not _argparse.SUPPRESS
                     ]
                     self.error(
-                        _gettext(f'one of the arguments {" ".join(names)} is required')
+                        _gettext(
+                            'one of the arguments ' +
+                            ' '.join(name for name in names if name is not None) +
+                            ' is required'
+                        )
                     )
 
         # return the updated namespace and the extra arguments
         return namespace, extras
 
 
 class _ArgumentGroup(_argparse._ArgumentGroup, _ActionsContainer):
```

### Comparing `log21-2.9.1/src/log21/Argumentify.py` & `log21-2.9.2/src/log21/Argumentify.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,19 +258,18 @@
     # Add the arguments
     for argument in info.arguments.values():
         config: _Dict[str, _Any] = {
             'action': 'store',
             'dest': argument.name,
             'help': argument.help
         }
-        if isinstance(argument.annotation, type):
-            config['type'] = argument.annotation
         if argument.annotation == bool:
             config['action'] = 'store_true'
-            config.pop('type')
+        elif argument.annotation:
+            config['type'] = argument.annotation
         if argument.kind == _inspect._ParameterKind.POSITIONAL_ONLY:
             config['required'] = True
         if argument.kind == _inspect._ParameterKind.VAR_POSITIONAL:
             config['nargs'] = '*'
         if argument.default:
             config['default'] = argument.default
         parser.add_argument(
```

### Comparing `log21-2.9.1/src/log21/Colors.py` & `log21-2.9.2/src/log21/Colors.py`

 * *Files identical despite different names*

### Comparing `log21-2.9.1/src/log21/CrashReporter/Formatters.py` & `log21-2.9.2/src/log21/CrashReporter/Formatters.py`

 * *Files identical despite different names*

### Comparing `log21-2.9.1/src/log21/CrashReporter/Reporters.py` & `log21-2.9.2/src/log21/CrashReporter/Reporters.py`

 * *Files identical despite different names*

### Comparing `log21-2.9.1/src/log21/FileHandler.py` & `log21-2.9.2/src/log21/FileHandler.py`

 * *Files identical despite different names*

### Comparing `log21-2.9.1/src/log21/Formatters.py` & `log21-2.9.2/src/log21/Formatters.py`

 * *Files identical despite different names*

### Comparing `log21-2.9.1/src/log21/Logger.py` & `log21-2.9.2/src/log21/Logger.py`

 * *Files identical despite different names*

### Comparing `log21-2.9.1/src/log21/LoggingWindow.py` & `log21-2.9.2/src/log21/LoggingWindow.py`

 * *Files identical despite different names*

### Comparing `log21-2.9.1/src/log21/Manager.py` & `log21-2.9.2/src/log21/Manager.py`

 * *Files identical despite different names*

### Comparing `log21-2.9.1/src/log21/PPrint.py` & `log21-2.9.2/src/log21/PPrint.py`

 * *Files identical despite different names*

### Comparing `log21-2.9.1/src/log21/ProgressBar.py` & `log21-2.9.2/src/log21/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `log21-2.9.1/src/log21/StreamHandler.py` & `log21-2.9.2/src/log21/StreamHandler.py`

 * *Files identical despite different names*

### Comparing `log21-2.9.1/src/log21/TreePrint.py` & `log21-2.9.2/src/log21/TreePrint.py`

 * *Files identical despite different names*

### Comparing `log21-2.9.1/src/log21/__init__.py` & `log21-2.9.2/src/log21/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from .Argumentify import argumentify
 from .FileHandler import FileHandler, DecolorizingFileHandler
 from .ProgressBar import ProgressBar
 from .LoggingWindow import LoggingWindow, LoggingWindowHandler
 from .StreamHandler import StreamHandler, ColorizingStreamHandler
 
 __author__ = 'CodeWriter21 (Mehrad Pooryoussof)'
-__version__ = '2.9.1'
+__version__ = '2.9.2'
 __github__ = 'Https://GitHub.com/MPCodeWriter21/log21'
 __all__ = [
     'ColorizingStreamHandler', 'DecolorizingFileHandler', 'ColorizingFormatter',
     'DecolorizingFormatter', 'get_logger', 'Logger', 'Colors', 'get_color',
     'get_colors', 'CRITICAL', 'FATAL', 'ERROR', 'WARNING', 'WARN', 'INFO', 'DEBUG',
     'NOTSET', 'INPUT', 'StreamHandler', 'ColorizingArgumentParser', 'PrettyPrinter',
     'pformat', 'pprint', 'pretty_print', 'tree_format', 'TreePrint', 'Manager',
```

### Comparing `log21-2.9.1/src/log21.egg-info/PKG-INFO` & `log21-2.9.2/src/log21.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log21
-Version: 2.9.1
+Version: 2.9.2
 Summary: A simple logging package that helps you log colorized messages in Windows console.
 Author-email: "CodeWriter21(Mehrad Pooryoussof)" <CodeWriter21@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/MPCodeWriter21/log21
 Project-URL: Donations, https://github.com/MPCodeWriter21/log21/blob/master/DONATE.md
 Project-URL: Source, https://github.com/MPCodeWriter21/log21
 Keywords: python,log,colorize,color,logging,Python3,CodeWriter21
@@ -88,17 +88,18 @@
 ```bash
 pip install git+https://github.com/MPCodeWriter21/log21
 ```
 
 Changes
 -------
 
-### 2.9.1
+### 2.9.2
 
-+ Update `README.md`.
++ Added `Sequence[T]` as a supported type to the ColorizingArgumentParser.
++ Bug fixes.
 
 [Full CHANGELOG](https://github.com/MPCodeWriter21/log21/blob/master/CHANGELOG.md)
 
 
 Usage Examples:
 ---------------
```

### Comparing `log21-2.9.1/src/log21.egg-info/SOURCES.txt` & `log21-2.9.2/src/log21.egg-info/SOURCES.txt`

 * *Files identical despite different names*

