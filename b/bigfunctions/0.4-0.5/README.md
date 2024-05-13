# Comparing `tmp/bigfunctions-0.4.tar.gz` & `tmp/bigfunctions-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigfunctions-0.4.tar", last modified: Fri May 10 17:04:08 2024, max compression
+gzip compressed data, was "bigfunctions-0.5.tar", last modified: Mon May 13 12:50:19 2024, max compression
```

## Comparing `bigfunctions-0.4.tar` & `bigfunctions-0.5.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 17:04:08.428198 bigfunctions-0.4/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1064 2023-11-08 21:20:23.000000 bigfunctions-0.4/LICENSE
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9822 2024-05-10 17:04:08.427198 bigfunctions-0.4/PKG-INFO
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9097 2024-02-22 22:16:20.000000 bigfunctions-0.4/README.md
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 17:04:08.401196 bigfunctions-0.4/bigfun/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2023-11-08 21:20:23.000000 bigfunctions-0.4/bigfun/__init__.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9876 2024-05-10 13:07:40.000000 bigfunctions-0.4/bigfun/bigfunctions.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     7860 2024-05-10 13:28:21.000000 bigfunctions-0.4/bigfun/cli.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      844 2023-12-01 17:33:50.000000 bigfunctions-0.4/bigfun/load_table.py
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 17:04:08.420198 bigfunctions-0.4/bigfun/templates/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1086 2023-11-08 21:20:23.000000 bigfunctions-0.4/bigfun/templates/Dockerfile
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    11320 2024-05-10 12:31:51.000000 bigfunctions-0.4/bigfun/templates/bigfunction.md
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     3784 2024-01-19 20:34:23.000000 bigfunctions-0.4/bigfun/templates/bookmarklet.js
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1618 2024-05-10 09:49:39.000000 bigfunctions-0.4/bigfun/templates/categories.md
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1958 2024-03-01 20:43:46.000000 bigfunctions-0.4/bigfun/templates/categories.yaml
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     4164 2024-01-24 23:20:01.000000 bigfunctions-0.4/bigfun/templates/data.md
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      554 2024-02-23 19:54:09.000000 bigfunctions-0.4/bigfun/templates/function_js.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     7724 2024-02-23 21:48:51.000000 bigfunctions-0.4/bigfun/templates/function_py.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      316 2024-02-23 19:48:03.000000 bigfunctions-0.4/bigfun/templates/function_py.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      212 2024-02-23 21:42:39.000000 bigfunctions-0.4/bigfun/templates/function_py_test.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      410 2024-02-23 19:54:09.000000 bigfunctions-0.4/bigfun/templates/function_sql.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      251 2024-02-23 22:59:01.000000 bigfunctions-0.4/bigfun/templates/function_sql_test.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      702 2024-02-23 19:54:09.000000 bigfunctions-0.4/bigfun/templates/procedure.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      717 2024-02-23 22:23:06.000000 bigfunctions-0.4/bigfun/templates/procedure_test.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      345 2024-02-23 19:54:09.000000 bigfunctions-0.4/bigfun/templates/table_function.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    13249 2024-02-28 09:48:29.000000 bigfunctions-0.4/bigfun/utils.py
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 17:04:08.420198 bigfunctions-0.4/bigfun/website/
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 17:04:08.424198 bigfunctions-0.4/bigfun/website/assets/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1714 2023-11-29 13:48:58.000000 bigfunctions-0.4/bigfun/website/assets/GitHub-Mark-32px.png
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)  1353755 2024-01-19 20:34:23.000000 bigfunctions-0.4/bigfun/website/assets/bookmarklet_usage.gif
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    23806 2023-11-29 13:48:58.000000 bigfunctions-0.4/bigfun/website/assets/logo.png
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    73519 2023-11-29 13:48:58.000000 bigfunctions-0.4/bigfun/website/assets/logo_and_name.png
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    49771 2023-11-29 13:48:58.000000 bigfunctions-0.4/bigfun/website/assets/logo_and_name_wo_supercharge.png
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      888 2024-05-10 16:32:26.000000 bigfunctions-0.4/bigfun/website/mkdocs.yml
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 17:04:08.425198 bigfunctions-0.4/bigfun/website/theme_overrides/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     6185 2024-05-10 12:11:21.000000 bigfunctions-0.4/bigfun/website/theme_overrides/main.html
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 17:04:08.427198 bigfunctions-0.4/bigfunctions.egg-info/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9822 2024-05-10 17:04:08.000000 bigfunctions-0.4/bigfunctions.egg-info/PKG-INFO
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1109 2024-05-10 17:04:08.000000 bigfunctions-0.4/bigfunctions.egg-info/SOURCES.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        1 2024-05-10 17:04:08.000000 bigfunctions-0.4/bigfunctions.egg-info/dependency_links.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       42 2024-05-10 17:04:08.000000 bigfunctions-0.4/bigfunctions.egg-info/entry_points.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      130 2024-05-10 17:04:08.000000 bigfunctions-0.4/bigfunctions.egg-info/requires.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        7 2024-05-10 17:04:08.000000 bigfunctions-0.4/bigfunctions.egg-info/top_level.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       38 2024-05-10 17:04:08.428198 bigfunctions-0.4/setup.cfg
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1112 2024-05-10 17:03:58.000000 bigfunctions-0.4/setup.py
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 12:50:19.496251 bigfunctions-0.5/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1064 2023-11-08 21:20:23.000000 bigfunctions-0.5/LICENSE
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9822 2024-05-13 12:50:19.495251 bigfunctions-0.5/PKG-INFO
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9097 2024-02-22 22:16:20.000000 bigfunctions-0.5/README.md
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 12:50:19.151225 bigfunctions-0.5/bigfun/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2023-11-08 21:20:23.000000 bigfunctions-0.5/bigfun/__init__.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     8507 2024-05-10 19:42:48.000000 bigfunctions-0.5/bigfun/bigfunctions.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9663 2024-05-10 19:32:19.000000 bigfunctions-0.5/bigfun/cli.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      844 2023-12-01 17:33:50.000000 bigfunctions-0.5/bigfun/load_table.py
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 12:50:19.302236 bigfunctions-0.5/bigfun/templates/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1086 2023-11-08 21:20:23.000000 bigfunctions-0.5/bigfun/templates/Dockerfile
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    11722 2024-05-10 19:28:43.000000 bigfunctions-0.5/bigfun/templates/bigfunction.md
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     3784 2024-01-19 20:34:23.000000 bigfunctions-0.5/bigfun/templates/bookmarklet.js
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1618 2024-05-10 09:49:39.000000 bigfunctions-0.5/bigfun/templates/categories.md
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     4164 2024-01-24 23:20:01.000000 bigfunctions-0.5/bigfun/templates/data.md
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      554 2024-02-23 19:54:09.000000 bigfunctions-0.5/bigfun/templates/function_js.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     7724 2024-02-23 21:48:51.000000 bigfunctions-0.5/bigfun/templates/function_py.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      316 2024-02-23 19:48:03.000000 bigfunctions-0.5/bigfun/templates/function_py.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      212 2024-02-23 21:42:39.000000 bigfunctions-0.5/bigfun/templates/function_py_test.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      410 2024-02-23 19:54:09.000000 bigfunctions-0.5/bigfun/templates/function_sql.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      251 2024-02-23 22:59:01.000000 bigfunctions-0.5/bigfun/templates/function_sql_test.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      702 2024-02-23 19:54:09.000000 bigfunctions-0.5/bigfun/templates/procedure.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      717 2024-02-23 22:23:06.000000 bigfunctions-0.5/bigfun/templates/procedure_test.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      345 2024-02-23 19:54:09.000000 bigfunctions-0.5/bigfun/templates/table_function.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    13269 2024-05-10 19:41:56.000000 bigfunctions-0.5/bigfun/utils.py
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 12:50:19.303236 bigfunctions-0.5/bigfun/website/
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 12:50:19.468249 bigfunctions-0.5/bigfun/website/assets/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1714 2023-11-29 13:48:58.000000 bigfunctions-0.5/bigfun/website/assets/GitHub-Mark-32px.png
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)  1353755 2024-01-19 20:34:23.000000 bigfunctions-0.5/bigfun/website/assets/bookmarklet_usage.gif
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    23806 2023-11-29 13:48:58.000000 bigfunctions-0.5/bigfun/website/assets/logo.png
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    73519 2023-11-29 13:48:58.000000 bigfunctions-0.5/bigfun/website/assets/logo_and_name.png
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    49771 2023-11-29 13:48:58.000000 bigfunctions-0.5/bigfun/website/assets/logo_and_name_wo_supercharge.png
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1712 2024-05-10 18:53:52.000000 bigfunctions-0.5/bigfun/website/mkdocs.yml
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 12:50:19.476249 bigfunctions-0.5/bigfun/website/theme_overrides/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     6185 2024-05-10 12:11:21.000000 bigfunctions-0.5/bigfun/website/theme_overrides/main.html
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 12:50:19.495251 bigfunctions-0.5/bigfunctions.egg-info/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9822 2024-05-13 12:50:19.000000 bigfunctions-0.5/bigfunctions.egg-info/PKG-INFO
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1076 2024-05-13 12:50:19.000000 bigfunctions-0.5/bigfunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        1 2024-05-13 12:50:19.000000 bigfunctions-0.5/bigfunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       42 2024-05-13 12:50:19.000000 bigfunctions-0.5/bigfunctions.egg-info/entry_points.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      130 2024-05-13 12:50:19.000000 bigfunctions-0.5/bigfunctions.egg-info/requires.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        7 2024-05-13 12:50:19.000000 bigfunctions-0.5/bigfunctions.egg-info/top_level.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       38 2024-05-13 12:50:19.496251 bigfunctions-0.5/setup.cfg
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1112 2024-05-13 12:49:39.000000 bigfunctions-0.5/setup.py
```

### Comparing `bigfunctions-0.4/LICENSE` & `bigfunctions-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.4/PKG-INFO` & `bigfunctions-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: bigfunctions
-Version: 0.4
+Version: 0.5
 Summary: Supercharge BigQuery with BigFunctions
