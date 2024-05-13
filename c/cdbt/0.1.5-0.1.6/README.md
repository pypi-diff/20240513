# Comparing `tmp/cdbt-0.1.5.tar.gz` & `tmp/cdbt-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdbt-0.1.5.tar", last modified: Sun May 12 23:48:01 2024, max compression
+gzip compressed data, was "cdbt-0.1.6.tar", last modified: Mon May 13 01:55:11 2024, max compression
```

## Comparing `cdbt-0.1.5.tar` & `cdbt-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-12 23:48:01.558055 cdbt-0.1.5/
--rw-r--r--   0 craiglathrop   (501) staff       (20)      391 2024-05-12 23:48:01.557484 cdbt-0.1.5/PKG-INFO
--rw-r--r--   0 craiglathrop   (501) staff       (20)     3396 2024-05-12 23:47:32.000000 cdbt-0.1.5/README.md
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-12 23:48:01.541266 cdbt-0.1.5/cdbt/
--rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2024-05-11 20:22:05.000000 cdbt-0.1.5/cdbt/__init__.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     2992 2024-05-12 23:33:23.000000 cdbt-0.1.5/cdbt/cmdline.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)    11636 2024-05-12 23:33:23.000000 cdbt-0.1.5/cdbt/main.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     6642 2024-05-11 23:20:14.000000 cdbt-0.1.5/cdbt/main_backup.py
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-12 23:48:01.556707 cdbt-0.1.5/cdbt.egg-info/
--rw-r--r--   0 craiglathrop   (501) staff       (20)      391 2024-05-12 23:48:01.000000 cdbt-0.1.5/cdbt.egg-info/PKG-INFO
--rw-r--r--   0 craiglathrop   (501) staff       (20)      273 2024-05-12 23:48:01.000000 cdbt-0.1.5/cdbt.egg-info/SOURCES.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2024-05-12 23:48:01.000000 cdbt-0.1.5/cdbt.egg-info/dependency_links.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       43 2024-05-12 23:48:01.000000 cdbt-0.1.5/cdbt.egg-info/entry_points.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        6 2024-05-12 23:48:01.000000 cdbt-0.1.5/cdbt.egg-info/requires.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        5 2024-05-12 23:48:01.000000 cdbt-0.1.5/cdbt.egg-info/top_level.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       38 2024-05-12 23:48:01.558144 cdbt-0.1.5/setup.cfg
--rwxrwx---   0 craiglathrop   (501) staff       (20)      644 2024-05-12 19:23:35.000000 cdbt-0.1.5/setup.py
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-12 23:48:01.555573 cdbt-0.1.5/tests/
--rw-r--r--   0 craiglathrop   (501) staff       (20)     6733 2024-05-12 23:31:04.000000 cdbt-0.1.5/tests/test_main.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-13 01:55:11.435546 cdbt-0.1.6/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      391 2024-05-13 01:55:11.434951 cdbt-0.1.6/PKG-INFO
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     3396 2024-05-12 23:47:32.000000 cdbt-0.1.6/README.md
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-13 01:55:11.427585 cdbt-0.1.6/cdbt/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2024-05-11 20:22:05.000000 cdbt-0.1.6/cdbt/__init__.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     3343 2024-05-13 01:47:05.000000 cdbt-0.1.6/cdbt/cmdline.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)    12462 2024-05-13 01:54:07.000000 cdbt-0.1.6/cdbt/main.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-13 01:55:11.434355 cdbt-0.1.6/cdbt.egg-info/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      391 2024-05-13 01:55:11.000000 cdbt-0.1.6/cdbt.egg-info/PKG-INFO
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      253 2024-05-13 01:55:11.000000 cdbt-0.1.6/cdbt.egg-info/SOURCES.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2024-05-13 01:55:11.000000 cdbt-0.1.6/cdbt.egg-info/dependency_links.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       43 2024-05-13 01:55:11.000000 cdbt-0.1.6/cdbt.egg-info/entry_points.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        6 2024-05-13 01:55:11.000000 cdbt-0.1.6/cdbt.egg-info/requires.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        5 2024-05-13 01:55:11.000000 cdbt-0.1.6/cdbt.egg-info/top_level.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       38 2024-05-13 01:55:11.435620 cdbt-0.1.6/setup.cfg
+-rwxrwx---   0 craiglathrop   (501) staff       (20)      644 2024-05-13 01:55:01.000000 cdbt-0.1.6/setup.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-13 01:55:11.433454 cdbt-0.1.6/tests/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     7405 2024-05-13 01:54:07.000000 cdbt-0.1.6/tests/test_main.py
```

### Comparing `cdbt-0.1.5/README.md` & `cdbt-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `cdbt-0.1.5/cdbt/cmdline.py` & `cdbt-0.1.6/cdbt/cmdline.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,51 +29,63 @@
         return click.Group.get_command(self, ctx, cmd_name)
 
     def list_commands(self, ctx):
         # List of all commands
         return ['build', 'trun', 'run', 'test', 'compile', 'sbuild', 'pbuild']
 
 
-cdbt = CustomCmdLoader()
+@click.group()
+@click.option('--threads', type=int, help='Number of threads to use during DBT operations.')
+@click.pass_context
+def cdbt(ctx, threads):
+    ctx.obj = {}
+    ctx.obj['threads'] = threads
+
+# cdbt = CustomCmdLoader()
 
 
 @cdbt.command()
 @click.option('--full-refresh', is_flag=True, help='Run a full refresh on all models.')
 @click.option('--select', type=str, help='DBT style select string')
 @click.option('--fail-fast', is_flag=True, help='Fail fast on errors.')
-def build(full_refresh, select, fail_fast):
-    cdbt_class.build(full_refresh, select, fail_fast)
+@click.pass_context
+def build(ctx, full_refresh, select, fail_fast):
+    cdbt_class.build(ctx, full_refresh, select, fail_fast)
 
 
 @cdbt.command()
 @click.option('--full-refresh', is_flag=True, help='Run a full refresh on all models.')
 @click.option('--select', type=str, help='DBT style select string')
 @click.option('--fail-fast', is_flag=True, help='Fail fast on errors.')
-def trun(full_refresh, select, fail_fast):
-    cdbt_class.trun(full_refresh, select, fail_fast)
+@click.pass_context
+def trun(ctx, full_refresh, select, fail_fast):
+    cdbt_class.trun(ctx, full_refresh, select, fail_fast)
 
 
 @cdbt.command()
 @click.option('--full-refresh', is_flag=True, help='Run a full refresh on all models.')
 @click.option('--select', type=str, help='DBT style select string')
 @click.option('--fail-fast', is_flag=True, help='Fail fast on errors.')
-def run(full_refresh, select, fail_fast):
-    cdbt_class.run(full_refresh, select, fail_fast)
+@click.pass_context
+def run(ctx, full_refresh, select, fail_fast):
+    cdbt_class.run(ctx, full_refresh, select, fail_fast)
 
 
 @cdbt.command()
 @click.option('--select', type=str, help='DBT style select string')
 @click.option('--fail-fast', is_flag=True, help='Fail fast on errors.')
-def test(select, fail_fast):
-    cdbt_class.test(select, fail_fast)
+@click.pass_context
+def test(ctx, select, fail_fast):
+    cdbt_class.test(ctx, select, fail_fast)
 
 
 @cdbt.command()
-def compile():
-    cdbt_class.compile()
+@click.pass_context
+def compile(ctx):
+    cdbt_class.compile(ctx)
 
 
 @cdbt.command()
 @click.option('--full-refresh', is_flag=True, help='Force a full refresh on all models in build scope.')
 @click.pass_context
 def sbuild(ctx, full_refresh):
     cdbt_class.sbuild(ctx, full_refresh)
```

