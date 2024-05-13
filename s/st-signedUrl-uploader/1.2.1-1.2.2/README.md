# Comparing `tmp/st_signedurl_uploader-1.2.1.tar.gz` & `tmp/st_signedurl_uploader-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_signedurl_uploader-1.2.1.tar", last modified: Mon May 13 09:36:25 2024, max compression
+gzip compressed data, was "st_signedurl_uploader-1.2.2.tar", last modified: Mon May 13 09:49:37 2024, max compression
```

## Comparing `st_signedurl_uploader-1.2.1.tar` & `st_signedurl_uploader-1.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:36:25.593554 st_signedurl_uploader-1.2.1/
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     1063 2024-04-10 04:21:46.000000 st_signedurl_uploader-1.2.1/LICENSE
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)       57 2024-05-13 09:21:19.000000 st_signedurl_uploader-1.2.1/MANIFEST.in
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     5021 2024-05-13 09:36:25.593236 st_signedurl_uploader-1.2.1/PKG-INFO
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     4351 2024-05-13 09:34:20.000000 st_signedurl_uploader-1.2.1/README.md
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)       38 2024-05-13 09:36:25.593645 st_signedurl_uploader-1.2.1/setup.cfg
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)      927 2024-05-13 09:36:06.000000 st_signedurl_uploader-1.2.1/setup.py
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:36:25.583854 st_signedurl_uploader-1.2.1/st-signedUrl-uploader/
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     2612 2024-05-13 08:18:08.000000 st_signedurl_uploader-1.2.1/st-signedUrl-uploader/__init__.py
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:36:25.582229 st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:36:25.585702 st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/build/
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)      221 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/build/asset-manifest.json
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)   197413 2024-05-11 08:08:11.000000 st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/build/bootstrap.min.css
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)      492 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/build/index.html
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:36:25.582457 st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/build/static/
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:36:25.588163 st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/build/static/js/
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)   317963 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     1293 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js.LICENSE.txt
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)  1248762 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js.map
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:36:25.592403 st_signedurl_uploader-1.2.1/st_signedUrl_uploader.egg-info/
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     5021 2024-05-13 09:36:25.000000 st_signedurl_uploader-1.2.1/st_signedUrl_uploader.egg-info/PKG-INFO
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)      664 2024-05-13 09:36:25.000000 st_signedurl_uploader-1.2.1/st_signedUrl_uploader.egg-info/SOURCES.txt
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)        1 2024-05-13 09:36:25.000000 st_signedurl_uploader-1.2.1/st_signedUrl_uploader.egg-info/dependency_links.txt
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)      140 2024-05-13 09:36:25.000000 st_signedurl_uploader-1.2.1/st_signedUrl_uploader.egg-info/requires.txt
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)       22 2024-05-13 09:36:25.000000 st_signedurl_uploader-1.2.1/st_signedUrl_uploader.egg-info/top_level.txt
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:49:37.861547 st_signedurl_uploader-1.2.2/
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     1063 2024-04-10 04:21:46.000000 st_signedurl_uploader-1.2.2/LICENSE
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)       57 2024-05-13 09:49:00.000000 st_signedurl_uploader-1.2.2/MANIFEST.in
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     5021 2024-05-13 09:49:37.861228 st_signedurl_uploader-1.2.2/PKG-INFO
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     4351 2024-05-13 09:48:53.000000 st_signedurl_uploader-1.2.2/README.md
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)       38 2024-05-13 09:49:37.861621 st_signedurl_uploader-1.2.2/setup.cfg
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)      927 2024-05-13 09:49:09.000000 st_signedurl_uploader-1.2.2/setup.py
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:49:37.851802 st_signedurl_uploader-1.2.2/st_signedUrl_uploader/
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     2612 2024-05-13 08:18:08.000000 st_signedurl_uploader-1.2.2/st_signedUrl_uploader/__init__.py
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:49:37.850336 st_signedurl_uploader-1.2.2/st_signedUrl_uploader/frontend/
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:49:37.854487 st_signedurl_uploader-1.2.2/st_signedUrl_uploader/frontend/build/
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)      221 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2.2/st_signedUrl_uploader/frontend/build/asset-manifest.json
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)   197413 2024-05-11 08:08:11.000000 st_signedurl_uploader-1.2.2/st_signedUrl_uploader/frontend/build/bootstrap.min.css
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)      492 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2.2/st_signedUrl_uploader/frontend/build/index.html
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:49:37.850548 st_signedurl_uploader-1.2.2/st_signedUrl_uploader/frontend/build/static/
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:49:37.856682 st_signedurl_uploader-1.2.2/st_signedUrl_uploader/frontend/build/static/js/
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)   317963 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2.2/st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     1293 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2.2/st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js.LICENSE.txt
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)  1248762 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2.2/st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js.map
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:49:37.860078 st_signedurl_uploader-1.2.2/st_signedUrl_uploader.egg-info/
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     5021 2024-05-13 09:49:37.000000 st_signedurl_uploader-1.2.2/st_signedUrl_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)      664 2024-05-13 09:49:37.000000 st_signedurl_uploader-1.2.2/st_signedUrl_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)        1 2024-05-13 09:49:37.000000 st_signedurl_uploader-1.2.2/st_signedUrl_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)      140 2024-05-13 09:49:37.000000 st_signedurl_uploader-1.2.2/st_signedUrl_uploader.egg-info/requires.txt
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)       22 2024-05-13 09:49:37.000000 st_signedurl_uploader-1.2.2/st_signedUrl_uploader.egg-info/top_level.txt
```

### Comparing `st_signedurl_uploader-1.2.1/LICENSE` & `st_signedurl_uploader-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.2.1/PKG-INFO` & `st_signedurl_uploader-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-signedUrl-uploader
-Version: 1.2.1
+Version: 1.2.2
 Summary: Streamlit component that allows you to upload files to Google Cloud Storage via signed url
 Home-page: 
 Author: Meryam Assermouh
 Author-email: 
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -26,15 +26,15 @@
 Considering the schema below, the Signed Url Uploader abstracts away steps 2 and 3. Check this article for more details.
 <img width="822" alt="image" src="https://github.com/Meryam-A/signed-url-uploader/assets/166532696/615e35a9-ab78-45ea-916f-0a2dd3e45bb2">
 
 ## Installation
 
 You can install the latest release using:
 ```
-pip install st-signedUrl-uploader
+pip install st_signedUrl_uploader
 ```
 
 ## Usage 
 This component serves as an efficient uploader for applications that are deployed on App Engine or Cloud Run, specifically designed to handle large file uploads by utilizing Google Cloud Storage (GCS) and signed URLs. To facilitate ease of integration and testing, the component can be used in two ways: directly in cloud deployments or locally using a service account for development and testing purposes. Below, you will find detailed instructions for both scenarios, including sample code and a list of infrastructure prerequisites necessary to ensure smooth operation and integration of the uploader in your projects.
 
 ### Usage with App Engine or Cloud Run
 