-Download-URL: https://github.com/unytics/bigfunctions/archive/refs/tags/v0.4.tar.gz
+Download-URL: https://github.com/unytics/bigfunctions/archive/refs/tags/v0.5.tar.gz
 Author: Unytics
 Author-email: paul.marcombes@unytics.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: bigfunctions Version: 0.4 Summary: Supercharge
+Metadata-Version: 2.1 Name: bigfunctions Version: 0.5 Summary: Supercharge
 BigQuery with BigFunctions Download-URL: https://github.com/unytics/
-bigfunctions/archive/refs/tags/v0.4.tar.gz Author: Unytics Author-email:
+bigfunctions/archive/refs/tags/v0.5.tar.gz Author: Unytics Author-email:
 paul.marcombes@unytics.io Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.10 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: google-cloud-bigquery Requires-
 Dist: google-cloud-bigquery_connection Requires-Dist: google-cloud-storage
 Requires-Dist: pyyaml Requires-Dist: jinja2 Requires-Dist: mkdocs-material
 Requires-Dist: click Requires-Dist: click-help-colors
```

### Comparing `bigfunctions-0.4/README.md` & `bigfunctions-0.5/README.md`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.4/bigfun/bigfunctions.py` & `bigfunctions-0.5/bigfun/bigfunctions.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,55 +11,27 @@
 from .utils import BigQuery, CloudRun, handle_error, print_success, print_info, print_command, build_and_upload_npm_package, merge_dict
 
 BIGFUNCTIONS_FOLDER = 'bigfunctions'
 DEFAULT_CONFIG_FILENAME = './config.yaml'
 REMOTE_CONNECTION_NAME = 'remote-bigfunctions'
 TEMPLATE_FOLDER = os.path.dirname(os.path.realpath(__file__)).replace('\\', '/') + '/templates'
 BIGFUNCTION_DOC_TEMPLATE_FILENAME = f'{TEMPLATE_FOLDER}/bigfunction.md'
-CATEGORIES_DOC_TEMPLATE_FILENAME = f'{TEMPLATE_FOLDER}/categories.md'
 DEFAULT_CONFIG = yaml.safe_load(open(DEFAULT_CONFIG_FILENAME, encoding='utf-8').read()) if os.path.isfile(DEFAULT_CONFIG_FILENAME) else {}
 TESTS_FOLDER = 'tests'
-CATEGORIES_FILENAME = 'categories.yaml'
-
 
 BIGFUNCTION_DOC_TEMPLATE = jinja2.Template(open(BIGFUNCTION_DOC_TEMPLATE_FILENAME, encoding='utf-8').read())
-DOC_FOLDER = 'docs/'
 
 
 
 
 
 def list_bigfunctions():
     return [f.replace('.yaml', '') for f in os.listdir(BIGFUNCTIONS_FOLDER) if f.endswith('.yaml')]
 
 
-def generate_doc(project, dataset):
-    shutil.rmtree(f'{DOC_FOLDER}/bigfunctions', ignore_errors=True)
-    os.makedirs(f'{DOC_FOLDER}/bigfunctions')
-
-    if not os.path.isfile(CATEGORIES_FILENAME):
-        print('INFO: CREATING A categories.yaml FILE IN CURRENT DIRECTORY CONTAINING BIGFUNCTIONS CATEGORIES FOR DOCUMENTATION')
-        shutil.copyfile(f'{TEMPLATE_FOLDER}/{CATEGORIES_FILENAME}', CATEGORIES_FILENAME)
-
-    bigfunctions = [
-        BigFunction(bigfunction_name, project=project, dataset=dataset)
-        for bigfunction_name in list_bigfunctions()
-    ]
-    for bigfunction in bigfunctions:
-        open(f'{DOC_FOLDER}/bigfunctions/{bigfunction.name}.md', 'w', encoding='utf-8').write(bigfunction.doc)
-
-    categories = yaml.safe_load(open(CATEGORIES_FILENAME, encoding='utf-8').read())
-    for category in categories:
-        category['bigfunctions'] = [b.config for b in bigfunctions if b.config['category'] == category['name']]
-    categories = [category for category in categories if category['bigfunctions']]
-    categories_template = jinja2.Template(open(CATEGORIES_DOC_TEMPLATE_FILENAME, encoding='utf-8').read())
-    categories_doc = categories_template.render(categories=categories, project=project, dataset=dataset)
-    open(f'{DOC_FOLDER}/bigfunctions/README.md', 'w', encoding='utf-8').write(categories_doc)
-
-
 
 class BigFunction:
 
     def __init__(self, name, project=None, dataset=None, **config_override):
         self.name = name
         self.config_override = config_override
         if project:
@@ -115,14 +87,18 @@
 
     @property
     def dataset(self):
         if self._dataset is None:
             self._dataset = self.bigquery.get_dataset(f'{self.project}.{self.dataset_name}')
         return self._dataset
 
+    @property
+    def location(self):
+        return self.dataset.location
+
     def test(self):
         # WARNING: TO CHANGE THIS AND DEPLOY A PYTHON FUNCTION HERE WE NEED TO HAVE A REMOTE CONNECTION PER DATASET AS users between dataset and remote connection are identical
         if self.config['type'] == 'function_py':
             return self._test_python_function_locally()
         self.deploy()
         print_info('Executing function with examples')
         template_file = f'{TEMPLATE_FOLDER}/{self.config["type"]}_test.sql'
@@ -159,15 +135,15 @@
             self._deploy_npm_packages()
         if self.config['type'] == 'function_py':
             self._deploy_cloud_run()
         template_file = f'{TEMPLATE_FOLDER}/{self.config["type"]}.sql'
         template = jinja2.Template(open(template_file, encoding='utf-8').read())
         query = template.render(**self.config)
         print_info('Creating function in dataset')
-        self.bigquery.query(query)
+        self.bigquery.query(query, location=self.location)
         print_success(f'successfully created {self.project}.{self.dataset_name}.{self.name}')
 
     @property
     def doc(self):
         return BIGFUNCTION_DOC_TEMPLATE.render(**self.config)
 
     def _deploy_npm_packages(self):
```