### Comparing `cdbt-0.1.5/cdbt/main.py` & `cdbt-0.1.6/cdbt/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import json
 import subprocess
 import re
 import sys
 import shutil
 import os
-from typing import List
+from typing import List, Optional
+import typing as t
+from click.core import Context, Command
 
 
 class ColdBoreCapitalDBT:
 
     def __init__(self, test_mode: bool = False):
         self.test_mode = test_mode
         self.dbt_ls_test_mode_output = None
         self.dbt_test_mode_command_check_value = None
         self.exclude_seed_snapshot = 'resource_type:snapshot resource_type:seed'
 
-    def build(self, full_refresh, select, fail_fast):
-        args = []
+    def build(self, ctx: Context, full_refresh, select, fail_fast):
+        args = self._create_common_args(ctx)
+
         if select:
             args.append('--select')
             args.append(select)
         if fail_fast:
             args.append('--fail-fast')
         if full_refresh:
             args.append('--full-refresh')
@@ -29,16 +32,17 @@
         except subprocess.CalledProcessError as e:
             print(e)
             sys.exit(1)
 
         if not run_result:
             raise DbtError('DBT build failed with errors.')
 
-    def trun(self, full_refresh, select, fail_fast):
-        args = ['--exclude', self.exclude_seed_snapshot]
+    def trun(self, ctx: Context, full_refresh, select, fail_fast):
+        args = self._create_common_args(ctx)
+        args = args + ['--exclude', self.exclude_seed_snapshot]
         if select:
             args.append('--select')
             args.append(select)
         if fail_fast:
             args.append('--fail-fast')
 
         if full_refresh:
