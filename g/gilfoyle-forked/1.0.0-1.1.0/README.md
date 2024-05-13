# Comparing `tmp/gilfoyle_forked-1.0.0.tar.gz` & `tmp/gilfoyle_forked-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gilfoyle_forked-1.0.0.tar", last modified: Mon May 13 18:55:35 2024, max compression
+gzip compressed data, was "gilfoyle_forked-1.1.0.tar", last modified: Mon May 13 19:57:32 2024, max compression
```

## Comparing `gilfoyle_forked-1.0.0.tar` & `gilfoyle_forked-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:55:35.725421 gilfoyle_forked-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-13 18:55:35.725421 gilfoyle_forked-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:55:35.721421 gilfoyle_forked-1.0.0/gilfoyle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:55:35.721421 gilfoyle_forked-1.0.0/gilfoyle/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:55:35.721421 gilfoyle_forked-1.0.0/gilfoyle/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/assets/css/default.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:55:35.721421 gilfoyle_forked-1.0.0/gilfoyle/assets/data/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/assets/data/ga-sample.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)     5299 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/assets/examples.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:55:35.721421 gilfoyle_forked-1.0.0/gilfoyle/assets/images/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2648 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/assets/images/barchart.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    86802 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/assets/images/cover.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)      923 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/assets/template.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:55:35.721421 gilfoyle_forked-1.0.0/gilfoyle/assets/templates/
--rwxr-xr-x   0 runner    (1001) docker     (127)      594 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/assets/templates/chapter.tmpl
--rwxr-xr-x   0 runner    (1001) docker     (127)      608 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/assets/templates/cover.tmpl
--rwxr-xr-x   0 runner    (1001) docker     (127)      227 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/assets/templates/message.tmpl
--rwxr-xr-x   0 runner    (1001) docker     (127)      554 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/assets/templates/metrics.tmpl
--rwxr-xr-x   0 runner    (1001) docker     (127)      206 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/assets/templates/notification.tmpl
--rwxr-xr-x   0 runner    (1001) docker     (127)     6920 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/assets/templates/report.tmpl
--rw-r--r--   0 runner    (1001) docker     (127)    12884 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:55:35.725421 gilfoyle_forked-1.0.0/gilfoyle_forked.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-13 18:55:35.000000 gilfoyle_forked-1.0.0/gilfoyle_forked.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-13 18:55:35.000000 gilfoyle_forked-1.0.0/gilfoyle_forked.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 18:55:35.000000 gilfoyle_forked-1.0.0/gilfoyle_forked.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-13 18:55:35.000000 gilfoyle_forked-1.0.0/gilfoyle_forked.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-13 18:55:35.000000 gilfoyle_forked-1.0.0/gilfoyle_forked.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 18:55:35.725421 gilfoyle_forked-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:57:32.846404 gilfoyle_forked-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-13 19:57:29.000000 gilfoyle_forked-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-13 19:57:29.000000 gilfoyle_forked-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-13 19:57:32.846404 gilfoyle_forked-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-13 19:57:29.000000 gilfoyle_forked-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:57:32.842404 gilfoyle_forked-1.1.0/gilfoyle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 19:57:29.000000 gilfoyle_forked-1.1.0/gilfoyle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:57:32.842404 gilfoyle_forked-1.1.0/gilfoyle/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:57:32.842404 gilfoyle_forked-1.1.0/gilfoyle/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-13 19:57:29.000000 gilfoyle_forked-1.1.0/gilfoyle/assets/css/default.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:57:32.842404 gilfoyle_forked-1.1.0/gilfoyle/assets/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-13 19:57:29.000000 gilfoyle_forked-1.1.0/gilfoyle/assets/data/ga-sample.csv
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5299 2024-05-13 19:57:29.000000 gilfoyle_forked-1.1.0/gilfoyle/assets/examples.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:57:32.846404 gilfoyle_forked-1.1.0/gilfoyle/assets/images/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2648 2024-05-13 19:57:29.000000 gilfoyle_forked-1.1.0/gilfoyle/assets/images/barchart.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    86802 2024-05-13 19:57:29.000000 gilfoyle_forked-1.1.0/gilfoyle/assets/images/cover.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      923 2024-05-13 19:57:29.000000 gilfoyle_forked-1.1.0/gilfoyle/assets/template.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:57:32.846404 gilfoyle_forked-1.1.0/gilfoyle/assets/templates/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      594 2024-05-13 19:57:29.000000 gilfoyle_forked-1.1.0/gilfoyle/assets/templates/chapter.tmpl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      608 2024-05-13 19:57:29.000000 gilfoyle_forked-1.1.0/gilfoyle/assets/templates/cover.tmpl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      227 2024-05-13 19:57:29.000000 gilfoyle_forked-1.1.0/gilfoyle/assets/templates/message.tmpl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      554 2024-05-13 19:57:29.000000 gilfoyle_forked-1.1.0/gilfoyle/assets/templates/metrics.tmpl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      206 2024-05-13 19:57:29.000000 gilfoyle_forked-1.1.0/gilfoyle/assets/templates/notification.tmpl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6920 2024-05-13 19:57:29.000000 gilfoyle_forked-1.1.0/gilfoyle/assets/templates/report.tmpl
+-rw-r--r--   0 runner    (1001) docker     (127)    12924 2024-05-13 19:57:29.000000 gilfoyle_forked-1.1.0/gilfoyle/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:57:32.846404 gilfoyle_forked-1.1.0/gilfoyle_forked.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-13 19:57:32.000000 gilfoyle_forked-1.1.0/gilfoyle_forked.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-13 19:57:32.000000 gilfoyle_forked-1.1.0/gilfoyle_forked.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:57:32.000000 gilfoyle_forked-1.1.0/gilfoyle_forked.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-13 19:57:32.000000 gilfoyle_forked-1.1.0/gilfoyle_forked.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-13 19:57:32.000000 gilfoyle_forked-1.1.0/gilfoyle_forked.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 19:57:32.846404 gilfoyle_forked-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-13 19:57:29.000000 gilfoyle_forked-1.1.0/setup.py
```

### Comparing `gilfoyle_forked-1.0.0/LICENSE` & `gilfoyle_forked-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gilfoyle_forked-1.0.0/PKG-INFO` & `gilfoyle_forked-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gilfoyle-forked
-Version: 1.0.0
+Version: 1.1.0
 Summary: Gilfoyle is a Python-based report generator for data scientists who use Pandas.
 Home-page: https://github.com/sr-auto/gilfoyle
 Download-URL: https://github.com/sr-auto/gilfoyle/archive/master.zip
 Author: Shahab Rashid
 Author-email: sr.python10@gmail.com
 License: MIT
 Keywords: python,reports,reporting,pandas,pdf
