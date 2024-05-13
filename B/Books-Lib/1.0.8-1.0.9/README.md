# Comparing `tmp/books_lib-1.0.8.tar.gz` & `tmp/books_lib-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "books_lib-1.0.8.tar", last modified: Mon May 13 19:29:57 2024, max compression
+gzip compressed data, was "books_lib-1.0.9.tar", last modified: Mon May 13 19:59:30 2024, max compression
```

## Comparing `books_lib-1.0.8.tar` & `books_lib-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 19:29:56.888801 books_lib-1.0.8/
-drwxrwxrwx   0        0        0        0 2024-05-13 19:29:56.831200 books_lib-1.0.8/Books_Lib/
--rw-rw-rw-   0        0        0       37 2024-05-11 19:12:54.000000 books_lib-1.0.8/Books_Lib/__init__.py
--rw-rw-rw-   0        0        0    12151 2015-08-14 13:17:32.000000 books_lib-1.0.8/Books_Lib/books.csv
--rw-rw-rw-   0        0        0     1268 2024-05-13 19:29:27.000000 books_lib-1.0.8/Books_Lib/random_books.py
-drwxrwxrwx   0        0        0        0 2024-05-13 19:29:56.880990 books_lib-1.0.8/Books_Lib.egg-info/
--rw-rw-rw-   0        0        0      334 2024-05-13 19:29:56.000000 books_lib-1.0.8/Books_Lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-05-13 19:29:56.000000 books_lib-1.0.8/Books_Lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 19:29:56.000000 books_lib-1.0.8/Books_Lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-13 19:29:56.000000 books_lib-1.0.8/Books_Lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-13 19:29:56.000000 books_lib-1.0.8/Books_Lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      334 2024-05-13 19:29:56.884894 books_lib-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      842 2024-05-11 20:04:41.000000 books_lib-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-05-13 19:29:56.888801 books_lib-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      538 2024-05-13 19:29:42.000000 books_lib-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:59:30.090480 books_lib-1.0.9/
+drwxrwxrwx   0        0        0        0 2024-05-13 19:59:30.053380 books_lib-1.0.9/Books_Lib/
+-rw-rw-rw-   0        0        0       37 2024-05-11 19:12:54.000000 books_lib-1.0.9/Books_Lib/__init__.py
+-rw-rw-rw-   0        0        0    12151 2015-08-14 13:17:32.000000 books_lib-1.0.9/Books_Lib/books.csv
+-rw-rw-rw-   0        0        0     1373 2024-05-13 19:59:00.000000 books_lib-1.0.9/Books_Lib/random_books.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:59:30.086574 books_lib-1.0.9/Books_Lib.egg-info/
+-rw-rw-rw-   0        0        0      334 2024-05-13 19:59:29.000000 books_lib-1.0.9/Books_Lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-13 19:59:29.000000 books_lib-1.0.9/Books_Lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 19:59:29.000000 books_lib-1.0.9/Books_Lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-13 19:59:29.000000 books_lib-1.0.9/Books_Lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-13 19:59:29.000000 books_lib-1.0.9/Books_Lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      334 2024-05-13 19:59:30.088526 books_lib-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      842 2024-05-11 20:04:41.000000 books_lib-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-13 19:59:30.091456 books_lib-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      538 2024-05-13 19:59:28.000000 books_lib-1.0.9/setup.py
```

### Comparing `books_lib-1.0.8/Books_Lib/books.csv` & `books_lib-1.0.9/Books_Lib/books.csv`

 * *Files identical despite different names*

### Comparing `books_lib-1.0.8/Books_Lib/random_books.py` & `books_lib-1.0.9/Books_Lib/random_books.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,46 +9,39 @@
         self._number = None
         self._title = None
         self._author = None
         self._genre = None
         self._height = None
         self._publisher = None
 
+    def generate_random(self):
+        self._books = self._file.saple()
+        self._number = self._books["#"].values[0]
+        self._title = self._books["Title"].values[0]
+        self._author = self._books["Author"].values[0]
+        self._genre = self._books["Genre"].values[0]
+        self._height = self._books["Height"].values[0]
+        self._publisher = self._books["Publisher"].values[0]
+
+    def buscar_Number(_number):
+        buscar = ["Title"] == _number
+        if buscar == 0:
+            return "No se encontro el titulo "
+        else:
+            return buscar
 
-    def buscar_Title(title):
-        file = "books.csv"
-        datos = pd.read_csv(file)
-        buscar = datos[datos["Title"] == title]
-        if buscar.size == 0:
+    def buscar_Title(_title):
+        buscar = ["Title"] == _title
+        if buscar == 0:
             return "No se encontro el titulo "
         else:
             return buscar
 
 
-    def buscar_Author(author):
-        file = "books.csv"
-        datos = pd.read_csv(file)
-        buscar = datos[datos["Author"] == author]
-        if buscar.size == 0:
+    def buscar_Author(_author):
+        buscar = ["Author"] == _author
+        if buscar == 0:
             return "No se encontro el autor"
         else:
             return buscar
 
 
-    def getNum(self):
-        return self._number
-
-    def getAuth(self):
-        return self._author
-
-    def getTitle(self):
-        return self._title
-
-    def getGenre(self):
-        return self._genre
-
-    def getHeight(self):
-        return self._height
-
-    def getPubli(self):
-        return self._publisher
-
```

### Comparing `books_lib-1.0.8/README.md` & `books_lib-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `books_lib-1.0.8/setup.py` & `books_lib-1.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
 
    name='Books_Lib',
-   version='1.0.8',
+   version='1.0.9',
    author= 'Milton Alejandro Angel Cardenas ',
    author_email='milton_ac@tesch.edu.mx',
    description='Es una libreria en la cual podremos encontrar el autor y el libro, de pende el que se escriba',
    packages= ['Books_Lib'],
    package_data={'Books_Lib': ['books.csv']},
    install_requires=['pandas',
                      'twine',
```

