# Comparing `tmp/books_lib-1.0.5.tar.gz` & `tmp/books_lib-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "books_lib-1.0.5.tar", last modified: Sat May 11 22:16:04 2024, max compression
+gzip compressed data, was "books_lib-1.0.7.tar", last modified: Mon May 13 19:03:57 2024, max compression
```

## Comparing `books_lib-1.0.5.tar` & `books_lib-1.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 22:16:03.704414 books_lib-1.0.5/
-drwxrwxrwx   0        0        0        0 2024-05-11 22:16:03.370978 books_lib-1.0.5/Books_Lib/
--rw-rw-rw-   0        0        0       37 2024-05-11 19:12:54.000000 books_lib-1.0.5/Books_Lib/__init__.py
--rw-rw-rw-   0        0        0    12151 2015-08-14 13:17:32.000000 books_lib-1.0.5/Books_Lib/books.csv
--rw-rw-rw-   0        0        0     1991 2024-05-11 22:15:37.000000 books_lib-1.0.5/Books_Lib/random_books.py
-drwxrwxrwx   0        0        0        0 2024-05-11 22:16:03.588183 books_lib-1.0.5/Books_Lib.egg-info/
--rw-rw-rw-   0        0        0      334 2024-05-11 22:16:00.000000 books_lib-1.0.5/Books_Lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-05-11 22:16:01.000000 books_lib-1.0.5/Books_Lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 22:16:00.000000 books_lib-1.0.5/Books_Lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-11 22:16:00.000000 books_lib-1.0.5/Books_Lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-11 22:16:00.000000 books_lib-1.0.5/Books_Lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      334 2024-05-11 22:16:03.699528 books_lib-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      842 2024-05-11 20:04:41.000000 books_lib-1.0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-11 22:16:03.705392 books_lib-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      538 2024-05-11 22:15:37.000000 books_lib-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:03:57.288279 books_lib-1.0.7/
+drwxrwxrwx   0        0        0        0 2024-05-13 19:03:57.155129 books_lib-1.0.7/Books_Lib/
+-rw-rw-rw-   0        0        0       37 2024-05-11 19:12:54.000000 books_lib-1.0.7/Books_Lib/__init__.py
+-rw-rw-rw-   0        0        0    12151 2015-08-14 13:17:32.000000 books_lib-1.0.7/Books_Lib/books.csv
+-rw-rw-rw-   0        0        0     2396 2024-05-13 18:52:22.000000 books_lib-1.0.7/Books_Lib/random_books.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:03:57.234296 books_lib-1.0.7/Books_Lib.egg-info/
+-rw-rw-rw-   0        0        0      334 2024-05-13 19:03:55.000000 books_lib-1.0.7/Books_Lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-13 19:03:55.000000 books_lib-1.0.7/Books_Lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 19:03:55.000000 books_lib-1.0.7/Books_Lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-13 19:03:55.000000 books_lib-1.0.7/Books_Lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-13 19:03:55.000000 books_lib-1.0.7/Books_Lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      334 2024-05-13 19:03:57.266515 books_lib-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      842 2024-05-11 20:04:41.000000 books_lib-1.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-13 19:03:57.289257 books_lib-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      538 2024-05-13 19:03:11.000000 books_lib-1.0.7/setup.py
```

### Comparing `books_lib-1.0.5/Books_Lib/books.csv` & `books_lib-1.0.7/Books_Lib/books.csv`

 * *Files identical despite different names*

### Comparing `books_lib-1.0.5/Books_Lib/random_books.py` & `books_lib-1.0.7/Books_Lib/random_books.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,69 +8,72 @@
         self._file = pd.read_csv(SelectBooks.FILE_PATH)
         self._title = None
         self._author = None
         self._genre = None
         self._height = None
         self._publisher = None
 
+    def generate_books(self):
+        self._books = self._file.saple()
+        self._number = self._books["#"].values[0]
+        self._title = self._books["Title"].values[0]
+        self._author = self._books["Author"].values[0]
+        self._genre = self._books["Genre"].values[0]
+        self._height = self._books["Height"].values[0]
+        self._publisher = self._books["Publisher"].values[0]
 
-    def buscar_Title(title):
+    def buscar_Number(_number):
         file = "books.csv"
         datos = pd.read_csv(file)
-        buscar = datos[datos["Title"] == title]
+        buscar = datos[datos["Number"] == _number]
         if buscar.size == 0:
             return "No se encontro el titulo "
         else:
             return buscar
 
+    def buscar_Title(_title):
+        file = "books.csv"
+        datos = pd.read_csv(file)
+        buscar = datos[datos["Title"] == _title]
+        if buscar.size == 0:
+            return "No se encontro el titulo "
+        else:
+            return buscar
 
-    def buscar_Author(author):
+
+    def buscar_Author(_author):
         file = "books.csv"
         datos = pd.read_csv(file)
-        buscar = datos[datos["Author"] == author]
+        buscar = datos[datos["Author"] == _author]
         if buscar.size == 0:
             return "No se encontro el autor"
         else:
             return buscar
 
-    def buscar_Genre(genre):
+    def buscar_Genre(_genre):
         file = "books.csv"
         datos = pd.read_csv(file)
-        buscar = datos[datos["Author"] == genre]
+        buscar = datos[datos["Genre"] == _genre]
         if buscar.size == 0:
             return "No se encontro el autor"
         else:
             return buscar
 
 
-    def buscar_Height(heigth):
+    def buscar_Height(_height):
         file = "books.csv"
         datos = pd.read_csv(file)
-        buscar = datos[datos["Author"] == heigth]
+        buscar = datos[datos["Height"] == _height]
         if buscar.size == 0:
             return "No se encontro el autor"
         else:
             return buscar
 
-    def buscar_Publisher(publisher):
+    def buscar_Publisher(_publisher):
         file = "books.csv"
         datos = pd.read_csv(file)
-        buscar = datos[datos["Author"] == publisher]
+        buscar = datos[datos["Publisher"] == _publisher]
         if buscar.size == 0:
             return "No se encontro el autor"
         else:
             return buscar
 
-    def getAuthor(self):
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
-    def getPublisher(self):
-        return self._publisher
```

### Comparing `books_lib-1.0.5/README.md` & `books_lib-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `books_lib-1.0.5/setup.py` & `books_lib-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
 
    name='Books_Lib',
-   version='1.0.5',
+   version='1.0.7',
    author= 'Milton Alejandro Angel Cardenas ',
    author_email='milton_ac@tesch.edu.mx',
    description='Es una libreria en la cual podremos encontrar el autor y el libro, de pende el que se escriba',
    packages= ['Books_Lib'],
    package_data={'Books_Lib': ['books.csv']},
    install_requires=['pandas',
                      'twine',
```

