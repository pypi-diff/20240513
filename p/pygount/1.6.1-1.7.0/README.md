# Comparing `tmp/pygount-1.6.1.tar.gz` & `tmp/pygount-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygount-1.6.1.tar", max compression
+gzip compressed data, was "pygount-1.7.0.tar", max compression
```

## Comparing `pygount-1.6.1.tar` & `pygount-1.7.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1488 2023-01-02 08:17:33.701239 pygount-1.6.1/LICENSE.txt
--rw-r--r--   0        0        0     4888 2023-06-25 23:16:15.321381 pygount-1.6.1/README.md
--rw-r--r--   0        0        0      685 2023-06-02 15:02:53.678813 pygount-1.6.1/pygount/__init__.py
--rw-r--r--   0        0        0    35167 2023-06-30 16:03:18.509620 pygount-1.6.1/pygount/analysis.py
--rw-r--r--   0        0        0    15396 2023-06-06 08:13:21.872180 pygount-1.6.1/pygount/command.py
--rw-r--r--   0        0        0     6476 2023-06-13 20:37:39.920761 pygount-1.6.1/pygount/common.py
--rw-r--r--   0        0        0     1371 2023-06-25 22:16:01.849583 pygount-1.6.1/pygount/git_storage.py
--rw-r--r--   0        0        0     2085 2023-01-02 08:17:33.702607 pygount-1.6.1/pygount/lexers.py
--rw-r--r--   0        0        0     9253 2023-01-02 08:17:33.702836 pygount-1.6.1/pygount/summary.py
--rw-r--r--   0        0        0    10648 2023-06-02 16:31:08.551599 pygount-1.6.1/pygount/write.py
--rw-r--r--   0        0        0     4296 2023-01-02 08:17:33.703237 pygount-1.6.1/pygount/xmldialect.py
--rw-r--r--   0        0        0     2138 2023-06-30 16:03:18.509974 pygount-1.6.1/pyproject.toml
--rw-r--r--   0        0        0     6315 1970-01-01 00:00:00.000000 pygount-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1488 2023-01-02 08:17:33.701239 pygount-1.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     4888 2023-07-03 04:32:22.600614 pygount-1.7.0/README.md
+-rw-r--r--   0        0        0      686 2024-05-12 13:06:18.720843 pygount-1.7.0/pygount/__init__.py
+-rw-r--r--   0        0        0    36066 2024-05-12 22:05:36.850358 pygount-1.7.0/pygount/analysis.py
+-rw-r--r--   0        0        0    16289 2024-05-12 22:36:04.083259 pygount-1.7.0/pygount/command.py
+-rw-r--r--   0        0        0     6477 2024-05-12 13:06:18.721251 pygount-1.7.0/pygount/common.py
+-rw-r--r--   0        0        0     1371 2023-07-03 04:32:22.605440 pygount-1.7.0/pygount/git_storage.py
+-rw-r--r--   0        0        0     2086 2024-05-12 13:06:18.721348 pygount-1.7.0/pygount/lexers.py
+-rw-r--r--   0        0        0     9254 2024-05-12 13:06:18.721489 pygount-1.7.0/pygount/summary.py
+-rw-r--r--   0        0        0    10833 2024-05-12 22:52:08.912560 pygount-1.7.0/pygount/write.py
+-rw-r--r--   0        0        0     4297 2024-05-12 13:06:18.721774 pygount-1.7.0/pygount/xmldialect.py
+-rw-r--r--   0        0        0     2246 2024-05-12 13:06:18.721999 pygount-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6360 1970-01-01 00:00:00.000000 pygount-1.7.0/PKG-INFO
```

### Comparing `pygount-1.6.1/LICENSE.txt` & `pygount-1.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygount-1.6.1/README.md` & `pygount-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pygount-1.6.1/pygount/__init__.py` & `pygount-1.7.0/pygount/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Pygount counts lines of source code using pygments lexers.
 """
+
 # Copyright (c) 2016-2023, Thomas Aglassinger.
 # All rights reserved. Distributed under the BSD License.
 from importlib.metadata import version
 
 from .analysis import DuplicatePool, SourceAnalysis, SourceScanner, SourceState, encoding_for, source_analysis
 from .common import Error, OptionError
 from .summary import LanguageSummary, ProjectSummary
```

### Comparing `pygount-1.6.1/pygount/analysis.py` & `pygount-1.7.0/pygount/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 Functions to analyze source code and count lines in it.
 """
