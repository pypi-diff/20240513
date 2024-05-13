# Comparing `tmp/google-auth-st-0.3.tar.gz` & `tmp/google-auth-st-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-auth-st-0.3.tar", last modified: Mon May 13 13:59:00 2024, max compression
+gzip compressed data, was "google-auth-st-1.1.tar", last modified: Mon May 13 14:15:57 2024, max compression
```

## Comparing `google-auth-st-0.3.tar` & `google-auth-st-1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 13:59:00.048537 google-auth-st-0.3/
--rw-rw-rw-   0        0        0     1065 2024-05-10 14:11:09.000000 google-auth-st-0.3/LICENSE
--rw-rw-rw-   0        0        0     1831 2024-05-13 13:59:00.047536 google-auth-st-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1478 2024-05-10 14:20:05.000000 google-auth-st-0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 13:59:00.006537 google-auth-st-0.3/google_auth_st/
--rw-rw-rw-   0        0        0       35 2024-05-13 13:58:10.000000 google-auth-st-0.3/google_auth_st/__init__.py
--rw-rw-rw-   0        0        0      567 2024-05-13 11:51:11.000000 google-auth-st-0.3/google_auth_st/aggregate_auth.py
--rw-rw-rw-   0        0        0     3186 2024-05-12 21:15:40.000000 google-auth-st-0.3/google_auth_st/google_auth.py
-drwxrwxrwx   0        0        0        0 2024-05-13 13:59:00.045535 google-auth-st-0.3/google_auth_st.egg-info/
--rw-rw-rw-   0        0        0     1831 2024-05-13 13:58:59.000000 google-auth-st-0.3/google_auth_st.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-13 13:58:59.000000 google-auth-st-0.3/google_auth_st.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 13:58:59.000000 google-auth-st-0.3/google_auth_st.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-05-13 13:58:59.000000 google-auth-st-0.3/google_auth_st.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-13 13:58:59.000000 google-auth-st-0.3/google_auth_st.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 13:59:00.048537 google-auth-st-0.3/setup.cfg
--rw-rw-rw-   0        0        0      603 2024-05-13 13:54:44.000000 google-auth-st-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:15:57.950206 google-auth-st-1.1/
+-rw-rw-rw-   0        0        0     1065 2024-05-10 14:11:09.000000 google-auth-st-1.1/LICENSE
+-rw-rw-rw-   0        0        0     1831 2024-05-13 14:15:57.949211 google-auth-st-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1478 2024-05-10 14:20:05.000000 google-auth-st-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 14:15:57.935255 google-auth-st-1.1/google_auth_st/
+-rw-rw-rw-   0        0        0       36 2024-05-13 14:10:25.000000 google-auth-st-1.1/google_auth_st/__init__.py
+-rw-rw-rw-   0        0        0      567 2024-05-13 11:51:11.000000 google-auth-st-1.1/google_auth_st/aggregate_auth.py
+-rw-rw-rw-   0        0        0     3186 2024-05-12 21:15:40.000000 google-auth-st-1.1/google_auth_st/google_auth.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:15:57.947209 google-auth-st-1.1/google_auth_st.egg-info/
+-rw-rw-rw-   0        0        0     1831 2024-05-13 14:15:57.000000 google-auth-st-1.1/google_auth_st.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-13 14:15:57.000000 google-auth-st-1.1/google_auth_st.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 14:15:57.000000 google-auth-st-1.1/google_auth_st.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-13 14:15:57.000000 google-auth-st-1.1/google_auth_st.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-13 14:15:57.000000 google-auth-st-1.1/google_auth_st.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 14:15:57.950206 google-auth-st-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      588 2024-05-13 14:12:11.000000 google-auth-st-1.1/setup.py
```

### Comparing `google-auth-st-0.3/LICENSE` & `google-auth-st-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-auth-st-0.3/PKG-INFO` & `google-auth-st-1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-auth-st
-Version: 0.3
+Version: 1.1
 Summary: Librería para añadir autenticación con Google en aplicaciones web con el framework de Streamlit.
 Home-page: https://github.com/valantoni/google-auth-st.git
 Author: Toni Dev
 Author-email: classtonidev@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `google-auth-st-0.3/README.md` & `google-auth-st-1.1/README.md`

 * *Files identical despite different names*

### Comparing `google-auth-st-0.3/google_auth_st/aggregate_auth.py` & `google-auth-st-1.1/google_auth_st/aggregate_auth.py`

 * *Files identical despite different names*

### Comparing `google-auth-st-0.3/google_auth_st/google_auth.py` & `google-auth-st-1.1/google_auth_st/google_auth.py`

 * *Files identical despite different names*

### Comparing `google-auth-st-0.3/google_auth_st.egg-info/PKG-INFO` & `google-auth-st-1.1/google_auth_st.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-auth-st
-Version: 0.3
+Version: 1.1
 Summary: Librería para añadir autenticación con Google en aplicaciones web con el framework de Streamlit.
 Home-page: https://github.com/valantoni/google-auth-st.git
 Author: Toni Dev
 Author-email: classtonidev@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `google-auth-st-0.3/setup.py` & `google-auth-st-1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 
 setup(
     name='google-auth-st',
-    version='0.3',
+    version='1.1',
     packages= ['google_auth_st'],
     description='Librería para añadir autenticación con Google en aplicaciones web con el framework de Streamlit.',
     long_description=open('README.md',encoding='utf-8').read(),
     long_description_content_type='text/markdown',  
     author='Toni Dev',
     author_email='classtonidev@gmail.com',
     url='https://github.com/valantoni/google-auth-st.git',
```

