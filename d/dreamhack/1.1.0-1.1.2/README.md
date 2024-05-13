# Comparing `tmp/dreamhack-1.1.0.tar.gz` & `tmp/dreamhack-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamhack-1.1.0.tar", last modified: Mon May 13 13:41:11 2024, max compression
+gzip compressed data, was "dreamhack-1.1.2.tar", last modified: Mon May 13 16:34:40 2024, max compression
```

## Comparing `dreamhack-1.1.0.tar` & `dreamhack-1.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 13:41:11.108555 dreamhack-1.1.0/
--rw-r--r--   0 runner    (1000) runner    (1000)     2180 2024-05-13 13:41:11.108555 dreamhack-1.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 13:41:11.076552 dreamhack-1.1.0/dreamhack/
--rw-r--r--   0 runner    (1000) runner    (1000)     1504 2024-05-13 13:21:37.000000 dreamhack-1.1.0/dreamhack/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      916 2024-05-10 15:50:24.000000 dreamhack-1.1.0/dreamhack/colorcodes.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1153 2024-05-11 23:10:11.000000 dreamhack-1.1.0/dreamhack/downloads.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2502 2024-05-10 15:02:31.000000 dreamhack-1.1.0/dreamhack/encryption.py
--rw-r--r--   0 runner    (1000) runner    (1000)      385 2024-05-10 15:50:41.000000 dreamhack-1.1.0/dreamhack/filepaths.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3819 2024-05-11 23:29:59.000000 dreamhack-1.1.0/dreamhack/gui.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1488 2024-05-10 15:51:14.000000 dreamhack-1.1.0/dreamhack/logging.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1541 2024-05-10 15:51:32.000000 dreamhack-1.1.0/dreamhack/networking.py
--rw-r--r--   0 runner    (1000) runner    (1000)      629 2024-05-10 15:51:48.000000 dreamhack-1.1.0/dreamhack/randoms.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4951 2024-05-13 13:39:48.000000 dreamhack-1.1.0/dreamhack/registry.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6246 2024-05-13 13:00:58.000000 dreamhack-1.1.0/dreamhack/windows.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1637 2024-05-10 15:53:29.000000 dreamhack-1.1.0/dreamhack/zipfiles.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 13:41:11.108555 dreamhack-1.1.0/dreamhack.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2180 2024-05-13 13:41:10.000000 dreamhack-1.1.0/dreamhack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      436 2024-05-13 13:41:11.000000 dreamhack-1.1.0/dreamhack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-13 13:41:10.000000 dreamhack-1.1.0/dreamhack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      119 2024-05-13 13:41:10.000000 dreamhack-1.1.0/dreamhack.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-05-13 13:41:10.000000 dreamhack-1.1.0/dreamhack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-13 13:41:11.108555 dreamhack-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     2433 2024-05-13 13:40:52.000000 dreamhack-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 16:34:40.654082 dreamhack-1.1.2/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2352 2024-05-13 16:34:40.654082 dreamhack-1.1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 16:34:40.646081 dreamhack-1.1.2/dreamhack/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1935 2024-05-13 16:15:37.000000 dreamhack-1.1.2/dreamhack/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      916 2024-05-10 15:50:24.000000 dreamhack-1.1.2/dreamhack/colorcodes.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1153 2024-05-11 23:10:11.000000 dreamhack-1.1.2/dreamhack/downloads.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2502 2024-05-10 15:02:31.000000 dreamhack-1.1.2/dreamhack/encryption.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      565 2024-05-13 15:44:44.000000 dreamhack-1.1.2/dreamhack/filepaths.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3819 2024-05-11 23:29:59.000000 dreamhack-1.1.2/dreamhack/gui.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1488 2024-05-10 15:51:14.000000 dreamhack-1.1.2/dreamhack/logging.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1541 2024-05-10 15:51:32.000000 dreamhack-1.1.2/dreamhack/networking.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      629 2024-05-10 15:51:48.000000 dreamhack-1.1.2/dreamhack/randoms.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4951 2024-05-13 13:39:48.000000 dreamhack-1.1.2/dreamhack/registry.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6641 2024-05-13 15:46:58.000000 dreamhack-1.1.2/dreamhack/windows.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1637 2024-05-10 15:53:29.000000 dreamhack-1.1.2/dreamhack/zipfiles.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 16:34:40.650082 dreamhack-1.1.2/dreamhack.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2352 2024-05-13 16:34:40.000000 dreamhack-1.1.2/dreamhack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      436 2024-05-13 16:34:40.000000 dreamhack-1.1.2/dreamhack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-13 16:34:40.000000 dreamhack-1.1.2/dreamhack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      123 2024-05-13 16:34:40.000000 dreamhack-1.1.2/dreamhack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-05-13 16:34:40.000000 dreamhack-1.1.2/dreamhack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-13 16:34:40.654082 dreamhack-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     2611 2024-05-13 16:34:07.000000 dreamhack-1.1.2/setup.py
```

### Comparing `dreamhack-1.1.0/PKG-INFO` & `dreamhack-1.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamhack
-Version: 1.1.0
+Version: 1.1.2
 Summary: The ultimate PyPi package for cyber-security and many other things.
 Author: Jack Burr
 Author-email: BurrJ22@Outlook.com
 Keywords: python,windows,encryption
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: cryptography
@@ -14,22 +14,36 @@
 Requires-Dist: requests
 Requires-Dist: public-ip
 Requires-Dist: keyboard
 Requires-Dist: pyautogui
 Requires-Dist: customtkinter
 Requires-Dist: CTkMessagebox
 Requires-Dist: unixreg