@@ -50,16 +54,16 @@
             print(e)
             print('dbt build ' + ' '.join(args))
             sys.exit(1)
 
         if not run_result:
             raise DbtError('DBT build failed with errors.')
 
-    def run(self, full_refresh, select, fail_fast):
-        args = []
+    def run(self, ctx: Context, full_refresh, select, fail_fast):
+        args = self._create_common_args(ctx)
         if select:
             args.append('--select')
             args.append(select)
         if fail_fast:
             args.append('--fail-fast')
 
         run_args = args
@@ -71,16 +75,16 @@
             print(e)
             print('dbt run ' + ' '.join(args))
             sys.exit(1)
 
         if not run_result:
             raise DbtError('DBT build failed with errors.')
 
-    def test(self, select, fail_fast):
-        args = []
+    def test(self, ctx: Context, select, fail_fast):
+        args = self._create_common_args(ctx)
         if select:
             args.append('--select')
             args.append(select)
         if fail_fast:
             args.append('--fail-fast')
         run_args = args
         try:
@@ -89,35 +93,36 @@
             print(e)
             print('dbt test ' + ' '.join(args))
             sys.exit(1)
 
         if not run_result:
             raise DbtError('DBT build failed with errors.')
 
-    def compile(self):
+    def compile(self, ctx: Context):
+        # We ignore the ctx object as compile has no threads.
         try:
             self.execute_dbt_command('compile', [])
         except subprocess.CalledProcessError as e:
             print(e)
             print('dbt compile')
             sys.exit(1)
 
-    def sbuild(self, ctx, full_refresh):
+    def sbuild(self, ctx: Context, full_refresh):
         print('Starting a state build based on local manifest.json')
         artifact_dir = '_artifacts'
         target_dir = 'target'
         # Path to the artifacts file that will be generated by the dbt compile command representing the current state.
         manifest_path = os.path.join('./', target_dir, 'manifest.json')
         # Path to the artifact file that represents the prior build state.
         manifest_artifact_path = os.path.join('./', artifact_dir, 'manifest.json')
 
         self.execute_state_based_build(ctx, artifact_dir, manifest_artifact_path, manifest_path, full_refresh,
                                        roll_back_manifest_flag=True)
 
-    def pbuild(self, ctx, full_refresh):
+    def pbuild(self, ctx: Context, full_refresh):
         print('Starting a state build based on production manifest.json')
         artifact_dir = 'logs'
         target_dir = 'target'
         # Pull artifacts from Snowflake. These are the latest production artifacts.
         try:
             if not self.test_mode:
                 subprocess.run(['dbt', 'run-operation', 'get_last_artifacts'], check=True)
@@ -128,15 +133,16 @@
 
         manifest_path = os.path.join('.', target_dir, 'manifest.json')
         manifest_artifact_path = os.path.join('.', artifact_dir, 'manifest.json')
 
         self.execute_state_based_build(ctx, artifact_dir, manifest_artifact_path, manifest_path, full_refresh,
                                        roll_back_manifest_flag=False)
 
