# Comparing `tmp/pygount-1.7.0.tar.gz` & `tmp/pygount-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygount-1.7.0.tar", max compression
+gzip compressed data, was "pygount-1.8.0.tar", max compression
```

## Comparing `pygount-1.7.0.tar` & `pygount-1.8.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1488 2023-01-02 08:17:33.701239 pygount-1.7.0/LICENSE.txt
--rw-r--r--   0        0        0     4888 2023-07-03 04:32:22.600614 pygount-1.7.0/README.md
--rw-r--r--   0        0        0      686 2024-05-12 13:06:18.720843 pygount-1.7.0/pygount/__init__.py
--rw-r--r--   0        0        0    36066 2024-05-12 22:05:36.850358 pygount-1.7.0/pygount/analysis.py
--rw-r--r--   0        0        0    16289 2024-05-12 22:36:04.083259 pygount-1.7.0/pygount/command.py
--rw-r--r--   0        0        0     6477 2024-05-12 13:06:18.721251 pygount-1.7.0/pygount/common.py
--rw-r--r--   0        0        0     1371 2023-07-03 04:32:22.605440 pygount-1.7.0/pygount/git_storage.py
--rw-r--r--   0        0        0     2086 2024-05-12 13:06:18.721348 pygount-1.7.0/pygount/lexers.py
--rw-r--r--   0        0        0     9254 2024-05-12 13:06:18.721489 pygount-1.7.0/pygount/summary.py
--rw-r--r--   0        0        0    10833 2024-05-12 22:52:08.912560 pygount-1.7.0/pygount/write.py
--rw-r--r--   0        0        0     4297 2024-05-12 13:06:18.721774 pygount-1.7.0/pygount/xmldialect.py
--rw-r--r--   0        0        0     2246 2024-05-12 13:06:18.721999 pygount-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     6360 1970-01-01 00:00:00.000000 pygount-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1488 2024-05-12 23:37:29.823738 pygount-1.8.0/LICENSE.txt
+-rw-r--r--   0        0        0     4888 2023-07-03 04:32:22.600614 pygount-1.8.0/README.md
+-rw-r--r--   0        0        0      686 2024-05-12 23:37:29.824278 pygount-1.8.0/pygount/__init__.py
+-rw-r--r--   0        0        0    36316 2024-05-13 12:45:14.902886 pygount-1.8.0/pygount/analysis.py
+-rw-r--r--   0        0        0    16289 2024-05-12 23:37:29.824627 pygount-1.8.0/pygount/command.py
+-rw-r--r--   0        0        0     6477 2024-05-12 23:37:29.824846 pygount-1.8.0/pygount/common.py
+-rw-r--r--   0        0        0     1371 2023-07-03 04:32:22.605440 pygount-1.8.0/pygount/git_storage.py
+-rw-r--r--   0        0        0     2086 2024-05-12 23:37:29.824973 pygount-1.8.0/pygount/lexers.py
+-rw-r--r--   0        0        0     9254 2024-05-13 14:37:07.088820 pygount-1.8.0/pygount/summary.py
+-rw-r--r--   0        0        0    11543 2024-05-13 16:00:30.206219 pygount-1.8.0/pygount/write.py
+-rw-r--r--   0        0        0     4297 2024-05-12 23:37:29.825523 pygount-1.8.0/pygount/xmldialect.py
+-rw-r--r--   0        0        0     2246 2024-05-13 16:05:21.637129 pygount-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     6360 1970-01-01 00:00:00.000000 pygount-1.8.0/PKG-INFO
```

### Comparing `pygount-1.7.0/LICENSE.txt` & `pygount-1.8.0/LICENSE.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2016-2023, Thomas Aglassinger
+Copyright (c) 2016-2024, Thomas Aglassinger
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `pygount-1.7.0/README.md` & `pygount-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pygount-1.7.0/pygount/__init__.py` & `pygount-1.8.0/pygount/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Pygount counts lines of source code using pygments lexers.
 """
 
-# Copyright (c) 2016-2023, Thomas Aglassinger.
+# Copyright (c) 2016-2024, Thomas Aglassinger.
 # All rights reserved. Distributed under the BSD License.
 from importlib.metadata import version
 
 from .analysis import DuplicatePool, SourceAnalysis, SourceScanner, SourceState, encoding_for, source_analysis
 from .common import Error, OptionError
 from .summary import LanguageSummary, ProjectSummary
```

### Comparing `pygount-1.7.0/pygount/analysis.py` & `pygount-1.8.0/pygount/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Functions to analyze source code and count lines in it.
 """
 
-# Copyright (c) 2016-2023, Thomas Aglassinger.
+# Copyright (c) 2016-2024, Thomas Aglassinger.
 # All rights reserved. Distributed under the BSD License.
 import codecs
 import collections
 import glob
 import hashlib
 import itertools
 import logging
@@ -412,14 +412,21 @@
         white characters or white code words
 
         See also: :py:func:`white_characters`, :py:func:`white_code_words`
         """
         return self._empty
 
     @property
