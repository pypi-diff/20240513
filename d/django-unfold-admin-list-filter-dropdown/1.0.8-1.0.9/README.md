# Comparing `tmp/django_unfold_admin_list_filter_dropdown-1.0.8.tar.gz` & `tmp/django_unfold_admin_list_filter_dropdown-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_unfold_admin_list_filter_dropdown-1.0.8.tar", last modified: Mon May 13 16:51:38 2024, max compression
+gzip compressed data, was "django_unfold_admin_list_filter_dropdown-1.0.9.tar", last modified: Mon May 13 17:35:01 2024, max compression
```

## Comparing `django_unfold_admin_list_filter_dropdown-1.0.8.tar` & `django_unfold_admin_list_filter_dropdown-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:51:38.476067 django_unfold_admin_list_filter_dropdown-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-13 16:51:35.000000 django_unfold_admin_list_filter_dropdown-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-13 16:51:35.000000 django_unfold_admin_list_filter_dropdown-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-13 16:51:38.476067 django_unfold_admin_list_filter_dropdown-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-13 16:51:35.000000 django_unfold_admin_list_filter_dropdown-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:51:38.476067 django_unfold_admin_list_filter_dropdown-1.0.8/django_unfold_admin_list_filter_dropdown.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-13 16:51:38.000000 django_unfold_admin_list_filter_dropdown-1.0.8/django_unfold_admin_list_filter_dropdown.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-13 16:51:38.000000 django_unfold_admin_list_filter_dropdown-1.0.8/django_unfold_admin_list_filter_dropdown.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:51:38.000000 django_unfold_admin_list_filter_dropdown-1.0.8/django_unfold_admin_list_filter_dropdown.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-13 16:51:38.000000 django_unfold_admin_list_filter_dropdown-1.0.8/django_unfold_admin_list_filter_dropdown.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:51:38.476067 django_unfold_admin_list_filter_dropdown-1.0.8/django_unfold_admin_listfilter_dropdown/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 16:51:35.000000 django_unfold_admin_list_filter_dropdown-1.0.8/django_unfold_admin_listfilter_dropdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-13 16:51:35.000000 django_unfold_admin_list_filter_dropdown-1.0.8/django_unfold_admin_listfilter_dropdown/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:51:38.476067 django_unfold_admin_list_filter_dropdown-1.0.8/django_unfold_admin_listfilter_dropdown/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:51:38.476067 django_unfold_admin_list_filter_dropdown-1.0.8/django_unfold_admin_listfilter_dropdown/templates/django_unfold_admin_listfilter_dropdown/
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-13 16:51:35.000000 django_unfold_admin_list_filter_dropdown-1.0.8/django_unfold_admin_listfilter_dropdown/templates/django_unfold_admin_listfilter_dropdown/dropdown_filter.html
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 16:51:38.476067 django_unfold_admin_list_filter_dropdown-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-13 16:51:35.000000 django_unfold_admin_list_filter_dropdown-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:35:01.229388 django_unfold_admin_list_filter_dropdown-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-13 17:34:58.000000 django_unfold_admin_list_filter_dropdown-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-13 17:34:58.000000 django_unfold_admin_list_filter_dropdown-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-13 17:35:01.225388 django_unfold_admin_list_filter_dropdown-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-13 17:34:58.000000 django_unfold_admin_list_filter_dropdown-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:35:01.225388 django_unfold_admin_list_filter_dropdown-1.0.9/django_unfold_admin_list_filter_dropdown.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-13 17:35:01.000000 django_unfold_admin_list_filter_dropdown-1.0.9/django_unfold_admin_list_filter_dropdown.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-13 17:35:01.000000 django_unfold_admin_list_filter_dropdown-1.0.9/django_unfold_admin_list_filter_dropdown.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 17:35:01.000000 django_unfold_admin_list_filter_dropdown-1.0.9/django_unfold_admin_list_filter_dropdown.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-13 17:35:01.000000 django_unfold_admin_list_filter_dropdown-1.0.9/django_unfold_admin_list_filter_dropdown.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:35:01.225388 django_unfold_admin_list_filter_dropdown-1.0.9/django_unfold_admin_listfilter_dropdown/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:34:58.000000 django_unfold_admin_list_filter_dropdown-1.0.9/django_unfold_admin_listfilter_dropdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-13 17:34:58.000000 django_unfold_admin_list_filter_dropdown-1.0.9/django_unfold_admin_listfilter_dropdown/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:35:01.225388 django_unfold_admin_list_filter_dropdown-1.0.9/django_unfold_admin_listfilter_dropdown/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:35:01.225388 django_unfold_admin_list_filter_dropdown-1.0.9/django_unfold_admin_listfilter_dropdown/templates/django_unfold_admin_listfilter_dropdown/
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-13 17:34:58.000000 django_unfold_admin_list_filter_dropdown-1.0.9/django_unfold_admin_listfilter_dropdown/templates/django_unfold_admin_listfilter_dropdown/dropdown_filter.html
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 17:35:01.229388 django_unfold_admin_list_filter_dropdown-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-13 17:34:58.000000 django_unfold_admin_list_filter_dropdown-1.0.9/setup.py
```

### Comparing `django_unfold_admin_list_filter_dropdown-1.0.8/LICENSE` & `django_unfold_admin_list_filter_dropdown-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django_unfold_admin_list_filter_dropdown-1.0.8/PKG-INFO` & `django_unfold_admin_list_filter_dropdown-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-unfold-admin-list-filter-dropdown
-Version: 1.0.8
+Version: 1.0.9
 Summary: Use dropdowns in Django admin list filter
 Home-page: https://github.com/francoborrelli/django-unfold-admin-list-filter-dropdown
