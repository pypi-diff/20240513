# Comparing `tmp/odoo-smile_test-15.0.0.tar.gz` & `tmp/odoo-smile_test-16.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/odoo-smile_test-15.0.0.tar", last modified: Mon Nov  6 15:50:45 2023, max compression
+gzip compressed data, was "odoo-smile_test-16.0.1.tar", last modified: Fri Oct  6 11:23:51 2023, max compression
```

## Comparing `odoo-smile_test-15.0.0.tar` & `odoo-smile_test-16.0.1.tar`

### file list

```diff
@@ -1,30 +1,27 @@
-drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-11-06 15:50:45.000000 odoo-smile_test-15.0.0/
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1693 2023-11-06 14:35:56.000000 odoo-smile_test-15.0.0/LICENSE.txt
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      646 2023-11-06 15:50:45.000000 odoo-smile_test-15.0.0/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      863 2023-11-06 14:35:56.000000 odoo-smile_test-15.0.0/README.md
-drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-11-06 15:50:45.000000 odoo-smile_test-15.0.0/odoo_smile_test.egg-info/
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      646 2023-11-06 15:50:45.000000 odoo-smile_test-15.0.0/odoo_smile_test.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      652 2023-11-06 15:50:45.000000 odoo-smile_test-15.0.0/odoo_smile_test.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        1 2023-11-06 15:50:45.000000 odoo-smile_test-15.0.0/odoo_smile_test.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)       56 2023-11-06 15:50:45.000000 odoo-smile_test-15.0.0/odoo_smile_test.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)       11 2023-11-06 15:50:45.000000 odoo-smile_test-15.0.0/odoo_smile_test.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)       87 2023-11-06 15:50:45.000000 odoo-smile_test-15.0.0/setup.cfg
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1024 2023-11-06 15:50:40.000000 odoo-smile_test-15.0.0/setup.py
-drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-11-06 15:50:45.000000 odoo-smile_test-15.0.0/smile_test/
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)       20 2023-11-06 14:35:56.000000 odoo-smile_test-15.0.0/smile_test/.coveragerc
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)       47 2023-11-06 14:35:56.000000 odoo-smile_test-15.0.0/smile_test/__init__.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      551 2023-11-06 14:35:56.000000 odoo-smile_test-15.0.0/smile_test/__manifest__.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     8129 2023-11-06 14:35:56.000000 odoo-smile_test-15.0.0/smile_test/run_tests.py
-drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-11-06 15:50:45.000000 odoo-smile_test-15.0.0/smile_test/service/
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)       46 2023-11-06 14:35:56.000000 odoo-smile_test-15.0.0/smile_test/service/__init__.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     3604 2023-11-06 14:35:56.000000 odoo-smile_test-15.0.0/smile_test/service/common.py
-drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-11-06 15:50:45.000000 odoo-smile_test-15.0.0/smile_test/tests/
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      143 2023-11-06 14:35:56.000000 odoo-smile_test-15.0.0/smile_test/tests/__init__.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     3390 2023-11-06 14:35:56.000000 odoo-smile_test-15.0.0/smile_test/tests/test_act_window.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     2010 2023-11-06 14:35:56.000000 odoo-smile_test-15.0.0/smile_test/tests/test_general_read.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      972 2023-11-06 14:35:56.000000 odoo-smile_test-15.0.0/smile_test/tests/test_get_views.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     2227 2023-11-06 14:35:56.000000 odoo-smile_test-15.0.0/smile_test/tests/test_ir_rule.py
-drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-11-06 15:50:45.000000 odoo-smile_test-15.0.0/smile_test/tools/
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)       76 2023-11-06 14:35:56.000000 odoo-smile_test-15.0.0/smile_test/tools/__init__.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)    14695 2023-11-06 14:35:56.000000 odoo-smile_test-15.0.0/smile_test/tools/test_utils.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     2933 2023-11-06 14:35:56.000000 odoo-smile_test-15.0.0/smile_test/tools/unit_test.py
+drwxr-xr-x   0 madec    (18152)    10000        0 2023-10-06 11:23:51.122129 odoo-smile_test-16.0.1/
+-rw-r--r--   0 madec    (18152)    10000      805 2023-10-06 11:23:51.122129 odoo-smile_test-16.0.1/PKG-INFO
+-rw-r--r--   0 madec    (18152)    10000       18 2023-10-06 10:12:35.000000 odoo-smile_test-16.0.1/README.md
+drwxr-xr-x   0 madec    (18152)    10000        0 2023-10-06 11:23:51.122129 odoo-smile_test-16.0.1/odoo_smile_test.egg-info/
+-rw-r--r--   0 madec    (18152)    10000      805 2023-10-06 11:23:51.000000 odoo-smile_test-16.0.1/odoo_smile_test.egg-info/PKG-INFO
+-rw-r--r--   0 madec    (18152)    10000      593 2023-10-06 11:23:51.000000 odoo-smile_test-16.0.1/odoo_smile_test.egg-info/SOURCES.txt
+-rw-r--r--   0 madec    (18152)    10000        1 2023-10-06 11:23:51.000000 odoo-smile_test-16.0.1/odoo_smile_test.egg-info/dependency_links.txt
+-rw-r--r--   0 madec    (18152)    10000       38 2023-10-06 11:23:51.000000 odoo-smile_test-16.0.1/odoo_smile_test.egg-info/requires.txt
+-rw-r--r--   0 madec    (18152)    10000       11 2023-10-06 11:23:51.000000 odoo-smile_test-16.0.1/odoo_smile_test.egg-info/top_level.txt
+-rw-r--r--   0 madec    (18152)    10000       79 2023-10-06 11:23:51.122129 odoo-smile_test-16.0.1/setup.cfg
+-rw-r--r--   0 madec    (18152)    10000     1117 2023-10-06 11:23:45.000000 odoo-smile_test-16.0.1/setup.py
+drwxr-xr-x   0 madec    (18152)    10000        0 2023-10-06 11:23:51.122129 odoo-smile_test-16.0.1/smile_test/
+-rw-r--r--   0 madec    (18152)    10000       47 2023-08-28 12:24:53.000000 odoo-smile_test-16.0.1/smile_test/__init__.py
+-rw-r--r--   0 madec    (18152)    10000      523 2023-08-28 12:24:53.000000 odoo-smile_test-16.0.1/smile_test/__manifest__.py
+drwxr-xr-x   0 madec    (18152)    10000        0 2023-10-06 11:23:51.122129 odoo-smile_test-16.0.1/smile_test/service/
+-rw-r--r--   0 madec    (18152)    10000       46 2023-08-28 12:24:53.000000 odoo-smile_test-16.0.1/smile_test/service/__init__.py
+-rw-r--r--   0 madec    (18152)    10000     3872 2023-08-28 12:24:53.000000 odoo-smile_test-16.0.1/smile_test/service/common.py
+drwxr-xr-x   0 madec    (18152)    10000        0 2023-10-06 11:23:51.122129 odoo-smile_test-16.0.1/smile_test/tests/
+-rw-r--r--   0 madec    (18152)    10000      143 2023-08-28 12:24:53.000000 odoo-smile_test-16.0.1/smile_test/tests/__init__.py
+-rw-r--r--   0 madec    (18152)    10000     3390 2023-08-28 12:24:53.000000 odoo-smile_test-16.0.1/smile_test/tests/test_act_window.py
+-rw-r--r--   0 madec    (18152)    10000     2010 2023-08-28 12:24:53.000000 odoo-smile_test-16.0.1/smile_test/tests/test_general_read.py
+-rw-r--r--   0 madec    (18152)    10000      972 2023-08-28 12:24:53.000000 odoo-smile_test-16.0.1/smile_test/tests/test_get_views.py
+-rw-r--r--   0 madec    (18152)    10000     2227 2023-08-28 12:24:53.000000 odoo-smile_test-16.0.1/smile_test/tests/test_ir_rule.py
+drwxr-xr-x   0 madec    (18152)    10000        0 2023-10-06 11:23:51.122129 odoo-smile_test-16.0.1/smile_test/tools/
+-rw-r--r--   0 madec    (18152)    10000       76 2023-08-28 12:24:53.000000 odoo-smile_test-16.0.1/smile_test/tools/__init__.py
+-rw-r--r--   0 madec    (18152)    10000     8887 2023-08-28 12:24:53.000000 odoo-smile_test-16.0.1/smile_test/tools/test_utils.py
+-rw-r--r--   0 madec    (18152)    10000     1641 2023-08-28 12:24:53.000000 odoo-smile_test-16.0.1/smile_test/tools/unit_test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `odoo-smile_test-15.0.0/odoo_smile_test.egg-info/SOURCES.txt` & `odoo-smile_test-16.0.1/odoo_smile_test.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-LICENSE.txt
 README.md
 setup.cfg
 setup.py
 odoo_smile_test.egg-info/PKG-INFO
 odoo_smile_test.egg-info/SOURCES.txt
 odoo_smile_test.egg-info/dependency_links.txt
 odoo_smile_test.egg-info/requires.txt
 odoo_smile_test.egg-info/top_level.txt
-smile_test/.coveragerc
 smile_test/__init__.py
 smile_test/__manifest__.py
-smile_test/run_tests.py
 smile_test/service/__init__.py
 smile_test/service/common.py
 smile_test/tests/__init__.py
 smile_test/tests/test_act_window.py
 smile_test/tests/test_general_read.py
 smile_test/tests/test_get_views.py
 smile_test/tests/test_ir_rule.py
```

