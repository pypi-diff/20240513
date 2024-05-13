# Comparing `tmp/dreamhack-1.1.2.tar.gz` & `tmp/dreamhack-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamhack-1.1.2.tar", last modified: Mon May 13 16:34:40 2024, max compression
+gzip compressed data, was "dreamhack-1.1.3.tar", last modified: Mon May 13 18:28:00 2024, max compression
```

## Comparing `dreamhack-1.1.2.tar` & `dreamhack-1.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 16:34:40.654082 dreamhack-1.1.2/
--rw-r--r--   0 runner    (1000) runner    (1000)     2352 2024-05-13 16:34:40.654082 dreamhack-1.1.2/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 16:34:40.646081 dreamhack-1.1.2/dreamhack/
--rw-r--r--   0 runner    (1000) runner    (1000)     1935 2024-05-13 16:15:37.000000 dreamhack-1.1.2/dreamhack/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      916 2024-05-10 15:50:24.000000 dreamhack-1.1.2/dreamhack/colorcodes.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1153 2024-05-11 23:10:11.000000 dreamhack-1.1.2/dreamhack/downloads.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2502 2024-05-10 15:02:31.000000 dreamhack-1.1.2/dreamhack/encryption.py
--rw-r--r--   0 runner    (1000) runner    (1000)      565 2024-05-13 15:44:44.000000 dreamhack-1.1.2/dreamhack/filepaths.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3819 2024-05-11 23:29:59.000000 dreamhack-1.1.2/dreamhack/gui.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1488 2024-05-10 15:51:14.000000 dreamhack-1.1.2/dreamhack/logging.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1541 2024-05-10 15:51:32.000000 dreamhack-1.1.2/dreamhack/networking.py
--rw-r--r--   0 runner    (1000) runner    (1000)      629 2024-05-10 15:51:48.000000 dreamhack-1.1.2/dreamhack/randoms.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4951 2024-05-13 13:39:48.000000 dreamhack-1.1.2/dreamhack/registry.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6641 2024-05-13 15:46:58.000000 dreamhack-1.1.2/dreamhack/windows.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1637 2024-05-10 15:53:29.000000 dreamhack-1.1.2/dreamhack/zipfiles.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 16:34:40.650082 dreamhack-1.1.2/dreamhack.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2352 2024-05-13 16:34:40.000000 dreamhack-1.1.2/dreamhack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      436 2024-05-13 16:34:40.000000 dreamhack-1.1.2/dreamhack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-13 16:34:40.000000 dreamhack-1.1.2/dreamhack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      123 2024-05-13 16:34:40.000000 dreamhack-1.1.2/dreamhack.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-05-13 16:34:40.000000 dreamhack-1.1.2/dreamhack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-13 16:34:40.654082 dreamhack-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     2611 2024-05-13 16:34:07.000000 dreamhack-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 18:28:00.944208 dreamhack-1.1.3/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2440 2024-05-13 18:28:00.940208 dreamhack-1.1.3/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 18:28:00.940208 dreamhack-1.1.3/dreamhack/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1987 2024-05-13 18:24:54.000000 dreamhack-1.1.3/dreamhack/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      916 2024-05-10 15:50:24.000000 dreamhack-1.1.3/dreamhack/colorcodes.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1153 2024-05-11 23:10:11.000000 dreamhack-1.1.3/dreamhack/downloads.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2502 2024-05-10 15:02:31.000000 dreamhack-1.1.3/dreamhack/encryption.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      565 2024-05-13 15:44:44.000000 dreamhack-1.1.3/dreamhack/filepaths.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3819 2024-05-11 23:29:59.000000 dreamhack-1.1.3/dreamhack/gui.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1488 2024-05-10 15:51:14.000000 dreamhack-1.1.3/dreamhack/logging.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1541 2024-05-10 15:51:32.000000 dreamhack-1.1.3/dreamhack/networking.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      629 2024-05-10 15:51:48.000000 dreamhack-1.1.3/dreamhack/randoms.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5726 2024-05-13 18:26:44.000000 dreamhack-1.1.3/dreamhack/registry.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7184 2024-05-13 18:10:13.000000 dreamhack-1.1.3/dreamhack/windows.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1637 2024-05-10 15:53:29.000000 dreamhack-1.1.3/dreamhack/zipfiles.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 18:28:00.940208 dreamhack-1.1.3/dreamhack.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2440 2024-05-13 18:28:00.000000 dreamhack-1.1.3/dreamhack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      436 2024-05-13 18:28:00.000000 dreamhack-1.1.3/dreamhack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-13 18:28:00.000000 dreamhack-1.1.3/dreamhack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      123 2024-05-13 18:28:00.000000 dreamhack-1.1.3/dreamhack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-05-13 18:28:00.000000 dreamhack-1.1.3/dreamhack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-13 18:28:00.944208 dreamhack-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     2702 2024-05-13 18:27:50.000000 dreamhack-1.1.3/setup.py
```

### Comparing `dreamhack-1.1.2/PKG-INFO` & `dreamhack-1.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamhack
-Version: 1.1.2
+Version: 1.1.3
 Summary: The ultimate PyPi package for cyber-security and many other things.
 Author: Jack Burr
 Author-email: BurrJ22@Outlook.com
 Keywords: python,windows,encryption
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: cryptography
@@ -22,14 +22,21 @@
 
 The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
 *DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any malicious purposes. 
 
 RELEASE NOTES: 
 