```

### Comparing `gilfoyle_forked-1.0.0/README.md` & `gilfoyle_forked-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gilfoyle_forked-1.0.0/gilfoyle/assets/css/default.css` & `gilfoyle_forked-1.1.0/gilfoyle/assets/css/default.css`

 * *Files identical despite different names*

### Comparing `gilfoyle_forked-1.0.0/gilfoyle/assets/data/ga-sample.csv` & `gilfoyle_forked-1.1.0/gilfoyle/assets/data/ga-sample.csv`

 * *Files identical despite different names*

### Comparing `gilfoyle_forked-1.0.0/gilfoyle/assets/examples.html` & `gilfoyle_forked-1.1.0/gilfoyle/assets/examples.html`

 * *Files identical despite different names*

### Comparing `gilfoyle_forked-1.0.0/gilfoyle/assets/images/barchart.png` & `gilfoyle_forked-1.1.0/gilfoyle/assets/images/barchart.png`

 * *Files identical despite different names*

### Comparing `gilfoyle_forked-1.0.0/gilfoyle/assets/images/cover.jpg` & `gilfoyle_forked-1.1.0/gilfoyle/assets/images/cover.jpg`

 * *Files identical despite different names*

### Comparing `gilfoyle_forked-1.0.0/gilfoyle/assets/template.html` & `gilfoyle_forked-1.1.0/gilfoyle/assets/template.html`

 * *Files identical despite different names*

### Comparing `gilfoyle_forked-1.0.0/gilfoyle/assets/templates/chapter.tmpl` & `gilfoyle_forked-1.1.0/gilfoyle/assets/templates/chapter.tmpl`

 * *Files identical despite different names*

### Comparing `gilfoyle_forked-1.0.0/gilfoyle/assets/templates/cover.tmpl` & `gilfoyle_forked-1.1.0/gilfoyle/assets/templates/cover.tmpl`

 * *Files identical despite different names*

### Comparing `gilfoyle_forked-1.0.0/gilfoyle/assets/templates/metrics.tmpl` & `gilfoyle_forked-1.1.0/gilfoyle/assets/templates/metrics.tmpl`

 * *Files identical despite different names*

### Comparing `gilfoyle_forked-1.0.0/gilfoyle/assets/templates/report.tmpl` & `gilfoyle_forked-1.1.0/gilfoyle/assets/templates/report.tmpl`

 * *Files identical despite different names*

### Comparing `gilfoyle_forked-1.0.0/gilfoyle/report.py` & `gilfoyle_forked-1.1.0/gilfoyle/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,16 @@
             format_options = {
                 "classes":['dataframe', 'table', 'is-striped', 'is-fullwidth'],
                 "escape":False,
                 "max_rows":len(dataframe.index),
                 "max_cols":len(dataframe.columns),
                 "index":False
             }
-            format_options.update(format_opts)
+            if format_opts != None:
+                format_options.update(format_opts)
             formatted_df = dataframe.to_html(**format_options)
             return formatted_df
 
     """
     Load template
     """
```

### Comparing `gilfoyle_forked-1.0.0/gilfoyle_forked.egg-info/PKG-INFO` & `gilfoyle_forked-1.1.0/gilfoyle_forked.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gilfoyle-forked
-Version: 1.0.0
+Version: 1.1.0
 Summary: Gilfoyle is a Python-based report generator for data scientists who use Pandas.
 Home-page: https://github.com/sr-auto/gilfoyle
 Download-URL: https://github.com/sr-auto/gilfoyle/archive/master.zip
 Author: Shahab Rashid
 Author-email: sr.python10@gmail.com
 License: MIT
 Keywords: python,reports,reporting,pandas,pdf
```

### Comparing `gilfoyle_forked-1.0.0/gilfoyle_forked.egg-info/SOURCES.txt` & `gilfoyle_forked-1.1.0/gilfoyle_forked.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gilfoyle_forked-1.0.0/setup.py` & `gilfoyle_forked-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='gilfoyle-forked',
     packages=['gilfoyle'],
-    version='1.0.0',
+    version='1.1.0',
     license='MIT',
     description='Gilfoyle is a Python-based report generator for data scientists who use Pandas.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Shahab Rashid',
     author_email='sr.python10@gmail.com',
     url='https://github.com/sr-auto/gilfoyle',
```

