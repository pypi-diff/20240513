# Comparing `tmp/article-parser-1.7.0.tar.gz` & `tmp/article-parser-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/article-parser-1.7.0.tar", last modified: Tue Feb 20 02:51:00 2024, max compression
+gzip compressed data, was "dist/article-parser-1.7.1.tar", last modified: Fri Mar 29 08:05:09 2024, max compression
```

## Comparing `article-parser-1.7.0.tar` & `article-parser-1.7.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 02:51:00.000000 article-parser-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-02-20 02:51:00.000000 article-parser-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-02-20 02:50:44.000000 article-parser-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 02:51:00.000000 article-parser-1.7.0/article_parser/
--rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-02-20 02:50:44.000000 article-parser-1.7.0/article_parser/Extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-02-20 02:50:44.000000 article-parser-1.7.0/article_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 02:51:00.000000 article-parser-1.7.0/article_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-02-20 02:51:00.000000 article-parser-1.7.0/article_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-02-20 02:51:00.000000 article-parser-1.7.0/article_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 02:51:00.000000 article-parser-1.7.0/article_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-20 02:51:00.000000 article-parser-1.7.0/article_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-20 02:51:00.000000 article-parser-1.7.0/article_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 02:51:00.000000 article-parser-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-02-20 02:50:44.000000 article-parser-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 02:51:00.000000 article-parser-1.7.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-02-20 02:50:44.000000 article-parser-1.7.0/test/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:05:09.000000 article-parser-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-03-29 08:05:09.000000 article-parser-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-03-29 08:04:50.000000 article-parser-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:05:09.000000 article-parser-1.7.1/article_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-03-29 08:04:50.000000 article-parser-1.7.1/article_parser/Extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-29 08:04:50.000000 article-parser-1.7.1/article_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:05:09.000000 article-parser-1.7.1/article_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-03-29 08:05:09.000000 article-parser-1.7.1/article_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-29 08:05:09.000000 article-parser-1.7.1/article_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 08:05:09.000000 article-parser-1.7.1/article_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-29 08:05:09.000000 article-parser-1.7.1/article_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-29 08:05:09.000000 article-parser-1.7.1/article_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 08:05:09.000000 article-parser-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-03-29 08:04:50.000000 article-parser-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:05:09.000000 article-parser-1.7.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-29 08:04:50.000000 article-parser-1.7.1/test/test_parser.py
```

### Comparing `article-parser-1.7.0/PKG-INFO` & `article-parser-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: article-parser
-Version: 1.7.0
+Version: 1.7.1
 Summary: A parser to parse article from url or html
 Home-page: https://github.com/myifeng/article-parser
 Author: myifeng
 Author-email: myifengs@gmail.com
 Maintainer: myifeng
 Maintainer-email: myifengs@gmail.com
 License: MIT
```

### Comparing `article-parser-1.7.0/README.md` & `article-parser-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `article-parser-1.7.0/article_parser/Extractor.py` & `article-parser-1.7.1/article_parser/Extractor.py`

 * *Files identical despite different names*

### Comparing `article-parser-1.7.0/article_parser/__init__.py` & `article-parser-1.7.1/article_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `article-parser-1.7.0/article_parser.egg-info/PKG-INFO` & `article-parser-1.7.1/article_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: article-parser
-Version: 1.7.0
+Version: 1.7.1
 Summary: A parser to parse article from url or html
 Home-page: https://github.com/myifeng/article-parser
 Author: myifeng
 Author-email: myifengs@gmail.com
 Maintainer: myifeng
 Maintainer-email: myifengs@gmail.com
 License: MIT
```

### Comparing `article-parser-1.7.0/setup.py` & `article-parser-1.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,9 +38,9 @@
     python_requires='>=3.7',
     version_config={
         "template": "{tag}",
         "dirty_template": "{tag}",
         "dev_template": "{tag}"
     },
     setup_requires=["setuptools-git-versioning"],
-    install_requires = ['beautifulsoup4==4.12.3', 'html2text==2020.1.16', 'requests==2.31.0', 'lxml==5.1.0']
+    install_requires = ['beautifulsoup4==4.12.3', 'html2text==2020.1.16', 'requests==2.31.0', 'lxml==5.1.1']
 )
```

### Comparing `article-parser-1.7.0/test/test_parser.py` & `article-parser-1.7.1/test/test_parser.py`

 * *Files identical despite different names*

