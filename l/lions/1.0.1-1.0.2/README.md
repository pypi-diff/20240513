# Comparing `tmp/lions-1.0.1.tar.gz` & `tmp/lions-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lions-1.0.1.tar", last modified: Mon May 13 13:04:52 2024, max compression
+gzip compressed data, was "lions-1.0.2.tar", last modified: Mon May 13 13:16:49 2024, max compression
```

## Comparing `lions-1.0.1.tar` & `lions-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:04:52.549715 lions-1.0.1/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1071 2024-04-30 12:52:47.000000 lions-1.0.1/LICENSE
--rw-r--r--   0 diogoferreira   (501) staff       (20)     8124 2024-05-13 13:04:52.549641 lions-1.0.1/PKG-INFO
--rw-r--r--   0 diogoferreira   (501) staff       (20)     7271 2024-05-10 14:36:28.000000 lions-1.0.1/README.md
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:04:52.545365 lions-1.0.1/lions/
--rw-r--r--   0 diogoferreira   (501) staff       (20)       23 2024-05-13 08:58:00.000000 lions-1.0.1/lions/__init__.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:04:52.546633 lions-1.0.1/lions/cpp_gen/
--rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-07 11:54:56.000000 lions-1.0.1/lions/cpp_gen/__init__.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2602 2024-05-08 14:15:59.000000 lions-1.0.1/lions/cpp_gen/cpp_generator.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:04:52.547971 lions-1.0.1/lions/cpp_gen/templates/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1132 2024-05-07 12:48:43.000000 lions-1.0.1/lions/cpp_gen/templates/lions.cpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)      961 2024-05-10 09:27:52.000000 lions-1.0.1/lions/cpp_gen/templates/lions.hpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2203 2024-05-10 09:08:10.000000 lions-1.0.1/lions/cpp_gen/templates/msg.cpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1551 2024-05-10 13:07:27.000000 lions-1.0.1/lions/cpp_gen/templates/msg.hpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     3175 2024-05-10 09:08:10.000000 lions-1.0.1/lions/errors.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     5199 2024-05-08 16:10:12.000000 lions-1.0.1/lions/lmsg.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2444 2024-05-08 16:10:12.000000 lions-1.0.1/lions/main.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     6813 2024-05-10 09:08:10.000000 lions-1.0.1/lions/yaml_parser.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:04:52.546452 lions-1.0.1/lions.egg-info/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     8124 2024-05-13 13:04:52.000000 lions-1.0.1/lions.egg-info/PKG-INFO
--rw-r--r--   0 diogoferreira   (501) staff       (20)      593 2024-05-13 13:04:52.000000 lions-1.0.1/lions.egg-info/SOURCES.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)        1 2024-05-13 13:04:52.000000 lions-1.0.1/lions.egg-info/dependency_links.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       42 2024-05-13 13:04:52.000000 lions-1.0.1/lions.egg-info/entry_points.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       59 2024-05-13 13:04:52.000000 lions-1.0.1/lions.egg-info/requires.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       12 2024-05-13 13:04:52.000000 lions-1.0.1/lions.egg-info/top_level.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       79 2024-05-13 13:04:52.549947 lions-1.0.1/setup.cfg
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1226 2024-05-13 13:04:29.000000 lions-1.0.1/setup.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:04:52.549037 lions-1.0.1/tests/
--rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-06 14:13:19.000000 lions-1.0.1/tests/__init__.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1353 2024-05-08 14:15:59.000000 lions-1.0.1/tests/test_cpp_gen.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2844 2024-05-08 16:10:12.000000 lions-1.0.1/tests/test_lmsg.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     4716 2024-05-10 09:08:10.000000 lions-1.0.1/tests/test_yaml_parser.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:16:49.912056 lions-1.0.2/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1071 2024-04-30 12:52:47.000000 lions-1.0.2/LICENSE
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     8124 2024-05-13 13:16:49.911992 lions-1.0.2/PKG-INFO
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     7271 2024-05-10 14:36:28.000000 lions-1.0.2/README.md
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:16:49.908329 lions-1.0.2/lions/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       23 2024-05-13 08:58:00.000000 lions-1.0.2/lions/__init__.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:16:49.909673 lions-1.0.2/lions/cpp_gen/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-07 11:54:56.000000 lions-1.0.2/lions/cpp_gen/__init__.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2663 2024-05-13 13:16:38.000000 lions-1.0.2/lions/cpp_gen/cpp_generator.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:16:49.910449 lions-1.0.2/lions/cpp_gen/templates/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1132 2024-05-07 12:48:43.000000 lions-1.0.2/lions/cpp_gen/templates/lions.cpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)      961 2024-05-10 09:27:52.000000 lions-1.0.2/lions/cpp_gen/templates/lions.hpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2203 2024-05-10 09:08:10.000000 lions-1.0.2/lions/cpp_gen/templates/msg.cpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1551 2024-05-10 13:07:27.000000 lions-1.0.2/lions/cpp_gen/templates/msg.hpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     3175 2024-05-10 09:08:10.000000 lions-1.0.2/lions/errors.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     5199 2024-05-08 16:10:12.000000 lions-1.0.2/lions/lmsg.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2444 2024-05-08 16:10:12.000000 lions-1.0.2/lions/main.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     6813 2024-05-10 09:08:10.000000 lions-1.0.2/lions/yaml_parser.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:16:49.909493 lions-1.0.2/lions.egg-info/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     8124 2024-05-13 13:16:49.000000 lions-1.0.2/lions.egg-info/PKG-INFO
+-rw-r--r--   0 diogoferreira   (501) staff       (20)      593 2024-05-13 13:16:49.000000 lions-1.0.2/lions.egg-info/SOURCES.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        1 2024-05-13 13:16:49.000000 lions-1.0.2/lions.egg-info/dependency_links.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       42 2024-05-13 13:16:49.000000 lions-1.0.2/lions.egg-info/entry_points.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       59 2024-05-13 13:16:49.000000 lions-1.0.2/lions.egg-info/requires.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       12 2024-05-13 13:16:49.000000 lions-1.0.2/lions.egg-info/top_level.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       79 2024-05-13 13:16:49.912254 lions-1.0.2/setup.cfg
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1226 2024-05-13 13:16:17.000000 lions-1.0.2/setup.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:16:49.911185 lions-1.0.2/tests/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-06 14:13:19.000000 lions-1.0.2/tests/__init__.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1353 2024-05-08 14:15:59.000000 lions-1.0.2/tests/test_cpp_gen.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2844 2024-05-08 16:10:12.000000 lions-1.0.2/tests/test_lmsg.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     4716 2024-05-10 09:08:10.000000 lions-1.0.2/tests/test_yaml_parser.py
```

### Comparing `lions-1.0.1/LICENSE` & `lions-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lions-1.0.1/PKG-INFO` & `lions-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lions
-Version: 1.0.1
+Version: 1.0.2
 Summary: LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.
 Home-page: https://github.com/ItsNotSoftware/lions
 Author: Diogo Ferreira
 Author-email: itsnotsoftware@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lions-1.0.1/README.md` & `lions-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `lions-1.0.1/lions/cpp_gen/cpp_generator.py` & `lions-1.0.2/lions/cpp_gen/cpp_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from jinja2 import Environment, FileSystemLoader
 from lions.lmsg import LMsg
 import time
 from colorama import Fore, Style
+import os
 
 
 def print_generation_status(output_dir, file_name):
     timestamp = time.strftime("%Y-%m-%d %H:%M:%S")
     print(f"{timestamp} - Successfully generated: {output_dir}/{file_name}")
 
 
@@ -16,15 +17,16 @@
 
         Args:
             output_dir (str): The output directory where the generated files will be saved
         """
 
         self.output_dir = output_dir
 
-        self.env = Environment(loader=FileSystemLoader("lions/cpp_gen/templates"))
+        template_dir = os.path.dirname(__file__) + "/templates"
+        self.env = Environment(loader=FileSystemLoader(template_dir))
 
         # Load the templates
         self.lions_hpp_template = self.env.get_template("lions.hpp.jinja")
         self.lions_cpp_template = self.env.get_template("lions.cpp.jinja")
         self.msg_hpp_template = self.env.get_template("msg.hpp.jinja")
         self.msg_cpp_template = self.env.get_template("msg.cpp.jinja")
```

