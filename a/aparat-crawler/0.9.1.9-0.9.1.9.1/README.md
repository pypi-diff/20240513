# Comparing `tmp/aparat_crawler-0.9.1.9.tar.gz` & `tmp/aparat_crawler-0.9.1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aparat_crawler-0.9.1.9.tar", last modified: Mon May 13 06:43:24 2024, max compression
+gzip compressed data, was "aparat_crawler-0.9.1.9.1.tar", last modified: Mon May 13 06:45:54 2024, max compression
```

## Comparing `aparat_crawler-0.9.1.9.tar` & `aparat_crawler-0.9.1.9.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 06:43:24.224488 aparat_crawler-0.9.1.9/
--rw-rw-rw-   0        0        0        0 2024-02-10 08:06:39.000000 aparat_crawler-0.9.1.9/LICENSE
--rw-rw-rw-   0        0        0      517 2024-05-13 06:43:24.224488 aparat_crawler-0.9.1.9/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-02-10 08:06:33.000000 aparat_crawler-0.9.1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 06:43:24.199648 aparat_crawler-0.9.1.9/aparatCrawler/
--rw-rw-rw-   0        0        0        0 2024-02-10 08:06:03.000000 aparat_crawler-0.9.1.9/aparatCrawler/__init__.py
--rw-rw-rw-   0        0        0     1230 2024-03-01 09:13:38.000000 aparat_crawler-0.9.1.9/aparatCrawler/firstPageFetcher.py
--rw-rw-rw-   0        0        0     2867 2024-03-09 09:08:39.000000 aparat_crawler-0.9.1.9/aparatCrawler/getChanneldetails.py
--rw-rw-rw-   0        0        0      613 2024-03-01 09:15:04.000000 aparat_crawler-0.9.1.9/aparatCrawler/getOfficialChannels.py
--rw-rw-rw-   0        0        0      755 2024-03-01 09:15:27.000000 aparat_crawler-0.9.1.9/aparatCrawler/getVideoRecommndedChannles.py
--rw-rw-rw-   0        0        0     4965 2024-05-13 06:42:58.000000 aparat_crawler-0.9.1.9/aparatCrawler/getVideodetails.py
--rw-rw-rw-   0        0        0     8111 2024-05-13 06:25:27.000000 aparat_crawler-0.9.1.9/aparatCrawler/getVideodetails_OLD.py
--rw-rw-rw-   0        0        0     7532 2024-05-11 10:46:18.000000 aparat_crawler-0.9.1.9/aparatCrawler/getchaneelVideosDetail.py
--rw-rw-rw-   0        0        0     2922 2024-03-01 09:14:44.000000 aparat_crawler-0.9.1.9/aparatCrawler/getchaneelVideosuid.py
--rw-rw-rw-   0        0        0     1894 2024-03-01 09:15:41.000000 aparat_crawler-0.9.1.9/aparatCrawler/search.py
-drwxrwxrwx   0        0        0        0 2024-05-13 06:43:24.224488 aparat_crawler-0.9.1.9/aparat_crawler.egg-info/
--rw-rw-rw-   0        0        0      517 2024-05-13 06:43:24.000000 aparat_crawler-0.9.1.9/aparat_crawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      572 2024-05-13 06:43:24.000000 aparat_crawler-0.9.1.9/aparat_crawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 06:43:24.000000 aparat_crawler-0.9.1.9/aparat_crawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2024-05-13 06:43:24.000000 aparat_crawler-0.9.1.9/aparat_crawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-13 06:43:24.000000 aparat_crawler-0.9.1.9/aparat_crawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 06:43:24.224488 aparat_crawler-0.9.1.9/setup.cfg
--rw-rw-rw-   0        0        0      669 2024-05-13 06:43:19.000000 aparat_crawler-0.9.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 06:45:54.706753 aparat_crawler-0.9.1.9.1/
+-rw-rw-rw-   0        0        0        0 2024-02-10 08:06:39.000000 aparat_crawler-0.9.1.9.1/LICENSE
+-rw-rw-rw-   0        0        0      519 2024-05-13 06:45:54.703882 aparat_crawler-0.9.1.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-02-10 08:06:33.000000 aparat_crawler-0.9.1.9.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 06:45:54.681434 aparat_crawler-0.9.1.9.1/aparatCrawler/
+-rw-rw-rw-   0        0        0        0 2024-02-10 08:06:03.000000 aparat_crawler-0.9.1.9.1/aparatCrawler/__init__.py
+-rw-rw-rw-   0        0        0     1230 2024-03-01 09:13:38.000000 aparat_crawler-0.9.1.9.1/aparatCrawler/firstPageFetcher.py
+-rw-rw-rw-   0        0        0     2867 2024-03-09 09:08:39.000000 aparat_crawler-0.9.1.9.1/aparatCrawler/getChanneldetails.py
+-rw-rw-rw-   0        0        0      613 2024-03-01 09:15:04.000000 aparat_crawler-0.9.1.9.1/aparatCrawler/getOfficialChannels.py
+-rw-rw-rw-   0        0        0      755 2024-03-01 09:15:27.000000 aparat_crawler-0.9.1.9.1/aparatCrawler/getVideoRecommndedChannles.py
+-rw-rw-rw-   0        0        0     4975 2024-05-13 06:45:39.000000 aparat_crawler-0.9.1.9.1/aparatCrawler/getVideodetails.py
+-rw-rw-rw-   0        0        0     8111 2024-05-13 06:25:27.000000 aparat_crawler-0.9.1.9.1/aparatCrawler/getVideodetails_OLD.py
+-rw-rw-rw-   0        0        0     7532 2024-05-11 10:46:18.000000 aparat_crawler-0.9.1.9.1/aparatCrawler/getchaneelVideosDetail.py
+-rw-rw-rw-   0        0        0     2922 2024-03-01 09:14:44.000000 aparat_crawler-0.9.1.9.1/aparatCrawler/getchaneelVideosuid.py
+-rw-rw-rw-   0        0        0     1894 2024-03-01 09:15:41.000000 aparat_crawler-0.9.1.9.1/aparatCrawler/search.py
+drwxrwxrwx   0        0        0        0 2024-05-13 06:45:54.703882 aparat_crawler-0.9.1.9.1/aparat_crawler.egg-info/
+-rw-rw-rw-   0        0        0      519 2024-05-13 06:45:54.000000 aparat_crawler-0.9.1.9.1/aparat_crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      572 2024-05-13 06:45:54.000000 aparat_crawler-0.9.1.9.1/aparat_crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 06:45:54.000000 aparat_crawler-0.9.1.9.1/aparat_crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2024-05-13 06:45:54.000000 aparat_crawler-0.9.1.9.1/aparat_crawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-13 06:45:54.000000 aparat_crawler-0.9.1.9.1/aparat_crawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 06:45:54.710158 aparat_crawler-0.9.1.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      671 2024-05-13 06:45:46.000000 aparat_crawler-0.9.1.9.1/setup.py
```

### Comparing `aparat_crawler-0.9.1.9/PKG-INFO` & `aparat_crawler-0.9.1.9.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aparat_crawler
-Version: 0.9.1.9
+Version: 0.9.1.9.1
 Summary: this is an aparat crawler library
 Home-page: https://github.com/maorojloo/aparat_crawler
 Author: Mohammad Amin Orojloo
 Author-email: ma.orojloo@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aparat_crawler-0.9.1.9/aparatCrawler/firstPageFetcher.py` & `aparat_crawler-0.9.1.9.1/aparatCrawler/firstPageFetcher.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1.9/aparatCrawler/getChanneldetails.py` & `aparat_crawler-0.9.1.9.1/aparatCrawler/getChanneldetails.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1.9/aparatCrawler/getOfficialChannels.py` & `aparat_crawler-0.9.1.9.1/aparatCrawler/getOfficialChannels.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1.9/aparatCrawler/getVideoRecommndedChannles.py` & `aparat_crawler-0.9.1.9.1/aparatCrawler/getVideoRecommndedChannles.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1.9/aparatCrawler/getVideodetails.py` & `aparat_crawler-0.9.1.9.1/aparatCrawler/getVideodetails.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 def getVideoDetail(videouid,proxy=None):
     url = "https://www.aparat.com/api/fa/v1/video/video/show/videohash/"+videouid
     response=None
     global video
 
     response=requests.get(url=url,proxies=proxy)
 
