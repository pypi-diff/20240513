# Comparing `tmp/rlmarlbot_plugin-0.1.2.tar.gz` & `tmp/rlmarlbot_plugin-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlmarlbot_plugin-0.1.2.tar", max compression
+gzip compressed data, was "rlmarlbot_plugin-0.1.3.tar", max compression
```

## Comparing `rlmarlbot_plugin-0.1.2.tar` & `rlmarlbot_plugin-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      334 2024-05-13 00:47:33.740665 rlmarlbot_plugin-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-13 00:20:02.783433 rlmarlbot_plugin-0.1.2/README.md
--rw-r--r--   0        0        0       51 2024-05-13 00:47:16.864668 rlmarlbot_plugin-0.1.2/rlmarlbot_plugin/__init__.py
--rw-r--r--   0        0        0     1129 2024-05-13 00:26:48.171097 rlmarlbot_plugin-0.1.2/rlmarlbot_plugin/base_plugin.py
--rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 rlmarlbot_plugin-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      334 2024-05-13 00:51:45.777539 rlmarlbot_plugin-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-13 00:20:02.783433 rlmarlbot_plugin-0.1.3/README.md
+-rw-r--r--   0        0        0       51 2024-05-13 00:47:16.864668 rlmarlbot_plugin-0.1.3/rlmarlbot_plugin/__init__.py
+-rw-r--r--   0        0        0      997 2024-05-13 00:52:31.806218 rlmarlbot_plugin-0.1.3/rlmarlbot_plugin/base_plugin.py
+-rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 rlmarlbot_plugin-0.1.3/PKG-INFO
```

### Comparing `rlmarlbot_plugin-0.1.2/rlmarlbot_plugin/base_plugin.py` & `rlmarlbot_plugin-0.1.3/rlmarlbot_plugin/base_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from rlsdk_python import RLSDK, EventTypes
 from rlbot.utils.logging_utils import get_logger
 from rlbot.agents.base_agent import SimpleControllerState
 from rlbot.utils.structures.game_data_struct import GameTickPacket
 
 class BasePlugin:
     
-    def __init__(self) {
+    def __init__(self):
         self.name = "BasePlugin"
         self.version = "1.0"
         self.author = "John Doe"
         self.description = "This is a base plugin"
-    }
-
 
     def get_name(self):
         return self.name
     
 
     def get_version(self):
         return self.version
@@ -25,19 +23,17 @@
         return self.author
     
 
     def get_description(self):
         return self.description
     
 
-    def init(self, sdk: RLSDK, config, logger):
-        
-       # Do your init stuff here, like subscribing to events
-
-       logger("Plugin " + self.name + " initialized") # [BASEPLUGIN] Plugin BasePlugin initialized
+    def init(self, sdk: RLSDK):
+        print("Plugin " + self.name + " initialized")
+       pass
        
        
     def override_output(self, output: SimpleControllerState, packet: GameTickPacket):
         
         # in this method you can override the output of the bot
         
         return output
```