-    def execute_state_based_build(self, ctx: object, artifact_dir: str, manifest_artifact_path: str, manifest_path: str,
+    def execute_state_based_build(self, ctx: Context, artifact_dir: str, manifest_artifact_path: str,
+                                  manifest_path: str,
                                   full_refresh: bool, roll_back_manifest_flag: bool):
         if roll_back_manifest_flag and not self.test_mode:
             print(f'Making a backup of the current manifest.json at {manifest_path} to {manifest_artifact_path}')
             # Move the manifest from ./target to ./_artifacts. This becomes the prior state. Only used for local state
             # build. Not used for pdbuild (production build).
             shutil.move(manifest_path, manifest_artifact_path)
         # Execute dbt compile
@@ -162,14 +168,15 @@
 
         state_flags = [
             '--select', state_modified_str,
             '--state', os.path.join('.', artifact_dir) + '/'
         ]
         exclude_flags = ['--exclude', self.exclude_seed_snapshot]
         # Get a list of models and their config
+
         args = state_flags + exclude_flags
         args = args + ['--output-keys', 'name resource_type config', '--output', 'json']
         cmd = ['dbt', 'ls']
         cmd = cmd + args
         try:
             if self.test_mode:
                 output = self.dbt_ls_test_mode_output
@@ -190,15 +197,16 @@
 
         if not full_refresh:
             full_refresh = self.test_full_refresh(models_json)
 
         run_result = None
         # Execute dbt build excluding snapshots and seeds
         # Rest the args.
-        args = state_flags + exclude_flags
+        args = self._create_common_args(ctx)
+        args = args + state_flags + exclude_flags
         if full_refresh:
             args = args + ['--full-refresh']
 
         try:
             run_result = self.execute_dbt_command('build', args)
         except subprocess.CalledProcessError as e:
             print(e)
@@ -209,15 +217,25 @@
                 sys.exit(1)
 
         if not run_result:
             e = 'DBT build failed with errors.'
             self.roll_back_manifest(e, manifest_artifact_path, manifest_path)
             raise DbtError('DBT build failed with errors.')
 
-    def roll_back_manifest(self, e, manifest_artifact_path, manifest_path):
+    @staticmethod
+    def _create_common_args(ctx: Context):
+        args = []
+        threads = ctx.obj.get('threads', None)
+        if threads:
+            args.append('--threads')
+            args.append(str(threads))
+        return args
+
+    @staticmethod
+    def roll_back_manifest(e, manifest_artifact_path, manifest_path):
         print(f"DBT build failed. Rolling back manifest state with error\n {e}")
         # Move the manifest.json from _artifacts back to target dir. If the build failed, we want to rebuild against this
         # state, not the one generated by the compile command.
         shutil.move(manifest_artifact_path, manifest_path)
         sys.exit(1)
 
     @staticmethod
@@ -265,40 +283,44 @@
                 raise subprocess.CalledProcessError(returncode=process.returncode, cmd=dbt_command, output=stderr)
 
             # Check for errors using a regex method if necessary
             if self.contains_errors(stdout + stderr):
                 return False
             return True
 
-    def contains_errors(self, text):
+    @staticmethod
+    def contains_errors(text):
         pattern = r"([2-9]|\d{2,})\s+errors?"
         error_flag = bool(re.search(pattern, text))
-        return
+        return error_flag
 
 
 class DbtError(Exception):
     def __init__(self, message):
         self.message = 'DBT build failed with errors.'
 
     def __str__(self):
         return self.message
 
 
-class MockCtx:
-    def __init__(self):
+class MockCtx(Context):
+    def __init__(self,
+                 command: t.Optional["Command"] = None,
+                 ) -> None:
         self.obj = {
             'build_children': False,
             'build_children_count': None,
             'parents_children': False,
             'build_parent_count': None
         }
 
+
 if __name__ == '__main__':
     cdbt = ColdBoreCapitalDBT()
     # cdbt.build(full_refresh=False, select=None, fail_fast=False)
     # cdbt.trun(full_refresh=False, select=None, fail_fast=False)
     # cdbt.run(full_refresh=False, select=None, fail_fast=False)
     # cdbt.test(select=None, fail_fast=False)
     # cdbt.compile()
     # cdbt.sbuild(ctx=None, full_refresh=False)
-    cdbt.pbuild(ctx=MockCtx(), full_refresh=False)
+    cdbt.pbuild(ctx=MockCtx(Command('Duck')), full_refresh=False)
     sys.exit(0)
```

### Comparing `cdbt-0.1.5/setup.py` & `cdbt-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cdbt',
-    version='0.1.5',
+    version='0.1.6',
     description='A CLI tool to manage dbt builds with state handling and manifest management',
     author='Craig Lathrop',
     author_email='development@coldborecapital.com',
     packages=find_packages(),
     install_requires=[
         'click',
     ],
```

### Comparing `cdbt-0.1.5/tests/test_main.py` & `cdbt-0.1.6/tests/test_main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
-from unittest.mock import patch
 import json
 from cdbt.main import ColdBoreCapitalDBT, MockCtx
 
+from click.core import Context, Command
 
 class TestCdbt(unittest.TestCase):
     def setUp(self):
         self.cdbt = ColdBoreCapitalDBT()
         self.cdbt.test_mode = True
         self.incremental_ls_example = '''22:06:42 Running with dbt=1.7.9
 22:06:43 Registered adapter: snowflake=1.7.2
@@ -15,92 +15,99 @@
 
         self.non_incremental_ls_example = '''22:06:42 Running with dbt=1.7.9
 22:06:43 Registered adapter: snowflake=1.7.2
 22:06:43 Found 123 models, 26 snapshots, 118 tests, 9 seeds, 46 sources, 0 exposures, 0 metrics, 992 macros, 0 groups, 0 semantic models
 {"name": "dim_patients", "resource_type": "model", "config": {"materialized": "view"}}'''
 
     def test_build_command_full_refresh(self):
-        self.cdbt.build(full_refresh=True, select="model1", fail_fast=True)
+        self.cdbt.build(ctx=MockCtx(Command('test')), full_refresh=True, select="model1", fail_fast=True)
         expected_command = ['dbt', 'build', '--select', 'model1', '--fail-fast', '--full-refresh']
         self.assertEqual(self.cdbt.dbt_test_mode_command_check_value, expected_command)
 
+        # Test threads
+        mc = MockCtx(Command('test'))
+        mc.obj['threads'] = 5
+        self.cdbt.build(ctx=mc, full_refresh=True, select="model1", fail_fast=True)
+        expected_command = ['dbt', 'build', '--threads', '5', '--select', 'model1', '--fail-fast', '--full-refresh']
+        self.assertEqual(self.cdbt.dbt_test_mode_command_check_value, expected_command)
+
     def test_build_command_no_full_refresh(self):
-        self.cdbt.build(full_refresh=False, select="model1", fail_fast=False)
+        self.cdbt.build(ctx=MockCtx(Command('test')), full_refresh=False, select="model1", fail_fast=False)
         expected_command = ['dbt', 'build', '--select', 'model1']
         self.assertEqual(self.cdbt.dbt_test_mode_command_check_value, expected_command)
 
     def test_trun_command(self):
-        self.cdbt.trun(full_refresh=True, select="model2", fail_fast=False)
+        self.cdbt.trun(ctx=MockCtx(Command('test')), full_refresh=True, select="model2", fail_fast=False)
         expected_command = ['dbt', 'build', '--exclude', 'resource_type:snapshot resource_type:seed', '--select',
                             'model2', '--full-refresh']
         self.assertEqual(self.cdbt.dbt_test_mode_command_check_value, expected_command)
 
     def test_run_command_full_refresh(self):
-        self.cdbt.run(full_refresh=True, select="model3", fail_fast=True)
+        self.cdbt.run(ctx=MockCtx(Command('test')), full_refresh=True, select="model3", fail_fast=True)
         expected_command = ['dbt', 'run', '--select', 'model3', '--fail-fast', '--full-refresh']
         self.assertEqual(self.cdbt.dbt_test_mode_command_check_value, expected_command)
 
     def test_test_command_selective(self):
-        self.cdbt.test(select="model4", fail_fast=True)
+        self.cdbt.test(ctx=MockCtx(Command('test')), select="model4", fail_fast=True)
         expected_command = ['dbt', 'test', '--select', 'model4', '--fail-fast']
         self.assertEqual(self.cdbt.dbt_test_mode_command_check_value, expected_command)
 
     def test_compile_command(self):
-        self.cdbt.compile()
+        self.cdbt.compile(ctx=MockCtx(Command('test')))
         expected_command = ['dbt', 'compile']
         self.assertEqual(self.cdbt.dbt_test_mode_command_check_value, expected_command)
 
     def test_sbuild_output(self):
         self.cdbt.dbt_ls_test_mode_output = self.incremental_ls_example
-        self.cdbt.sbuild(ctx=MockCtx(), full_refresh=False)
+        self.cdbt.sbuild(ctx=MockCtx(Command('test')), full_refresh=False)
         expected_command = ['dbt', 'build', '--select', 'state:modified', '--state', './_artifacts/', '--exclude', 'resource_type:snapshot resource_type:seed', '--full-refresh']
         self.assertEqual(self.cdbt.dbt_test_mode_command_check_value, expected_command)
 
         # Test build parents
-        mc = MockCtx()
+        mc = MockCtx(Command('test'))
         mc.obj['build_parents'] = True
         self.cdbt.dbt_ls_test_mode_output = self.incremental_ls_example
         self.cdbt.sbuild(ctx=mc, full_refresh=False)
         expected_command = ['dbt', 'build', '--select', '+state:modified', '--state', './_artifacts/', '--exclude', 'resource_type:snapshot resource_type:seed', '--full-refresh']
         self.assertEqual(self.cdbt.dbt_test_mode_command_check_value, expected_command)
 
         # Test build parents graph count limit (i.e. 3+sbuild)
-        mc = MockCtx()
+        mc = MockCtx(Command('test'))
         mc.obj['build_parents'] = True
         mc.obj['build_parents_count'] = 3
         self.cdbt.dbt_ls_test_mode_output = self.incremental_ls_example
         self.cdbt.sbuild(ctx=mc, full_refresh=False)
         expected_command = ['dbt', 'build', '--select', '3+state:modified', '--state', './_artifacts/', '--exclude', 'resource_type:snapshot resource_type:seed', '--full-refresh']
         self.assertEqual(self.cdbt.dbt_test_mode_command_check_value, expected_command)
 
         # Test build children
-        mc = MockCtx()
+        mc = MockCtx(Command('test'))
         mc.obj['build_children'] = True
         self.cdbt.dbt_ls_test_mode_output = self.incremental_ls_example
         self.cdbt.sbuild(ctx=mc, full_refresh=False)
         expected_command = ['dbt', 'build', '--select', 'state:modified+', '--state', './_artifacts/', '--exclude', 'resource_type:snapshot resource_type:seed', '--full-refresh']
         self.assertEqual(self.cdbt.dbt_test_mode_command_check_value, expected_command)
 
         # Test build children graph count limit (i.e. sbuild+3)
-        mc = MockCtx()
+        mc = MockCtx(Command('test'))
         mc.obj['build_children'] = True
         mc.obj['build_children_count'] = 2
         self.cdbt.dbt_ls_test_mode_output = self.incremental_ls_example
         self.cdbt.sbuild(ctx=mc, full_refresh=False)
         expected_command = ['dbt', 'build', '--select', 'state:modified+2', '--state', './_artifacts/', '--exclude', 'resource_type:snapshot resource_type:seed', '--full-refresh']
         self.assertEqual(self.cdbt.dbt_test_mode_command_check_value, expected_command)
 
     def test_pbuild_output(self):
         self.cdbt.dbt_ls_test_mode_output = self.incremental_ls_example
-        self.cdbt.pbuild(ctx=MockCtx(), full_refresh=False)
+        self.cdbt.pbuild(ctx=MockCtx(Command('test')), full_refresh=False)
         expected_command = ['dbt', 'build', '--select', 'state:modified', '--state', './logs/', '--exclude', 'resource_type:snapshot resource_type:seed', '--full-refresh']
         self.assertEqual(self.cdbt.dbt_test_mode_command_check_value, expected_command)
 
         self.cdbt.dbt_ls_test_mode_output = self.non_incremental_ls_example
-        self.cdbt.pbuild(ctx=MockCtx(), full_refresh=False)
+        self.cdbt.pbuild(ctx=MockCtx(Command('test')), full_refresh=False)
         expected_command = ['dbt', 'build', '--select', 'state:modified', '--state', './logs/', '--exclude', 'resource_type:snapshot resource_type:seed']
         self.assertEqual(self.cdbt.dbt_test_mode_command_check_value, expected_command)
 
     def test_dbt_ls_test_mode_output_incremental(self):
         self.cdbt.dbt_ls_test_mode_output = self.incremental_ls_example
         result = self.cdbt.test_full_refresh([json.loads(
             '''{"name": "dim_patients", "resource_type": "model", "config": {"materialized": "incremental"}}''')])
```

