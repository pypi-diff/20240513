# Comparing `tmp/aparat_crawler-0.9.1.6.tar.gz` & `tmp/aparat_crawler-0.9.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aparat_crawler-0.9.1.6.tar", last modified: Mon May 13 06:15:27 2024, max compression
+gzip compressed data, was "aparat_crawler-0.9.1.7.tar", last modified: Mon May 13 06:25:39 2024, max compression
```

## Comparing `aparat_crawler-0.9.1.6.tar` & `aparat_crawler-0.9.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 06:15:27.878009 aparat_crawler-0.9.1.6/
--rw-rw-rw-   0        0        0        0 2024-02-10 08:06:39.000000 aparat_crawler-0.9.1.6/LICENSE
--rw-rw-rw-   0        0        0      517 2024-05-13 06:15:27.878009 aparat_crawler-0.9.1.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-02-10 08:06:33.000000 aparat_crawler-0.9.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 06:15:27.854555 aparat_crawler-0.9.1.6/aparatCrawler/
--rw-rw-rw-   0        0        0        0 2024-02-10 08:06:03.000000 aparat_crawler-0.9.1.6/aparatCrawler/__init__.py
--rw-rw-rw-   0        0        0     1230 2024-03-01 09:13:38.000000 aparat_crawler-0.9.1.6/aparatCrawler/firstPageFetcher.py
--rw-rw-rw-   0        0        0     2867 2024-03-09 09:08:39.000000 aparat_crawler-0.9.1.6/aparatCrawler/getChanneldetails.py
--rw-rw-rw-   0        0        0      613 2024-03-01 09:15:04.000000 aparat_crawler-0.9.1.6/aparatCrawler/getOfficialChannels.py
--rw-rw-rw-   0        0        0      755 2024-03-01 09:15:27.000000 aparat_crawler-0.9.1.6/aparatCrawler/getVideoRecommndedChannles.py
--rw-rw-rw-   0        0        0     8110 2024-05-13 06:14:50.000000 aparat_crawler-0.9.1.6/aparatCrawler/getVideodetails.py
--rw-rw-rw-   0        0        0     7532 2024-05-11 10:46:18.000000 aparat_crawler-0.9.1.6/aparatCrawler/getchaneelVideosDetail.py
--rw-rw-rw-   0        0        0     2922 2024-03-01 09:14:44.000000 aparat_crawler-0.9.1.6/aparatCrawler/getchaneelVideosuid.py
--rw-rw-rw-   0        0        0     1894 2024-03-01 09:15:41.000000 aparat_crawler-0.9.1.6/aparatCrawler/search.py
-drwxrwxrwx   0        0        0        0 2024-05-13 06:15:27.876998 aparat_crawler-0.9.1.6/aparat_crawler.egg-info/
--rw-rw-rw-   0        0        0      517 2024-05-13 06:15:27.000000 aparat_crawler-0.9.1.6/aparat_crawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2024-05-13 06:15:27.000000 aparat_crawler-0.9.1.6/aparat_crawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 06:15:27.000000 aparat_crawler-0.9.1.6/aparat_crawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2024-05-13 06:15:27.000000 aparat_crawler-0.9.1.6/aparat_crawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-13 06:15:27.000000 aparat_crawler-0.9.1.6/aparat_crawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 06:15:27.881721 aparat_crawler-0.9.1.6/setup.cfg
--rw-rw-rw-   0        0        0      669 2024-05-13 06:15:23.000000 aparat_crawler-0.9.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 06:25:39.616743 aparat_crawler-0.9.1.7/
+-rw-rw-rw-   0        0        0        0 2024-02-10 08:06:39.000000 aparat_crawler-0.9.1.7/LICENSE
+-rw-rw-rw-   0        0        0      517 2024-05-13 06:25:39.616743 aparat_crawler-0.9.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-02-10 08:06:33.000000 aparat_crawler-0.9.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 06:25:39.586878 aparat_crawler-0.9.1.7/aparatCrawler/
+-rw-rw-rw-   0        0        0        0 2024-02-10 08:06:03.000000 aparat_crawler-0.9.1.7/aparatCrawler/__init__.py
+-rw-rw-rw-   0        0        0     1230 2024-03-01 09:13:38.000000 aparat_crawler-0.9.1.7/aparatCrawler/firstPageFetcher.py
+-rw-rw-rw-   0        0        0     2867 2024-03-09 09:08:39.000000 aparat_crawler-0.9.1.7/aparatCrawler/getChanneldetails.py
+-rw-rw-rw-   0        0        0      613 2024-03-01 09:15:04.000000 aparat_crawler-0.9.1.7/aparatCrawler/getOfficialChannels.py
+-rw-rw-rw-   0        0        0      755 2024-03-01 09:15:27.000000 aparat_crawler-0.9.1.7/aparatCrawler/getVideoRecommndedChannles.py
+-rw-rw-rw-   0        0        0     8111 2024-05-13 06:25:27.000000 aparat_crawler-0.9.1.7/aparatCrawler/getVideodetails.py
+-rw-rw-rw-   0        0        0     7532 2024-05-11 10:46:18.000000 aparat_crawler-0.9.1.7/aparatCrawler/getchaneelVideosDetail.py
+-rw-rw-rw-   0        0        0     2922 2024-03-01 09:14:44.000000 aparat_crawler-0.9.1.7/aparatCrawler/getchaneelVideosuid.py
+-rw-rw-rw-   0        0        0     1894 2024-03-01 09:15:41.000000 aparat_crawler-0.9.1.7/aparatCrawler/search.py
+drwxrwxrwx   0        0        0        0 2024-05-13 06:25:39.615101 aparat_crawler-0.9.1.7/aparat_crawler.egg-info/
+-rw-rw-rw-   0        0        0      517 2024-05-13 06:25:39.000000 aparat_crawler-0.9.1.7/aparat_crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      535 2024-05-13 06:25:39.000000 aparat_crawler-0.9.1.7/aparat_crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 06:25:39.000000 aparat_crawler-0.9.1.7/aparat_crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2024-05-13 06:25:39.000000 aparat_crawler-0.9.1.7/aparat_crawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-13 06:25:39.000000 aparat_crawler-0.9.1.7/aparat_crawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 06:25:39.616743 aparat_crawler-0.9.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      669 2024-05-13 06:25:33.000000 aparat_crawler-0.9.1.7/setup.py
```

### Comparing `aparat_crawler-0.9.1.6/PKG-INFO` & `aparat_crawler-0.9.1.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aparat_crawler
-Version: 0.9.1.6
+Version: 0.9.1.7
 Summary: this is an aparat crawler library
 Home-page: https://github.com/maorojloo/aparat_crawler
 Author: Mohammad Amin Orojloo
 Author-email: ma.orojloo@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aparat_crawler-0.9.1.6/aparatCrawler/firstPageFetcher.py` & `aparat_crawler-0.9.1.7/aparatCrawler/firstPageFetcher.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1.6/aparatCrawler/getChanneldetails.py` & `aparat_crawler-0.9.1.7/aparatCrawler/getChanneldetails.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1.6/aparatCrawler/getOfficialChannels.py` & `aparat_crawler-0.9.1.7/aparatCrawler/getOfficialChannels.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1.6/aparatCrawler/getVideoRecommndedChannles.py` & `aparat_crawler-0.9.1.7/aparatCrawler/getVideoRecommndedChannles.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1.6/aparatCrawler/getVideodetails.py` & `aparat_crawler-0.9.1.7/aparatCrawler/getVideodetails.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,17 +62,18 @@
     response=None
     global video
 
     connector = ProxyConnector.from_url(proxy)
     async with aiohttp.ClientSession(connector=connector) as session:
         async with session.get(url) as response:
             if response.status != 200:
