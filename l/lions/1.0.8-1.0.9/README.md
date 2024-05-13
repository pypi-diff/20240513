# Comparing `tmp/lions-1.0.8.tar.gz` & `tmp/lions-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lions-1.0.8.tar", last modified: Mon May 13 14:31:44 2024, max compression
+gzip compressed data, was "lions-1.0.9.tar", last modified: Mon May 13 14:36:16 2024, max compression
```

## Comparing `lions-1.0.8.tar` & `lions-1.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 14:31:44.484646 lions-1.0.8/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1071 2024-04-30 12:52:47.000000 lions-1.0.8/LICENSE
--rw-r--r--   0 diogoferreira   (501) staff       (20)     8124 2024-05-13 14:31:44.484579 lions-1.0.8/PKG-INFO
--rw-r--r--   0 diogoferreira   (501) staff       (20)     7271 2024-05-10 14:36:28.000000 lions-1.0.8/README.md
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 14:31:44.481453 lions-1.0.8/lions/
--rw-r--r--   0 diogoferreira   (501) staff       (20)       23 2024-05-13 08:58:00.000000 lions-1.0.8/lions/__init__.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 14:31:44.482500 lions-1.0.8/lions/cpp_gen/
--rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-07 11:54:56.000000 lions-1.0.8/lions/cpp_gen/__init__.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2709 2024-05-13 14:07:26.000000 lions-1.0.8/lions/cpp_gen/cpp_generator.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 14:31:44.483238 lions-1.0.8/lions/cpp_gen/templates/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1132 2024-05-07 12:48:43.000000 lions-1.0.8/lions/cpp_gen/templates/lions.cpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)      961 2024-05-10 09:27:52.000000 lions-1.0.8/lions/cpp_gen/templates/lions.hpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2209 2024-05-13 14:31:30.000000 lions-1.0.8/lions/cpp_gen/templates/msg.cpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1551 2024-05-10 13:07:27.000000 lions-1.0.8/lions/cpp_gen/templates/msg.hpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     3175 2024-05-10 09:08:10.000000 lions-1.0.8/lions/errors.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     5199 2024-05-08 16:10:12.000000 lions-1.0.8/lions/lmsg.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2444 2024-05-08 16:10:12.000000 lions-1.0.8/lions/main.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     6813 2024-05-10 09:08:10.000000 lions-1.0.8/lions/yaml_parser.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 14:31:44.482318 lions-1.0.8/lions.egg-info/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     8124 2024-05-13 14:31:44.000000 lions-1.0.8/lions.egg-info/PKG-INFO
--rw-r--r--   0 diogoferreira   (501) staff       (20)      593 2024-05-13 14:31:44.000000 lions-1.0.8/lions.egg-info/SOURCES.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)        1 2024-05-13 14:31:44.000000 lions-1.0.8/lions.egg-info/dependency_links.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       42 2024-05-13 14:31:44.000000 lions-1.0.8/lions.egg-info/entry_points.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       59 2024-05-13 14:31:44.000000 lions-1.0.8/lions.egg-info/requires.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       12 2024-05-13 14:31:44.000000 lions-1.0.8/lions.egg-info/top_level.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       79 2024-05-13 14:31:44.484853 lions-1.0.8/setup.cfg
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1226 2024-05-13 14:31:15.000000 lions-1.0.8/setup.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 14:31:44.483968 lions-1.0.8/tests/
--rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-06 14:13:19.000000 lions-1.0.8/tests/__init__.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1353 2024-05-08 14:15:59.000000 lions-1.0.8/tests/test_cpp_gen.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2844 2024-05-08 16:10:12.000000 lions-1.0.8/tests/test_lmsg.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     4716 2024-05-10 09:08:10.000000 lions-1.0.8/tests/test_yaml_parser.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 14:36:16.320764 lions-1.0.9/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1071 2024-04-30 12:52:47.000000 lions-1.0.9/LICENSE
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     8124 2024-05-13 14:36:16.320695 lions-1.0.9/PKG-INFO
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     7271 2024-05-10 14:36:28.000000 lions-1.0.9/README.md
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 14:36:16.317061 lions-1.0.9/lions/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       23 2024-05-13 08:58:00.000000 lions-1.0.9/lions/__init__.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 14:36:16.318356 lions-1.0.9/lions/cpp_gen/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-07 11:54:56.000000 lions-1.0.9/lions/cpp_gen/__init__.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2709 2024-05-13 14:07:26.000000 lions-1.0.9/lions/cpp_gen/cpp_generator.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 14:36:16.319292 lions-1.0.9/lions/cpp_gen/templates/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1132 2024-05-07 12:48:43.000000 lions-1.0.9/lions/cpp_gen/templates/lions.cpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)      961 2024-05-10 09:27:52.000000 lions-1.0.9/lions/cpp_gen/templates/lions.hpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2221 2024-05-13 14:34:59.000000 lions-1.0.9/lions/cpp_gen/templates/msg.cpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1550 2024-05-13 14:35:51.000000 lions-1.0.9/lions/cpp_gen/templates/msg.hpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     3175 2024-05-10 09:08:10.000000 lions-1.0.9/lions/errors.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     5199 2024-05-08 16:10:12.000000 lions-1.0.9/lions/lmsg.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2444 2024-05-08 16:10:12.000000 lions-1.0.9/lions/main.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     6813 2024-05-10 09:08:10.000000 lions-1.0.9/lions/yaml_parser.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 14:36:16.318152 lions-1.0.9/lions.egg-info/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     8124 2024-05-13 14:36:16.000000 lions-1.0.9/lions.egg-info/PKG-INFO
+-rw-r--r--   0 diogoferreira   (501) staff       (20)      593 2024-05-13 14:36:16.000000 lions-1.0.9/lions.egg-info/SOURCES.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        1 2024-05-13 14:36:16.000000 lions-1.0.9/lions.egg-info/dependency_links.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       42 2024-05-13 14:36:16.000000 lions-1.0.9/lions.egg-info/entry_points.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       59 2024-05-13 14:36:16.000000 lions-1.0.9/lions.egg-info/requires.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       12 2024-05-13 14:36:16.000000 lions-1.0.9/lions.egg-info/top_level.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       79 2024-05-13 14:36:16.320978 lions-1.0.9/setup.cfg
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1226 2024-05-13 14:36:03.000000 lions-1.0.9/setup.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 14:36:16.319994 lions-1.0.9/tests/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-06 14:13:19.000000 lions-1.0.9/tests/__init__.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1353 2024-05-08 14:15:59.000000 lions-1.0.9/tests/test_cpp_gen.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2844 2024-05-08 16:10:12.000000 lions-1.0.9/tests/test_lmsg.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     4716 2024-05-10 09:08:10.000000 lions-1.0.9/tests/test_yaml_parser.py
```

### Comparing `lions-1.0.8/LICENSE` & `lions-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lions-1.0.8/PKG-INFO` & `lions-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lions
-Version: 1.0.8
+Version: 1.0.9
 Summary: LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.
 Home-page: https://github.com/ItsNotSoftware/lions
 Author: Diogo Ferreira
 Author-email: itsnotsoftware@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lions-1.0.8/README.md` & `lions-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `lions-1.0.8/lions/cpp_gen/cpp_generator.py` & `lions-1.0.9/lions/cpp_gen/cpp_generator.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.8/lions/cpp_gen/templates/lions.cpp.jinja` & `lions-1.0.9/lions/cpp_gen/templates/lions.cpp.jinja`

 * *Files identical despite different names*

