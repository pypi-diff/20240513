# Comparing `tmp/exetest-0.9.1.tar.gz` & `tmp/exetest-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exetest-0.9.1.tar", last modified: Mon Mar 18 15:52:56 2024, max compression
+gzip compressed data, was "exetest-0.9.2.tar", last modified: Mon May 13 09:28:32 2024, max compression
```

## Comparing `exetest-0.9.1.tar` & `exetest-0.9.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 ggiraud   (1000) ggiraud   (1000)        0 2024-03-18 15:52:56.013184 exetest-0.9.1/
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)      699 2024-03-18 15:52:56.013184 exetest-0.9.1/PKG-INFO
-drwxr-xr-x   0 ggiraud   (1000) ggiraud   (1000)        0 2024-03-18 15:52:56.013184 exetest-0.9.1/exetest/
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)      186 2023-11-30 08:15:26.698418 exetest-0.9.1/exetest/__init__.py
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     4973 2024-03-18 15:47:15.583173 exetest-0.9.1/exetest/dataframe_utils.py
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     8148 2023-10-23 03:34:07.458212 exetest-0.9.1/exetest/diff_utils.py
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)      443 2024-03-18 15:50:16.763180 exetest-0.9.1/exetest/env_vars.py
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)    22847 2024-03-18 15:50:16.383180 exetest-0.9.1/exetest/exetest_decorator.py
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     1717 2023-10-23 03:45:50.258216 exetest-0.9.1/exetest/expects_exception.py
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     7458 2024-02-20 11:00:23.675917 exetest-0.9.1/exetest/misc_utils.py
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     7082 2024-03-18 15:50:16.543180 exetest-0.9.1/exetest/runmain.py
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)       65 2022-04-25 16:23:33.239740 exetest-0.9.1/setup.cfg
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     1563 2024-03-18 15:47:30.343175 exetest-0.9.1/setup.py
+drwxr-xr-x   0 ggiraud   (1000) ggiraud   (1000)        0 2024-05-13 09:28:32.266216 exetest-0.9.2/
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)      699 2024-05-13 09:28:32.266216 exetest-0.9.2/PKG-INFO
+drwxr-xr-x   0 ggiraud   (1000) ggiraud   (1000)        0 2024-05-13 09:28:32.266216 exetest-0.9.2/exetest/
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)      183 2024-05-13 08:36:57.942206 exetest-0.9.2/exetest/__init__.py
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     6755 2024-05-13 09:19:49.446325 exetest-0.9.2/exetest/dataframe_utils.py
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     7914 2024-05-13 08:36:57.942206 exetest-0.9.2/exetest/diff_utils.py
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)      429 2024-05-13 08:36:57.942206 exetest-0.9.2/exetest/env_vars.py
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)    22270 2024-05-13 08:36:57.942206 exetest-0.9.2/exetest/exetest_decorator.py
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     1670 2024-05-13 08:36:57.942206 exetest-0.9.2/exetest/expects_exception.py
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     7196 2024-05-13 08:36:57.952206 exetest-0.9.2/exetest/misc_utils.py
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     6885 2024-05-13 08:36:57.952206 exetest-0.9.2/exetest/runmain.py
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)       62 2024-05-13 08:26:18.252304 exetest-0.9.2/setup.cfg
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     1539 2024-05-13 09:22:06.446295 exetest-0.9.2/setup.py
```

### Comparing `exetest-0.9.1/PKG-INFO` & `exetest-0.9.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: exetest
-Version: 0.9.1
+Version: 0.9.2
 Summary: A pytest-based test framework for black-box approach to testing executables
 Home-page: https://github.com/Guillaume227/exetest
 Author: Guillaume227
 Author-email: guillaume227@gmail.com
 License: MIT
 Download-URL: https://github.com/Guillaume227/exetest/archive/v0.1-alpha.tar.gz
 Description: UNKNOWN
