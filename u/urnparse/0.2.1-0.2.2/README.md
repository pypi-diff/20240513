# Comparing `tmp/urnparse-0.2.1.tar.gz` & `tmp/urnparse-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urnparse-0.2.1.tar", last modified: Tue Sep 12 10:58:04 2023, max compression
+gzip compressed data, was "urnparse-0.2.2.tar", last modified: Mon May 13 08:47:41 2024, max compression
```

## Comparing `urnparse-0.2.1.tar` & `urnparse-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 10:58:04.138828 urnparse-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2023-09-12 10:57:47.000000 urnparse-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      304 2023-09-12 10:57:47.000000 urnparse-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2023-09-12 10:58:04.138828 urnparse-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2023-09-12 10:57:47.000000 urnparse-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      277 2023-09-12 10:57:47.000000 urnparse-0.2.1/pytest.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)      317 2023-09-12 10:57:47.000000 urnparse-0.2.1/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)       92 2023-09-12 10:58:04.138828 urnparse-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2023-09-12 10:57:47.000000 urnparse-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 10:58:04.134828 urnparse-0.2.1/urnparse/
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2023-09-12 10:57:47.000000 urnparse-0.2.1/urnparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2023-09-12 10:57:47.000000 urnparse-0.2.1/urnparse/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 10:58:04.138828 urnparse-0.2.1/urnparse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2023-09-12 10:58:04.000000 urnparse-0.2.1/urnparse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-09-12 10:58:04.000000 urnparse-0.2.1/urnparse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-12 10:58:04.000000 urnparse-0.2.1/urnparse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-12 10:57:58.000000 urnparse-0.2.1/urnparse.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-09-12 10:58:04.000000 urnparse-0.2.1/urnparse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-09-12 10:58:04.000000 urnparse-0.2.1/urnparse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:47:41.982903 urnparse-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-13 08:47:27.000000 urnparse-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-13 08:47:27.000000 urnparse-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-13 08:47:41.982903 urnparse-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-13 08:47:27.000000 urnparse-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-13 08:47:27.000000 urnparse-0.2.2/pytest.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)      300 2024-05-13 08:47:27.000000 urnparse-0.2.2/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-13 08:47:41.982903 urnparse-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-13 08:47:27.000000 urnparse-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:47:41.978903 urnparse-0.2.2/urnparse/
+-rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-05-13 08:47:27.000000 urnparse-0.2.2/urnparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:47:27.000000 urnparse-0.2.2/urnparse/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-13 08:47:27.000000 urnparse-0.2.2/urnparse/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:47:41.978903 urnparse-0.2.2/urnparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-13 08:47:41.000000 urnparse-0.2.2/urnparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-13 08:47:41.000000 urnparse-0.2.2/urnparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:47:41.000000 urnparse-0.2.2/urnparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:47:38.000000 urnparse-0.2.2/urnparse.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-13 08:47:41.000000 urnparse-0.2.2/urnparse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-13 08:47:41.000000 urnparse-0.2.2/urnparse.egg-info/top_level.txt
```

### Comparing `urnparse-0.2.1/LICENSE` & `urnparse-0.2.2/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Open Access Repository
+Copyright (c) 2024 CESNET
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `urnparse-0.2.1/PKG-INFO` & `urnparse-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urnparse
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python library for generating and parsing and RFC 8141 compliant uniform resource names (URN).
 Home-page: https://github.com/oarepo/urnparse
 Author: Miroslav Bauer @ CESNET
 Author-email: bauer@cesnet.cz
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing_extensions>=4.11.0
 Provides-Extra: tests
 Requires-Dist: pydocstyle; extra == "tests"
 Requires-Dist: isort; extra == "tests"
 Requires-Dist: check-manifest; extra == "tests"
 Requires-Dist: pytest; extra == "tests"
 
 # urnparse
```

### Comparing `urnparse-0.2.1/README.md` & `urnparse-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `urnparse-0.2.1/setup.py` & `urnparse-0.2.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2021 Miroslav Bauer @ CESNET.
+# Copyright (C) 2024 CESNET.
 #
 # urnparse is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Python library for generating and parsing and RFC 8141 compliant uniform resource names (URN)."""
 
 import os