+
 # Copyright (c) 2016-2023, Thomas Aglassinger.
 # All rights reserved. Distributed under the BSD License.
 import codecs
 import collections
 import glob
 import hashlib
 import itertools
 import logging
 import os
 import re
 from enum import Enum
 from io import SEEK_CUR, BufferedIOBase, IOBase, RawIOBase, TextIOBase
-from typing import Dict, Iterator, List, Optional, Pattern, Sequence, Set, Tuple, Union
+from typing import Iterator, List, Optional, Pattern, Sequence, Set, Tuple, Union
 
 import pygments.lexer
 import pygments.lexers
 import pygments.token
 import pygments.util
 
 import pygount.common
@@ -43,14 +44,16 @@
     [".?*", "_svn", "__pycache__"]  # Subversion hack for Windows  # Python byte code
 )
 
 
 #: Pygments token type; we need to define our own type because pygments' ``_TokenType`` is internal.
 TokenType = type(pygments.token.Token)
 
+_BASE_LANGUAGE_REGEX = re.compile(r"^(?P<base_language>[^+]+)\+[^+].*$")
+
 
 class SourceState(Enum):
     """
     Possible values for :py:attr:`SourceAnalysis.state`.
     """
 
     #: successfully analyzed
@@ -108,15 +111,15 @@
     "changelog",
     "copying",
     "install",
     "license",
     "news",
     "readme",
     "thanks",
-    # Github community recommendations, see
+    # GitHub community recommendations, see
     # <https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions>.
     # By now, in practice most projects use a suffix like "*.md" but some older ones
     # still might have such files without suffix.
     "code_of_conduct",
     "contributing",
     "support",
     # Other common text files.
@@ -151,21 +154,21 @@
     def __init__(self):
         self._size_to_paths_map = {}
         self._size_and_hash_to_path_map = {}
 
     @staticmethod
     def _hash_for(path_to_hash):
         buffer_size = 1024 * 1024
-        md5_hash = hashlib.md5()
+        sha256_hash = hashlib.sha256()
         with open(path_to_hash, "rb", buffer_size) as file_to_hash:
             data = file_to_hash.read(buffer_size)
             while len(data) >= 1:
-                md5_hash.update(data)
+                sha256_hash.update(data)
                 data = file_to_hash.read(buffer_size)
-        return md5_hash.digest()
+        return sha256_hash.digest()
 
     def duplicate_path(self, source_path: str) -> Optional[str]:
         """
         Path to a duplicate for ``source_path`` or ``None`` if no duplicate exists.
 
         Internally information is stored to identify possible future duplicates of
         ``source_path``.
@@ -241,52 +244,52 @@
             state=state,
             state_info=state_info,
         )
 
     @staticmethod
     def _check_state_info(state: SourceState, state_info: Optional[str]):
         states_that_require_state_info = [SourceState.duplicate, SourceState.error, SourceState.generated]
-        assert (state in states_that_require_state_info) == (
-            state_info is not None
-        ), "state={} and state_info={} but state_info must be specified for the following states: {}".format(
-            state,
-            state_info,
-            states_that_require_state_info,
+        assert (state in states_that_require_state_info) == (state_info is not None), (
+            f"state={state} and state_info={state_info} "
+            f"but state_info must be specified for the following states: {states_that_require_state_info}"
         )
 
     @staticmethod
     def from_file(
         source_path: str,
         group: str,
         encoding: str = "automatic",
         fallback_encoding: str = "cp1252",
-        generated_regexes=pygount.common.regexes_from(DEFAULT_GENERATED_PATTERNS_TEXT),
+        generated_regexes: Optional[List[Pattern]] = None,
         duplicate_pool: Optional[DuplicatePool] = None,
         file_handle: Optional[IOBase] = None,
+        merge_embedded_language: bool = False,
     ) -> "SourceAnalysis":
         """
         Factory method to create a :py:class:`SourceAnalysis` by analyzing
         the source code in ``source_path`` or the open file ``file_handle``.
 
         :param source_path: path to source code to analyze
