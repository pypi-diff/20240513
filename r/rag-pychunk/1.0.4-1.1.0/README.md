# Comparing `tmp/rag_pychunk-1.0.4.tar.gz` & `tmp/rag_pychunk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rag_pychunk-1.0.4.tar", last modified: Sat May 11 16:24:45 2024, max compression
+gzip compressed data, was "rag_pychunk-1.1.0.tar", last modified: Mon May 13 06:56:18 2024, max compression
```

## Comparing `rag_pychunk-1.0.4.tar` & `rag_pychunk-1.1.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-11 16:24:45.871025 rag_pychunk-1.0.4/
--rw-r--r--   0 Jaime      (502) staff       (20)     1076 2024-05-10 11:33:20.000000 rag_pychunk-1.0.4/LICENSE
--rw-r--r--   0 Jaime      (502) staff       (20)       17 2024-05-08 16:43:09.000000 rag_pychunk-1.0.4/MANIFEST.in
--rw-r--r--   0 Jaime      (502) staff       (20)     1404 2024-05-11 16:24:45.870597 rag_pychunk-1.0.4/PKG-INFO
-drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-11 16:24:45.867364 rag_pychunk-1.0.4/pychunk/
--rw-r--r--   0 Jaime      (502) staff       (20)        0 2024-05-09 06:52:18.000000 rag_pychunk-1.0.4/pychunk/__init__.py
-drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-11 16:24:45.867711 rag_pychunk-1.0.4/pychunk/chunkers/
--rw-r--r--   0 Jaime      (502) staff       (20)        0 2024-05-08 16:40:23.000000 rag_pychunk-1.0.4/pychunk/chunkers/__init__.py
--rw-r--r--   0 Jaime      (502) staff       (20)     3177 2024-05-11 16:22:57.000000 rag_pychunk-1.0.4/pychunk/chunkers/base.py
--rw-r--r--   0 Jaime      (502) staff       (20)     9616 2024-05-10 15:52:23.000000 rag_pychunk-1.0.4/pychunk/chunkers/python_chunker.py
-drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-11 16:24:45.868292 rag_pychunk-1.0.4/pychunk/nodes/
--rw-r--r--   0 Jaime      (502) staff       (20)        0 2024-05-08 16:47:25.000000 rag_pychunk-1.0.4/pychunk/nodes/__init__.py
--rw-r--r--   0 Jaime      (502) staff       (20)     4177 2024-05-11 15:33:13.000000 rag_pychunk-1.0.4/pychunk/nodes/base.py
--rw-r--r--   0 Jaime      (502) staff       (20)     3070 2024-05-10 08:23:09.000000 rag_pychunk-1.0.4/pychunk/nodes/nodes.py
--rw-r--r--   0 Jaime      (502) staff       (20)      780 2024-05-10 11:18:52.000000 rag_pychunk-1.0.4/pychunk/nodes/types.py
-drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-11 16:24:45.868691 rag_pychunk-1.0.4/pychunk/parser/
--rw-r--r--   0 Jaime      (502) staff       (20)        0 2024-05-11 15:34:39.000000 rag_pychunk-1.0.4/pychunk/parser/__init__.py
--rw-r--r--   0 Jaime      (502) staff       (20)     1511 2024-05-11 16:03:58.000000 rag_pychunk-1.0.4/pychunk/parser/langchain_parser.py
--rw-r--r--   0 Jaime      (502) staff       (20)     2169 2024-05-11 15:58:22.000000 rag_pychunk-1.0.4/pychunk/parser/llama_index_parser.py
-drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-11 16:24:45.869059 rag_pychunk-1.0.4/pychunk/utils/
--rw-r--r--   0 Jaime      (502) staff       (20)        0 2024-05-08 16:45:35.000000 rag_pychunk-1.0.4/pychunk/utils/__init__.py
--rw-r--r--   0 Jaime      (502) staff       (20)      543 2024-05-09 08:16:14.000000 rag_pychunk-1.0.4/pychunk/utils/files_handler.py
--rw-r--r--   0 Jaime      (502) staff       (20)     7991 2024-05-10 10:46:57.000000 rag_pychunk-1.0.4/pychunk/utils/nodes_utils.py
-drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-11 16:24:45.870290 rag_pychunk-1.0.4/rag_pychunk.egg-info/
--rw-r--r--   0 Jaime      (502) staff       (20)     1404 2024-05-11 16:24:45.000000 rag_pychunk-1.0.4/rag_pychunk.egg-info/PKG-INFO
--rw-r--r--   0 Jaime      (502) staff       (20)      702 2024-05-11 16:24:45.000000 rag_pychunk-1.0.4/rag_pychunk.egg-info/SOURCES.txt
--rw-r--r--   0 Jaime      (502) staff       (20)        1 2024-05-11 16:24:45.000000 rag_pychunk-1.0.4/rag_pychunk.egg-info/dependency_links.txt
--rw-r--r--   0 Jaime      (502) staff       (20)        8 2024-05-11 16:24:45.000000 rag_pychunk-1.0.4/rag_pychunk.egg-info/top_level.txt
-drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-11 16:24:45.866805 rag_pychunk-1.0.4/scripts/
-drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-11 16:24:45.870043 rag_pychunk-1.0.4/scripts/python-scripts/
--rwxr-xr-x   0 Jaime      (502) staff       (20)     5374 2024-05-10 10:54:57.000000 rag_pychunk-1.0.4/scripts/python-scripts/classify-python-code.sh
--rwxr-xr-x   0 Jaime      (502) staff       (20)      788 2024-05-10 10:12:20.000000 rag_pychunk-1.0.4/scripts/python-scripts/find-node-relationships.sh
--rwxr-xr-x   0 Jaime      (502) staff       (20)     7163 2024-05-10 14:27:25.000000 rag_pychunk-1.0.4/scripts/python-scripts/generate-node-metadata.sh
--rw-r--r--   0 Jaime      (502) staff       (20)       38 2024-05-11 16:24:45.871087 rag_pychunk-1.0.4/setup.cfg
--rw-r--r--   0 Jaime      (502) staff       (20)     1716 2024-05-11 16:24:22.000000 rag_pychunk-1.0.4/setup.py
+drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-13 06:56:18.319881 rag_pychunk-1.1.0/
+-rw-r--r--   0 Jaime      (502) staff       (20)     1076 2024-05-10 11:33:20.000000 rag_pychunk-1.1.0/LICENSE
+-rw-r--r--   0 Jaime      (502) staff       (20)       17 2024-05-08 16:43:09.000000 rag_pychunk-1.1.0/MANIFEST.in
+-rw-r--r--   0 Jaime      (502) staff       (20)     1404 2024-05-13 06:56:18.319505 rag_pychunk-1.1.0/PKG-INFO
+drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-13 06:56:18.315387 rag_pychunk-1.1.0/pychunk/
+-rw-r--r--   0 Jaime      (502) staff       (20)        0 2024-05-09 06:52:18.000000 rag_pychunk-1.1.0/pychunk/__init__.py
+drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-13 06:56:18.315863 rag_pychunk-1.1.0/pychunk/chunkers/
+-rw-r--r--   0 Jaime      (502) staff       (20)        0 2024-05-08 16:40:23.000000 rag_pychunk-1.1.0/pychunk/chunkers/__init__.py
+-rw-r--r--   0 Jaime      (502) staff       (20)     3177 2024-05-11 16:22:57.000000 rag_pychunk-1.1.0/pychunk/chunkers/base.py
+-rw-r--r--   0 Jaime      (502) staff       (20)     9821 2024-05-13 06:50:41.000000 rag_pychunk-1.1.0/pychunk/chunkers/python_chunker.py
+drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-13 06:56:18.316494 rag_pychunk-1.1.0/pychunk/nodes/
+-rw-r--r--   0 Jaime      (502) staff       (20)        0 2024-05-08 16:47:25.000000 rag_pychunk-1.1.0/pychunk/nodes/__init__.py
+-rw-r--r--   0 Jaime      (502) staff       (20)     4177 2024-05-11 15:33:13.000000 rag_pychunk-1.1.0/pychunk/nodes/base.py
+-rw-r--r--   0 Jaime      (502) staff       (20)     3070 2024-05-10 08:23:09.000000 rag_pychunk-1.1.0/pychunk/nodes/nodes.py
+-rw-r--r--   0 Jaime      (502) staff       (20)      780 2024-05-10 11:18:52.000000 rag_pychunk-1.1.0/pychunk/nodes/types.py
+drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-13 06:56:18.316902 rag_pychunk-1.1.0/pychunk/parser/
+-rw-r--r--   0 Jaime      (502) staff       (20)        0 2024-05-11 15:34:39.000000 rag_pychunk-1.1.0/pychunk/parser/__init__.py
+-rw-r--r--   0 Jaime      (502) staff       (20)     1511 2024-05-11 16:03:58.000000 rag_pychunk-1.1.0/pychunk/parser/langchain_parser.py
+-rw-r--r--   0 Jaime      (502) staff       (20)     2169 2024-05-11 15:58:22.000000 rag_pychunk-1.1.0/pychunk/parser/llama_index_parser.py
+drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-13 06:56:18.317547 rag_pychunk-1.1.0/pychunk/utils/
+-rw-r--r--   0 Jaime      (502) staff       (20)        0 2024-05-08 16:45:35.000000 rag_pychunk-1.1.0/pychunk/utils/__init__.py
+-rw-r--r--   0 Jaime      (502) staff       (20)      543 2024-05-09 08:16:14.000000 rag_pychunk-1.1.0/pychunk/utils/files_handler.py
+-rw-r--r--   0 Jaime      (502) staff       (20)     8717 2024-05-13 06:55:37.000000 rag_pychunk-1.1.0/pychunk/utils/nodes_utils.py
+drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-13 06:56:18.319195 rag_pychunk-1.1.0/rag_pychunk.egg-info/
+-rw-r--r--   0 Jaime      (502) staff       (20)     1404 2024-05-13 06:56:18.000000 rag_pychunk-1.1.0/rag_pychunk.egg-info/PKG-INFO
+-rw-r--r--   0 Jaime      (502) staff       (20)      702 2024-05-13 06:56:18.000000 rag_pychunk-1.1.0/rag_pychunk.egg-info/SOURCES.txt
+-rw-r--r--   0 Jaime      (502) staff       (20)        1 2024-05-13 06:56:18.000000 rag_pychunk-1.1.0/rag_pychunk.egg-info/dependency_links.txt
+-rw-r--r--   0 Jaime      (502) staff       (20)        8 2024-05-13 06:56:18.000000 rag_pychunk-1.1.0/rag_pychunk.egg-info/top_level.txt
+drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-13 06:56:18.314744 rag_pychunk-1.1.0/scripts/
+drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-13 06:56:18.318924 rag_pychunk-1.1.0/scripts/python-scripts/
+-rwxr-xr-x   0 Jaime      (502) staff       (20)     5374 2024-05-10 10:54:57.000000 rag_pychunk-1.1.0/scripts/python-scripts/classify-python-code.sh
+-rwxr-xr-x   0 Jaime      (502) staff       (20)      788 2024-05-10 10:12:20.000000 rag_pychunk-1.1.0/scripts/python-scripts/find-node-relationships.sh
+-rwxr-xr-x   0 Jaime      (502) staff       (20)     7163 2024-05-10 14:27:25.000000 rag_pychunk-1.1.0/scripts/python-scripts/generate-node-metadata.sh
+-rw-r--r--   0 Jaime      (502) staff       (20)       38 2024-05-13 06:56:18.319941 rag_pychunk-1.1.0/setup.cfg
+-rw-r--r--   0 Jaime      (502) staff       (20)     1716 2024-05-13 06:53:50.000000 rag_pychunk-1.1.0/setup.py
```

### Comparing `rag_pychunk-1.0.4/LICENSE` & `rag_pychunk-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rag_pychunk-1.0.4/PKG-INFO` & `rag_pychunk-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rag-pychunk
-Version: 1.0.4
+Version: 1.1.0
 Summary: Improve your RAG pipelines for your python repositories.
 Author: Jaime Sancho Molero
 Author-email: jimysanchomolero@gmail.com
 License-File: LICENSE
 
 
     It leverages the python programming language syntax to improve:
```

### Comparing `rag_pychunk-1.0.4/pychunk/chunkers/base.py` & `rag_pychunk-1.1.0/pychunk/chunkers/base.py`

 * *Files identical despite different names*

### Comparing `rag_pychunk-1.0.4/pychunk/chunkers/python_chunker.py` & `rag_pychunk-1.1.0/pychunk/chunkers/python_chunker.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,18 +25,22 @@
         NodeType.MODULE: ModuleNode
     }
     
     _not_valid_relationships_to_look_pattern = r"^__[^_]*__$"
     
     def __init__(self, files_path: str | List[str], hash_function: Optional[Callable] | None = None):
         super(PythonChunker, self).__init__(files_path=files_path, hash_function=hash_function)
+        _venv_folder = self._find_venv()
+        if _venv_folder is None:
+            raise FileNotFoundError(f"Could not find .venv folder. Maybe you are too far from it or have not create it?")
+        
+        self.__bin_folder = os.path.join(self._find_venv(), "bin")
         
     def _create_nodes_of_file(self, file_path: str) -> Dict[str, Type['BaseNode']]:
         
-        self.__bin_folder = os.path.join(self._find_venv(), "bin")
         tmp_folder = self._file_handler.tmp_folder
         if file_path.startswith("."): file_path = file_path[2:]
         elif file_path.startswith(".."): file_path = file_path[3:]
         file_name = file_path.replace("/", "_").split(".")[0]
         # command = f"./pychunk/scripts/python-scripts/generate-node-metadata.sh {file_path} {tmp_folder}/{file_name}_info.txt > {tmp_folder}/{file_name}_final.txt 2> /dev/null"
         command = f"{self.__bin_folder}/generate-node-metadata.sh {file_path} {tmp_folder}/{file_name}_info.txt > {tmp_folder}/{file_name}_final.txt 2> /dev/null"
         subprocess.run(["bash", "-c", command])
