# Comparing `tmp/st_signedurl_uploader-1.2.tar.gz` & `tmp/st_signedurl_uploader-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_signedurl_uploader-1.2.tar", last modified: Mon May 13 09:32:13 2024, max compression
+gzip compressed data, was "st_signedurl_uploader-1.2.1.tar", last modified: Mon May 13 09:36:25 2024, max compression
```

## Comparing `st_signedurl_uploader-1.2.tar` & `st_signedurl_uploader-1.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:32:13.494417 st_signedurl_uploader-1.2/
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     1063 2024-04-10 04:21:46.000000 st_signedurl_uploader-1.2/LICENSE
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)       57 2024-05-13 09:21:19.000000 st_signedurl_uploader-1.2/MANIFEST.in
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     5021 2024-05-13 09:32:13.494097 st_signedurl_uploader-1.2/PKG-INFO
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     4353 2024-05-13 09:31:22.000000 st_signedurl_uploader-1.2/README.md
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)       38 2024-05-13 09:32:13.494500 st_signedurl_uploader-1.2/setup.cfg
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)      925 2024-05-13 09:31:55.000000 st_signedurl_uploader-1.2/setup.py
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:32:13.484785 st_signedurl_uploader-1.2/st-signedUrl-uploader/
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     2612 2024-05-13 08:18:08.000000 st_signedurl_uploader-1.2/st-signedUrl-uploader/__init__.py
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:32:13.483225 st_signedurl_uploader-1.2/st-signedUrl-uploader/frontend/
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:32:13.486441 st_signedurl_uploader-1.2/st-signedUrl-uploader/frontend/build/
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)      221 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2/st-signedUrl-uploader/frontend/build/asset-manifest.json
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)   197413 2024-05-11 08:08:11.000000 st_signedurl_uploader-1.2/st-signedUrl-uploader/frontend/build/bootstrap.min.css
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)      492 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2/st-signedUrl-uploader/frontend/build/index.html
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:32:13.483489 st_signedurl_uploader-1.2/st-signedUrl-uploader/frontend/build/static/
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:32:13.488537 st_signedurl_uploader-1.2/st-signedUrl-uploader/frontend/build/static/js/
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)   317963 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2/st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     1293 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2/st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js.LICENSE.txt
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)  1248762 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2/st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js.map
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:32:13.492930 st_signedurl_uploader-1.2/st_signedUrl_uploader.egg-info/
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     5021 2024-05-13 09:32:13.000000 st_signedurl_uploader-1.2/st_signedUrl_uploader.egg-info/PKG-INFO
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)      664 2024-05-13 09:32:13.000000 st_signedurl_uploader-1.2/st_signedUrl_uploader.egg-info/SOURCES.txt
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)        1 2024-05-13 09:32:13.000000 st_signedurl_uploader-1.2/st_signedUrl_uploader.egg-info/dependency_links.txt
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)      140 2024-05-13 09:32:13.000000 st_signedurl_uploader-1.2/st_signedUrl_uploader.egg-info/requires.txt
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)       22 2024-05-13 09:32:13.000000 st_signedurl_uploader-1.2/st_signedUrl_uploader.egg-info/top_level.txt
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:36:25.593554 st_signedurl_uploader-1.2.1/
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     1063 2024-04-10 04:21:46.000000 st_signedurl_uploader-1.2.1/LICENSE
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)       57 2024-05-13 09:21:19.000000 st_signedurl_uploader-1.2.1/MANIFEST.in
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     5021 2024-05-13 09:36:25.593236 st_signedurl_uploader-1.2.1/PKG-INFO
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     4351 2024-05-13 09:34:20.000000 st_signedurl_uploader-1.2.1/README.md
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)       38 2024-05-13 09:36:25.593645 st_signedurl_uploader-1.2.1/setup.cfg
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)      927 2024-05-13 09:36:06.000000 st_signedurl_uploader-1.2.1/setup.py
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:36:25.583854 st_signedurl_uploader-1.2.1/st-signedUrl-uploader/
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     2612 2024-05-13 08:18:08.000000 st_signedurl_uploader-1.2.1/st-signedUrl-uploader/__init__.py
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:36:25.582229 st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:36:25.585702 st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/build/
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)      221 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/build/asset-manifest.json
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)   197413 2024-05-11 08:08:11.000000 st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/build/bootstrap.min.css
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)      492 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/build/index.html
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:36:25.582457 st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/build/static/
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:36:25.588163 st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/build/static/js/
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)   317963 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     1293 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js.LICENSE.txt
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)  1248762 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js.map
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:36:25.592403 st_signedurl_uploader-1.2.1/st_signedUrl_uploader.egg-info/
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     5021 2024-05-13 09:36:25.000000 st_signedurl_uploader-1.2.1/st_signedUrl_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)      664 2024-05-13 09:36:25.000000 st_signedurl_uploader-1.2.1/st_signedUrl_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)        1 2024-05-13 09:36:25.000000 st_signedurl_uploader-1.2.1/st_signedUrl_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)      140 2024-05-13 09:36:25.000000 st_signedurl_uploader-1.2.1/st_signedUrl_uploader.egg-info/requires.txt
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)       22 2024-05-13 09:36:25.000000 st_signedurl_uploader-1.2.1/st_signedUrl_uploader.egg-info/top_level.txt
```

### Comparing `st_signedurl_uploader-1.2/LICENSE` & `st_signedurl_uploader-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.2/PKG-INFO` & `st_signedurl_uploader-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-signedUrl-uploader
-Version: 1.2
+Version: 1.2.1
 Summary: Streamlit component that allows you to upload files to Google Cloud Storage via signed url
 Home-page: 
 Author: Meryam Assermouh
 Author-email: 
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -47,15 +47,15 @@
 ```
 Example CORS configuration file can be found in [CORS.json](https://github.com/Meryam-A/signed-url-uploader/blob/main/CORS.json) or create your own based on [Google Cloud Documentation](https://cloud.google.com/storage/docs/cross-origin)
 
 ### Implementation : 
 - **Service Account Permissions:** Ensure the App Engine or Cloud Run service account has the `roles/iam.serviceAccountTokenCreator` role for generating signed URLs.
 - **Install Cloud Storage library:** 
 ```
