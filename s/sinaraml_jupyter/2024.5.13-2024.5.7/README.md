# Comparing `tmp/sinaraml_jupyter-2024.5.13.tar.gz` & `tmp/sinaraml_jupyter-2024.5.7.tar.gz`

## Comparing `sinaraml_jupyter-2024.5.13.tar` & `sinaraml_jupyter-2024.5.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.5.13/sinaraml_jupyter/__init__.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.5.13/sinaraml_jupyter/_version.py
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.5.13/sinaraml_jupyter/org_manager.py
--rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.5.13/sinaraml_jupyter/sinaraml_jupyter.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.5.13/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.5.13/LICENSE
--rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.5.13/README.md
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.5.13/pyproject.toml
--rw-r--r--   0        0        0     5977 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.5.13/PKG-INFO
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.5.7/sinaraml_jupyter/__init__.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.5.7/sinaraml_jupyter/_version.py
+-rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.5.7/sinaraml_jupyter/org_manager.py
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.5.7/sinaraml_jupyter/sinaraml_jupyter.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.5.7/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.5.7/LICENSE
+-rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.5.7/README.md
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.5.7/pyproject.toml
+-rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.5.7/PKG-INFO
```

### Comparing `sinaraml_jupyter-2024.5.13/sinaraml_jupyter/org_manager.py` & `sinaraml_jupyter-2024.5.7/sinaraml_jupyter/org_manager.py`

 * *Files identical despite different names*

### Comparing `sinaraml_jupyter-2024.5.13/sinaraml_jupyter/sinaraml_jupyter.py` & `sinaraml_jupyter-2024.5.7/sinaraml_jupyter/sinaraml_jupyter.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 
 def check_any_org_exists():
     if not SinaraOrgManager.check_last_update():
         jupyter_cli_org = "https://github.com/4-DS/mlops_jupyter_organization.git"
         if os.environ.get('SINARA_ORG'):
             platform = os.environ.get('SINARA_PLATFORM')
             sinara_org = json.loads(os.environ.get('SINARA_ORG').replace("'", '"'))
-            platform_short = platform.split('_')[-1]
-            body = [body for body in sinara_org["cli_bodies"] if platform_short in body["platform_names"]]
+            body = [body for body in sinara_org["cli_bodies"] if platform in body["platform_names"]]
             if body and "mlops_jupyter_organization" in body[0].keys():
                 jupyter_cli_org = body[0]["mlops_jupyter_organization"]
+            
         args = Gitref(gitref = jupyter_cli_org)
         SinaraOrgManager.install_from_git(args)
 
 def init_cli(root_parser, subject_parser, platform=None):
     root_parser.subjects = []
 
     SinaraOrgManager.add_command_handlers(root_parser, subject_parser)
```

### Comparing `sinaraml_jupyter-2024.5.13/.gitignore` & `sinaraml_jupyter-2024.5.7/.gitignore`

 * *Files identical despite different names*

### Comparing `sinaraml_jupyter-2024.5.13/LICENSE` & `sinaraml_jupyter-2024.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sinaraml_jupyter-2024.5.13/README.md` & `sinaraml_jupyter-2024.5.7/README.md`

 * *Files identical despite different names*

### Comparing `sinaraml_jupyter-2024.5.13/pyproject.toml` & `sinaraml_jupyter-2024.5.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sinaraml_jupyter-2024.5.13/PKG-INFO` & `sinaraml_jupyter-2024.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sinaraml_jupyter
-Version: 2024.5.13
+Version: 2024.5.7
 Summary: SinaraML Jupyter CLI
 Project-URL: Homepage, https://github.com/4-DS/sinaraml_jupyter
 Author-email: sinaraml <sinaraml.official@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 SinaraML
```

