# Comparing `tmp/lions-1.0.2.tar.gz` & `tmp/lions-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lions-1.0.2.tar", last modified: Mon May 13 13:16:49 2024, max compression
+gzip compressed data, was "lions-1.0.4.tar", last modified: Mon May 13 13:25:32 2024, max compression
```

## Comparing `lions-1.0.2.tar` & `lions-1.0.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:16:49.912056 lions-1.0.2/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1071 2024-04-30 12:52:47.000000 lions-1.0.2/LICENSE
--rw-r--r--   0 diogoferreira   (501) staff       (20)     8124 2024-05-13 13:16:49.911992 lions-1.0.2/PKG-INFO
--rw-r--r--   0 diogoferreira   (501) staff       (20)     7271 2024-05-10 14:36:28.000000 lions-1.0.2/README.md
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:16:49.908329 lions-1.0.2/lions/
--rw-r--r--   0 diogoferreira   (501) staff       (20)       23 2024-05-13 08:58:00.000000 lions-1.0.2/lions/__init__.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:16:49.909673 lions-1.0.2/lions/cpp_gen/
--rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-07 11:54:56.000000 lions-1.0.2/lions/cpp_gen/__init__.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2663 2024-05-13 13:16:38.000000 lions-1.0.2/lions/cpp_gen/cpp_generator.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:16:49.910449 lions-1.0.2/lions/cpp_gen/templates/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1132 2024-05-07 12:48:43.000000 lions-1.0.2/lions/cpp_gen/templates/lions.cpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)      961 2024-05-10 09:27:52.000000 lions-1.0.2/lions/cpp_gen/templates/lions.hpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2203 2024-05-10 09:08:10.000000 lions-1.0.2/lions/cpp_gen/templates/msg.cpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1551 2024-05-10 13:07:27.000000 lions-1.0.2/lions/cpp_gen/templates/msg.hpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     3175 2024-05-10 09:08:10.000000 lions-1.0.2/lions/errors.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     5199 2024-05-08 16:10:12.000000 lions-1.0.2/lions/lmsg.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2444 2024-05-08 16:10:12.000000 lions-1.0.2/lions/main.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     6813 2024-05-10 09:08:10.000000 lions-1.0.2/lions/yaml_parser.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:16:49.909493 lions-1.0.2/lions.egg-info/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     8124 2024-05-13 13:16:49.000000 lions-1.0.2/lions.egg-info/PKG-INFO
--rw-r--r--   0 diogoferreira   (501) staff       (20)      593 2024-05-13 13:16:49.000000 lions-1.0.2/lions.egg-info/SOURCES.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)        1 2024-05-13 13:16:49.000000 lions-1.0.2/lions.egg-info/dependency_links.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       42 2024-05-13 13:16:49.000000 lions-1.0.2/lions.egg-info/entry_points.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       59 2024-05-13 13:16:49.000000 lions-1.0.2/lions.egg-info/requires.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       12 2024-05-13 13:16:49.000000 lions-1.0.2/lions.egg-info/top_level.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       79 2024-05-13 13:16:49.912254 lions-1.0.2/setup.cfg
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1226 2024-05-13 13:16:17.000000 lions-1.0.2/setup.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:16:49.911185 lions-1.0.2/tests/
--rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-06 14:13:19.000000 lions-1.0.2/tests/__init__.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1353 2024-05-08 14:15:59.000000 lions-1.0.2/tests/test_cpp_gen.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2844 2024-05-08 16:10:12.000000 lions-1.0.2/tests/test_lmsg.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     4716 2024-05-10 09:08:10.000000 lions-1.0.2/tests/test_yaml_parser.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:25:32.467359 lions-1.0.4/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1071 2024-04-30 12:52:47.000000 lions-1.0.4/LICENSE
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     8124 2024-05-13 13:25:32.467291 lions-1.0.4/PKG-INFO
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     7271 2024-05-10 14:36:28.000000 lions-1.0.4/README.md
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:25:32.462560 lions-1.0.4/lions/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       23 2024-05-13 08:58:00.000000 lions-1.0.4/lions/__init__.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:25:32.463730 lions-1.0.4/lions/cpp_gen/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-07 11:54:56.000000 lions-1.0.4/lions/cpp_gen/__init__.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2663 2024-05-13 13:16:38.000000 lions-1.0.4/lions/cpp_gen/cpp_generator.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:25:32.464610 lions-1.0.4/lions/cpp_gen/templates/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1132 2024-05-07 12:48:43.000000 lions-1.0.4/lions/cpp_gen/templates/lions.cpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)      961 2024-05-10 09:27:52.000000 lions-1.0.4/lions/cpp_gen/templates/lions.hpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2203 2024-05-10 09:08:10.000000 lions-1.0.4/lions/cpp_gen/templates/msg.cpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1551 2024-05-10 13:07:27.000000 lions-1.0.4/lions/cpp_gen/templates/msg.hpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     3175 2024-05-10 09:08:10.000000 lions-1.0.4/lions/errors.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     5199 2024-05-08 16:10:12.000000 lions-1.0.4/lions/lmsg.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2444 2024-05-08 16:10:12.000000 lions-1.0.4/lions/main.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     6813 2024-05-10 09:08:10.000000 lions-1.0.4/lions/yaml_parser.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:25:32.463539 lions-1.0.4/lions.egg-info/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     8124 2024-05-13 13:25:32.000000 lions-1.0.4/lions.egg-info/PKG-INFO
+-rw-r--r--   0 diogoferreira   (501) staff       (20)      593 2024-05-13 13:25:32.000000 lions-1.0.4/lions.egg-info/SOURCES.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        1 2024-05-13 13:25:32.000000 lions-1.0.4/lions.egg-info/dependency_links.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       42 2024-05-13 13:25:32.000000 lions-1.0.4/lions.egg-info/entry_points.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       59 2024-05-13 13:25:32.000000 lions-1.0.4/lions.egg-info/requires.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       12 2024-05-13 13:25:32.000000 lions-1.0.4/lions.egg-info/top_level.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       79 2024-05-13 13:25:32.467562 lions-1.0.4/setup.cfg
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1226 2024-05-13 13:24:30.000000 lions-1.0.4/setup.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 13:25:32.466615 lions-1.0.4/tests/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-06 14:13:19.000000 lions-1.0.4/tests/__init__.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1353 2024-05-08 14:15:59.000000 lions-1.0.4/tests/test_cpp_gen.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2844 2024-05-08 16:10:12.000000 lions-1.0.4/tests/test_lmsg.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     4716 2024-05-10 09:08:10.000000 lions-1.0.4/tests/test_yaml_parser.py
```

### Comparing `lions-1.0.2/LICENSE` & `lions-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lions-1.0.2/PKG-INFO` & `lions-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lions
-Version: 1.0.2
+Version: 1.0.4
 Summary: LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.
 Home-page: https://github.com/ItsNotSoftware/lions
 Author: Diogo Ferreira
 Author-email: itsnotsoftware@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lions-1.0.2/README.md` & `lions-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lions-1.0.2/lions/cpp_gen/cpp_generator.py` & `lions-1.0.4/lions/cpp_gen/cpp_generator.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.2/lions/cpp_gen/templates/lions.cpp.jinja` & `lions-1.0.4/lions/cpp_gen/templates/lions.cpp.jinja`

 * *Files identical despite different names*

### Comparing `lions-1.0.2/lions/cpp_gen/templates/lions.hpp.jinja` & `lions-1.0.4/lions/cpp_gen/templates/lions.hpp.jinja`

 * *Files identical despite different names*

### Comparing `lions-1.0.2/lions/cpp_gen/templates/msg.cpp.jinja` & `lions-1.0.4/lions/cpp_gen/templates/msg.cpp.jinja`

 * *Files identical despite different names*

### Comparing `lions-1.0.2/lions/cpp_gen/templates/msg.hpp.jinja` & `lions-1.0.4/lions/cpp_gen/templates/msg.hpp.jinja`

 * *Files identical despite different names*

### Comparing `lions-1.0.2/lions/errors.py` & `lions-1.0.4/lions/errors.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.2/lions/lmsg.py` & `lions-1.0.4/lions/lmsg.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.2/lions/main.py` & `lions-1.0.4/lions/main.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.2/lions/yaml_parser.py` & `lions-1.0.4/lions/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.2/lions.egg-info/PKG-INFO` & `lions-1.0.4/lions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lions
-Version: 1.0.2
+Version: 1.0.4
 Summary: LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.
 Home-page: https://github.com/ItsNotSoftware/lions
 Author: Diogo Ferreira
 Author-email: itsnotsoftware@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lions-1.0.2/lions.egg-info/SOURCES.txt` & `lions-1.0.4/lions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lions-1.0.2/setup.py` & `lions-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="lions",
-    version="1.0.2",
+    version="1.0.4",
     author="Diogo Ferreira",
     author_email="itsnotsoftware@gmail.com",
     description="LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_data={"lions": ["cpp_gen/templates/*.jinja"]},
     url="https://github.com/ItsNotSoftware/lions",
```

### Comparing `lions-1.0.2/tests/test_cpp_gen.py` & `lions-1.0.4/tests/test_cpp_gen.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.2/tests/test_lmsg.py` & `lions-1.0.4/tests/test_lmsg.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.2/tests/test_yaml_parser.py` & `lions-1.0.4/tests/test_yaml_parser.py`

 * *Files identical despite different names*