+v1.1.3: 
+
+- Added new error detection to registry class 
+
+- Added a few new features 
+
+
 v1.1.2: 
 
 - Added a few new features 
 
 - Fixed some new bugs 
 
 - Added new classes
```

### Comparing `dreamhack-1.1.2/dreamhack/__init__.py` & `dreamhack-1.1.3/dreamhack/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .gui import gui
 from .windows import ctypesMessageBoxIcons
 from .windows import computer_stats
 from .registry import RegistryEditor
 from .registry import disable_regedit
 from .registry import lock_all_drives
 from .registry import disable_task_manager
+from .registry import convert_registry_path_to_list
 from .registry import add_to_windows_startup
 
 #type:ignore
 
 import os
 import sys
 import subprocess
```

### Comparing `dreamhack-1.1.2/dreamhack/colorcodes.py` & `dreamhack-1.1.3/dreamhack/colorcodes.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.2/dreamhack/downloads.py` & `dreamhack-1.1.3/dreamhack/downloads.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.2/dreamhack/encryption.py` & `dreamhack-1.1.3/dreamhack/encryption.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.2/dreamhack/filepaths.py` & `dreamhack-1.1.3/dreamhack/filepaths.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.2/dreamhack/gui.py` & `dreamhack-1.1.3/dreamhack/gui.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.2/dreamhack/logging.py` & `dreamhack-1.1.3/dreamhack/logging.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.2/dreamhack/networking.py` & `dreamhack-1.1.3/dreamhack/networking.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.2/dreamhack/randoms.py` & `dreamhack-1.1.3/dreamhack/randoms.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.2/dreamhack/registry.py` & `dreamhack-1.1.3/dreamhack/registry.py`

 * *Files 10% similar despite different names*

```diff
@@ -140,8 +140,39 @@
   RUNKEYS = ["SOFTWARE", "Microsoft", "Windows", "CurrentVersion", "Run"]
   path01 = RegistryEditor.RegistryPath(HKCU, RUNKEYS)
   path01.build()
   path02 = RegistryEditor.RegistryPath(HKLM, RUNKEYS)
   RegistryEditor.set(path01, name, str(path))
   RegistryEditor.set(path02, name, str(path))
 
+@staticmethod
+def convert_registry_path_to_list(path):
+  def split(string, character):
+    try:
+      return string.split(character)
+    except Exception:
+      return -1
+
+  SPLIT = ['0','1','2']
+  path = str(path)
+  split_1 = split(path, r"\\")
+  split_2 = split(path, "/")
+  split_3 = split(path, "//")
+  if split_1 == -1 and split_2 == -1:
+    SPLIT = split_3
+  elif split_2 == -1 and split_3 == -1:
+    SPLIT = split_1 #type:ignore
+  elif split_3 != -1 and split_1 == -1:
+    SPLIT = split_2 #type:ignore
+  else:
+    raise Exception("Invalid registry path.")
+  if type(SPLIT) == list: #type:ignore
+    if "HKEY" in SPLIT[0]:
+      return SPLIT.pop(0) 
+    else:
+      raise Exception("Invalid registry path.")
+  else:
+    raise Exception("Invalid registry path.")
+
+  
+
```

### Comparing `dreamhack-1.1.2/dreamhack/windows.py` & `dreamhack-1.1.3/dreamhack/windows.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 class windows():
+  @staticmethod
+  def is_windows():
+    import platform
+    return platform.platform() == 'Windows'
 
   @staticmethod
   def run_as_admin():
     import pyuac
     if not pyuac.isUserAdmin():
       pyuac.runAsAdmin()
 
@@ -14,25 +18,29 @@
     except Exception as e:
       return -1, e
     else:
       return 1, on
 
   @staticmethod
   def block_keyboard_key(key): #type:ignore
+    if not windows.is_windows():
+      return
     import keyboard #type:ignore
     try:
       keyboard.block_key(key) #type:ignore
     except Exception:
       raise Exception('Invalid Keyboard Key.') #type:ignore
     else:
       return key
 
   
   @staticmethod
   def unblock_keyboard_key(key): #type:ignore
