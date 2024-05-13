# Comparing `tmp/roc-punk-0.2.7.tar.gz` & `tmp/roc-punk-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roc-punk-0.2.7.tar", max compression
+gzip compressed data, was "roc-punk-0.2.8.tar", max compression
```

## Comparing `roc-punk-0.2.7.tar` & `roc-punk-0.2.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      240 2023-01-30 16:00:29.919606 roc-punk-0.2.7/README.md
--rw-r--r--   0        0        0     1131 2023-02-03 15:35:48.181362 roc-punk-0.2.7/pyproject.toml
--rw-r--r--   0        0        0       67 2023-01-30 16:00:29.919606 roc-punk-0.2.7/roc/punk/__init__.py
--rw-r--r--   0        0        0     3438 2023-01-30 16:00:29.919606 roc-punk-0.2.7/roc/punk/commands.py
--rw-r--r--   0        0        0     1629 2023-02-02 15:46:04.514064 roc-punk-0.2.7/roc/punk/constants.py
--rw-r--r--   0        0        0     1126 2023-02-03 15:35:48.181362 roc-punk-0.2.7/roc/punk/descriptor.json
--rw-r--r--   0        0        0      210 2023-01-30 16:00:29.919606 roc-punk-0.2.7/roc/punk/tasks/__init__.py
--rw-r--r--   0        0        0     2920 2023-01-30 16:00:29.919606 roc-punk-0.2.7/roc/punk/tasks/descriptor_report.py
--rw-r--r--   0        0        0     2982 2023-02-03 15:35:48.181362 roc-punk-0.2.7/roc/punk/tasks/sbm_query.py
--rw-r--r--   0        0        0     2413 2023-01-30 16:00:29.919606 roc-punk-0.2.7/roc/punk/tasks/sbm_report.py
--rw-r--r--   0        0        0      810 2023-01-30 16:00:29.919606 roc-punk-0.2.7/roc/punk/tasks.py
--rw-r--r--   0        0        0       67 2023-01-30 16:00:29.919606 roc-punk-0.2.7/roc/punk/templates/__init__.py
--rw-r--r--   0        0        0     5934 2023-01-30 16:00:29.919606 roc-punk-0.2.7/roc/punk/templates/software_report.html
--rw-r--r--   0        0        0       67 2023-01-30 16:00:29.919606 roc-punk-0.2.7/roc/punk/tests/__init__.py
--rw-r--r--   0        0        0     1321 2023-01-30 16:00:29.919606 roc-punk-0.2.7/roc/punk/tests/test_punk.py
--rw-r--r--   0        0        0     5218 2023-01-30 16:00:29.923606 roc-punk-0.2.7/roc/punk/tests/test_sbm.py
--rw-r--r--   0        0        0     1125 2023-02-03 15:49:29.926743 roc-punk-0.2.7/setup.py
--rw-r--r--   0        0        0     1085 2023-02-03 15:49:29.927013 roc-punk-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      240 2024-05-13 08:26:29.046908 roc-punk-0.2.8/README.md
+-rw-r--r--   0        0        0     1131 2024-05-13 08:26:29.054908 roc-punk-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0       67 2024-05-13 08:26:29.054908 roc-punk-0.2.8/roc/punk/__init__.py
+-rw-r--r--   0        0        0     3438 2024-05-13 08:26:29.054908 roc-punk-0.2.8/roc/punk/commands.py
+-rw-r--r--   0        0        0     1629 2024-05-13 08:26:29.054908 roc-punk-0.2.8/roc/punk/constants.py
+-rw-r--r--   0        0        0     1126 2024-05-13 08:26:29.054908 roc-punk-0.2.8/roc/punk/descriptor.json
+-rw-r--r--   0        0        0      210 2024-05-13 08:26:29.054908 roc-punk-0.2.8/roc/punk/tasks/__init__.py
+-rw-r--r--   0        0        0     2920 2024-05-13 08:26:29.054908 roc-punk-0.2.8/roc/punk/tasks/descriptor_report.py
+-rw-r--r--   0        0        0     3033 2024-05-13 08:26:29.054908 roc-punk-0.2.8/roc/punk/tasks/sbm_query.py
+-rw-r--r--   0        0        0     2413 2024-05-13 08:26:29.054908 roc-punk-0.2.8/roc/punk/tasks/sbm_report.py
+-rw-r--r--   0        0        0      810 2024-05-13 08:26:29.054908 roc-punk-0.2.8/roc/punk/tasks.py
+-rw-r--r--   0        0        0       67 2024-05-13 08:26:29.054908 roc-punk-0.2.8/roc/punk/templates/__init__.py
+-rw-r--r--   0        0        0     5934 2024-05-13 08:26:29.054908 roc-punk-0.2.8/roc/punk/templates/software_report.html
+-rw-r--r--   0        0        0       67 2024-05-13 08:26:29.054908 roc-punk-0.2.8/roc/punk/tests/__init__.py
+-rw-r--r--   0        0        0     1321 2024-05-13 08:26:29.054908 roc-punk-0.2.8/roc/punk/tests/test_punk.py
+-rw-r--r--   0        0        0     5218 2024-05-13 08:26:29.054908 roc-punk-0.2.8/roc/punk/tests/test_sbm.py
+-rw-r--r--   0        0        0     1125 2024-05-13 08:30:49.553323 roc-punk-0.2.8/setup.py
+-rw-r--r--   0        0        0     1085 2024-05-13 08:30:49.553630 roc-punk-0.2.8/PKG-INFO
```

### Comparing `roc-punk-0.2.7/pyproject.toml` & `roc-punk-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 skip-string-normalization = true
 line-length = 79
 include = "\\.pyi?$"
 exclude = "/(\n    \\.git\n  | \\.hg\n  | \\.mypy_cache\n  | \\.tox\n  | \\.venv\n  | _build\n  | buck-out\n  | build\n  | dist\n)/\n"
 
 [tool.poetry]
 name = "roc-punk"