-        :param group: name of a logical group the sourc code belongs to, e.g. a
+        :param group: name of a logical group the source code belongs to, e.g. a
           package.
         :param encoding: encoding according to :func:`encoding_for`
         :param fallback_encoding: fallback encoding according to
           :func:`encoding_for`
         :param generated_regexes: list of regular expression that if found within the first few lines
           if a source code identify is as generated source code for which SLOC should not be counted
         :param duplicate_pool: a :class:`DuplicatePool` where information about possible duplicates is
           collected, or ``None`` if possible duplicates should be counted multiple times.
         :param file_handle: a file-like object, or ``None`` to read and open the file from
           ``source_path``. If the file is open in text mode, it must be opened with the correct
           encoding.
+        :param merge_embedded_language: If pygments detects a base and embedded language, the source
+          code counts towards the base language. For example: "JavaScript+Lasso" counts as
+          "JavaScript".
         """
         assert encoding is not None
-        assert generated_regexes is not None
 
         result = None
         lexer = None
         source_code = None
         if file_handle is None:
             source_size = os.path.getsize(source_path)
             if source_size == 0:
@@ -318,25 +321,32 @@
                     source_code = file_handle.read()
             except (LookupError, OSError, UnicodeError) as error:
                 _log.warning("cannot read %s using encoding %s: %s", source_path, encoding, error)
                 result = SourceAnalysis.from_state(source_path, group, SourceState.error, error)
             if result is None:
                 lexer = guess_lexer(source_path, source_code)
                 assert lexer is not None
-        if (result is None) and (len(generated_regexes) != 0):
-            number_line_and_regex = matching_number_line_and_regex(pygount.common.lines(source_code), generated_regexes)
+        actual_generated_regexes = (
+            generated_regexes
+            if generated_regexes is not None
+            else pygount.common.regexes_from(DEFAULT_GENERATED_PATTERNS_TEXT)
+        )
+        if (result is None) and (len(actual_generated_regexes) != 0):
+            number_line_and_regex = matching_number_line_and_regex(
+                pygount.common.lines(source_code), actual_generated_regexes
+            )
             if number_line_and_regex is not None:
                 number, _, regex = number_line_and_regex
                 message = f"line {number} matches {regex}"
                 _log.info("%s: is generated code because %s", source_path, message)
                 result = SourceAnalysis.from_state(source_path, group, SourceState.generated, message)
         if result is None:
             assert lexer is not None
             assert source_code is not None
-            language = lexer.name
+            language = base_language(lexer.name) if merge_embedded_language else lexer.name
             if ("xml" in language.lower()) or (language == "Genshi"):
                 dialect = pygount.xmldialect.xml_dialect(source_path, source_code)
                 if dialect is not None:
                     language = dialect
             _log.info("%s: analyze as %s using encoding %s", source_path, language, encoding)
             mark_to_count_map = {"c": 0, "d": 0, "e": 0, "s": 0}
             for line_parts in _line_parts(lexer, source_code):
@@ -447,15 +457,15 @@
         """
         Possible additional information about :py:attr:`state`:
 
         * :py:attr:`SourceState.duplicate`: path to the original source file
           the :py:attr:`path` is a duplicate of
         * :py:attr:`SourceState.error`: the :py:exc:`Exception` causing the
           error
