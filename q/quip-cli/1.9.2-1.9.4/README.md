# Comparing `tmp/quip-cli-1.9.2.tar.gz` & `tmp/quip-cli-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quip-cli-1.9.2.tar", last modified: Thu Apr 18 17:29:18 2024, max compression
+gzip compressed data, was "quip-cli-1.9.4.tar", last modified: Mon May 13 18:57:43 2024, max compression
```

## Comparing `quip-cli-1.9.2.tar` & `quip-cli-1.9.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-18 17:29:18.822640 quip-cli-1.9.2/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    29453 2024-04-18 17:29:18.822402 quip-cli-1.9.2/PKG-INFO
--rwxrw-r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    29053 2024-04-16 13:47:26.000000 quip-cli-1.9.2/README.md
--rwxrw-r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       89 2023-02-23 14:36:14.000000 quip-cli-1.9.2/pyproject.toml
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-18 17:29:18.819697 quip-cli-1.9.2/quip/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2277 2024-04-18 17:29:08.000000 quip-cli-1.9.2/quip/__init__.py
--rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    20123 2023-04-14 18:15:41.000000 quip-cli-1.9.2/quip/external.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5307 2023-08-21 16:56:55.000000 quip-cli-1.9.2/quip/fact.py
--rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    25603 2024-04-18 17:15:32.000000 quip-cli-1.9.2/quip/field_builder.py
--rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    74410 2024-04-16 14:28:06.000000 quip-cli-1.9.2/quip/quip.py
--rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     7104 2022-12-05 17:10:38.000000 quip-cli-1.9.2/quip/version_builder.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-18 17:29:18.822041 quip-cli-1.9.2/quip_cli.egg-info/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    29453 2024-04-18 17:29:18.000000 quip-cli-1.9.2/quip_cli.egg-info/PKG-INFO
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      333 2024-04-18 17:29:18.000000 quip-cli-1.9.2/quip_cli.egg-info/SOURCES.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2024-04-18 17:29:18.000000 quip-cli-1.9.2/quip_cli.egg-info/dependency_links.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       39 2024-04-18 17:29:18.000000 quip-cli-1.9.2/quip_cli.egg-info/entry_points.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      101 2024-04-18 17:29:18.000000 quip-cli-1.9.2/quip_cli.egg-info/requires.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        5 2024-04-18 17:29:18.000000 quip-cli-1.9.2/quip_cli.egg-info/top_level.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2024-04-18 17:29:18.822687 quip-cli-1.9.2/setup.cfg
--rwxrw-r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1281 2022-10-06 20:00:12.000000 quip-cli-1.9.2/setup.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-13 18:57:43.831951 quip-cli-1.9.4/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    29453 2024-05-13 18:57:43.831745 quip-cli-1.9.4/PKG-INFO
+-rwxrw-r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    29053 2024-04-16 13:47:26.000000 quip-cli-1.9.4/README.md
+-rwxrw-r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       89 2023-02-23 14:36:14.000000 quip-cli-1.9.4/pyproject.toml
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-13 18:57:43.828955 quip-cli-1.9.4/quip/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2277 2024-04-23 04:31:48.000000 quip-cli-1.9.4/quip/__init__.py
+-rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    20123 2023-04-14 18:15:41.000000 quip-cli-1.9.4/quip/external.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5307 2023-08-21 16:56:55.000000 quip-cli-1.9.4/quip/fact.py
+-rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    25604 2024-04-23 04:35:24.000000 quip-cli-1.9.4/quip/field_builder.py
+-rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    74868 2024-04-23 04:31:03.000000 quip-cli-1.9.4/quip/quip.py
+-rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     7104 2022-12-05 17:10:38.000000 quip-cli-1.9.4/quip/version_builder.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-13 18:57:43.831369 quip-cli-1.9.4/quip_cli.egg-info/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    29453 2024-05-13 18:57:43.000000 quip-cli-1.9.4/quip_cli.egg-info/PKG-INFO
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      333 2024-05-13 18:57:43.000000 quip-cli-1.9.4/quip_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2024-05-13 18:57:43.000000 quip-cli-1.9.4/quip_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       39 2024-05-13 18:57:43.000000 quip-cli-1.9.4/quip_cli.egg-info/entry_points.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      101 2024-05-13 18:57:43.000000 quip-cli-1.9.4/quip_cli.egg-info/requires.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        5 2024-05-13 18:57:43.000000 quip-cli-1.9.4/quip_cli.egg-info/top_level.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2024-05-13 18:57:43.831992 quip-cli-1.9.4/setup.cfg
+-rwxrw-r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1281 2022-10-06 20:00:12.000000 quip-cli-1.9.4/setup.py
```

### Comparing `quip-cli-1.9.2/PKG-INFO` & `quip-cli-1.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quip-cli
-Version: 1.9.2
+Version: 1.9.4
 Summary: Tool for creating/updating new universal integrations
 Author: Stonebranch
 Author-email: huseyin.gomleksizoglu@stonebranch.com
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `quip-cli-1.9.2/README.md` & `quip-cli-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `quip-cli-1.9.2/quip/__init__.py` & `quip-cli-1.9.4/quip/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from colorama import Fore, Style, init
 
 init()
 
