# Comparing `tmp/synochatbot-2.2.tar.gz` & `tmp/synochatbot-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synochatbot-2.2.tar", last modified: Mon May 13 17:01:17 2024, max compression
+gzip compressed data, was "synochatbot-2.3.tar", last modified: Mon May 13 17:04:58 2024, max compression
```

## Comparing `synochatbot-2.2.tar` & `synochatbot-2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 17:01:17.678933 synochatbot-2.2/
--rw-r--r--   0 ct         (502) staff       (20)      886 2024-05-13 17:01:17.678444 synochatbot-2.2/PKG-INFO
--rw-r--r--   0 ct         (502) staff       (20)       38 2024-05-13 17:01:17.678999 synochatbot-2.2/setup.cfg
--rw-r--r--   0 ct         (502) staff       (20)     1035 2024-05-13 17:00:57.000000 synochatbot-2.2/setup.py
-drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 17:01:17.675735 synochatbot-2.2/synochat/
--rw-r--r--   0 ct         (502) staff       (20)      968 2024-05-13 16:57:00.000000 synochatbot-2.2/synochat/__init__.py
--rw-r--r--   0 ct         (502) staff       (20)     3707 2024-05-13 16:59:15.000000 synochatbot-2.2/synochat/bot.py
-drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 17:01:17.677801 synochatbot-2.2/synochatbot.egg-info/
--rw-r--r--   0 ct         (502) staff       (20)      886 2024-05-13 17:01:17.000000 synochatbot-2.2/synochatbot.egg-info/PKG-INFO
--rw-r--r--   0 ct         (502) staff       (20)      219 2024-05-13 17:01:17.000000 synochatbot-2.2/synochatbot.egg-info/SOURCES.txt
--rw-r--r--   0 ct         (502) staff       (20)        1 2024-05-13 17:01:17.000000 synochatbot-2.2/synochatbot.egg-info/dependency_links.txt
--rw-r--r--   0 ct         (502) staff       (20)       30 2024-05-13 17:01:17.000000 synochatbot-2.2/synochatbot.egg-info/requires.txt
--rw-r--r--   0 ct         (502) staff       (20)        9 2024-05-13 17:01:17.000000 synochatbot-2.2/synochatbot.egg-info/top_level.txt
+drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 17:04:58.113732 synochatbot-2.3/
+-rw-r--r--   0 ct         (502) staff       (20)      886 2024-05-13 17:04:58.113521 synochatbot-2.3/PKG-INFO
+-rw-r--r--   0 ct         (502) staff       (20)       38 2024-05-13 17:04:58.113782 synochatbot-2.3/setup.cfg
+-rw-r--r--   0 ct         (502) staff       (20)     1035 2024-05-13 17:04:27.000000 synochatbot-2.3/setup.py
+drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 17:04:58.112217 synochatbot-2.3/synochatbot/
+-rw-r--r--   0 ct         (502) staff       (20)      968 2024-05-13 16:57:00.000000 synochatbot-2.3/synochatbot/__init__.py
+-rw-r--r--   0 ct         (502) staff       (20)     3707 2024-05-13 16:59:15.000000 synochatbot-2.3/synochatbot/bot.py
+drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 17:04:58.113261 synochatbot-2.3/synochatbot.egg-info/
+-rw-r--r--   0 ct         (502) staff       (20)      886 2024-05-13 17:04:58.000000 synochatbot-2.3/synochatbot.egg-info/PKG-INFO
+-rw-r--r--   0 ct         (502) staff       (20)      225 2024-05-13 17:04:58.000000 synochatbot-2.3/synochatbot.egg-info/SOURCES.txt
+-rw-r--r--   0 ct         (502) staff       (20)        1 2024-05-13 17:04:58.000000 synochatbot-2.3/synochatbot.egg-info/dependency_links.txt
+-rw-r--r--   0 ct         (502) staff       (20)       30 2024-05-13 17:04:58.000000 synochatbot-2.3/synochatbot.egg-info/requires.txt
+-rw-r--r--   0 ct         (502) staff       (20)       12 2024-05-13 17:04:58.000000 synochatbot-2.3/synochatbot.egg-info/top_level.txt
```

### Comparing `synochatbot-2.2/PKG-INFO` & `synochatbot-2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synochatbot
-Version: 2.2
+Version: 2.3
 Summary: A discord.py like thing but for synology chat
 Author: kokofixcomputers
 Description-Content-Type: text/markdown
 Requires-Dist: flask==3.0.3
 Requires-Dist: requests==2.31.0
```

### Comparing `synochatbot-2.2/setup.py` & `synochatbot-2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='synochatbot',
-    version='2.2',
+    version='2.3',
     author='kokofixcomputers',
     description='A discord.py like thing but for synology chat',
     long_description_content_type='text/markdown',
     long_description='''
 # A python library like discord.py but for synology chat.
 
 It allows you to create a bot that can be used to respond to messages in synology chat.
```

### Comparing `synochatbot-2.2/synochat/__init__.py` & `synochatbot-2.3/synochatbot/__init__.py`

 * *Files identical despite different names*

### Comparing `synochatbot-2.2/synochat/bot.py` & `synochatbot-2.3/synochatbot/bot.py`

 * *Files identical despite different names*

### Comparing `synochatbot-2.2/synochatbot.egg-info/PKG-INFO` & `synochatbot-2.3/synochatbot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synochatbot
-Version: 2.2
+Version: 2.3
 Summary: A discord.py like thing but for synology chat
 Author: kokofixcomputers
 Description-Content-Type: text/markdown
 Requires-Dist: flask==3.0.3
 Requires-Dist: requests==2.31.0
```