### Comparing `lions-1.0.1/lions/cpp_gen/templates/lions.cpp.jinja` & `lions-1.0.2/lions/cpp_gen/templates/lions.cpp.jinja`

 * *Files identical despite different names*

### Comparing `lions-1.0.1/lions/cpp_gen/templates/lions.hpp.jinja` & `lions-1.0.2/lions/cpp_gen/templates/lions.hpp.jinja`

 * *Files identical despite different names*

### Comparing `lions-1.0.1/lions/cpp_gen/templates/msg.cpp.jinja` & `lions-1.0.2/lions/cpp_gen/templates/msg.cpp.jinja`

 * *Files identical despite different names*

### Comparing `lions-1.0.1/lions/cpp_gen/templates/msg.hpp.jinja` & `lions-1.0.2/lions/cpp_gen/templates/msg.hpp.jinja`

 * *Files identical despite different names*

### Comparing `lions-1.0.1/lions/errors.py` & `lions-1.0.2/lions/errors.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.1/lions/lmsg.py` & `lions-1.0.2/lions/lmsg.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.1/lions/main.py` & `lions-1.0.2/lions/main.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.1/lions/yaml_parser.py` & `lions-1.0.2/lions/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.1/lions.egg-info/PKG-INFO` & `lions-1.0.2/lions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lions
-Version: 1.0.1
+Version: 1.0.2
 Summary: LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.
 Home-page: https://github.com/ItsNotSoftware/lions
 Author: Diogo Ferreira
 Author-email: itsnotsoftware@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lions-1.0.1/lions.egg-info/SOURCES.txt` & `lions-1.0.2/lions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lions-1.0.1/setup.py` & `lions-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="lions",
-    version="1.0.1",
+    version="1.0.2",
     author="Diogo Ferreira",
     author_email="itsnotsoftware@gmail.com",
     description="LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    package_data={'lions': ['cpp_gen/templates/*.jinja']},
+    package_data={"lions": ["cpp_gen/templates/*.jinja"]},
     url="https://github.com/ItsNotSoftware/lions",
     license="MIT",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

### Comparing `lions-1.0.1/tests/test_cpp_gen.py` & `lions-1.0.2/tests/test_cpp_gen.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.1/tests/test_lmsg.py` & `lions-1.0.2/tests/test_lmsg.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.1/tests/test_yaml_parser.py` & `lions-1.0.2/tests/test_yaml_parser.py`

 * *Files identical despite different names*