@@ -19,15 +19,17 @@
     "tests": ["pydocstyle", "isort", "check-manifest", "pytest"],
 }
 
 setup_requires = [
     "pytest-runner>=3.0.0,<5",
 ]
 
-install_requires = []
+install_requires = [
+        "typing_extensions>=4.11.0"
+]
 
 packages = find_packages(exclude=["tests"])
 
 # Get the version string. Cannot be done with import!
 g = {}
 with open(os.path.join("urnparse", "version.py"), "rt") as fp:
     exec(fp.read(), g)
```

### Comparing `urnparse-0.2.1/urnparse/__init__.py` & `urnparse-0.2.2/urnparse/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,65 +1,73 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2021 Miroslav Bauer @ CESNET.
+# Copyright (C) 2024 CESNET.
 #
 # urnparse is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Python library for generating and parsing and RFC 8141 compliant uniform resource names (URN)."""
 
 import re
+from typing import Any, ClassVar, Pattern
+
+try:
+    from typing import Self
+except ImportError:
+    # For backwards comaptibility with Python<3.11
+    from typing_extensions import Self
+
 from urllib.parse import parse_qs, quote, unquote, urlencode
 
 URN_SCHEME = 'urn'
-NID_PATTERN = re.compile(r'^[0-9a-z][0-9a-z-]{1,31}$', flags=re.IGNORECASE)
+NID_PATTERN: Pattern = re.compile(r'^[0-9a-z][0-9a-z-]{1,31}$', flags=re.IGNORECASE)
 NSS_PCHAR = '[a-z0-9-._~]|%[a-f0-9]{2}|[!$&\'()*+,;=]|:|@'