### Comparing `bigfunctions-0.4/bigfun/cli.py` & `bigfunctions-0.5/bigfun/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import os
 import shutil
 import multiprocessing
 
+import jinja2
 import yaml
 import click
 from click_help_colors import HelpColorsGroup
 from watchdog.observers import Observer
 from watchdog.events import RegexMatchingEventHandler
 
 from . import bigfunctions as bf
 from . import utils
 
 
-
 TABLES_FOLDER = 'data'
 THIS_FOLDER = os.path.dirname(os.path.realpath(__file__)).replace('\\', '/')
 WEBSITE_CONFIG_FOLDER = THIS_FOLDER + '/website'
+CATEGORIES_DOC_TEMPLATE_FILENAME = f'{THIS_FOLDER}/templates/categories.md'
 CONFIG_FILENAME = 'config.yaml'
 CONFIG = {}
 if os.path.exists(CONFIG_FILENAME):
     CONFIG = yaml.safe_load(open(CONFIG_FILENAME, encoding='utf-8').read()) or {}
 
 
 def get_config_value(name):
@@ -35,40 +36,68 @@
     CONFIG[name] = click.prompt(text, default=default)
     with open(CONFIG_FILENAME, 'w', encoding='utf-8') as outfile:
         yaml.dump(CONFIG, outfile, default_flow_style=False)
     return CONFIG[name]
 
 
 def generate_doc(project, dataset):
