# Comparing `tmp/synochatbot-1.4.tar.gz` & `tmp/synochatbot-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synochatbot-1.4.tar", last modified: Mon May 13 15:58:21 2024, max compression
+gzip compressed data, was "synochatbot-1.5.tar", last modified: Mon May 13 16:13:35 2024, max compression
```

## Comparing `synochatbot-1.4.tar` & `synochatbot-1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 15:58:21.479067 synochatbot-1.4/
--rw-r--r--   0 ct         (502) staff       (20)      856 2024-05-13 15:58:21.478883 synochatbot-1.4/PKG-INFO
--rw-r--r--   0 ct         (502) staff       (20)       38 2024-05-13 15:58:21.479105 synochatbot-1.4/setup.cfg
--rw-r--r--   0 ct         (502) staff       (20)     1005 2024-05-13 15:55:16.000000 synochatbot-1.4/setup.py
-drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 15:58:21.477852 synochatbot-1.4/synochatbot/
--rw-r--r--   0 ct         (502) staff       (20)      573 2024-05-13 04:29:50.000000 synochatbot-1.4/synochatbot/__init__.py
--rw-r--r--   0 ct         (502) staff       (20)     3372 2024-05-13 15:08:15.000000 synochatbot-1.4/synochatbot/bot.py
-drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 15:58:21.478680 synochatbot-1.4/synochatbot.egg-info/
--rw-r--r--   0 ct         (502) staff       (20)      856 2024-05-13 15:58:21.000000 synochatbot-1.4/synochatbot.egg-info/PKG-INFO
--rw-r--r--   0 ct         (502) staff       (20)      225 2024-05-13 15:58:21.000000 synochatbot-1.4/synochatbot.egg-info/SOURCES.txt
--rw-r--r--   0 ct         (502) staff       (20)        1 2024-05-13 15:58:21.000000 synochatbot-1.4/synochatbot.egg-info/dependency_links.txt
--rw-r--r--   0 ct         (502) staff       (20)       30 2024-05-13 15:58:21.000000 synochatbot-1.4/synochatbot.egg-info/requires.txt
--rw-r--r--   0 ct         (502) staff       (20)       12 2024-05-13 15:58:21.000000 synochatbot-1.4/synochatbot.egg-info/top_level.txt
+drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 16:13:35.478146 synochatbot-1.5/
+-rw-r--r--   0 ct         (502) staff       (20)      865 2024-05-13 16:13:35.477905 synochatbot-1.5/PKG-INFO
+-rw-r--r--   0 ct         (502) staff       (20)       38 2024-05-13 16:13:35.478195 synochatbot-1.5/setup.cfg
+-rw-r--r--   0 ct         (502) staff       (20)     1014 2024-05-13 16:13:11.000000 synochatbot-1.5/setup.py
+drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 16:13:35.476760 synochatbot-1.5/synochatbot/
+-rw-r--r--   0 ct         (502) staff       (20)      573 2024-05-13 04:29:50.000000 synochatbot-1.5/synochatbot/__init__.py
+-rw-r--r--   0 ct         (502) staff       (20)     3930 2024-05-13 16:12:07.000000 synochatbot-1.5/synochatbot/bot.py
+drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 16:13:35.477642 synochatbot-1.5/synochatbot.egg-info/
+-rw-r--r--   0 ct         (502) staff       (20)      865 2024-05-13 16:13:35.000000 synochatbot-1.5/synochatbot.egg-info/PKG-INFO
+-rw-r--r--   0 ct         (502) staff       (20)      225 2024-05-13 16:13:35.000000 synochatbot-1.5/synochatbot.egg-info/SOURCES.txt
+-rw-r--r--   0 ct         (502) staff       (20)        1 2024-05-13 16:13:35.000000 synochatbot-1.5/synochatbot.egg-info/dependency_links.txt
+-rw-r--r--   0 ct         (502) staff       (20)       30 2024-05-13 16:13:35.000000 synochatbot-1.5/synochatbot.egg-info/requires.txt
+-rw-r--r--   0 ct         (502) staff       (20)       12 2024-05-13 16:13:35.000000 synochatbot-1.5/synochatbot.egg-info/top_level.txt
```

### Comparing `synochatbot-1.4/PKG-INFO` & `synochatbot-1.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synochatbot
-Version: 1.4
+Version: 1.5
 Summary: A discord.py like thing but for synology chat
 Author: kokofixcomputers
 Description-Content-Type: text/markdown
 Requires-Dist: flask==3.0.3
 Requires-Dist: requests==2.31.0
 
 
@@ -27,14 +27,14 @@
 
 @instance.message(alias="hi")
 def say_hi(message):
     return ('Hi!')
 
 @instance.message(alias='return_test')
 def return_test(message, command=None):
-    return "Hello"
+    return message.username
 
 # ... (other message handlers)
 
 synochat.run_bot(instance, outgoing_webhook, incomming_webhook_token)
 ```
```

### Comparing `synochatbot-1.4/setup.py` & `synochatbot-1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='synochatbot',
-    version='1.4',
+    version='1.5',
     author='kokofixcomputers',
     description='A discord.py like thing but for synology chat',
     long_description_content_type='text/markdown',
     long_description='''
 # A python library like discord.py but for synology chat.
 
 It allows you to create a bot that can be used to respond to messages in synology chat.
@@ -26,15 +26,15 @@
 
 @instance.message(alias="hi")
 def say_hi(message):
     return ('Hi!')
 
 @instance.message(alias='return_test')
 def return_test(message, command=None):
-    return "Hello"
+    return message.username
 
 # ... (other message handlers)
 
 synochat.run_bot(instance, outgoing_webhook, incomming_webhook_token)
 ```
     ''',
     packages=find_packages(),
```

### Comparing `synochatbot-1.4/synochatbot/__init__.py` & `synochatbot-1.5/synochatbot/__init__.py`

 * *Files identical despite different names*

### Comparing `synochatbot-1.4/synochatbot.egg-info/PKG-INFO` & `synochatbot-1.5/synochatbot.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synochatbot
-Version: 1.4
+Version: 1.5
 Summary: A discord.py like thing but for synology chat
 Author: kokofixcomputers
 Description-Content-Type: text/markdown
 Requires-Dist: flask==3.0.3
 Requires-Dist: requests==2.31.0
 
 
@@ -27,14 +27,14 @@
 
 @instance.message(alias="hi")
 def say_hi(message):
     return ('Hi!')
 
 @instance.message(alias='return_test')
 def return_test(message, command=None):
-    return "Hello"
+    return message.username
 
 # ... (other message handlers)
 
 synochat.run_bot(instance, outgoing_webhook, incomming_webhook_token)
 ```
```

