# Comparing `tmp/heare-config-1.0.2.tar.gz` & `tmp/heare_config-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heare-config-1.0.2.tar", last modified: Fri Dec 24 07:08:31 2021, max compression
+gzip compressed data, was "heare_config-1.0.4.tar", last modified: Mon May 13 06:29:02 2024, max compression
```

## Comparing `heare-config-1.0.2.tar` & `heare_config-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-24 07:08:31.048664 heare-config-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)     7653 2021-12-24 07:08:16.000000 heare-config-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     9595 2021-12-24 07:08:31.048664 heare-config-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9289 2021-12-24 07:08:16.000000 heare-config-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-24 07:08:31.048664 heare-config-1.0.2/heare/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-24 07:08:31.048664 heare-config-1.0.2/heare/config/
--rw-r--r--   0 runner    (1001) docker     (121)    17682 2021-12-24 07:08:16.000000 heare-config-1.0.2/heare/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-24 07:08:31.048664 heare-config-1.0.2/heare_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9595 2021-12-24 07:08:31.000000 heare-config-1.0.2/heare_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      195 2021-12-24 07:08:31.000000 heare-config-1.0.2/heare_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-24 07:08:31.000000 heare-config-1.0.2/heare_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-12-24 07:08:31.000000 heare-config-1.0.2/heare_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-24 07:08:31.048664 heare-config-1.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      542 2021-12-24 07:08:16.000000 heare-config-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:29:02.582966 heare_config-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-05-13 06:28:53.000000 heare_config-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9558 2024-05-13 06:29:02.582966 heare_config-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9289 2024-05-13 06:28:53.000000 heare_config-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:29:02.578966 heare_config-1.0.4/heare/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:29:02.578966 heare_config-1.0.4/heare/config/
+-rw-r--r--   0 runner    (1001) docker     (127)    18070 2024-05-13 06:28:53.000000 heare_config-1.0.4/heare/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:29:02.582966 heare_config-1.0.4/heare_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9558 2024-05-13 06:29:02.000000 heare_config-1.0.4/heare_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-13 06:29:02.000000 heare_config-1.0.4/heare_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 06:29:02.000000 heare_config-1.0.4/heare_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 06:29:02.000000 heare_config-1.0.4/heare_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 06:29:02.582966 heare_config-1.0.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      542 2024-05-13 06:28:53.000000 heare_config-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:29:02.582966 heare_config-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-13 06:28:53.000000 heare_config-1.0.4/tests/test_cli_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-05-13 06:28:53.000000 heare_config-1.0.4/tests/test_setting.py
```

### Comparing `heare-config-1.0.2/LICENSE` & `heare_config-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `heare-config-1.0.2/PKG-INFO` & `heare_config-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: heare-config
-Version: 1.0.2
+Version: 1.0.4
 Summary: Heare.io Configuration Utilities
 Home-page: https://github.com/heare-io/heare-config
 Author: Sean Fitzgerald
 Author-email: seanfitz@heare.io
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # heare-config
 Configuration library used by projects under heare.io
 
 
@@ -255,9 +253,7 @@
 # MyFirstConfig.foo = ["bar"]
 # MySecondConfig.foo = "baz"
 ```
 
 
 
 
-
-
```

### Comparing `heare-config-1.0.2/README.md` & `heare_config-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `heare-config-1.0.2/heare/config/__init__.py` & `heare_config-1.0.4/heare/config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import copy
 import os
 import re
 import sys
+import typing
 from abc import ABCMeta, abstractmethod
 from collections import defaultdict
 from json import JSONEncoder
 from typing import TypeVar, Generic, Callable, \
     Optional, List, Tuple, Union, Dict, Generator, Set
 import configparser
 
@@ -137,15 +138,15 @@
         self.required: bool = required
         self.aliases: Optional[SettingAliases] = aliases
 
     def from_raw_value(self, value: str) -> List[T]:
         result: List[T] = []
         # ListSetting assumes values are CSV. Repeated command line flags
         # must be treated specially, but will also work with csv values.
-        value_parts = value.split(",")  # TODO: Replace with csv lib?
+        value_parts = value.split(",") if isinstance(value, str) else [value]
         for part in value_parts:
             try:
                 result.append(self.formatter(part))
             except Exception as _:
                 raise ValueError(
                     f"{value} cannot be parsed as {self.formatter.__name__}"
                 )
@@ -213,14 +214,17 @@
                         flag = flag[3:]
                 else:
                     # flag with argument, separated by space
                     value = args[idx + 1].strip()
                     idx += 1
             else:
                 value = parts[1].strip()
+            # translate hyphens to underscores to match
+            # syntax requirements
+            flag = flag.replace('-', '_')
             results.append((flag, value))
         idx += 1
 
     return results, positional
 
 
 ##################################################################
@@ -489,18 +493,25 @@
 
             if setting_spec.required and \
                     not (setting_candidates or setting_spec.default):
                 raise ValueError(
                     f"Required config not satisfied: {name}, {setting_spec}"
                 )
 
-            value = setting_spec.default if \
-                not setting_candidates else setting_candidates[0].raw_value
+            if setting_candidates:
+                if isinstance(setting_candidates[0].raw_value, bool):
+                    value = setting_candidates[0].raw_value
+                else:
+                    value = setting_spec.from_raw_value(
+                        setting_candidates[0].raw_value
+                    )
+            else:
+                value = setting_spec.default
 
             setattr(
                 result,
                 name, setting_spec.to_gettable(
-                    setting_spec.from_raw_value(value)
+                    value
                 )
             )
 
         return result
```

### Comparing `heare-config-1.0.2/heare_config.egg-info/PKG-INFO` & `heare_config-1.0.4/heare_config.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: heare-config
-Version: 1.0.2
+Version: 1.0.4
 Summary: Heare.io Configuration Utilities
 Home-page: https://github.com/heare-io/heare-config
 Author: Sean Fitzgerald
 Author-email: seanfitz@heare.io
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # heare-config
 Configuration library used by projects under heare.io
 
 
@@ -255,9 +253,7 @@
 # MyFirstConfig.foo = ["bar"]
 # MySecondConfig.foo = "baz"
 ```
 
 
 
 
-
-
```

### Comparing `heare-config-1.0.2/setup.py` & `heare_config-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 long_description = None
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(name='heare-config',
-      version='1.0.2',
+      version='1.0.4',
       description='Heare.io Configuration Utilities',
       long_description=long_description,
       long_description_content_type="text/markdown",
       author='Sean Fitzgerald',
       author_email='seanfitz@heare.io',
       url='https://github.com/heare-io/heare-config',
       packages=['heare.config'],
```

