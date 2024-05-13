# Comparing `tmp/zhlyr-3.7.tar.gz` & `tmp/zhlyr-3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhlyr-3.7.tar", last modified: Fri May 10 18:27:43 2024, max compression
+gzip compressed data, was "zhlyr-3.8.tar", last modified: Mon May 13 08:39:06 2024, max compression
```

## Comparing `zhlyr-3.7.tar` & `zhlyr-3.8.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0 whoami    (1000) whoami    (1000)        0 2024-05-10 18:27:43.271094 zhlyr-3.7/
--rwxrwxrwx   0 whoami    (1000) whoami    (1000)      865 2024-05-10 18:27:43.265589 zhlyr-3.7/PKG-INFO
--rwxrwxrwx   0 whoami    (1000) whoami    (1000)       38 2024-05-10 18:27:43.272098 zhlyr-3.7/setup.cfg
--rwxrwxrwx   0 whoami    (1000) whoami    (1000)     1081 2024-05-10 18:27:28.000000 zhlyr-3.7/setup.py
-drwxrwxrwx   0 whoami    (1000) whoami    (1000)        0 2024-05-10 18:27:43.189770 zhlyr-3.7/zhlyr/
--rwxrwxrwx   0 whoami    (1000) whoami    (1000)       92 2024-05-10 14:01:33.000000 zhlyr-3.7/zhlyr/__init__.py
--rwxrwxrwx   0 whoami    (1000) whoami    (1000)     1445 2024-05-10 10:49:35.000000 zhlyr-3.7/zhlyr/recosnize.py
--rwxrwxrwx   0 whoami    (1000) whoami    (1000)     1933 2024-05-10 13:40:19.000000 zhlyr-3.7/zhlyr/serilize.py
--rwxrwxrwx   0 whoami    (1000) whoami    (1000)     2179 2024-05-10 18:26:37.000000 zhlyr-3.7/zhlyr/zhlyr.py
-drwxrwxrwx   0 whoami    (1000) whoami    (1000)        0 2024-05-10 18:27:43.258080 zhlyr-3.7/zhlyr.egg-info/
--rwxrwxrwx   0 whoami    (1000) whoami    (1000)      865 2024-05-10 18:27:43.000000 zhlyr-3.7/zhlyr.egg-info/PKG-INFO
--rwxrwxrwx   0 whoami    (1000) whoami    (1000)      194 2024-05-10 18:27:43.000000 zhlyr-3.7/zhlyr.egg-info/SOURCES.txt
--rwxrwxrwx   0 whoami    (1000) whoami    (1000)        1 2024-05-10 18:27:43.000000 zhlyr-3.7/zhlyr.egg-info/dependency_links.txt
--rwxrwxrwx   0 whoami    (1000) whoami    (1000)        6 2024-05-10 18:27:43.000000 zhlyr-3.7/zhlyr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 08:39:06.406922 zhlyr-3.8/
+-rw-rw-rw-   0        0        0     3941 2024-05-13 08:39:06.404922 zhlyr-3.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3166 2024-05-13 08:38:44.000000 zhlyr-3.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-13 08:39:06.406922 zhlyr-3.8/setup.cfg
+-rw-rw-rw-   0        0        0     1113 2024-05-13 08:36:32.000000 zhlyr-3.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:39:06.378872 zhlyr-3.8/zhlyr/
+-rw-rw-rw-   0        0        0       92 2024-05-10 14:01:33.000000 zhlyr-3.8/zhlyr/__init__.py
+-rw-rw-rw-   0        0        0     1847 2024-05-13 08:30:55.000000 zhlyr-3.8/zhlyr/recosnize.py
+-rw-rw-rw-   0        0        0     1933 2024-05-10 13:40:19.000000 zhlyr-3.8/zhlyr/serilize.py
+-rw-rw-rw-   0        0        0     2179 2024-05-10 18:26:37.000000 zhlyr-3.8/zhlyr/zhlyr.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:39:06.403922 zhlyr-3.8/zhlyr.egg-info/
+-rw-rw-rw-   0        0        0     3941 2024-05-13 08:39:06.000000 zhlyr-3.8/zhlyr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2024-05-13 08:39:06.000000 zhlyr-3.8/zhlyr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 08:39:06.000000 zhlyr-3.8/zhlyr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-13 08:39:06.000000 zhlyr-3.8/zhlyr.egg-info/top_level.txt
```

### Comparing `zhlyr-3.7/setup.py` & `zhlyr-3.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup , find_packages
-
-setup(
-    name = 'zhlyr',
-    version = '3.7',
-    packages = find_packages(),
-    requires = ['requests','shazamio','shazam'],
-    long_description ='**A python package to get lyrics from music , serialize data from json response and recognize data from musics**',
-    long_description_content_type='text/markdown',
-    description = 'Python library for music handling',
-    author = 'Mtsky',
-    author_email = 'secon2636@gmail.com',
-    url = 'https://github.com/Gaoc3/zhlyr',
-    license = 'MIT',
-    classifiers=[
-        "Development Status :: 1 - Planning",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3",
-        "Operating System :: Unix",
-        "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Microsoft :: Windows",
-    ],
-    keywords= ['lyrics','music','shazam','serialize','serializer','recognize'],
-    python_requires=">=3.9"
-)
+with open('README.md','r') as file:
+    setup(
+        name = 'zhlyr',
+        version = '3.8',
+        packages = find_packages(),
+        requires = ['requests','shazamio','shazam'],
+        long_description =file.read(),
+        long_description_content_type='text/markdown',
+        description = 'Python library for music handling',
+        author = 'Mtsky',
+        author_email = 'secon2636@gmail.com',
+        url = 'https://gaoc3.github.io/zhlyr/',
+        license = 'MIT',
+        classifiers=[
+            "Development Status :: 1 - Planning",
+            "Intended Audience :: Developers",
+            "License :: OSI Approved :: MIT License",
+            "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3",
+            "Operating System :: Unix",
+            "Operating System :: MacOS :: MacOS X",
+            "Operating System :: Microsoft :: Windows",
+        ],
+        keywords= ['lyrics','music','shazam','serialize','serializer','recognize'],
+        python_requires=">=3.9"
+    )
```

### Comparing `zhlyr-3.7/zhlyr/recosnize.py` & `zhlyr-3.8/zhlyr/recosnize.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 from typing import Union, Optional
 from shazamio import Shazam as RecoSnizer
