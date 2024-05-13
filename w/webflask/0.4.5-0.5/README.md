# Comparing `tmp/webflask-0.4.5.tar.gz` & `tmp/webflask-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webflask-0.4.5.tar", last modified: Sun May 12 17:15:24 2024, max compression
+gzip compressed data, was "webflask-0.5.tar", last modified: Mon May 13 00:35:43 2024, max compression
```

## Comparing `webflask-0.4.5.tar` & `webflask-0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 17:15:24.106796 webflask-0.4.5/
--rw-rw-rw-   0        0        0       55 2024-05-12 17:15:24.103360 webflask-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0      285 2024-05-12 14:04:29.000000 webflask-0.4.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-12 17:15:24.106796 webflask-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0      413 2024-05-12 17:13:11.000000 webflask-0.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 17:15:24.080565 webflask-0.4.5/webflask/
--rw-rw-rw-   0        0        0        0 2024-05-12 15:16:13.000000 webflask-0.4.5/webflask/__init__.py
--rw-rw-rw-   0        0        0     3966 2024-05-06 15:34:58.000000 webflask-0.4.5/webflask/ajax.zip
--rw-rw-rw-   0        0        0  7982659 2024-05-12 16:34:09.000000 webflask-0.4.5/webflask/authorization.zip
--rw-rw-rw-   0        0        0     1282 2024-05-06 16:27:21.000000 webflask-0.4.5/webflask/cal.zip
--rw-rw-rw-   0        0        0      758 2024-05-12 15:45:15.000000 webflask-0.4.5/webflask/cssnbox.zip
--rw-rw-rw-   0        0        0      834 2024-05-12 15:16:24.000000 webflask-0.4.5/webflask/functions.py
--rw-rw-rw-   0        0        0     4236 2024-05-12 15:27:40.000000 webflask-0.4.5/webflask/one.html
--rw-rw-rw-   0        0        0      570 2024-05-12 17:00:33.000000 webflask-0.4.5/webflask/resume.txt
--rw-rw-rw-   0        0        0     1657 2024-05-12 15:27:51.000000 webflask-0.4.5/webflask/three.rb
--rw-rw-rw-   0        0        0      499 2024-05-12 16:59:48.000000 webflask-0.4.5/webflask/todo.txt
--rw-rw-rw-   0        0        0     1868 2024-05-12 15:27:44.000000 webflask-0.4.5/webflask/two.html
--rw-rw-rw-   0        0        0     1059 2024-05-12 17:12:52.000000 webflask-0.4.5/webflask/uploads.txt
-drwxrwxrwx   0        0        0        0 2024-05-12 17:15:24.101359 webflask-0.4.5/webflask.egg-info/
--rw-rw-rw-   0        0        0       55 2024-05-12 17:15:23.000000 webflask-0.4.5/webflask.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2024-05-12 17:15:23.000000 webflask-0.4.5/webflask.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 17:15:23.000000 webflask-0.4.5/webflask.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-12 17:15:23.000000 webflask-0.4.5/webflask.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 00:35:43.404773 webflask-0.5/
+-rw-rw-rw-   0        0        0       53 2024-05-13 00:35:43.403413 webflask-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2024-05-12 14:04:29.000000 webflask-0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-13 00:35:43.404773 webflask-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      411 2024-05-13 00:35:40.000000 webflask-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 00:35:43.382551 webflask-0.5/webflask/
+-rw-rw-rw-   0        0        0        0 2024-05-12 15:16:13.000000 webflask-0.5/webflask/__init__.py
+-rw-rw-rw-   0        0        0     3966 2024-05-06 15:34:58.000000 webflask-0.5/webflask/ajax.zip
+-rw-rw-rw-   0        0        0  7982659 2024-05-12 16:34:09.000000 webflask-0.5/webflask/authorization.zip
+-rw-rw-rw-   0        0        0     1282 2024-05-06 16:27:21.000000 webflask-0.5/webflask/cal.zip
+-rw-rw-rw-   0        0        0      758 2024-05-12 15:45:15.000000 webflask-0.5/webflask/cssnbox.zip
+-rw-rw-rw-   0        0        0      834 2024-05-12 15:16:24.000000 webflask-0.5/webflask/functions.py
+-rw-rw-rw-   0        0        0     4236 2024-05-12 15:27:40.000000 webflask-0.5/webflask/one.html
+-rw-rw-rw-   0        0        0      581 2024-05-13 00:35:11.000000 webflask-0.5/webflask/resume.txt
+-rw-rw-rw-   0        0        0     1657 2024-05-12 15:27:51.000000 webflask-0.5/webflask/three.rb
+-rw-rw-rw-   0        0        0      510 2024-05-13 00:34:50.000000 webflask-0.5/webflask/todo.txt
+-rw-rw-rw-   0        0        0     1868 2024-05-12 15:27:44.000000 webflask-0.5/webflask/two.html
+-rw-rw-rw-   0        0        0     1070 2024-05-13 00:35:12.000000 webflask-0.5/webflask/uploads.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 00:35:43.401404 webflask-0.5/webflask.egg-info/
+-rw-rw-rw-   0        0        0       53 2024-05-13 00:35:43.000000 webflask-0.5/webflask.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2024-05-13 00:35:43.000000 webflask-0.5/webflask.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 00:35:43.000000 webflask-0.5/webflask.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-13 00:35:43.000000 webflask-0.5/webflask.egg-info/top_level.txt
```

### Comparing `webflask-0.4.5/webflask/ajax.zip` & `webflask-0.5/webflask/ajax.zip`

 * *Files identical despite different names*

### Comparing `webflask-0.4.5/webflask/authorization.zip` & `webflask-0.5/webflask/authorization.zip`

 * *Files identical despite different names*

### Comparing `webflask-0.4.5/webflask/cal.zip` & `webflask-0.5/webflask/cal.zip`

 * *Files identical despite different names*

### Comparing `webflask-0.4.5/webflask/cssnbox.zip` & `webflask-0.5/webflask/cssnbox.zip`

 * *Files identical despite different names*

### Comparing `webflask-0.4.5/webflask/functions.py` & `webflask-0.5/webflask/functions.py`

 * *Files identical despite different names*

### Comparing `webflask-0.4.5/webflask/one.html` & `webflask-0.5/webflask/one.html`

 * *Files identical despite different names*

### Comparing `webflask-0.4.5/webflask/resume.txt` & `webflask-0.5/webflask/resume.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Step 1: create a new Rails application 
-    rails new resume 
+    rails new resume --skip-git 
     cd resume
 Step 2: Generate a scaffold for the To-Do model. 
     rails generate scaffold Resume name:string email:string phone:string summary:text education:text experience:text skills:text  
 Step 3: Run the migration to create the database table 
     rails db:migrate 
 Step 4: Under config/routes.rb change
     #root 'posts#index' to 'resumes#index'
```

### Comparing `webflask-0.4.5/webflask/three.rb` & `webflask-0.5/webflask/three.rb`

 * *Files identical despite different names*

### Comparing `webflask-0.4.5/webflask/two.html` & `webflask-0.5/webflask/two.html`

 * *Files identical despite different names*

### Comparing `webflask-0.4.5/webflask/uploads.txt` & `webflask-0.5/webflask/uploads.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 rails new file_upload_example
-cd file_upload_example
+cd file_upload_example --skip-git
 
 rails generate controller uploads new create
 
 Open `config/routes.rb` and add:
 
 
 Rails.application.routes.draw do
```

