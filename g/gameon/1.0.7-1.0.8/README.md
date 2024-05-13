# Comparing `tmp/gameon-1.0.7.tar.gz` & `tmp/gameon-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameon-1.0.7.tar", last modified: Thu May  2 19:52:08 2024, max compression
+gzip compressed data, was "gameon-1.0.8.tar", last modified: Mon May 13 13:49:03 2024, max compression
```

## Comparing `gameon-1.0.7.tar` & `gameon-1.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 19:52:08.959020 gameon-1.0.7/
--rw-rw-rw-   0        0        0      628 2024-05-02 19:51:48.000000 gameon-1.0.7/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1060 2022-07-06 14:58:58.000000 gameon-1.0.7/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2022-07-06 14:59:00.000000 gameon-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      262 2024-05-02 19:52:08.959020 gameon-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      172 2022-07-06 14:47:52.000000 gameon-1.0.7/README.txt
-drwxrwxrwx   0        0        0        0 2024-05-02 19:52:08.944713 gameon-1.0.7/gameon/
--rw-rw-rw-   0        0        0    19268 2024-05-02 19:50:50.000000 gameon-1.0.7/gameon/__init__.py
--rw-rw-rw-   0        0        0    11661 2024-04-25 10:58:03.000000 gameon-1.0.7/gameon/icon.ico
-drwxrwxrwx   0        0        0        0 2024-05-02 19:52:08.957775 gameon-1.0.7/gameon.egg-info/
--rw-rw-rw-   0        0        0      262 2024-05-02 19:52:08.000000 gameon-1.0.7/gameon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2024-05-02 19:52:08.000000 gameon-1.0.7/gameon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 19:52:08.000000 gameon-1.0.7/gameon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-05-02 19:52:08.000000 gameon-1.0.7/gameon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-02 19:52:08.000000 gameon-1.0.7/gameon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 19:52:08.959020 gameon-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      396 2024-05-02 19:51:57.000000 gameon-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 13:49:03.654429 gameon-1.0.8/
+-rw-rw-rw-   0        0        0      683 2024-05-13 13:48:41.000000 gameon-1.0.8/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1060 2022-07-06 14:58:58.000000 gameon-1.0.8/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2022-07-06 14:59:00.000000 gameon-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      262 2024-05-13 13:49:03.653427 gameon-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2022-07-06 14:47:52.000000 gameon-1.0.8/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 13:49:03.642054 gameon-1.0.8/gameon/
+-rw-rw-rw-   0        0        0    19206 2024-05-13 13:47:54.000000 gameon-1.0.8/gameon/__init__.py
+-rw-rw-rw-   0        0        0    11661 2024-04-25 10:58:03.000000 gameon-1.0.8/gameon/icon.ico
+drwxrwxrwx   0        0        0        0 2024-05-13 13:49:03.652061 gameon-1.0.8/gameon.egg-info/
+-rw-rw-rw-   0        0        0      262 2024-05-13 13:49:03.000000 gameon-1.0.8/gameon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2024-05-13 13:49:03.000000 gameon-1.0.8/gameon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 13:49:03.000000 gameon-1.0.8/gameon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-13 13:49:03.000000 gameon-1.0.8/gameon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-13 13:49:03.000000 gameon-1.0.8/gameon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 13:49:03.654429 gameon-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      396 2024-05-13 13:48:48.000000 gameon-1.0.8/setup.py
```

### Comparing `gameon-1.0.7/CHANGELOG.txt` & `gameon-1.0.8/CHANGELOG.txt`

 * *Files 9% similar despite different names*

```diff
@@ -27,8 +27,12 @@
 
 1.0.6 (4/27/2024)
 -------------------
 - Fixed icon not loading causing issues again x2
 
 1.0.7 (5/02/2024)
 -------------------
-- Added load() function to load images
+- Added load() function to load images
+
+1.0.8 (5/13/2024)
+-------------------
+- Bug fixes
```

### Comparing `gameon-1.0.7/LICENCE.txt` & `gameon-1.0.8/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `gameon-1.0.7/gameon/__init__.py` & `gameon-1.0.8/gameon/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,61 +125,65 @@
     pygame.display.flip()
     pass
 
 def delay(time):
     pygame.time.delay(time)
     pass
 
-class timer:
-    def __init__(self, seconds, countdown=False, integer=True):
+import time as t
+
+class Timer:
+    def __init__(self, seconds, countdown=False):
         self.sec = seconds
         self.start_time = None
         self.run_timer = True
         self.timer = 0
         self.start_timer = True
         self.countdown = countdown
-        self.integer = integer
-    def start(self):
+        self.run_once = True
+    def start(self, seconds='default'):
+        if self.run_once:
+            if seconds != 'default':
+                self.sec = seconds
+            self.run_once = False
         if self.start_timer:
             self.start_time = t.time()
             self.start_timer = False
         self.current_time = t.time()
         if self.run_timer:
             if self.start_time != None:
                 if not self.countdown:
-                    if not self.integer:
-                        self.timer = self.current_time - self.start_time
-                    else:
-                        self.timer = int(self.current_time - self.start_time)
+                    self.timer = self.current_time - self.start_time
                 else:    
-                    if not self.integer:
-                        self.timer = self.sec - (self.current_time - self.start_time)
-                    else:
-                        self.timer = int(self.sec - (self.current_time - self.start_time))
+                    self.timer = self.sec - (self.current_time - self.start_time)
+
         if not self.countdown:
             if self.timer >= self.sec:
                 self.run_timer = False
                 self.timer = self.sec
         else:
             if self.timer <= 0:
                 self.run_timer = False
                 self.timer = 0
     def stop(self):
         self.run_timer = False
         pass
-    def restart(self,seconds='default'):
+    def restart(self, seconds='default'):
         self.new_time = seconds
         self.start_time = None
         self.run_timer = True
         if self.new_time != 'default':
             self.sec = self.new_time
         self.start_timer = True
         pass
-    def time(self):
-        return self.timer
+    def time(self, integer=True):
+        if integer:
+            return int(self.timer)
+        else:
+            return self.timer   
         pass
     def __bool__(self):
         if not self.countdown:
             if self.timer != self.sec:
                 return False
             else:
                 return True
```

### Comparing `gameon-1.0.7/gameon/icon.ico` & `gameon-1.0.8/gameon/icon.ico`

 * *Files identical despite different names*