-__version__ = "1.9.2"
+__version__ = "1.9.4"
 
 def cprint(text, color, end='\n', style='Normal'):
     if len(str(text).strip()) == 0: return
     fore = getattr(Fore, color.upper())
     style = getattr(Style, style.upper())
     print('{0}{1}{2}{3}'.format(fore, style, text, Style.RESET_ALL), end=end)
```

### Comparing `quip-cli-1.9.2/quip/external.py` & `quip-cli-1.9.4/quip/external.py`

 * *Files identical despite different names*

### Comparing `quip-cli-1.9.2/quip/fact.py` & `quip-cli-1.9.4/quip/fact.py`

 * *Files identical despite different names*

### Comparing `quip-cli-1.9.2/quip/field_builder.py` & `quip-cli-1.9.4/quip/field_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -501,15 +501,15 @@
         print("""    return ExtensionResult(
     rc = 0,
     message = "Available Fields: '{}'".format(_fields),
     values = _fields
     )""")
     
     if code_type == "choice":
-        print(f"\nclass {name.capitalize()}(Enum)")
+        print(f"\nclass {name.capitalize()}(Enum):")
         if items is not None:
             for item in items:
                 if isinstance(item, dict):
                     print(f"    {list(item.keys())[0].upper()} = \"{list(item.keys())[0]}\"")
                 else:
                     print(f"    {item.upper()} = \"{item}\"")
```

### Comparing `quip-cli-1.9.2/quip/quip.py` & `quip-cli-1.9.4/quip/quip.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,28 +82,32 @@
         parser_fields.add_argument('name', nargs="?", help='name of the project')
         parser_fields.add_argument('--update', '-u', action='store_true',
                              help='Update fields from fields.yml')
         parser_fields.add_argument('--dump', '-d', action='store_true',
                              help='dump fields to fields.yml')
         parser_fields.add_argument('--code', action='store_true',
                             help='Give some code samples')
+        parser_fields.add_argument('--common', action='store_true',
+                            help='Give some code samples in ue-common format')
 
         parser_delete = subparsers.add_parser('delete', aliases=DELETE_ACTION[1:], help='Deletes the integration folder')
         parser_delete.add_argument('name', help='name of the project')
 
         parser_clone = subparsers.add_parser('clone', aliases=CLONE_ACTION[1:], help='Clones existing integration with a new name')
         parser_clone.add_argument('name', help='name of the project')
         parser_clone.add_argument('source', help='source project path')
         parser_clone.add_argument('--template', '-t', action='store_true',
                              help='create template instead of extension')
 
         parser_bootstrap = subparsers.add_parser('bootstrap', aliases=BOOTSTRAP_ACTION[1:], help='Bootstrap new integration from baseline project')
         parser_bootstrap.add_argument('name', nargs="?", help='name of the project')
         parser_bootstrap.add_argument('--template', '-t', action='store_true',
                              help='create template instead of extension')
+        parser_bootstrap.add_argument('--baseline', '-b',
+                             help='Path of the baseline project')
 
         parser_upload = subparsers.add_parser('upload', aliases=UPLOAD_ACTION[1:], help='Uploads the template to Universal Controller. (Template Only)')
         parser_upload.add_argument('name', nargs="?", help='name of the project')
         parser_upload.add_argument('--template', '-t', action='store_true',
                              help='create template instead of extension')
 
         parser_download = subparsers.add_parser('download', aliases=DOWNLOAD_ACTION[1:], help='Download the template from Universal Controller.')
@@ -205,14 +209,16 @@
                 self.create_icon()
             else:
                 self.update_icon()
         elif action in FIELD_ACTION:
             if self.args.dump:
                 self.dump_fields(write=True)
             else:
+                if self.args.common:
+                    self.code_type = "common"
                 self.update_fields(self.args.code)
         elif action in UPDATE_ACTION:
             if self.args.rename_scripts:
                 self.update_rename_scripts()
             else:
                 self.update_project(self.args.uuid, self.args.new_uuid, new_project=False)
             self.dump_fields(write=True)
@@ -564,15 +570,18 @@
                     shutil.copy2(source_file_path, self.join_path(source_file))
                     logging.info(f"Copying file {source_file}")
         
         self.update_project(update_uuid=True, update_new_uuid=True, new_project=True)
 
     def bootstrap_project(self):
         # get bootstrap source
-        from_project_path = self._global_conf_defaults.get("bootstrap", {}).get("source", None)
+        if self.args.baseline:
+            from_project_path = self.args.baseline
+        else:    
+            from_project_path = self._global_conf_defaults.get("bootstrap", {}).get("source", None)
         if from_project_path is None:
             logging.error("Bootstrap source not found. Please check the config file.")
             sys.exit(2)
         
         exclude_list = self._global_conf_defaults.get("bootstrap", {}).get("exclude", None)
         
         self.clone_project(from_project_path, all_files=True, exclude_list=exclude_list)
```

### Comparing `quip-cli-1.9.2/quip/version_builder.py` & `quip-cli-1.9.4/quip/version_builder.py`

 * *Files identical despite different names*

### Comparing `quip-cli-1.9.2/quip_cli.egg-info/PKG-INFO` & `quip-cli-1.9.4/quip_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quip-cli
-Version: 1.9.2
+Version: 1.9.4
 Summary: Tool for creating/updating new universal integrations
 Author: Stonebranch
 Author-email: huseyin.gomleksizoglu@stonebranch.com
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `quip-cli-1.9.2/setup.py` & `quip-cli-1.9.4/setup.py`

 * *Files identical despite different names*