+    def line_count(self) -> int:
+        """number of total lines, which is what you text editor a `wc -l`
+        would show
+        """
+        return self.code_count + self.documentation_count + self.empty_count + self.string_count
+
+    @property
     def string_count(self) -> int:
         """number of lines containing only strings but no other code"""
         return self._string
 
     @property
     def source_count(self) -> int:
         """number of source lines of code (the sum of code_count and string_count)"""
```

### Comparing `pygount-1.7.0/pygount/command.py` & `pygount-1.8.0/pygount/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Command line interface for pygount.
 """
 
-# Copyright (c) 2016-2023, Thomas Aglassinger.
+# Copyright (c) 2016-2024, Thomas Aglassinger.
 # All rights reserved. Distributed under the BSD License.
 import argparse
 import contextlib
 import logging
 import os
 import sys
```

### Comparing `pygount-1.7.0/pygount/common.py` & `pygount-1.8.0/pygount/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Common classes and functions for pygount.
 """
 
-# Copyright (c) 2016-2023, Thomas Aglassinger.
+# Copyright (c) 2016-2024, Thomas Aglassinger.
 # All rights reserved. Distributed under the BSD License.
 import fnmatch
 import functools
 import inspect
 import re
 import warnings
 from typing import Iterator, List, Optional, Pattern, Sequence, Union
```

### Comparing `pygount-1.7.0/pygount/git_storage.py` & `pygount-1.8.0/pygount/git_storage.py`

 * *Files identical despite different names*

### Comparing `pygount-1.7.0/pygount/lexers.py` & `pygount-1.8.0/pygount/lexers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Additional lexers for pygount that fill gaps left by :py:mod:`pygments`.
 """
 
-# Copyright (c) 2016-2023, Thomas Aglassinger.
+# Copyright (c) 2016-2024, Thomas Aglassinger.
 # All rights reserved. Distributed under the BSD License.
 import pygments.lexer
 import pygments.lexers
 import pygments.token
 import pygments.util
```

### Comparing `pygount-1.7.0/pygount/summary.py` & `pygount-1.8.0/pygount/summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Summaries of analyses of multiple source codes.
 """
 
-# Copyright (c) 2016-2023, Thomas Aglassinger.
+# Copyright (c) 2016-2024, Thomas Aglassinger.
 # All rights reserved. Distributed under the BSD License.
 import functools
 import re
 from typing import Dict, Hashable
 
 from .analysis import SourceAnalysis
 
@@ -196,36 +196,36 @@
         return self._total_empty_count
 
     @property
     def total_empty_percentage(self) -> float:
         return _percentage_or_0(self.total_empty_count, self.total_line_count)
 
     @property
-    def total_string_count(self) -> int:
-        return self._total_string_count
+    def total_file_count(self) -> int:
+        return self._total_file_count
 
     @property
-    def total_string_percentage(self) -> float:
-        return _percentage_or_0(self.total_string_count, self.total_line_count)
+    def total_line_count(self) -> int:
+        return self._total_line_count
 
     @property
     def total_source_count(self) -> int:
         return self.total_code_count + self.total_string_count
 
     @property
     def total_source_percentage(self) -> float:
         return _percentage_or_0(self.total_source_count, self.total_line_count)
 
     @property
-    def total_file_count(self) -> int:
-        return self._total_file_count
+    def total_string_count(self) -> int:
+        return self._total_string_count
 
     @property
-    def total_line_count(self) -> int:
-        return self._total_line_count
+    def total_string_percentage(self) -> float:
+        return _percentage_or_0(self.total_string_count, self.total_line_count)
 
     def add(self, source_analysis: SourceAnalysis) -> None:
         """
         Add counts from ``source_analysis`` to total counts.
         """
         self._total_file_count += 1
         language_summary = self.language_to_language_summary_map.get(source_analysis.language)
