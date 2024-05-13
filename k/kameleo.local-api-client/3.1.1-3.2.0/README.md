# Comparing `tmp/kameleo.local_api_client-3.1.1.tar.gz` & `tmp/kameleo.local_api_client-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kameleo.local_api_client-3.1.1.tar", last modified: Wed Mar 20 14:58:16 2024, max compression
+gzip compressed data, was "kameleo.local_api_client-3.2.0.tar", last modified: Mon May 13 14:14:42 2024, max compression
```

## Comparing `kameleo.local_api_client-3.1.1.tar` & `kameleo.local_api_client-3.2.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-03-20 14:58:16.528781 kameleo.local_api_client-3.1.1/
--rw-rw-rw-   0        0        0     1100 2022-02-14 15:54:51.000000 kameleo.local_api_client-3.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0    11356 2024-03-20 14:58:16.528781 kameleo.local_api_client-3.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    10808 2024-03-12 16:06:13.000000 kameleo.local_api_client-3.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-20 14:58:16.479704 kameleo.local_api_client-3.1.1/kameleo/
--rw-rw-rw-   0        0        0       81 2024-03-20 14:58:15.000000 kameleo.local_api_client-3.1.1/kameleo/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-20 14:58:16.503549 kameleo.local_api_client-3.1.1/kameleo/local_api_client/
--rw-rw-rw-   0        0        0      783 2024-03-20 14:58:15.000000 kameleo.local_api_client-3.1.1/kameleo/local_api_client/__init__.py
--rw-rw-rw-   0        0        0     3012 2024-03-20 14:58:15.000000 kameleo.local_api_client-3.1.1/kameleo/local_api_client/_client.py
--rw-rw-rw-   0        0        0     1937 2024-03-20 14:58:15.000000 kameleo.local_api_client-3.1.1/kameleo/local_api_client/_configuration.py
-drwxrwxrwx   0        0        0        0 2024-03-20 14:58:16.508552 kameleo.local_api_client-3.1.1/kameleo/local_api_client/_operations/
--rw-rw-rw-   0        0        0      710 2024-03-20 14:58:15.000000 kameleo.local_api_client-3.1.1/kameleo/local_api_client/_operations/__init__.py
--rw-rw-rw-   0        0        0    83615 2024-03-20 14:58:15.000000 kameleo.local_api_client-3.1.1/kameleo/local_api_client/_operations/_operations.py
--rw-rw-rw-   0        0        0      677 2024-03-20 14:58:15.000000 kameleo.local_api_client-3.1.1/kameleo/local_api_client/_operations/_patch.py
--rw-rw-rw-   0        0        0      677 2024-03-20 14:58:15.000000 kameleo.local_api_client-3.1.1/kameleo/local_api_client/_patch.py
--rw-rw-rw-   0        0        0    78836 2024-03-20 14:58:15.000000 kameleo.local_api_client-3.1.1/kameleo/local_api_client/_serialization.py
--rw-rw-rw-   0        0        0     1399 2024-03-20 14:58:15.000000 kameleo.local_api_client-3.1.1/kameleo/local_api_client/_vendor.py
--rw-rw-rw-   0        0        0      383 2024-03-20 14:58:15.000000 kameleo.local_api_client-3.1.1/kameleo/local_api_client/_version.py
-drwxrwxrwx   0        0        0        0 2024-03-20 14:58:16.516512 kameleo.local_api_client-3.1.1/kameleo/local_api_client/aio/
--rw-rw-rw-   0        0        0      730 2024-03-20 14:58:15.000000 kameleo.local_api_client-3.1.1/kameleo/local_api_client/aio/__init__.py
--rw-rw-rw-   0        0        0     3117 2024-03-20 14:58:15.000000 kameleo.local_api_client-3.1.1/kameleo/local_api_client/aio/_client.py
--rw-rw-rw-   0        0        0     1948 2024-03-20 14:58:15.000000 kameleo.local_api_client-3.1.1/kameleo/local_api_client/aio/_configuration.py
-drwxrwxrwx   0        0        0        0 2024-03-20 14:58:16.517610 kameleo.local_api_client-3.1.1/kameleo/local_api_client/aio/_operations/
--rw-rw-rw-   0        0        0      710 2024-03-20 14:58:15.000000 kameleo.local_api_client-3.1.1/kameleo/local_api_client/aio/_operations/__init__.py
--rw-rw-rw-   0        0        0    71018 2024-03-20 14:58:15.000000 kameleo.local_api_client-3.1.1/kameleo/local_api_client/aio/_operations/_operations.py
--rw-rw-rw-   0        0        0      677 2024-03-20 14:58:15.000000 kameleo.local_api_client-3.1.1/kameleo/local_api_client/aio/_operations/_patch.py
--rw-rw-rw-   0        0        0      677 2024-03-20 14:58:15.000000 kameleo.local_api_client-3.1.1/kameleo/local_api_client/aio/_patch.py
--rw-rw-rw-   0        0        0      905 2024-03-20 14:58:15.000000 kameleo.local_api_client-3.1.1/kameleo/local_api_client/aio/_vendor.py
--rw-rw-rw-   0        0        0    14053 2024-03-12 13:15:38.000000 kameleo.local_api_client-3.1.1/kameleo/local_api_client/builder_for_create_profile.py
-drwxrwxrwx   0        0        0        0 2024-03-20 14:58:16.523209 kameleo.local_api_client-3.1.1/kameleo/local_api_client/models/
--rw-rw-rw-   0        0        0     4428 2024-03-20 14:58:15.000000 kameleo.local_api_client-3.1.1/kameleo/local_api_client/models/__init__.py
--rw-rw-rw-   0        0        0     7499 2024-03-20 14:58:15.000000 kameleo.local_api_client-3.1.1/kameleo/local_api_client/models/_enums.py
--rw-rw-rw-   0        0        0   116234 2024-03-20 14:58:15.000000 kameleo.local_api_client-3.1.1/kameleo/local_api_client/models/_models.py
--rw-rw-rw-   0        0        0      677 2024-03-20 14:58:15.000000 kameleo.local_api_client-3.1.1/kameleo/local_api_client/models/_patch.py
-drwxrwxrwx   0        0        0        0 2024-03-20 14:58:16.484481 kameleo.local_api_client-3.1.1/kameleo.local_api_client.egg-info/
--rw-rw-rw-   0        0        0    11356 2024-03-20 14:58:16.000000 kameleo.local_api_client-3.1.1/kameleo.local_api_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1297 2024-03-20 14:58:16.000000 kameleo.local_api_client-3.1.1/kameleo.local_api_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-20 14:58:16.000000 kameleo.local_api_client-3.1.1/kameleo.local_api_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-03-20 14:58:16.000000 kameleo.local_api_client-3.1.1/kameleo.local_api_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-20 14:58:16.000000 kameleo.local_api_client-3.1.1/kameleo.local_api_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-20 14:58:16.529787 kameleo.local_api_client-3.1.1/setup.cfg
--rw-rw-rw-   0        0        0      895 2023-10-26 13:51:31.000000 kameleo.local_api_client-3.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:14:42.972078 kameleo.local_api_client-3.2.0/
+-rw-rw-rw-   0        0        0     1100 2022-02-14 15:54:51.000000 kameleo.local_api_client-3.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0    11456 2024-05-13 14:14:42.971115 kameleo.local_api_client-3.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10908 2024-05-09 11:04:09.000000 kameleo.local_api_client-3.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 14:14:42.932080 kameleo.local_api_client-3.2.0/kameleo/
+-rw-rw-rw-   0        0        0       81 2024-05-13 14:14:41.000000 kameleo.local_api_client-3.2.0/kameleo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:14:42.950085 kameleo.local_api_client-3.2.0/kameleo/local_api_client/
+-rw-rw-rw-   0        0        0      783 2024-05-13 14:14:41.000000 kameleo.local_api_client-3.2.0/kameleo/local_api_client/__init__.py
+-rw-rw-rw-   0        0        0     3012 2024-05-13 14:14:41.000000 kameleo.local_api_client-3.2.0/kameleo/local_api_client/_client.py
+-rw-rw-rw-   0        0        0     1937 2024-05-13 14:14:41.000000 kameleo.local_api_client-3.2.0/kameleo/local_api_client/_configuration.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:14:42.954080 kameleo.local_api_client-3.2.0/kameleo/local_api_client/_operations/
+-rw-rw-rw-   0        0        0      710 2024-05-13 14:14:41.000000 kameleo.local_api_client-3.2.0/kameleo/local_api_client/_operations/__init__.py
+-rw-rw-rw-   0        0        0    83615 2024-05-13 14:14:41.000000 kameleo.local_api_client-3.2.0/kameleo/local_api_client/_operations/_operations.py
+-rw-rw-rw-   0        0        0      677 2024-05-13 14:14:41.000000 kameleo.local_api_client-3.2.0/kameleo/local_api_client/_operations/_patch.py
+-rw-rw-rw-   0        0        0      677 2024-05-13 14:14:41.000000 kameleo.local_api_client-3.2.0/kameleo/local_api_client/_patch.py
+-rw-rw-rw-   0        0        0    78836 2024-05-13 14:14:41.000000 kameleo.local_api_client-3.2.0/kameleo/local_api_client/_serialization.py
+-rw-rw-rw-   0        0        0     1399 2024-05-13 14:14:41.000000 kameleo.local_api_client-3.2.0/kameleo/local_api_client/_vendor.py
+-rw-rw-rw-   0        0        0      383 2024-05-13 14:14:41.000000 kameleo.local_api_client-3.2.0/kameleo/local_api_client/_version.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:14:42.961082 kameleo.local_api_client-3.2.0/kameleo/local_api_client/aio/
+-rw-rw-rw-   0        0        0      730 2024-05-13 14:14:41.000000 kameleo.local_api_client-3.2.0/kameleo/local_api_client/aio/__init__.py
+-rw-rw-rw-   0        0        0     3117 2024-05-13 14:14:41.000000 kameleo.local_api_client-3.2.0/kameleo/local_api_client/aio/_client.py
+-rw-rw-rw-   0        0        0     1948 2024-05-13 14:14:41.000000 kameleo.local_api_client-3.2.0/kameleo/local_api_client/aio/_configuration.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:14:42.965077 kameleo.local_api_client-3.2.0/kameleo/local_api_client/aio/_operations/
+-rw-rw-rw-   0        0        0      710 2024-05-13 14:14:41.000000 kameleo.local_api_client-3.2.0/kameleo/local_api_client/aio/_operations/__init__.py
+-rw-rw-rw-   0        0        0    71018 2024-05-13 14:14:41.000000 kameleo.local_api_client-3.2.0/kameleo/local_api_client/aio/_operations/_operations.py
+-rw-rw-rw-   0        0        0      677 2024-05-13 14:14:41.000000 kameleo.local_api_client-3.2.0/kameleo/local_api_client/aio/_operations/_patch.py
+-rw-rw-rw-   0        0        0      677 2024-05-13 14:14:41.000000 kameleo.local_api_client-3.2.0/kameleo/local_api_client/aio/_patch.py
+-rw-rw-rw-   0        0        0      905 2024-05-13 14:14:41.000000 kameleo.local_api_client-3.2.0/kameleo/local_api_client/aio/_vendor.py
+-rw-rw-rw-   0        0        0    13598 2024-05-09 11:04:09.000000 kameleo.local_api_client-3.2.0/kameleo/local_api_client/builder_for_create_profile.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:14:42.970114 kameleo.local_api_client-3.2.0/kameleo/local_api_client/models/
+-rw-rw-rw-   0        0        0     4316 2024-05-13 14:14:41.000000 kameleo.local_api_client-3.2.0/kameleo/local_api_client/models/__init__.py
+-rw-rw-rw-   0        0        0     7420 2024-05-13 14:14:41.000000 kameleo.local_api_client-3.2.0/kameleo/local_api_client/models/_enums.py
+-rw-rw-rw-   0        0        0   115867 2024-05-13 14:14:41.000000 kameleo.local_api_client-3.2.0/kameleo/local_api_client/models/_models.py
+-rw-rw-rw-   0        0        0      677 2024-05-13 14:14:41.000000 kameleo.local_api_client-3.2.0/kameleo/local_api_client/models/_patch.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:14:42.939078 kameleo.local_api_client-3.2.0/kameleo.local_api_client.egg-info/
+-rw-rw-rw-   0        0        0    11456 2024-05-13 14:14:42.000000 kameleo.local_api_client-3.2.0/kameleo.local_api_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1297 2024-05-13 14:14:42.000000 kameleo.local_api_client-3.2.0/kameleo.local_api_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 14:14:42.000000 kameleo.local_api_client-3.2.0/kameleo.local_api_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-13 14:14:42.000000 kameleo.local_api_client-3.2.0/kameleo.local_api_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-13 14:14:42.000000 kameleo.local_api_client-3.2.0/kameleo.local_api_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 14:14:42.972078 kameleo.local_api_client-3.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      895 2023-10-26 13:51:31.000000 kameleo.local_api_client-3.2.0/setup.py
```

### Comparing `kameleo.local_api_client-3.1.1/LICENSE.txt` & `kameleo.local_api_client-3.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-3.1.1/PKG-INFO` & `kameleo.local_api_client-3.2.0/kameleo.local_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: kameleo.local_api_client
-Version: 3.1.1
+Name: kameleo.local-api-client
+Version: 3.2.0
 Summary: This Python package provides convenient access to the Local API REST interface of the Kameleo Client.
 Home-page: https://github.com/kameleo-io/local-api-client-python
 Author: Kameleo Team
 Author-email: support@kameleo.io
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -59,14 +59,15 @@
     browser_product='chrome'
 )
 
 # Create a new profile with recommended settings
 # for browser fingerprinting protection
 create_profile_request = BuilderForCreateProfile \
     .for_base_profile(base_profiles[0].id) \
