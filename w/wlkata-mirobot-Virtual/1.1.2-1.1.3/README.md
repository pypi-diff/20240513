# Comparing `tmp/wlkata_mirobot_Virtual-1.1.2.tar.gz` & `tmp/wlkata_mirobot_Virtual-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wlkata_mirobot_Virtual-1.1.2.tar", last modified: Mon May 13 01:09:17 2024, max compression
+gzip compressed data, was "wlkata_mirobot_Virtual-1.1.3.tar", last modified: Mon May 13 02:50:17 2024, max compression
```

## Comparing `wlkata_mirobot_Virtual-1.1.2.tar` & `wlkata_mirobot_Virtual-1.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 01:09:17.901435 wlkata_mirobot_Virtual-1.1.2/
--rw-rw-rw-   0        0        0      110 2024-05-13 01:09:17.899439 wlkata_mirobot_Virtual-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      592 2024-05-11 10:00:37.000000 wlkata_mirobot_Virtual-1.1.2/license.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 01:09:17.901435 wlkata_mirobot_Virtual-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      236 2024-05-13 01:04:28.000000 wlkata_mirobot_Virtual-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 01:09:17.895450 wlkata_mirobot_Virtual-1.1.2/wlkata_mirobot_Virtual/
--rw-rw-rw-   0        0        0       83 2024-05-12 02:38:37.000000 wlkata_mirobot_Virtual-1.1.2/wlkata_mirobot_Virtual/__init__.py
--rw-rw-rw-   0        0        0    15615 2024-05-13 01:08:43.000000 wlkata_mirobot_Virtual-1.1.2/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py
-drwxrwxrwx   0        0        0        0 2024-05-13 01:09:17.899439 wlkata_mirobot_Virtual-1.1.2/wlkata_mirobot_Virtual.egg-info/
--rw-rw-rw-   0        0        0      110 2024-05-13 01:09:17.000000 wlkata_mirobot_Virtual-1.1.2/wlkata_mirobot_Virtual.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2024-05-13 01:09:17.000000 wlkata_mirobot_Virtual-1.1.2/wlkata_mirobot_Virtual.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 01:09:17.000000 wlkata_mirobot_Virtual-1.1.2/wlkata_mirobot_Virtual.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-05-13 01:09:17.000000 wlkata_mirobot_Virtual-1.1.2/wlkata_mirobot_Virtual.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 02:50:17.183944 wlkata_mirobot_Virtual-1.1.3/
+-rw-rw-rw-   0        0        0      110 2024-05-13 02:50:17.182947 wlkata_mirobot_Virtual-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      592 2024-05-11 10:00:37.000000 wlkata_mirobot_Virtual-1.1.3/license.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 02:50:17.183944 wlkata_mirobot_Virtual-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      236 2024-05-13 02:50:01.000000 wlkata_mirobot_Virtual-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 02:50:17.177960 wlkata_mirobot_Virtual-1.1.3/wlkata_mirobot_Virtual/
+-rw-rw-rw-   0        0        0       83 2024-05-12 02:38:37.000000 wlkata_mirobot_Virtual-1.1.3/wlkata_mirobot_Virtual/__init__.py
+-rw-rw-rw-   0        0        0    15649 2024-05-13 02:49:27.000000 wlkata_mirobot_Virtual-1.1.3/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py
+drwxrwxrwx   0        0        0        0 2024-05-13 02:50:17.182947 wlkata_mirobot_Virtual-1.1.3/wlkata_mirobot_Virtual.egg-info/
+-rw-rw-rw-   0        0        0      110 2024-05-13 02:50:17.000000 wlkata_mirobot_Virtual-1.1.3/wlkata_mirobot_Virtual.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2024-05-13 02:50:17.000000 wlkata_mirobot_Virtual-1.1.3/wlkata_mirobot_Virtual.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 02:50:17.000000 wlkata_mirobot_Virtual-1.1.3/wlkata_mirobot_Virtual.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-13 02:50:17.000000 wlkata_mirobot_Virtual-1.1.3/wlkata_mirobot_Virtual.egg-info/top_level.txt
```

### Comparing `wlkata_mirobot_Virtual-1.1.2/license.txt` & `wlkata_mirobot_Virtual-1.1.3/license.txt`

 * *Files identical despite different names*

### Comparing `wlkata_mirobot_Virtual-1.1.2/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py` & `wlkata_mirobot_Virtual-1.1.3/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
     def __init__(self,server_IP='', server_port=None):
         
         self.server_IP = server_IP  
         self.server_port = server_port
         self.invalid_IP_Port_Connect()
         self.status_state = None
+        self.status_state2 = None
         self.robot_type = 1
         self.global_state = [1,1,1]
         self.IO = [0,0,0,0,0,0,0,0]
         self.default_speed = 1000
         ### 第七轴/滑轨
         self.angles_7 = 0
```