-    os.makedirs('docs', exist_ok=True)
-
-    if not os.path.isfile('README.md'):
-        print('INFO: CREATING A README.md FILE IN CURRENT DIRECTORY WHICH WILL BE THE ROOT CONTENT OF THE WEBSITE')
-        open('README.md', 'w', encoding='utf-8').write('# Hello from README!')
-
-    if not os.path.isfile('mkdocs.yml'):
-        print('INFO: CREATING mkdocs.yml FILE in CURRENT DIRECTORY. It is the configuration file of the website...')
-        shutil.copyfile(WEBSITE_CONFIG_FOLDER + '/mkdocs.yml', 'mkdocs.yml')
-
-    if not os.path.isdir('docs/assets'):
-        print('INFO: COPYING assets FOLDER into docs FOLDER...')
-        shutil.copytree(WEBSITE_CONFIG_FOLDER + '/assets', 'docs/assets')
-
-    if not os.path.isdir('docs/theme_overrides'):
-        print('INFO: COPYING theme_overrides FOLDER into docs FOLDER...')
-        shutil.copytree(WEBSITE_CONFIG_FOLDER + '/theme_overrides', 'docs/theme_overrides')
-
-    shutil.copyfile('README.md', 'docs/README.md')
-    if os.path.isfile('CONTRIBUTING.md'):
-        shutil.copyfile('CONTRIBUTING.md', 'docs/CONTRIBUTING.md')
-
-    bf.generate_doc(project, dataset)
 