+    .set_name('example profile') \
     .set_recommended_defaults() \
     .build()
 profile = client.create_profile(body=create_profile_request)
 
 # Start the browser
 client.start_profile(profile.id)
 
@@ -199,14 +200,15 @@
 )
 
 # Create a new profile with recommended settings
 # Choose one of the Base Profiles
 # Set the launcher to 'chromium' so the mobile profile will be started in Chroma browser
 create_profile_request = BuilderForCreateProfile \
     .for_base_profile(base_profile_list[0].id) \
+    .set_name('automate mobile profiles on desktop example') \
     .set_recommended_defaults() \
     .set_launcher('chromium') \
     .build()
 profile = client.create_profile(body=create_profile_request)
 
 # Start the profile
 client.start_profile_with_options(profile.id, body={
```

### Comparing `kameleo.local_api_client-3.1.1/README.md` & `kameleo.local_api_client-3.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     browser_product='chrome'
 )
 
 # Create a new profile with recommended settings
 # for browser fingerprinting protection
 create_profile_request = BuilderForCreateProfile \
     .for_base_profile(base_profiles[0].id) \
+    .set_name('example profile') \
     .set_recommended_defaults() \
     .build()
 profile = client.create_profile(body=create_profile_request)
 
 # Start the browser
 client.start_profile(profile.id)
 
@@ -185,14 +186,15 @@
 )
 
 # Create a new profile with recommended settings
 # Choose one of the Base Profiles
 # Set the launcher to 'chromium' so the mobile profile will be started in Chroma browser
 create_profile_request = BuilderForCreateProfile \
     .for_base_profile(base_profile_list[0].id) \