@@ -52,15 +52,15 @@
 - **Install Cloud Storage library:** 
 ```
 pip install google-cloud-storage
 ```
 #### Sample Code :
 
 ```python
-from st-signedUrl-uploader import signedUrl_uploader
+from st_signedUrl_uploader import signedUrl_uploader
 from google import auth
 from google.cloud import storage
 
 def main():
   bucket_name = "your-bucket-name" # Specify your GCS bucket name here
 
   # Authenticate and create a storage client
@@ -93,15 +93,15 @@
 - **Install Cloud Storage library:** 
 ```
 pip install google-cloud-storage
 ```
 #### Sample Code :
 
 ```python
-from st-signedUrl-uploader import signedUrl_uploader
+from st_signedUrl_uploader import signedUrl_uploader
 from google import auth
 from google.cloud import storage
 import os
 
 def main():
   bucket_name = "your-bucket-name"  # Specify your GCS bucket name here
```

### Comparing `st_signedurl_uploader-1.2.1/README.md` & `st_signedurl_uploader-1.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Considering the schema below, the Signed Url Uploader abstracts away steps 2 and 3. Check this article for more details.
 <img width="822" alt="image" src="https://github.com/Meryam-A/signed-url-uploader/assets/166532696/615e35a9-ab78-45ea-916f-0a2dd3e45bb2">
 
 ## Installation
 
 You can install the latest release using:
 ```
-pip install st-signedUrl-uploader
+pip install st_signedUrl_uploader
 ```
 
 ## Usage 
 This component serves as an efficient uploader for applications that are deployed on App Engine or Cloud Run, specifically designed to handle large file uploads by utilizing Google Cloud Storage (GCS) and signed URLs. To facilitate ease of integration and testing, the component can be used in two ways: directly in cloud deployments or locally using a service account for development and testing purposes. Below, you will find detailed instructions for both scenarios, including sample code and a list of infrastructure prerequisites necessary to ensure smooth operation and integration of the uploader in your projects.
 
 ### Usage with App Engine or Cloud Run
 
@@ -33,15 +33,15 @@
 - **Install Cloud Storage library:** 
 ```
 pip install google-cloud-storage
 ```
 #### Sample Code :
 
 ```python
-from st-signedUrl-uploader import signedUrl_uploader
+from st_signedUrl_uploader import signedUrl_uploader
 from google import auth
 from google.cloud import storage
 
 def main():
   bucket_name = "your-bucket-name" # Specify your GCS bucket name here
 
   # Authenticate and create a storage client
@@ -74,15 +74,15 @@
 - **Install Cloud Storage library:** 
 ```
 pip install google-cloud-storage
 ```
 #### Sample Code :
 
 ```python