-import json
+import json , os , asyncio
 from pathlib import Path
+from serilize import Serializer
 RecoSnizer_ = RecoSnizer()
 class RecoSnize(RecoSnizer):
     '''
     :param `data`: `bytes` | `bytearray` or `str path` | `Path` object 
     to get info from it.
     :param `proxy`: `str` | `None` to set `proxy` for your `request`
     '''
     def __init__(self, data: Union[str, bytes, bytearray , Path], proxy: Optional[str] = None,*args,**kwargs):
         super().__init__(*args, **kwargs)
         self.data = data
         self.proxy = proxy
-        with open(self.data, 'rb') as f:
-            self.data_bytes = f.read()
-        self.recognizer = self.recognize(self.data_bytes, self.proxy)
+        if isinstance(self.data,Path) or isinstance(self.data,str):
+            with open(self.data, 'rb') as f:
+                self.data_bytes = f.read()
+            self.recognizer = self.recognize(self.data_bytes, self.proxy)
+        elif isinstance(self.data,bytes) or isinstance(self.data,bytearray):
+            self.recognizer = self.recognize(self.data, self.proxy)
+        else:
+            raise TypeError('Use str , bytes , btyearry , or Path jsut.')
 
     async def json(self, **kwargs) -> dict:
         '''
         Returns a json object of the recognizer.
         '''
         respstr_ = json.dumps(await self.recognizer , **kwargs)
         resp_ = json.loads(respstr_, **kwargs)
@@ -30,14 +36,16 @@
         '''
         Returns a string of the recognizer.
         '''
         return str(await self.recognizer)
 
 
 
+# Example to use to RecoSnizer :
+
 # async def main():
 #     data_path = r'C:\Users\Mtsky\Downloads\Telegram Desktop\mzaf_17549133339911745381.plus.aac.ep (2).m4a'
 #     result = await RecoSnize(data_path).json()
 #     print(Serializer(result).track.title)
 
 # loop = asyncio.new_event_loop()
 # loop.run_until_complete(main())
```

### Comparing `zhlyr-3.7/zhlyr/serilize.py` & `zhlyr-3.8/zhlyr/serilize.py`

 * *Files identical despite different names*

### Comparing `zhlyr-3.7/zhlyr/zhlyr.py` & `zhlyr-3.8/zhlyr/zhlyr.py`

 * *Files identical despite different names*