-Requires-Dist: pypiwin32
+Requires-Dist: win32security
 
 The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
 *DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any malicious purposes. 
 
 RELEASE NOTES: 
 
+v1.1.2: 
+
+- Added a few new features 
+
+- Fixed some new bugs 
+
+- Added new classes 
+
+
+v1.1.1: 
+
+- This version had to be deleted because of an error with pypiwin32. 
+
+
 v1.1.0: 
 
 - Fixed a winreg error with setting the value 
 
 
 v1.0.9:
```

### Comparing `dreamhack-1.1.0/dreamhack/__init__.py` & `dreamhack-1.1.2/dreamhack/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from .zipfiles import zipfiles
 from .logging import logging 
 from .networking import networking
 from .randoms import randoms
 from .downloads import downloads
 from .filepaths import filepaths
 from .gui import gui
+from .windows import ctypesMessageBoxIcons
+from .windows import computer_stats
 from .registry import RegistryEditor
 from .registry import disable_regedit
 from .registry import lock_all_drives
 from .registry import disable_task_manager
 from .registry import add_to_windows_startup
 
 #type:ignore
@@ -51,7 +53,19 @@
     install(package)
 
 def random_int_in_range(min, max):
   return randoms.random_number_in_range(min,max)
 
 def list_directory(directory):
   return filepaths.get_all_files_in_directory(directory)
+
+def create_blank_file(file_path):
+  try:
+    with open(file_path, 'w') as f:
+      f.write("")
+      f.close()
+  except PermissionError:
+    raise PermissionError(f"Error creating {file_path}: Access Denied.") #type:ignore
+  except Exception as e:
+    raise Exception(f"Error creating file {file_path} : {e}") #type:ignore
+  else:
+    return file_path
```

### Comparing `dreamhack-1.1.0/dreamhack/colorcodes.py` & `dreamhack-1.1.2/dreamhack/colorcodes.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.0/dreamhack/downloads.py` & `dreamhack-1.1.2/dreamhack/downloads.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.0/dreamhack/encryption.py` & `dreamhack-1.1.2/dreamhack/encryption.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.0/dreamhack/gui.py` & `dreamhack-1.1.2/dreamhack/gui.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.0/dreamhack/logging.py` & `dreamhack-1.1.2/dreamhack/logging.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.0/dreamhack/networking.py` & `dreamhack-1.1.2/dreamhack/networking.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.0/dreamhack/randoms.py` & `dreamhack-1.1.2/dreamhack/randoms.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.0/dreamhack/registry.py` & `dreamhack-1.1.2/dreamhack/registry.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.0/dreamhack/windows.py` & `dreamhack-1.1.2/dreamhack/windows.py`

 * *Files 6% similar despite different names*

```diff
@@ -130,14 +130,86 @@
     try:
       split = base.split(".")[0]
     except Exception:
       split = base
     command = rf'netsh advfirewall firewall add rule name="{split}" dir=in action=allow program="{file}" enable=yes' #type:ignore
     windows.run_shell_command(command) #type:ignore
 
