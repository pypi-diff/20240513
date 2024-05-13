# Comparing `tmp/lions-1.0.0.tar.gz` & `tmp/lions-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lions-1.0.0.tar", last modified: Mon May 13 12:08:05 2024, max compression
+gzip compressed data, was "lions-1.0.1.tar", last modified: Mon May 13 13:04:52 2024, max compression
```

## Comparing `lions-1.0.0.tar` & `lions-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,32 @@
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 12:08:05.451677 lions-1.0.0/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1071 2024-04-30 12:52:47.000000 lions-1.0.0/LICENSE
--rw-r--r--   0 diogoferreira   (501) staff       (20)     8124 2024-05-13 12:08:05.451608 lions-1.0.0/PKG-INFO
--rw-r--r--   0 diogoferreira   (501) staff       (20)     7271 2024-05-10 14:36:28.000000 lions-1.0.0/README.md
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 12:08:05.448712 lions-1.0.0/lions/
--rw-r--r--   0 diogoferreira   (501) staff       (20)       23 2024-05-13 08:58:00.000000 lions-1.0.0/lions/__init__.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 12:08:05.449947 lions-1.0.0/lions/cpp_gen/
--rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-07 11:54:56.000000 lions-1.0.0/lions/cpp_gen/__init__.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2602 2024-05-08 14:15:59.000000 lions-1.0.0/lions/cpp_gen/cpp_generator.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     3175 2024-05-10 09:08:10.000000 lions-1.0.0/lions/errors.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     5199 2024-05-08 16:10:12.000000 lions-1.0.0/lions/lmsg.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2444 2024-05-08 16:10:12.000000 lions-1.0.0/lions/main.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     6813 2024-05-10 09:08:10.000000 lions-1.0.0/lions/yaml_parser.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 12:08:05.449750 lions-1.0.0/lions.egg-info/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     8124 2024-05-13 12:08:05.000000 lions-1.0.0/lions.egg-info/PKG-INFO
--rw-r--r--   0 diogoferreira   (501) staff       (20)      437 2024-05-13 12:08:05.000000 lions-1.0.0/lions.egg-info/SOURCES.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)        1 2024-05-13 12:08:05.000000 lions-1.0.0/lions.egg-info/dependency_links.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       42 2024-05-13 12:08:05.000000 lions-1.0.0/lions.egg-info/entry_points.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       59 2024-05-13 12:08:05.000000 lions-1.0.0/lions.egg-info/requires.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       12 2024-05-13 12:08:05.000000 lions-1.0.0/lions.egg-info/top_level.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       79 2024-05-13 12:08:05.451883 lions-1.0.0/setup.cfg
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1136 2024-05-13 12:07:56.000000 lions-1.0.0/setup.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 12:08:05.450898 lions-1.0.0/tests/
--rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-06 14:13:19.000000 lions-1.0.0/tests/__init__.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1353 2024-05-08 14:15:59.000000 lions-1.0.0/tests/test_cpp_gen.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2844 2024-05-08 16:10:12.000000 lions-1.0.0/tests/test_lmsg.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     4716 2024-05-10 09:08:10.000000 lions-1.0.0/tests/test_yaml_parser.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:04:52.549715 lions-1.0.1/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1071 2024-04-30 12:52:47.000000 lions-1.0.1/LICENSE
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     8124 2024-05-13 13:04:52.549641 lions-1.0.1/PKG-INFO
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     7271 2024-05-10 14:36:28.000000 lions-1.0.1/README.md
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:04:52.545365 lions-1.0.1/lions/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       23 2024-05-13 08:58:00.000000 lions-1.0.1/lions/__init__.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:04:52.546633 lions-1.0.1/lions/cpp_gen/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-07 11:54:56.000000 lions-1.0.1/lions/cpp_gen/__init__.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2602 2024-05-08 14:15:59.000000 lions-1.0.1/lions/cpp_gen/cpp_generator.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:04:52.547971 lions-1.0.1/lions/cpp_gen/templates/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1132 2024-05-07 12:48:43.000000 lions-1.0.1/lions/cpp_gen/templates/lions.cpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)      961 2024-05-10 09:27:52.000000 lions-1.0.1/lions/cpp_gen/templates/lions.hpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2203 2024-05-10 09:08:10.000000 lions-1.0.1/lions/cpp_gen/templates/msg.cpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1551 2024-05-10 13:07:27.000000 lions-1.0.1/lions/cpp_gen/templates/msg.hpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     3175 2024-05-10 09:08:10.000000 lions-1.0.1/lions/errors.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     5199 2024-05-08 16:10:12.000000 lions-1.0.1/lions/lmsg.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2444 2024-05-08 16:10:12.000000 lions-1.0.1/lions/main.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     6813 2024-05-10 09:08:10.000000 lions-1.0.1/lions/yaml_parser.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:04:52.546452 lions-1.0.1/lions.egg-info/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     8124 2024-05-13 13:04:52.000000 lions-1.0.1/lions.egg-info/PKG-INFO
+-rw-r--r--   0 diogoferreira   (501) staff       (20)      593 2024-05-13 13:04:52.000000 lions-1.0.1/lions.egg-info/SOURCES.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        1 2024-05-13 13:04:52.000000 lions-1.0.1/lions.egg-info/dependency_links.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       42 2024-05-13 13:04:52.000000 lions-1.0.1/lions.egg-info/entry_points.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       59 2024-05-13 13:04:52.000000 lions-1.0.1/lions.egg-info/requires.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       12 2024-05-13 13:04:52.000000 lions-1.0.1/lions.egg-info/top_level.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       79 2024-05-13 13:04:52.549947 lions-1.0.1/setup.cfg
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1226 2024-05-13 13:04:29.000000 lions-1.0.1/setup.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:04:52.549037 lions-1.0.1/tests/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-06 14:13:19.000000 lions-1.0.1/tests/__init__.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1353 2024-05-08 14:15:59.000000 lions-1.0.1/tests/test_cpp_gen.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2844 2024-05-08 16:10:12.000000 lions-1.0.1/tests/test_lmsg.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     4716 2024-05-10 09:08:10.000000 lions-1.0.1/tests/test_yaml_parser.py
```

### Comparing `lions-1.0.0/LICENSE` & `lions-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lions-1.0.0/PKG-INFO` & `lions-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lions
-Version: 1.0.0
+Version: 1.0.1
 Summary: LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.
 Home-page: https://github.com/ItsNotSoftware/lions
 Author: Diogo Ferreira
 Author-email: itsnotsoftware@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lions-1.0.0/README.md` & `lions-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `lions-1.0.0/lions/cpp_gen/cpp_generator.py` & `lions-1.0.1/lions/cpp_gen/cpp_generator.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.0/lions/errors.py` & `lions-1.0.1/lions/errors.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.0/lions/lmsg.py` & `lions-1.0.1/lions/lmsg.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.0/lions/main.py` & `lions-1.0.1/lions/main.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.0/lions/yaml_parser.py` & `lions-1.0.1/lions/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.0/lions.egg-info/PKG-INFO` & `lions-1.0.1/lions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lions
-Version: 1.0.0
+Version: 1.0.1
 Summary: LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.
 Home-page: https://github.com/ItsNotSoftware/lions
 Author: Diogo Ferreira
 Author-email: itsnotsoftware@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lions-1.0.0/setup.py` & `lions-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="lions",
-    version="1.0.0",
+    version="1.0.1",
     author="Diogo Ferreira",
     author_email="itsnotsoftware@gmail.com",
     description="LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
+    package_data={'lions': ['cpp_gen/templates/*.jinja']},
     url="https://github.com/ItsNotSoftware/lions",
     license="MIT",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(),
     install_requires=["pydantic", "pyyaml", "jinja2", "pytest", "colorama"],
     extras_require={
         "dev": ["twine>=4.0.2"],
     },
+    include_package_data=True,
     entry_points={
         "console_scripts": [
             "lions = lions.main:main",
         ],
     },
 )
```

### Comparing `lions-1.0.0/tests/test_cpp_gen.py` & `lions-1.0.1/tests/test_cpp_gen.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.0/tests/test_lmsg.py` & `lions-1.0.1/tests/test_lmsg.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.0/tests/test_yaml_parser.py` & `lions-1.0.1/tests/test_yaml_parser.py`

 * *Files identical despite different names*