-    for image in [f for f in os.listdir('bigfunctions') if f.endswith('.png')]:
-        shutil.copy(f'bigfunctions/{image}', f'docs/bigfunctions/{image}')
+    def init_docs_folder():
+        os.makedirs('docs', exist_ok=True)
+        shutil.rmtree('docs/bigfunctions', ignore_errors=True)
+        os.makedirs('docs/bigfunctions')
+
+    def copy_readme_and_contributing():
+        if not os.path.isfile('README.md'):
+            print('INFO: CREATING A README.md FILE IN CURRENT DIRECTORY WHICH WILL BE THE ROOT CONTENT OF THE WEBSITE')
+            open('README.md', 'w', encoding='utf-8').write('# Hello from README!')
+        shutil.copyfile('README.md', 'docs/README.md')
+        if os.path.isfile('CONTRIBUTING.md'):
+            shutil.copyfile('CONTRIBUTING.md', 'docs/CONTRIBUTING.md')
+
+    def copy_default_site_config():
+        if not os.path.isfile('mkdocs.yml'):
+            print('INFO: CREATING mkdocs.yml FILE in CURRENT DIRECTORY. It is the configuration file of the website...')
+            shutil.copyfile(WEBSITE_CONFIG_FOLDER + '/mkdocs.yml', 'mkdocs.yml')
+        if not os.path.isdir('docs/assets'):
+            print('INFO: COPYING assets FOLDER into docs FOLDER...')
+            shutil.copytree(WEBSITE_CONFIG_FOLDER + '/assets', 'docs/assets')
+        if not os.path.isdir('docs/theme_overrides'):
+            print('INFO: COPYING theme_overrides FOLDER into docs FOLDER...')
+            shutil.copytree(WEBSITE_CONFIG_FOLDER + '/theme_overrides', 'docs/theme_overrides')
+
+    def generate_bigfunctions_markdown(bigfunctions):
+        for bigfunction in bigfunctions:
+            open(f'docs/bigfunctions/{bigfunction.name}.md', 'w', encoding='utf-8').write(bigfunction.doc)
+
+    def copy_screenshots_to_docs_folder():
+        for image in [f for f in os.listdir('bigfunctions') if f.endswith('.png')]:
+            shutil.copy(f'bigfunctions/{image}', f'docs/bigfunctions/{image}')
+
+    def generate_bigfunctions_list_markdown(bigfunctions):
+        mkdocs_config = yaml.safe_load(open('mkdocs.yml', encoding='utf-8').read())
+        categories = mkdocs_config['bigfunctions_categories']
+        for category in categories:
+            category['bigfunctions'] = [b.config for b in bigfunctions if b.config['category'] == category['name']]
+        categories = [category for category in categories if category['bigfunctions']]
+        categories_template = jinja2.Template(open(CATEGORIES_DOC_TEMPLATE_FILENAME, encoding='utf-8').read())
+        categories_doc = categories_template.render(categories=categories, project=project, dataset=dataset)
+        open('bigfunctions/README.md', 'w', encoding='utf-8').write(categories_doc)
+        open('docs/bigfunctions/README.md', 'w', encoding='utf-8').write(categories_doc)
+
+    bigfunctions = [
+        bf.BigFunction(bigfunction_name, project=project, dataset=dataset)
+        for bigfunction_name in bf.list_bigfunctions()
+    ]
+    init_docs_folder()
+    copy_readme_and_contributing()
+    copy_default_site_config()
+    generate_bigfunctions_markdown(bigfunctions)
+    copy_screenshots_to_docs_folder()
+    generate_bigfunctions_list_markdown(bigfunctions)
 
 
 @click.group(
     cls=HelpColorsGroup,
     help_headers_color='yellow',
     help_options_color='cyan'
 )