-    if response.status != 200:
+    if response.status_code != 200:
         print(f"proxy is : {proxy}")
         print(f"url is :{url}")
-        raise Exception(f"Aparat api error {response.status}")
+        raise Exception(f"Aparat api error {response.status_code}")
 
     data = response.json()
 
 
 
     video=None
     if isinstance(data["data"], list):
```

### Comparing `aparat_crawler-0.9.1.9/aparatCrawler/getVideodetails_OLD.py` & `aparat_crawler-0.9.1.9.1/aparatCrawler/getVideodetails_OLD.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1.9/aparatCrawler/getchaneelVideosDetail.py` & `aparat_crawler-0.9.1.9.1/aparatCrawler/getchaneelVideosDetail.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1.9/aparatCrawler/getchaneelVideosuid.py` & `aparat_crawler-0.9.1.9.1/aparatCrawler/getchaneelVideosuid.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1.9/aparatCrawler/search.py` & `aparat_crawler-0.9.1.9.1/aparatCrawler/search.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1.9/aparat_crawler.egg-info/PKG-INFO` & `aparat_crawler-0.9.1.9.1/aparat_crawler.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aparat_crawler
-Version: 0.9.1.9
+Version: 0.9.1.9.1
 Summary: this is an aparat crawler library
 Home-page: https://github.com/maorojloo/aparat_crawler
 Author: Mohammad Amin Orojloo
 Author-email: ma.orojloo@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aparat_crawler-0.9.1.9/aparat_crawler.egg-info/SOURCES.txt` & `aparat_crawler-0.9.1.9.1/aparat_crawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1.9/setup.py` & `aparat_crawler-0.9.1.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aparat_crawler',
-    version='0.9.1.9',
+    version='0.9.1.9.1',
     packages=find_packages(),
     author='Mohammad Amin Orojloo',
     author_email='ma.orojloo@gmail.com',
     description='this is an aparat crawler library',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/maorojloo/aparat_crawler',
```

