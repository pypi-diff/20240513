# Comparing `tmp/simplevc-0.0.2.tar.gz` & `tmp/simplevc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplevc-0.0.2.tar", last modified: Tue Apr 30 02:35:32 2024, max compression
+gzip compressed data, was "simplevc-0.0.3.tar", last modified: Mon May 13 02:49:17 2024, max compression
```

## Comparing `simplevc-0.0.2.tar` & `simplevc-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-04-30 02:35:32.024893 simplevc-0.0.2/
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)     5744 2024-04-30 02:35:32.024893 simplevc-0.0.2/PKG-INFO
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)     5268 2024-04-30 02:34:53.000000 simplevc-0.0.2/README.md
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)       38 2024-04-30 02:35:32.024893 simplevc-0.0.2/setup.cfg
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)      700 2024-04-30 02:33:21.000000 simplevc-0.0.2/setup.py
-drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-04-30 02:35:32.022893 simplevc-0.0.2/simplevc/
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)       23 2024-04-30 02:11:58.000000 simplevc-0.0.2/simplevc/__init__.py
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)    15327 2024-04-30 02:24:11.000000 simplevc-0.0.2/simplevc/simplevc.py
-drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-04-30 02:35:32.022893 simplevc-0.0.2/simplevc.egg-info/
--rw-r--r--   0 kl945     (5298) hy299_0001 (80905)     5744 2024-04-30 02:35:31.000000 simplevc-0.0.2/simplevc.egg-info/PKG-INFO
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)      188 2024-04-30 02:35:31.000000 simplevc-0.0.2/simplevc.egg-info/SOURCES.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)        1 2024-04-30 02:35:31.000000 simplevc-0.0.2/simplevc.egg-info/dependency_links.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)        9 2024-04-30 02:35:31.000000 simplevc-0.0.2/simplevc.egg-info/top_level.txt
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-05-13 02:49:17.493511 simplevc-0.0.3/
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)     5644 2024-05-13 02:49:17.493511 simplevc-0.0.3/PKG-INFO
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)     5268 2024-04-30 02:34:53.000000 simplevc-0.0.3/README.md
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)       38 2024-05-13 02:49:17.494511 simplevc-0.0.3/setup.cfg
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)      614 2024-05-08 12:24:16.000000 simplevc-0.0.3/setup.py
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-05-13 02:49:17.492511 simplevc-0.0.3/simplevc/
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)       23 2024-04-30 02:11:58.000000 simplevc-0.0.3/simplevc/__init__.py
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)    15638 2024-05-08 04:31:39.000000 simplevc-0.0.3/simplevc/simplevc.py
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-05-13 02:49:17.493511 simplevc-0.0.3/simplevc.egg-info/
+-rw-r--r--   0 kl945     (5298) hy299_0001 (80905)     5644 2024-05-13 02:49:11.000000 simplevc-0.0.3/simplevc.egg-info/PKG-INFO
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)      188 2024-05-13 02:49:11.000000 simplevc-0.0.3/simplevc.egg-info/SOURCES.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)        1 2024-05-13 02:49:11.000000 simplevc-0.0.3/simplevc.egg-info/dependency_links.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)        9 2024-05-13 02:49:11.000000 simplevc-0.0.3/simplevc.egg-info/top_level.txt
```

### Comparing `simplevc-0.0.2/PKG-INFO` & `simplevc-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: simplevc
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple Python version control package
 Home-page: https://github.com/aldenleung/simplevc/
 Author: Alden Leung
 Author-email: alden.leung@gmail.com
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 
 # simplevc - A simple Python version control package
```

### Comparing `simplevc-0.0.2/README.md` & `simplevc-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `simplevc-0.0.2/setup.py` & `simplevc-0.0.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,23 +3,21 @@
 with open("README.md", "r") as readme_file:
 	readme = readme_file.read()
 
 requirements = []
 
 setup(
 	name="simplevc",
-	version="0.0.2",
+	version="0.0.3",
 	author="Alden Leung",
 	author_email="alden.leung@gmail.com",
 	description="A simple Python version control package",
 	long_description=readme,
 	long_description_content_type="text/markdown",
 	url="https://github.com/aldenleung/simplevc/",
 	packages=find_packages(),
 	install_requires=requirements,
 	classifiers=[
-		"Programming Language :: Python :: 3.7",
-		"Programming Language :: Python :: 3.8",
 		"Programming Language :: Python :: 3.9",
 		"License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 	],
 )
```

### Comparing `simplevc-0.0.2/simplevc/simplevc.py` & `simplevc-0.0.3/simplevc/simplevc.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,15 +282,16 @@
 
 def module_main(module):
 	'''
 	The default routine for main
 	'''
 	import argparse
 	import sys
-	
+	from types import GenericAlias
+	import typing
 	display_help = False
 	i = 1
 	while i < len(sys.argv):
 		if sys.argv[i] == "-v":
 			module.set_version(sys.argv[i + 1])
 			i += 2
 		elif sys.argv[i] == "-h":
@@ -318,29 +319,36 @@
 		for param in signature.parameters.values():
 			import inspect
 			kwargs = {}
 			if param.name in helps:
 				kwargs["help"] = helps[param.name]
 			else:
 				kwargs["help"] = "_"
-				
-			if param.name in types:
-				kwargs["type"] = types[param.name]
-			elif param.annotation != inspect._empty:
-				kwargs["type"] = param.annotation
-				
+
 			if param.name in defaults:
 				kwargs["default"] = defaults[param.name] 
 				kwargs["required"] = False
 			elif param.default != inspect._empty:
 				kwargs["default"] = param.default 
 				kwargs["required"] = False
 			else:
 				kwargs["required"] = True
 				
+			if param.name in types:
+				kwargs["type"] = types[param.name]
+			elif param.annotation != inspect._empty:
+				if isinstance(param.annotation, GenericAlias):
+					if typing.get_origin(param.annotation) != list:
+						raise Exception("Only list is supported in GenericAlias")
+					kwargs["type"] = typing.get_args(param.annotation)[0]
+					kwargs["nargs"] = "*"
+				else:
+					kwargs["type"] = param.annotation
+				
+				
 			parser.add_argument(f"-{param.name}", **kwargs)
 		
 		if return_routine is not None:
 			return_params = return_routine[1]
 			_return_routines[func_name] = return_routine
 			for param_name in return_params:
 				kwargs = {}
```

### Comparing `simplevc-0.0.2/simplevc.egg-info/PKG-INFO` & `simplevc-0.0.3/simplevc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: simplevc
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple Python version control package
 Home-page: https://github.com/aldenleung/simplevc/
 Author: Alden Leung
 Author-email: alden.leung@gmail.com
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 
 # simplevc - A simple Python version control package
```

