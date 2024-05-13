# Comparing `tmp/code_to_gpt-0.3.tar.gz` & `tmp/code_to_gpt-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_to_gpt-0.3.tar", last modified: Mon May 13 19:58:42 2024, max compression
+gzip compressed data, was "code_to_gpt-0.4.tar", last modified: Mon May 13 20:00:28 2024, max compression
```

## Comparing `code_to_gpt-0.3.tar` & `code_to_gpt-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 PIL        (504) staff       (20)        0 2024-05-13 19:58:42.173672 code_to_gpt-0.3/
--rw-r--r--   0 PIL        (504) staff       (20)     1070 2024-05-13 19:15:09.000000 code_to_gpt-0.3/LICENSE
--rw-r--r--   0 PIL        (504) staff       (20)     2759 2024-05-13 19:58:42.173429 code_to_gpt-0.3/PKG-INFO
--rw-r--r--   0 PIL        (504) staff       (20)     2288 2024-05-13 19:25:30.000000 code_to_gpt-0.3/README.md
-drwxr-xr-x   0 PIL        (504) staff       (20)        0 2024-05-13 19:58:42.173182 code_to_gpt-0.3/code_to_gpt.egg-info/
--rw-r--r--   0 PIL        (504) staff       (20)     2759 2024-05-13 19:58:42.000000 code_to_gpt-0.3/code_to_gpt.egg-info/PKG-INFO
--rw-r--r--   0 PIL        (504) staff       (20)      248 2024-05-13 19:58:42.000000 code_to_gpt-0.3/code_to_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 PIL        (504) staff       (20)        1 2024-05-13 19:58:42.000000 code_to_gpt-0.3/code_to_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 PIL        (504) staff       (20)       54 2024-05-13 19:58:42.000000 code_to_gpt-0.3/code_to_gpt.egg-info/entry_points.txt
--rw-r--r--   0 PIL        (504) staff       (20)       10 2024-05-13 19:58:42.000000 code_to_gpt-0.3/code_to_gpt.egg-info/top_level.txt
-drwxr-xr-x   0 PIL        (504) staff       (20)        0 2024-05-13 19:58:42.172745 code_to_gpt-0.3/codetogpt/
--rw-r--r--   0 PIL        (504) staff       (20)        0 2024-05-13 17:58:04.000000 code_to_gpt-0.3/codetogpt/__init__.py
--rw-r--r--   0 PIL        (504) staff       (20)     1934 2024-05-13 19:07:17.000000 code_to_gpt-0.3/codetogpt/packager.py
--rw-r--r--   0 PIL        (504) staff       (20)       38 2024-05-13 19:58:42.173721 code_to_gpt-0.3/setup.cfg
--rw-r--r--   0 PIL        (504) staff       (20)      938 2024-05-13 19:58:28.000000 code_to_gpt-0.3/setup.py
+drwxr-xr-x   0 PIL        (504) staff       (20)        0 2024-05-13 20:00:28.140845 code_to_gpt-0.4/
+-rw-r--r--   0 PIL        (504) staff       (20)     1070 2024-05-13 19:15:09.000000 code_to_gpt-0.4/LICENSE
+-rw-r--r--   0 PIL        (504) staff       (20)     2697 2024-05-13 20:00:28.140621 code_to_gpt-0.4/PKG-INFO
+-rw-r--r--   0 PIL        (504) staff       (20)     2226 2024-05-13 20:00:21.000000 code_to_gpt-0.4/README.md
+drwxr-xr-x   0 PIL        (504) staff       (20)        0 2024-05-13 20:00:28.140364 code_to_gpt-0.4/code_to_gpt.egg-info/
+-rw-r--r--   0 PIL        (504) staff       (20)     2697 2024-05-13 20:00:28.000000 code_to_gpt-0.4/code_to_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 PIL        (504) staff       (20)      248 2024-05-13 20:00:28.000000 code_to_gpt-0.4/code_to_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 PIL        (504) staff       (20)        1 2024-05-13 20:00:28.000000 code_to_gpt-0.4/code_to_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 PIL        (504) staff       (20)       54 2024-05-13 20:00:28.000000 code_to_gpt-0.4/code_to_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 PIL        (504) staff       (20)       10 2024-05-13 20:00:28.000000 code_to_gpt-0.4/code_to_gpt.egg-info/top_level.txt
+drwxr-xr-x   0 PIL        (504) staff       (20)        0 2024-05-13 20:00:28.139789 code_to_gpt-0.4/codetogpt/
+-rw-r--r--   0 PIL        (504) staff       (20)        0 2024-05-13 17:58:04.000000 code_to_gpt-0.4/codetogpt/__init__.py
+-rw-r--r--   0 PIL        (504) staff       (20)     1934 2024-05-13 19:07:17.000000 code_to_gpt-0.4/codetogpt/packager.py
+-rw-r--r--   0 PIL        (504) staff       (20)       38 2024-05-13 20:00:28.140897 code_to_gpt-0.4/setup.cfg
+-rw-r--r--   0 PIL        (504) staff       (20)      938 2024-05-13 19:59:57.000000 code_to_gpt-0.4/setup.py
```

### Comparing `code_to_gpt-0.3/LICENSE` & `code_to_gpt-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `code_to_gpt-0.3/PKG-INFO` & `code_to_gpt-0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code-to-gpt
-Version: 0.3
+Version: 0.4
 Summary: A simple tool to concatenate code files for ChatGPT prompts
 Home-page: https://github.com/yourusername/codepackager
 Author: Sameel Shahid
 Author-email: sameelshahid@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,17 +29,15 @@
 Before you start using **CodeToGPT**, make sure you have Python 3.6 or higher installed on your machine.
 
 ### Installation
 
 To install **CodeToGPT**, follow these steps:
 
 ```bash
