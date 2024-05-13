# Comparing `tmp/google_auth_st-0.1.tar.gz` & `tmp/google-auth-st-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_auth_st-0.1.tar", last modified: Mon May 13 09:27:31 2024, max compression
+gzip compressed data, was "google-auth-st-0.2.tar", last modified: Mon May 13 12:22:11 2024, max compression
```

## Comparing `google_auth_st-0.1.tar` & `google-auth-st-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 09:27:31.782592 google_auth_st-0.1/
--rw-rw-rw-   0        0        0     1065 2024-05-10 14:11:09.000000 google_auth_st-0.1/LICENSE
--rw-rw-rw-   0        0        0     1831 2024-05-13 09:27:31.781590 google_auth_st-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1478 2024-05-10 14:20:05.000000 google_auth_st-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 09:27:31.779590 google_auth_st-0.1/google_auth_st.egg-info/
--rw-rw-rw-   0        0        0     1831 2024-05-13 09:27:31.000000 google_auth_st-0.1/google_auth_st.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2024-05-13 09:27:31.000000 google_auth_st-0.1/google_auth_st.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 09:27:31.000000 google_auth_st-0.1/google_auth_st.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-05-13 09:27:31.000000 google_auth_st-0.1/google_auth_st.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 09:27:31.000000 google_auth_st-0.1/google_auth_st.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 09:27:31.783681 google_auth_st-0.1/setup.cfg
--rw-rw-rw-   0        0        0      597 2024-05-13 08:41:54.000000 google_auth_st-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 12:22:11.613491 google-auth-st-0.2/
+-rw-rw-rw-   0        0        0     1065 2024-05-10 14:11:09.000000 google-auth-st-0.2/LICENSE
+-rw-rw-rw-   0        0        0     1831 2024-05-13 12:22:11.612490 google-auth-st-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1478 2024-05-10 14:20:05.000000 google-auth-st-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 12:22:11.610490 google-auth-st-0.2/google_auth_st.egg-info/
+-rw-rw-rw-   0        0        0     1831 2024-05-13 12:22:11.000000 google-auth-st-0.2/google_auth_st.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2024-05-13 12:22:11.000000 google-auth-st-0.2/google_auth_st.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 12:22:11.000000 google-auth-st-0.2/google_auth_st.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-13 12:22:11.000000 google-auth-st-0.2/google_auth_st.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 12:22:11.000000 google-auth-st-0.2/google_auth_st.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 12:22:11.613836 google-auth-st-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      599 2024-05-13 12:13:56.000000 google-auth-st-0.2/setup.py
```

### Comparing `google_auth_st-0.1/LICENSE` & `google-auth-st-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google_auth_st-0.1/PKG-INFO` & `google-auth-st-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: google_auth_st
-Version: 0.1
+Name: google-auth-st
+Version: 0.2
 Summary: Librería para añadir autenticación con Google en aplicaciones web con el framework de Streamlit.
 Home-page: https://github.com/valantoni/google-auth-st.git
 Author: Toni Dev
 Author-email: classtonidev@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `google_auth_st-0.1/README.md` & `google-auth-st-0.2/README.md`

 * *Files identical despite different names*

### Comparing `google_auth_st-0.1/google_auth_st.egg-info/PKG-INFO` & `google-auth-st-0.2/google_auth_st.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-auth-st
-Version: 0.1
+Version: 0.2
 Summary: Librería para añadir autenticación con Google en aplicaciones web con el framework de Streamlit.
 Home-page: https://github.com/valantoni/google-auth-st.git
 Author: Toni Dev
 Author-email: classtonidev@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `google_auth_st-0.1/setup.py` & `google-auth-st-0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='google_auth_st',
-    version='0.1',
+    name='google-auth-st',
+    version='0.2',
     packages=find_packages(),
     description='Librería para añadir autenticación con Google en aplicaciones web con el framework de Streamlit.',
     long_description=open('README.md',encoding='utf-8').read(),
     long_description_content_type='text/markdown',  
     author='Toni Dev',
     author_email='classtonidev@gmail.com',
     url='https://github.com/valantoni/google-auth-st.git',
     install_requires=[
         'streamlit',
         'httpx_oauth',
         'PyJWT'
     ],
-)
+)
```

