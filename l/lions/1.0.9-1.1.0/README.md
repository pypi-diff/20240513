# Comparing `tmp/lions-1.0.9.tar.gz` & `tmp/lions-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lions-1.0.9.tar", last modified: Mon May 13 14:36:16 2024, max compression
+gzip compressed data, was "lions-1.1.0.tar", last modified: Mon May 13 15:12:13 2024, max compression
```

## Comparing `lions-1.0.9.tar` & `lions-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 14:36:16.320764 lions-1.0.9/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1071 2024-04-30 12:52:47.000000 lions-1.0.9/LICENSE
--rw-r--r--   0 diogoferreira   (501) staff       (20)     8124 2024-05-13 14:36:16.320695 lions-1.0.9/PKG-INFO
--rw-r--r--   0 diogoferreira   (501) staff       (20)     7271 2024-05-10 14:36:28.000000 lions-1.0.9/README.md
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 14:36:16.317061 lions-1.0.9/lions/
--rw-r--r--   0 diogoferreira   (501) staff       (20)       23 2024-05-13 08:58:00.000000 lions-1.0.9/lions/__init__.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 14:36:16.318356 lions-1.0.9/lions/cpp_gen/
--rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-07 11:54:56.000000 lions-1.0.9/lions/cpp_gen/__init__.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2709 2024-05-13 14:07:26.000000 lions-1.0.9/lions/cpp_gen/cpp_generator.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 14:36:16.319292 lions-1.0.9/lions/cpp_gen/templates/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1132 2024-05-07 12:48:43.000000 lions-1.0.9/lions/cpp_gen/templates/lions.cpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)      961 2024-05-10 09:27:52.000000 lions-1.0.9/lions/cpp_gen/templates/lions.hpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2221 2024-05-13 14:34:59.000000 lions-1.0.9/lions/cpp_gen/templates/msg.cpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1550 2024-05-13 14:35:51.000000 lions-1.0.9/lions/cpp_gen/templates/msg.hpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     3175 2024-05-10 09:08:10.000000 lions-1.0.9/lions/errors.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     5199 2024-05-08 16:10:12.000000 lions-1.0.9/lions/lmsg.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2444 2024-05-08 16:10:12.000000 lions-1.0.9/lions/main.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     6813 2024-05-10 09:08:10.000000 lions-1.0.9/lions/yaml_parser.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 14:36:16.318152 lions-1.0.9/lions.egg-info/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     8124 2024-05-13 14:36:16.000000 lions-1.0.9/lions.egg-info/PKG-INFO
--rw-r--r--   0 diogoferreira   (501) staff       (20)      593 2024-05-13 14:36:16.000000 lions-1.0.9/lions.egg-info/SOURCES.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)        1 2024-05-13 14:36:16.000000 lions-1.0.9/lions.egg-info/dependency_links.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       42 2024-05-13 14:36:16.000000 lions-1.0.9/lions.egg-info/entry_points.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       59 2024-05-13 14:36:16.000000 lions-1.0.9/lions.egg-info/requires.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       12 2024-05-13 14:36:16.000000 lions-1.0.9/lions.egg-info/top_level.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       79 2024-05-13 14:36:16.320978 lions-1.0.9/setup.cfg
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1226 2024-05-13 14:36:03.000000 lions-1.0.9/setup.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 14:36:16.319994 lions-1.0.9/tests/
--rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-06 14:13:19.000000 lions-1.0.9/tests/__init__.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1353 2024-05-08 14:15:59.000000 lions-1.0.9/tests/test_cpp_gen.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2844 2024-05-08 16:10:12.000000 lions-1.0.9/tests/test_lmsg.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     4716 2024-05-10 09:08:10.000000 lions-1.0.9/tests/test_yaml_parser.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 15:12:13.652979 lions-1.1.0/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1071 2024-04-30 12:52:47.000000 lions-1.1.0/LICENSE
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     8124 2024-05-13 15:12:13.652910 lions-1.1.0/PKG-INFO
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     7271 2024-05-10 14:36:28.000000 lions-1.1.0/README.md
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 15:12:13.649139 lions-1.1.0/lions/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       23 2024-05-13 08:58:00.000000 lions-1.1.0/lions/__init__.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 15:12:13.650395 lions-1.1.0/lions/cpp_gen/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-07 11:54:56.000000 lions-1.1.0/lions/cpp_gen/__init__.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2709 2024-05-13 14:07:26.000000 lions-1.1.0/lions/cpp_gen/cpp_generator.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 15:12:13.651319 lions-1.1.0/lions/cpp_gen/templates/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1202 2024-05-13 14:58:05.000000 lions-1.1.0/lions/cpp_gen/templates/lions.cpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1125 2024-05-13 15:10:01.000000 lions-1.1.0/lions/cpp_gen/templates/lions.hpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2221 2024-05-13 14:34:59.000000 lions-1.1.0/lions/cpp_gen/templates/msg.cpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1550 2024-05-13 14:35:51.000000 lions-1.1.0/lions/cpp_gen/templates/msg.hpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     3175 2024-05-10 09:08:10.000000 lions-1.1.0/lions/errors.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     5199 2024-05-08 16:10:12.000000 lions-1.1.0/lions/lmsg.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2444 2024-05-08 16:10:12.000000 lions-1.1.0/lions/main.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     6813 2024-05-10 09:08:10.000000 lions-1.1.0/lions/yaml_parser.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 15:12:13.650183 lions-1.1.0/lions.egg-info/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     8124 2024-05-13 15:12:13.000000 lions-1.1.0/lions.egg-info/PKG-INFO
+-rw-r--r--   0 diogoferreira   (501) staff       (20)      593 2024-05-13 15:12:13.000000 lions-1.1.0/lions.egg-info/SOURCES.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        1 2024-05-13 15:12:13.000000 lions-1.1.0/lions.egg-info/dependency_links.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       42 2024-05-13 15:12:13.000000 lions-1.1.0/lions.egg-info/entry_points.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       59 2024-05-13 15:12:13.000000 lions-1.1.0/lions.egg-info/requires.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       12 2024-05-13 15:12:13.000000 lions-1.1.0/lions.egg-info/top_level.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       79 2024-05-13 15:12:13.653184 lions-1.1.0/setup.cfg
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1226 2024-05-13 15:12:06.000000 lions-1.1.0/setup.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 15:12:13.652077 lions-1.1.0/tests/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-06 14:13:19.000000 lions-1.1.0/tests/__init__.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1353 2024-05-08 14:15:59.000000 lions-1.1.0/tests/test_cpp_gen.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2844 2024-05-08 16:10:12.000000 lions-1.1.0/tests/test_lmsg.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     4716 2024-05-10 09:08:10.000000 lions-1.1.0/tests/test_yaml_parser.py
```

### Comparing `lions-1.0.9/LICENSE` & `lions-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lions-1.0.9/PKG-INFO` & `lions-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lions
-Version: 1.0.9
+Version: 1.1.0
 Summary: LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.
 Home-page: https://github.com/ItsNotSoftware/lions
 Author: Diogo Ferreira
 Author-email: itsnotsoftware@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lions-1.0.9/README.md` & `lions-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `lions-1.0.9/lions/cpp_gen/cpp_generator.py` & `lions-1.1.0/lions/cpp_gen/cpp_generator.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.9/lions/cpp_gen/templates/lions.cpp.jinja` & `lions-1.1.0/lions/cpp_gen/templates/lions.cpp.jinja`

 * *Files 19% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 #include "lions.hpp"
 
 namespace lions {
 
 LMsg::LMsg(uint8_t payload_size) : payload_size(payload_size) {}
 
 uint16_t LMsg::calculate_checksum() {
-    checksum = 0;
+    header.checksum = 0;
 
     // Calculate checksum for the header
-    checksum += header.src;
-    checksum += header.dst;
-    checksum += header.msg_id;
-    checksum += header.next_hop;
+    header.checksum += header.src;
+    header.checksum += header.dst;
+    header.checksum += header.msg_id;
+    header.checksum += header.next_hop;
 
     // Calculate checksum for the payload
-    checksum += std::accumulate(payload, payload + payload_size, 0);
+    header.checksum += std::accumulate(payload, payload + payload_size, 0);
 
-    checksum = ~checksum;
+    header.checksum = ~header.checksum;
 
-    return checksum;
+    return header.checksum;
 }
 
 bool LMsg::valid_checksum() {
-    uint16_t prev_checksum = checksum;
+    uint16_t prev_checksum = header.checksum;
     return calculate_checksum() == prev_checksum;
 }
 
 }  // namespace lions