-version = "0.2.7"
+version = "0.2.8"
 readme = "README.md"
 license = "CeCILL-C"
 repository = "https://gitlab.obspm.fr/ROC/Pipelines/Plugins/PUNK"
 description = "Pipeline UNit Keeper (PUNK) plugin is used to report activities monitored by the pipeline"
 authors = [ "Florence Henry <florence.henry@obspm.fr>", "ROC Team <roc.support@sympa.obspm.fr>",]
 exclude = [ "bump_descriptor.py",]
 [[tool.poetry.packages]]
```

### Comparing `roc-punk-0.2.7/roc/punk/commands.py` & `roc-punk-0.2.8/roc/punk/commands.py`

 * *Files identical despite different names*

### Comparing `roc-punk-0.2.7/roc/punk/constants.py` & `roc-punk-0.2.8/roc/punk/constants.py`

 * *Files identical despite different names*

### Comparing `roc-punk-0.2.7/roc/punk/descriptor.json` & `roc-punk-0.2.8/roc/punk/descriptor.json`

 * *Files identical despite different names*

### Comparing `roc-punk-0.2.7/roc/punk/tasks/descriptor_report.py` & `roc-punk-0.2.8/roc/punk/tasks/descriptor_report.py`

 * *Files identical despite different names*

### Comparing `roc-punk-0.2.7/roc/punk/tasks/sbm_query.py` & `roc-punk-0.2.8/roc/punk/tasks/sbm_query.py`

 * *Files 8% similar despite different names*

```diff
@@ -89,13 +89,14 @@
 
         params = {}
         params['title'] = f'[SBM{self.sbm_type}] Report from {period}'
         params['labels'] = 'SBM'
         params['assignee_id'] = 35  # 35 is xbonnin
         params['description'] = f'{len(sbms)} SBM type {self.sbm_type} '\
                                 f'detections from {period}:\n\n'
-        params['description'] += '@xbonnin @dberard @maksimov @jsoucek\n\n'
+        params['description'] += '@xbonnin @dberard @maksimov '\
+                                 '@jsoucek @oalexandrova\n\n'
         for sbm in sbms:
             params['description'] += f'- {sbm.utc_time} {sissi_url}/{sbm.id}\n'
 
         # Set outputs
         self.outputs['report_params'].data = params
```

### Comparing `roc-punk-0.2.7/roc/punk/tasks/sbm_report.py` & `roc-punk-0.2.8/roc/punk/tasks/sbm_report.py`

 * *Files identical despite different names*

### Comparing `roc-punk-0.2.7/roc/punk/tasks.py` & `roc-punk-0.2.8/roc/punk/tasks.py`

 * *Files identical despite different names*

### Comparing `roc-punk-0.2.7/roc/punk/templates/software_report.html` & `roc-punk-0.2.8/roc/punk/templates/software_report.html`

 * *Files identical despite different names*

### Comparing `roc-punk-0.2.7/roc/punk/tests/test_punk.py` & `roc-punk-0.2.8/roc/punk/tests/test_punk.py`

 * *Files identical despite different names*

### Comparing `roc-punk-0.2.7/roc/punk/tests/test_sbm.py` & `roc-punk-0.2.8/roc/punk/tests/test_sbm.py`

 * *Files identical despite different names*

### Comparing `roc-punk-0.2.7/setup.py` & `roc-punk-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'poppy-core>=0.9.4',
  'poppy-pop>=0.7.5',
  'psycopg2>=2.8.4,<3.0.0',
  'weasyprint==0.28']
 
 setup_kwargs = {
     'name': 'roc-punk',
-    'version': '0.2.7',
+    'version': '0.2.8',
     'description': 'Pipeline UNit Keeper (PUNK) plugin is used to report activities monitored by the pipeline',
     'long_description': 'PUNK PLUGIN README\n===================\n\nThis directory contains the source files of the Pipeline UNit Keeper (PUNK), a plugin used to monitor and report the ROC pipeline activities.\nPUNK is developed with and run under the POPPY framework.\n',
     'author': 'Florence Henry',
     'author_email': 'florence.henry@obspm.fr',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.obspm.fr/ROC/Pipelines/Plugins/PUNK',
```

### Comparing `roc-punk-0.2.7/PKG-INFO` & `roc-punk-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roc-punk
-Version: 0.2.7
+Version: 0.2.8
 Summary: Pipeline UNit Keeper (PUNK) plugin is used to report activities monitored by the pipeline
 Home-page: https://gitlab.obspm.fr/ROC/Pipelines/Plugins/PUNK
 License: CECILL-C
 Author: Florence Henry
 Author-email: florence.henry@obspm.fr
 Requires-Python: >=3.8,<4
 Classifier: License :: CeCILL-C Free Software License Agreement (CECILL-C)
```

