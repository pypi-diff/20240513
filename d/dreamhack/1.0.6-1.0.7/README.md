# Comparing `tmp/dreamhack-1.0.6.tar.gz` & `tmp/dreamhack-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamhack-1.0.6.tar", last modified: Sat May 11 23:33:48 2024, max compression
+gzip compressed data, was "dreamhack-1.0.7.tar", last modified: Sun May 12 21:50:41 2024, max compression
```

## Comparing `dreamhack-1.0.6.tar` & `dreamhack-1.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-11 23:33:48.058742 dreamhack-1.0.6/
--rw-r--r--   0 runner    (1000) runner    (1000)     1733 2024-05-11 23:33:48.058742 dreamhack-1.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-11 23:33:48.058742 dreamhack-1.0.6/dreamhack/
--rw-r--r--   0 runner    (1000) runner    (1000)      843 2024-05-10 16:58:55.000000 dreamhack-1.0.6/dreamhack/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      916 2024-05-10 15:50:24.000000 dreamhack-1.0.6/dreamhack/colorcodes.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1153 2024-05-11 23:10:11.000000 dreamhack-1.0.6/dreamhack/downloads.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2502 2024-05-10 15:02:31.000000 dreamhack-1.0.6/dreamhack/encryption.py
--rw-r--r--   0 runner    (1000) runner    (1000)      385 2024-05-10 15:50:41.000000 dreamhack-1.0.6/dreamhack/filepaths.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3819 2024-05-11 23:29:59.000000 dreamhack-1.0.6/dreamhack/gui.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1488 2024-05-10 15:51:14.000000 dreamhack-1.0.6/dreamhack/logging.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1541 2024-05-10 15:51:32.000000 dreamhack-1.0.6/dreamhack/networking.py
--rw-r--r--   0 runner    (1000) runner    (1000)      629 2024-05-10 15:51:48.000000 dreamhack-1.0.6/dreamhack/randoms.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2481 2024-05-11 23:31:49.000000 dreamhack-1.0.6/dreamhack/registry.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3741 2024-05-10 15:52:40.000000 dreamhack-1.0.6/dreamhack/windows.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1637 2024-05-10 15:53:29.000000 dreamhack-1.0.6/dreamhack/zipfiles.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-11 23:33:48.058742 dreamhack-1.0.6/dreamhack.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1733 2024-05-11 23:33:47.000000 dreamhack-1.0.6/dreamhack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      436 2024-05-11 23:33:47.000000 dreamhack-1.0.6/dreamhack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-11 23:33:47.000000 dreamhack-1.0.6/dreamhack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      109 2024-05-11 23:33:47.000000 dreamhack-1.0.6/dreamhack.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-05-11 23:33:47.000000 dreamhack-1.0.6/dreamhack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-11 23:33:48.058742 dreamhack-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     1959 2024-05-11 23:33:11.000000 dreamhack-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-12 21:50:41.871703 dreamhack-1.0.7/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1859 2024-05-12 21:50:41.871703 dreamhack-1.0.7/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-12 21:50:41.867704 dreamhack-1.0.7/dreamhack/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1130 2024-05-12 21:49:00.000000 dreamhack-1.0.7/dreamhack/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      916 2024-05-10 15:50:24.000000 dreamhack-1.0.7/dreamhack/colorcodes.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1153 2024-05-11 23:10:11.000000 dreamhack-1.0.7/dreamhack/downloads.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2502 2024-05-10 15:02:31.000000 dreamhack-1.0.7/dreamhack/encryption.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      385 2024-05-10 15:50:41.000000 dreamhack-1.0.7/dreamhack/filepaths.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3819 2024-05-11 23:29:59.000000 dreamhack-1.0.7/dreamhack/gui.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1488 2024-05-10 15:51:14.000000 dreamhack-1.0.7/dreamhack/logging.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1541 2024-05-10 15:51:32.000000 dreamhack-1.0.7/dreamhack/networking.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      629 2024-05-10 15:51:48.000000 dreamhack-1.0.7/dreamhack/randoms.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4884 2024-05-12 21:30:05.000000 dreamhack-1.0.7/dreamhack/registry.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5052 2024-05-12 21:45:39.000000 dreamhack-1.0.7/dreamhack/windows.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1637 2024-05-10 15:53:29.000000 dreamhack-1.0.7/dreamhack/zipfiles.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-12 21:50:41.871703 dreamhack-1.0.7/dreamhack.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1859 2024-05-12 21:50:41.000000 dreamhack-1.0.7/dreamhack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      436 2024-05-12 21:50:41.000000 dreamhack-1.0.7/dreamhack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-12 21:50:41.000000 dreamhack-1.0.7/dreamhack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      109 2024-05-12 21:50:41.000000 dreamhack-1.0.7/dreamhack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-05-12 21:50:41.000000 dreamhack-1.0.7/dreamhack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-12 21:50:41.875703 dreamhack-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     2082 2024-05-12 21:50:37.000000 dreamhack-1.0.7/setup.py
```

### Comparing `dreamhack-1.0.6/PKG-INFO` & `dreamhack-1.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamhack
-Version: 1.0.6
+Version: 1.0.7
 Summary: The ultimate PyPi package for cyber-security and many other things.
 Author: Jack Burr
 Author-email: BurrJ22@Outlook.com
 Keywords: python,windows,encryption
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: cryptography
@@ -19,15 +19,23 @@
 Requires-Dist: CTkMessagebox
 Requires-Dist: unixreg
 
 The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
 *DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any malicious purposes.
 