-        * :py:attr:`SourceState.generated`: a human readable explanation why
+        * :py:attr:`SourceState.generated`: a human-readable explanation why
           the file is considered to be generated
         """
         return self._state_info
 
     @property
     def is_countable(self) -> bool:
         """
@@ -620,15 +630,15 @@
 
 _LANGUAGE_TO_WHITE_WORDS_MAP = {"batchfile": {"@"}, "python": {"pass"}, "sql": {"begin", "end"}}
 for _language in _LANGUAGE_TO_WHITE_WORDS_MAP.keys():
     assert _language.islower()
 
 
 def matching_number_line_and_regex(
-    source_lines: Sequence[str], generated_regexes: Sequence[Pattern], max_line_count: int = 15
+    source_lines: Iterator[str], generated_regexes: Sequence[Pattern], max_line_count: int = 15
 ) -> Optional[Tuple[int, str, Pattern]]:
     """
     The first line and its number (starting with 0) in the source code that
     indicated that the source code is generated.
     :param source_lines: lines of text to scan
     :param generated_regexes: regular expressions a line must match to indicate
         the source code is generated.
@@ -656,15 +666,15 @@
     line.
     """
     assert language_id is not None
     assert language_id.islower()
     return "(),:;[]{}"
 
 
-def white_code_words(language_id: str) -> Dict[str, List[str]]:
+def white_code_words(language_id: str) -> Set[str]:
     """
     Words that do not count as code if it is the only word in a line.
     """
     assert language_id is not None
     assert language_id.islower()
     return _LANGUAGE_TO_WHITE_WORDS_MAP.get(language_id, set())
 
@@ -678,15 +688,15 @@
             newline_index = token_text.find("\n")
         if token_text != "":
             yield token_type, token_text
 
 
 def _pythonized_comments(tokens: Sequence[Tuple[TokenType, str]]) -> Iterator[TokenType]:
     """
-    Similar to tokens but converts strings after a colon (:) to comments.
+    Similar to tokens but converts strings after a colon (`:`) to comments.
     """
     is_after_colon = True
     for token_type, token_text in tokens:
         if is_after_colon and (token_type in pygments.token.String):
             token_type = pygments.token.Comment
         elif token_text == ":":
             is_after_colon = True
@@ -885,11 +895,23 @@
 
 @deprecated(f"use {SourceAnalysis.__name__}.{SourceAnalysis.from_file.__name__}")
 def source_analysis(
     source_path,
     group,
     encoding="automatic",
     fallback_encoding="cp1252",
-    generated_regexes=pygount.common.regexes_from(DEFAULT_GENERATED_PATTERNS_TEXT),
+    generated_regexes: Optional[List[Pattern]] = None,
     duplicate_pool: Optional[DuplicatePool] = None,
 ):
