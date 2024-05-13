# Comparing `tmp/lions-1.1.0.tar.gz` & `tmp/lions-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lions-1.1.0.tar", last modified: Mon May 13 15:12:13 2024, max compression
+gzip compressed data, was "lions-1.1.1.tar", last modified: Mon May 13 15:18:19 2024, max compression
```

## Comparing `lions-1.1.0.tar` & `lions-1.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 15:12:13.652979 lions-1.1.0/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1071 2024-04-30 12:52:47.000000 lions-1.1.0/LICENSE
--rw-r--r--   0 diogoferreira   (501) staff       (20)     8124 2024-05-13 15:12:13.652910 lions-1.1.0/PKG-INFO
--rw-r--r--   0 diogoferreira   (501) staff       (20)     7271 2024-05-10 14:36:28.000000 lions-1.1.0/README.md
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 15:12:13.649139 lions-1.1.0/lions/
--rw-r--r--   0 diogoferreira   (501) staff       (20)       23 2024-05-13 08:58:00.000000 lions-1.1.0/lions/__init__.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 15:12:13.650395 lions-1.1.0/lions/cpp_gen/
--rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-07 11:54:56.000000 lions-1.1.0/lions/cpp_gen/__init__.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2709 2024-05-13 14:07:26.000000 lions-1.1.0/lions/cpp_gen/cpp_generator.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 15:12:13.651319 lions-1.1.0/lions/cpp_gen/templates/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1202 2024-05-13 14:58:05.000000 lions-1.1.0/lions/cpp_gen/templates/lions.cpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1125 2024-05-13 15:10:01.000000 lions-1.1.0/lions/cpp_gen/templates/lions.hpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2221 2024-05-13 14:34:59.000000 lions-1.1.0/lions/cpp_gen/templates/msg.cpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1550 2024-05-13 14:35:51.000000 lions-1.1.0/lions/cpp_gen/templates/msg.hpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     3175 2024-05-10 09:08:10.000000 lions-1.1.0/lions/errors.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     5199 2024-05-08 16:10:12.000000 lions-1.1.0/lions/lmsg.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2444 2024-05-08 16:10:12.000000 lions-1.1.0/lions/main.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     6813 2024-05-10 09:08:10.000000 lions-1.1.0/lions/yaml_parser.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 15:12:13.650183 lions-1.1.0/lions.egg-info/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     8124 2024-05-13 15:12:13.000000 lions-1.1.0/lions.egg-info/PKG-INFO
--rw-r--r--   0 diogoferreira   (501) staff       (20)      593 2024-05-13 15:12:13.000000 lions-1.1.0/lions.egg-info/SOURCES.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)        1 2024-05-13 15:12:13.000000 lions-1.1.0/lions.egg-info/dependency_links.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       42 2024-05-13 15:12:13.000000 lions-1.1.0/lions.egg-info/entry_points.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       59 2024-05-13 15:12:13.000000 lions-1.1.0/lions.egg-info/requires.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       12 2024-05-13 15:12:13.000000 lions-1.1.0/lions.egg-info/top_level.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       79 2024-05-13 15:12:13.653184 lions-1.1.0/setup.cfg
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1226 2024-05-13 15:12:06.000000 lions-1.1.0/setup.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 15:12:13.652077 lions-1.1.0/tests/
--rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-06 14:13:19.000000 lions-1.1.0/tests/__init__.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1353 2024-05-08 14:15:59.000000 lions-1.1.0/tests/test_cpp_gen.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2844 2024-05-08 16:10:12.000000 lions-1.1.0/tests/test_lmsg.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     4716 2024-05-10 09:08:10.000000 lions-1.1.0/tests/test_yaml_parser.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 15:18:19.262684 lions-1.1.1/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1071 2024-04-30 12:52:47.000000 lions-1.1.1/LICENSE
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     8244 2024-05-13 15:18:19.262485 lions-1.1.1/PKG-INFO
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     7391 2024-05-13 15:15:40.000000 lions-1.1.1/README.md
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 15:18:19.258869 lions-1.1.1/lions/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       23 2024-05-13 08:58:00.000000 lions-1.1.1/lions/__init__.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 15:18:19.260246 lions-1.1.1/lions/cpp_gen/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-07 11:54:56.000000 lions-1.1.1/lions/cpp_gen/__init__.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2709 2024-05-13 14:07:26.000000 lions-1.1.1/lions/cpp_gen/cpp_generator.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 15:18:19.261091 lions-1.1.1/lions/cpp_gen/templates/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1202 2024-05-13 14:58:05.000000 lions-1.1.1/lions/cpp_gen/templates/lions.cpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1125 2024-05-13 15:10:01.000000 lions-1.1.1/lions/cpp_gen/templates/lions.hpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2221 2024-05-13 14:34:59.000000 lions-1.1.1/lions/cpp_gen/templates/msg.cpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1551 2024-05-13 15:18:02.000000 lions-1.1.1/lions/cpp_gen/templates/msg.hpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     3175 2024-05-10 09:08:10.000000 lions-1.1.1/lions/errors.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     5199 2024-05-08 16:10:12.000000 lions-1.1.1/lions/lmsg.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2444 2024-05-08 16:10:12.000000 lions-1.1.1/lions/main.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     6813 2024-05-10 09:08:10.000000 lions-1.1.1/lions/yaml_parser.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 15:18:19.260039 lions-1.1.1/lions.egg-info/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     8244 2024-05-13 15:18:19.000000 lions-1.1.1/lions.egg-info/PKG-INFO
+-rw-r--r--   0 diogoferreira   (501) staff       (20)      593 2024-05-13 15:18:19.000000 lions-1.1.1/lions.egg-info/SOURCES.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        1 2024-05-13 15:18:19.000000 lions-1.1.1/lions.egg-info/dependency_links.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       42 2024-05-13 15:18:19.000000 lions-1.1.1/lions.egg-info/entry_points.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       59 2024-05-13 15:18:19.000000 lions-1.1.1/lions.egg-info/requires.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       12 2024-05-13 15:18:19.000000 lions-1.1.1/lions.egg-info/top_level.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       79 2024-05-13 15:18:19.262897 lions-1.1.1/setup.cfg
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1226 2024-05-13 15:18:13.000000 lions-1.1.1/setup.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 15:18:19.261895 lions-1.1.1/tests/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-06 14:13:19.000000 lions-1.1.1/tests/__init__.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1353 2024-05-08 14:15:59.000000 lions-1.1.1/tests/test_cpp_gen.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2844 2024-05-08 16:10:12.000000 lions-1.1.1/tests/test_lmsg.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     4716 2024-05-10 09:08:10.000000 lions-1.1.1/tests/test_yaml_parser.py
```

### Comparing `lions-1.1.0/LICENSE` & `lions-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lions-1.1.0/PKG-INFO` & `lions-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lions
-Version: 1.1.0
+Version: 1.1.1
 Summary: LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.
 Home-page: https://github.com/ItsNotSoftware/lions
 Author: Diogo Ferreira
 Author-email: itsnotsoftware@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -79,28 +79,34 @@
 
 ```C++
 struct Header {
     uint8_t src;
     uint8_t dst;
     uint8_t next_hop;
     uint8_t msg_id;
+
+    union{
+        uint16_t checksum;
+
+        struct{
+            uint8_t checksum_low;
+            uint8_t checksum_high;
+        };
+    };
 };
 
 class LMsg {
    public:
     Header header;
-    uint8_t payload[248];
+    uint8_t payload[MAX_PAYLOAD_SIZE];
     uint8_t payload_size;
 
     LMsg(uint8_t payload_size = 0);
     uint16_t calculate_checksum();
     bool valid_checksum();
-
-   private:
-    uint16_t checksum;
 };
 ```
 
 ## Defining Messages
 
 LIONS uses `.lmsg.yaml` files to define message specifications for IoT networks. Each file can contain multiple message definitions that are used by the LIONS compiler to generate C++ code for message handling.
