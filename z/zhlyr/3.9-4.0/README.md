# Comparing `tmp/zhlyr-3.9.tar.gz` & `tmp/zhlyr-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhlyr-3.9.tar", last modified: Mon May 13 08:43:09 2024, max compression
+gzip compressed data, was "zhlyr-4.0.tar", last modified: Mon May 13 08:48:26 2024, max compression
```

## Comparing `zhlyr-3.9.tar` & `zhlyr-4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 08:43:09.803451 zhlyr-3.9/
--rw-rw-rw-   0        0        0     3541 2024-05-13 08:43:09.802453 zhlyr-3.9/PKG-INFO
--rw-rw-rw-   0        0        0     2766 2024-05-13 08:42:41.000000 zhlyr-3.9/README.md
--rw-rw-rw-   0        0        0       42 2024-05-13 08:43:09.804450 zhlyr-3.9/setup.cfg
--rw-rw-rw-   0        0        0     1113 2024-05-13 08:42:59.000000 zhlyr-3.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:43:09.777454 zhlyr-3.9/zhlyr/
--rw-rw-rw-   0        0        0       92 2024-05-10 14:01:33.000000 zhlyr-3.9/zhlyr/__init__.py
--rw-rw-rw-   0        0        0     1847 2024-05-13 08:30:55.000000 zhlyr-3.9/zhlyr/recosnize.py
--rw-rw-rw-   0        0        0     1933 2024-05-10 13:40:19.000000 zhlyr-3.9/zhlyr/serilize.py
--rw-rw-rw-   0        0        0     2179 2024-05-10 18:26:37.000000 zhlyr-3.9/zhlyr/zhlyr.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:43:09.800451 zhlyr-3.9/zhlyr.egg-info/
--rw-rw-rw-   0        0        0     3541 2024-05-13 08:43:09.000000 zhlyr-3.9/zhlyr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2024-05-13 08:43:09.000000 zhlyr-3.9/zhlyr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 08:43:09.000000 zhlyr-3.9/zhlyr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-13 08:43:09.000000 zhlyr-3.9/zhlyr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 08:48:26.249710 zhlyr-4.0/
+-rw-rw-rw-   0        0        0     3536 2024-05-13 08:48:26.248706 zhlyr-4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2761 2024-05-13 08:47:46.000000 zhlyr-4.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-13 08:48:26.250705 zhlyr-4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1113 2024-05-13 08:48:15.000000 zhlyr-4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:48:26.228681 zhlyr-4.0/zhlyr/
+-rw-rw-rw-   0        0        0       92 2024-05-10 14:01:33.000000 zhlyr-4.0/zhlyr/__init__.py
+-rw-rw-rw-   0        0        0     1847 2024-05-13 08:30:55.000000 zhlyr-4.0/zhlyr/recosnize.py
+-rw-rw-rw-   0        0        0     1933 2024-05-10 13:40:19.000000 zhlyr-4.0/zhlyr/serilize.py
+-rw-rw-rw-   0        0        0     2179 2024-05-10 18:26:37.000000 zhlyr-4.0/zhlyr/zhlyr.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:48:26.246705 zhlyr-4.0/zhlyr.egg-info/
+-rw-rw-rw-   0        0        0     3536 2024-05-13 08:48:26.000000 zhlyr-4.0/zhlyr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2024-05-13 08:48:26.000000 zhlyr-4.0/zhlyr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 08:48:26.000000 zhlyr-4.0/zhlyr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-13 08:48:26.000000 zhlyr-4.0/zhlyr.egg-info/top_level.txt
```

### Comparing `zhlyr-3.9/PKG-INFO` & `zhlyr-4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhlyr
-Version: 3.9
+Version: 4.0
 Summary: Python library for music handling
 Home-page: https://gaoc3.github.io/zhlyr/
 Author: Mtsky
 Author-email: secon2636@gmail.com
 License: MIT
 Keywords: lyrics,music,shazam,serialize,serializer,recognize
 Classifier: Development Status :: 1 - Planning
