# Comparing `tmp/partenaire-qualif-0.2.0.tar.gz` & `tmp/partenaire-qualif-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "partenaire-qualif-0.2.0.tar", last modified: Mon May 13 15:47:27 2024, max compression
+gzip compressed data, was "partenaire-qualif-0.2.1.tar", last modified: Mon May 13 15:49:47 2024, max compression
```

## Comparing `partenaire-qualif-0.2.0.tar` & `partenaire-qualif-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 15:47:27.966069 partenaire-qualif-0.2.0/
--rw-rw-rw-   0        0        0     1087 2024-05-09 03:19:27.000000 partenaire-qualif-0.2.0/LICENSE
--rw-rw-rw-   0        0        0       30 2024-05-13 15:42:14.000000 partenaire-qualif-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3112 2024-05-13 15:47:27.966069 partenaire-qualif-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2589 2024-05-10 17:50:16.000000 partenaire-qualif-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 15:47:27.950519 partenaire-qualif-0.2.0/partenaire_qualif.egg-info/
--rw-rw-rw-   0        0        0     3112 2024-05-13 15:47:27.000000 partenaire-qualif-0.2.0/partenaire_qualif.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      408 2024-05-13 15:47:27.000000 partenaire-qualif-0.2.0/partenaire_qualif.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 15:47:27.000000 partenaire-qualif-0.2.0/partenaire_qualif.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-05-13 15:47:27.000000 partenaire-qualif-0.2.0/partenaire_qualif.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-13 15:47:27.000000 partenaire-qualif-0.2.0/partenaire_qualif.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 15:47:27.966069 partenaire-qualif-0.2.0/qualif/
--rw-rw-rw-   0        0        0       76 2024-05-10 17:15:12.000000 partenaire-qualif-0.2.0/qualif/__init__.py
--rw-rw-rw-   0        0        0     9667 2024-05-10 17:13:51.000000 partenaire-qualif-0.2.0/qualif/qualif.py
-drwxrwxrwx   0        0        0        0 2024-05-13 15:47:27.966069 partenaire-qualif-0.2.0/qualif/templates/
--rw-rw-rw-   0        0        0        0 2024-05-13 15:47:06.000000 partenaire-qualif-0.2.0/qualif/templates/__init__.py
--rw-rw-rw-   0        0        0     2426 2024-05-10 17:08:42.000000 partenaire-qualif-0.2.0/qualif/templates/prompt_find_website_template.txt
--rw-rw-rw-   0        0        0     1987 2024-05-10 17:12:26.000000 partenaire-qualif-0.2.0/qualif/templates/prompt_qualification_template.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 15:47:27.966069 partenaire-qualif-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      979 2024-05-13 15:47:27.000000 partenaire-qualif-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:49:47.388191 partenaire-qualif-0.2.1/
+-rw-rw-rw-   0        0        0     1087 2024-05-09 03:19:27.000000 partenaire-qualif-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0       30 2024-05-13 15:42:14.000000 partenaire-qualif-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3167 2024-05-13 15:49:47.388191 partenaire-qualif-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2644 2024-05-13 15:49:03.000000 partenaire-qualif-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 15:49:47.388191 partenaire-qualif-0.2.1/partenaire_qualif.egg-info/
+-rw-rw-rw-   0        0        0     3167 2024-05-13 15:49:47.000000 partenaire-qualif-0.2.1/partenaire_qualif.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      408 2024-05-13 15:49:47.000000 partenaire-qualif-0.2.1/partenaire_qualif.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 15:49:47.000000 partenaire-qualif-0.2.1/partenaire_qualif.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-05-13 15:49:47.000000 partenaire-qualif-0.2.1/partenaire_qualif.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-13 15:49:47.000000 partenaire-qualif-0.2.1/partenaire_qualif.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 15:49:47.388191 partenaire-qualif-0.2.1/qualif/
+-rw-rw-rw-   0        0        0       76 2024-05-10 17:15:12.000000 partenaire-qualif-0.2.1/qualif/__init__.py
+-rw-rw-rw-   0        0        0     9667 2024-05-10 17:13:51.000000 partenaire-qualif-0.2.1/qualif/qualif.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:49:47.388191 partenaire-qualif-0.2.1/qualif/templates/
+-rw-rw-rw-   0        0        0        0 2024-05-13 15:47:06.000000 partenaire-qualif-0.2.1/qualif/templates/__init__.py
+-rw-rw-rw-   0        0        0     2426 2024-05-10 17:08:42.000000 partenaire-qualif-0.2.1/qualif/templates/prompt_find_website_template.txt
+-rw-rw-rw-   0        0        0     1987 2024-05-10 17:12:26.000000 partenaire-qualif-0.2.1/qualif/templates/prompt_qualification_template.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 15:49:47.388191 partenaire-qualif-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      979 2024-05-13 15:49:46.000000 partenaire-qualif-0.2.1/setup.py
```

### Comparing `partenaire-qualif-0.2.0/LICENSE` & `partenaire-qualif-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `partenaire-qualif-0.2.0/PKG-INFO` & `partenaire-qualif-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: partenaire-qualif
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple tool that automates the qualification of a partner(reseller/integrator/editor) by finding its website, industries, business functions and services.
 Home-page: https://github.com/ymurong/partenaire_qualif.git
 Author: Yanchao MURONG
 Author-email: yanchao.murong@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -20,15 +20,15 @@
 
 An example of qualification result:
 
 * (industry column) Target your industry
 * (job column) The jobs that can be targeted through their industry
 * (offers column) The services they offer.
 
-![alt text](samples/qualification_results_example.png)
+![alt text](https://github.com/ymurong/partenaire_qualif/blob/main/samples/qualification_results_example.png)
 
 # Install
 
 ```bash
 pip install partenaire-qualif
 ```
```