+    if not windows.is_windows():
+      return
     import keyboard #type:ignore
     try:
       keyboard.unblock_key(key) #type:ignore
     except Exception:
       raise Exception('Invalid Keyboard Key.') #type:ignore
     else:
       return key
@@ -48,20 +56,27 @@
     keys_list = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789!@#"
     for key in keys_list:
       windows.unblock_keyboard_key(key) #type:ignore
 
   @staticmethod
   def shutdown(timeout_seconds): #type:ignore
     import os
-    try:
-      timeout = int(timeout_seconds) #type:ignore
-    except Exception as e:
-      raise e
+    import time
+    if not windows.is_windows():
+      if timeout_seconds == 0:
+        os.system('shutdown -h now')
+        os.system('sudo shutdown -h now')
+        return
+      time.sleep(timeout_seconds)
+      os.system('shutdown -h now')
+      os.system('sudo shutdown -h now')
+      return
     else:
-      os.system(f'shutdown /s /f /t {timeout_seconds}')
+      time.sleep(timeout_seconds)
+      os.system('shutdown /s /f /t 0')
 
   @staticmethod
   def get_windows_user_directory(): #type:ignore
     import os
     return os.path.expanduser('~')
 
   @staticmethod
@@ -76,14 +91,16 @@
   @staticmethod
   def get_documents_path(): #type:ignore
     return windows.get_folder_in_user_dir('Documents') #type:ignore
 
   @staticmethod
   def create_windows_account(username, password): #type:ignore
     import subprocess
+    if not windows.is_windows():
+      return
     command = f"net user {username} {password} /add /Y"
     try:
       subprocess.run(command, shell=False, check=True)
     except Exception as e: 
       raise e
     else:
       return username, password
@@ -147,14 +164,16 @@
       result = ctypes.windll.user32.MessageBoxA(0, text, title, box_type | icon | icons.TOPMOST) #type:ignore
     else:
       result = ctypes.windll.user32.MessageBoxA(0, text, title, box_type | icon) #type:ignore
     return result
 
   @staticmethod
   def set_windows_desktop_wallpaper(wallpaper_path):
+    if not windows.is_windows():
+      return
     import ctypes
     import os
     SPI_SETDESKWALLPAPER = 20
     SPI_SETDESKWALLPAPER_W = 20
     # Path to the wallpaper image
     wallpaper_path = os.path.realpath(wallpaper_path)
     if os.path.exists(wallpaper_path):
@@ -191,14 +210,16 @@
     #type:ignore
     if platform.platform() != 'Windows':
       return
     subprocess.check_call(['cmd', '/c', f'"{command}"'])
 
   @staticmethod
   def create_appdata_folder(path):
+    if not windows.is_windows():
+      return
     import os
     from .windows import windows
     #type:ignore
     path = os.path.join(windows.get_folder_in_user_dir('AppData'), path)
     try:
       os.makedirs(path)
     except Exception:
```

### Comparing `dreamhack-1.1.2/dreamhack/zipfiles.py` & `dreamhack-1.1.3/dreamhack/zipfiles.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.2/dreamhack.egg-info/PKG-INFO` & `dreamhack-1.1.3/dreamhack.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamhack
-Version: 1.1.2
+Version: 1.1.3
 Summary: The ultimate PyPi package for cyber-security and many other things.
 Author: Jack Burr
 Author-email: BurrJ22@Outlook.com
 Keywords: python,windows,encryption
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: cryptography
@@ -22,14 +22,21 @@
 
 The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
 *DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any malicious purposes. 
 
 RELEASE NOTES: 
 
+v1.1.3: 
+
+- Added new error detection to registry class 
+
+- Added a few new features 
+
+
 v1.1.2: 
 
 - Added a few new features 
 
 - Fixed some new bugs 
 
 - Added new classes
```

### Comparing `dreamhack-1.1.2/setup.py` & `dreamhack-1.1.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from setuptools import setup, find_packages
 #type:ignore
 
-VERSION = '1.1.2' 
+VERSION = '1.1.3' 
 DESCRIPTION = 'The ultimate PyPi package for cyber-security and many other things.'
 LONG_DESCRIPTION = '''The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
 *DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any malicious purposes. 
 
 RELEASE NOTES: \n
+v1.1.3: \n
+- Added new error detection to registry class \n
+- Added a few new features \n
+
 v1.1.2: \n
 - Added a few new features \n
 - Fixed some new bugs \n
 - Added new classes \n
 
 v1.1.1: \n
 - This version had to be deleted because of an error with pypiwin32. \n
```

