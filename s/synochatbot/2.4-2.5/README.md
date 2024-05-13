# Comparing `tmp/synochatbot-2.4.tar.gz` & `tmp/synochatbot-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synochatbot-2.4.tar", last modified: Mon May 13 17:09:14 2024, max compression
+gzip compressed data, was "synochatbot-2.5.tar", last modified: Mon May 13 17:11:26 2024, max compression
```

## Comparing `synochatbot-2.4.tar` & `synochatbot-2.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 17:09:14.285298 synochatbot-2.4/
--rw-r--r--   0 ct         (502) staff       (20)     1030 2024-05-13 17:09:14.285091 synochatbot-2.4/PKG-INFO
--rw-r--r--   0 ct         (502) staff       (20)       38 2024-05-13 17:09:14.285349 synochatbot-2.4/setup.cfg
--rw-r--r--   0 ct         (502) staff       (20)     1179 2024-05-13 17:07:53.000000 synochatbot-2.4/setup.py
-drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 17:09:14.283968 synochatbot-2.4/synochatbot/
--rw-r--r--   0 ct         (502) staff       (20)      917 2024-05-13 17:06:26.000000 synochatbot-2.4/synochatbot/__init__.py
--rw-r--r--   0 ct         (502) staff       (20)     3699 2024-05-13 17:06:15.000000 synochatbot-2.4/synochatbot/bot.py
-drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 17:09:14.284826 synochatbot-2.4/synochatbot.egg-info/
--rw-r--r--   0 ct         (502) staff       (20)     1030 2024-05-13 17:09:14.000000 synochatbot-2.4/synochatbot.egg-info/PKG-INFO
--rw-r--r--   0 ct         (502) staff       (20)      225 2024-05-13 17:09:14.000000 synochatbot-2.4/synochatbot.egg-info/SOURCES.txt
--rw-r--r--   0 ct         (502) staff       (20)        1 2024-05-13 17:09:14.000000 synochatbot-2.4/synochatbot.egg-info/dependency_links.txt
--rw-r--r--   0 ct         (502) staff       (20)       30 2024-05-13 17:09:14.000000 synochatbot-2.4/synochatbot.egg-info/requires.txt
--rw-r--r--   0 ct         (502) staff       (20)       12 2024-05-13 17:09:14.000000 synochatbot-2.4/synochatbot.egg-info/top_level.txt
+drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 17:11:26.003090 synochatbot-2.5/
+-rw-r--r--   0 ct         (502) staff       (20)     1030 2024-05-13 17:11:26.002891 synochatbot-2.5/PKG-INFO
+-rw-r--r--   0 ct         (502) staff       (20)       38 2024-05-13 17:11:26.003130 synochatbot-2.5/setup.cfg
+-rw-r--r--   0 ct         (502) staff       (20)     1179 2024-05-13 17:10:59.000000 synochatbot-2.5/setup.py
+drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 17:11:26.000016 synochatbot-2.5/synochatbot/
+-rw-r--r--   0 ct         (502) staff       (20)      905 2024-05-13 17:10:46.000000 synochatbot-2.5/synochatbot/__init__.py
+-rw-r--r--   0 ct         (502) staff       (20)     3699 2024-05-13 17:06:15.000000 synochatbot-2.5/synochatbot/bot.py
+drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 17:11:26.001839 synochatbot-2.5/synochatbot.egg-info/
+-rw-r--r--   0 ct         (502) staff       (20)     1030 2024-05-13 17:11:25.000000 synochatbot-2.5/synochatbot.egg-info/PKG-INFO
+-rw-r--r--   0 ct         (502) staff       (20)      225 2024-05-13 17:11:25.000000 synochatbot-2.5/synochatbot.egg-info/SOURCES.txt
+-rw-r--r--   0 ct         (502) staff       (20)        1 2024-05-13 17:11:25.000000 synochatbot-2.5/synochatbot.egg-info/dependency_links.txt
+-rw-r--r--   0 ct         (502) staff       (20)       30 2024-05-13 17:11:25.000000 synochatbot-2.5/synochatbot.egg-info/requires.txt
+-rw-r--r--   0 ct         (502) staff       (20)       12 2024-05-13 17:11:25.000000 synochatbot-2.5/synochatbot.egg-info/top_level.txt
```

### Comparing `synochatbot-2.4/PKG-INFO` & `synochatbot-2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synochatbot
-Version: 2.4
+Version: 2.5
 Summary: A discord.py like thing but for synology chat
 Author: kokofixcomputers
 Description-Content-Type: text/markdown
 Requires-Dist: flask==3.0.3
 Requires-Dist: requests==2.31.0
```

### Comparing `synochatbot-2.4/setup.py` & `synochatbot-2.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='synochatbot',
-    version='2.4',
+    version='2.5',
     author='kokofixcomputers',
     description='A discord.py like thing but for synology chat',
     long_description_content_type='text/markdown',
     long_description='''
 # A python library like discord.py but for synology chat.
 
 It allows you to create a bot that can be used to respond to messages in synology chat.
```

### Comparing `synochatbot-2.4/synochatbot/__init__.py` & `synochatbot-2.5/synochatbot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,9 +25,9 @@
             return func(*args, **kwargs)
     
         return wrapper
 
     def run(self, **kwargs):
         flask_thread = threading.Thread(target=app.run, kwargs=kwargs)
         flask_thread.start()
-def instance(prefix):
-    return SynoBot(prefix)
+def instance():
+    return SynoBot()
```

### Comparing `synochatbot-2.4/synochatbot/bot.py` & `synochatbot-2.5/synochatbot/bot.py`

 * *Files identical despite different names*

### Comparing `synochatbot-2.4/synochatbot.egg-info/PKG-INFO` & `synochatbot-2.5/synochatbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synochatbot
-Version: 2.4
+Version: 2.5
 Summary: A discord.py like thing but for synology chat
 Author: kokofixcomputers
 Description-Content-Type: text/markdown
 Requires-Dist: flask==3.0.3
 Requires-Dist: requests==2.31.0
```

