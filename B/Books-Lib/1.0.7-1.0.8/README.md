# Comparing `tmp/books_lib-1.0.7.tar.gz` & `tmp/books_lib-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "books_lib-1.0.7.tar", last modified: Mon May 13 19:03:57 2024, max compression
+gzip compressed data, was "books_lib-1.0.8.tar", last modified: Mon May 13 19:29:57 2024, max compression
```

## Comparing `books_lib-1.0.7.tar` & `books_lib-1.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 19:03:57.288279 books_lib-1.0.7/
-drwxrwxrwx   0        0        0        0 2024-05-13 19:03:57.155129 books_lib-1.0.7/Books_Lib/
--rw-rw-rw-   0        0        0       37 2024-05-11 19:12:54.000000 books_lib-1.0.7/Books_Lib/__init__.py
--rw-rw-rw-   0        0        0    12151 2015-08-14 13:17:32.000000 books_lib-1.0.7/Books_Lib/books.csv
--rw-rw-rw-   0        0        0     2396 2024-05-13 18:52:22.000000 books_lib-1.0.7/Books_Lib/random_books.py
-drwxrwxrwx   0        0        0        0 2024-05-13 19:03:57.234296 books_lib-1.0.7/Books_Lib.egg-info/
--rw-rw-rw-   0        0        0      334 2024-05-13 19:03:55.000000 books_lib-1.0.7/Books_Lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-05-13 19:03:55.000000 books_lib-1.0.7/Books_Lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 19:03:55.000000 books_lib-1.0.7/Books_Lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-13 19:03:55.000000 books_lib-1.0.7/Books_Lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-13 19:03:55.000000 books_lib-1.0.7/Books_Lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      334 2024-05-13 19:03:57.266515 books_lib-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      842 2024-05-11 20:04:41.000000 books_lib-1.0.7/README.md
--rw-rw-rw-   0        0        0       42 2024-05-13 19:03:57.289257 books_lib-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      538 2024-05-13 19:03:11.000000 books_lib-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:29:56.888801 books_lib-1.0.8/
+drwxrwxrwx   0        0        0        0 2024-05-13 19:29:56.831200 books_lib-1.0.8/Books_Lib/
+-rw-rw-rw-   0        0        0       37 2024-05-11 19:12:54.000000 books_lib-1.0.8/Books_Lib/__init__.py
+-rw-rw-rw-   0        0        0    12151 2015-08-14 13:17:32.000000 books_lib-1.0.8/Books_Lib/books.csv
+-rw-rw-rw-   0        0        0     1268 2024-05-13 19:29:27.000000 books_lib-1.0.8/Books_Lib/random_books.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:29:56.880990 books_lib-1.0.8/Books_Lib.egg-info/
+-rw-rw-rw-   0        0        0      334 2024-05-13 19:29:56.000000 books_lib-1.0.8/Books_Lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-13 19:29:56.000000 books_lib-1.0.8/Books_Lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 19:29:56.000000 books_lib-1.0.8/Books_Lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-13 19:29:56.000000 books_lib-1.0.8/Books_Lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-13 19:29:56.000000 books_lib-1.0.8/Books_Lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      334 2024-05-13 19:29:56.884894 books_lib-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      842 2024-05-11 20:04:41.000000 books_lib-1.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-13 19:29:56.888801 books_lib-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      538 2024-05-13 19:29:42.000000 books_lib-1.0.8/setup.py
```

### Comparing `books_lib-1.0.7/Books_Lib/books.csv` & `books_lib-1.0.8/Books_Lib/books.csv`

 * *Files identical despite different names*

### Comparing `books_lib-1.0.7/README.md` & `books_lib-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `books_lib-1.0.7/setup.py` & `books_lib-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
 
    name='Books_Lib',
-   version='1.0.7',
+   version='1.0.8',
    author= 'Milton Alejandro Angel Cardenas ',
    author_email='milton_ac@tesch.edu.mx',
    description='Es una libreria en la cual podremos encontrar el autor y el libro, de pende el que se escriba',
    packages= ['Books_Lib'],
    package_data={'Books_Lib': ['books.csv']},
    install_requires=['pandas',
                      'twine',
```