```

### Comparing `rag_pychunk-1.0.4/pychunk/nodes/base.py` & `rag_pychunk-1.1.0/pychunk/nodes/base.py`

 * *Files identical despite different names*

### Comparing `rag_pychunk-1.0.4/pychunk/nodes/nodes.py` & `rag_pychunk-1.1.0/pychunk/nodes/nodes.py`

 * *Files identical despite different names*

### Comparing `rag_pychunk-1.0.4/pychunk/nodes/types.py` & `rag_pychunk-1.1.0/pychunk/nodes/types.py`

 * *Files identical despite different names*

### Comparing `rag_pychunk-1.0.4/pychunk/parser/langchain_parser.py` & `rag_pychunk-1.1.0/pychunk/parser/langchain_parser.py`

 * *Files identical despite different names*

### Comparing `rag_pychunk-1.0.4/pychunk/parser/llama_index_parser.py` & `rag_pychunk-1.1.0/pychunk/parser/llama_index_parser.py`

 * *Files identical despite different names*

### Comparing `rag_pychunk-1.0.4/pychunk/utils/files_handler.py` & `rag_pychunk-1.1.0/pychunk/utils/files_handler.py`

 * *Files identical despite different names*

### Comparing `rag_pychunk-1.0.4/pychunk/utils/nodes_utils.py` & `rag_pychunk-1.1.0/pychunk/utils/nodes_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -91,51 +91,69 @@
                             
             metadata = class_metadata.split(":")[-1].split("-")[0]
             del class_text[0]
             class_content = "".join(class_text)
             class_text = None 
             end_class_line = True 
             begin_class_line = False 
