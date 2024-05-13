# Comparing `tmp/gilfoyle_forked-0.915.tar.gz` & `tmp/gilfoyle_forked-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gilfoyle_forked-0.915.tar", last modified: Mon May 13 18:43:42 2024, max compression
+gzip compressed data, was "gilfoyle_forked-1.0.0.tar", last modified: Mon May 13 18:55:35 2024, max compression
```

## Comparing `gilfoyle_forked-0.915.tar` & `gilfoyle_forked-1.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:43:42.066077 gilfoyle_forked-0.915/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-13 18:43:35.000000 gilfoyle_forked-0.915/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-13 18:43:35.000000 gilfoyle_forked-0.915/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-13 18:43:42.062077 gilfoyle_forked-0.915/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-13 18:43:35.000000 gilfoyle_forked-0.915/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:43:42.058077 gilfoyle_forked-0.915/gilfoyle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:43:35.000000 gilfoyle_forked-0.915/gilfoyle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:43:42.062077 gilfoyle_forked-0.915/gilfoyle/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:43:42.062077 gilfoyle_forked-0.915/gilfoyle/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-13 18:43:35.000000 gilfoyle_forked-0.915/gilfoyle/assets/css/default.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:43:42.062077 gilfoyle_forked-0.915/gilfoyle/assets/data/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-13 18:43:35.000000 gilfoyle_forked-0.915/gilfoyle/assets/data/ga-sample.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)     5299 2024-05-13 18:43:35.000000 gilfoyle_forked-0.915/gilfoyle/assets/examples.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:43:42.062077 gilfoyle_forked-0.915/gilfoyle/assets/images/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2648 2024-05-13 18:43:35.000000 gilfoyle_forked-0.915/gilfoyle/assets/images/barchart.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    86802 2024-05-13 18:43:35.000000 gilfoyle_forked-0.915/gilfoyle/assets/images/cover.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)      923 2024-05-13 18:43:35.000000 gilfoyle_forked-0.915/gilfoyle/assets/template.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:43:42.062077 gilfoyle_forked-0.915/gilfoyle/assets/templates/
--rwxr-xr-x   0 runner    (1001) docker     (127)      594 2024-05-13 18:43:35.000000 gilfoyle_forked-0.915/gilfoyle/assets/templates/chapter.tmpl
--rwxr-xr-x   0 runner    (1001) docker     (127)      608 2024-05-13 18:43:35.000000 gilfoyle_forked-0.915/gilfoyle/assets/templates/cover.tmpl
--rwxr-xr-x   0 runner    (1001) docker     (127)      227 2024-05-13 18:43:35.000000 gilfoyle_forked-0.915/gilfoyle/assets/templates/message.tmpl
--rwxr-xr-x   0 runner    (1001) docker     (127)      554 2024-05-13 18:43:35.000000 gilfoyle_forked-0.915/gilfoyle/assets/templates/metrics.tmpl
--rwxr-xr-x   0 runner    (1001) docker     (127)      206 2024-05-13 18:43:35.000000 gilfoyle_forked-0.915/gilfoyle/assets/templates/notification.tmpl
--rwxr-xr-x   0 runner    (1001) docker     (127)     6920 2024-05-13 18:43:35.000000 gilfoyle_forked-0.915/gilfoyle/assets/templates/report.tmpl
--rw-r--r--   0 runner    (1001) docker     (127)    12884 2024-05-13 18:43:35.000000 gilfoyle_forked-0.915/gilfoyle/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:43:42.062077 gilfoyle_forked-0.915/gilfoyle_forked.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-13 18:43:42.000000 gilfoyle_forked-0.915/gilfoyle_forked.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-13 18:43:42.000000 gilfoyle_forked-0.915/gilfoyle_forked.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 18:43:42.000000 gilfoyle_forked-0.915/gilfoyle_forked.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-13 18:43:42.000000 gilfoyle_forked-0.915/gilfoyle_forked.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-13 18:43:42.000000 gilfoyle_forked-0.915/gilfoyle_forked.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 18:43:42.066077 gilfoyle_forked-0.915/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-13 18:43:35.000000 gilfoyle_forked-0.915/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:55:35.725421 gilfoyle_forked-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-13 18:55:35.725421 gilfoyle_forked-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:55:35.721421 gilfoyle_forked-1.0.0/gilfoyle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:55:35.721421 gilfoyle_forked-1.0.0/gilfoyle/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:55:35.721421 gilfoyle_forked-1.0.0/gilfoyle/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/assets/css/default.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:55:35.721421 gilfoyle_forked-1.0.0/gilfoyle/assets/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/assets/data/ga-sample.csv
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5299 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/assets/examples.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:55:35.721421 gilfoyle_forked-1.0.0/gilfoyle/assets/images/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2648 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/assets/images/barchart.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    86802 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/assets/images/cover.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      923 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/assets/template.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:55:35.721421 gilfoyle_forked-1.0.0/gilfoyle/assets/templates/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      594 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/assets/templates/chapter.tmpl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      608 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/assets/templates/cover.tmpl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      227 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/assets/templates/message.tmpl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      554 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/assets/templates/metrics.tmpl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      206 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/assets/templates/notification.tmpl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6920 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/assets/templates/report.tmpl
+-rw-r--r--   0 runner    (1001) docker     (127)    12884 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/gilfoyle/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:55:35.725421 gilfoyle_forked-1.0.0/gilfoyle_forked.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-13 18:55:35.000000 gilfoyle_forked-1.0.0/gilfoyle_forked.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-13 18:55:35.000000 gilfoyle_forked-1.0.0/gilfoyle_forked.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 18:55:35.000000 gilfoyle_forked-1.0.0/gilfoyle_forked.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-13 18:55:35.000000 gilfoyle_forked-1.0.0/gilfoyle_forked.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-13 18:55:35.000000 gilfoyle_forked-1.0.0/gilfoyle_forked.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 18:55:35.725421 gilfoyle_forked-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-13 18:55:27.000000 gilfoyle_forked-1.0.0/setup.py
```

### Comparing `gilfoyle_forked-0.915/LICENSE` & `gilfoyle_forked-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gilfoyle_forked-0.915/PKG-INFO` & `gilfoyle_forked-1.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gilfoyle-forked
-Version: 0.915
+Version: 1.0.0
 Summary: Gilfoyle is a Python-based report generator for data scientists who use Pandas.