@@ -18,16 +18,15 @@
 Requires: requests
 Requires: shazamio
 Requires: shazam
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 - ## What is zhlyr?
-
-  - **A python library aimed at music enthusiasts, providing tools for managing and discovering music, fetching song lyrics, and utilizing machine learning algorithms to predict the name of a song from a short audio snippet.**
+- **A python library aimed at music enthusiasts, providing tools for managing and discovering music, fetching song lyrics, and utilizing machine learning algorithms to predict the name of a song from a short audio snippet.**
 - ## Code Area :
 
 <details> 
 <summary>
 <i>⏬Install Zhlyr</i>
 </summary>
 
@@ -139,10 +138,10 @@
 
 </details>
 
 ## My Accounts
 
 - [GitHub](https://github.com/Gaoc3/)
 - [Instagram](https://www.instagram.com/mtsky.sensei/)
-- [Telegram](https://nar4nar.t.me) 
+- [Telegram](https://nar4nar.t.me)
 
 ---
```

### Comparing `zhlyr-3.9/README.md` & `zhlyr-4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 - ## What is zhlyr?
-
-  - **A python library aimed at music enthusiasts, providing tools for managing and discovering music, fetching song lyrics, and utilizing machine learning algorithms to predict the name of a song from a short audio snippet.**
+- **A python library aimed at music enthusiasts, providing tools for managing and discovering music, fetching song lyrics, and utilizing machine learning algorithms to predict the name of a song from a short audio snippet.**
 - ## Code Area :
 
 <details> 
 <summary>
 <i>⏬Install Zhlyr</i>
 </summary>
 
@@ -116,10 +115,10 @@
 
 </details>
 
 ## My Accounts
 
 - [GitHub](https://github.com/Gaoc3/)
 - [Instagram](https://www.instagram.com/mtsky.sensei/)
-- [Telegram](https://nar4nar.t.me) 
+- [Telegram](https://nar4nar.t.me)
 
 ---
```

### Comparing `zhlyr-3.9/setup.py` & `zhlyr-4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup , find_packages
 with open('README.md','r') as file:
     setup(
         name = 'zhlyr',
-        version = '3.9',
+        version = '4.0',
         packages = find_packages(),
         requires = ['requests','shazamio','shazam'],
         long_description =file.read(),
         long_description_content_type='text/markdown',
         description = 'Python library for music handling',
         author = 'Mtsky',
         author_email = 'secon2636@gmail.com',
```

### Comparing `zhlyr-3.9/zhlyr/recosnize.py` & `zhlyr-4.0/zhlyr/recosnize.py`

 * *Files identical despite different names*

### Comparing `zhlyr-3.9/zhlyr/serilize.py` & `zhlyr-4.0/zhlyr/serilize.py`

 * *Files identical despite different names*

### Comparing `zhlyr-3.9/zhlyr/zhlyr.py` & `zhlyr-4.0/zhlyr/zhlyr.py`

 * *Files identical despite different names*

### Comparing `zhlyr-3.9/zhlyr.egg-info/PKG-INFO` & `zhlyr-4.0/zhlyr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhlyr
-Version: 3.9
+Version: 4.0
 Summary: Python library for music handling
 Home-page: https://gaoc3.github.io/zhlyr/
 Author: Mtsky
 Author-email: secon2636@gmail.com
 License: MIT
 Keywords: lyrics,music,shazam,serialize,serializer,recognize
 Classifier: Development Status :: 1 - Planning
@@ -18,16 +18,15 @@
 Requires: requests
 Requires: shazamio
 Requires: shazam
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 - ## What is zhlyr?
-
-  - **A python library aimed at music enthusiasts, providing tools for managing and discovering music, fetching song lyrics, and utilizing machine learning algorithms to predict the name of a song from a short audio snippet.**
+- **A python library aimed at music enthusiasts, providing tools for managing and discovering music, fetching song lyrics, and utilizing machine learning algorithms to predict the name of a song from a short audio snippet.**
 - ## Code Area :
 
 <details> 
 <summary>
 <i>⏬Install Zhlyr</i>
 </summary>
 
@@ -139,10 +138,10 @@
 
 </details>
 
 ## My Accounts
 
 - [GitHub](https://github.com/Gaoc3/)
 - [Instagram](https://www.instagram.com/mtsky.sensei/)
-- [Telegram](https://nar4nar.t.me) 
+- [Telegram](https://nar4nar.t.me)
 
 ---
```