+  @staticmethod
+  def message_box(title, text, icon, box_type, TOPMOST = False):
+    import platform
+    if platform.platform() != 'Windows':
+      return
+    import ctypes
+    from .windows import windows
+    #type:ignore
+    icons = ctypesMessageBoxIcons
+    if TOPMOST:
+      result = ctypes.windll.user32.MessageBoxA(0, text, title, box_type | icon | icons.TOPMOST) #type:ignore
+    else:
+      result = ctypes.windll.user32.MessageBoxA(0, text, title, box_type | icon) #type:ignore
+    return result
+
+  @staticmethod
+  def set_windows_desktop_wallpaper(wallpaper_path):
+    import ctypes
+    import os
+    SPI_SETDESKWALLPAPER = 20
+    SPI_SETDESKWALLPAPER_W = 20
+    # Path to the wallpaper image
+    wallpaper_path = os.path.realpath(wallpaper_path)
+    if os.path.exists(wallpaper_path):
+      try:
+        ctypes.windll.user32.SystemParametersInfoW(SPI_SETDESKWALLPAPER_W, 0, wallpaper_path, 6) #type:ignore
+      except Exception as e:
+        raise Exception(f"Error setting desktop wallpaper: {e}") #type:ignore
+    else:
+      raise FileNotFoundError("Invalid wallpaper path.")
+
+  @staticmethod
+  def type_keys(message, delay_seconds):
+    import pyautogui #type:ignore
+    try:
+      message = str(message)
+    except Exception:
+      raise ValueError("Invalid message.") #type:ignore
+    else:
+      pyautogui.write(message, interval=delay_seconds)
+
+  @staticmethod 
+  def open_notepad():
+    import subprocess
+    import platform
+    #type:ignore
+    if platform.platform() != 'Windows':
+      return
+    subprocess.check_call(['notepad.exe'])
+
+  @staticmethod
+  def run_cmd_command(command):
+    import subprocess
+    import platform
+    #type:ignore
+    if platform.platform() != 'Windows':
+      return
+    subprocess.check_call(['cmd', '/c', f'"{command}"'])
+
+  @staticmethod
+  def create_appdata_folder(path):
+    import os
+    from .windows import windows
+    #type:ignore
+    path = os.path.join(windows.get_folder_in_user_dir('AppData'), path)
+    try:
+      os.makedirs(path)
+    except Exception:
+      return
+    else:
+      return path
+
 class computer_stats():
   @staticmethod
   def get_stats():
     import socket
     import os
     from .networking import networking
     #type:ignore
@@ -166,65 +238,7 @@
   TOPMOST = 0x40000
 
   # icons
   ICON_EXCLAIM = 0x30
   ICON_INFO = 0x40
   ICON_STOP = 0x10
 