@@ -121,15 +150,15 @@
 
     for name in bigfunctions:
         bigfunction = bf.BigFunction(name, project=project, dataset=datasets[0])
         bigfunction.deploy()
         if len(datasets) > 1:
             with multiprocessing.Pool(processes=8) as pool:
                 pool.map(
-                    BigFunction.deploy,
+                    bf.BigFunction.deploy,
                     [
                         bf.BigFunction(name, project=project, dataset=dataset)
                         for dataset in datasets[1:]
                     ]
                 )
```

### Comparing `bigfunctions-0.4/bigfun/load_table.py` & `bigfunctions-0.5/bigfun/load_table.py`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.4/bigfun/templates/Dockerfile` & `bigfunctions-0.5/bigfun/templates/Dockerfile`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.4/bigfun/templates/bigfunction.md` & `bigfunctions-0.5/bigfun/templates/bigfunction.md`

 * *Files 3% similar despite different names*

```diff
@@ -67,30 +67,46 @@
 
 {% for dataset in datasets[:nb_datasets] %}
 
 
 === "{% if dataset|length <=2 %}{{ dataset | upper | replace('_', '-') }}{% else %}{{ dataset | replace('_', '-') }}{% endif %}"
 
     ```sql
+    {% if example.with_clause is defined %}
+    with sample_data as (
+      {{ example.with_clause | indent(6) }}
+    )
+    {% endif %}
     {% if type == 'procedure' %}call{% elif type == 'table_function' %}select * from{% else %}select{% endif %} {{ project }}.{{ dataset }}.{{ name }}({% for argument in example.arguments %}{{ argument | replace('{BIGFUNCTIONS_DATASET}', dataset) | replace('\n', '\n      ') }}{% if not loop.last %}, {% endif %}{% endfor %}){% if type == 'procedure' %};{% elif 'output' in bigfunction and type != 'table_function' %} as {{ output.name }}{% endif %}
+    {%- if example.with_clause is defined %}
+    from sample_data
+    {% endif %}
     {% if type == 'procedure' and template %}select html from bigfunction_result;{% endif %}
     {%- if type == 'procedure' and example.output %}select * from bigfunction_result;{% endif %}
     ```
 
 {% endfor %}
 
 
 {% else %}
 
 {% for dataset in datasets %}
 
 ```sql
-{% if type == 'procedure' %}call{% elif type == 'table_function' %}select * from{% else %}select{% endif %} {{ project }}.{{ dataset }}.{{ name }}({% for argument in example.arguments %}{{ argument | replace('{BIGFUNCTIONS_DATASET}', dataset) | replace('\n', '\n  ') }}{% if not loop.last %}, {% endif %}{% endfor %}){% if type == 'procedure' %};{% elif 'output' in bigfunction and type != 'table_function' %} as {{ output.name }}{% endif %}
+{% if example.with_clause is defined %}
+with sample_data as (
+  {{ example.with_clause | indent(2) }}
+)
+{% endif %}{% if type == 'procedure' %}call{% elif type == 'table_function' %}select * from{% else %}select{% endif %} {{ project }}.{{ dataset }}.{{ name }}({% for argument in example.arguments %}{{ argument | replace('{BIGFUNCTIONS_DATASET}', dataset) | replace('\n', '\n  ') }}{% if not loop.last %}, {% endif %}{% endfor %}){% if type == 'procedure' %};{% elif 'output' in bigfunction and type != 'table_function' %} as {{ output.name }}{% endif %}
+{%- if example.with_clause is defined %}
+from sample_data
+{% endif %}
 {% if type == 'procedure' and template %}select html from bigfunction_result;{% endif %}
 {%- if type == 'procedure' and example.output %}select * from bigfunction_result;{% endif %}
+
 ```
 
 {% endfor %}
 
 {% endif %}
 
 