### Comparing `lions-1.0.8/lions/cpp_gen/templates/lions.hpp.jinja` & `lions-1.0.9/lions/cpp_gen/templates/lions.hpp.jinja`

 * *Files identical despite different names*

### Comparing `lions-1.0.8/lions/cpp_gen/templates/msg.cpp.jinja` & `lions-1.0.9/lions/cpp_gen/templates/msg.cpp.jinja`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 /**
  * @file {{filename}}_lmsgs.cpp
  *
- * @brief Implementation of {{filename}}.hpp Classes
+ * @brief Implementation of {{filename}}_lmsgs.hpp Classes
  * 
  * This file contains the implementation of the message classes generated by the Lions Compiler.
  * 
  * @details
  * This file was generated by the Lions Compiler (https://github.com/ItsNotSoftware/lions) on {{date}}.
  * Modifying this file manually is not recommended as it may lead to unexpected behavior.
  * 
  * @note
  * Generated files should not be manually edited.
  * 
  * @author Lions Compiler
 */
 
-#include "{{filename}}.hpp"
+#include "{{filename}}_lmsgs.hpp"
 
 #include <algorithm>
 #include <utility>
 
 namespace lions {
 {% for msg in msgs %} 
 {{ msg.name | capitalize }}Msg::{{ msg.name | capitalize }}Msg({% for field in msg.fields %}const {{ field.type }} {{ field.name }}{% if not loop.last %}, {% endif %}{% endfor %})
```

### Comparing `lions-1.0.8/lions/cpp_gen/templates/msg.hpp.jinja` & `lions-1.0.9/lions/cpp_gen/templates/msg.hpp.jinja`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 /**
- * @file {{filename}}.hpp
+ * @file {{filename}}_lmsgs.hpp
  *
- * @brief Implementation of {{filename}}.hpp Classes
+ * @brief {{filename}}_lmsgs Classes
  * 
- * This file contains the implementation of the message classes generated by the Lions Compiler.
+ * This file contains the declaration of the message classes generated by the Lions Compiler.
  * 
  * @details
  * This file was generated by the Lions Compiler (https://github.com/ItsNotSoftware/lions) on {{date}}.
  * Modifying this file manually is not recommended as it may lead to unexpected behavior.
  * 
  * @note
  * Generated files should not be manually edited.
  * 
  * @author Lions Compiler
 */
 
-#ifndef {{filename | upper}}_HPP
-#define {{filename | upper}}_HPP
+#ifndef {{filename | upper}}_LMSGS_HPP
+#define {{filename | upper}}_LMSGS_HPP
 
 #include "lions.hpp"
 #include <string>
 
 
 namespace lions {
```

### Comparing `lions-1.0.8/lions/errors.py` & `lions-1.0.9/lions/errors.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.8/lions/lmsg.py` & `lions-1.0.9/lions/lmsg.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.8/lions/main.py` & `lions-1.0.9/lions/main.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.8/lions/yaml_parser.py` & `lions-1.0.9/lions/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.8/lions.egg-info/PKG-INFO` & `lions-1.0.9/lions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lions
-Version: 1.0.8
+Version: 1.0.9
 Summary: LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.
 Home-page: https://github.com/ItsNotSoftware/lions
 Author: Diogo Ferreira
 Author-email: itsnotsoftware@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lions-1.0.8/lions.egg-info/SOURCES.txt` & `lions-1.0.9/lions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lions-1.0.8/setup.py` & `lions-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="lions",
-    version="1.0.8",
+    version="1.0.9",
     author="Diogo Ferreira",
     author_email="itsnotsoftware@gmail.com",
     description="LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_data={"lions": ["cpp_gen/templates/*.jinja"]},
     url="https://github.com/ItsNotSoftware/lions",
```

### Comparing `lions-1.0.8/tests/test_cpp_gen.py` & `lions-1.0.9/tests/test_cpp_gen.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.8/tests/test_lmsg.py` & `lions-1.0.9/tests/test_lmsg.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.8/tests/test_yaml_parser.py` & `lions-1.0.9/tests/test_yaml_parser.py`

 * *Files identical despite different names*

