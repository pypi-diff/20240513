# Comparing `tmp/journeylib-2.0.1.tar.gz` & `tmp/journeylib-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "journeylib-2.0.1.tar", last modified: Tue May  7 10:53:09 2024, max compression
+gzip compressed data, was "journeylib-2.0.2.tar", last modified: Mon May 13 18:00:17 2024, max compression
```

## Comparing `journeylib-2.0.1.tar` & `journeylib-2.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-07 10:53:09.810241 journeylib-2.0.1/
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1471 2024-05-07 10:53:09.807093 journeylib-2.0.1/PKG-INFO
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1147 2024-05-06 08:54:27.000000 journeylib-2.0.1/README.md
-drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-07 10:53:09.644870 journeylib-2.0.1/journeylib/
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       24 2024-04-25 11:14:41.000000 journeylib-2.0.1/journeylib/__init__.py
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)      949 2024-05-07 09:10:42.000000 journeylib-2.0.1/journeylib/funciones.py
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1676 2024-05-06 08:54:27.000000 journeylib-2.0.1/journeylib/tests.py
-drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-07 10:53:09.776380 journeylib-2.0.1/journeylib.egg-info/
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1471 2024-05-07 10:53:09.000000 journeylib-2.0.1/journeylib.egg-info/PKG-INFO
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)      254 2024-05-07 10:53:09.000000 journeylib-2.0.1/journeylib.egg-info/SOURCES.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)        1 2024-05-07 10:53:09.000000 journeylib-2.0.1/journeylib.egg-info/dependency_links.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       17 2024-05-07 10:53:09.000000 journeylib-2.0.1/journeylib.egg-info/requires.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       11 2024-05-07 10:53:09.000000 journeylib-2.0.1/journeylib.egg-info/top_level.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       38 2024-05-07 10:53:09.811637 journeylib-2.0.1/setup.cfg
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1361 2024-05-07 10:52:36.000000 journeylib-2.0.1/setup.py
+drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-13 18:00:17.795108 journeylib-2.0.2/
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1471 2024-05-13 18:00:17.788402 journeylib-2.0.2/PKG-INFO
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1147 2024-05-06 08:54:27.000000 journeylib-2.0.2/README.md
+drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-13 18:00:17.603423 journeylib-2.0.2/journeylib/
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       24 2024-04-25 11:14:41.000000 journeylib-2.0.2/journeylib/__init__.py
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1489 2024-05-13 17:58:31.000000 journeylib-2.0.2/journeylib/funciones.py
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     2772 2024-05-13 17:14:25.000000 journeylib-2.0.2/journeylib/tests.py
+drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-13 18:00:17.760513 journeylib-2.0.2/journeylib.egg-info/
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1471 2024-05-13 18:00:17.000000 journeylib-2.0.2/journeylib.egg-info/PKG-INFO
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)      254 2024-05-13 18:00:17.000000 journeylib-2.0.2/journeylib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)        1 2024-05-13 18:00:17.000000 journeylib-2.0.2/journeylib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       17 2024-05-13 18:00:17.000000 journeylib-2.0.2/journeylib.egg-info/requires.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       11 2024-05-13 18:00:17.000000 journeylib-2.0.2/journeylib.egg-info/top_level.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       38 2024-05-13 18:00:17.799623 journeylib-2.0.2/setup.cfg
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1361 2024-05-13 17:58:55.000000 journeylib-2.0.2/setup.py
```

### Comparing `journeylib-2.0.1/PKG-INFO` & `journeylib-2.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: journeylib
-Version: 2.0.1
+Version: 2.0.2
 Summary: Libreria para gestionar datos del historico del proyecto GPTravel
 Home-page: https://ismigit.fi.upm.es/gptravel-2024/ai-squad/journeygenai
 Author: Equipo JourneyGen UPM
 Author-email: f.gonzalez.lopez@alumnos.upm.es
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `journeylib-2.0.1/README.md` & `journeylib-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `journeylib-2.0.1/journeylib.egg-info/PKG-INFO` & `journeylib-2.0.2/journeylib.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: journeylib
-Version: 2.0.1
+Version: 2.0.2
 Summary: Libreria para gestionar datos del historico del proyecto GPTravel
 Home-page: https://ismigit.fi.upm.es/gptravel-2024/ai-squad/journeygenai
 Author: Equipo JourneyGen UPM
 Author-email: f.gonzalez.lopez@alumnos.upm.es
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `journeylib-2.0.1/setup.py` & `journeylib-2.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '2.0.1' #Numero de version que decidamos, cambiarlo al añadir nuevas funcionalidades o cambios
+VERSION = '2.0.2' #Numero de version que decidamos, cambiarlo al añadir nuevas funcionalidades o cambios
 PACKAGE_NAME = 'journeylib' #Nombre de la libreria
 AUTHOR = 'Equipo JourneyGen UPM' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'f.gonzalez.lopez@alumnos.upm.es' #Modificar con vuestros datos
 URL = 'https://ismigit.fi.upm.es/gptravel-2024/ai-squad/journeygenai' #Modificar con vuestros datos
 
 LICENSE = 'MIT' #Tipo de licencia
 DESCRIPTION = 'Libreria para gestionar datos del historico del proyecto GPTravel' #Descripción corta
```