-git clone https://github.com/sameelshahid/CodeToGPT.git
-cd codetogpt
-pip install -e .
+pip install code-to-gpt
 ```
 
 
 ## Usage
 
 To run **CodeToGPT**, navigate to your project directory and execute:
```

### Comparing `code_to_gpt-0.3/README.md` & `code_to_gpt-0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,15 @@
 Before you start using **CodeToGPT**, make sure you have Python 3.6 or higher installed on your machine.
 
 ### Installation
 
 To install **CodeToGPT**, follow these steps:
 
 ```bash
-git clone https://github.com/sameelshahid/CodeToGPT.git
-cd codetogpt
-pip install -e .
+pip install code-to-gpt
 ```
 
 
 ## Usage
 
 To run **CodeToGPT**, navigate to your project directory and execute:
```

### Comparing `code_to_gpt-0.3/code_to_gpt.egg-info/PKG-INFO` & `code_to_gpt-0.4/code_to_gpt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code-to-gpt
-Version: 0.3
+Version: 0.4
 Summary: A simple tool to concatenate code files for ChatGPT prompts
 Home-page: https://github.com/yourusername/codepackager
 Author: Sameel Shahid
 Author-email: sameelshahid@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,17 +29,15 @@
 Before you start using **CodeToGPT**, make sure you have Python 3.6 or higher installed on your machine.
 
 ### Installation
 
 To install **CodeToGPT**, follow these steps:
 
 ```bash
-git clone https://github.com/sameelshahid/CodeToGPT.git
-cd codetogpt
-pip install -e .
+pip install code-to-gpt
 ```
 
 
 ## Usage
 
 To run **CodeToGPT**, navigate to your project directory and execute:
```

### Comparing `code_to_gpt-0.3/codetogpt/packager.py` & `code_to_gpt-0.4/codetogpt/packager.py`

 * *Files identical despite different names*

### Comparing `code_to_gpt-0.3/setup.py` & `code_to_gpt-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Read the contents of your README file
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='code-to-gpt',
-    version='0.3',
+    version='0.4',
     packages=find_packages(),
     description='A simple tool to concatenate code files for ChatGPT prompts',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Sameel Shahid',
     author_email='sameelshahid@hotmail.com',
     url='https://github.com/yourusername/codepackager',
```

