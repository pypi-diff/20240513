# Comparing `tmp/spider-client-0.0.8.tar.gz` & `tmp/spider-client-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spider-client-0.0.8.tar", last modified: Thu Apr 25 16:53:30 2024, max compression
+gzip compressed data, was "spider-client-0.0.9.tar", last modified: Thu Apr 25 20:21:01 2024, max compression
```

## Comparing `spider-client-0.0.8.tar` & `spider-client-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-25 16:53:30.334222 spider-client-0.0.8/
--rw-r--r--   0 jeffreymendez   (501) staff       (20)       10 2024-04-18 16:30:24.000000 spider-client-0.0.8/LICENSE
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     4417 2024-04-25 16:53:30.334069 spider-client-0.0.8/PKG-INFO
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     3676 2024-04-23 13:53:54.000000 spider-client-0.0.8/README.md
--rw-r--r--   0 jeffreymendez   (501) staff       (20)       38 2024-04-25 16:53:30.334269 spider-client-0.0.8/setup.cfg
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     1060 2024-04-25 16:53:28.000000 spider-client-0.0.8/setup.py
-drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-25 16:53:30.333127 spider-client-0.0.8/spider/
--rw-r--r--   0 jeffreymendez   (501) staff       (20)       26 2024-04-22 13:01:33.000000 spider-client-0.0.8/spider/__init__.py
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     6479 2024-04-25 16:53:02.000000 spider-client-0.0.8/spider/spider.py
-drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-25 16:53:30.333850 spider-client-0.0.8/spider_client.egg-info/
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     4417 2024-04-25 16:53:30.000000 spider-client-0.0.8/spider_client.egg-info/PKG-INFO
--rw-r--r--   0 jeffreymendez   (501) staff       (20)      246 2024-04-25 16:53:30.000000 spider-client-0.0.8/spider_client.egg-info/SOURCES.txt
--rw-r--r--   0 jeffreymendez   (501) staff       (20)        1 2024-04-25 16:53:30.000000 spider-client-0.0.8/spider_client.egg-info/dependency_links.txt
--rw-r--r--   0 jeffreymendez   (501) staff       (20)        9 2024-04-25 16:53:30.000000 spider-client-0.0.8/spider_client.egg-info/requires.txt
--rw-r--r--   0 jeffreymendez   (501) staff       (20)        7 2024-04-25 16:53:30.000000 spider-client-0.0.8/spider_client.egg-info/top_level.txt
+drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-25 20:21:01.789296 spider-client-0.0.9/
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)       10 2024-04-18 16:30:24.000000 spider-client-0.0.9/LICENSE
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     4417 2024-04-25 20:21:01.789115 spider-client-0.0.9/PKG-INFO
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     3676 2024-04-23 13:53:54.000000 spider-client-0.0.9/README.md
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)       38 2024-04-25 20:21:01.789349 spider-client-0.0.9/setup.cfg
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     1060 2024-04-25 20:20:12.000000 spider-client-0.0.9/setup.py
+drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-25 20:21:01.788042 spider-client-0.0.9/spider/
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)       26 2024-04-22 13:01:33.000000 spider-client-0.0.9/spider/__init__.py
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     6480 2024-04-25 20:20:07.000000 spider-client-0.0.9/spider/spider.py
+drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-25 20:21:01.788909 spider-client-0.0.9/spider_client.egg-info/
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     4417 2024-04-25 20:21:01.000000 spider-client-0.0.9/spider_client.egg-info/PKG-INFO
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)      246 2024-04-25 20:21:01.000000 spider-client-0.0.9/spider_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)        1 2024-04-25 20:21:01.000000 spider-client-0.0.9/spider_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)        9 2024-04-25 20:21:01.000000 spider-client-0.0.9/spider_client.egg-info/requires.txt
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)        7 2024-04-25 20:21:01.000000 spider-client-0.0.9/spider_client.egg-info/top_level.txt
```

### Comparing `spider-client-0.0.8/PKG-INFO` & `spider-client-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-client
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python SDK for Spider Cloud API
 Home-page: https://github.com/spider-rs/spider-clients/tree/main/python
 Author: Spider
 Author-email: jeff@a11ywatch.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `spider-client-0.0.8/README.md` & `spider-client-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `spider-client-0.0.8/setup.py` & `spider-client-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def read_file(fname):
     return open(os.path.join(os.path.dirname(__file__), fname), encoding="utf-8").read()
 
 
 setup(
     name="spider-client",
-    version="0.0.8",
+    version="0.0.9",
     url="https://github.com/spider-rs/spider-clients/tree/main/python",
     author="Spider",
     author_email="jeff@a11ywatch.com",
     description="Python SDK for Spider Cloud API",
     packages=find_packages(),
     install_requires=[
         "requests",
```

### Comparing `spider-client-0.0.8/spider/spider.py` & `spider-client-0.0.9/spider/spider.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 
     def get_crawl_state(self, url, params=None):
         """
         Retrieve the website active crawl state.
 
         :return: JSON response of the crawl state and credits used.
         """
-        return self.api_post("crawl-state", {"url": url, **(params or {})})
+        return self.api_post("crawl/status", {"url": url, **(params or {})})
 
     def get_credits(self):
         """
         Retrieve the account's remaining credits.
 
         :return: JSON response containing the number of credits left.
         """
```

### Comparing `spider-client-0.0.8/spider_client.egg-info/PKG-INFO` & `spider-client-0.0.9/spider_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-client
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python SDK for Spider Cloud API
 Home-page: https://github.com/spider-rs/spider-clients/tree/main/python
 Author: Spider
 Author-email: jeff@a11ywatch.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