-                raise Exception(f"Aparat api error {response.status}")
                 print(f"proxy is : {proxy}")
                 print(f"url is :{url}")
+                raise Exception(f"Aparat api error {response.status}")
+
             data = await response.json()
 
 
 
     video=None
     if isinstance(data["data"], list):
         included=data["data"][0]
```

### Comparing `aparat_crawler-0.9.1.6/aparatCrawler/getchaneelVideosDetail.py` & `aparat_crawler-0.9.1.7/aparatCrawler/getchaneelVideosDetail.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1.6/aparatCrawler/getchaneelVideosuid.py` & `aparat_crawler-0.9.1.7/aparatCrawler/getchaneelVideosuid.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1.6/aparatCrawler/search.py` & `aparat_crawler-0.9.1.7/aparatCrawler/search.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1.6/aparat_crawler.egg-info/PKG-INFO` & `aparat_crawler-0.9.1.7/aparat_crawler.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aparat_crawler
-Version: 0.9.1.6
+Version: 0.9.1.7
 Summary: this is an aparat crawler library
 Home-page: https://github.com/maorojloo/aparat_crawler
 Author: Mohammad Amin Orojloo
 Author-email: ma.orojloo@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aparat_crawler-0.9.1.6/aparat_crawler.egg-info/SOURCES.txt` & `aparat_crawler-0.9.1.7/aparat_crawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1.6/setup.py` & `aparat_crawler-0.9.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aparat_crawler',
-    version='0.9.1.6',
+    version='0.9.1.7',
     packages=find_packages(),
     author='Mohammad Amin Orojloo',
     author_email='ma.orojloo@gmail.com',
     description='this is an aparat crawler library',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/maorojloo/aparat_crawler',
```

