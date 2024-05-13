# Comparing `tmp/synochatbot-2.0.tar.gz` & `tmp/synochatbot-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synochatbot-2.0.tar", last modified: Mon May 13 16:30:57 2024, max compression
+gzip compressed data, was "synochatbot-2.1.tar", last modified: Mon May 13 16:34:22 2024, max compression
```

## Comparing `synochatbot-2.0.tar` & `synochatbot-2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 16:30:57.979387 synochatbot-2.0/
--rw-r--r--   0 ct         (502) staff       (20)      865 2024-05-13 16:30:57.979154 synochatbot-2.0/PKG-INFO
--rw-r--r--   0 ct         (502) staff       (20)       38 2024-05-13 16:30:57.979433 synochatbot-2.0/setup.cfg
--rw-r--r--   0 ct         (502) staff       (20)     1014 2024-05-13 16:30:13.000000 synochatbot-2.0/setup.py
-drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 16:30:57.977939 synochatbot-2.0/synochatbot/
--rw-r--r--   0 ct         (502) staff       (20)      573 2024-05-13 04:29:50.000000 synochatbot-2.0/synochatbot/__init__.py
--rw-r--r--   0 ct         (502) staff       (20)     3699 2024-05-13 16:29:29.000000 synochatbot-2.0/synochatbot/bot.py
-drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 16:30:57.978887 synochatbot-2.0/synochatbot.egg-info/
--rw-r--r--   0 ct         (502) staff       (20)      865 2024-05-13 16:30:57.000000 synochatbot-2.0/synochatbot.egg-info/PKG-INFO
--rw-r--r--   0 ct         (502) staff       (20)      225 2024-05-13 16:30:57.000000 synochatbot-2.0/synochatbot.egg-info/SOURCES.txt
--rw-r--r--   0 ct         (502) staff       (20)        1 2024-05-13 16:30:57.000000 synochatbot-2.0/synochatbot.egg-info/dependency_links.txt
--rw-r--r--   0 ct         (502) staff       (20)       30 2024-05-13 16:30:57.000000 synochatbot-2.0/synochatbot.egg-info/requires.txt
--rw-r--r--   0 ct         (502) staff       (20)       12 2024-05-13 16:30:57.000000 synochatbot-2.0/synochatbot.egg-info/top_level.txt
+drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 16:34:22.025163 synochatbot-2.1/
+-rw-r--r--   0 ct         (502) staff       (20)      886 2024-05-13 16:34:22.024613 synochatbot-2.1/PKG-INFO
+-rw-r--r--   0 ct         (502) staff       (20)       38 2024-05-13 16:34:22.025222 synochatbot-2.1/setup.cfg
+-rw-r--r--   0 ct         (502) staff       (20)     1035 2024-05-13 16:34:07.000000 synochatbot-2.1/setup.py
+drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 16:34:22.023386 synochatbot-2.1/synochatbot/
+-rw-r--r--   0 ct         (502) staff       (20)      573 2024-05-13 04:29:50.000000 synochatbot-2.1/synochatbot/__init__.py
+-rw-r--r--   0 ct         (502) staff       (20)     3699 2024-05-13 16:29:29.000000 synochatbot-2.1/synochatbot/bot.py
+drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 16:34:22.024365 synochatbot-2.1/synochatbot.egg-info/
+-rw-r--r--   0 ct         (502) staff       (20)      886 2024-05-13 16:34:22.000000 synochatbot-2.1/synochatbot.egg-info/PKG-INFO
+-rw-r--r--   0 ct         (502) staff       (20)      225 2024-05-13 16:34:22.000000 synochatbot-2.1/synochatbot.egg-info/SOURCES.txt
+-rw-r--r--   0 ct         (502) staff       (20)        1 2024-05-13 16:34:22.000000 synochatbot-2.1/synochatbot.egg-info/dependency_links.txt
+-rw-r--r--   0 ct         (502) staff       (20)       30 2024-05-13 16:34:22.000000 synochatbot-2.1/synochatbot.egg-info/requires.txt
+-rw-r--r--   0 ct         (502) staff       (20)       12 2024-05-13 16:34:22.000000 synochatbot-2.1/synochatbot.egg-info/top_level.txt
```

### Comparing `synochatbot-2.0/PKG-INFO` & `synochatbot-2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synochatbot
-Version: 2.0
+Version: 2.1
 Summary: A discord.py like thing but for synology chat
 Author: kokofixcomputers
 Description-Content-Type: text/markdown
 Requires-Dist: flask==3.0.3
 Requires-Dist: requests==2.31.0
 
 
@@ -21,19 +21,19 @@
 
 import time
 time.sleep(1)
 
 outgoing_webhook = "your url"
 instance = synochat.instance(prefix="?")
 
-@instance.message(alias="hi")
+@instance.message(alias="return_full_message")
 def say_hi(message):
-    return ('Hi!')
+    return message
 
-@instance.message(alias='return_test')
+@instance.message(alias='return_username')
 def return_test(message, command=None):
     return message.username
 
 # ... (other message handlers)
 
 synochat.run_bot(instance, outgoing_webhook, incomming_webhook_token)
 ```
```

### Comparing `synochatbot-2.0/setup.py` & `synochatbot-2.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='synochatbot',
-    version='2.0',
+    version='2.1',
     author='kokofixcomputers',
     description='A discord.py like thing but for synology chat',
     long_description_content_type='text/markdown',
     long_description='''
 # A python library like discord.py but for synology chat.
 
 It allows you to create a bot that can be used to respond to messages in synology chat.
@@ -20,19 +20,19 @@
 
 import time
 time.sleep(1)
 
 outgoing_webhook = "your url"
 instance = synochat.instance(prefix="?")
 
-@instance.message(alias="hi")
+@instance.message(alias="return_full_message")
 def say_hi(message):
-    return ('Hi!')
+    return message
 
-@instance.message(alias='return_test')
+@instance.message(alias='return_username')
 def return_test(message, command=None):
     return message.username
 
 # ... (other message handlers)
 
 synochat.run_bot(instance, outgoing_webhook, incomming_webhook_token)
 ```
```

### Comparing `synochatbot-2.0/synochatbot/__init__.py` & `synochatbot-2.1/synochatbot/__init__.py`

 * *Files identical despite different names*

### Comparing `synochatbot-2.0/synochatbot/bot.py` & `synochatbot-2.1/synochatbot/bot.py`

 * *Files identical despite different names*

### Comparing `synochatbot-2.0/synochatbot.egg-info/PKG-INFO` & `synochatbot-2.1/synochatbot.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synochatbot
-Version: 2.0
+Version: 2.1
 Summary: A discord.py like thing but for synology chat
 Author: kokofixcomputers
 Description-Content-Type: text/markdown
 Requires-Dist: flask==3.0.3
 Requires-Dist: requests==2.31.0
 
 
@@ -21,19 +21,19 @@
 
 import time
 time.sleep(1)
 
 outgoing_webhook = "your url"
 instance = synochat.instance(prefix="?")
 
-@instance.message(alias="hi")
+@instance.message(alias="return_full_message")
 def say_hi(message):
-    return ('Hi!')
+    return message
 
-@instance.message(alias='return_test')
+@instance.message(alias='return_username')
 def return_test(message, command=None):
     return message.username
 
 # ... (other message handlers)
 
 synochat.run_bot(instance, outgoing_webhook, incomming_webhook_token)
 ```
```