-Download-URL: https://github.com/francoborrelli/django-unfold-admin-list-filter-dropdow/archive/1.0.8.zip
+Download-URL: https://github.com/francoborrelli/django-unfold-admin-list-filter-dropdow/archive/1.0.9.zip
 Author: Franco Borrelli
 Author-email: francoborrelli96@gmail.com
 License: MIT License
 Keywords: django,admin,filter,dropdown,unfold,django-unfold
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `django_unfold_admin_list_filter_dropdown-1.0.8/README.md` & `django_unfold_admin_list_filter_dropdown-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `django_unfold_admin_list_filter_dropdown-1.0.8/django_unfold_admin_list_filter_dropdown.egg-info/PKG-INFO` & `django_unfold_admin_list_filter_dropdown-1.0.9/django_unfold_admin_list_filter_dropdown.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-unfold-admin-list-filter-dropdown
-Version: 1.0.8
+Version: 1.0.9
 Summary: Use dropdowns in Django admin list filter
 Home-page: https://github.com/francoborrelli/django-unfold-admin-list-filter-dropdown
-Download-URL: https://github.com/francoborrelli/django-unfold-admin-list-filter-dropdow/archive/1.0.8.zip
+Download-URL: https://github.com/francoborrelli/django-unfold-admin-list-filter-dropdow/archive/1.0.9.zip
 Author: Franco Borrelli
 Author-email: francoborrelli96@gmail.com
 License: MIT License
 Keywords: django,admin,filter,dropdown,unfold,django-unfold
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `django_unfold_admin_list_filter_dropdown-1.0.8/django_unfold_admin_listfilter_dropdown/filters.py` & `django_unfold_admin_list_filter_dropdown-1.0.9/django_unfold_admin_listfilter_dropdown/filters.py`

 * *Files identical despite different names*

### Comparing `django_unfold_admin_list_filter_dropdown-1.0.8/setup.py` & `django_unfold_admin_list_filter_dropdown-1.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # encoding: utf-8
 
 import os
 from setuptools import find_packages, setup
 
-VERSION = '1.0.8'
+VERSION = '1.0.9'
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 description = 'Use dropdowns in Django admin list filter'
 
 setup(
```