```

### Comparing `pygount-1.7.0/pygount/write.py` & `pygount-1.8.0/pygount/write.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Writers to store the results of a pygount analysis.
 """
 
-# Copyright (c) 2016-2023, Thomas Aglassinger.
+# Copyright (c) 2016-2024, Thomas Aglassinger.
 # All rights reserved. Distributed under the BSD License.
 import datetime
 import json
 import math
 import os
 from xml.etree import ElementTree
 
@@ -17,15 +17,15 @@
 
 from . import SourceAnalysis
 from .summary import ProjectSummary
 
 #: Version of cloc the --format=cloc-xml pretends to be.
 CLOC_VERSION = "1.60"
 
-JSON_FORMAT_VERSION = "1.0.0"
+JSON_FORMAT_VERSION = "1.1.0"
 
 
 class BaseWriter:
     def __init__(self, target_stream):
         self._target_stream = target_stream
         try:
             self.target_name = self._target_stream.name
@@ -197,19 +197,21 @@
         super().__init__(target_stream)
         self.source_analyses = []
 
     def add(self, source_analysis: SourceAnalysis):
         super().add(source_analysis)
         self.source_analyses.append(
             {
-                "emptyCount": source_analysis.empty_count,
+                "codeCount": source_analysis.code_count,
                 "documentationCount": source_analysis.documentation_count,
+                "emptyCount": source_analysis.empty_count,
                 "group": source_analysis.group,
                 "isCountable": source_analysis.is_countable,
                 "language": source_analysis.language,
+                "lineCount": source_analysis.line_count,
                 "path": source_analysis.path,
                 "state": source_analysis.state.name,
                 "stateInfo": source_analysis.state_info,
                 "sourceCount": source_analysis.source_count,
             }
         )
 
@@ -220,40 +222,48 @@
             "formatVersion": JSON_FORMAT_VERSION,
             "pygountVersion": pygount.__version__,
             "files": self.source_analyses,
             "languages": [
                 {
                     "documentationCount": language_summary.documentation_count,
                     "documentationPercentage": language_summary.documentation_percentage,
+                    "codeCount": language_summary.code_count,
+                    "codePercentage": language_summary.code_percentage,
                     "emptyCount": language_summary.empty_count,
                     "emptyPercentage": language_summary.empty_percentage,
                     "fileCount": language_summary.file_count,
                     "filePercentage": language_summary.file_percentage,
                     "isPseudoLanguage": language_summary.is_pseudo_language,
                     "language": language_summary.language,
                     "sourceCount": language_summary.source_count,
                     "sourcePercentage": language_summary.source_percentage,
+                    "stringCount": language_summary.string_count,
+                    "stringPercentage": language_summary.string_percentage,
                 }
                 for language_summary in self.project_summary.language_to_language_summary_map.values()
             ],
             "runtime": {
                 "durationInSeconds": self.duration_in_seconds,
                 "filesPerSecond": self.files_per_second,
                 "finishedAt": self.finished_at.isoformat(),
                 "linesPerSecond": self.lines_per_second,
                 "startedAt": self.started_at.isoformat(),
             },
             "summary": {
+                "totalCodeCount": self.project_summary.total_code_count,
+                "totalCodePercentage": self.project_summary.total_code_percentage,
                 "totalDocumentationCount": self.project_summary.total_documentation_count,
                 "totalDocumentationPercentage": self.project_summary.total_documentation_percentage,
                 "totalEmptyCount": self.project_summary.total_empty_count,
                 "totalEmptyPercentage": self.project_summary.total_empty_percentage,
                 "totalFileCount": self.project_summary.total_file_count,
                 "totalSourceCount": self.project_summary.total_source_count,
                 "totalSourcePercentage": self.project_summary.total_source_percentage,
+                "totalStringCount": self.project_summary.total_string_count,
+                "totalStringPercentage": self.project_summary.total_string_percentage,
             },
         }
         json.dump(json_map, self._target_stream)
 
 
 def digit_width(line_count: int) -> int:
     assert line_count >= 0
```

### Comparing `pygount-1.7.0/pygount/xmldialect.py` & `pygount-1.8.0/pygount/xmldialect.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Function to obtain the language dialect used by XML source code.
 """
 
-# Copyright (c) 2016-2023, Thomas Aglassinger.
+# Copyright (c) 2016-2024, Thomas Aglassinger.
 # All rights reserved. Distributed under the BSD License.
 import logging
 import re
 import xml.sax
 
 # TODO #10: Replace regex for DTD by working DTD handler.
 #: Regular expression to obtain DTD.
```

### Comparing `pygount-1.7.0/pyproject.toml` & `pygount-1.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ]
 testpaths = [
     "tests",
 ]
 
 [tool.poetry]
 name = "pygount"
-version = "1.7.0"
+version = "1.8.0"
 description = "count source lines of code (SLOC) using pygments"
 readme = "README.md"
 authors = ["Thomas Aglassinger <roskakori@users.sourceforge.net>"]
 license = "BSD"
 homepage = "https://github.com/roskakori/pygount"
 repository = "https://github.com/roskakori/pygount.git"
 documentation = "https://pygount.readthedocs.io"
```

### Comparing `pygount-1.7.0/PKG-INFO` & `pygount-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygount
-Version: 1.7.0
+Version: 1.8.0
 Summary: count source lines of code (SLOC) using pygments
 Home-page: https://github.com/roskakori/pygount
 License: BSD
 Keywords: code analysis,count,SLOC
 Author: Thomas Aglassinger
 Author-email: roskakori@users.sourceforge.net
 Requires-Python: >=3.8,<3.13
```