-NSS_PATTERN = re.compile(fr'^({NSS_PCHAR})({NSS_PCHAR}|/|\?)*$', re.IGNORECASE)
-RQF_PATTERN = re.compile(
+NSS_PATTERN: Pattern = re.compile(fr'^({NSS_PCHAR})({NSS_PCHAR}|/|\?)*$', re.IGNORECASE)
+RQF_PATTERN: Pattern = re.compile(
     r"^(?!$)(?:\?\+(?P<resolution_string>.*?))?(?:\?=(?P<query_string>.*?))?(?:#(?P<fragment>.*?))?$",
     flags=re.IGNORECASE)
 
 
-def _validate_nid(value, min_len, max_len, pattern):
+def _validate_nid(value: str, min_len: int, max_len: int, pattern: Pattern[str]):
     strlen = len(value)
     if strlen < min_len:
         raise InvalidURNFormatError(f'{value} is shorter than {min_len}')
     elif strlen > max_len:
         raise InvalidURNFormatError(f'{value} is longer than {max_len}')
 
     if not re.match(pattern, value):
         raise InvalidURNFormatError(f'{value} contains invalid characters')
 
 
 class NSIdentifier:
     """Namespace identifier class."""
 
-    MIN_LENGTH = 2
-    MAX_LENGTH = 32
+    MIN_LENGTH: ClassVar[int] = 2
+    MAX_LENGTH: ClassVar[int] = 32
 
-    def __init__(self, val):
+    def __init__(self, val: str):
         """Initialize a Namespace identifier."""
         _validate_nid(val, self.MIN_LENGTH, self.MAX_LENGTH, NID_PATTERN)
         self.value = val
 
     def __repr__(self):
         """Representation of Namespace identifier."""
         return str(self.value)
 
-    def __eq__(self, other):
+    def __eq__(self, other: Self | Any):
         """Compare two Namespace identifiers."""
         if isinstance(other, self.__class__):
             return str(self.value) == str(other.value)
         return str(self) == str(other)
 
 
 class NSSString:
     """Namespace specific string class."""
 
-    def __init__(self, val, encoded=True):
+    def __init__(self, val: str, encoded:bool=True):
         """Initialize a NSS String."""
         if encoded:
             if len(val) == 0 or not re.match(NSS_PATTERN, val):
                 raise InvalidURNFormatError('NSS string is invalid.')
 
             self.encoded = val
             self._value = unquote(val)
@@ -77,32 +85,32 @@
         """Colon-separated parts of a NSSString."""
         return self._value.split(':')
 
     def __repr__(self):
         """Representation of NSSString."""
         return str(self.encoded)
 
-    def __eq__(self, other):
+    def __eq__(self, other: Self | Any):
         """Compare two NSSStrings."""
         if isinstance(other, self.__class__):
             return str(self.encoded) == str(other.encoded)
         return str(self) == str(other)
 
 
 class RQFComponent:
     """RQF Component class."""
 
-    RESOLUTION_SEPERATOR = '?+'
-    QUERY_SEPERATOR = '?='
-    FRAGMENT_SEPERATOR = '#'
+    RESOLUTION_SEPERATOR: ClassVar[str] = '?+'
+    QUERY_SEPERATOR: ClassVar[str] = '?='
+    FRAGMENT_SEPERATOR: ClassVar[str] = '#'
 
     def __init__(self, resolution_string: str, query_string: str, fragment: str):
         """Initialize a RQF Component."""
-        query_args = []
-        resolution_args = []
+        query_args = dict()
+        resolution_args = dict()
         if query_string != '':
             query_args = {k: v[0] for k, v in parse_qs(query_string).items()}
         if resolution_string != '':
             resolution_args = {k: v[0] for k, v in parse_qs(resolution_string).items()}
 
         self._resolution_args = resolution_args
         self._query_args = query_args
@@ -141,15 +149,15 @@
 class URN8141:
     """
     A RFC 8141 compliant uniform resource name (URN).
 
     @see https://tools.ietf.org/html/rfc8141
     """
 
-    def __init__(self, nid: NSIdentifier = None, nss: NSSString = None, rqf=None):
+    def __init__(self, nid: NSIdentifier, nss: NSSString, rqf=None):
         """
         Initialize a RFC 8141 compliant uniform resource name.
 
         :param nid: The namespace identifier
         :param nss: The namespace specific string
         :param rqf: R, Q and F components of the URN
         """
@@ -169,15 +177,15 @@
 
     @property
     def rqf_component(self) -> RQFComponent:
         """Rqfcomponent parts of the URN."""
         return self._rqf
 
     @classmethod
-    def from_string(cls, urn_string, encoded=True):
+    def from_string(cls, urn_string: str, encoded: bool=True):
         """Create an instance from a RFC 8141 formatted URN string.
 
         :param urn_string: A RFC 8141 formatted URN string
         :param encoded: URN string is urlencoded
         :raises InvalidURNFormatError
         """
         if not urn_string.startswith(URN_SCHEME) or urn_string.count(':') < 2:
@@ -217,15 +225,15 @@
 
         return RQFComponent(**matched.groupdict())
 
     def __repr__(self):
         """Representation of the URN."""
         return f'urn:{self._nid}:{self._nss}{self._rqf}'
 
-    def __eq__(self, other):
+    def __eq__(self, other: Self|Any):
         """Compare two URNs."""
         if isinstance(other, self.__class__):
             return self._nid == other.namespace_id and self._nss == other.specific_string
         return str(self) == str(other)
 
 
 class InvalidURNFormatError(Exception):
```

### Comparing `urnparse-0.2.1/urnparse.egg-info/PKG-INFO` & `urnparse-0.2.2/urnparse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urnparse
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python library for generating and parsing and RFC 8141 compliant uniform resource names (URN).
 Home-page: https://github.com/oarepo/urnparse
 Author: Miroslav Bauer @ CESNET
 Author-email: bauer@cesnet.cz
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing_extensions>=4.11.0
 Provides-Extra: tests
 Requires-Dist: pydocstyle; extra == "tests"
 Requires-Dist: isort; extra == "tests"
 Requires-Dist: check-manifest; extra == "tests"
 Requires-Dist: pytest; extra == "tests"
 
 # urnparse
```

