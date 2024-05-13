# Comparing `tmp/visualgo-2024.2.4.tar.gz` & `tmp/visualgo-2024.5.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visualgo-2024.2.4.tar", last modified: Sun Feb  4 12:10:32 2024, max compression
+gzip compressed data, was "visualgo-2024.5.13.tar", last modified: Mon May 13 20:19:07 2024, max compression
```

## Comparing `visualgo-2024.2.4.tar` & `visualgo-2024.5.13.tar`

### file list

```diff
@@ -1,18 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 12:10:32.778827 visualgo-2024.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-02-04 12:10:22.000000 visualgo-2024.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-04 12:10:22.000000 visualgo-2024.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-02-04 12:10:32.778827 visualgo-2024.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-04 12:10:22.000000 visualgo-2024.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-02-04 12:10:22.000000 visualgo-2024.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-04 12:10:32.778827 visualgo-2024.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-04 12:10:22.000000 visualgo-2024.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 12:10:32.774827 visualgo-2024.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 12:10:32.778827 visualgo-2024.2.4/src/visualgo/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-04 12:10:22.000000 visualgo-2024.2.4/src/visualgo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-04 12:10:22.000000 visualgo-2024.2.4/src/visualgo/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 12:10:32.778827 visualgo-2024.2.4/src/visualgo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-02-04 12:10:32.000000 visualgo-2024.2.4/src/visualgo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-02-04 12:10:32.000000 visualgo-2024.2.4/src/visualgo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-04 12:10:32.000000 visualgo-2024.2.4/src/visualgo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-04 12:10:32.000000 visualgo-2024.2.4/src/visualgo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-04 12:10:32.000000 visualgo-2024.2.4/src/visualgo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:07.530128 visualgo-2024.5.13/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-13 20:19:01.000000 visualgo-2024.5.13/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-13 20:19:01.000000 visualgo-2024.5.13/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-13 20:19:07.530128 visualgo-2024.5.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-13 20:19:01.000000 visualgo-2024.5.13/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-13 20:19:01.000000 visualgo-2024.5.13/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 20:19:07.530128 visualgo-2024.5.13/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-13 20:19:01.000000 visualgo-2024.5.13/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:07.518128 visualgo-2024.5.13/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:07.522128 visualgo-2024.5.13/src/visualgo/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:07.522128 visualgo-2024.5.13/src/visualgo/logic/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24875 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/controller_callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:07.522128 visualgo-2024.5.13/src/visualgo/logic/debugger/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/debugger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:07.522128 visualgo-2024.5.13/src/visualgo/logic/debugger/__private/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/debugger/__private/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/debugger/__private/bdb_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:07.522128 visualgo-2024.5.13/src/visualgo/logic/debugger/__private/comm_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/debugger/__private/comm_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/debugger/__private/comm_api/from_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/debugger/__private/comm_api/to_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:07.526128 visualgo-2024.5.13/src/visualgo/logic/debugger/__private/comm_impl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/debugger/__private/comm_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/debugger/__private/comm_impl/python_process_from_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/debugger/__private/comm_impl/python_process_to_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/debugger/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/debugger/py_debugger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/debugger/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:07.526128 visualgo-2024.5.13/src/visualgo/logic/static/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/static/static_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/static/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:07.526128 visualgo-2024.5.13/src/visualgo/logic/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/ui/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/ui/ui_callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:07.526128 visualgo-2024.5.13/src/visualgo/structures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/Array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/BinaryTreeNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/BinaryTreeNodeBack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8083 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/DoublyLinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/Graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/LinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/List.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/Node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/Queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/Set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/Stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/Tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/TreeNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/TwoWayNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:07.530128 visualgo-2024.5.13/src/visualgo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-13 20:19:07.000000 visualgo-2024.5.13/src/visualgo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-13 20:19:07.000000 visualgo-2024.5.13/src/visualgo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:19:07.000000 visualgo-2024.5.13/src/visualgo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-13 20:19:07.000000 visualgo-2024.5.13/src/visualgo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-13 20:19:07.000000 visualgo-2024.5.13/src/visualgo.egg-info/top_level.txt
```

### Comparing `visualgo-2024.2.4/PKG-INFO` & `visualgo-2024.5.13/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,47 @@
 Metadata-Version: 2.1
 Name: visualgo
-Version: 2024.2.4
-Summary: Enjoy classic datatype and run python code
+Version: 2024.5.13
+Summary: Enjoy classic datatypes and debug user python code
 Author: PFA-Visualgo
-License: 
+License: MIT License
         
-        Copyright 2024 PFA-Visualgo
+        Copyright (c) 2024 PFA-Visualgo
         
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
         
-        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
         
-        THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
         
-Project-URL: Homepage, https://github.com/PFA-Visualgo/Visualgo
-Project-URL: Issues, https://github.com/PFA-Visualgo/Visualgo/issues
+Project-URL: Homepage, https://github.com/PFA-Visualgo/Visualgo-PyPI
+Project-URL: Issues, https://github.com/PFA-Visualgo/Visualgo-PyPI/issues
 Keywords: visualgo,structure,types,debugger
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
 
-# Visualgo
-A PFA project from 2023-2024 students of ENSEIRB-MATMECA.
+# Visualgo-PyPI
+This repository contains the main logic for debugging and custom types with python. This can be used by a visualisation as it is the case in the repository 'Visualgo' for example.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `visualgo-2024.2.4/src/visualgo.egg-info/PKG-INFO` & `visualgo-2024.5.13/src/visualgo.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,47 @@
 Metadata-Version: 2.1
 Name: visualgo
-Version: 2024.2.4
-Summary: Enjoy classic datatype and run python code
+Version: 2024.5.13
+Summary: Enjoy classic datatypes and debug user python code
 Author: PFA-Visualgo
-License: 
+License: MIT License
         
-        Copyright 2024 PFA-Visualgo
+        Copyright (c) 2024 PFA-Visualgo
         
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
         
-        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
         
-        THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
         
-Project-URL: Homepage, https://github.com/PFA-Visualgo/Visualgo
-Project-URL: Issues, https://github.com/PFA-Visualgo/Visualgo/issues
+Project-URL: Homepage, https://github.com/PFA-Visualgo/Visualgo-PyPI
+Project-URL: Issues, https://github.com/PFA-Visualgo/Visualgo-PyPI/issues
 Keywords: visualgo,structure,types,debugger
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
 
-# Visualgo
-A PFA project from 2023-2024 students of ENSEIRB-MATMECA.
+# Visualgo-PyPI
+This repository contains the main logic for debugging and custom types with python. This can be used by a visualisation as it is the case in the repository 'Visualgo' for example.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

