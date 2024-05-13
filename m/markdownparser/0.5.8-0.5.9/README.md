# Comparing `tmp/markdownparser-0.5.8.tar.gz` & `tmp/markdownparser-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdownparser-0.5.8.tar", max compression
+gzip compressed data, was "markdownparser-0.5.9.tar", max compression
```

## Comparing `markdownparser-0.5.8.tar` & `markdownparser-0.5.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 markdownparser-0.5.8/LICENSE
--rw-r--r--   0        0        0      123 2023-07-29 05:45:52.175866 markdownparser-0.5.8/MarkdownParser/__init__.py
--rw-r--r--   0        0        0     5969 2023-07-29 05:13:27.554441 markdownparser-0.5.8/MarkdownParser/base_class.py
--rw-r--r--   0        0        0    24841 2023-08-01 01:26:27.149482 markdownparser-0.5.8/MarkdownParser/block_parser.py
--rw-r--r--   0        0        0     7072 2023-07-29 05:12:59.301866 markdownparser-0.5.8/MarkdownParser/core.py
--rw-r--r--   0        0        0     3285 2023-07-29 04:08:11.133670 markdownparser-0.5.8/MarkdownParser/preprocess_parser.py
--rw-r--r--   0        0        0    21736 2023-07-29 04:08:19.718060 markdownparser-0.5.8/MarkdownParser/tree_parser.py
--rw-r--r--   0        0        0      442 2023-08-01 01:27:20.327866 markdownparser-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     4862 2023-07-30 04:45:57.984577 markdownparser-0.5.8/README.md
--rw-r--r--   0        0        0     5635 1970-01-01 00:00:00.000000 markdownparser-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 markdownparser-0.5.9/LICENSE
+-rw-r--r--   0        0        0      123 2023-07-29 05:45:52.175866 markdownparser-0.5.9/MarkdownParser/__init__.py
+-rw-r--r--   0        0        0     5969 2023-07-29 05:13:27.554441 markdownparser-0.5.9/MarkdownParser/base_class.py
+-rw-r--r--   0        0        0    24841 2023-08-01 08:01:42.436211 markdownparser-0.5.9/MarkdownParser/block_parser.py
+-rw-r--r--   0        0        0     7072 2023-07-29 05:12:59.301866 markdownparser-0.5.9/MarkdownParser/core.py
+-rw-r--r--   0        0        0     3285 2023-07-29 04:08:11.133670 markdownparser-0.5.9/MarkdownParser/preprocess_parser.py
+-rw-r--r--   0        0        0    21736 2023-07-29 04:08:19.718060 markdownparser-0.5.9/MarkdownParser/tree_parser.py
+-rw-r--r--   0        0        0      442 2023-08-01 08:02:17.441626 markdownparser-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     4862 2023-07-30 04:45:57.984577 markdownparser-0.5.9/README.md
+-rw-r--r--   0        0        0     5635 1970-01-01 00:00:00.000000 markdownparser-0.5.9/PKG-INFO
```

### Comparing `markdownparser-0.5.8/LICENSE` & `markdownparser-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.8/MarkdownParser/base_class.py` & `markdownparser-0.5.9/MarkdownParser/base_class.py`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.8/MarkdownParser/block_parser.py` & `markdownparser-0.5.9/MarkdownParser/block_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -593,17 +593,17 @@
     # 处理特殊字符
     # 不考虑 * 的多级嵌套
 
     def __init__(self) -> None:
         super().__init__()
         self.RE = re.compile(
             r"""(
-            \*{3}[^ ](.+?)[^ ]\*{3}|                           # 粗体+斜体
-            \*{2}[^ ](.+?)[^ ]\*{2}|                           # 粗体
-            \*[^ ](.+?)[^ ]\*|                                 # 斜体
+            \*{3}([^ ].+?[^ ])\*{3}|                           # 粗体+斜体
+            \*{2}([^ ].+?[^ ])\*{2}|                           # 粗体
+            \*([^ ].+?[^ ])\*|                                 # 斜体
             ~~(.+?)~~|                                 # 删除线
             ``(.+?)``|                                 # 高亮
             `(.+?)`                                    # 高亮
         )""",
             re.VERBOSE,
         )
         self.groupid_tag = {
```

### Comparing `markdownparser-0.5.8/MarkdownParser/core.py` & `markdownparser-0.5.9/MarkdownParser/core.py`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.8/MarkdownParser/preprocess_parser.py` & `markdownparser-0.5.9/MarkdownParser/preprocess_parser.py`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.8/MarkdownParser/tree_parser.py` & `markdownparser-0.5.9/MarkdownParser/tree_parser.py`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.8/README.md` & `markdownparser-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.8/PKG-INFO` & `markdownparser-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdownparser
-Version: 0.5.8
+Version: 0.5.9
 Summary: 
 Home-page: https://github.com/luzhixing12345/MarkdownParser
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