+    .set_name('automate mobile profiles on desktop example') \
     .set_recommended_defaults() \
     .set_launcher('chromium') \
     .build()
 profile = client.create_profile(body=create_profile_request)
 
 # Start the profile
 client.start_profile_with_options(profile.id, body={
```

### Comparing `kameleo.local_api_client-3.1.1/kameleo/local_api_client/__init__.py` & `kameleo.local_api_client-3.2.0/kameleo/local_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-3.1.1/kameleo/local_api_client/_client.py` & `kameleo.local_api_client-3.2.0/kameleo/local_api_client/_client.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-3.1.1/kameleo/local_api_client/_configuration.py` & `kameleo.local_api_client-3.2.0/kameleo/local_api_client/_configuration.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-3.1.1/kameleo/local_api_client/_operations/__init__.py` & `kameleo.local_api_client-3.2.0/kameleo/local_api_client/_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-3.1.1/kameleo/local_api_client/_operations/_operations.py` & `kameleo.local_api_client-3.2.0/kameleo/local_api_client/_operations/_operations.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-3.1.1/kameleo/local_api_client/_operations/_patch.py` & `kameleo.local_api_client-3.2.0/kameleo/local_api_client/_operations/_patch.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-3.1.1/kameleo/local_api_client/_patch.py` & `kameleo.local_api_client-3.2.0/kameleo/local_api_client/_patch.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-3.1.1/kameleo/local_api_client/_serialization.py` & `kameleo.local_api_client-3.2.0/kameleo/local_api_client/_serialization.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-3.1.1/kameleo/local_api_client/_vendor.py` & `kameleo.local_api_client-3.2.0/kameleo/local_api_client/_vendor.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-3.1.1/kameleo/local_api_client/aio/__init__.py` & `kameleo.local_api_client-3.2.0/kameleo/local_api_client/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-3.1.1/kameleo/local_api_client/aio/_client.py` & `kameleo.local_api_client-3.2.0/kameleo/local_api_client/aio/_client.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-3.1.1/kameleo/local_api_client/aio/_configuration.py` & `kameleo.local_api_client-3.2.0/kameleo/local_api_client/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-3.1.1/kameleo/local_api_client/aio/_operations/__init__.py` & `kameleo.local_api_client-3.2.0/kameleo/local_api_client/aio/_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-3.1.1/kameleo/local_api_client/aio/_operations/_operations.py` & `kameleo.local_api_client-3.2.0/kameleo/local_api_client/aio/_operations/_operations.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-3.1.1/kameleo/local_api_client/aio/_operations/_patch.py` & `kameleo.local_api_client-3.2.0/kameleo/local_api_client/aio/_operations/_patch.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-3.1.1/kameleo/local_api_client/aio/_patch.py` & `kameleo.local_api_client-3.2.0/kameleo/local_api_client/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-3.1.1/kameleo/local_api_client/aio/_vendor.py` & `kameleo.local_api_client-3.2.0/kameleo/local_api_client/aio/_vendor.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-3.1.1/kameleo/local_api_client/builder_for_create_profile.py` & `kameleo.local_api_client-3.2.0/kameleo/local_api_client/builder_for_create_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,24 +112,21 @@
         :param options: When the WebRTC spoofing is set to manual, the private_ip and public_ip must be provided
         :type options: ~kameleo.local_api_client.models.WebRtcSpoofingOptions
         """
         self.profile_request['webRtc']['value'] = value
         self.profile_request['webRtc']['extra'] = options
         return self
 
-    def set_fonts(self, value, options):
+    def set_fonts(self, value):
         """Specifies how the fonts will be spoofed. Possible values:
-            'enabled': Enable fonts spoofing. A list can be provided to override the fonts coming from the base profile.
+            'enabled': Enable fonts spoofing.
             'disable': Disable fonts spoofing.
         :param string value: Fonts spoofing type. Possible values: 'enabled', 'disabled'
-        :param options: When the Font spoofing is set to enabled, a list can be provided to overrider the fonts coming from the base profile.
-        :type options: list[str]
         """
-        self.profile_request['fonts']['value'] = value
-        self.profile_request['fonts']['extra'] = options
+        self.profile_request['fonts'] = value
         return self
 
     def set_start_page(self, value):
         """This website will be opened in the browser when the profile launches.
         :param string value: The url of the start page
         """
         self.profile_request['startPage'] = value
@@ -217,23 +214,22 @@
         """
         self.profile_request['launcher'] = browser_launcher
         return self
 
     def set_recommended_defaults(self):
         """This sets all the profile options to the defaults recommended by Kameleo Team. Please consider providing Proxy settings to your profile.
         """
-        self.profile_request['name'] = ""
         self.profile_request['canvas'] = "intelligent"
         self.profile_request['webgl'] = "off"
         self.profile_request['webglMeta']['value'] = "automatic"
         self.profile_request['audio'] = "off"
         self.profile_request['timezone']['value'] = "automatic"
         self.profile_request['geolocation']['value'] = "automatic"
         self.profile_request['webRtc']['value'] = "automatic"
-        self.profile_request['fonts']['value'] = "enabled"
+        self.profile_request['fonts'] = "enabled"
         self.profile_request['screen']['value'] = "automatic"
         self.profile_request['hardwareConcurrency']['value'] = "automatic"
         self.profile_request['deviceMemory']['value'] = "automatic"
         self.profile_request['launcher'] = "automatic"
 
         return self
 
@@ -259,18 +255,15 @@
                 "value": "none",
                 "extra": None
             },
             "webRtc": {
                 "value": "off",
                 "extra": None
             },
-            "fonts": {
-                "value": "disabled",
-                "extra": None
-            },
+            "fonts": "disabled",
             "screen": {
                 "value": "off",
                 "extra": None
             },
             "hardwareConcurrency": {
                 "value": "off",
                 "extra": None
```

### Comparing `kameleo.local_api_client-3.1.1/kameleo/local_api_client/models/__init__.py` & `kameleo.local_api_client-3.2.0/kameleo/local_api_client/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from ._models import Browser
 from ._models import BrowserCookie
 from ._models import CookieRequest
 from ._models import CreateProfileRequest
 from ._models import Device
 from ._models import DeviceMemorySpoofingTypeDoubleNullableMultiLevelChoice
 from ._models import ExportProfileRequest
-from ._models import FontSpoofingTypeFontIListMultiLevelChoice
 from ._models import GeolocationSpoofingOptions
 from ._models import GeolocationSpoofingTypeGeolocationSpoofingOptionsMultiLevelChoice
 from ._models import HardwareConcurrencySpoofingTypeInt32NullableMultiLevelChoice
 from ._models import ImportProfileRequest
 from ._models import Os
 from ._models import Preference
 from ._models import ProblemResponse
@@ -66,15 +65,14 @@
     "Browser",
     "BrowserCookie",
     "CookieRequest",
     "CreateProfileRequest",
     "Device",
     "DeviceMemorySpoofingTypeDoubleNullableMultiLevelChoice",
     "ExportProfileRequest",
-    "FontSpoofingTypeFontIListMultiLevelChoice",
     "GeolocationSpoofingOptions",
     "GeolocationSpoofingTypeGeolocationSpoofingOptionsMultiLevelChoice",
     "HardwareConcurrencySpoofingTypeInt32NullableMultiLevelChoice",
     "ImportProfileRequest",
     "Os",
     "Preference",
     "ProblemResponse",
```

### Comparing `kameleo.local_api_client-3.1.1/kameleo/local_api_client/models/_enums.py` & `kameleo.local_api_client-3.2.0/kameleo/local_api_client/models/_enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,16 +45,15 @@
     AUTOMATIC = "automatic"
     MANUAL = "manual"
     OFF = "off"
 
 
 class FontSpoofingType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Specifies how the fonts will be spoofed. Possible values:
-    'enabled': Enable fonts spoofing. A list can be provided to override the fonts coming from the
-    base profile.
+    'enabled': Enable fonts spoofing.
     'disable': Disable fonts spoofing.
     """
 
     ENABLED = "enabled"
     DISABLED = "disabled"
```

### Comparing `kameleo.local_api_client-3.1.1/kameleo/local_api_client/models/_models.py` & `kameleo.local_api_client-3.2.0/kameleo/local_api_client/models/_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,58 +30,58 @@
     :vartype device: ~kameleo.local_api_client.models.Device
     :ivar os: Required.
     :vartype os: ~kameleo.local_api_client.models.Os
     :ivar browser: Required.
     :vartype browser: ~kameleo.local_api_client.models.Browser
     :ivar language: Language of the base profile. Using ISO 639-1 language codes. Required.
     :vartype language: str
+    :ivar webgl_meta: Required.
+    :vartype webgl_meta: ~kameleo.local_api_client.models.WebglMeta
     :ivar resolution: The screen size of the device in pixels. Required.
     :vartype resolution: str
     :ivar fonts: A list of font types included in the profile. Required.
     :vartype fonts: list[str]
-    :ivar webgl_meta: Required.
-    :vartype webgl_meta: ~kameleo.local_api_client.models.WebglMeta
     """
 
     _validation = {
         "version": {"required": True},
         "id": {"required": True},
         "device": {"required": True},
         "os": {"required": True},
         "browser": {"required": True},
         "language": {"required": True},
+        "webgl_meta": {"required": True},
         "resolution": {"required": True},
         "fonts": {"required": True},
-        "webgl_meta": {"required": True},
     }
 
     _attribute_map = {
         "version": {"key": "version", "type": "str"},
         "id": {"key": "id", "type": "str"},
         "device": {"key": "device", "type": "Device"},
         "os": {"key": "os", "type": "Os"},
         "browser": {"key": "browser", "type": "Browser"},
         "language": {"key": "language", "type": "str"},
+        "webgl_meta": {"key": "webglMeta", "type": "WebglMeta"},
         "resolution": {"key": "resolution", "type": "str"},
         "fonts": {"key": "fonts", "type": "[str]"},
-        "webgl_meta": {"key": "webglMeta", "type": "WebglMeta"},
     }
 
     def __init__(
         self,
         *,
         version: str,
         id: str,  # pylint: disable=redefined-builtin
         device: "_models.Device",
         os: "_models.Os",
         browser: "_models.Browser",
         language: str,
+        webgl_meta: "_models.WebglMeta",
         resolution: str,
         fonts: List[str],
-        webgl_meta: "_models.WebglMeta",
         **kwargs: Any
     ) -> None:
         """
         :keyword version: The version of the base profile. As time passes new base profile versions
          will be introduced. It is recommended to use the latest one. Required.
         :paramtype version: str
         :keyword id: The unique identifier of the base profile. You can use this as a reference to
@@ -91,31 +91,31 @@
         :paramtype device: ~kameleo.local_api_client.models.Device
         :keyword os: Required.
         :paramtype os: ~kameleo.local_api_client.models.Os
         :keyword browser: Required.
         :paramtype browser: ~kameleo.local_api_client.models.Browser
         :keyword language: Language of the base profile. Using ISO 639-1 language codes. Required.
         :paramtype language: str
+        :keyword webgl_meta: Required.
+        :paramtype webgl_meta: ~kameleo.local_api_client.models.WebglMeta
         :keyword resolution: The screen size of the device in pixels. Required.
         :paramtype resolution: str
         :keyword fonts: A list of font types included in the profile. Required.
         :paramtype fonts: list[str]
-        :keyword webgl_meta: Required.
-        :paramtype webgl_meta: ~kameleo.local_api_client.models.WebglMeta
         """
         super().__init__(**kwargs)
         self.version = version
         self.id = id
         self.device = device
         self.os = os
         self.browser = browser
         self.language = language
+        self.webgl_meta = webgl_meta
         self.resolution = resolution
         self.fonts = fonts
-        self.webgl_meta = webgl_meta
 
 
 class BaseProfilePreview(_serialization.Model):
     """A preview object of a searched base profile. This contains some information about the base
     profile that will help you choose the right one.
 
     All required parameters must be populated in order to send to Azure.
@@ -127,61 +127,69 @@
     :vartype device: ~kameleo.local_api_client.models.Device
     :ivar os: Required.
     :vartype os: ~kameleo.local_api_client.models.Os
     :ivar browser: Required.
     :vartype browser: ~kameleo.local_api_client.models.Browser
     :ivar language: Language of the base profile. Using ISO 639-1 language codes. Required.
     :vartype language: str
+    :ivar webgl_meta: Required.
+    :vartype webgl_meta: ~kameleo.local_api_client.models.WebglMeta
     """
 
     _validation = {
         "id": {"required": True},
         "device": {"required": True},
         "os": {"required": True},
         "browser": {"required": True},
         "language": {"required": True},
+        "webgl_meta": {"required": True},
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "device": {"key": "device", "type": "Device"},
         "os": {"key": "os", "type": "Os"},
         "browser": {"key": "browser", "type": "Browser"},
         "language": {"key": "language", "type": "str"},
+        "webgl_meta": {"key": "webglMeta", "type": "WebglMeta"},
     }
 
     def __init__(
         self,
         *,
         id: str,  # pylint: disable=redefined-builtin
         device: "_models.Device",
         os: "_models.Os",
         browser: "_models.Browser",
         language: str,
+        webgl_meta: "_models.WebglMeta",
         **kwargs: Any
     ) -> None:
         """
         :keyword id: The unique identifier of the base profile. You can use this as a reference to
          create a new profile from this base profile. Required.
         :paramtype id: str
         :keyword device: Required.
         :paramtype device: ~kameleo.local_api_client.models.Device
         :keyword os: Required.
         :paramtype os: ~kameleo.local_api_client.models.Os
         :keyword browser: Required.
         :paramtype browser: ~kameleo.local_api_client.models.Browser
         :keyword language: Language of the base profile. Using ISO 639-1 language codes. Required.
         :paramtype language: str
+        :keyword webgl_meta: Required.
+        :paramtype webgl_meta: ~kameleo.local_api_client.models.WebglMeta
         """
         super().__init__(**kwargs)
         self.id = id
         self.device = device
         self.os = os
         self.browser = browser
         self.language = language
+        self.webgl_meta = webgl_meta
 
 
 class BaseProfileSearchParameters(_serialization.Model):
     """Provides possible values for base profile filtering. For example it tells what os languages are
     available.
 
     All required parameters must be populated in order to send to Azure.
@@ -566,16 +574,16 @@
     """CreateProfileRequest.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar base_profile_id: The unique identifier of the base profile. This references the base
      profile which should be used to build the new profile. Required.
     :vartype base_profile_id: str
-    :ivar name: Sets a human readable name for the profile. The value obtained by file name for
-     existing profiles. For new profiles the value is generated by random.
+    :ivar name: Sets a human-readable name for the profile, which is modifiable at any time.
+     Required.
     :vartype name: str
     :ivar tags: Use tags to categorize profiles by labeling them accordingly.
     :vartype tags: list[str]
     :ivar canvas: Specifies how the canvas will be spoofed. Possible values:
      'intelligent': Use intelligent canvas spoofing. This will result non-unique canvas
      fingerprints.
      'noise': Add some noise to canvas generation.
@@ -605,16 +613,18 @@
     :vartype geolocation:
      ~kameleo.local_api_client.models.GeolocationSpoofingTypeGeolocationSpoofingOptionsMultiLevelChoice
     :ivar proxy: Required.
     :vartype proxy: ~kameleo.local_api_client.models.ProxyConnectionTypeServerMultiLevelChoice
     :ivar web_rtc: Required.
     :vartype web_rtc:
      ~kameleo.local_api_client.models.WebRtcSpoofingTypeWebRtcSpoofingOptionsMultiLevelChoice
-    :ivar fonts: Required.
-    :vartype fonts: ~kameleo.local_api_client.models.FontSpoofingTypeFontIListMultiLevelChoice
+    :ivar fonts: Specifies how the fonts will be spoofed. Possible values:
+     'enabled': Enable fonts spoofing.
+     'disable': Disable fonts spoofing. Required. Known values are: "enabled" and "disabled".
+    :vartype fonts: str or ~kameleo.local_api_client.models.FontSpoofingType
     :ivar screen: Required.
     :vartype screen: ~kameleo.local_api_client.models.ScreenSpoofingTypeScreenSizeMultiLevelChoice
     :ivar hardware_concurrency:
     :vartype hardware_concurrency:
      ~kameleo.local_api_client.models.HardwareConcurrencySpoofingTypeInt32NullableMultiLevelChoice
     :ivar device_memory:
     :vartype device_memory:
@@ -639,14 +649,15 @@
      started. This can be modified only before the first start. Possible values for Desktop
      profiles: 'automatic'. Possible values for Mobile profiles: 'chromium', 'external'.
     :vartype launcher: str
     """
 
     _validation = {
         "base_profile_id": {"required": True, "min_length": 1},
+        "name": {"required": True, "min_length": 1},
         "canvas": {"required": True},
         "webgl": {"required": True},
         "webgl_meta": {"required": True},
         "audio": {"required": True},
         "timezone": {"required": True},
         "geolocation": {"required": True},
         "proxy": {"required": True},
@@ -667,15 +678,15 @@
         "timezone": {"key": "timezone", "type": "TimezoneSpoofingTypeTimezoneMultiLevelChoice"},
         "geolocation": {
             "key": "geolocation",
             "type": "GeolocationSpoofingTypeGeolocationSpoofingOptionsMultiLevelChoice",
         },
         "proxy": {"key": "proxy", "type": "ProxyConnectionTypeServerMultiLevelChoice"},
         "web_rtc": {"key": "webRtc", "type": "WebRtcSpoofingTypeWebRtcSpoofingOptionsMultiLevelChoice"},
-        "fonts": {"key": "fonts", "type": "FontSpoofingTypeFontIListMultiLevelChoice"},
+        "fonts": {"key": "fonts", "type": "str"},
         "screen": {"key": "screen", "type": "ScreenSpoofingTypeScreenSizeMultiLevelChoice"},
         "hardware_concurrency": {
             "key": "hardwareConcurrency",
             "type": "HardwareConcurrencySpoofingTypeInt32NullableMultiLevelChoice",
         },
         "device_memory": {"key": "deviceMemory", "type": "DeviceMemorySpoofingTypeDoubleNullableMultiLevelChoice"},
         "start_page": {"key": "startPage", "type": "str"},
@@ -686,42 +697,42 @@
         "launcher": {"key": "launcher", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         base_profile_id: str,
+        name: str,
         canvas: Union[str, "_models.CanvasSpoofingType"],
         webgl: Union[str, "_models.WebglSpoofingType"],
         webgl_meta: "_models.WebglMetaSpoofingTypeWebglMetaSpoofingOptionsMultiLevelChoice",
         audio: Union[str, "_models.AudioSpoofingType"],
         timezone: "_models.TimezoneSpoofingTypeTimezoneMultiLevelChoice",
         geolocation: "_models.GeolocationSpoofingTypeGeolocationSpoofingOptionsMultiLevelChoice",
         proxy: "_models.ProxyConnectionTypeServerMultiLevelChoice",
         web_rtc: "_models.WebRtcSpoofingTypeWebRtcSpoofingOptionsMultiLevelChoice",
-        fonts: "_models.FontSpoofingTypeFontIListMultiLevelChoice",
+        fonts: Union[str, "_models.FontSpoofingType"],
         screen: "_models.ScreenSpoofingTypeScreenSizeMultiLevelChoice",
         password_manager: Union[str, "_models.PasswordManagerType"],
-        name: Optional[str] = None,
         tags: Optional[List[str]] = None,
         hardware_concurrency: Optional["_models.HardwareConcurrencySpoofingTypeInt32NullableMultiLevelChoice"] = None,
         device_memory: Optional["_models.DeviceMemorySpoofingTypeDoubleNullableMultiLevelChoice"] = None,
         start_page: Optional[str] = None,
         extensions: Optional[List[str]] = None,
         notes: Optional[str] = None,
         storage: Optional[Union[str, "_models.ProfileStorageLocation"]] = None,
         launcher: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword base_profile_id: The unique identifier of the base profile. This references the base
          profile which should be used to build the new profile. Required.
         :paramtype base_profile_id: str
-        :keyword name: Sets a human readable name for the profile. The value obtained by file name for
-         existing profiles. For new profiles the value is generated by random.
+        :keyword name: Sets a human-readable name for the profile, which is modifiable at any time.
+         Required.
         :paramtype name: str
         :keyword tags: Use tags to categorize profiles by labeling them accordingly.
         :paramtype tags: list[str]
         :keyword canvas: Specifies how the canvas will be spoofed. Possible values:
          'intelligent': Use intelligent canvas spoofing. This will result non-unique canvas
          fingerprints.
          'noise': Add some noise to canvas generation.
@@ -751,16 +762,18 @@
         :paramtype geolocation:
          ~kameleo.local_api_client.models.GeolocationSpoofingTypeGeolocationSpoofingOptionsMultiLevelChoice
         :keyword proxy: Required.
         :paramtype proxy: ~kameleo.local_api_client.models.ProxyConnectionTypeServerMultiLevelChoice
         :keyword web_rtc: Required.
         :paramtype web_rtc:
          ~kameleo.local_api_client.models.WebRtcSpoofingTypeWebRtcSpoofingOptionsMultiLevelChoice
-        :keyword fonts: Required.
-        :paramtype fonts: ~kameleo.local_api_client.models.FontSpoofingTypeFontIListMultiLevelChoice
+        :keyword fonts: Specifies how the fonts will be spoofed. Possible values:
+         'enabled': Enable fonts spoofing.
+         'disable': Disable fonts spoofing. Required. Known values are: "enabled" and "disabled".
+        :paramtype fonts: str or ~kameleo.local_api_client.models.FontSpoofingType
         :keyword screen: Required.
         :paramtype screen:
          ~kameleo.local_api_client.models.ScreenSpoofingTypeScreenSizeMultiLevelChoice
         :keyword hardware_concurrency:
         :paramtype hardware_concurrency:
          ~kameleo.local_api_client.models.HardwareConcurrencySpoofingTypeInt32NullableMultiLevelChoice
         :keyword device_memory:
@@ -907,54 +920,14 @@
         :keyword path: Specifies the file path for exporting the profile. Required.
         :paramtype path: str
         """
         super().__init__(**kwargs)
         self.path = path
 
 
-class FontSpoofingTypeFontIListMultiLevelChoice(_serialization.Model):
-    """FontSpoofingTypeFontIListMultiLevelChoice.
-
-    All required parameters must be populated in order to send to Azure.
-
-    :ivar value: Specifies how the fonts will be spoofed. Possible values:
-     'enabled': Enable fonts spoofing. A list can be provided to override the fonts coming from the
-     base profile.
-     'disable': Disable fonts spoofing. Required. Known values are: "enabled" and "disabled".
-    :vartype value: str or ~kameleo.local_api_client.models.FontSpoofingType
-    :ivar extra:
-    :vartype extra: list[str]
-    """
-
-    _validation = {
-        "value": {"required": True},
-    }
-
-    _attribute_map = {
-        "value": {"key": "value", "type": "str"},
-        "extra": {"key": "extra", "type": "[str]"},
-    }
-
-    def __init__(
-        self, *, value: Union[str, "_models.FontSpoofingType"], extra: Optional[List[str]] = None, **kwargs: Any
-    ) -> None:
-        """
-        :keyword value: Specifies how the fonts will be spoofed. Possible values:
-         'enabled': Enable fonts spoofing. A list can be provided to override the fonts coming from the
-         base profile.
-         'disable': Disable fonts spoofing. Required. Known values are: "enabled" and "disabled".
-        :paramtype value: str or ~kameleo.local_api_client.models.FontSpoofingType
-        :keyword extra:
-        :paramtype extra: list[str]
-        """
-        super().__init__(**kwargs)
-        self.value = value
-        self.extra = extra
-
-
 class GeolocationSpoofingOptions(_serialization.Model):
     """When the Geolocation spoofing is set to manual these extra settings will be used as well.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar latitude: From -90 to 90. Required.
     :vartype latitude: float
@@ -1386,16 +1359,18 @@
     :vartype geolocation:
      ~kameleo.local_api_client.models.GeolocationSpoofingTypeGeolocationSpoofingOptionsMultiLevelChoice
     :ivar proxy: Required.
     :vartype proxy: ~kameleo.local_api_client.models.ProxyConnectionTypeServerMultiLevelChoice
     :ivar web_rtc: Required.
     :vartype web_rtc:
      ~kameleo.local_api_client.models.WebRtcSpoofingTypeWebRtcSpoofingOptionsMultiLevelChoice
-    :ivar fonts: Required.
-    :vartype fonts: ~kameleo.local_api_client.models.FontSpoofingTypeFontIListMultiLevelChoice
+    :ivar fonts: Specifies how the fonts will be spoofed. Possible values:
+     'enabled': Enable fonts spoofing.
+     'disable': Disable fonts spoofing. Required. Known values are: "enabled" and "disabled".
+    :vartype fonts: str or ~kameleo.local_api_client.models.FontSpoofingType
     :ivar screen: Required.
     :vartype screen: ~kameleo.local_api_client.models.ScreenSpoofingTypeScreenSizeMultiLevelChoice
     :ivar hardware_concurrency: Required.
     :vartype hardware_concurrency:
      ~kameleo.local_api_client.models.HardwareConcurrencySpoofingTypeInt32NullableMultiLevelChoice
     :ivar device_memory: Required.
     :vartype device_memory:
@@ -1464,15 +1439,15 @@
         "timezone": {"key": "timezone", "type": "TimezoneSpoofingTypeTimezoneMultiLevelChoice"},
         "geolocation": {
             "key": "geolocation",
             "type": "GeolocationSpoofingTypeGeolocationSpoofingOptionsMultiLevelChoice",
         },
         "proxy": {"key": "proxy", "type": "ProxyConnectionTypeServerMultiLevelChoice"},
         "web_rtc": {"key": "webRtc", "type": "WebRtcSpoofingTypeWebRtcSpoofingOptionsMultiLevelChoice"},
-        "fonts": {"key": "fonts", "type": "FontSpoofingTypeFontIListMultiLevelChoice"},
+        "fonts": {"key": "fonts", "type": "str"},
         "screen": {"key": "screen", "type": "ScreenSpoofingTypeScreenSizeMultiLevelChoice"},
         "hardware_concurrency": {
             "key": "hardwareConcurrency",
             "type": "HardwareConcurrencySpoofingTypeInt32NullableMultiLevelChoice",
         },
         "device_memory": {"key": "deviceMemory", "type": "DeviceMemorySpoofingTypeDoubleNullableMultiLevelChoice"},
         "start_page": {"key": "startPage", "type": "str"},
@@ -1496,15 +1471,15 @@
         webgl: Union[str, "_models.WebglSpoofingType"],
         webgl_meta: "_models.WebglMetaSpoofingTypeWebglMetaSpoofingOptionsMultiLevelChoice",
         audio: Union[str, "_models.AudioSpoofingType"],
         timezone: "_models.TimezoneSpoofingTypeTimezoneMultiLevelChoice",
         geolocation: "_models.GeolocationSpoofingTypeGeolocationSpoofingOptionsMultiLevelChoice",
         proxy: "_models.ProxyConnectionTypeServerMultiLevelChoice",
         web_rtc: "_models.WebRtcSpoofingTypeWebRtcSpoofingOptionsMultiLevelChoice",
-        fonts: "_models.FontSpoofingTypeFontIListMultiLevelChoice",
+        fonts: Union[str, "_models.FontSpoofingType"],
         screen: "_models.ScreenSpoofingTypeScreenSizeMultiLevelChoice",
         hardware_concurrency: "_models.HardwareConcurrencySpoofingTypeInt32NullableMultiLevelChoice",
         device_memory: "_models.DeviceMemorySpoofingTypeDoubleNullableMultiLevelChoice",
         start_page: str,
         password_manager: Union[str, "_models.PasswordManagerType"],
         extensions: List[str],
         notes: str,
@@ -1556,16 +1531,18 @@
         :paramtype geolocation:
          ~kameleo.local_api_client.models.GeolocationSpoofingTypeGeolocationSpoofingOptionsMultiLevelChoice
         :keyword proxy: Required.
         :paramtype proxy: ~kameleo.local_api_client.models.ProxyConnectionTypeServerMultiLevelChoice
         :keyword web_rtc: Required.
         :paramtype web_rtc:
          ~kameleo.local_api_client.models.WebRtcSpoofingTypeWebRtcSpoofingOptionsMultiLevelChoice
-        :keyword fonts: Required.
-        :paramtype fonts: ~kameleo.local_api_client.models.FontSpoofingTypeFontIListMultiLevelChoice
+        :keyword fonts: Specifies how the fonts will be spoofed. Possible values:
+         'enabled': Enable fonts spoofing.
+         'disable': Disable fonts spoofing. Required. Known values are: "enabled" and "disabled".
+        :paramtype fonts: str or ~kameleo.local_api_client.models.FontSpoofingType
         :keyword screen: Required.
         :paramtype screen:
          ~kameleo.local_api_client.models.ScreenSpoofingTypeScreenSizeMultiLevelChoice
         :keyword hardware_concurrency: Required.
         :paramtype hardware_concurrency:
          ~kameleo.local_api_client.models.HardwareConcurrencySpoofingTypeInt32NullableMultiLevelChoice
         :keyword device_memory: Required.
@@ -1969,16 +1946,18 @@
     :vartype geolocation:
      ~kameleo.local_api_client.models.GeolocationSpoofingTypeGeolocationSpoofingOptionsMultiLevelChoice
     :ivar proxy: Required.
     :vartype proxy: ~kameleo.local_api_client.models.ProxyConnectionTypeServerMultiLevelChoice
     :ivar web_rtc: Required.
     :vartype web_rtc:
      ~kameleo.local_api_client.models.WebRtcSpoofingTypeWebRtcSpoofingOptionsMultiLevelChoice
-    :ivar fonts: Required.
-    :vartype fonts: ~kameleo.local_api_client.models.FontSpoofingTypeFontIListMultiLevelChoice
+    :ivar fonts: Specifies how the fonts will be spoofed. Possible values:
+     'enabled': Enable fonts spoofing.
+     'disable': Disable fonts spoofing. Required. Known values are: "enabled" and "disabled".
+    :vartype fonts: str or ~kameleo.local_api_client.models.FontSpoofingType
     :ivar screen: Required.
     :vartype screen: ~kameleo.local_api_client.models.ScreenSpoofingTypeScreenSizeMultiLevelChoice
     :ivar hardware_concurrency: Required.
     :vartype hardware_concurrency:
      ~kameleo.local_api_client.models.HardwareConcurrencySpoofingTypeInt32NullableMultiLevelChoice
     :ivar device_memory:
     :vartype device_memory:
@@ -2035,15 +2014,15 @@
         "timezone": {"key": "timezone", "type": "TimezoneSpoofingTypeTimezoneMultiLevelChoice"},
         "geolocation": {
             "key": "geolocation",
             "type": "GeolocationSpoofingTypeGeolocationSpoofingOptionsMultiLevelChoice",
         },
         "proxy": {"key": "proxy", "type": "ProxyConnectionTypeServerMultiLevelChoice"},
         "web_rtc": {"key": "webRtc", "type": "WebRtcSpoofingTypeWebRtcSpoofingOptionsMultiLevelChoice"},
-        "fonts": {"key": "fonts", "type": "FontSpoofingTypeFontIListMultiLevelChoice"},
+        "fonts": {"key": "fonts", "type": "str"},
         "screen": {"key": "screen", "type": "ScreenSpoofingTypeScreenSizeMultiLevelChoice"},
         "hardware_concurrency": {
             "key": "hardwareConcurrency",
             "type": "HardwareConcurrencySpoofingTypeInt32NullableMultiLevelChoice",
         },
         "device_memory": {"key": "deviceMemory", "type": "DeviceMemorySpoofingTypeDoubleNullableMultiLevelChoice"},
         "start_page": {"key": "startPage", "type": "str"},
@@ -2063,15 +2042,15 @@
         webgl: Union[str, "_models.WebglSpoofingType"],
         webgl_meta: "_models.WebglMetaSpoofingTypeWebglMetaSpoofingOptionsMultiLevelChoice",
         audio: Union[str, "_models.AudioSpoofingType"],
         timezone: "_models.TimezoneSpoofingTypeTimezoneMultiLevelChoice",
         geolocation: "_models.GeolocationSpoofingTypeGeolocationSpoofingOptionsMultiLevelChoice",
         proxy: "_models.ProxyConnectionTypeServerMultiLevelChoice",
         web_rtc: "_models.WebRtcSpoofingTypeWebRtcSpoofingOptionsMultiLevelChoice",
-        fonts: "_models.FontSpoofingTypeFontIListMultiLevelChoice",
+        fonts: Union[str, "_models.FontSpoofingType"],
         screen: "_models.ScreenSpoofingTypeScreenSizeMultiLevelChoice",
         hardware_concurrency: "_models.HardwareConcurrencySpoofingTypeInt32NullableMultiLevelChoice",
         password_manager: Union[str, "_models.PasswordManagerType"],
         name: str,
         device_memory: Optional["_models.DeviceMemorySpoofingTypeDoubleNullableMultiLevelChoice"] = None,
         start_page: Optional[str] = None,
         extensions: Optional[List[str]] = None,
@@ -2112,16 +2091,18 @@
         :paramtype geolocation:
          ~kameleo.local_api_client.models.GeolocationSpoofingTypeGeolocationSpoofingOptionsMultiLevelChoice
         :keyword proxy: Required.
         :paramtype proxy: ~kameleo.local_api_client.models.ProxyConnectionTypeServerMultiLevelChoice
         :keyword web_rtc: Required.
         :paramtype web_rtc:
          ~kameleo.local_api_client.models.WebRtcSpoofingTypeWebRtcSpoofingOptionsMultiLevelChoice
-        :keyword fonts: Required.
-        :paramtype fonts: ~kameleo.local_api_client.models.FontSpoofingTypeFontIListMultiLevelChoice
+        :keyword fonts: Specifies how the fonts will be spoofed. Possible values:
+         'enabled': Enable fonts spoofing.
+         'disable': Disable fonts spoofing. Required. Known values are: "enabled" and "disabled".
+        :paramtype fonts: str or ~kameleo.local_api_client.models.FontSpoofingType
         :keyword screen: Required.
         :paramtype screen:
          ~kameleo.local_api_client.models.ScreenSpoofingTypeScreenSizeMultiLevelChoice
         :keyword hardware_concurrency: Required.
         :paramtype hardware_concurrency:
          ~kameleo.local_api_client.models.HardwareConcurrencySpoofingTypeInt32NullableMultiLevelChoice
         :keyword device_memory:
```

### Comparing `kameleo.local_api_client-3.1.1/kameleo/local_api_client/models/_patch.py` & `kameleo.local_api_client-3.2.0/kameleo/local_api_client/models/_patch.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-3.1.1/kameleo.local_api_client.egg-info/PKG-INFO` & `kameleo.local_api_client-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: kameleo.local-api-client
-Version: 3.1.1
+Name: kameleo.local_api_client
+Version: 3.2.0
 Summary: This Python package provides convenient access to the Local API REST interface of the Kameleo Client.
 Home-page: https://github.com/kameleo-io/local-api-client-python
 Author: Kameleo Team
 Author-email: support@kameleo.io
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -59,14 +59,15 @@
     browser_product='chrome'
 )
 
 # Create a new profile with recommended settings
 # for browser fingerprinting protection
 create_profile_request = BuilderForCreateProfile \
     .for_base_profile(base_profiles[0].id) \
+    .set_name('example profile') \
     .set_recommended_defaults() \
     .build()
 profile = client.create_profile(body=create_profile_request)
 
 # Start the browser
 client.start_profile(profile.id)
 
@@ -199,14 +200,15 @@
 )
 
 # Create a new profile with recommended settings
 # Choose one of the Base Profiles
 # Set the launcher to 'chromium' so the mobile profile will be started in Chroma browser
 create_profile_request = BuilderForCreateProfile \
     .for_base_profile(base_profile_list[0].id) \
+    .set_name('automate mobile profiles on desktop example') \
     .set_recommended_defaults() \
     .set_launcher('chromium') \
     .build()
 profile = client.create_profile(body=create_profile_request)
 
 # Start the profile
 client.start_profile_with_options(profile.id, body={
```

### Comparing `kameleo.local_api_client-3.1.1/kameleo.local_api_client.egg-info/SOURCES.txt` & `kameleo.local_api_client-3.2.0/kameleo.local_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-3.1.1/setup.py` & `kameleo.local_api_client-3.2.0/setup.py`

 * *Files identical despite different names*

