# Comparing `tmp/google-auth-st-0.2.tar.gz` & `tmp/google-auth-st-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-auth-st-0.2.tar", last modified: Mon May 13 12:22:11 2024, max compression
+gzip compressed data, was "google-auth-st-0.3.tar", last modified: Mon May 13 13:59:00 2024, max compression
```

## Comparing `google-auth-st-0.2.tar` & `google-auth-st-0.3.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 12:22:11.613491 google-auth-st-0.2/
--rw-rw-rw-   0        0        0     1065 2024-05-10 14:11:09.000000 google-auth-st-0.2/LICENSE
--rw-rw-rw-   0        0        0     1831 2024-05-13 12:22:11.612490 google-auth-st-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1478 2024-05-10 14:20:05.000000 google-auth-st-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 12:22:11.610490 google-auth-st-0.2/google_auth_st.egg-info/
--rw-rw-rw-   0        0        0     1831 2024-05-13 12:22:11.000000 google-auth-st-0.2/google_auth_st.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2024-05-13 12:22:11.000000 google-auth-st-0.2/google_auth_st.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 12:22:11.000000 google-auth-st-0.2/google_auth_st.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-05-13 12:22:11.000000 google-auth-st-0.2/google_auth_st.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 12:22:11.000000 google-auth-st-0.2/google_auth_st.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 12:22:11.613836 google-auth-st-0.2/setup.cfg
--rw-rw-rw-   0        0        0      599 2024-05-13 12:13:56.000000 google-auth-st-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 13:59:00.048537 google-auth-st-0.3/
+-rw-rw-rw-   0        0        0     1065 2024-05-10 14:11:09.000000 google-auth-st-0.3/LICENSE
+-rw-rw-rw-   0        0        0     1831 2024-05-13 13:59:00.047536 google-auth-st-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1478 2024-05-10 14:20:05.000000 google-auth-st-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 13:59:00.006537 google-auth-st-0.3/google_auth_st/
+-rw-rw-rw-   0        0        0       35 2024-05-13 13:58:10.000000 google-auth-st-0.3/google_auth_st/__init__.py
+-rw-rw-rw-   0        0        0      567 2024-05-13 11:51:11.000000 google-auth-st-0.3/google_auth_st/aggregate_auth.py
+-rw-rw-rw-   0        0        0     3186 2024-05-12 21:15:40.000000 google-auth-st-0.3/google_auth_st/google_auth.py
+drwxrwxrwx   0        0        0        0 2024-05-13 13:59:00.045535 google-auth-st-0.3/google_auth_st.egg-info/
+-rw-rw-rw-   0        0        0     1831 2024-05-13 13:58:59.000000 google-auth-st-0.3/google_auth_st.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-13 13:58:59.000000 google-auth-st-0.3/google_auth_st.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 13:58:59.000000 google-auth-st-0.3/google_auth_st.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-13 13:58:59.000000 google-auth-st-0.3/google_auth_st.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-13 13:58:59.000000 google-auth-st-0.3/google_auth_st.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 13:59:00.048537 google-auth-st-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      603 2024-05-13 13:54:44.000000 google-auth-st-0.3/setup.py
```

### Comparing `google-auth-st-0.2/LICENSE` & `google-auth-st-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-auth-st-0.2/PKG-INFO` & `google-auth-st-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-auth-st
-Version: 0.2
+Version: 0.3
 Summary: Librería para añadir autenticación con Google en aplicaciones web con el framework de Streamlit.
 Home-page: https://github.com/valantoni/google-auth-st.git
 Author: Toni Dev
 Author-email: classtonidev@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `google-auth-st-0.2/README.md` & `google-auth-st-0.3/README.md`

 * *Files identical despite different names*

### Comparing `google-auth-st-0.2/google_auth_st.egg-info/PKG-INFO` & `google-auth-st-0.3/google_auth_st.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-auth-st
-Version: 0.2
+Version: 0.3
 Summary: Librería para añadir autenticación con Google en aplicaciones web con el framework de Streamlit.
 Home-page: https://github.com/valantoni/google-auth-st.git
 Author: Toni Dev
 Author-email: classtonidev@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `google-auth-st-0.2/setup.py` & `google-auth-st-0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='google-auth-st',
-    version='0.2',
-    packages=find_packages(),
+    version='0.3',
+    packages= ['google_auth_st'],
     description='Librería para añadir autenticación con Google en aplicaciones web con el framework de Streamlit.',
     long_description=open('README.md',encoding='utf-8').read(),
     long_description_content_type='text/markdown',  
     author='Toni Dev',
     author_email='classtonidev@gmail.com',
     url='https://github.com/valantoni/google-auth-st.git',
     install_requires=[
```

