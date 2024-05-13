# Comparing `tmp/zenaura-0.9.16a0.tar.gz` & `tmp/zenaura-0.9.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenaura-0.9.16a0.tar", last modified: Sun May 12 10:57:13 2024, max compression
+gzip compressed data, was "zenaura-0.9.31.tar", last modified: Mon May 13 15:56:20 2024, max compression
```

## Comparing `zenaura-0.9.16a0.tar` & `zenaura-0.9.31.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 10:57:13.599095 zenaura-0.9.16a0/
--rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.16a0/LICENSE
--rw-rw-rw-   0        0        0     1451 2024-05-12 10:57:13.598096 zenaura-0.9.16a0/PKG-INFO
--rw-rw-rw-   0        0        0     1044 2024-05-12 07:30:19.000000 zenaura-0.9.16a0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-12 10:57:13.599095 zenaura-0.9.16a0/setup.cfg
--rw-rw-rw-   0        0        0      710 2024-05-12 10:52:51.000000 zenaura-0.9.16a0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 10:57:13.592096 zenaura-0.9.16a0/tests/
--rw-rw-rw-   0        0        0     6348 2024-05-11 22:30:53.000000 zenaura-0.9.16a0/tests/test_compiler.py
--rw-rw-rw-   0        0        0     4109 2024-05-11 18:58:32.000000 zenaura-0.9.16a0/tests/test_component_e2e.py
--rw-rw-rw-   0        0        0     1131 2024-05-11 17:44:57.000000 zenaura-0.9.16a0/tests/test_component_unit.py
--rw-rw-rw-   0        0        0     1435 2024-05-11 20:36:50.000000 zenaura-0.9.16a0/tests/test_observer.py
--rw-rw-rw-   0        0        0     2994 2024-05-11 17:44:57.000000 zenaura-0.9.16a0/tests/test_tags.py
--rw-rw-rw-   0        0        0    13311 2024-05-12 09:57:10.000000 zenaura-0.9.16a0/tests/test_zenaura_dom.py
-drwxrwxrwx   0        0        0        0 2024-05-12 10:57:13.592597 zenaura-0.9.16a0/zenaura/
--rw-rw-rw-   0        0        0        0 2024-05-11 11:31:00.000000 zenaura-0.9.16a0/zenaura/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 10:57:13.597595 zenaura-0.9.16a0/zenaura.egg-info/
--rw-rw-rw-   0        0        0     1451 2024-05-12 10:57:13.000000 zenaura-0.9.16a0/zenaura.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-05-12 10:57:13.000000 zenaura-0.9.16a0/zenaura.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 10:57:13.000000 zenaura-0.9.16a0/zenaura.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-12 10:57:13.000000 zenaura-0.9.16a0/zenaura.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 15:56:20.881262 zenaura-0.9.31/
+-rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.31/LICENSE
+-rw-rw-rw-   0        0        0     1557 2024-05-13 15:56:20.880262 zenaura-0.9.31/PKG-INFO
+-rw-rw-rw-   0        0        0     1152 2024-05-13 15:49:51.000000 zenaura-0.9.31/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-13 15:56:20.881262 zenaura-0.9.31/setup.cfg
+-rw-rw-rw-   0        0        0      707 2024-05-13 15:55:30.000000 zenaura-0.9.31/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:56:20.873762 zenaura-0.9.31/tests/
+-rw-rw-rw-   0        0        0     6329 2024-05-13 15:49:51.000000 zenaura-0.9.31/tests/test_compiler.py
+-rw-rw-rw-   0        0        0     4109 2024-05-11 18:58:32.000000 zenaura-0.9.31/tests/test_component_e2e.py
+-rw-rw-rw-   0        0        0     1131 2024-05-11 17:44:57.000000 zenaura-0.9.31/tests/test_component_unit.py
+-rw-rw-rw-   0        0        0     1435 2024-05-11 20:36:50.000000 zenaura-0.9.31/tests/test_observer.py
+-rw-rw-rw-   0        0        0    15531 2024-05-13 15:49:51.000000 zenaura-0.9.31/tests/test_tags.py
+-rw-rw-rw-   0        0        0    13311 2024-05-13 15:49:51.000000 zenaura-0.9.31/tests/test_zenaura_dom.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:56:20.874262 zenaura-0.9.31/zenaura/
+-rw-rw-rw-   0        0        0        0 2024-05-11 11:31:00.000000 zenaura-0.9.31/zenaura/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:56:20.879762 zenaura-0.9.31/zenaura.egg-info/
+-rw-rw-rw-   0        0        0     1557 2024-05-13 15:56:20.000000 zenaura-0.9.31/zenaura.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-05-13 15:56:20.000000 zenaura-0.9.31/zenaura.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 15:56:20.000000 zenaura-0.9.31/zenaura.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-13 15:56:20.000000 zenaura-0.9.31/zenaura.egg-info/top_level.txt
```

### Comparing `zenaura-0.9.16a0/LICENSE` & `zenaura-0.9.31/LICENSE`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.16a0/PKG-INFO` & `zenaura-0.9.31/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.16a0
+Version: 0.9.31
 Summary: Zenaura, light weight, super fast python full-stack development framework, in which every line of code emit the aura of python zen, build interactive SPA with pure Python, create secure and scalable endpoints.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Zenaura 
@@ -41,7 +41,16 @@
 zenaura\client\component.py      22      2    91%   24, 34
 zenaura\client\dom.py            50      2    96%   68, 71
 zenaura\client\tags.py          144      3    98%   9-11
 -----------------------------------------------------------
 ```
 
 - important note : test coverage must be kept at 95%
