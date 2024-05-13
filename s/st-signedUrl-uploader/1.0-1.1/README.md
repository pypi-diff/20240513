# Comparing `tmp/st_signedurl_uploader-1.0.tar.gz` & `tmp/st_signedurl_uploader-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_signedurl_uploader-1.0.tar", last modified: Mon May 13 08:20:19 2024, max compression
+gzip compressed data, was "st_signedurl_uploader-1.1.tar", last modified: Mon May 13 09:26:00 2024, max compression
```

## Comparing `st_signedurl_uploader-1.0.tar` & `st_signedurl_uploader-1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 08:20:19.305497 st_signedurl_uploader-1.0/
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     1063 2024-04-10 04:21:46.000000 st_signedurl_uploader-1.0/LICENSE
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)       57 2024-05-08 09:44:56.000000 st_signedurl_uploader-1.0/MANIFEST.in
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     4785 2024-05-13 08:20:19.305198 st_signedurl_uploader-1.0/PKG-INFO
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     4118 2024-05-13 08:18:02.000000 st_signedurl_uploader-1.0/README.md
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)       38 2024-05-13 08:20:19.305567 st_signedurl_uploader-1.0/setup.cfg
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)      925 2024-05-13 08:19:22.000000 st_signedurl_uploader-1.0/setup.py
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 08:20:19.295722 st_signedurl_uploader-1.0/st_signedUrl_uploader/
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     2612 2024-05-13 08:18:08.000000 st_signedurl_uploader-1.0/st_signedUrl_uploader/__init__.py
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 08:20:19.294242 st_signedurl_uploader-1.0/st_signedUrl_uploader/frontend/
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 08:20:19.298742 st_signedurl_uploader-1.0/st_signedUrl_uploader/frontend/build/
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)      221 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.0/st_signedUrl_uploader/frontend/build/asset-manifest.json
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)   197413 2024-05-11 08:08:11.000000 st_signedurl_uploader-1.0/st_signedUrl_uploader/frontend/build/bootstrap.min.css
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)      492 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.0/st_signedUrl_uploader/frontend/build/index.html
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 08:20:19.294470 st_signedurl_uploader-1.0/st_signedUrl_uploader/frontend/build/static/
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 08:20:19.300895 st_signedurl_uploader-1.0/st_signedUrl_uploader/frontend/build/static/js/
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)   317963 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.0/st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     1293 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.0/st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js.LICENSE.txt
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)  1248762 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.0/st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js.map
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 08:20:19.304059 st_signedurl_uploader-1.0/st_signedUrl_uploader.egg-info/
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     4785 2024-05-13 08:20:19.000000 st_signedurl_uploader-1.0/st_signedUrl_uploader.egg-info/PKG-INFO
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)      664 2024-05-13 08:20:19.000000 st_signedurl_uploader-1.0/st_signedUrl_uploader.egg-info/SOURCES.txt
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)        1 2024-05-13 08:20:19.000000 st_signedurl_uploader-1.0/st_signedUrl_uploader.egg-info/dependency_links.txt
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)      140 2024-05-13 08:20:19.000000 st_signedurl_uploader-1.0/st_signedUrl_uploader.egg-info/requires.txt
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)       22 2024-05-13 08:20:19.000000 st_signedurl_uploader-1.0/st_signedUrl_uploader.egg-info/top_level.txt
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:26:00.051909 st_signedurl_uploader-1.1/
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     1063 2024-04-10 04:21:46.000000 st_signedurl_uploader-1.1/LICENSE
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)       57 2024-05-13 09:21:19.000000 st_signedurl_uploader-1.1/MANIFEST.in
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     4871 2024-05-13 09:26:00.051587 st_signedurl_uploader-1.1/PKG-INFO
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     4203 2024-05-13 09:12:17.000000 st_signedurl_uploader-1.1/README.md
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)       38 2024-05-13 09:26:00.051990 st_signedurl_uploader-1.1/setup.cfg
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)      925 2024-05-13 09:25:00.000000 st_signedurl_uploader-1.1/setup.py
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:26:00.041592 st_signedurl_uploader-1.1/st-signedUrl-uploader/
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     2612 2024-05-13 08:18:08.000000 st_signedurl_uploader-1.1/st-signedUrl-uploader/__init__.py
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:26:00.039741 st_signedurl_uploader-1.1/st-signedUrl-uploader/frontend/
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:26:00.043845 st_signedurl_uploader-1.1/st-signedUrl-uploader/frontend/build/
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)      221 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.1/st-signedUrl-uploader/frontend/build/asset-manifest.json
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)   197413 2024-05-11 08:08:11.000000 st_signedurl_uploader-1.1/st-signedUrl-uploader/frontend/build/bootstrap.min.css
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)      492 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.1/st-signedUrl-uploader/frontend/build/index.html
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:26:00.039947 st_signedurl_uploader-1.1/st-signedUrl-uploader/frontend/build/static/
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:26:00.046005 st_signedurl_uploader-1.1/st-signedUrl-uploader/frontend/build/static/js/
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)   317963 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.1/st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     1293 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.1/st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js.LICENSE.txt
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)  1248762 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.1/st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js.map
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 09:26:00.050568 st_signedurl_uploader-1.1/st_signedUrl_uploader.egg-info/
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     4871 2024-05-13 09:26:00.000000 st_signedurl_uploader-1.1/st_signedUrl_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)      664 2024-05-13 09:26:00.000000 st_signedurl_uploader-1.1/st_signedUrl_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)        1 2024-05-13 09:26:00.000000 st_signedurl_uploader-1.1/st_signedUrl_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)      140 2024-05-13 09:26:00.000000 st_signedurl_uploader-1.1/st_signedUrl_uploader.egg-info/requires.txt
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)       22 2024-05-13 09:26:00.000000 st_signedurl_uploader-1.1/st_signedUrl_uploader.egg-info/top_level.txt
```

### Comparing `st_signedurl_uploader-1.0/LICENSE` & `st_signedurl_uploader-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.0/PKG-INFO` & `st_signedurl_uploader-1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: st_signedUrl_uploader
-Version: 1.0
+Name: st-signedUrl-uploader
+Version: 1.1
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
-pip install st_signedUrl_uploader
+pip install st-signedUrl-uploader
 ```
 
 ## Usage 
 This component serves as an efficient uploader for applications that are deployed on App Engine or Cloud Run, specifically designed to handle large file uploads by utilizing Google Cloud Storage (GCS) and signed URLs. To facilitate ease of integration and testing, the component can be used in two ways: directly in cloud deployments or locally using a service account for development and testing purposes. Below, you will find detailed instructions for both scenarios, including sample code and a list of infrastructure prerequisites necessary to ensure smooth operation and integration of the uploader in your projects.
 
 ### Usage with App Engine or Cloud Run
 
@@ -49,15 +49,15 @@
 
 ### Implementation : 
 - **Service Account Permissions:** Ensure the App Engine or Cloud Run service account has the `roles/iam.serviceAccountTokenCreator` role for generating signed URLs.
     
 #### Sample Code :
 
 ```python