```

### Comparing `lions-1.1.0/README.md` & `lions-1.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -58,28 +58,34 @@
 
 ```C++
 struct Header {
     uint8_t src;
     uint8_t dst;
     uint8_t next_hop;
     uint8_t msg_id;
+
+    union{
+        uint16_t checksum;
+
+        struct{
+            uint8_t checksum_low;
+            uint8_t checksum_high;
+        };
+    };
 };
 
 class LMsg {
    public:
     Header header;
-    uint8_t payload[248];
+    uint8_t payload[MAX_PAYLOAD_SIZE];
     uint8_t payload_size;
 
     LMsg(uint8_t payload_size = 0);
     uint16_t calculate_checksum();
     bool valid_checksum();
-
-   private:
-    uint16_t checksum;
 };
 ```
 
 ## Defining Messages
 
 LIONS uses `.lmsg.yaml` files to define message specifications for IoT networks. Each file can contain multiple message definitions that are used by the LIONS compiler to generate C++ code for message handling.
```

### Comparing `lions-1.1.0/lions/cpp_gen/cpp_generator.py` & `lions-1.1.1/lions/cpp_gen/cpp_generator.py`

 * *Files identical despite different names*

### Comparing `lions-1.1.0/lions/cpp_gen/templates/lions.cpp.jinja` & `lions-1.1.1/lions/cpp_gen/templates/lions.cpp.jinja`

 * *Files identical despite different names*

### Comparing `lions-1.1.0/lions/cpp_gen/templates/lions.hpp.jinja` & `lions-1.1.1/lions/cpp_gen/templates/lions.hpp.jinja`

 * *Files identical despite different names*

### Comparing `lions-1.1.0/lions/cpp_gen/templates/msg.cpp.jinja` & `lions-1.1.1/lions/cpp_gen/templates/msg.cpp.jinja`

 * *Files identical despite different names*

### Comparing `lions-1.1.0/lions/cpp_gen/templates/msg.hpp.jinja` & `lions-1.1.1/lions/cpp_gen/templates/msg.hpp.jinja`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 #include "lions.hpp"
 #include <string>
 
 
 namespace lions {
 
    namespace msg_id {
-{% for msg in msgs %}   constexpr uint8_t {{msg.name|upper}} = {{msg.id}};
+{% for msg in msgs %}   constexpr uint32_t {{msg.name|upper}} = {{msg.id}};
 {% endfor %}   }  // namespace msg_id
    
    namespace msg_period {
 {% for msg in msgs %}   constexpr uint8_t {{msg.name|upper}} = {{msg.period}};
 {% endfor %}   }  // namespace msg_period
 
 {% for msg in msgs %}
```