-from st-signedUrl-uploader import signedUrl_uploader
+from st_signedUrl_uploader import signedUrl_uploader
 from google import auth
 from google.cloud import storage
 import os
 
 def main():
   bucket_name = "your-bucket-name"  # Specify your GCS bucket name here
```

### Comparing `st_signedurl_uploader-1.2.1/setup.py` & `st_signedurl_uploader-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="st-signedUrl-uploader",
-    version="1.2.1",
+    version="1.2.2",
     author="Meryam Assermouh",
     author_email="",
     description="Streamlit component that allows you to upload files to Google Cloud Storage via signed url",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st_signedurl_uploader-1.2.1/st-signedUrl-uploader/__init__.py` & `st_signedurl_uploader-1.2.2/st_signedUrl_uploader/__init__.py`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/build/bootstrap.min.css` & `st_signedurl_uploader-1.2.2/st_signedUrl_uploader/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js` & `st_signedurl_uploader-1.2.2/st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js.LICENSE.txt` & `st_signedurl_uploader-1.2.2/st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.2.1/st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js.map` & `st_signedurl_uploader-1.2.2/st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js.map`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.2.1/st_signedUrl_uploader.egg-info/PKG-INFO` & `st_signedurl_uploader-1.2.2/st_signedUrl_uploader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-signedUrl-uploader
-Version: 1.2.1
+Version: 1.2.2
 Summary: Streamlit component that allows you to upload files to Google Cloud Storage via signed url
 Home-page: 
 Author: Meryam Assermouh
 Author-email: 
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -26,15 +26,15 @@
 Considering the schema below, the Signed Url Uploader abstracts away steps 2 and 3. Check this article for more details.
 <img width="822" alt="image" src="https://github.com/Meryam-A/signed-url-uploader/assets/166532696/615e35a9-ab78-45ea-916f-0a2dd3e45bb2">
 
 ## Installation
 
 You can install the latest release using:
 ```
-pip install st-signedUrl-uploader
+pip install st_signedUrl_uploader
 ```
 
 ## Usage 
 This component serves as an efficient uploader for applications that are deployed on App Engine or Cloud Run, specifically designed to handle large file uploads by utilizing Google Cloud Storage (GCS) and signed URLs. To facilitate ease of integration and testing, the component can be used in two ways: directly in cloud deployments or locally using a service account for development and testing purposes. Below, you will find detailed instructions for both scenarios, including sample code and a list of infrastructure prerequisites necessary to ensure smooth operation and integration of the uploader in your projects.
 
 ### Usage with App Engine or Cloud Run
 
@@ -52,15 +52,15 @@
 - **Install Cloud Storage library:** 
 ```
 pip install google-cloud-storage
 ```
 #### Sample Code :
 
 ```python
-from st-signedUrl-uploader import signedUrl_uploader
+from st_signedUrl_uploader import signedUrl_uploader
 from google import auth
 from google.cloud import storage
 
 def main():
   bucket_name = "your-bucket-name" # Specify your GCS bucket name here
 
   # Authenticate and create a storage client
@@ -93,15 +93,15 @@
 - **Install Cloud Storage library:** 
 ```
 pip install google-cloud-storage
 ```
 #### Sample Code :
 
 ```python
-from st-signedUrl-uploader import signedUrl_uploader
+from st_signedUrl_uploader import signedUrl_uploader
 from google import auth
 from google.cloud import storage
 import os
 
 def main():
   bucket_name = "your-bucket-name"  # Specify your GCS bucket name here
```

### Comparing `st_signedurl_uploader-1.2.1/st_signedUrl_uploader.egg-info/SOURCES.txt` & `st_signedurl_uploader-1.2.2/st_signedUrl_uploader.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
-st-signedUrl-uploader/__init__.py
-st-signedUrl-uploader/frontend/build/asset-manifest.json
-st-signedUrl-uploader/frontend/build/bootstrap.min.css
-st-signedUrl-uploader/frontend/build/index.html
-st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js
-st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js.LICENSE.txt
-st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js.map
+st_signedUrl_uploader/__init__.py
 st_signedUrl_uploader.egg-info/PKG-INFO
 st_signedUrl_uploader.egg-info/SOURCES.txt
 st_signedUrl_uploader.egg-info/dependency_links.txt
 st_signedUrl_uploader.egg-info/requires.txt
-st_signedUrl_uploader.egg-info/top_level.txt
+st_signedUrl_uploader.egg-info/top_level.txt
+st_signedUrl_uploader/frontend/build/asset-manifest.json
+st_signedUrl_uploader/frontend/build/bootstrap.min.css
+st_signedUrl_uploader/frontend/build/index.html
+st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js
+st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js.LICENSE.txt
+st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js.map
```

