# Comparing `tmp/webflask-0.5.tar.gz` & `tmp/webflask-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webflask-0.5.tar", last modified: Mon May 13 00:35:43 2024, max compression
+gzip compressed data, was "webflask-0.5.5.tar", last modified: Mon May 13 00:47:10 2024, max compression
```

## Comparing `webflask-0.5.tar` & `webflask-0.5.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 00:35:43.404773 webflask-0.5/
--rw-rw-rw-   0        0        0       53 2024-05-13 00:35:43.403413 webflask-0.5/PKG-INFO
--rw-rw-rw-   0        0        0      285 2024-05-12 14:04:29.000000 webflask-0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-13 00:35:43.404773 webflask-0.5/setup.cfg
--rw-rw-rw-   0        0        0      411 2024-05-13 00:35:40.000000 webflask-0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 00:35:43.382551 webflask-0.5/webflask/
--rw-rw-rw-   0        0        0        0 2024-05-12 15:16:13.000000 webflask-0.5/webflask/__init__.py
--rw-rw-rw-   0        0        0     3966 2024-05-06 15:34:58.000000 webflask-0.5/webflask/ajax.zip
--rw-rw-rw-   0        0        0  7982659 2024-05-12 16:34:09.000000 webflask-0.5/webflask/authorization.zip
--rw-rw-rw-   0        0        0     1282 2024-05-06 16:27:21.000000 webflask-0.5/webflask/cal.zip
--rw-rw-rw-   0        0        0      758 2024-05-12 15:45:15.000000 webflask-0.5/webflask/cssnbox.zip
--rw-rw-rw-   0        0        0      834 2024-05-12 15:16:24.000000 webflask-0.5/webflask/functions.py
--rw-rw-rw-   0        0        0     4236 2024-05-12 15:27:40.000000 webflask-0.5/webflask/one.html
--rw-rw-rw-   0        0        0      581 2024-05-13 00:35:11.000000 webflask-0.5/webflask/resume.txt
--rw-rw-rw-   0        0        0     1657 2024-05-12 15:27:51.000000 webflask-0.5/webflask/three.rb
--rw-rw-rw-   0        0        0      510 2024-05-13 00:34:50.000000 webflask-0.5/webflask/todo.txt
--rw-rw-rw-   0        0        0     1868 2024-05-12 15:27:44.000000 webflask-0.5/webflask/two.html
--rw-rw-rw-   0        0        0     1070 2024-05-13 00:35:12.000000 webflask-0.5/webflask/uploads.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 00:35:43.401404 webflask-0.5/webflask.egg-info/
--rw-rw-rw-   0        0        0       53 2024-05-13 00:35:43.000000 webflask-0.5/webflask.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2024-05-13 00:35:43.000000 webflask-0.5/webflask.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 00:35:43.000000 webflask-0.5/webflask.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-13 00:35:43.000000 webflask-0.5/webflask.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 00:47:10.566155 webflask-0.5.5/
+-rw-rw-rw-   0        0        0       55 2024-05-13 00:47:10.563145 webflask-0.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2024-05-12 14:04:29.000000 webflask-0.5.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-13 00:47:10.566155 webflask-0.5.5/setup.cfg
+-rw-rw-rw-   0        0        0      413 2024-05-13 00:46:59.000000 webflask-0.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 00:47:10.543101 webflask-0.5.5/webflask/
+-rw-rw-rw-   0        0        0        0 2024-05-12 15:16:13.000000 webflask-0.5.5/webflask/__init__.py
+-rw-rw-rw-   0        0        0     3966 2024-05-06 15:34:58.000000 webflask-0.5.5/webflask/ajax.zip
+-rw-rw-rw-   0        0        0  7982659 2024-05-12 16:34:09.000000 webflask-0.5.5/webflask/authorization.zip
+-rw-rw-rw-   0        0        0     1282 2024-05-06 16:27:21.000000 webflask-0.5.5/webflask/cal.zip
+-rw-rw-rw-   0        0        0      758 2024-05-12 15:45:15.000000 webflask-0.5.5/webflask/cssnbox.zip
+-rw-rw-rw-   0        0        0      834 2024-05-12 15:16:24.000000 webflask-0.5.5/webflask/functions.py
+-rw-rw-rw-   0        0        0     4236 2024-05-12 15:27:40.000000 webflask-0.5.5/webflask/one.html
+-rw-rw-rw-   0        0        0      581 2024-05-13 00:35:11.000000 webflask-0.5.5/webflask/resume.txt
+-rw-rw-rw-   0        0        0     1657 2024-05-12 15:27:51.000000 webflask-0.5.5/webflask/three.rb
+-rw-rw-rw-   0        0        0      510 2024-05-13 00:34:50.000000 webflask-0.5.5/webflask/todo.txt
+-rw-rw-rw-   0        0        0     2567 2024-05-13 00:46:42.000000 webflask-0.5.5/webflask/two.html
+-rw-rw-rw-   0        0        0     1070 2024-05-13 00:35:12.000000 webflask-0.5.5/webflask/uploads.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 00:47:10.561697 webflask-0.5.5/webflask.egg-info/
+-rw-rw-rw-   0        0        0       55 2024-05-13 00:47:10.000000 webflask-0.5.5/webflask.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2024-05-13 00:47:10.000000 webflask-0.5.5/webflask.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 00:47:10.000000 webflask-0.5.5/webflask.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-13 00:47:10.000000 webflask-0.5.5/webflask.egg-info/top_level.txt
```

### Comparing `webflask-0.5/webflask/ajax.zip` & `webflask-0.5.5/webflask/ajax.zip`

 * *Files identical despite different names*

### Comparing `webflask-0.5/webflask/authorization.zip` & `webflask-0.5.5/webflask/authorization.zip`

 * *Files identical despite different names*

### Comparing `webflask-0.5/webflask/cal.zip` & `webflask-0.5.5/webflask/cal.zip`

 * *Files identical despite different names*

### Comparing `webflask-0.5/webflask/cssnbox.zip` & `webflask-0.5.5/webflask/cssnbox.zip`

 * *Files identical despite different names*

### Comparing `webflask-0.5/webflask/functions.py` & `webflask-0.5.5/webflask/functions.py`

 * *Files identical despite different names*

### Comparing `webflask-0.5/webflask/one.html` & `webflask-0.5.5/webflask/one.html`

 * *Files identical despite different names*

### Comparing `webflask-0.5/webflask/resume.txt` & `webflask-0.5.5/webflask/resume.txt`

 * *Files identical despite different names*

### Comparing `webflask-0.5/webflask/three.rb` & `webflask-0.5.5/webflask/three.rb`

 * *Files identical despite different names*

### Comparing `webflask-0.5/webflask/uploads.txt` & `webflask-0.5.5/webflask/uploads.txt`

 * *Files identical despite different names*