### Comparing `partenaire-qualif-0.2.0/README.md` & `partenaire-qualif-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 An example of qualification result:
 
 * (industry column) Target your industry
 * (job column) The jobs that can be targeted through their industry
 * (offers column) The services they offer.
 
-![alt text](samples/qualification_results_example.png)
+![alt text](https://github.com/ymurong/partenaire_qualif/blob/main/samples/qualification_results_example.png)
 
 # Install
 
 ```bash
 pip install partenaire-qualif
 ```
```

### Comparing `partenaire-qualif-0.2.0/partenaire_qualif.egg-info/PKG-INFO` & `partenaire-qualif-0.2.1/partenaire_qualif.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: partenaire-qualif
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple tool that automates the qualification of a partner(reseller/integrator/editor) by finding its website, industries, business functions and services.
 Home-page: https://github.com/ymurong/partenaire_qualif.git
 Author: Yanchao MURONG
 Author-email: yanchao.murong@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -20,15 +20,15 @@
 
 An example of qualification result:
 
 * (industry column) Target your industry
 * (job column) The jobs that can be targeted through their industry
 * (offers column) The services they offer.
 
-![alt text](samples/qualification_results_example.png)
+![alt text](https://github.com/ymurong/partenaire_qualif/blob/main/samples/qualification_results_example.png)
 
 # Install
 
 ```bash
 pip install partenaire-qualif
 ```
```

### Comparing `partenaire-qualif-0.2.0/qualif/qualif.py` & `partenaire-qualif-0.2.1/qualif/qualif.py`

 * *Files identical despite different names*

### Comparing `partenaire-qualif-0.2.0/qualif/templates/prompt_find_website_template.txt` & `partenaire-qualif-0.2.1/qualif/templates/prompt_find_website_template.txt`

 * *Files identical despite different names*

### Comparing `partenaire-qualif-0.2.0/qualif/templates/prompt_qualification_template.txt` & `partenaire-qualif-0.2.1/qualif/templates/prompt_qualification_template.txt`

 * *Files identical despite different names*

### Comparing `partenaire-qualif-0.2.0/setup.py` & `partenaire-qualif-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="partenaire-qualif",
-    version='0.2.0',
+    version='0.2.1',
     author="Yanchao MURONG",
     author_email="yanchao.murong@gmail.com",
     description="A simple tool that automates the qualification of a partner(reseller/integrator/editor) by finding its website, industries, business functions and services.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ymurong/partenaire_qualif.git",
     packages=setuptools.find_packages(),
```

