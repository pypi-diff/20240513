# Comparing `tmp/zhlyr-3.8.tar.gz` & `tmp/zhlyr-3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhlyr-3.8.tar", last modified: Mon May 13 08:39:06 2024, max compression
+gzip compressed data, was "zhlyr-3.9.tar", last modified: Mon May 13 08:43:09 2024, max compression
```

## Comparing `zhlyr-3.8.tar` & `zhlyr-3.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 08:39:06.406922 zhlyr-3.8/
--rw-rw-rw-   0        0        0     3941 2024-05-13 08:39:06.404922 zhlyr-3.8/PKG-INFO
--rw-rw-rw-   0        0        0     3166 2024-05-13 08:38:44.000000 zhlyr-3.8/README.md
--rw-rw-rw-   0        0        0       42 2024-05-13 08:39:06.406922 zhlyr-3.8/setup.cfg
--rw-rw-rw-   0        0        0     1113 2024-05-13 08:36:32.000000 zhlyr-3.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:39:06.378872 zhlyr-3.8/zhlyr/
--rw-rw-rw-   0        0        0       92 2024-05-10 14:01:33.000000 zhlyr-3.8/zhlyr/__init__.py
--rw-rw-rw-   0        0        0     1847 2024-05-13 08:30:55.000000 zhlyr-3.8/zhlyr/recosnize.py
--rw-rw-rw-   0        0        0     1933 2024-05-10 13:40:19.000000 zhlyr-3.8/zhlyr/serilize.py
--rw-rw-rw-   0        0        0     2179 2024-05-10 18:26:37.000000 zhlyr-3.8/zhlyr/zhlyr.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:39:06.403922 zhlyr-3.8/zhlyr.egg-info/
--rw-rw-rw-   0        0        0     3941 2024-05-13 08:39:06.000000 zhlyr-3.8/zhlyr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2024-05-13 08:39:06.000000 zhlyr-3.8/zhlyr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 08:39:06.000000 zhlyr-3.8/zhlyr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-13 08:39:06.000000 zhlyr-3.8/zhlyr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 08:43:09.803451 zhlyr-3.9/
+-rw-rw-rw-   0        0        0     3541 2024-05-13 08:43:09.802453 zhlyr-3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2766 2024-05-13 08:42:41.000000 zhlyr-3.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-13 08:43:09.804450 zhlyr-3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1113 2024-05-13 08:42:59.000000 zhlyr-3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:43:09.777454 zhlyr-3.9/zhlyr/
+-rw-rw-rw-   0        0        0       92 2024-05-10 14:01:33.000000 zhlyr-3.9/zhlyr/__init__.py
+-rw-rw-rw-   0        0        0     1847 2024-05-13 08:30:55.000000 zhlyr-3.9/zhlyr/recosnize.py
+-rw-rw-rw-   0        0        0     1933 2024-05-10 13:40:19.000000 zhlyr-3.9/zhlyr/serilize.py
+-rw-rw-rw-   0        0        0     2179 2024-05-10 18:26:37.000000 zhlyr-3.9/zhlyr/zhlyr.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:43:09.800451 zhlyr-3.9/zhlyr.egg-info/
+-rw-rw-rw-   0        0        0     3541 2024-05-13 08:43:09.000000 zhlyr-3.9/zhlyr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2024-05-13 08:43:09.000000 zhlyr-3.9/zhlyr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 08:43:09.000000 zhlyr-3.9/zhlyr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-13 08:43:09.000000 zhlyr-3.9/zhlyr.egg-info/top_level.txt
```

### Comparing `zhlyr-3.8/PKG-INFO` & `zhlyr-3.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhlyr
-Version: 3.8
+Version: 3.9
 Summary: Python library for music handling
 Home-page: https://gaoc3.github.io/zhlyr/
 Author: Mtsky
 Author-email: secon2636@gmail.com
 License: MIT
 Keywords: lyrics,music,shazam,serialize,serializer,recognize
 Classifier: Development Status :: 1 - Planning
@@ -137,12 +137,12 @@
 
 ---
 
 </details>
 
 ## My Accounts
 