-[1m RELEASE NOTES: [0m 
+RELEASE NOTES: 
+
+
+v1.0.7:
+- Added new features to the registry class 
+
+- Added a computer stats class 
+
+- Refresh explorer.exe when registry is edited 
 
 
 v1.0.6:
 - Fixed a critical error with the registry class 
 
 - Added message box function to the gui class
```

### Comparing `dreamhack-1.0.6/dreamhack/colorcodes.py` & `dreamhack-1.0.7/dreamhack/colorcodes.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.6/dreamhack/downloads.py` & `dreamhack-1.0.7/dreamhack/downloads.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.6/dreamhack/encryption.py` & `dreamhack-1.0.7/dreamhack/encryption.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.6/dreamhack/gui.py` & `dreamhack-1.0.7/dreamhack/gui.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.6/dreamhack/logging.py` & `dreamhack-1.0.7/dreamhack/logging.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.6/dreamhack/networking.py` & `dreamhack-1.0.7/dreamhack/networking.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.6/dreamhack/randoms.py` & `dreamhack-1.0.7/dreamhack/randoms.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.6/dreamhack/windows.py` & `dreamhack-1.0.7/dreamhack/windows.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 class windows():
 
   @staticmethod
+  def run_as_admin():
+    import pyuac
+    if not pyuac.isUserAdmin():
+      pyuac.runAsAdmin()
+
+  @staticmethod
   def block_mouse_input(on): #type:ignore
     import ctypes
     try:
       ctypes.windll.user32.BlockInput(on) #type:ignore
     except Exception as e:
       return -1, e
     else:
@@ -40,22 +46,22 @@
   @staticmethod
   def enable_all_keyboard_keys(): #type:ignore
     keys_list = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789!@#"
     for key in keys_list:
       windows.unblock_keyboard_key(key) #type:ignore
 
   @staticmethod
-  def shutdown(timeout): #type:ignore
+  def shutdown(timeout_seconds): #type:ignore
     import os
     try:
-      timeout = int(timeout) #type:ignore
+      timeout = int(timeout_seconds) #type:ignore
     except Exception as e:
       raise e
     else:
-      os.system(f'shutdown /s /f /t {timeout}')
+      os.system(f'shutdown /s /f /t {timeout_seconds}')
 
   @staticmethod
   def get_windows_user_directory(): #type:ignore
     import os
     return os.path.expanduser('~')
 
   @staticmethod
@@ -122,8 +128,59 @@
     import os
     base = os.path.basename(file) #type:ignore
     try:
       split = base.split(".")[0]
     except Exception:
       split = base
     command = rf'netsh advfirewall firewall add rule name="{split}" dir=in action=allow program="{file}" enable=yes' #type:ignore
-    windows.run_shell_command(command) #type:ignore
+    windows.run_shell_command(command) #type:ignore
+
+class computer_stats():
+  @staticmethod
+  def get_stats():
+    import socket
+    import os
+    from .networking import networking
+    #type:ignore
+    HOSTNAME = socket.gethostname()
+    IP = socket.gethostbyname(HOSTNAME)
+    PUBLIC_IP = networking.get_public_ip()
+    try:
+      LOGIN = os.getlogin()
+    except Exception:
+      LOGIN = ""
+      
+    dict_ = {
+      "hostname": HOSTNAME,
+      "ip": IP,
+      "public_ip": PUBLIC_IP,
+      "login" : LOGIN
+    }
+    return dict_
+
+class ctypesMessageBoxIcons():
+  MB_OK = 0x0
+  MB_OKCXL = 0x01
+  MB_YESNOCXL = 0x03
+  MB_YESNO = 0x04
+  MB_HELP = 0x4000
+  TOPMOST = 0x40000
+
+  # icons
+  ICON_EXCLAIM = 0x30
+  ICON_INFO = 0x40
+  ICON_STOP = 0x10
+
+@staticmethod
+def message_box(title, text, icon, box_type, TOPMOST = False):
+  import platform
+  if platform.platform() != 'Windows':
+    return
+  import ctypes
+  from .windows import windows
+  #type:ignore
+  icons = ctypesMessageBoxIcons
+  if TOPMOST:
+    result = ctypes.windll.user32.MessageBoxA(0, text, title, box_type | icon | icons.TOPMOST) #type:ignore
+  else:
+    result = ctypes.windll.user32.MessageBoxA(0, text, title, box_type | icon) #type:ignore
+  return result
```

### Comparing `dreamhack-1.0.6/dreamhack/zipfiles.py` & `dreamhack-1.0.7/dreamhack/zipfiles.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.6/dreamhack.egg-info/PKG-INFO` & `dreamhack-1.0.7/dreamhack.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamhack
-Version: 1.0.6
+Version: 1.0.7
 Summary: The ultimate PyPi package for cyber-security and many other things.
 Author: Jack Burr
 Author-email: BurrJ22@Outlook.com
 Keywords: python,windows,encryption
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: cryptography
@@ -19,15 +19,23 @@
 Requires-Dist: CTkMessagebox
 Requires-Dist: unixreg
 
 The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
 *DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any malicious purposes.
 
-[1m RELEASE NOTES: [0m 
+RELEASE NOTES: 
+
+
+v1.0.7:
+- Added new features to the registry class 
+
+- Added a computer stats class 
+
+- Refresh explorer.exe when registry is edited 
 
 
 v1.0.6:
 - Fixed a critical error with the registry class 
 
 - Added message box function to the gui class
```

### Comparing `dreamhack-1.0.6/setup.py` & `dreamhack-1.0.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.6' 
+VERSION = '1.0.7' 
 DESCRIPTION = 'The ultimate PyPi package for cyber-security and many other things.'
 LONG_DESCRIPTION = '''The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
 *DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any malicious purposes.
 
-\033[1m RELEASE NOTES: \033[0m \n
+RELEASE NOTES: \n
+
+v1.0.7:
+- Added new features to the registry class \n
+- Added a computer stats class \n
+- Refresh explorer.exe when registry is edited \n
 
 v1.0.6:
 - Fixed a critical error with the registry class \n
 - Added message box function to the gui class \n
 
 v1.0.5:
 - Added new features to GUI class \n
```