@@ -125,9 +141,7 @@
 </pre>
 
 {% endif %}
 
 
 {% if example.screenshot %}<a href="../{{ example.screenshot }}"><img alt="screenshot" src="../{{ example.screenshot }}" style="border: var(--md-code-bg-color) solid 1rem; margin-top: -1rem; width: 100%"></a>{% endif %}
 {% endfor %}
-
-
```

### Comparing `bigfunctions-0.4/bigfun/templates/bookmarklet.js` & `bigfunctions-0.5/bigfun/templates/bookmarklet.js`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.4/bigfun/templates/categories.md` & `bigfunctions-0.5/bigfun/templates/categories.md`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.4/bigfun/templates/data.md` & `bigfunctions-0.5/bigfun/templates/data.md`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.4/bigfun/templates/function_js.sql` & `bigfunctions-0.5/bigfun/templates/function_js.sql`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.4/bigfun/templates/function_py.py` & `bigfunctions-0.5/bigfun/templates/function_py.py`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.4/bigfun/templates/procedure.sql` & `bigfunctions-0.5/bigfun/templates/procedure.sql`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.4/bigfun/templates/procedure_test.sql` & `bigfunctions-0.5/bigfun/templates/procedure_test.sql`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.4/bigfun/utils.py` & `bigfunctions-0.5/bigfun/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,17 +133,17 @@
         dataset.users = [
             dataset_access_entry2user(access_entry)
             for access_entry in dataset.access_entries
             if access_entry.entity_id not in ['projectOwners', 'projectWriters', 'projectReaders']
         ]
         return dataset
 
-    def query(self, query):
+    def query(self, query, **kwargs):
         try:
-            return self.client.query(query).result()
+            return self.client.query(query, **kwargs).result()
         except google.api_core.exceptions.Forbidden as e:
             handle_error("Access Denied", e.message)
         except (
             google.api_core.exceptions.BadRequest,
             google.api_core.exceptions.NotFound,
         ) as e:
             handle_error(e.message, "Query:\n" + prefix_lines_with_line_number(query))
```