-    return SourceAnalysis.from_file(source_path, group, encoding, fallback_encoding, generated_regexes, duplicate_pool)
+    actual_generated_regexes = (
+        generated_regexes
+        if generated_regexes is not None
+        else pygount.common.regexes_from(DEFAULT_GENERATED_PATTERNS_TEXT)
+    )
+    return SourceAnalysis.from_file(
+        source_path, group, encoding, fallback_encoding, actual_generated_regexes, duplicate_pool
+    )
+
+
+def base_language(language: str) -> str:
+    base_language_match = _BASE_LANGUAGE_REGEX.match(language)
+    return language if base_language_match is None else base_language_match.group("base_language")
```

### Comparing `pygount-1.6.1/pygount/command.py` & `pygount-1.7.0/pygount/command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Command line interface for pygount.
 """
+
 # Copyright (c) 2016-2023, Thomas Aglassinger.
 # All rights reserved. Distributed under the BSD License.
 import argparse
 import contextlib
 import logging
 import os
 import sys
@@ -40,14 +41,17 @@
 _HELP_FORMAT = 'output format, one of: {}; default: "%(default)s"'.format(
     ", ".join(['"' + format + '"' for format in VALID_OUTPUT_FORMATS])
 )
 
 _HELP_GENERATED = """comma separated list of regular expressions to detect
  generated code; default: %(default)s"""
 
+_HELP_MERGE_EMBEDDED_LANGUAGES = """merge counts for embedded languages into
+ their base language; for example, HTML+Jinja2 counts as HTML"""
+
 _HELP_FOLDERS_TO_SKIP = """comma separated list of glob patterns for folder
  names not to analyze. Use "..." as first entry to append patterns to the
  default patterns; default: %(default)s"""
 
 _HELP_NAMES_TO_SKIP = """comma separated list of glob patterns for file names
  not to analyze. Use "..." as first entry to append patterns to the default
  patterns; default: %(default)s"""
@@ -97,14 +101,15 @@
 
     def __init__(self):
         self.set_encodings(_DEFAULT_ENCODING)
         self._folders_to_skip = pygount.common.regexes_from(pygount.analysis.DEFAULT_FOLDER_PATTERNS_TO_SKIP_TEXT)
         self._generated_regexs = pygount.common.regexes_from(pygount.analysis.DEFAULT_GENERATED_PATTERNS_TEXT)
         self._has_duplicates = False
         self._has_summary = False
+        self._has_to_merge_embedded_languages = False
         self._is_verbose = False
         self._names_to_skip = pygount.common.regexes_from(pygount.analysis.DEFAULT_NAME_PATTERNS_TO_SKIP_TEXT)
         self._output = _DEFAULT_OUTPUT
         self._output_format = _DEFAULT_OUTPUT_FORMAT
         self._source_patterns = _DEFAULT_SOURCE_PATTERNS
         self._suffixes = pygount.common.regexes_from(_DEFAULT_SUFFIXES)
 
@@ -164,14 +169,21 @@
     def has_duplicates(self):
         return self._has_duplicates
 
     def set_has_duplicates(self, has_duplicates, source=None):
         self._has_duplicates = bool(has_duplicates)
 
     @property
+    def has_to_merge_embedded_languages(self):
+        return self._has_to_merge_embedded_languages
+
+    def set_has_to_merge_embedded_languages(self, has_to_merge_embedded_languages, source=None):
+        self._has_to_merge_embedded_languages = bool(has_to_merge_embedded_languages)
+
+    @property
     def is_verbose(self):
         return self._is_verbose
 
     def set_is_verbose(self, is_verbose, source=None):
         self._is_verbose = bool(is_verbose)
 
     @property
@@ -243,14 +255,20 @@
             "--generated",
             "-g",
             metavar="PATTERNS",
             default=pygount.analysis.DEFAULT_GENERATED_PATTERNS_TEXT,
             help=_HELP_GENERATED,
         )
         parser.add_argument(
+            "--merge-embedded-languages",
+            "-m",
+            action="store_true",
+            help=_HELP_MERGE_EMBEDDED_LANGUAGES,
+        )
+        parser.add_argument(
             "--names-to-skip",
             "-N",
             metavar="PATTERNS",
             default=pygount.analysis.DEFAULT_NAME_PATTERNS_TO_SKIP_TEXT,
             help=_HELP_NAMES_TO_SKIP,
         )
         parser.add_argument(
@@ -308,14 +326,15 @@
             arguments = sys.argv[1:]
         args, default_encoding, fallback_encoding = self.parsed_args(arguments)
         self.set_default_encoding(default_encoding, "option --encoding")
         self.set_fallback_encoding(fallback_encoding, "option --encoding")
         self.set_folders_to_skip(args.folders_to_skip, "option --folders-to-skip")
         self.set_generated_regexps(args.generated, "option --generated")
         self.set_has_duplicates(args.duplicates, "option --duplicates")
+        self.set_has_to_merge_embedded_languages(args.merge_embedded_languages, "option --merge-embedded-languages")
         self.set_is_verbose(args.verbose, "option --verbose")
         self.set_names_to_skip(args.names_to_skip, "option --folders-to-skip")
         self.set_output(args.out, "option --out")
         self.set_output_format(args.format, "option --format")
         self.set_source_patterns(args.source_patterns, "option PATTERNS")
         self.set_suffixes(args.suffix, "option --suffix")
 
@@ -341,14 +360,15 @@
                                 pygount.analysis.SourceAnalysis.from_file(
                                     source_path,
                                     group,
                                     self.default_encoding,
                                     self.fallback_encoding,
                                     generated_regexes=self._generated_regexs,
                                     duplicate_pool=duplicate_pool,
+                                    merge_embedded_language=self.has_to_merge_embedded_languages,
                                 )
                             )
                     finally:
                         progress.stop()
 
 
 def pygount_command(arguments=None):
```

### Comparing `pygount-1.6.1/pygount/common.py` & `pygount-1.7.0/pygount/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Common classes and functions for pygount.
 """
