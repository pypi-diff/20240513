# Comparing `tmp/metals_api_zylalabs-0.2.tar.gz` & `tmp/metals_api_zylalabs-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metals_api_zylalabs-0.2.tar", last modified: Mon May 13 19:29:39 2024, max compression
+gzip compressed data, was "metals_api_zylalabs-0.3.tar", last modified: Mon May 13 19:52:24 2024, max compression
```

## Comparing `metals_api_zylalabs-0.2.tar` & `metals_api_zylalabs-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 19:29:39.628836 metals_api_zylalabs-0.2/
--rw-rw-rw-   0        0        0     1065 2024-05-13 19:29:39.627836 metals_api_zylalabs-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      956 2024-05-13 19:28:57.000000 metals_api_zylalabs-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 19:29:39.606860 metals_api_zylalabs-0.2/metals_api_zylalabs/
--rw-rw-rw-   0        0        0       27 2024-05-13 19:02:06.000000 metals_api_zylalabs-0.2/metals_api_zylalabs/__init__.py
--rw-rw-rw-   0        0        0      615 2024-05-13 18:59:52.000000 metals_api_zylalabs-0.2/metals_api_zylalabs/main.py
-drwxrwxrwx   0        0        0        0 2024-05-13 19:29:39.626840 metals_api_zylalabs-0.2/metals_api_zylalabs.egg-info/
--rw-rw-rw-   0        0        0     1065 2024-05-13 19:29:39.000000 metals_api_zylalabs-0.2/metals_api_zylalabs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-05-13 19:29:39.000000 metals_api_zylalabs-0.2/metals_api_zylalabs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 19:29:39.000000 metals_api_zylalabs-0.2/metals_api_zylalabs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-05-13 19:29:39.000000 metals_api_zylalabs-0.2/metals_api_zylalabs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 19:29:39.629898 metals_api_zylalabs-0.2/setup.cfg
--rw-rw-rw-   0        0        0      333 2024-05-13 19:29:19.000000 metals_api_zylalabs-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:52:24.013785 metals_api_zylalabs-0.3/
+-rw-rw-rw-   0        0        0     1072 2024-05-13 19:52:24.012772 metals_api_zylalabs-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      963 2024-05-13 19:51:07.000000 metals_api_zylalabs-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 19:52:23.983941 metals_api_zylalabs-0.3/metals_api_zylalabs/
+-rw-rw-rw-   0        0        0       88 2024-05-13 19:50:11.000000 metals_api_zylalabs-0.3/metals_api_zylalabs/__init__.py
+-rw-rw-rw-   0        0        0      621 2024-05-13 19:49:31.000000 metals_api_zylalabs-0.3/metals_api_zylalabs/client.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:52:24.011432 metals_api_zylalabs-0.3/metals_api_zylalabs.egg-info/
+-rw-rw-rw-   0        0        0     1072 2024-05-13 19:52:23.000000 metals_api_zylalabs-0.3/metals_api_zylalabs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2024-05-13 19:52:23.000000 metals_api_zylalabs-0.3/metals_api_zylalabs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 19:52:23.000000 metals_api_zylalabs-0.3/metals_api_zylalabs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-13 19:52:23.000000 metals_api_zylalabs-0.3/metals_api_zylalabs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 19:52:24.014775 metals_api_zylalabs-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      333 2024-05-13 19:48:50.000000 metals_api_zylalabs-0.3/setup.py
```

### Comparing `metals_api_zylalabs-0.2/PKG-INFO` & `metals_api_zylalabs-0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metals_api_zylalabs
-Version: 0.2
+Version: 0.3
 Description-Content-Type: text/markdown
 
 # Metals-API Python SDK
 
 [Metals-API](https://metals-api.com) - The ultimate API for accessing precious metals spot prices and historical data effortlessly. Explore real-time and historical metal rates with exceptional accuracy.
 
 ## Installation
@@ -20,15 +20,15 @@
 The Metals-API Python SDK is a wrapper around the [requests](https://docs.python-requests.org/en/master/) library. Metals-API supports a GET request for now.
 
 Sign-up to Metals-API to [get your API key](https://metals-api.com/register) and some credits to get started.
 
 ### Making the GET request
 
 ```python
->>> from metals_api_zylalabs.main import MetalsAPI
+>>> from metals_api_zylalabs import MetalsApiClient
 
->>> client = MetalsAPI(access_key='REPLACE-WITH-YOUR-ACCESS-KEY')
+>>> client = MetalsApiClient(access_key='REPLACE-WITH-YOUR-ACCESS-KEY')
 
 >>> response = client.get_latest("base", ["symbols"])
 ```
 
 You can find all the documentation on [Metals documentation](https://metals-api.com/documentation).
```

### Comparing `metals_api_zylalabs-0.2/README.md` & `metals_api_zylalabs-0.3/metals_api_zylalabs.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Metadata-Version: 2.1
+Name: metals-api-zylalabs
+Version: 0.3
+Description-Content-Type: text/markdown
+
 # Metals-API Python SDK
 
 [Metals-API](https://metals-api.com) - The ultimate API for accessing precious metals spot prices and historical data effortlessly. Explore real-time and historical metal rates with exceptional accuracy.
 
 ## Installation
 
 You can install Metals-API Python SDK with pip.
@@ -15,15 +20,15 @@
 The Metals-API Python SDK is a wrapper around the [requests](https://docs.python-requests.org/en/master/) library. Metals-API supports a GET request for now.
 
 Sign-up to Metals-API to [get your API key](https://metals-api.com/register) and some credits to get started.
 
 ### Making the GET request
 
 ```python
->>> from metals_api_zylalabs.main import MetalsAPI
+>>> from metals_api_zylalabs import MetalsApiClient
 
->>> client = MetalsAPI(access_key='REPLACE-WITH-YOUR-ACCESS-KEY')
+>>> client = MetalsApiClient(access_key='REPLACE-WITH-YOUR-ACCESS-KEY')
 
 >>> response = client.get_latest("base", ["symbols"])
 ```
 
-You can find all the documentation on [Metals documentation](https://metals-api.com/documentation).
+You can find all the documentation on [Metals documentation](https://metals-api.com/documentation).
```

### Comparing `metals_api_zylalabs-0.2/metals_api_zylalabs/main.py` & `metals_api_zylalabs-0.3/metals_api_zylalabs/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
 
-class MetalsAPI:
+class MetalsApiClient:
     
     def __init__(self, access_key:str):
         self.access_key = access_key
         
     def get_latest(self, base:str, symbols):
         URL = "https://metals-api.com/api/latest"        
         params = {
```

### Comparing `metals_api_zylalabs-0.2/metals_api_zylalabs.egg-info/PKG-INFO` & `metals_api_zylalabs-0.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-Metadata-Version: 2.1
-Name: metals-api-zylalabs
-Version: 0.2
-Description-Content-Type: text/markdown
-
 # Metals-API Python SDK
 
 [Metals-API](https://metals-api.com) - The ultimate API for accessing precious metals spot prices and historical data effortlessly. Explore real-time and historical metal rates with exceptional accuracy.
 
 ## Installation
 
 You can install Metals-API Python SDK with pip.
@@ -20,15 +15,15 @@
 The Metals-API Python SDK is a wrapper around the [requests](https://docs.python-requests.org/en/master/) library. Metals-API supports a GET request for now.
 
 Sign-up to Metals-API to [get your API key](https://metals-api.com/register) and some credits to get started.
 
 ### Making the GET request
 
 ```python
->>> from metals_api_zylalabs.main import MetalsAPI
+>>> from metals_api_zylalabs import MetalsApiClient
 
->>> client = MetalsAPI(access_key='REPLACE-WITH-YOUR-ACCESS-KEY')
+>>> client = MetalsApiClient(access_key='REPLACE-WITH-YOUR-ACCESS-KEY')
 
 >>> response = client.get_latest("base", ["symbols"])
 ```
 
-You can find all the documentation on [Metals documentation](https://metals-api.com/documentation).
+You can find all the documentation on [Metals documentation](https://metals-api.com/documentation).
```