-from st_signedUrl_uploader import signedUrl_uploader
+from st-signedUrl-uploader import signedUrl_uploader
 from google import auth
 from google.cloud import storage
 
 def main():
   bucket_name = "your-bucket-name" # Specify your GCS bucket name here
 
   # Authenticate and create a storage client
@@ -87,15 +87,15 @@
 
 ### Implementation : 
 - Create a service account and give it the role `roles/iam.serviceAccountTokenCreator`
     
 #### Sample Code :
 
 ```python
-from st_signedUrl_uploader import signedUrl_uploader
+from st-signedUrl-uploader import signedUrl_uploader
 from google import auth
 from google.cloud import storage
 import os
 
 def main():
   bucket_name = "your-bucket-name"  # Specify your GCS bucket name here
 
@@ -107,7 +107,10 @@
 
   # Use the uploader function to handle file uploads
   signedUrl_uploader(storage_client, credentials, bucket_name)
 
 if __name__ == "__main__":
     main()
 ```
+## Useful links
+
+[GitHub Repository](https://github.com/Meryam-A/signed-url-uploader)
```

### Comparing `st_signedurl_uploader-1.0/README.md` & `st_signedurl_uploader-1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Considering the schema below, the Signed Url Uploader abstracts away steps 2 and 3. Check this article for more details.
 <img width="822" alt="image" src="https://github.com/Meryam-A/signed-url-uploader/assets/166532696/615e35a9-ab78-45ea-916f-0a2dd3e45bb2">
 
 ## Installation
 
 You can install the latest release using:
 ```
-pip install st_signedUrl_uploader
+pip install st-signedUrl-uploader
 ```
 
 ## Usage 
 This component serves as an efficient uploader for applications that are deployed on App Engine or Cloud Run, specifically designed to handle large file uploads by utilizing Google Cloud Storage (GCS) and signed URLs. To facilitate ease of integration and testing, the component can be used in two ways: directly in cloud deployments or locally using a service account for development and testing purposes. Below, you will find detailed instructions for both scenarios, including sample code and a list of infrastructure prerequisites necessary to ensure smooth operation and integration of the uploader in your projects.
 
 ### Usage with App Engine or Cloud Run
 
@@ -30,15 +30,15 @@
 
 ### Implementation : 
 - **Service Account Permissions:** Ensure the App Engine or Cloud Run service account has the `roles/iam.serviceAccountTokenCreator` role for generating signed URLs.
     
 #### Sample Code :
 
 ```python
-from st_signedUrl_uploader import signedUrl_uploader
+from st-signedUrl-uploader import signedUrl_uploader
 from google import auth
 from google.cloud import storage
 
 def main():
   bucket_name = "your-bucket-name" # Specify your GCS bucket name here
 
   # Authenticate and create a storage client
@@ -68,15 +68,15 @@
 
 ### Implementation : 
 - Create a service account and give it the role `roles/iam.serviceAccountTokenCreator`
     
 #### Sample Code :
 
 ```python
-from st_signedUrl_uploader import signedUrl_uploader
+from st-signedUrl-uploader import signedUrl_uploader
 from google import auth
 from google.cloud import storage
 import os
 
 def main():
   bucket_name = "your-bucket-name"  # Specify your GCS bucket name here
 
@@ -88,7 +88,10 @@
 
   # Use the uploader function to handle file uploads
   signedUrl_uploader(storage_client, credentials, bucket_name)
 
 if __name__ == "__main__":
     main()
 ```
+## Useful links
+
+[GitHub Repository](https://github.com/Meryam-A/signed-url-uploader)
```

### Comparing `st_signedurl_uploader-1.0/setup.py` & `st_signedurl_uploader-1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
-    name="st_signedUrl_uploader",
-    version="1.0",
+    name="st-signedUrl-uploader",
+    version="1.1",
     author="Meryam Assermouh",
     author_email="",
     description="Streamlit component that allows you to upload files to Google Cloud Storage via signed url",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st_signedurl_uploader-1.0/st_signedUrl_uploader/__init__.py` & `st_signedurl_uploader-1.1/st-signedUrl-uploader/__init__.py`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.0/st_signedUrl_uploader/frontend/build/bootstrap.min.css` & `st_signedurl_uploader-1.1/st-signedUrl-uploader/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.0/st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js` & `st_signedurl_uploader-1.1/st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.0/st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js.LICENSE.txt` & `st_signedurl_uploader-1.1/st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.0/st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js.map` & `st_signedurl_uploader-1.1/st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js.map`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.0/st_signedUrl_uploader.egg-info/PKG-INFO` & `st_signedurl_uploader-1.1/st_signedUrl_uploader.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: st_signedUrl_uploader
-Version: 1.0
+Name: st-signedUrl-uploader
+Version: 1.1
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
-pip install st_signedUrl_uploader
+pip install st-signedUrl-uploader
 ```
 
 ## Usage 
 This component serves as an efficient uploader for applications that are deployed on App Engine or Cloud Run, specifically designed to handle large file uploads by utilizing Google Cloud Storage (GCS) and signed URLs. To facilitate ease of integration and testing, the component can be used in two ways: directly in cloud deployments or locally using a service account for development and testing purposes. Below, you will find detailed instructions for both scenarios, including sample code and a list of infrastructure prerequisites necessary to ensure smooth operation and integration of the uploader in your projects.
 
 ### Usage with App Engine or Cloud Run
 
@@ -49,15 +49,15 @@
 
 ### Implementation : 
 - **Service Account Permissions:** Ensure the App Engine or Cloud Run service account has the `roles/iam.serviceAccountTokenCreator` role for generating signed URLs.
     
 #### Sample Code :
 
 ```python
-from st_signedUrl_uploader import signedUrl_uploader
+from st-signedUrl-uploader import signedUrl_uploader
 from google import auth
 from google.cloud import storage
 
 def main():
   bucket_name = "your-bucket-name" # Specify your GCS bucket name here
 
   # Authenticate and create a storage client
@@ -87,15 +87,15 @@
 
 ### Implementation : 
 - Create a service account and give it the role `roles/iam.serviceAccountTokenCreator`
     
 #### Sample Code :
 
 ```python
-from st_signedUrl_uploader import signedUrl_uploader
+from st-signedUrl-uploader import signedUrl_uploader
 from google import auth
 from google.cloud import storage
 import os
 
 def main():
   bucket_name = "your-bucket-name"  # Specify your GCS bucket name here
 
@@ -107,7 +107,10 @@
 
   # Use the uploader function to handle file uploads
   signedUrl_uploader(storage_client, credentials, bucket_name)
 
 if __name__ == "__main__":
     main()
 ```
+## Useful links
+
+[GitHub Repository](https://github.com/Meryam-A/signed-url-uploader)
```

### Comparing `st_signedurl_uploader-1.0/st_signedUrl_uploader.egg-info/SOURCES.txt` & `st_signedurl_uploader-1.1/st_signedUrl_uploader.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
-st_signedUrl_uploader/__init__.py
+st-signedUrl-uploader/__init__.py
+st-signedUrl-uploader/frontend/build/asset-manifest.json
+st-signedUrl-uploader/frontend/build/bootstrap.min.css
+st-signedUrl-uploader/frontend/build/index.html
+st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js
+st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js.LICENSE.txt
+st-signedUrl-uploader/frontend/build/static/js/main.022a2283.js.map
 st_signedUrl_uploader.egg-info/PKG-INFO
 st_signedUrl_uploader.egg-info/SOURCES.txt
 st_signedUrl_uploader.egg-info/dependency_links.txt
 st_signedUrl_uploader.egg-info/requires.txt
-st_signedUrl_uploader.egg-info/top_level.txt
-st_signedUrl_uploader/frontend/build/asset-manifest.json
-st_signedUrl_uploader/frontend/build/bootstrap.min.css
-st_signedUrl_uploader/frontend/build/index.html
-st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js
-st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js.LICENSE.txt
-st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js.map
+st_signedUrl_uploader.egg-info/top_level.txt
```