+
 # Copyright (c) 2016-2023, Thomas Aglassinger.
 # All rights reserved. Distributed under the BSD License.
 import fnmatch
 import functools
 import inspect
 import re
 import warnings
```

### Comparing `pygount-1.6.1/pygount/git_storage.py` & `pygount-1.7.0/pygount/git_storage.py`

 * *Files identical despite different names*

### Comparing `pygount-1.6.1/pygount/lexers.py` & `pygount-1.7.0/pygount/lexers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Additional lexers for pygount that fill gaps left by :py:mod:`pygments`.
 """
+
 # Copyright (c) 2016-2023, Thomas Aglassinger.
 # All rights reserved. Distributed under the BSD License.
 import pygments.lexer
 import pygments.lexers
 import pygments.token
 import pygments.util
```

### Comparing `pygount-1.6.1/pygount/summary.py` & `pygount-1.7.0/pygount/summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Summaries of analyses of multiple source codes.
 """
+
 # Copyright (c) 2016-2023, Thomas Aglassinger.
 # All rights reserved. Distributed under the BSD License.
 import functools
 import re
 from typing import Dict, Hashable
 
 from .analysis import SourceAnalysis
```

### Comparing `pygount-1.6.1/pygount/write.py` & `pygount-1.7.0/pygount/write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Writers to store the results of a pygount analysis.
 """
+
 # Copyright (c) 2016-2023, Thomas Aglassinger.
 # All rights reserved. Distributed under the BSD License.
 import datetime
 import json
 import math
 import os
 from xml.etree import ElementTree
@@ -27,15 +28,15 @@
     def __init__(self, target_stream):
         self._target_stream = target_stream
         try:
             self.target_name = self._target_stream.name
         except AttributeError:
             self.target_name = "<io>"
         self.project_summary = ProjectSummary()
-        self.started_at = datetime.datetime.utcnow()
+        self.started_at = self._utc_now()
         self.finished_at = None
         self.files_per_second = 0
         self.lines_per_second = 0
         self.duration = None
         self.duration_in_seconds = 0.0
         self.has_to_track_progress = True
 
@@ -47,22 +48,27 @@
         return False
 
     def add(self, source_analysis):
         self.project_summary.add(source_analysis)
 
     def close(self):
         self.project_summary.update_file_percentages()
-        self.finished_at = datetime.datetime.utcnow()
+        self.finished_at = self._utc_now()
         self.duration = self.finished_at - self.started_at
         self.duration_in_seconds = max(
             0.001, self.duration.microseconds * 1e-6 + self.duration.seconds + self.duration.days * 3600 * 24
         )
         self.lines_per_second = self.project_summary.total_line_count / self.duration_in_seconds
         self.files_per_second = self.project_summary.total_file_count / self.duration_in_seconds
 
+    @staticmethod
+    def _utc_now() -> datetime.datetime:
+        # After switching to Python 3.11+, we can change this to `now(datetime.UTC)`.
+        return datetime.datetime.now(datetime.timezone.utc)
+
 
 class LineWriter(BaseWriter):
     """
     Writer that simply writes a line of text for each source code.
     """
 
     def __init__(self, target_stream):
```

### Comparing `pygount-1.6.1/pygount/xmldialect.py` & `pygount-1.7.0/pygount/xmldialect.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Function to obtain the language dialect used by XML source code.
 """