-            yield class_content, (int(begin_line), int(end_line)), class_name, None, NodeType.CLASS, metadata
+            try:
+                yield class_content, (int(begin_line), int(end_line)), class_name, None, NodeType.CLASS, metadata
+            except:
+                yield class_content, None, class_name, None, NodeType.CLASS, metadata
                             
         elif line.startswith(Delimiter.function_delimiter[Pointer.end]) and isinstance(function_text, list):
 
             end_function_line = True 
             begin_function_line = False 
             function_metadata = function_text[0]
             metadata = function_text[0].split("Arguments:")[-1].split("-")[0]
             function_name = line.split("FUNCTION:")[-1].replace(" ", "")[:-3]
-            begin_line, end_line = function_metadata.split("-")[-1].split(",")
+            try:
+                begin_line, end_line = function_metadata.split("-")[-1].split(",")
+            except Exception as e:
+                begin_line, end_line = None, None
+                
             if not len(end_line.strip()): end_line = int(begin_line) + 1
             del function_text[0]
             function_content = "".join(function_text)
             function_text = None 
-            yield (function_content, 
-                  (int(begin_line), 
-                   int(end_line)), 
-                   None, 
-                   function_name, 
-                   NodeType.FUNCTION, 
-                   metadata)
+            try:
+                yield (function_content, 
+                    (int(begin_line), 
+                    int(end_line)), 
+                    None, 
+                    function_name, 
+                    NodeType.FUNCTION, 
+                    metadata)
+            except Exception as e:
+                yield (function_content, None, None, function_name, NodeType.FUNCTION, metadata)
             
         elif line.startswith(Delimiter.free_code_delimiter[Pointer.end]) and isinstance(free_code, list):
             end_free_code = True 
             begin_free_code = False 
             code_metadata = free_code[0]