-Home-page: https://github.com/practical-data-science/gilfoyle
-Download-URL: https://github.com/practical-data-science/gilfoyle/archive/master.zip
-Author: Matt Clarke
-Author-email: matt@practicaldatascience.co.uk
+Home-page: https://github.com/sr-auto/gilfoyle
+Download-URL: https://github.com/sr-auto/gilfoyle/archive/master.zip
+Author: Shahab Rashid
+Author-email: sr.python10@gmail.com
 License: MIT
 Keywords: python,reports,reporting,pandas,pdf
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -20,15 +20,15 @@
 Requires-Dist: jinja2
 Requires-Dist: seaborn
 
 # Gilfoyle
 Gilfoyle is a report generation tool for Python which makes it quick and easy to create stylish looking reports or presentations using data. 
 
 #### Installation
-You can install Gilfoyle by entering `pip3 install gilfoyle` in your terminal. 
+You can install Gilfoyle by entering `pip3 install gilfoyle-forked` in your terminal. 
 
 #### Usage
 Gilfoyle can be used within a regular Python script or from inside a Jupyter notebook. See the `example.py`
 file for some working examples. 
 
 ```python
 # Load packages
```

### Comparing `gilfoyle_forked-0.915/README.md` & `gilfoyle_forked-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Gilfoyle
 Gilfoyle is a report generation tool for Python which makes it quick and easy to create stylish looking reports or presentations using data. 
 
 #### Installation
-You can install Gilfoyle by entering `pip3 install gilfoyle` in your terminal. 
+You can install Gilfoyle by entering `pip3 install gilfoyle-forked` in your terminal. 
 
 #### Usage
 Gilfoyle can be used within a regular Python script or from inside a Jupyter notebook. See the `example.py`
 file for some working examples. 
 
 ```python
 # Load packages
```

### Comparing `gilfoyle_forked-0.915/gilfoyle/assets/css/default.css` & `gilfoyle_forked-1.0.0/gilfoyle/assets/css/default.css`

 * *Files identical despite different names*

### Comparing `gilfoyle_forked-0.915/gilfoyle/assets/data/ga-sample.csv` & `gilfoyle_forked-1.0.0/gilfoyle/assets/data/ga-sample.csv`

 * *Files identical despite different names*

### Comparing `gilfoyle_forked-0.915/gilfoyle/assets/examples.html` & `gilfoyle_forked-1.0.0/gilfoyle/assets/examples.html`

 * *Files identical despite different names*