+
 # Copyright (c) 2016-2023, Thomas Aglassinger.
 # All rights reserved. Distributed under the BSD License.
 import logging
 import re
 import xml.sax
 
 # TODO #10: Replace regex for DTD by working DTD handler.
```

### Comparing `pygount-1.6.1/pyproject.toml` & `pygount-1.7.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 line-length = 120
 include = '\.pyi?$'
 target-version = [
     "py38",
     "py39",
     "py310",
     "py311",
+    "py312",
 ]
 exclude = '''
 /(
     \.eggs
   | \.git
   | build
   | dist
@@ -29,15 +30,15 @@
 ]
 testpaths = [
     "tests",
 ]
 
 [tool.poetry]
 name = "pygount"
-version = "1.6.1"
+version = "1.7.0"
 description = "count source lines of code (SLOC) using pygments"
 readme = "README.md"
 authors = ["Thomas Aglassinger <roskakori@users.sourceforge.net>"]
 license = "BSD"
 homepage = "https://github.com/roskakori/pygount"
 repository = "https://github.com/roskakori/pygount.git"
 documentation = "https://pygount.readthedocs.io"
@@ -50,35 +51,36 @@
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Software Development",
 ]
 packages = [
     { include = "pygount" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8, <4"
+python = ">=3.8, <3.13"  # NOTE We cannot use <4 because of coveralls.
 pygments = "^2"
 chardet = "^5"
 rich = ">=9, <14"
-gitpython = "^3.1.31"
+gitpython = "^3"
 
 [tool.poetry.dev-dependencies]
-coveralls = "^3"
-coverage = "^6"
-pytest = "^7"
-pytest-cov = "^4"
+coveralls = "^4"
+coverage = "^7"
+pytest = "^8"
+pytest-cov = "^5"
 pre-commit = "^3"
 pur = "^7"
-twine = "^4"
+twine = "^5"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 Sphinx = "^7"
 
@@ -89,9 +91,9 @@
 "Issue Tracker" = "https://github.com/roskakori/pygount/issues"
 "Changes" = "https://pygount.readthedocs.io/en/latest/changes.html"
 
 [pycodestyle]
 max-line-length = 120
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.8.1"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pygount-1.6.1/PKG-INFO` & `pygount-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: pygount
-Version: 1.6.1
+Version: 1.7.0
 Summary: count source lines of code (SLOC) using pygments
 Home-page: https://github.com/roskakori/pygount
 License: BSD
 Keywords: code analysis,count,SLOC
 Author: Thomas Aglassinger
 Author-email: roskakori@users.sourceforge.net
-Requires-Python: >=3.8,<4
+Requires-Python: >=3.8,<3.13
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Requires-Dist: chardet (>=5,<6)
-Requires-Dist: gitpython (>=3.1.31,<4.0.0)
+Requires-Dist: gitpython (>=3,<4)
 Requires-Dist: pygments (>=2,<3)
 Requires-Dist: rich (>=9,<14)
 Project-URL: Changes, https://pygount.readthedocs.io/en/latest/changes.html
 Project-URL: Documentation, https://pygount.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/roskakori/pygount/issues
 Project-URL: Repository, https://github.com/roskakori/pygount.git
 Description-Content-Type: text/markdown
```

