# Comparing `tmp/synochatbot-2.1.tar.gz` & `tmp/synochatbot-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synochatbot-2.1.tar", last modified: Mon May 13 16:34:22 2024, max compression
+gzip compressed data, was "synochatbot-2.2.tar", last modified: Mon May 13 17:01:17 2024, max compression
```

## Comparing `synochatbot-2.1.tar` & `synochatbot-2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 16:34:22.025163 synochatbot-2.1/
--rw-r--r--   0 ct         (502) staff       (20)      886 2024-05-13 16:34:22.024613 synochatbot-2.1/PKG-INFO
--rw-r--r--   0 ct         (502) staff       (20)       38 2024-05-13 16:34:22.025222 synochatbot-2.1/setup.cfg
--rw-r--r--   0 ct         (502) staff       (20)     1035 2024-05-13 16:34:07.000000 synochatbot-2.1/setup.py
-drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 16:34:22.023386 synochatbot-2.1/synochatbot/
--rw-r--r--   0 ct         (502) staff       (20)      573 2024-05-13 04:29:50.000000 synochatbot-2.1/synochatbot/__init__.py
--rw-r--r--   0 ct         (502) staff       (20)     3699 2024-05-13 16:29:29.000000 synochatbot-2.1/synochatbot/bot.py
-drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 16:34:22.024365 synochatbot-2.1/synochatbot.egg-info/
--rw-r--r--   0 ct         (502) staff       (20)      886 2024-05-13 16:34:22.000000 synochatbot-2.1/synochatbot.egg-info/PKG-INFO
--rw-r--r--   0 ct         (502) staff       (20)      225 2024-05-13 16:34:22.000000 synochatbot-2.1/synochatbot.egg-info/SOURCES.txt
--rw-r--r--   0 ct         (502) staff       (20)        1 2024-05-13 16:34:22.000000 synochatbot-2.1/synochatbot.egg-info/dependency_links.txt
--rw-r--r--   0 ct         (502) staff       (20)       30 2024-05-13 16:34:22.000000 synochatbot-2.1/synochatbot.egg-info/requires.txt
--rw-r--r--   0 ct         (502) staff       (20)       12 2024-05-13 16:34:22.000000 synochatbot-2.1/synochatbot.egg-info/top_level.txt
+drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 17:01:17.678933 synochatbot-2.2/
+-rw-r--r--   0 ct         (502) staff       (20)      886 2024-05-13 17:01:17.678444 synochatbot-2.2/PKG-INFO
+-rw-r--r--   0 ct         (502) staff       (20)       38 2024-05-13 17:01:17.678999 synochatbot-2.2/setup.cfg
+-rw-r--r--   0 ct         (502) staff       (20)     1035 2024-05-13 17:00:57.000000 synochatbot-2.2/setup.py
+drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 17:01:17.675735 synochatbot-2.2/synochat/
+-rw-r--r--   0 ct         (502) staff       (20)      968 2024-05-13 16:57:00.000000 synochatbot-2.2/synochat/__init__.py
+-rw-r--r--   0 ct         (502) staff       (20)     3707 2024-05-13 16:59:15.000000 synochatbot-2.2/synochat/bot.py
+drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-13 17:01:17.677801 synochatbot-2.2/synochatbot.egg-info/
+-rw-r--r--   0 ct         (502) staff       (20)      886 2024-05-13 17:01:17.000000 synochatbot-2.2/synochatbot.egg-info/PKG-INFO
+-rw-r--r--   0 ct         (502) staff       (20)      219 2024-05-13 17:01:17.000000 synochatbot-2.2/synochatbot.egg-info/SOURCES.txt
+-rw-r--r--   0 ct         (502) staff       (20)        1 2024-05-13 17:01:17.000000 synochatbot-2.2/synochatbot.egg-info/dependency_links.txt
+-rw-r--r--   0 ct         (502) staff       (20)       30 2024-05-13 17:01:17.000000 synochatbot-2.2/synochatbot.egg-info/requires.txt
+-rw-r--r--   0 ct         (502) staff       (20)        9 2024-05-13 17:01:17.000000 synochatbot-2.2/synochatbot.egg-info/top_level.txt
```

### Comparing `synochatbot-2.1/PKG-INFO` & `synochatbot-2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synochatbot
-Version: 2.1
+Version: 2.2
 Summary: A discord.py like thing but for synology chat
 Author: kokofixcomputers
 Description-Content-Type: text/markdown
 Requires-Dist: flask==3.0.3
 Requires-Dist: requests==2.31.0
```

### Comparing `synochatbot-2.1/setup.py` & `synochatbot-2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='synochatbot',
-    version='2.1',
+    version='2.2',
     author='kokofixcomputers',
     description='A discord.py like thing but for synology chat',
     long_description_content_type='text/markdown',
     long_description='''
 # A python library like discord.py but for synology chat.
 
 It allows you to create a bot that can be used to respond to messages in synology chat.
```

### Comparing `synochatbot-2.1/synochatbot/__init__.py` & `synochatbot-2.2/synochat/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,19 +4,31 @@
 import time
 time.sleep(1)
 
 class SynoBot:
     def __init__(self, prefix):
         self.prefix = prefix
         self.alias_to_func = {}
+        self.on_unknown_message1 = False
 
     def message(self, alias, arguments=0):
         def decorator(func):
-            self.alias_to_func[alias] = func
+            self.alias_to_func[alias] = self.prefix + func
             return func
         return decorator
+    
+    def on_unknown_message(self, func):
+        def wrapper(*args, **kwargs):
+            # Code to handle unknown messages goes here
+            print("Unknown message.")
+            self.on_unknown_message1 = True
+        
+            # Call the original function
+            return func(*args, **kwargs)
+    
+        return wrapper
 
     def run(self, **kwargs):
         flask_thread = threading.Thread(target=app.run, kwargs=kwargs)
         flask_thread.start()
 def instance(prefix):
     return SynoBot(prefix)
```

### Comparing `synochatbot-2.1/synochatbot/bot.py` & `synochatbot-2.2/synochat/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,19 +75,19 @@
             # Process the message here
             if alias in instance.alias_to_func:
                 func = instance.alias_to_func[alias]
                 parts = msg.content.split(" ")
                 if len(parts) > 1:
                     arg_str = " ".join(parts[1:])
                     arg_parts = arg_str.split(":::")
-                    response = func(msg, *arg_parts)
+                    response = func(msg[:1], *arg_parts)
                     if response:
                         send_message(str(response), outgoing_webhook)
                 else:
-                    response = func(msg)
+                    response = func(msg[:1])
                     if response:
                         send_message(str(response), outgoing_webhook)
             else:
                 print(f"Unknown alias: {alias}")
         except queue.Empty:
             # No messages in the queue, wait for the next one
             pass
```

### Comparing `synochatbot-2.1/synochatbot.egg-info/PKG-INFO` & `synochatbot-2.2/synochatbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synochatbot
-Version: 2.1
+Version: 2.2
 Summary: A discord.py like thing but for synology chat
 Author: kokofixcomputers
 Description-Content-Type: text/markdown
 Requires-Dist: flask==3.0.3
 Requires-Dist: requests==2.31.0
```