### Comparing `odoo-smile_test-15.0.0/setup.py` & `odoo-smile_test-16.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 
 setup(
     name='odoo-smile_test',
-    version='15.0.0',
+    version='16.0.1',
     packages=find_packages(),
-    data_files=[
-        'smile_test/.coveragerc',
-    ],
     include_package_data=True,
     license='LGPL',
     description='Smile test module',
     author='Smile',
     author_email='martin.deconinck@smile.fr',
+    url='https://github.com/madecsmile/odoo_smile_test',
+    download_url='https://github.com/madecsmile/odoo_smile_test/archive/refs/tags/16.0.0.zip',
     keywords=['odoo', 'test', 'smile_test', 'smile'],
-    install_requires=[
+    install_requires=[            # I get to this in a second
         'coverage',
         'flake8',
         'unittest2',
         'pycobertura',
-        'xmlrunner',
-        'debugpy',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
         'Programming Language :: Python :: 3',
```

### Comparing `odoo-smile_test-15.0.0/smile_test/__manifest__.py` & `odoo-smile_test-16.0.1/smile_test/__manifest__.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 """,
     "author": "Smile",
     "website": "http://www.smile.fr",
     "license": "AGPL-3",
     "depends": ["base"],
     "auto_install": True,
     "external_dependencies": {
-        "python": ["coverage", "xmlrunner", "pycobertura"],
+        "python": ["coverage"],
         "bin": ["flake8"],
     },
 }
```

### Comparing `odoo-smile_test-15.0.0/smile_test/service/common.py` & `odoo-smile_test-16.0.1/smile_test/service/common.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,78 +1,87 @@
 # -*- coding: utf-8 -*-
 
+import coverage
 import logging
 import os
 import threading
-import coverage
 
 from odoo.service import common
 from odoo.service.db import check_super
 from odoo.tests.common import BaseCase
 from odoo.tools import config
-from odoo.modules import get_module_path
 
 from .. import tools
 
 _logger = logging.getLogger(__name__)
 
-
 OMIT_FILES = [
     "__manifest__.py",
-    "__openerp__.py",
-    "__terp__.py",
     "__init__.py",
 ]
-OMIT_DIRS = ["web", "static", "controllers", "doc", "test", "tests"]
+OMIT_DIRS = ["web", "static", "controllers", "doc", "tests"]
 
 
 class NewServices:
+    @staticmethod
+    def _get_coverage_sources():
+        coverage_sources = []
+        if config.get("code_path"):
+            for relpath in config["code_path"].split(","):
+                for dirpath, dirnames, filenames in os.walk(relpath):
+                    for omit in OMIT_DIRS:
+                        if f"*/{omit}/*" in dirpath:
+                            break
+                    else:
+                        coverage_sources.extend(
+                            os.path.join(dirpath, filename)
+                            for filename in filenames
+                            if (
+                                filename.endswith(".py")
+                                and filename not in OMIT_FILES
+                            )
+                        )
+        return coverage_sources
 
     @staticmethod
     def coverage_start():
         if hasattr(common, "coverage"):
             return False
         _logger.info("Starting code coverage...")
-        module_path = get_module_path('smile_test')
-        dft_config_file = os.path.join(module_path, ".coveragerc")
-        _logger.info('default coveragerc file: %s', dft_config_file)
-        config_file = config.get("coverage_config_file") or dft_config_file
-        _logger.info('coverage config file: %s', config_file)
-        data_file = config.get("coverage_data_file") or '/tmp/.coveragerc'
-        common.coverage = coverage.coverage(
-            data_file=data_file,
-            config_file=config_file,
-        )
+        data_file = config.get("coverage_data_file") or "/tmp/.coverage"
+        common.coverage = coverage.coverage(branch=True, data_file=data_file)
+        common.coverage.exclude("(.*?)fields.(.*?)")
         common.coverage.start()
         return True
 
     @staticmethod
     def coverage_stop():
         if not hasattr(common, "coverage"):
             return False
         _logger.info("Stopping code coverage...")
         common.coverage.stop()
         common.coverage.save()
         coverage_result = tools.test_utils._get_coverage_result_file()
+        sources = NewServices._get_coverage_sources()
         common.coverage.xml_report(
+            morfs=sources,
             outfile=coverage_result,
             ignore_errors=True,
         )
         del common.coverage
         return True
 
     @staticmethod
     def run_tests(dbname, modules=None, with_coverage=True):
         init_test_enable = config.get("test_enable")
         config["test_enable"] = True
         threading.currentThread().dbname = dbname
         modules = tools.filter_modules_list(dbname, modules)
         tools.test_utils._remove_results_files()
         tools.run_unit_tests(dbname, modules)
-        tools.run_other_tests(dbname, modules)
         config["test_enable"] = init_test_enable
         return True
 
     @staticmethod
     def prepare_results_files():
         result = {"tests": {}}
         coverage_result_file = tools.test_utils._get_coverage_result_file()
@@ -89,33 +98,29 @@
 native_dispatch = common.dispatch
 additional_methods = [
     attr
     for attr in dir(NewServices)
     if not attr.startswith("_") and callable(getattr(NewServices, attr))
 ]
 
+
 def new_dispatch(*args):
-    i = 0
-    method = args[i]
+    method = args[0]
     if method in additional_methods:
-        params = args[i + 1]
+        params = args[1]
         admin_passwd, params = params[0], params[1:]
         check_super(admin_passwd)
         return getattr(NewServices, method)(*params)
     return native_dispatch(*args)
 
 
 common.dispatch = new_dispatch
 
-# only if AUTO_COVERAGE env var is set
-if os.environ.get("AUTO_COVERAGE", False):
-    NewServices.coverage_start()
 
 @classmethod
 def tearDownClass(cls):
-    if hasattr(cls, "cr"):
-        cls.cr.close()
+    cls.cr.close()
     old_tearDownClass()
 
 
 old_tearDownClass = BaseCase.tearDownClass
 BaseCase.tearDownClass = tearDownClass
```

### Comparing `odoo-smile_test-15.0.0/smile_test/tests/test_act_window.py` & `odoo-smile_test-16.0.1/smile_test/tests/test_act_window.py`

 * *Files identical despite different names*

### Comparing `odoo-smile_test-15.0.0/smile_test/tests/test_general_read.py` & `odoo-smile_test-16.0.1/smile_test/tests/test_general_read.py`

 * *Files identical despite different names*

### Comparing `odoo-smile_test-15.0.0/smile_test/tests/test_get_views.py` & `odoo-smile_test-16.0.1/smile_test/tests/test_get_views.py`

 * *Files identical despite different names*

### Comparing `odoo-smile_test-15.0.0/smile_test/tests/test_ir_rule.py` & `odoo-smile_test-16.0.1/smile_test/tests/test_ir_rule.py`

 * *Files identical despite different names*

