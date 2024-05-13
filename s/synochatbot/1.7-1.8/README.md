# Comparing `tmp/synochatbot-1.7.tar.gz` & `tmp/synochatbot-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synochatbot-1.7.tar", last modified: Mon May 13 16:20:47 2024, max compression
+gzip compressed data, was "synochatbot-1.8.tar", last modified: Mon May 13 16:22:59 2024, max compression
```

## Comparing `synochatbot-1.7.tar` & `synochatbot-1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 16:20:47.688223 synochatbot-1.7/
--rw-r--r--   0 ct         (502) staff       (20)      865 2024-05-13 16:20:47.688030 synochatbot-1.7/PKG-INFO
--rw-r--r--   0 ct         (502) staff       (20)       38 2024-05-13 16:20:47.688271 synochatbot-1.7/setup.cfg
--rw-r--r--   0 ct         (502) staff       (20)     1014 2024-05-13 16:20:42.000000 synochatbot-1.7/setup.py
-drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 16:20:47.686968 synochatbot-1.7/synochatbot/
--rw-r--r--   0 ct         (502) staff       (20)      573 2024-05-13 04:29:50.000000 synochatbot-1.7/synochatbot/__init__.py
--rw-r--r--   0 ct         (502) staff       (20)     3733 2024-05-13 16:20:26.000000 synochatbot-1.7/synochatbot/bot.py
-drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 16:20:47.687816 synochatbot-1.7/synochatbot.egg-info/
--rw-r--r--   0 ct         (502) staff       (20)      865 2024-05-13 16:20:47.000000 synochatbot-1.7/synochatbot.egg-info/PKG-INFO
--rw-r--r--   0 ct         (502) staff       (20)      225 2024-05-13 16:20:47.000000 synochatbot-1.7/synochatbot.egg-info/SOURCES.txt
--rw-r--r--   0 ct         (502) staff       (20)        1 2024-05-13 16:20:47.000000 synochatbot-1.7/synochatbot.egg-info/dependency_links.txt
--rw-r--r--   0 ct         (502) staff       (20)       30 2024-05-13 16:20:47.000000 synochatbot-1.7/synochatbot.egg-info/requires.txt
--rw-r--r--   0 ct         (502) staff       (20)       12 2024-05-13 16:20:47.000000 synochatbot-1.7/synochatbot.egg-info/top_level.txt
+drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 16:22:59.937395 synochatbot-1.8/
+-rw-r--r--   0 ct         (502) staff       (20)      865 2024-05-13 16:22:59.937173 synochatbot-1.8/PKG-INFO
+-rw-r--r--   0 ct         (502) staff       (20)       38 2024-05-13 16:22:59.937441 synochatbot-1.8/setup.cfg
+-rw-r--r--   0 ct         (502) staff       (20)     1014 2024-05-13 16:22:52.000000 synochatbot-1.8/setup.py
+drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 16:22:59.935913 synochatbot-1.8/synochatbot/
+-rw-r--r--   0 ct         (502) staff       (20)      573 2024-05-13 04:29:50.000000 synochatbot-1.8/synochatbot/__init__.py
+-rw-r--r--   0 ct         (502) staff       (20)     3737 2024-05-13 16:22:21.000000 synochatbot-1.8/synochatbot/bot.py
+drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 16:22:59.936941 synochatbot-1.8/synochatbot.egg-info/
+-rw-r--r--   0 ct         (502) staff       (20)      865 2024-05-13 16:22:59.000000 synochatbot-1.8/synochatbot.egg-info/PKG-INFO
+-rw-r--r--   0 ct         (502) staff       (20)      225 2024-05-13 16:22:59.000000 synochatbot-1.8/synochatbot.egg-info/SOURCES.txt
+-rw-r--r--   0 ct         (502) staff       (20)        1 2024-05-13 16:22:59.000000 synochatbot-1.8/synochatbot.egg-info/dependency_links.txt
+-rw-r--r--   0 ct         (502) staff       (20)       30 2024-05-13 16:22:59.000000 synochatbot-1.8/synochatbot.egg-info/requires.txt
+-rw-r--r--   0 ct         (502) staff       (20)       12 2024-05-13 16:22:59.000000 synochatbot-1.8/synochatbot.egg-info/top_level.txt
```

### Comparing `synochatbot-1.7/PKG-INFO` & `synochatbot-1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synochatbot
-Version: 1.7
+Version: 1.8
 Summary: A discord.py like thing but for synology chat
 Author: kokofixcomputers
 Description-Content-Type: text/markdown
 Requires-Dist: flask==3.0.3
 Requires-Dist: requests==2.31.0
```

### Comparing `synochatbot-1.7/setup.py` & `synochatbot-1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='synochatbot',
-    version='1.7',
+    version='1.8',
     author='kokofixcomputers',
     description='A discord.py like thing but for synology chat',
     long_description_content_type='text/markdown',
     long_description='''
 # A python library like discord.py but for synology chat.
 
 It allows you to create a bot that can be used to respond to messages in synology chat.
```

### Comparing `synochatbot-1.7/synochatbot/__init__.py` & `synochatbot-1.8/synochatbot/__init__.py`

 * *Files identical despite different names*

### Comparing `synochatbot-1.7/synochatbot/bot.py` & `synochatbot-1.8/synochatbot/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,38 +58,38 @@
 
 def process_messages(instance, outgoing_webhook, incoming_webhook_url):
     global incoming_webhook_url1
     incoming_webhook_url1 = incoming_webhook_url
     while True:
         try:
             alias, message, username = message_queue.get(block=True, timeout=1)
-            class Message:
+            class Message1:
                 def __init__(self, content, username):
                     self.content = content
                     self.username = username
     
                 def __str__(self):
                     return self.content
     
-            msg = Message(message, username)
+            msg = Message1(message, username)
             
             # Process the message here
             if alias in instance.alias_to_func:
                 func = instance.alias_to_func[alias]
                 parts = msg.content.split(" ")
                 if len(parts) > 1:
                     arg_str = " ".join(parts[1:])
                     arg_parts = arg_str.split(":::")
                     response = func(msg, *arg_parts)
                     if response:
-                        send_message(Message(response, msg.username), outgoing_webhook)
+                        send_message(Message1(response, msg.username), outgoing_webhook)
                 else:
                     response = func(msg)
                     if response:
-                        send_message(Message(response, msg.username), outgoing_webhook)
+                        send_message(Message1(response, msg.username), outgoing_webhook)
             else:
                 print(f"Unknown alias: {alias}")
         except queue.Empty:
             # No messages in the queue, wait for the next one
             pass
 
 def run_bot(instance, outgoing_webhook, incomming_token):
```

### Comparing `synochatbot-1.7/synochatbot.egg-info/PKG-INFO` & `synochatbot-1.8/synochatbot.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synochatbot
-Version: 1.7
+Version: 1.8
 Summary: A discord.py like thing but for synology chat
 Author: kokofixcomputers
 Description-Content-Type: text/markdown
 Requires-Dist: flask==3.0.3
 Requires-Dist: requests==2.31.0
```