```

### Comparing `exetest-0.9.1/exetest/diff_utils.py` & `exetest-0.9.2/exetest/diff_utils.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,234 +1,234 @@
-import filecmp
-import os
-import os.path
-import platform
-import sys
-import difflib
-
-# import subprocess
-# import numpy as np
-# import pandas as pd
-
-
-globalIgnoreLines = {}
-
-
-class FilteredFileReader:
-    """
-    a file reader that optionally selects lines containing a substring
-    """
-
-    def __init__(self, file_path, filter_tag=None, skip_lines=None):
-        """
-
-        :param file_path:
-        :param filter_tag: keep only lines containing that substring
-        :param skip_lines: list of line indexes to keep
-        """
-        self._file = open(file_path, 'r')
-        self._filter_tag = filter_tag
-        self._skip_lines = skip_lines
-
-    def readlines(self):
-
-        if self._filter_tag is None:
-            lines = self._file.readlines()
-        else:
-            lines = [line.split(self._filter_tag)[-1] for line in self._file.readlines()]
-
-        if self._skip_lines is None:
-            return lines
-        else:
-            return [line for i, line in enumerate(lines) if i not in self._skip_lines]
-
-
-def default_file_diff(file_path1, file_path2,
-                      print_diff=True,
-                      ignore_patterns=tuple(),
-                      filter_tag=None,
-                      skip_lines=None,
-                      max_diff_in_log=25):
-    """ compare two files line by line:
-        @:return: False if a difference is found
-    """
-
-    try:
-        filter_tag1, filter_tag2 = filter_tag
-    except:
-        filter_tag1 = filter_tag2 = filter_tag
-
-    file1 = FilteredFileReader(file_path1, filter_tag=filter_tag1, skip_lines=skip_lines)
-    file2 = FilteredFileReader(file_path2, filter_tag=filter_tag2, skip_lines=skip_lines)
-
-    try:
-        diff = difflib.unified_diff(file1.readlines(), file2.readlines(),
-                                    # fromfile=file_path1, tofile=file_path2,
-                                    n=0  # no context lines
-                                    )
-
-        num_diffs = 0
-        ignored_diffs = 0
-        first_diff = True
-
-        for diff_line in diff:
-
-            if first_diff:
-                first_diff = False
-                print()
-
-            if any(diff_line.startswith(tag) for tag in ['---', '+++', '@@ ']):
-                # skip diff output meta data
-                continue
-            else:
-
-                ignore = False
-                for ignore_pattern in ignore_patterns:
-                    # assume it's a list of patterns
-                    if callable(ignore_pattern):
-                        ignore = ignore_pattern(diff_line)
-                    else:
-                        ignore = ignore_pattern in diff_line
-
-                    if ignore:
-                        ignored_diffs += 1
-                        break
-
-                if ignore:
-                    continue
-
-            if print_diff:
-                print(diff_line, end='', file=sys.stderr)
-
-            num_diffs += 1
-
-            if max_diff_in_log == 0:
-                return False
-
-            if num_diffs >= max_diff_in_log:
-                print(f'Only showing {max_diff_in_log} differences out of {num_diffs} '
-                      f'- diff file manually for more details', file=sys.stderr)
-                break
-
-        if num_diffs == 0:
-            if ignored_diffs > 0 and platform.system() != 'Windows':
-                print('        Ignoring Diff on {0} coming from line endings unix vs windows'.format(file_path1))
-
-            return True
-
-        return False
-
-    except UnicodeDecodeError:
-        print("     skipping text diff on non-text file:", file_path1)
-        return False
-
-
-def diff_dirs(ref_dir, test_dir, print_diff=True, ignore_lines=None, comparators=None, ignore_missing=False):
-    """
-    recursive directory compare:
-    :param ref_dir:
-    :param test_dir:
-    :param print_diff:
-    :param ignore_lines: {file_ext: [ string1, string2, ... ]}
-        where the differing line will be ignored if it contains any of the strings
-    :param comparators: {file_ext: comparator_func}
-        where comparator_func: f(file1, file2) -> bool (True if no diff)
-    :param ignore_missing:
-    :return: differing files in @ref_dir vs @test_dir
-    """
-
-    dir_comp_res = filecmp.dircmp(ref_dir, test_dir)
-
-    # print out what was found in each directory for information
-    if print_diff:
-        print()
-        dir_comp_res.report()
-        print()
-
-    if not ignore_missing:
-        # check number of files is the same
-        assert len(dir_comp_res.right_only) == 0, f'Files only in {dir_comp_res.right}: {dir_comp_res.right_only}'
-        assert len(dir_comp_res.left_only) == 0, f'Files only in {dir_comp_res.left}: {dir_comp_res.left_only}'
-
-        # check names of files are the same
-        assert set(dir_comp_res.right_list).issuperset(dir_comp_res.left_list), \
-            f'Different file names found {set(dir_comp_res.right_list).difference(dir_comp_res.left_list)}'
-
-    for diff_file in dir_comp_res.diff_files:
-
-        file_name1 = os.path.join(ref_dir, diff_file)
-        file_name2 = os.path.join(test_dir, diff_file)
-
-        if ignore_missing:
-            if not os.path.exists(file_name1):
-                missing = file_name1
-            elif not os.path.exists(file_name2):
-                missing = file_name2
-            else:
-                missing = None
-
-            if missing:
-                print(f'missing directory', missing, file=sys.stderr)
-                continue
-
-        found_comparator = False
-        # use a custom comparator fun if it exists for that file extension
-        for comparator_dict in [comparators, globalIgnoreLines]:
-            for file_ext in comparator_dict:
-                if diff_file.endswith(file_ext):
-                    found_comparator = True
-
-                    if comparator_dict[file_ext](file_name1, file_name2):
-                        yield diff_file
-
-                    break
-
-        if not found_comparator:
-            if default_file_diff(file_name1, file_name2, print_diff, ignore_lines):
-                yield diff_file
-
-    for file_name in os.listdir(ref_dir):
-        if os.path.isdir(os.path.join(ref_dir, file_name)):
-            dir_path1 = os.path.join(ref_dir, file_name)
-            dir_path2 = os.path.join(test_dir, file_name)
-
-            if ignore_missing:
-                if not os.path.exists(dir_path1):
-                    missing = dir_path1
-                elif not os.path.exists(dir_path2):
-                    missing = dir_path2
-                else:
-                    missing = None
-
-                if missing:
-                    print('Missing directory', missing, file=sys.stderr)
-                    continue
-
-            for diff_file in diff_dirs(dir_path1, dir_path2, print_diff=print_diff,
-                                       ignore_lines=ignore_lines,
-                                       comparators=comparators,
-                                       ignore_missing=ignore_missing):
-                yield os.path.join(file_name, diff_file)
-
-
-class FileComparator:
-
-    def __init__(self, include_line_if_contains=None, skip_lines=None, **kwargs):
-
-        self.include_line_if_contains = include_line_if_contains
-        self.skip_lines = skip_lines
-        self.kwargs = kwargs
-
-    def description(self):
-        if self.include_line_if_contains:
-            if isinstance(self.include_line_if_contains, str):
-                include_str = f'"{self.include_line_if_contains}"'
-            else:
-                include_str = ", ".join(f'"{line}"' for line in self.include_line_if_contains if line is not None)
-            return f'filter lines on {include_str}'
-        return ''
-
-    def __call__(self, *args, **kwargs):
-        return default_file_diff(*args, **kwargs,
-                                 filter_tag=self.include_line_if_contains,
-                                 skip_lines=self.skip_lines,
-                                 **self.kwargs)
+import filecmp
+import os
+import os.path
+import platform
+import sys
+import difflib
+
+# import subprocess
+# import numpy as np
+# import pandas as pd
+
+
+globalIgnoreLines = {}
+
+
+class FilteredFileReader:
+    """
+    a file reader that optionally selects lines containing a substring
+    """
+
+    def __init__(self, file_path, filter_tag=None, skip_lines=None):
+        """
+
+        :param file_path:
+        :param filter_tag: keep only lines containing that substring
+        :param skip_lines: list of line indexes to keep
+        """
+        self._file = open(file_path, 'r')
+        self._filter_tag = filter_tag
+        self._skip_lines = skip_lines
+
+    def readlines(self):
+
+        if self._filter_tag is None:
+            lines = self._file.readlines()
+        else:
+            lines = [line.split(self._filter_tag)[-1] for line in self._file.readlines()]
+
+        if self._skip_lines is None:
+            return lines
+        else:
+            return [line for i, line in enumerate(lines) if i not in self._skip_lines]
+
+
+def default_file_diff(file_path1, file_path2,
+                      print_diff=True,
+                      ignore_patterns=tuple(),
+                      filter_tag=None,
+                      skip_lines=None,
+                      max_diff_in_log=25):
+    """ compare two files line by line:
+        @:return: False if a difference is found
+    """
+
+    try:
+        filter_tag1, filter_tag2 = filter_tag
+    except:
+        filter_tag1 = filter_tag2 = filter_tag
+
+    file1 = FilteredFileReader(file_path1, filter_tag=filter_tag1, skip_lines=skip_lines)
+    file2 = FilteredFileReader(file_path2, filter_tag=filter_tag2, skip_lines=skip_lines)
+
+    try:
+        diff = difflib.unified_diff(file1.readlines(), file2.readlines(),
+                                    # fromfile=file_path1, tofile=file_path2,
+                                    n=0  # no context lines
+                                    )
+
+        num_diffs = 0
+        ignored_diffs = 0
+        first_diff = True
+
+        for diff_line in diff:
+
+            if first_diff:
+                first_diff = False
+                print()
+
+            if any(diff_line.startswith(tag) for tag in ['---', '+++', '@@ ']):
+                # skip diff output meta data
+                continue
+            else:
+
+                ignore = False
+                for ignore_pattern in ignore_patterns:
+                    # assume it's a list of patterns
+                    if callable(ignore_pattern):
+                        ignore = ignore_pattern(diff_line)
+                    else:
+                        ignore = ignore_pattern in diff_line
+
+                    if ignore:
+                        ignored_diffs += 1
+                        break
+
+                if ignore:
+                    continue
+
+            if print_diff:
+                print(diff_line, end='', file=sys.stderr)
+
+            num_diffs += 1
+
+            if max_diff_in_log == 0:
+                return False
+
+            if num_diffs >= max_diff_in_log:
+                print(f'Only showing {max_diff_in_log} differences out of {num_diffs} '
+                      f'- diff file manually for more details', file=sys.stderr)
+                break
+
+        if num_diffs == 0:
+            if ignored_diffs > 0 and platform.system() != 'Windows':
+                print('        Ignoring Diff on {0} coming from line endings unix vs windows'.format(file_path1))
+
+            return True
+
+        return False
+
+    except UnicodeDecodeError:
+        print("     skipping text diff on non-text file:", file_path1)
+        return False
+
+
+def diff_dirs(ref_dir, test_dir, print_diff=True, ignore_lines=None, comparators=None, ignore_missing=False):
+    """
+    recursive directory compare:
+    :param ref_dir:
+    :param test_dir:
+    :param print_diff:
+    :param ignore_lines: {file_ext: [ string1, string2, ... ]}
+        where the differing line will be ignored if it contains any of the strings
+    :param comparators: {file_ext: comparator_func}
+        where comparator_func: f(file1, file2) -> bool (True if no diff)
+    :param ignore_missing:
+    :return: differing files in @ref_dir vs @test_dir
+    """
+
+    dir_comp_res = filecmp.dircmp(ref_dir, test_dir)
+
+    # print out what was found in each directory for information
+    if print_diff:
+        print()
+        dir_comp_res.report()
+        print()
+
+    if not ignore_missing:
+        # check number of files is the same
+        assert len(dir_comp_res.right_only) == 0, f'Files only in {dir_comp_res.right}: {dir_comp_res.right_only}'
+        assert len(dir_comp_res.left_only) == 0, f'Files only in {dir_comp_res.left}: {dir_comp_res.left_only}'
+
+        # check names of files are the same
+        assert set(dir_comp_res.right_list).issuperset(dir_comp_res.left_list), \
+            f'Different file names found {set(dir_comp_res.right_list).difference(dir_comp_res.left_list)}'
+
+    for diff_file in dir_comp_res.diff_files:
+
+        file_name1 = os.path.join(ref_dir, diff_file)
+        file_name2 = os.path.join(test_dir, diff_file)
+
+        if ignore_missing:
+            if not os.path.exists(file_name1):
+                missing = file_name1
+            elif not os.path.exists(file_name2):
+                missing = file_name2
+            else:
+                missing = None
+
+            if missing:
+                print(f'missing directory', missing, file=sys.stderr)
+                continue
+
+        found_comparator = False
+        # use a custom comparator fun if it exists for that file extension
+        for comparator_dict in [comparators, globalIgnoreLines]:
+            for file_ext in comparator_dict:
+                if diff_file.endswith(file_ext):
+                    found_comparator = True
+
+                    if comparator_dict[file_ext](file_name1, file_name2):
+                        yield diff_file
+
+                    break
+
+        if not found_comparator:
+            if default_file_diff(file_name1, file_name2, print_diff, ignore_lines):
+                yield diff_file
+
+    for file_name in os.listdir(ref_dir):
+        if os.path.isdir(os.path.join(ref_dir, file_name)):
+            dir_path1 = os.path.join(ref_dir, file_name)
+            dir_path2 = os.path.join(test_dir, file_name)
+
+            if ignore_missing:
+                if not os.path.exists(dir_path1):
+                    missing = dir_path1
+                elif not os.path.exists(dir_path2):
+                    missing = dir_path2
+                else:
+                    missing = None
+
+                if missing:
+                    print('Missing directory', missing, file=sys.stderr)
+                    continue
+
+            for diff_file in diff_dirs(dir_path1, dir_path2, print_diff=print_diff,
+                                       ignore_lines=ignore_lines,
+                                       comparators=comparators,
+                                       ignore_missing=ignore_missing):
+                yield os.path.join(file_name, diff_file)
+
+
+class FileComparator:
+
+    def __init__(self, include_line_if_contains=None, skip_lines=None, **kwargs):
+
+        self.include_line_if_contains = include_line_if_contains
+        self.skip_lines = skip_lines
+        self.kwargs = kwargs
+
+    def description(self):
+        if self.include_line_if_contains:
+            if isinstance(self.include_line_if_contains, str):
+                include_str = f'"{self.include_line_if_contains}"'
+            else:
+                include_str = ", ".join(f'"{line}"' for line in self.include_line_if_contains if line is not None)
+            return f'filter lines on {include_str}'
+        return ''
+
+    def __call__(self, *args, **kwargs):
+        return default_file_diff(*args, **kwargs,
+                                 filter_tag=self.include_line_if_contains,
+                                 skip_lines=self.skip_lines,
+                                 **self.kwargs)
```

### Comparing `exetest-0.9.1/exetest/exetest_decorator.py` & `exetest-0.9.2/exetest/exetest_decorator.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,577 +1,577 @@
-import os
-import os.path
-import pathlib
-import traceback
-from . import misc_utils
-from .misc_utils import working_dir, rmdir
-from .diff_utils import FileComparator, diff_dirs
-from functools import wraps
-import shutil
-import sys
-import unittest
-from .env_vars import ExeTestEnvVars
-import pytest
-
-
-FORCE_REBASE = 'FORCE'
-REBASE_YES_DEFAULT = 'y'
-
-
-def skip_test(reason=''):
-    """
-    A decorator for marking tests as skipped and still allowing to force-run them.
-    Bypassing behavior is triggered by the presence of an environment variable.
-    :param reason: why the test is being skipped
-    """
-    if ExeTestEnvVars.DISABLE_SKIP in os.environ:
-        return lambda x: x
-    else:
-        return pytest.mark.skip(reason=reason)
-
-
-def skip_module(reason=''):
-    if ExeTestEnvVars.DISABLE_SKIP not in os.environ:
-        pytest.skip(reason, allow_module_level=True)
-
-
-class ExeTestCaseDecorator:
-    """
-    A test case decorator for testing an executable outputs
-    by comparing new output to reference output
-    """
-
-    def __init__(self,
-                 exe: str,
-                 test_root: str = '.',  # =os.path.dirname(__file__),
-                 ref_dir: str = 'ref_dir',
-                 out_dir: str = 'out_dir',
-                 exe_args=None,
-                 compare_spec=None,
-                 run_from_out_dir: bool = True,
-                 test_name_as_dir: bool = True,
-                 nested_ref_dir: bool = True,
-                 nested_out_dir: bool = False, 
-                 comparators=None,
-                 ref_diff_only: bool = False,
-                 exception_handler=None,
-                 env_vars=None,
-                 pre_cmd=None,
-                 exe_path_ref=None,
-                 log_output_path=None):
-        """
-
-        :param exe: path to the executable to test
-        :param test_root: working directory for test execution from which ref_dir/out_dir paths are defined if relative.
-        :param ref_dir: absolute path or relative to test_root directory where test case is defined
-        :param out_dir: directory to write test output to
-        :param exe_args: test executable arguments in string format - as would be passed to command line
-        :param run_from_out_dir: whether the executable working directory should be the output directory
-        :param test_name_as_dir: whether the test name should be used to infer the ref and output directories
-        :param nested_ref_dir: whether ref_dir should be nested in the test_name directory (otherwise, test_name is nested under ref_dir)
-        :param nested_out_dir: whether out_dir should be nested in the test_name directory (otherwise, test_name is nested under out_dir)
-        :param comparators:
-        :param ref_diff_only: files in out_dir but not in ref_dir will not be flagged
-        :param exception_handler: what to do in case of exception
-        :param env_vars: environment variables to populate for the test run
-        :param pre_cmd: a command to run before the executable is run
-        :param exe_path_ref:
-        :param log_output_path:
-        """
-
-        self.exe_path_ref = exe_path_ref if exe_path_ref else {}
-
-        def get_test_exe(val):
-            if val in self.exe_path_ref:
-                return self.exe_path_ref[val]
-            elif val:
-                if os.path.isdir(val):
-                    return os.path.join(val, os.path.basename(exe))
-                else:
-                    return val
-            else:
-                return exe
-
-        use_test_exe = os.environ.get(ExeTestEnvVars.USE_EXE)
-
-        # if USE_TEST_EXE has special target value, run against reference executable
-        if use_test_exe is not None:
-            self.exe_path = get_test_exe(use_test_exe)
-        else:
-            self.exe_path = exe
-
-        self.test_root = test_root
-        self.REF_OUTPUT_DIR = ref_dir
-        self.TMP_OUTPUT_DIR = out_dir
-        self.test_name_as_dir = test_name_as_dir
-        self.run_from_out_dir = run_from_out_dir
-        self.ref_diff_only = ref_diff_only
-
-        self.test_name = ''
-        self.comparators = comparators or {}
-        self.exception_handler = exception_handler
-        self.common_env_vars = env_vars or dict()
-        self.pre_cmd = pre_cmd if pre_cmd else []
-        self.exe_args = exe_args
-        self.log_output_path = log_output_path
-
-        self.verbose = ExeTestEnvVars.VERBOSE in os.environ
-        if ExeTestEnvVars.NO_RUN in os.environ:
-            self.norun = os.environ[ExeTestEnvVars.NO_RUN]
-            if not self.norun:
-                self.norun = 'default'
-        else:
-            self.norun = None
-
-        self._compare_spec = compare_spec
-        self._nested_ref_dir = nested_ref_dir
-        self._nested_out_dir = nested_out_dir
-        self._num_lines_diff = int(os.environ.get(ExeTestEnvVars.NUM_DIFFS, 20))
-        self._file_filter = os.environ.get(ExeTestEnvVars.FILE_FILTER, '').split('+')
-
-    @staticmethod
-    def get_test_subdir(test_name):
-        return test_name
-
-    def get_out_dir(self, test_name):
-        return self.make_dir_path(self.TMP_OUTPUT_DIR, test_name, self._nested_out_dir)
-
-    def get_ref_dir(self, test_name):
-        return self.make_dir_path(self.REF_OUTPUT_DIR, test_name, self._nested_ref_dir)
-
-    def __call__(self,
-                 exe_args=None,
-                 extra_args=None,
-                 compare_spec=None,
-                 pre_cmd=None,
-                 env_vars=None,
-                 post_cmd=None,
-                 owners=None):
-        """
-
-        :param exe_args: overrides arguments specified in the constructor
-        :param extra_args: appends arguments to the ones specified in the constructor
-        :param compare_spec:
-        :param pre_cmd:
-        :param env_vars:
-        :param post_cmd:
-        :param owners:
-        :return:
-        """
-        all_env_vars = dict(self.common_env_vars)
-        if env_vars:
-            all_env_vars.update(env_vars)
-
-        pre_cmds = self.pre_cmd
-        if pre_cmd:
-            if isinstance(pre_cmd, str):
-                pre_cmds = pre_cmds + [pre_cmd]
-            else:
-                pre_cmds = pre_cmds + pre_cmd
-
-        if exe_args is None:
-            if self.exe_args is not None:
-                exe_args = self.exe_args
-            else:
-                exe_args = ''
-
-        if extra_args is not None:
-            exe_args += ' ' + extra_args
-
-        if compare_spec is None:
-            compare_spec = self._compare_spec
-
-        self._compare_only = ExeTestEnvVars.COMPARE_ONLY in os.environ
-
-        def func_wrapper(test_func):
-            """
-            :param test_func:
-            :return: decorated function
-            """
-            test_name = test_func.__name__.split("_", 1)[-1]
-            import inspect
-            parent_module_name = inspect.getmodule(test_func).__name__
-
-            resolved_env_vars = {}
-            for name, value in all_env_vars.items():
-                resolved_env_vars[name] = str(value).format(test_name=test_name)
-
-            @wraps(test_func)
-            def f(*args, **kwargs):
-                ret = test_func(*args, **kwargs)
-                try:
-                    self.run_test(exe_args,
-                                  compare_spec,
-                                  pre_cmd=pre_cmds,
-                                  env_vars=resolved_env_vars,
-                                  post_cmd=post_cmd,
-                                  test_name=test_name,
-                                  parent_module_name=parent_module_name,
-                                  verbose=self.verbose)
-                except unittest.SkipTest:
-                    raise
-
-                return ret
-
-            def doc_gist(func):
-                """
-                :param func:
-                :return:
-                """
-
-                if func.__doc__:
-                    for line in func.__doc__.splitlines():
-                        if line.strip():
-                            return line.strip()
-                    return ""
-
-            # set description attribute for test framework to display
-            doc = doc_gist(test_func)
-            if doc:
-                f.description = (test_name + ": ").ljust(10) + doc
-            else:
-                f.description = test_name.ljust(10)
-
-            return f
-
-        return func_wrapper
-
-    @classmethod
-    def do_test_rebase(cls):
-        """
-        :return: whether to run test in rebase mode, whether to not prompt for applying changes
-        """
-        val = os.getenv(ExeTestEnvVars.REBASE)
-        if val is None:
-            return False, False, False
-
-        do_rebase = val != '0'
-        return do_rebase, do_rebase and val != FORCE_REBASE, val == REBASE_YES_DEFAULT
-
-    def raise_exception(self, msg):
-        raise Exception(msg)
-
-    def run_test(self, exe_args, compare_spec,
-                 pre_cmd, env_vars, post_cmd,
-                 test_name, parent_module_name,
-                 verbose):
-
-        do_rebase, rebase_with_prompt, rebase_yes_default = self.do_test_rebase()
-        if rebase_with_prompt:
-            if not sys.stdout.isatty():
-                self.raise_exception("cannot rebase unless confirmation "
-                                     "prompt is displayed in terminal. "
-                                     "Make sure you are using --capture=no pytest option")
-
-        with working_dir(self.test_root):
-
-            files_to_compare = self.get_files_to_compare(test_name, compare_spec)
-
-            if compare_spec and not files_to_compare.items():
-                self.raise_exception(f"No reference output files for {compare_spec}")
-
-            tmp_output_dir = self.get_out_dir(test_name)
-            run_from_dir = os.path.join(self.test_root, tmp_output_dir) \
-                if self.run_from_out_dir else self.test_root
-
-        if not self._compare_only:
-            self.clear_dir(tmp_output_dir, recreate=True)
-
-        with working_dir(run_from_dir):
-            try:
-                misc_utils.exec_cmdline(self.exe_path,
-                                        exe_args,
-                                        pre_cmd=pre_cmd,
-                                        env_vars=env_vars,
-                                        post_cmd=post_cmd,
-                                        log_save_path=self.log_output_path,
-                                        norun=self.norun or self._compare_only,
-                                        verbose=verbose)
-            except Exception as exc:
-                if self.exception_handler:
-                    self.exception_handler(exc)
-                else:
-                    raise
-
-        if self.norun:
-            if self.norun == 'ctest':
-                print()
-                print('|'.join(
-                    str(item) for item in ((parent_module_name.replace('.', '/') + '.py::test_' + test_name),
-                                           run_from_dir,
-                                           ' '.join(f'{key}={val}' for key, val in env_vars.items()),
-                                           os.path.basename(self.exe_path),
-                                           exe_args)))
-            if not self._compare_only:
-                # this will mark the test as skipped
-                pytest.skip("no-run mode")
-
-        with working_dir(self.test_root):
-
-            if do_rebase:
-                self.run_rebase_compare(files_to_compare,
-                                        force_rebase=not rebase_with_prompt,
-                                        rebase_prompt_default=rebase_yes_default)
-            else:
-                self.run_compare(files_to_compare)
-
-    def run_compare(self, files_to_compare):
-
-        for _ref_file, new_file in files_to_compare.items():
-            if not os.path.exists(new_file):
-                self.raise_exception(f"Missing output file: {new_file}")
-
-        for ref_file, new_file in files_to_compare.items():
-            has_ref = os.path.exists(ref_file)
-            has_new = os.path.exists(new_file)
-            if not has_ref and not has_new:
-                self.raise_exception(f"Missing both ref and new files:\n{ref_file}\n{new_file}")
-            else:
-                if not has_ref:
-                    self.raise_exception(f"Missing reference file: {ref_file} - "
-                                         f"you can rebase with --rebase option")
-                if not has_new:
-                    while not os.path.exists(os.path.dirname(new_file)):
-                        new_file = os.path.dirname(new_file)
-                    self.raise_exception(f"Missing output file: {new_file}")
-
-        num_diffs = 0
-        for ref_file, new_file in files_to_compare.items():
-            if not self.compare_equal(ref_file, new_file, throw=False):
-                num_diffs += 1
-
-        assert num_diffs == 0, f"{num_diffs} differences found"
-
-    def run_rebase_compare(self,
-                           files_to_compare,
-                           force_rebase: bool = False,
-                           rebase_prompt_default: bool = False):
-
-        failed_rebase_msg = ''
-        incomplete_rebase = False
-
-        for ref_file, new_file in files_to_compare.items():
-
-            if not os.path.exists(new_file) and os.path.exists(ref_file):
-                print()
-                print(f'{new_file} does not exist')
-                if force_rebase or misc_utils.prompt_user("Remove it from reference output?",
-                                                          default=rebase_prompt_default):
-                    if os.path.isdir(ref_file):
-                        shutil.rmtree(ref_file)
-                    else:
-                        os.remove(ref_file)
-                    print(f'removed {new_file} from reference output')
-                continue
-
-            ref_file_is_present = os.path.exists(ref_file)
-            if not ref_file_is_present:
-                os.makedirs(os.path.dirname(ref_file), exist_ok=True)
-            elif self.compare_equal(ref_file, new_file, throw=False):
-                continue
-
-            print()
-            if ref_file_is_present:
-                print(f"rebasing test baseline:\n {new_file} ->\n {ref_file}")
-            else:
-                print(f"creating test baseline:\n  {new_file} ->\n  {ref_file}")
-            try:
-                if force_rebase or misc_utils.prompt_user("Are you sure?",
-                                                          default=rebase_prompt_default):
-                    try:
-                        # we want to copy symlinks as symlinks, not copy what they refer to
-                        if os.path.isdir(new_file):
-                            shutil.copytree(new_file, ref_file, symlinks=True)
-                            #shutil.rmtree(new_file)
-                        else:
-                            shutil.copy(new_file, ref_file, follow_symlinks=False)
-                            #os.remove(new_file)
-                    except PermissionError as err:
-                        failed_rebase_msg += f'\ncp {new_file} {ref_file}'
-                        print('rebase failed', str(err))
-                    else:
-                        print('rebase successful')
-                else:
-                    incomplete_rebase = True
-            except KeyboardInterrupt:
-                incomplete_rebase = True
-                break
-
-        if incomplete_rebase:
-            raise unittest.SkipTest('incomplete rebase')
-
-        if failed_rebase_msg:
-            self.raise_exception(f'failed rebasing tests: {failed_rebase_msg}')
-
-    def get_file_comparator(self, filepath):
-        filename = os.path.basename(filepath)
-        if filename in self.comparators:
-            return self.comparators[filename]
-
-        for pattern, comparator in self.comparators.items():
-            if pathlib.PurePath(filename).match(pattern):
-                return comparator
-
-        if os.path.isdir(filepath):
-            return diff_dirs
-        # default file comparator
-        return FileComparator(max_diff_in_log=self._num_lines_diff)
-
-    def compare_equal(self, ref_file, new_file, throw=True):
-
-        compare_functors = self.get_file_comparator(ref_file)
-
-        if compare_functors is None:
-            # do not compare that file
-            print(f"ignoring file: {ref_file}")
-            return True
-
-        max_len = max(len(ref_file), len(new_file)) + 10
-        fmtd_file1 = ref_file.rjust(max_len)
-        fmtd_file2 = new_file.rjust(max_len)
-        files_info = f'\n{fmtd_file1}\n{fmtd_file2}'
-
-        if not isinstance(compare_functors, (tuple, list)):
-            compare_functors = [compare_functors]
-
-        if self.verbose:
-            print()
-
-        all_equal = True
-        for compare_functor in compare_functors:
-            comparison_description = compare_functor.description()
-            if comparison_description:
-                comparison_description = f' ({comparison_description})'
-            try:
-                compare_equal = compare_functor(ref_file, new_file)
-            except Exception as exc:
-                all_equal = False
-                print(f'failed comparing files: {files_info}')
-                print('error:', exc)
-                continue
-
-            if compare_equal:
-                if self.verbose:
-                    print(f'files match{comparison_description}: {ref_file}')
-            else:
-                all_equal = False
-                error_msg = f'files differ{comparison_description}: {files_info}'
-                if self.verbose:
-                    print(error_msg)
-                if throw:
-                    self.raise_exception(error_msg)
-
-        return all_equal
-
-    def make_dir_path(self, dir_stem, test_name, nested_dir):
-        if self.test_name_as_dir:
-            if nested_dir:
-                return os.path.join(test_name, dir_stem)
-            else:
-                return os.path.join(dir_stem, test_name)
-        else:
-            return dir_stem
-
-    def get_files_to_compare(self, test_name, compare_spec=None) -> dict:
-        """
-        :param test_name: name of the test, used to deduce the ref dir path.
-        :param compare_spec: specifies output files to compare; either:
-                - a path to a file
-                - a path to a directory (in which case all its contents are compared)
-                - a list of those.
-            if left to its None default, compares everything in ref_dir
-        :return: a list of pairs of filepaths to compare: [(ref_file_path, new_file_path), ...]
-        """
-
-        ref_dir = self.get_ref_dir(test_name)
-        out_dir = self.get_out_dir(test_name)
-
-        if compare_spec is None:
-            compare_spec = ref_dir
-            if not os.path.exists(ref_dir):
-                return {ref_dir: out_dir}
-
-        elif not compare_spec:
-            return {}
-
-        if isinstance(compare_spec, str):
-            # single reference file
-            compare_spec = [compare_spec]
-
-        files_to_compare = {}
-
-        for ref_path in compare_spec:
-
-            if isinstance(ref_path, tuple):
-                file1, file2 = ref_path
-                files_to_compare[os.path.join(ref_dir, file1)] = os.path.join(out_dir, file2)
-                continue
-            elif isinstance(compare_spec, dict):
-                new_path = compare_spec[ref_path]
-            else:
-                new_path = out_dir
-
-            if os.path.isdir(ref_path):
-                # add all files under ref directory
-                ref_path = os.path.normpath(ref_path)
-                new_path = os.path.normpath(new_path)
-
-                for dirpath, dirnames, filenames in os.walk(ref_path, followlinks=True):
-                    tmp_path = dirpath.replace(ref_path, new_path, 1)
-                    for filename in filenames:
-                        ref_filepath = os.path.join(dirpath, filename)
-                        new_filepath = os.path.join(tmp_path, filename)
-                        files_to_compare[ref_filepath] = new_filepath
-
-                if not self.ref_diff_only:
-                    for dirpath, dirnames, filenames in os.walk(new_path):
-                        tmp_path = dirpath.replace(new_path, ref_path, 1)
-                        for filename in filenames:
-                            files_to_compare[os.path.join(tmp_path, filename)] = os.path.join(dirpath, filename)
-
-            else:
-                if not os.path.exists(ref_path):
-                    ref_path = os.path.join(ref_dir, ref_path)
-
-                # self.raise_exception(ref_path.replace(ref_dir, new_path))
-                files_to_compare[ref_path] = ref_path.replace(ref_dir, new_path)
-
-        excluded_files = []
-        if self._file_filter:
-            for file in files_to_compare:
-                if not misc_utils.pattern_matches(pattern=self._file_filter, path_string=file):
-                    excluded_files.append(file)
-
-        patterns_to_ignore = []
-        for key, value in self.comparators.items():
-            if value is None:
-                patterns_to_ignore.append(key)
-
-        for file in files_to_compare:
-            file_path = pathlib.PurePath(file)
-            for pattern in patterns_to_ignore:
-                if file_path.match(pattern):
-                    if self.verbose:
-                        print(f'ignoring {file} based on {pattern} pattern')
-                    excluded_files.append(file)
-
-        for file in excluded_files:
-            files_to_compare.pop(file)
-
-        return files_to_compare
-
-    def clear_dir(self, dir_path, recreate=False):
-        with working_dir(self.test_root):
-            output_dir = dir_path
-            if recreate:
-                if os.path.exists(output_dir):
-                    shutil.rmtree(output_dir)
-            else:
-                # the only temporary files left behind should be
-                # files exhibiting differences to reference directory.
-                # Keep those around for investigation.
-                for dirpath, dirnames, filenames in os.walk(output_dir):
-                    if not filenames and not dirnames:
-                        shutil.rmtree(dirpath)
-
-            if recreate:
-                os.makedirs(output_dir, exist_ok=True)
+import os
+import os.path
+import pathlib
+import traceback
+from . import misc_utils
+from .misc_utils import working_dir, rmdir
+from .diff_utils import FileComparator, diff_dirs
+from functools import wraps
+import shutil
+import sys
+import unittest
+from .env_vars import ExeTestEnvVars
+import pytest
+
+
+FORCE_REBASE = 'FORCE'
+REBASE_YES_DEFAULT = 'y'
+
+
+def skip_test(reason=''):
+    """
+    A decorator for marking tests as skipped and still allowing to force-run them.
+    Bypassing behavior is triggered by the presence of an environment variable.
+    :param reason: why the test is being skipped
+    """
+    if ExeTestEnvVars.DISABLE_SKIP in os.environ:
+        return lambda x: x
+    else:
+        return pytest.mark.skip(reason=reason)
+
+
+def skip_module(reason=''):
+    if ExeTestEnvVars.DISABLE_SKIP not in os.environ:
+        pytest.skip(reason, allow_module_level=True)
+
+
+class ExeTestCaseDecorator:
+    """
+    A test case decorator for testing an executable outputs
+    by comparing new output to reference output
+    """
+
+    def __init__(self,
+                 exe: str,
+                 test_root: str = '.',  # =os.path.dirname(__file__),
+                 ref_dir: str = 'ref_dir',
+                 out_dir: str = 'out_dir',
+                 exe_args=None,
+                 compare_spec=None,
+                 run_from_out_dir: bool = True,
+                 test_name_as_dir: bool = True,
+                 nested_ref_dir: bool = True,
+                 nested_out_dir: bool = False, 
+                 comparators=None,
+                 ref_diff_only: bool = False,
+                 exception_handler=None,
+                 env_vars=None,
+                 pre_cmd=None,
+                 exe_path_ref=None,
+                 log_output_path=None):
+        """
+
+        :param exe: path to the executable to test
+        :param test_root: working directory for test execution from which ref_dir/out_dir paths are defined if relative.
+        :param ref_dir: absolute path or relative to test_root directory where test case is defined
+        :param out_dir: directory to write test output to
+        :param exe_args: test executable arguments in string format - as would be passed to command line
+        :param run_from_out_dir: whether the executable working directory should be the output directory
+        :param test_name_as_dir: whether the test name should be used to infer the ref and output directories
+        :param nested_ref_dir: whether ref_dir should be nested in the test_name directory (otherwise, test_name is nested under ref_dir)
+        :param nested_out_dir: whether out_dir should be nested in the test_name directory (otherwise, test_name is nested under out_dir)
+        :param comparators:
+        :param ref_diff_only: files in out_dir but not in ref_dir will not be flagged
+        :param exception_handler: what to do in case of exception
+        :param env_vars: environment variables to populate for the test run
+        :param pre_cmd: a command to run before the executable is run
+        :param exe_path_ref:
+        :param log_output_path:
+        """
+
+        self.exe_path_ref = exe_path_ref if exe_path_ref else {}
+
+        def get_test_exe(val):
+            if val in self.exe_path_ref:
+                return self.exe_path_ref[val]
+            elif val:
+                if os.path.isdir(val):
+                    return os.path.join(val, os.path.basename(exe))
+                else:
+                    return val
+            else:
+                return exe
+
+        use_test_exe = os.environ.get(ExeTestEnvVars.USE_EXE)
+
+        # if USE_TEST_EXE has special target value, run against reference executable
+        if use_test_exe is not None:
+            self.exe_path = get_test_exe(use_test_exe)
+        else:
+            self.exe_path = exe
+
+        self.test_root = test_root
+        self.REF_OUTPUT_DIR = ref_dir
+        self.TMP_OUTPUT_DIR = out_dir
+        self.test_name_as_dir = test_name_as_dir
+        self.run_from_out_dir = run_from_out_dir
+        self.ref_diff_only = ref_diff_only
+
+        self.test_name = ''
+        self.comparators = comparators or {}
+        self.exception_handler = exception_handler
+        self.common_env_vars = env_vars or dict()
+        self.pre_cmd = pre_cmd if pre_cmd else []
+        self.exe_args = exe_args
+        self.log_output_path = log_output_path
+
+        self.verbose = ExeTestEnvVars.VERBOSE in os.environ
+        if ExeTestEnvVars.NO_RUN in os.environ:
+            self.norun = os.environ[ExeTestEnvVars.NO_RUN]
+            if not self.norun:
+                self.norun = 'default'
+        else:
+            self.norun = None
+
+        self._compare_spec = compare_spec
+        self._nested_ref_dir = nested_ref_dir
+        self._nested_out_dir = nested_out_dir
+        self._num_lines_diff = int(os.environ.get(ExeTestEnvVars.NUM_DIFFS, 20))
+        self._file_filter = os.environ.get(ExeTestEnvVars.FILE_FILTER, '').split('+')
+
+    @staticmethod
+    def get_test_subdir(test_name):
+        return test_name
+
+    def get_out_dir(self, test_name):
+        return self.make_dir_path(self.TMP_OUTPUT_DIR, test_name, self._nested_out_dir)
+
+    def get_ref_dir(self, test_name):
+        return self.make_dir_path(self.REF_OUTPUT_DIR, test_name, self._nested_ref_dir)
+
+    def __call__(self,
+                 exe_args=None,
+                 extra_args=None,
+                 compare_spec=None,
+                 pre_cmd=None,
+                 env_vars=None,
+                 post_cmd=None,
+                 owners=None):
+        """
+
+        :param exe_args: overrides arguments specified in the constructor
+        :param extra_args: appends arguments to the ones specified in the constructor
+        :param compare_spec:
+        :param pre_cmd:
+        :param env_vars:
+        :param post_cmd:
+        :param owners:
+        :return:
+        """
+        all_env_vars = dict(self.common_env_vars)
+        if env_vars:
+            all_env_vars.update(env_vars)
+
+        pre_cmds = self.pre_cmd
+        if pre_cmd:
+            if isinstance(pre_cmd, str):
+                pre_cmds = pre_cmds + [pre_cmd]
+            else:
+                pre_cmds = pre_cmds + pre_cmd
+
+        if exe_args is None:
+            if self.exe_args is not None:
+                exe_args = self.exe_args
+            else:
+                exe_args = ''
+
+        if extra_args is not None:
+            exe_args += ' ' + extra_args
+
+        if compare_spec is None:
+            compare_spec = self._compare_spec
+
+        self._compare_only = ExeTestEnvVars.COMPARE_ONLY in os.environ
+
+        def func_wrapper(test_func):
+            """
+            :param test_func:
+            :return: decorated function
+            """
+            test_name = test_func.__name__.split("_", 1)[-1]
+            import inspect
+            parent_module_name = inspect.getmodule(test_func).__name__
+
+            resolved_env_vars = {}
+            for name, value in all_env_vars.items():
+                resolved_env_vars[name] = str(value).format(test_name=test_name)
+
+            @wraps(test_func)
+            def f(*args, **kwargs):
+                ret = test_func(*args, **kwargs)
+                try:
+                    self.run_test(exe_args,
+                                  compare_spec,
+                                  pre_cmd=pre_cmds,
+                                  env_vars=resolved_env_vars,
+                                  post_cmd=post_cmd,
+                                  test_name=test_name,
+                                  parent_module_name=parent_module_name,
+                                  verbose=self.verbose)
+                except unittest.SkipTest:
+                    raise
+
+                return ret
+
+            def doc_gist(func):
+                """
+                :param func:
+                :return:
+                """
+
+                if func.__doc__:
+                    for line in func.__doc__.splitlines():
+                        if line.strip():
+                            return line.strip()
+                    return ""
+
+            # set description attribute for test framework to display
+            doc = doc_gist(test_func)
+            if doc:
+                f.description = (test_name + ": ").ljust(10) + doc
+            else:
+                f.description = test_name.ljust(10)
+
+            return f
+
+        return func_wrapper
+
+    @classmethod
+    def do_test_rebase(cls):
+        """
+        :return: whether to run test in rebase mode, whether to not prompt for applying changes
+        """
+        val = os.getenv(ExeTestEnvVars.REBASE)
+        if val is None:
+            return False, False, False
+
+        do_rebase = val != '0'
+        return do_rebase, do_rebase and val != FORCE_REBASE, val == REBASE_YES_DEFAULT
+
+    def raise_exception(self, msg):
+        raise Exception(msg)
+
+    def run_test(self, exe_args, compare_spec,
+                 pre_cmd, env_vars, post_cmd,
+                 test_name, parent_module_name,
+                 verbose):
+
+        do_rebase, rebase_with_prompt, rebase_yes_default = self.do_test_rebase()
+        if rebase_with_prompt:
+            if not sys.stdout.isatty():
+                self.raise_exception("cannot rebase unless confirmation "
+                                     "prompt is displayed in terminal. "
+                                     "Make sure you are using --capture=no pytest option")
+
+        with working_dir(self.test_root):
+
+            files_to_compare = self.get_files_to_compare(test_name, compare_spec)
+
+            if compare_spec and not files_to_compare.items():
+                self.raise_exception(f"No reference output files for {compare_spec}")
+
+            tmp_output_dir = self.get_out_dir(test_name)
+            run_from_dir = os.path.join(self.test_root, tmp_output_dir) \
+                if self.run_from_out_dir else self.test_root
+
+        if not self._compare_only:
+            self.clear_dir(tmp_output_dir, recreate=True)
+
+        with working_dir(run_from_dir):
+            try:
+                misc_utils.exec_cmdline(self.exe_path,
+                                        exe_args,
+                                        pre_cmd=pre_cmd,
+                                        env_vars=env_vars,
+                                        post_cmd=post_cmd,
+                                        log_save_path=self.log_output_path,
+                                        norun=self.norun or self._compare_only,
+                                        verbose=verbose)
+            except Exception as exc:
+                if self.exception_handler:
+                    self.exception_handler(exc)
+                else:
+                    raise
+
+        if self.norun:
+            if self.norun == 'ctest':
+                print()
+                print('|'.join(
+                    str(item) for item in ((parent_module_name.replace('.', '/') + '.py::test_' + test_name),
+                                           run_from_dir,
+                                           ' '.join(f'{key}={val}' for key, val in env_vars.items()),
+                                           os.path.basename(self.exe_path),
+                                           exe_args)))
+            if not self._compare_only:
+                # this will mark the test as skipped
+                pytest.skip("no-run mode")
+
+        with working_dir(self.test_root):
+
+            if do_rebase:
+                self.run_rebase_compare(files_to_compare,
+                                        force_rebase=not rebase_with_prompt,
+                                        rebase_prompt_default=rebase_yes_default)
+            else:
+                self.run_compare(files_to_compare)
+
+    def run_compare(self, files_to_compare):
+
+        for _ref_file, new_file in files_to_compare.items():
+            if not os.path.exists(new_file):
+                self.raise_exception(f"Missing output file: {new_file}")
+
+        for ref_file, new_file in files_to_compare.items():
+            has_ref = os.path.exists(ref_file)
+            has_new = os.path.exists(new_file)
+            if not has_ref and not has_new:
+                self.raise_exception(f"Missing both ref and new files:\n{ref_file}\n{new_file}")
+            else:
+                if not has_ref:
+                    self.raise_exception(f"Missing reference file: {ref_file} - "
+                                         f"you can rebase with --rebase option")
+                if not has_new:
+                    while not os.path.exists(os.path.dirname(new_file)):
+                        new_file = os.path.dirname(new_file)
+                    self.raise_exception(f"Missing output file: {new_file}")
+
+        num_diffs = 0
+        for ref_file, new_file in files_to_compare.items():
+            if not self.compare_equal(ref_file, new_file, throw=False):
+                num_diffs += 1
+
+        assert num_diffs == 0, f"{num_diffs} differences found"
+
+    def run_rebase_compare(self,
+                           files_to_compare,
+                           force_rebase: bool = False,
+                           rebase_prompt_default: bool = False):
+
+        failed_rebase_msg = ''
+        incomplete_rebase = False
+
+        for ref_file, new_file in files_to_compare.items():
+
+            if not os.path.exists(new_file) and os.path.exists(ref_file):
+                print()
+                print(f'{new_file} does not exist')
+                if force_rebase or misc_utils.prompt_user("Remove it from reference output?",
+                                                          default=rebase_prompt_default):
+                    if os.path.isdir(ref_file):
+                        shutil.rmtree(ref_file)
+                    else:
+                        os.remove(ref_file)
+                    print(f'removed {new_file} from reference output')
+                continue
+
+            ref_file_is_present = os.path.exists(ref_file)
+            if not ref_file_is_present:
+                os.makedirs(os.path.dirname(ref_file), exist_ok=True)
+            elif self.compare_equal(ref_file, new_file, throw=False):
+                continue
+
+            print()
+            if ref_file_is_present:
+                print(f"rebasing test baseline:\n {new_file} ->\n {ref_file}")
+            else:
+                print(f"creating test baseline:\n  {new_file} ->\n  {ref_file}")
+            try:
+                if force_rebase or misc_utils.prompt_user("Are you sure?",
+                                                          default=rebase_prompt_default):
+                    try:
+                        # we want to copy symlinks as symlinks, not copy what they refer to
+                        if os.path.isdir(new_file):
+                            shutil.copytree(new_file, ref_file, symlinks=True)
+                            #shutil.rmtree(new_file)
+                        else:
+                            shutil.copy(new_file, ref_file, follow_symlinks=False)
+                            #os.remove(new_file)
+                    except PermissionError as err:
+                        failed_rebase_msg += f'\ncp {new_file} {ref_file}'
+                        print('rebase failed', str(err))
+                    else:
+                        print('rebase successful')
+                else:
+                    incomplete_rebase = True
+            except KeyboardInterrupt:
+                incomplete_rebase = True
+                break
+
+        if incomplete_rebase:
+            raise unittest.SkipTest('incomplete rebase')
+
+        if failed_rebase_msg:
+            self.raise_exception(f'failed rebasing tests: {failed_rebase_msg}')
+
+    def get_file_comparator(self, filepath):
+        filename = os.path.basename(filepath)
+        if filename in self.comparators:
+            return self.comparators[filename]
+
+        for pattern, comparator in self.comparators.items():
+            if pathlib.PurePath(filename).match(pattern):
+                return comparator
+
+        if os.path.isdir(filepath):
+            return diff_dirs
+        # default file comparator
+        return FileComparator(max_diff_in_log=self._num_lines_diff)
+
+    def compare_equal(self, ref_file, new_file, throw=True):
+
+        compare_functors = self.get_file_comparator(ref_file)
+
+        if compare_functors is None:
+            # do not compare that file
+            print(f"ignoring file: {ref_file}")
+            return True
+
+        max_len = max(len(ref_file), len(new_file)) + 10
+        fmtd_file1 = ref_file.rjust(max_len)
+        fmtd_file2 = new_file.rjust(max_len)
+        files_info = f'\n{fmtd_file1}\n{fmtd_file2}'
+
+        if not isinstance(compare_functors, (tuple, list)):
+            compare_functors = [compare_functors]
+
+        if self.verbose:
+            print()
+
+        all_equal = True
+        for compare_functor in compare_functors:
+            comparison_description = compare_functor.description()
+            if comparison_description:
+                comparison_description = f' ({comparison_description})'
+            try:
+                compare_equal = compare_functor(ref_file, new_file)
+            except Exception as exc:
+                all_equal = False
+                print(f'failed comparing files: {files_info}')
+                print('error:', exc)
+                continue
+
+            if compare_equal:
+                if self.verbose:
+                    print(f'files match{comparison_description}: {ref_file}')
+            else:
+                all_equal = False
+                error_msg = f'files differ{comparison_description}: {files_info}'
+                if self.verbose:
+                    print(error_msg)
+                if throw:
+                    self.raise_exception(error_msg)
+
+        return all_equal
+
+    def make_dir_path(self, dir_stem, test_name, nested_dir):
+        if self.test_name_as_dir:
+            if nested_dir:
+                return os.path.join(test_name, dir_stem)
+            else:
+                return os.path.join(dir_stem, test_name)
+        else:
+            return dir_stem
+
+    def get_files_to_compare(self, test_name, compare_spec=None) -> dict:
+        """
+        :param test_name: name of the test, used to deduce the ref dir path.
+        :param compare_spec: specifies output files to compare; either:
+                - a path to a file
+                - a path to a directory (in which case all its contents are compared)
+                - a list of those.
+            if left to its None default, compares everything in ref_dir
+        :return: a list of pairs of filepaths to compare: [(ref_file_path, new_file_path), ...]
+        """
+
+        ref_dir = self.get_ref_dir(test_name)
+        out_dir = self.get_out_dir(test_name)
+
+        if compare_spec is None:
+            compare_spec = ref_dir
+            if not os.path.exists(ref_dir):
+                return {ref_dir: out_dir}
+
+        elif not compare_spec:
+            return {}
+
+        if isinstance(compare_spec, str):
+            # single reference file
+            compare_spec = [compare_spec]
+
+        files_to_compare = {}
+
+        for ref_path in compare_spec:
+
+            if isinstance(ref_path, tuple):
+                file1, file2 = ref_path
+                files_to_compare[os.path.join(ref_dir, file1)] = os.path.join(out_dir, file2)
+                continue
+            elif isinstance(compare_spec, dict):
+                new_path = compare_spec[ref_path]
+            else:
+                new_path = out_dir
+
+            if os.path.isdir(ref_path):
+                # add all files under ref directory
+                ref_path = os.path.normpath(ref_path)
+                new_path = os.path.normpath(new_path)
+
+                for dirpath, dirnames, filenames in os.walk(ref_path, followlinks=True):
+                    tmp_path = dirpath.replace(ref_path, new_path, 1)
+                    for filename in filenames:
+                        ref_filepath = os.path.join(dirpath, filename)
+                        new_filepath = os.path.join(tmp_path, filename)
+                        files_to_compare[ref_filepath] = new_filepath
+
+                if not self.ref_diff_only:
+                    for dirpath, dirnames, filenames in os.walk(new_path):
+                        tmp_path = dirpath.replace(new_path, ref_path, 1)
+                        for filename in filenames:
+                            files_to_compare[os.path.join(tmp_path, filename)] = os.path.join(dirpath, filename)
+
+            else:
+                if not os.path.exists(ref_path):
+                    ref_path = os.path.join(ref_dir, ref_path)
+
+                # self.raise_exception(ref_path.replace(ref_dir, new_path))
+                files_to_compare[ref_path] = ref_path.replace(ref_dir, new_path)
+
+        excluded_files = []
+        if self._file_filter:
+            for file in files_to_compare:
+                if not misc_utils.pattern_matches(pattern=self._file_filter, path_string=file):
+                    excluded_files.append(file)
+
+        patterns_to_ignore = []
+        for key, value in self.comparators.items():
+            if value is None:
+                patterns_to_ignore.append(key)
+
+        for file in files_to_compare:
+            file_path = pathlib.PurePath(file)
+            for pattern in patterns_to_ignore:
+                if file_path.match(pattern):
+                    if self.verbose:
+                        print(f'ignoring {file} based on {pattern} pattern')
+                    excluded_files.append(file)
+
+        for file in excluded_files:
+            files_to_compare.pop(file)
+
+        return files_to_compare
+
+    def clear_dir(self, dir_path, recreate=False):
+        with working_dir(self.test_root):
+            output_dir = dir_path
+            if recreate:
+                if os.path.exists(output_dir):
+                    shutil.rmtree(output_dir)
+            else:
+                # the only temporary files left behind should be
+                # files exhibiting differences to reference directory.
+                # Keep those around for investigation.
+                for dirpath, dirnames, filenames in os.walk(output_dir):
+                    if not filenames and not dirnames:
+                        shutil.rmtree(dirpath)
+
+            if recreate:
+                os.makedirs(output_dir, exist_ok=True)
```

### Comparing `exetest-0.9.1/exetest/expects_exception.py` & `exetest-0.9.2/exetest/expects_exception.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-from functools import wraps
-
-
-def expects_exception(exception_type=Exception,
-                      expected_message=None,
-                      expected_message_validator=None):
-    """
-    A decorator to test that a function throws an exception.
-
-    sample usage:
-        @except_exception()
-        def test_my_func():
-            ...
-            # some code here that should raise Exception
-            ...
-
-    the test will pass if calling test_my_func raises an Exception, otherwise it will raise.
-    In addition, the exception message content can be asserted.
-
-    :param exception_type: exception type that a call to the method should raise.
-    :param expected_message: excepted Exception message
-    :param expected_message_validator: a predicate that takes the exception message and returns True if it is valid.
-    :return: decorated function
-    """
-    def decorator(test_func):
-
-        @wraps(test_func)
-        def wrapped_func(*args, **kwargs):
-            try:
-                ret = test_func(*args, **kwargs)
-            except exception_type as exc:
-                message = exc.args[0]
-                if expected_message is not None:
-                    assert(expected_message == message), \
-                        "exception message is not as expected"
-
-                if expected_message_validator is not None:
-                    assert(expected_message_validator(message)), \
-                        "exception message is not as expected"
-
-                return
-
-            raise Exception('Expected exception was not thrown. '
-                            f'returned value: "{ret}"')
-        return wrapped_func
-
-    return decorator
+from functools import wraps
+
+
+def expects_exception(exception_type=Exception,
+                      expected_message=None,
+                      expected_message_validator=None):
+    """
+    A decorator to test that a function throws an exception.
+
+    sample usage:
+        @except_exception()
+        def test_my_func():
+            ...
+            # some code here that should raise Exception
+            ...
+
+    the test will pass if calling test_my_func raises an Exception, otherwise it will raise.
+    In addition, the exception message content can be asserted.
+
+    :param exception_type: exception type that a call to the method should raise.
+    :param expected_message: excepted Exception message
+    :param expected_message_validator: a predicate that takes the exception message and returns True if it is valid.
+    :return: decorated function
+    """
+    def decorator(test_func):
+
+        @wraps(test_func)
+        def wrapped_func(*args, **kwargs):
+            try:
+                ret = test_func(*args, **kwargs)
+            except exception_type as exc:
+                message = exc.args[0]
+                if expected_message is not None:
+                    assert(expected_message == message), \
+                        "exception message is not as expected"
+
+                if expected_message_validator is not None:
+                    assert(expected_message_validator(message)), \
+                        "exception message is not as expected"
+
+                return
+
+            raise Exception('Expected exception was not thrown. '
+                            f'returned value: "{ret}"')
+        return wrapped_func
+
+    return decorator
```

### Comparing `exetest-0.9.1/exetest/misc_utils.py` & `exetest-0.9.2/exetest/misc_utils.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,262 +1,262 @@
-import os
-import sys
-import shutil
-import time
-from contextlib import contextmanager
-import subprocess
-import typing
-import pathlib
-
-
-def print_test_meta(*message):
-    print(*message, file=sys.stderr)
-
-
-def rmdir(dir_path):
-    if os.path.exists(os.path.join(os.getcwd(), dir_path)):
-        shutil.rmtree(dir_path)
-
-
-@contextmanager
-def working_dir(path):
-    """temporary switch of working directory"""
-
-    current_dir = os.getcwd()
-    if path is not None:
-        os.chdir(path)
-
-    try:
-        yield
-    finally:
-        if path is not None:
-            os.chdir(current_dir)
-
-
-def prompt_user(message_prompt: str,
-                yes_entries=('y',),
-                no_entries=('n',),
-                default: bool = None) -> bool:
-    if default is not None:
-        if default:
-            reply_usage = f'[{yes_entries[0]}]/{no_entries[0]}'
-        else:
-            reply_usage = f'{yes_entries[0]}/[{no_entries[0]}]'
-    else:
-        reply_usage = f'{yes_entries[0]}/{no_entries[0]}'
-
-    message_prompt += ' ' + reply_usage + '\n'
-
-    while True:
-        user_input = input(message_prompt)
-        if user_input == '' and default is not None:
-            return default
-        if user_input in yes_entries:
-            return True
-        if user_input in no_entries:
-            return False
-
-        print(f'Invalid choice: {user_input}')
-
-
-@contextmanager
-def revert_file_modif(file_path):
-    """ Saves file content and  write original content back on exit.
-        Creates file if it does not exist and deletes it on exist.
-    """
-
-    file_exists = os.path.exists(file_path)
-    with open(file_path) as f:
-        original_content = f.read()
-
-    try:
-        yield original_content
-    finally:
-        if not file_exists:
-            os.remove(file_path)
-        else:
-            with open(file_path, 'w') as f:
-                f.write(original_content)
-
-
-@contextmanager
-def perf_timer(message='Time elapsed:', verbose=True):
-    """timer context (includes time spent during process sleep)"""
-    start_time = time.perf_counter()
-    try:
-        yield
-    finally:
-        if verbose:
-            time_elapsed = time.perf_counter() - start_time
-            print(message, '%.3fsec' % time_elapsed)
-
-
-def diff_directory(path1, path2):
-    """
-    Iterate on dir tree below path2 and report if  a path under path2 does not exist under path2
-    If some file or dir should be ignored, add them to ignored_dir_or_file.
-    :param path1:
-    :param path2:
-    :return:
-    """
-    ignored_dir_or_file = ['.svn', '.git', '.gitignore', 'README.md']
-
-    for path in os.listdir(path2):
-        if path not in ignored_dir_or_file:
-            abs1 = os.path.join(path1, path)
-            abs2 = os.path.join(path2, path)
-
-            if not os.path.exists(abs1):
-                yield abs2
-
-            if os.path.isdir(abs2):
-                for diff_path in diff_directory(abs1, abs2):
-                    yield diff_path
-
-
-class ExeFailedException(Exception):
-    pass
-
-
-def format_log_for_exception(exc, max_num_lines=20):
-    """
-    extract information from streams captured by a subprocess error
-    :param exc: an instance of subprocess.CalledProcessError
-    :param max_num_lines: max number of log lines to append to reraised exception
-    :return: formatted exception message with extra info from the captured executable log
-    """
-
-    exec_log = exc.stderr
-    if not exec_log:
-        exec_log = exc.stdout
-
-    if exec_log:
-        message = exec_log.decode('latin-1', errors='ignore')
-        last_few_lines = os.linesep.join(message.rsplit(os.linesep, max_num_lines)[-(max_num_lines-1):])
-        msg_len = len(message)
-
-        if msg_len > len(last_few_lines):
-            return last_few_lines + f'\n[truncated to last {max_num_lines} lines\n'
-        else:
-            return last_few_lines
-
-
-def handle_subprocess_error(exc):
-    message = format_log_for_exception(exc)
-    if message:
-        raise ExeFailedException(message) from exc
-
-
-def exec_cmdline(command, args_list, check_ret_code=True,
-                 log_save_path=None, env_vars=None,
-                 pre_cmd=None, post_cmd=None, verbose=True, norun=False):
-    """
-    Runs command and returns the captured stdout log
-    :param command:
-    :param args_list:
-    :param check_ret_code:
-    :param log_save_path:
-    :param env_vars:
-    :param pre_cmd:
-    :param post_cmd:
-    :param verbose:
-    :param norun:
-    :return:
-    """
-
-    env_vars_line = ''
-    if env_vars:
-        env_vars_line = ' '.join([k + '=' + str(v) for k, v in env_vars.items()])
-        env_vars_line += ' '
-
-    if isinstance(args_list, str):
-        args_list = [args_list]
-
-    # get rid of new lines in command line args
-    args_list = [' '.join(line.strip() for line in args.splitlines()) for args in args_list]
-
-    cmd_line_tasks = [command + ' ' + args for args in args_list]
-
-    # chain commands
-    cmd_line = ''
-    for task in cmd_line_tasks[:-1]:
-        cmd_line += '{ ' + env_vars_line + task + ' & } ; '
-
-    cmd_line += env_vars_line + cmd_line_tasks[-1]
-
-    # add pre/post commands
-    if pre_cmd:
-        cmd_line = ' && '.join(pre_cmd) + ' && ' + cmd_line
-
-    if post_cmd:
-        cmd_line += ' && ' + ' && '.join(post_cmd)
-
-    if verbose:
-        print()
-        print('working dir/command line:')
-        print(os.getcwd())
-        print(cmd_line)
-        print()
-
-    if not norun:
-        if not os.path.exists(command):
-            raise Exception(f'{command} '
-                            f'not found from {os.getcwd()}. '
-                            f'Is it in your path? Did you compile?')
-
-        exe_name = os.path.basename(command.split()[0])
-        try:
-            with perf_timer(exe_name + ' execution took '):
-                result_info = subprocess.run(cmd_line, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
-
-            log_out = result_info.stdout
-            if log_save_path is not None:
-                # log_out = log_out.decode('latin-1')
-                with open(log_save_path, 'wb') as f:
-                    f.write(log_out)
-
-            if check_ret_code:
-                result_info.check_returncode()
-
-            return log_out
-
-        except subprocess.CalledProcessError as exc:
-            handle_subprocess_error(exc)
-            raise
-
-    return cmd_line
-
-
-def pattern_matches(pattern: typing.Union[str, typing.List[str]],
-                    path_string: str) -> bool:
-
-    if isinstance(pattern, str):
-        patterns = [pattern]
-    else:
-        patterns = pattern
-
-    has_suppress = False
-    has_keep = False
-    keep = None
-
-    def match(pattern, string):
-        if '*' in pattern:
-            return pathlib.PurePath(string).match(pattern)
-        else:
-            return pattern in string
-
-    for pattern in patterns:
-        if pattern.startswith('~'):
-            has_suppress = True
-            if match(pattern=pattern[1:], string=path_string):
-                keep = False
-
-        else:
-            has_keep = True
-            if match(pattern=pattern, string=path_string):
-                keep = True
-
-    if keep is None:
-        # default
-        keep = has_suppress and not has_keep
-
-    return keep
+import os
+import sys
+import shutil
+import time
+from contextlib import contextmanager
+import subprocess
+import typing
+import pathlib
+
+
+def print_test_meta(*message):
+    print(*message, file=sys.stderr)
+
+
+def rmdir(dir_path):
+    if os.path.exists(os.path.join(os.getcwd(), dir_path)):
+        shutil.rmtree(dir_path)
+
+
+@contextmanager
+def working_dir(path):
+    """temporary switch of working directory"""
+
+    current_dir = os.getcwd()
+    if path is not None:
+        os.chdir(path)
+
+    try:
+        yield
+    finally:
+        if path is not None:
+            os.chdir(current_dir)
+
+
+def prompt_user(message_prompt: str,
+                yes_entries=('y',),
+                no_entries=('n',),
+                default: bool = None) -> bool:
+    if default is not None:
+        if default:
+            reply_usage = f'[{yes_entries[0]}]/{no_entries[0]}'
+        else:
+            reply_usage = f'{yes_entries[0]}/[{no_entries[0]}]'
+    else:
+        reply_usage = f'{yes_entries[0]}/{no_entries[0]}'
+
+    message_prompt += ' ' + reply_usage + '\n'
+
+    while True:
+        user_input = input(message_prompt)
+        if user_input == '' and default is not None:
+            return default
+        if user_input in yes_entries:
+            return True
+        if user_input in no_entries:
+            return False
+
+        print(f'Invalid choice: {user_input}')
+
+
+@contextmanager
+def revert_file_modif(file_path):
+    """ Saves file content and  write original content back on exit.
+        Creates file if it does not exist and deletes it on exist.
+    """
+
+    file_exists = os.path.exists(file_path)
+    with open(file_path) as f:
+        original_content = f.read()
+
+    try:
+        yield original_content
+    finally:
+        if not file_exists:
+            os.remove(file_path)
+        else:
+            with open(file_path, 'w') as f:
+                f.write(original_content)
+
+
+@contextmanager
+def perf_timer(message='Time elapsed:', verbose=True):
+    """timer context (includes time spent during process sleep)"""
+    start_time = time.perf_counter()
+    try:
+        yield
+    finally:
+        if verbose:
+            time_elapsed = time.perf_counter() - start_time
+            print(message, '%.3fsec' % time_elapsed)
+
+
+def diff_directory(path1, path2):
+    """
+    Iterate on dir tree below path2 and report if  a path under path2 does not exist under path2
+    If some file or dir should be ignored, add them to ignored_dir_or_file.
+    :param path1:
+    :param path2:
+    :return:
+    """
+    ignored_dir_or_file = ['.svn', '.git', '.gitignore', 'README.md']
+
+    for path in os.listdir(path2):
+        if path not in ignored_dir_or_file:
+            abs1 = os.path.join(path1, path)
+            abs2 = os.path.join(path2, path)
+
+            if not os.path.exists(abs1):
+                yield abs2
+
+            if os.path.isdir(abs2):
+                for diff_path in diff_directory(abs1, abs2):
+                    yield diff_path
+
+
+class ExeFailedException(Exception):
+    pass
+
+
+def format_log_for_exception(exc, max_num_lines=20):
+    """
+    extract information from streams captured by a subprocess error
+    :param exc: an instance of subprocess.CalledProcessError
+    :param max_num_lines: max number of log lines to append to reraised exception
+    :return: formatted exception message with extra info from the captured executable log
+    """
+
+    exec_log = exc.stderr
+    if not exec_log:
+        exec_log = exc.stdout
+
+    if exec_log:
+        message = exec_log.decode('latin-1', errors='ignore')
+        last_few_lines = os.linesep.join(message.rsplit(os.linesep, max_num_lines)[-(max_num_lines-1):])
+        msg_len = len(message)
+
+        if msg_len > len(last_few_lines):
+            return last_few_lines + f'\n[truncated to last {max_num_lines} lines\n'
+        else:
+            return last_few_lines
+
+
+def handle_subprocess_error(exc):
+    message = format_log_for_exception(exc)
+    if message:
+        raise ExeFailedException(message) from exc
+
+
+def exec_cmdline(command, args_list, check_ret_code=True,
+                 log_save_path=None, env_vars=None,
+                 pre_cmd=None, post_cmd=None, verbose=True, norun=False):
+    """
+    Runs command and returns the captured stdout log
+    :param command:
+    :param args_list:
+    :param check_ret_code:
+    :param log_save_path:
+    :param env_vars:
+    :param pre_cmd:
+    :param post_cmd:
+    :param verbose:
+    :param norun:
+    :return:
+    """
+
+    env_vars_line = ''
+    if env_vars:
+        env_vars_line = ' '.join([k + '=' + str(v) for k, v in env_vars.items()])
+        env_vars_line += ' '
+
+    if isinstance(args_list, str):
+        args_list = [args_list]
+
+    # get rid of new lines in command line args
+    args_list = [' '.join(line.strip() for line in args.splitlines()) for args in args_list]
+
+    cmd_line_tasks = [command + ' ' + args for args in args_list]
+
+    # chain commands
+    cmd_line = ''
+    for task in cmd_line_tasks[:-1]:
+        cmd_line += '{ ' + env_vars_line + task + ' & } ; '
+
+    cmd_line += env_vars_line + cmd_line_tasks[-1]
+
+    # add pre/post commands
+    if pre_cmd:
+        cmd_line = ' && '.join(pre_cmd) + ' && ' + cmd_line
+
+    if post_cmd:
+        cmd_line += ' && ' + ' && '.join(post_cmd)
+
+    if verbose:
+        print()
+        print('working dir/command line:')
+        print(os.getcwd())
+        print(cmd_line)
+        print()
+
+    if not norun:
+        if not os.path.exists(command):
+            raise Exception(f'{command} '
+                            f'not found from {os.getcwd()}. '
+                            f'Is it in your path? Did you compile?')
+
+        exe_name = os.path.basename(command.split()[0])
+        try:
+            with perf_timer(exe_name + ' execution took '):
+                result_info = subprocess.run(cmd_line, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
+
+            log_out = result_info.stdout
+            if log_save_path is not None:
+                # log_out = log_out.decode('latin-1')
+                with open(log_save_path, 'wb') as f:
+                    f.write(log_out)
+
+            if check_ret_code:
+                result_info.check_returncode()
+
+            return log_out
+
+        except subprocess.CalledProcessError as exc:
+            handle_subprocess_error(exc)
+            raise
+
+    return cmd_line
+
+
+def pattern_matches(pattern: typing.Union[str, typing.List[str]],
+                    path_string: str) -> bool:
+
+    if isinstance(pattern, str):
+        patterns = [pattern]
+    else:
+        patterns = pattern
+
+    has_suppress = False
+    has_keep = False
+    keep = None
+
+    def match(pattern, string):
+        if '*' in pattern:
+            return pathlib.PurePath(string).match(pattern)
+        else:
+            return pattern in string
+
+    for pattern in patterns:
+        if pattern.startswith('~'):
+            has_suppress = True
+            if match(pattern=pattern[1:], string=path_string):
+                keep = False
+
+        else:
+            has_keep = True
+            if match(pattern=pattern, string=path_string):
+                keep = True
+
+    if keep is None:
+        # default
+        keep = has_suppress and not has_keep
+
+    return keep
```

### Comparing `exetest-0.9.1/setup.py` & `exetest-0.9.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from distutils.core import setup
-setup(
-  name='exetest',         # How you named your package folder (MyLib)
-  packages=['exetest'],   # Chose the same as "name"
-  version='0.9.1',      # Start with a small number and increase it with every change you make
-  license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
-  description='A pytest-based test framework for black-box approach to testing executables',   # Give a short description about your library
-  author='Guillaume227',                   # Type in your name
-  author_email='guillaume227@gmail.com',      # Type in your E-Mail
-  url='https://github.com/Guillaume227/exetest',   # Provide either the link to your github or to your website
-  download_url='https://github.com/Guillaume227/exetest/archive/v0.1-alpha.tar.gz',
-  keywords=['test', 'pytest', 'nosetest'],  # Keywords that define your package best
-  install_requires=[            # I get to this in a second
-      ],
-  classifiers=[
-    'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
-    'Intended Audience :: Developers',      # Define that your audience are developers
-    'Topic :: Software Development :: Build Tools',
-    'Operating System :: OS Independent',
-    'License :: OSI Approved :: MIT License',   # Again, pick a license
-    'Programming Language :: Python :: 3',      #Specify the python versions that you want to support
-  ],
-  python_requires='>=3.6'
-)
+from distutils.core import setup
+setup(
+  name='exetest',         # How you named your package folder (MyLib)
+  packages=['exetest'],   # Chose the same as "name"
+  version='0.9.2',      # Start with a small number and increase it with every change you make
+  license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
+  description='A pytest-based test framework for black-box approach to testing executables',   # Give a short description about your library
+  author='Guillaume227',                   # Type in your name
+  author_email='guillaume227@gmail.com',      # Type in your E-Mail
+  url='https://github.com/Guillaume227/exetest',   # Provide either the link to your github or to your website
+  download_url='https://github.com/Guillaume227/exetest/archive/v0.1-alpha.tar.gz',
+  keywords=['test', 'pytest', 'nosetest'],  # Keywords that define your package best
+  install_requires=[            # I get to this in a second
+      ],
+  classifiers=[
+    'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
+    'Intended Audience :: Developers',      # Define that your audience are developers
+    'Topic :: Software Development :: Build Tools',
+    'Operating System :: OS Independent',
+    'License :: OSI Approved :: MIT License',   # Again, pick a license
+    'Programming Language :: Python :: 3',      #Specify the python versions that you want to support
+  ],
+  python_requires='>=3.6'
+)
```

