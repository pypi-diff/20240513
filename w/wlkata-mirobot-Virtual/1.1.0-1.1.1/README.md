# Comparing `tmp/wlkata_mirobot_Virtual-1.1.0.tar.gz` & `tmp/wlkata_mirobot_Virtual-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wlkata_mirobot_Virtual-1.1.0.tar", last modified: Sun May 12 07:16:54 2024, max compression
+gzip compressed data, was "wlkata_mirobot_Virtual-1.1.1.tar", last modified: Sun May 12 09:34:49 2024, max compression
```

## Comparing `wlkata_mirobot_Virtual-1.1.0.tar` & `wlkata_mirobot_Virtual-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 07:16:54.628884 wlkata_mirobot_Virtual-1.1.0/
--rw-rw-rw-   0        0        0      110 2024-05-12 07:16:54.627886 wlkata_mirobot_Virtual-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      592 2024-05-11 10:00:37.000000 wlkata_mirobot_Virtual-1.1.0/license.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 07:16:54.628884 wlkata_mirobot_Virtual-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      236 2024-05-12 07:16:24.000000 wlkata_mirobot_Virtual-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 07:16:54.622900 wlkata_mirobot_Virtual-1.1.0/wlkata_mirobot_Virtual/
--rw-rw-rw-   0        0        0       83 2024-05-12 02:38:37.000000 wlkata_mirobot_Virtual-1.1.0/wlkata_mirobot_Virtual/__init__.py
--rw-rw-rw-   0        0        0    15587 2024-05-12 05:43:43.000000 wlkata_mirobot_Virtual-1.1.0/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py
-drwxrwxrwx   0        0        0        0 2024-05-12 07:16:54.626889 wlkata_mirobot_Virtual-1.1.0/wlkata_mirobot_Virtual.egg-info/
--rw-rw-rw-   0        0        0      110 2024-05-12 07:16:54.000000 wlkata_mirobot_Virtual-1.1.0/wlkata_mirobot_Virtual.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2024-05-12 07:16:54.000000 wlkata_mirobot_Virtual-1.1.0/wlkata_mirobot_Virtual.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 07:16:54.000000 wlkata_mirobot_Virtual-1.1.0/wlkata_mirobot_Virtual.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-05-12 07:16:54.000000 wlkata_mirobot_Virtual-1.1.0/wlkata_mirobot_Virtual.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 09:34:49.053572 wlkata_mirobot_Virtual-1.1.1/
+-rw-rw-rw-   0        0        0      110 2024-05-12 09:34:49.051577 wlkata_mirobot_Virtual-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      592 2024-05-11 10:00:37.000000 wlkata_mirobot_Virtual-1.1.1/license.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 09:34:49.053572 wlkata_mirobot_Virtual-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      236 2024-05-12 09:34:36.000000 wlkata_mirobot_Virtual-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 09:34:49.047588 wlkata_mirobot_Virtual-1.1.1/wlkata_mirobot_Virtual/
+-rw-rw-rw-   0        0        0       83 2024-05-12 02:38:37.000000 wlkata_mirobot_Virtual-1.1.1/wlkata_mirobot_Virtual/__init__.py
+-rw-rw-rw-   0        0        0    15592 2024-05-12 09:34:01.000000 wlkata_mirobot_Virtual-1.1.1/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py
+drwxrwxrwx   0        0        0        0 2024-05-12 09:34:49.051577 wlkata_mirobot_Virtual-1.1.1/wlkata_mirobot_Virtual.egg-info/
+-rw-rw-rw-   0        0        0      110 2024-05-12 09:34:48.000000 wlkata_mirobot_Virtual-1.1.1/wlkata_mirobot_Virtual.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2024-05-12 09:34:48.000000 wlkata_mirobot_Virtual-1.1.1/wlkata_mirobot_Virtual.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 09:34:48.000000 wlkata_mirobot_Virtual-1.1.1/wlkata_mirobot_Virtual.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-12 09:34:48.000000 wlkata_mirobot_Virtual-1.1.1/wlkata_mirobot_Virtual.egg-info/top_level.txt
```

### Comparing `wlkata_mirobot_Virtual-1.1.0/license.txt` & `wlkata_mirobot_Virtual-1.1.1/license.txt`

 * *Files identical despite different names*

### Comparing `wlkata_mirobot_Virtual-1.1.0/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py` & `wlkata_mirobot_Virtual-1.1.1/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         try:
             value = float(text)
             if value < -100 or value > 160:
                 print ("Value out of range")
         except ValueError:
             print()
 
-    def send_msg(self,com1_data, com2_data = None, wait_idle=False):
+    def send_msg(self,com1_data=None, com2_data = None, wait_idle=False):
         robot_type = self.robot_type
         state = self.global_state
         com1 = com1_data
         com2 = com2_data ### if com2_data is not None else com1_data
         rs485 = ""
         com1Float = self.angles_6 
         com2Float = self.angles_6
```