```

### Comparing `lions-1.0.9/lions/cpp_gen/templates/lions.hpp.jinja` & `lions-1.1.0/lions/cpp_gen/templates/lions.hpp.jinja`

 * *Files 13% similar despite different names*

```diff
@@ -18,31 +18,40 @@
 
 #ifndef LMSG_HPP
 #define LMSG_HPP
 
 #include <cstdint>
 
 namespace lions {
+
+constexpr uint8_t MAX_PAYLOAD_SIZE = 248;
+
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
 
 }  // namespace lions
 
 #endif
```

### Comparing `lions-1.0.9/lions/cpp_gen/templates/msg.cpp.jinja` & `lions-1.1.0/lions/cpp_gen/templates/msg.cpp.jinja`

 * *Files identical despite different names*

### Comparing `lions-1.0.9/lions/cpp_gen/templates/msg.hpp.jinja` & `lions-1.1.0/lions/cpp_gen/templates/msg.hpp.jinja`

 * *Files identical despite different names*

### Comparing `lions-1.0.9/lions/errors.py` & `lions-1.1.0/lions/errors.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.9/lions/lmsg.py` & `lions-1.1.0/lions/lmsg.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.9/lions/main.py` & `lions-1.1.0/lions/main.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.9/lions/yaml_parser.py` & `lions-1.1.0/lions/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.9/lions.egg-info/PKG-INFO` & `lions-1.1.0/lions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lions
-Version: 1.0.9
+Version: 1.1.0
 Summary: LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.
 Home-page: https://github.com/ItsNotSoftware/lions
 Author: Diogo Ferreira
 Author-email: itsnotsoftware@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lions-1.0.9/lions.egg-info/SOURCES.txt` & `lions-1.1.0/lions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lions-1.0.9/setup.py` & `lions-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="lions",
-    version="1.0.9",
+    version="1.1.0",
     author="Diogo Ferreira",
     author_email="itsnotsoftware@gmail.com",
     description="LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_data={"lions": ["cpp_gen/templates/*.jinja"]},
     url="https://github.com/ItsNotSoftware/lions",
```

### Comparing `lions-1.0.9/tests/test_cpp_gen.py` & `lions-1.1.0/tests/test_cpp_gen.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.9/tests/test_lmsg.py` & `lions-1.1.0/tests/test_lmsg.py`

 * *Files identical despite different names*

### Comparing `lions-1.0.9/tests/test_yaml_parser.py` & `lions-1.1.0/tests/test_yaml_parser.py`

 * *Files identical despite different names*