+
+# run example :
+
+cd to examples folder
+cd into example folder 
+run 
+```
+flask --app hello run
+```
```

### Comparing `zenaura-0.9.16a0/README.md` & `zenaura-0.9.31/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -31,8 +31,17 @@
 zenaura\client\compiler.py       46      5    89%   38-39, 66, 88, 119
 zenaura\client\component.py      22      2    91%   24, 34
 zenaura\client\dom.py            50      2    96%   68, 71
 zenaura\client\tags.py          144      3    98%   9-11
 -----------------------------------------------------------
 ```
 
-- important note : test coverage must be kept at 95%
+- important note : test coverage must be kept at 95%
+
+# run example :
+
+cd to examples folder
+cd into example folder 
+run 
+```
+flask --app hello run
+```
```

### Comparing `zenaura-0.9.16a0/setup.py` & `zenaura-0.9.31/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='zenaura',
-    version='v0.9.16-a',
+    version='0.9.31',
     description="Zenaura, light weight, super fast python full-stack development framework, in which every line of code emit the aura of python zen, build interactive SPA with pure Python, create secure and scalable endpoints.",
     author="Ahmed Rakan",
     author_email="ar.aldhafeeri11@gmail.com",
     packages=['zenaura'],
     install_requires=[
         # Add any dependencies here
     ],
```

### Comparing `zenaura-0.9.16a0/tests/test_compiler.py` & `zenaura-0.9.31/tests/test_compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from zenaura.client.tags import Node, Child, Attribute
+from zenaura.client.tags import Node, Attribute
 from zenaura.client.compiler import Compiler
 import unittest
 
 compiler = Compiler() 
 
 class CompilerTests(unittest.TestCase):
     def test_compile_simple_node(self):
@@ -110,15 +110,15 @@
         grandchild3 = Node("img")
         grandchild3.attributes.append(Attribute("src", "image.jpg"))
         grandchild3.attributes.append(Attribute("alt", "Image"))
         grandchild1.children = ["Hello"]
         child1.children.extend([grandchild1, grandchild2, grandchild3])
         root.children.extend([child1, child2])
         result = compiler.compile(root, zenaura_dom_mode=False)
-        expected_output = '<div><div><span>Hello</span><a href="https://example.com">Link</a><img src="image.jpg" alt="Image"></img></div><div></div></div>'
+        expected_output = '<div><div><span>Hello</span><a href="https://example.com">Link</a><img src="image.jpg" alt="Image"></div><div></div></div>'
         self.assertEqual(result, expected_output)
 
 
     def test_compile_with_even_more_nested_structure(self):
         root = Node("div")
         child1 = Node("div")
         child2 = Node("div")
@@ -137,9 +137,9 @@
         greatGrandchild2 = Node("div")
         greatGrandchild3 = Node("div")
         greatGrandchild1.children.extend([greatGrandchild2, greatGrandchild3])
         grandchild2.children.extend([greatGrandchild1])
 
         result = compiler.compile(root, zenaura_dom_mode=False)
         
-        expected_output = '<div><div><span>Hello</span><a href="https://example.com">Link<div><div></div><div></div></div></a><img src="image.jpg" alt="Image"></img></div><div></div></div>'
+        expected_output = '<div><div><span>Hello</span><a href="https://example.com">Link<div><div></div><div></div></div></a><img src="image.jpg" alt="Image"></div><div></div></div>'
         self.assertEqual(result, expected_output)
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-from zenaura.client.tags import Node, Child, Attribute from
-zenaura.client.compiler import Compiler import unittest compiler = Compiler()
-class CompilerTests(unittest.TestCase): def test_compile_simple_node(self): elm
-= Node("div") result = compiler.compile(elm) self.assertEqual(result, "
+from zenaura.client.tags import Node, Attribute from zenaura.client.compiler
+import Compiler import unittest compiler = Compiler() class CompilerTests
+(unittest.TestCase): def test_compile_simple_node(self): elm = Node("div")
+result = compiler.compile(elm) self.assertEqual(result, "
 ") def test_compile_with_attributes(self): elm = Node("p") elm.children.append
 (Attribute("styles", "my-paragraph")) elm.children.append(Attribute("id",
 "main-content")) result = compiler.compile(elm, zenaura_dom_mode=False)
 self.assertEqual(result, '
 ') def test_compile_with_attributes(self): elm = Node("p")
 elm.attributes.append(Attribute("styles", "my-paragraph"))
 elm.attributes.append(Attribute("id", "main-content")) result =
```

### Comparing `zenaura-0.9.16a0/tests/test_component_e2e.py` & `zenaura-0.9.31/tests/test_component_e2e.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.16a0/tests/test_component_unit.py` & `zenaura-0.9.31/tests/test_component_unit.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.16a0/tests/test_observer.py` & `zenaura-0.9.31/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.16a0/tests/test_zenaura_dom.py` & `zenaura-0.9.31/tests/test_zenaura_dom.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.16a0/zenaura.egg-info/PKG-INFO` & `zenaura-0.9.31/zenaura.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.16a0
+Version: 0.9.31
 Summary: Zenaura, light weight, super fast python full-stack development framework, in which every line of code emit the aura of python zen, build interactive SPA with pure Python, create secure and scalable endpoints.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Zenaura 
@@ -41,7 +41,16 @@
 zenaura\client\component.py      22      2    91%   24, 34
 zenaura\client\dom.py            50      2    96%   68, 71
 zenaura\client\tags.py          144      3    98%   9-11
 -----------------------------------------------------------
 ```
 
 - important note : test coverage must be kept at 95%
+
+# run example :
+
+cd to examples folder
+cd into example folder 
+run 
+```
+flask --app hello run
+```
```