### Comparing `bigfunctions-0.4/bigfun/website/assets/GitHub-Mark-32px.png` & `bigfunctions-0.5/bigfun/website/assets/GitHub-Mark-32px.png`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.4/bigfun/website/assets/bookmarklet_usage.gif` & `bigfunctions-0.5/bigfun/website/assets/bookmarklet_usage.gif`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.4/bigfun/website/assets/logo.png` & `bigfunctions-0.5/bigfun/website/assets/logo.png`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.4/bigfun/website/assets/logo_and_name.png` & `bigfunctions-0.5/bigfun/website/assets/logo_and_name.png`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.4/bigfun/website/assets/logo_and_name_wo_supercharge.png` & `bigfunctions-0.5/bigfun/website/assets/logo_and_name_wo_supercharge.png`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.4/bigfun/website/theme_overrides/main.html` & `bigfunctions-0.5/bigfun/website/theme_overrides/main.html`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.4/bigfunctions.egg-info/PKG-INFO` & `bigfunctions-0.5/bigfunctions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: bigfunctions
-Version: 0.4
+Version: 0.5
 Summary: Supercharge BigQuery with BigFunctions
-Download-URL: https://github.com/unytics/bigfunctions/archive/refs/tags/v0.4.tar.gz
+Download-URL: https://github.com/unytics/bigfunctions/archive/refs/tags/v0.5.tar.gz
 Author: Unytics
 Author-email: paul.marcombes@unytics.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: bigfunctions Version: 0.4 Summary: Supercharge
+Metadata-Version: 2.1 Name: bigfunctions Version: 0.5 Summary: Supercharge
 BigQuery with BigFunctions Download-URL: https://github.com/unytics/
-bigfunctions/archive/refs/tags/v0.4.tar.gz Author: Unytics Author-email:
+bigfunctions/archive/refs/tags/v0.5.tar.gz Author: Unytics Author-email:
 paul.marcombes@unytics.io Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.10 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: google-cloud-bigquery Requires-
 Dist: google-cloud-bigquery_connection Requires-Dist: google-cloud-storage
 Requires-Dist: pyyaml Requires-Dist: jinja2 Requires-Dist: mkdocs-material
 Requires-Dist: click Requires-Dist: click-help-colors
```

### Comparing `bigfunctions-0.4/bigfunctions.egg-info/SOURCES.txt` & `bigfunctions-0.5/bigfunctions.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 bigfun/cli.py
 bigfun/load_table.py
 bigfun/utils.py
 bigfun/templates/Dockerfile
 bigfun/templates/bigfunction.md
 bigfun/templates/bookmarklet.js
 bigfun/templates/categories.md
-bigfun/templates/categories.yaml
 bigfun/templates/data.md
 bigfun/templates/function_js.sql
 bigfun/templates/function_py.py
 bigfun/templates/function_py.sql
 bigfun/templates/function_py_test.py
 bigfun/templates/function_sql.sql
 bigfun/templates/function_sql_test.sql
```

### Comparing `bigfunctions-0.4/setup.py` & `bigfunctions-0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-VERSION = '0.4'
+VERSION = '0.5'
 
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
```