### Comparing `gilfoyle_forked-0.915/gilfoyle/assets/images/barchart.png` & `gilfoyle_forked-1.0.0/gilfoyle/assets/images/barchart.png`

 * *Files identical despite different names*

### Comparing `gilfoyle_forked-0.915/gilfoyle/assets/images/cover.jpg` & `gilfoyle_forked-1.0.0/gilfoyle/assets/images/cover.jpg`

 * *Files identical despite different names*

### Comparing `gilfoyle_forked-0.915/gilfoyle/assets/template.html` & `gilfoyle_forked-1.0.0/gilfoyle/assets/template.html`

 * *Files identical despite different names*

### Comparing `gilfoyle_forked-0.915/gilfoyle/assets/templates/chapter.tmpl` & `gilfoyle_forked-1.0.0/gilfoyle/assets/templates/chapter.tmpl`

 * *Files identical despite different names*

### Comparing `gilfoyle_forked-0.915/gilfoyle/assets/templates/cover.tmpl` & `gilfoyle_forked-1.0.0/gilfoyle/assets/templates/cover.tmpl`

 * *Files identical despite different names*

### Comparing `gilfoyle_forked-0.915/gilfoyle/assets/templates/metrics.tmpl` & `gilfoyle_forked-1.0.0/gilfoyle/assets/templates/metrics.tmpl`

 * *Files identical despite different names*

### Comparing `gilfoyle_forked-0.915/gilfoyle/assets/templates/report.tmpl` & `gilfoyle_forked-1.0.0/gilfoyle/assets/templates/report.tmpl`

 * *Files identical despite different names*

### Comparing `gilfoyle_forked-0.915/gilfoyle/report.py` & `gilfoyle_forked-1.0.0/gilfoyle/report.py`

 * *Files identical despite different names*

### Comparing `gilfoyle_forked-0.915/gilfoyle_forked.egg-info/PKG-INFO` & `gilfoyle_forked-1.0.0/gilfoyle_forked.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gilfoyle-forked
-Version: 0.915
+Version: 1.0.0
 Summary: Gilfoyle is a Python-based report generator for data scientists who use Pandas.
-Home-page: https://github.com/practical-data-science/gilfoyle
-Download-URL: https://github.com/practical-data-science/gilfoyle/archive/master.zip
-Author: Matt Clarke
-Author-email: matt@practicaldatascience.co.uk
+Home-page: https://github.com/sr-auto/gilfoyle
+Download-URL: https://github.com/sr-auto/gilfoyle/archive/master.zip
+Author: Shahab Rashid
+Author-email: sr.python10@gmail.com
 License: MIT
 Keywords: python,reports,reporting,pandas,pdf
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -20,15 +20,15 @@
 Requires-Dist: jinja2
 Requires-Dist: seaborn
 
 # Gilfoyle
 Gilfoyle is a report generation tool for Python which makes it quick and easy to create stylish looking reports or presentations using data. 
 
 #### Installation
-You can install Gilfoyle by entering `pip3 install gilfoyle` in your terminal. 
+You can install Gilfoyle by entering `pip3 install gilfoyle-forked` in your terminal. 
 
 #### Usage
 Gilfoyle can be used within a regular Python script or from inside a Jupyter notebook. See the `example.py`
 file for some working examples. 
 
 ```python
 # Load packages
```

### Comparing `gilfoyle_forked-0.915/gilfoyle_forked.egg-info/SOURCES.txt` & `gilfoyle_forked-1.0.0/gilfoyle_forked.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gilfoyle_forked-0.915/setup.py` & `gilfoyle_forked-1.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='gilfoyle-forked',
     packages=['gilfoyle'],
-    version='0.915',
+    version='1.0.0',
     license='MIT',
     description='Gilfoyle is a Python-based report generator for data scientists who use Pandas.',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    author='Matt Clarke',
-    author_email='matt@practicaldatascience.co.uk',
-    url='https://github.com/practical-data-science/gilfoyle',
-    download_url='https://github.com/practical-data-science/gilfoyle/archive/master.zip',
+    author='Shahab Rashid',
+    author_email='sr.python10@gmail.com',
+    url='https://github.com/sr-auto/gilfoyle',
+    download_url='https://github.com/sr-auto/gilfoyle/archive/master.zip',
     keywords=['python', 'reports', 'reporting', 'pandas', 'pdf'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
```