-- [GitHub](https://github.com/Gaoc3/) [`<img src="https://cdn-icons-png.flaticon.com/512/25/25231.png" alt="GitHub" width="20" height="20">`](https://github.com/)
-- [Instagram](https://www.instagram.com/mtsky.sensei/) [`<img src="https://cdn-icons-png.flaticon.com/512/2111/2111463.png" alt="Instagram" width="20" height="20">`](https://www.instagram.com/)
-- [Telegram](https://nar4nar.t.me) [`<img src="https://cdn-icons-png.flaticon.com/512/2111/2111646.png" alt="Telegram" width="20" height="20">`](https://web.telegram.org/)
+- [GitHub](https://github.com/Gaoc3/)
+- [Instagram](https://www.instagram.com/mtsky.sensei/)
+- [Telegram](https://nar4nar.t.me) 
 
 ---
```

### Comparing `zhlyr-3.8/README.md` & `zhlyr-3.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -114,12 +114,12 @@
 
 ---
 
 </details>
 
 ## My Accounts
 
-- [GitHub](https://github.com/Gaoc3/) [`<img src="https://cdn-icons-png.flaticon.com/512/25/25231.png" alt="GitHub" width="20" height="20">`](https://github.com/)
-- [Instagram](https://www.instagram.com/mtsky.sensei/) [`<img src="https://cdn-icons-png.flaticon.com/512/2111/2111463.png" alt="Instagram" width="20" height="20">`](https://www.instagram.com/)
-- [Telegram](https://nar4nar.t.me) [`<img src="https://cdn-icons-png.flaticon.com/512/2111/2111646.png" alt="Telegram" width="20" height="20">`](https://web.telegram.org/)
+- [GitHub](https://github.com/Gaoc3/)
+- [Instagram](https://www.instagram.com/mtsky.sensei/)
+- [Telegram](https://nar4nar.t.me) 
 
 ---
```

### Comparing `zhlyr-3.8/setup.py` & `zhlyr-3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup , find_packages
 with open('README.md','r') as file:
     setup(
         name = 'zhlyr',
-        version = '3.8',
+        version = '3.9',
         packages = find_packages(),
         requires = ['requests','shazamio','shazam'],
         long_description =file.read(),
         long_description_content_type='text/markdown',
         description = 'Python library for music handling',
         author = 'Mtsky',
         author_email = 'secon2636@gmail.com',
```

### Comparing `zhlyr-3.8/zhlyr/recosnize.py` & `zhlyr-3.9/zhlyr/recosnize.py`

 * *Files identical despite different names*

### Comparing `zhlyr-3.8/zhlyr/serilize.py` & `zhlyr-3.9/zhlyr/serilize.py`

 * *Files identical despite different names*

### Comparing `zhlyr-3.8/zhlyr/zhlyr.py` & `zhlyr-3.9/zhlyr/zhlyr.py`

 * *Files identical despite different names*

### Comparing `zhlyr-3.8/zhlyr.egg-info/PKG-INFO` & `zhlyr-3.9/zhlyr.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhlyr
-Version: 3.8
+Version: 3.9
 Summary: Python library for music handling
 Home-page: https://gaoc3.github.io/zhlyr/
 Author: Mtsky
 Author-email: secon2636@gmail.com
 License: MIT
 Keywords: lyrics,music,shazam,serialize,serializer,recognize
 Classifier: Development Status :: 1 - Planning
@@ -137,12 +137,12 @@
 
 ---
 
 </details>
 
 ## My Accounts
 
-- [GitHub](https://github.com/Gaoc3/) [`<img src="https://cdn-icons-png.flaticon.com/512/25/25231.png" alt="GitHub" width="20" height="20">`](https://github.com/)
-- [Instagram](https://www.instagram.com/mtsky.sensei/) [`<img src="https://cdn-icons-png.flaticon.com/512/2111/2111463.png" alt="Instagram" width="20" height="20">`](https://www.instagram.com/)
-- [Telegram](https://nar4nar.t.me) [`<img src="https://cdn-icons-png.flaticon.com/512/2111/2111646.png" alt="Telegram" width="20" height="20">`](https://web.telegram.org/)
+- [GitHub](https://github.com/Gaoc3/)
+- [Instagram](https://www.instagram.com/mtsky.sensei/)
+- [Telegram](https://nar4nar.t.me) 
 
 ---
```