-@staticmethod
-def message_box(title, text, icon, box_type, TOPMOST = False):
-  import platform
-  if platform.platform() != 'Windows':
-    return
-  import ctypes
-  from .windows import windows
-  #type:ignore
-  icons = ctypesMessageBoxIcons
-  if TOPMOST:
-    result = ctypes.windll.user32.MessageBoxA(0, text, title, box_type | icon | icons.TOPMOST) #type:ignore
-  else:
-    result = ctypes.windll.user32.MessageBoxA(0, text, title, box_type | icon) #type:ignore
-  return result
-
-@staticmethod
-def set_windows_desktop_wallpaper(wallpaper_path):
-  import ctypes
-  import os
-  SPI_SETDESKWALLPAPER = 20
-  SPI_SETDESKWALLPAPER_W = 20
-  # Path to the wallpaper image
-  wallpaper_path = os.path.realpath(wallpaper_path)
-  if os.path.exists(wallpaper_path):
-    try:
-      ctypes.windll.user32.SystemParametersInfoW(SPI_SETDESKWALLPAPER_W, 0, wallpaper_path, 6) #type:ignore
-    except Exception as e:
-      raise Exception(f"Error setting desktop wallpaper: {e}") #type:ignore
-  else:
-    raise FileNotFoundError("Invalid wallpaper path.")
-
-@staticmethod
-def type_keys(message, delay_seconds):
-  import pyautogui #type:ignore
-  try:
-    message = str(message)
-  except Exception:
-    raise ValueError("Invalid message.") #type:ignore
-  else:
-    pyautogui.write(message, interval=delay_seconds)
-
-@staticmethod 
-def open_notepad():
-  import subprocess
-  import platform
-  #type:ignore
-  if platform.platform() != 'Windows':
-    return
-  subprocess.check_call(['notepad.exe'])
-
-@staticmethod
-def run_cmd_command(command):
-  import subprocess
-  import platform
-  #type:ignore
-  if platform.platform() != 'Windows':
-    return
-  subprocess.check_call(['cmd', '/c', f'"{command}"'])
```

### Comparing `dreamhack-1.1.0/dreamhack/zipfiles.py` & `dreamhack-1.1.2/dreamhack/zipfiles.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.0/dreamhack.egg-info/PKG-INFO` & `dreamhack-1.1.2/dreamhack.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamhack
-Version: 1.1.0
+Version: 1.1.2
 Summary: The ultimate PyPi package for cyber-security and many other things.
 Author: Jack Burr
 Author-email: BurrJ22@Outlook.com
 Keywords: python,windows,encryption
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: cryptography
@@ -14,22 +14,36 @@
 Requires-Dist: requests
 Requires-Dist: public-ip
 Requires-Dist: keyboard
 Requires-Dist: pyautogui
 Requires-Dist: customtkinter
 Requires-Dist: CTkMessagebox
 Requires-Dist: unixreg
-Requires-Dist: pypiwin32
+Requires-Dist: win32security
 
 The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
 *DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any malicious purposes. 
 
 RELEASE NOTES: 
 
+v1.1.2: 
+
+- Added a few new features 
+
+- Fixed some new bugs 
+
+- Added new classes 
+
+
+v1.1.1: 
+
+- This version had to be deleted because of an error with pypiwin32. 
+
+
 v1.1.0: 
 
 - Fixed a winreg error with setting the value 
 
 
 v1.0.9:
```

### Comparing `dreamhack-1.1.0/setup.py` & `dreamhack-1.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 from setuptools import setup, find_packages
 #type:ignore
 
-VERSION = '1.1.0' 
+VERSION = '1.1.2' 
 DESCRIPTION = 'The ultimate PyPi package for cyber-security and many other things.'
 LONG_DESCRIPTION = '''The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
 *DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any malicious purposes. 
 
 RELEASE NOTES: \n
+v1.1.2: \n
+- Added a few new features \n
+- Fixed some new bugs \n
+- Added new classes \n
+
+v1.1.1: \n
+- This version had to be deleted because of an error with pypiwin32. \n
+
 v1.1.0: \n
 - Fixed a winreg error with setting the value \n
 
 v1.0.9: \n
 - Fixed minor error with functions not showing up in registry class \n
 - Added function to get current version of this package \n
 
@@ -63,14 +71,14 @@
         name="dreamhack", 
         version=VERSION,
         author="Jack Burr",
         author_email="BurrJ22@Outlook.com",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=['cryptography', 'tqdm', 'setuptools', 'pyuac', 'requests', 'public-ip', 'keyboard', 'pyautogui', 'customtkinter', 'CTkMessagebox', 'unixreg', 'pypiwin32'],  #type:ignore
+        install_requires=['cryptography', 'tqdm', 'setuptools', 'pyuac', 'requests', 'public-ip', 'keyboard', 'pyautogui', 'customtkinter', 'CTkMessagebox', 'unixreg', 'win32security'],  #type:ignore
         keywords=['python', 'windows', 'encryption'],
         classifiers= [
             "Programming Language :: Python :: 3",
             "Operating System :: Microsoft :: Windows",
         ]
 )
```