-            begin_line, end_line = code_metadata.split(":")[-1].split(",")
+            try:
+                begin_line, end_line = code_metadata.split(":")[-1].split(",")
+            except Exception as e:
+                begin_line = None
+                end_line = None
+                
             del free_code[0]
             code_content = "".join(free_code)
             free_code = None 
-            yield (code_content, 
-                  (int(begin_line), 
-                   int(end_line)), 
-                   None, 
-                   None, 
-                   NodeType.CODE, 
-                   None)
+            try:
+                yield (code_content, 
+                    (int(begin_line), 
+                    int(end_line)), 
+                    None, 
+                    None, 
+                    NodeType.CODE, 
+                    None)
+            except Exception as e:
+                yield (code_content, None, None, None, NodeType.CODE, None)
             
         if isinstance(modules_text, list):
             if begin_module_line: 
                 begin_module_line = False 
                 continue
             if end_module_line:
                 continue
@@ -196,15 +214,15 @@
                       (int(begin_line), 
                        int(end_line)), 
                        class_name, 
                        method_name, 
                        NodeType.METHOD, 
                        metadata)
             except Exception as e:
-                yield (None, None, None, None, None, None)
+                yield (method_content, None, class_name, method_name, NodeType.METHOD, metadata)
             
         if isinstance(method_text, list):
             if begin_method_line: 
                 begin_method_line = False 
                 continue
             if end_method_line:
                 continue
```

### Comparing `rag_pychunk-1.0.4/rag_pychunk.egg-info/PKG-INFO` & `rag_pychunk-1.1.0/rag_pychunk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rag-pychunk
-Version: 1.0.4
+Version: 1.1.0
 Summary: Improve your RAG pipelines for your python repositories.
 Author: Jaime Sancho Molero
 Author-email: jimysanchomolero@gmail.com
 License-File: LICENSE
 
 
     It leverages the python programming language syntax to improve:
```

### Comparing `rag_pychunk-1.0.4/rag_pychunk.egg-info/SOURCES.txt` & `rag_pychunk-1.1.0/rag_pychunk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rag_pychunk-1.0.4/scripts/python-scripts/classify-python-code.sh` & `rag_pychunk-1.1.0/scripts/python-scripts/classify-python-code.sh`

 * *Files identical despite different names*

### Comparing `rag_pychunk-1.0.4/scripts/python-scripts/find-node-relationships.sh` & `rag_pychunk-1.1.0/scripts/python-scripts/find-node-relationships.sh`

 * *Files identical despite different names*

### Comparing `rag_pychunk-1.0.4/scripts/python-scripts/generate-node-metadata.sh` & `rag_pychunk-1.1.0/scripts/python-scripts/generate-node-metadata.sh`

 * *Files identical despite different names*

### Comparing `rag_pychunk-1.0.4/setup.py` & `rag_pychunk-1.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='rag-pychunk',
-    version='1.0.4',
+    version='1.1.0',
     packages=find_packages(),
     scripts=['scripts/python-scripts/classify-python-code.sh', 
              'scripts/python-scripts/find-node-relationships.sh', 
              'scripts/python-scripts/generate-node-metadata.sh'],
     author="Jaime Sancho Molero", 
     author_email="jimysanchomolero@gmail.com", 
     description="Improve your RAG pipelines for your python repositories.",
```

