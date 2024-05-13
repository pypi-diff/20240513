# Comparing `tmp/synochatbot-1.9.tar.gz` & `tmp/synochatbot-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synochatbot-1.9.tar", last modified: Mon May 13 16:27:30 2024, max compression
+gzip compressed data, was "synochatbot-2.0.tar", last modified: Mon May 13 16:30:57 2024, max compression
```

## Comparing `synochatbot-1.9.tar` & `synochatbot-2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 16:27:30.003203 synochatbot-1.9/
--rw-r--r--   0 ct         (502) staff       (20)      865 2024-05-13 16:27:30.002937 synochatbot-1.9/PKG-INFO
--rw-r--r--   0 ct         (502) staff       (20)       38 2024-05-13 16:27:30.003271 synochatbot-1.9/setup.cfg
--rw-r--r--   0 ct         (502) staff       (20)     1014 2024-05-13 16:27:16.000000 synochatbot-1.9/setup.py
-drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 16:27:29.999208 synochatbot-1.9/synochatbot/
--rw-r--r--   0 ct         (502) staff       (20)      573 2024-05-13 04:29:50.000000 synochatbot-1.9/synochatbot/__init__.py
--rw-r--r--   0 ct         (502) staff       (20)     3689 2024-05-13 16:26:31.000000 synochatbot-1.9/synochatbot/bot.py
-drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 16:27:30.002137 synochatbot-1.9/synochatbot.egg-info/
--rw-r--r--   0 ct         (502) staff       (20)      865 2024-05-13 16:27:29.000000 synochatbot-1.9/synochatbot.egg-info/PKG-INFO
--rw-r--r--   0 ct         (502) staff       (20)      225 2024-05-13 16:27:29.000000 synochatbot-1.9/synochatbot.egg-info/SOURCES.txt
--rw-r--r--   0 ct         (502) staff       (20)        1 2024-05-13 16:27:29.000000 synochatbot-1.9/synochatbot.egg-info/dependency_links.txt
--rw-r--r--   0 ct         (502) staff       (20)       30 2024-05-13 16:27:29.000000 synochatbot-1.9/synochatbot.egg-info/requires.txt
--rw-r--r--   0 ct         (502) staff       (20)       12 2024-05-13 16:27:29.000000 synochatbot-1.9/synochatbot.egg-info/top_level.txt
+drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 16:30:57.979387 synochatbot-2.0/
+-rw-r--r--   0 ct         (502) staff       (20)      865 2024-05-13 16:30:57.979154 synochatbot-2.0/PKG-INFO
+-rw-r--r--   0 ct         (502) staff       (20)       38 2024-05-13 16:30:57.979433 synochatbot-2.0/setup.cfg
+-rw-r--r--   0 ct         (502) staff       (20)     1014 2024-05-13 16:30:13.000000 synochatbot-2.0/setup.py
+drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 16:30:57.977939 synochatbot-2.0/synochatbot/
+-rw-r--r--   0 ct         (502) staff       (20)      573 2024-05-13 04:29:50.000000 synochatbot-2.0/synochatbot/__init__.py
+-rw-r--r--   0 ct         (502) staff       (20)     3699 2024-05-13 16:29:29.000000 synochatbot-2.0/synochatbot/bot.py
+drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 16:30:57.978887 synochatbot-2.0/synochatbot.egg-info/
+-rw-r--r--   0 ct         (502) staff       (20)      865 2024-05-13 16:30:57.000000 synochatbot-2.0/synochatbot.egg-info/PKG-INFO
+-rw-r--r--   0 ct         (502) staff       (20)      225 2024-05-13 16:30:57.000000 synochatbot-2.0/synochatbot.egg-info/SOURCES.txt
+-rw-r--r--   0 ct         (502) staff       (20)        1 2024-05-13 16:30:57.000000 synochatbot-2.0/synochatbot.egg-info/dependency_links.txt
+-rw-r--r--   0 ct         (502) staff       (20)       30 2024-05-13 16:30:57.000000 synochatbot-2.0/synochatbot.egg-info/requires.txt
+-rw-r--r--   0 ct         (502) staff       (20)       12 2024-05-13 16:30:57.000000 synochatbot-2.0/synochatbot.egg-info/top_level.txt
```

### Comparing `synochatbot-1.9/PKG-INFO` & `synochatbot-2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synochatbot
-Version: 1.9
+Version: 2.0
 Summary: A discord.py like thing but for synology chat
 Author: kokofixcomputers
 Description-Content-Type: text/markdown
 Requires-Dist: flask==3.0.3
 Requires-Dist: requests==2.31.0
```

### Comparing `synochatbot-1.9/setup.py` & `synochatbot-2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='synochatbot',
-    version='1.9',
+    version='2.0',
     author='kokofixcomputers',
     description='A discord.py like thing but for synology chat',
     long_description_content_type='text/markdown',
     long_description='''
 # A python library like discord.py but for synology chat.
 
 It allows you to create a bot that can be used to respond to messages in synology chat.
```

### Comparing `synochatbot-1.9/synochatbot/__init__.py` & `synochatbot-2.0/synochatbot/__init__.py`

 * *Files identical despite different names*

### Comparing `synochatbot-1.9/synochatbot/bot.py` & `synochatbot-2.0/synochatbot/bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,19 +77,19 @@
                 func = instance.alias_to_func[alias]
                 parts = msg.content.split(" ")
                 if len(parts) > 1:
                     arg_str = " ".join(parts[1:])
                     arg_parts = arg_str.split(":::")
                     response = func(msg, *arg_parts)
                     if response:
-                        send_message(response, outgoing_webhook)
+                        send_message(str(response), outgoing_webhook)
                 else:
                     response = func(msg)
                     if response:
-                        send_message(response, outgoing_webhook)
+                        send_message(str(response), outgoing_webhook)
             else:
                 print(f"Unknown alias: {alias}")
         except queue.Empty:
             # No messages in the queue, wait for the next one
             pass
 
 def run_bot(instance, outgoing_webhook, incomming_token):
```

### Comparing `synochatbot-1.9/synochatbot.egg-info/PKG-INFO` & `synochatbot-2.0/synochatbot.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synochatbot
-Version: 1.9
+Version: 2.0
 Summary: A discord.py like thing but for synology chat
 Author: kokofixcomputers
 Description-Content-Type: text/markdown
 Requires-Dist: flask==3.0.3
 Requires-Dist: requests==2.31.0
```