-pip install st-signedUrl-uploader
+pip install google-cloud-storage
 ```
 #### Sample Code :
 
 ```python
 from st-signedUrl-uploader import signedUrl_uploader
 from google import auth
 from google.cloud import storage
@@ -88,15 +88,15 @@
 ```
 Example CORS configuration file can be found in [CORS.json](https://github.com/Meryam-A/signed-url-uploader/blob/main/CORS.json) or create your own based on [Google Cloud Documentation](https://cloud.google.com/storage/docs/cross-origin)
 
 ### Implementation : 
 - Create a service account and give it the role `roles/iam.serviceAccountTokenCreator`
 - **Install Cloud Storage library:** 
 ```
-pip install st-signedUrl-uploader
+pip install google-cloud-storage
 ```
 #### Sample Code :
 
 ```python
 from st-signedUrl-uploader import signedUrl_uploader
 from google import auth
 from google.cloud import storage
```

### Comparing `st_signedurl_uploader-1.2/README.md` & `st_signedurl_uploader-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ```
 Example CORS configuration file can be found in [CORS.json](https://github.com/Meryam-A/signed-url-uploader/blob/main/CORS.json) or create your own based on [Google Cloud Documentation](https://cloud.google.com/storage/docs/cross-origin)
 
 ### Implementation : 
 - **Service Account Permissions:** Ensure the App Engine or Cloud Run service account has the `roles/iam.serviceAccountTokenCreator` role for generating signed URLs.
 - **Install Cloud Storage library:** 
 ```
-pip install st-signedUrl-uploader
+pip install google-cloud-storage
 ```
 #### Sample Code :
 
 ```python
 from st-signedUrl-uploader import signedUrl_uploader
 from google import auth
 from google.cloud import storage
@@ -69,15 +69,15 @@
 ```
 Example CORS configuration file can be found in [CORS.json](https://github.com/Meryam-A/signed-url-uploader/blob/main/CORS.json) or create your own based on [Google Cloud Documentation](https://cloud.google.com/storage/docs/cross-origin)
 
 ### Implementation : 
 - Create a service account and give it the role `roles/iam.serviceAccountTokenCreator`
 - **Install Cloud Storage library:** 
 ```
-pip install st-signedUrl-uploader
+pip install google-cloud-storage
 ```
 #### Sample Code :
 
 ```python
 from st-signedUrl-uploader import signedUrl_uploader
 from google import auth
 from google.cloud import storage
```

### Comparing `st_signedurl_uploader-1.2/setup.py` & `st_signedurl_uploader-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="st-signedUrl-uploader",
-    version="1.2",
+    version="1.2.1",
     author="Meryam Assermouh",
     author_email="",
     description="Streamlit component that allows you to upload files to Google Cloud Storage via signed url",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st_signedurl_uploader-1.2/st-signedUrl-uploader/__init__.py` & `st_signedurl_uploader-1.2.1/st-signedUrl-uploader/__init__.py`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.2/st-signedUrl-uploader/frontend/build/bootstrap.min.css` & `st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.2/st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js` & `st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.2/st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js.LICENSE.txt` & `st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.2/st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js.map` & `st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js.map`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.2/st_signedUrl_uploader.egg-info/PKG-INFO` & `st_signedurl_uploader-1.2.1/st_signedUrl_uploader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-signedUrl-uploader
-Version: 1.2
+Version: 1.2.1
 Summary: Streamlit component that allows you to upload files to Google Cloud Storage via signed url
 Home-page: 
 Author: Meryam Assermouh
 Author-email: 
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -47,15 +47,15 @@
 ```
 Example CORS configuration file can be found in [CORS.json](https://github.com/Meryam-A/signed-url-uploader/blob/main/CORS.json) or create your own based on [Google Cloud Documentation](https://cloud.google.com/storage/docs/cross-origin)
 
 ### Implementation : 
 - **Service Account Permissions:** Ensure the App Engine or Cloud Run service account has the `roles/iam.serviceAccountTokenCreator` role for generating signed URLs.
 - **Install Cloud Storage library:** 
 ```
-pip install st-signedUrl-uploader
+pip install google-cloud-storage
 ```
 #### Sample Code :
 
 ```python
 from st-signedUrl-uploader import signedUrl_uploader
 from google import auth
 from google.cloud import storage
@@ -88,15 +88,15 @@
 ```
 Example CORS configuration file can be found in [CORS.json](https://github.com/Meryam-A/signed-url-uploader/blob/main/CORS.json) or create your own based on [Google Cloud Documentation](https://cloud.google.com/storage/docs/cross-origin)
 
 ### Implementation : 
 - Create a service account and give it the role `roles/iam.serviceAccountTokenCreator`
 - **Install Cloud Storage library:** 
 ```
-pip install st-signedUrl-uploader
+pip install google-cloud-storage
 ```
 #### Sample Code :
 
 ```python
 from st-signedUrl-uploader import signedUrl_uploader
 from google import auth
 from google.cloud import storage
```

### Comparing `st_signedurl_uploader-1.2/st_signedUrl_uploader.egg-info/SOURCES.txt` & `st_signedurl_uploader-1.2.1/st_signedUrl_uploader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