### Comparing `lions-1.1.0/lions/errors.py` & `lions-1.1.1/lions/errors.py`

 * *Files identical despite different names*

### Comparing `lions-1.1.0/lions/lmsg.py` & `lions-1.1.1/lions/lmsg.py`

 * *Files identical despite different names*

### Comparing `lions-1.1.0/lions/main.py` & `lions-1.1.1/lions/main.py`

 * *Files identical despite different names*

### Comparing `lions-1.1.0/lions/yaml_parser.py` & `lions-1.1.1/lions/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `lions-1.1.0/lions.egg-info/PKG-INFO` & `lions-1.1.1/lions.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lions
-Version: 1.1.0
+Version: 1.1.1
 Summary: LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.
 Home-page: https://github.com/ItsNotSoftware/lions
 Author: Diogo Ferreira
 Author-email: itsnotsoftware@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -79,28 +79,34 @@
 
 ```C++
 struct Header {
     uint8_t src;
     uint8_t dst;
     uint8_t next_hop;
     uint8_t msg_id;
+
+    union{
+        uint16_t checksum;
+
+        struct{
+            uint8_t checksum_low;
+            uint8_t checksum_high;
+        };
+    };
 };
 
 class LMsg {
    public:
     Header header;
-    uint8_t payload[248];
+    uint8_t payload[MAX_PAYLOAD_SIZE];
     uint8_t payload_size;
 
     LMsg(uint8_t payload_size = 0);
     uint16_t calculate_checksum();
     bool valid_checksum();
-
-   private:
-    uint16_t checksum;
 };
 ```
 
 ## Defining Messages
 
 LIONS uses `.lmsg.yaml` files to define message specifications for IoT networks. Each file can contain multiple message definitions that are used by the LIONS compiler to generate C++ code for message handling.
```

### Comparing `lions-1.1.0/lions.egg-info/SOURCES.txt` & `lions-1.1.1/lions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lions-1.1.0/setup.py` & `lions-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="lions",
-    version="1.1.0",
+    version="1.1.1",
     author="Diogo Ferreira",
     author_email="itsnotsoftware@gmail.com",
     description="LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_data={"lions": ["cpp_gen/templates/*.jinja"]},
     url="https://github.com/ItsNotSoftware/lions",
```

### Comparing `lions-1.1.0/tests/test_cpp_gen.py` & `lions-1.1.1/tests/test_cpp_gen.py`

 * *Files identical despite different names*

### Comparing `lions-1.1.0/tests/test_lmsg.py` & `lions-1.1.1/tests/test_lmsg.py`

 * *Files identical despite different names*

### Comparing `lions-1.1.0/tests/test_yaml_parser.py` & `lions-1.1.1/tests/test_yaml_parser.py`

 * *Files identical despite different names*

