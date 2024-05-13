# Comparing `tmp/dreamhack-1.0.7.tar.gz` & `tmp/dreamhack-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamhack-1.0.7.tar", last modified: Sun May 12 21:50:41 2024, max compression
+gzip compressed data, was "dreamhack-1.0.8.tar", last modified: Mon May 13 13:04:19 2024, max compression
```

## Comparing `dreamhack-1.0.7.tar` & `dreamhack-1.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-12 21:50:41.871703 dreamhack-1.0.7/
--rw-r--r--   0 runner    (1000) runner    (1000)     1859 2024-05-12 21:50:41.871703 dreamhack-1.0.7/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-12 21:50:41.867704 dreamhack-1.0.7/dreamhack/
--rw-r--r--   0 runner    (1000) runner    (1000)     1130 2024-05-12 21:49:00.000000 dreamhack-1.0.7/dreamhack/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      916 2024-05-10 15:50:24.000000 dreamhack-1.0.7/dreamhack/colorcodes.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1153 2024-05-11 23:10:11.000000 dreamhack-1.0.7/dreamhack/downloads.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2502 2024-05-10 15:02:31.000000 dreamhack-1.0.7/dreamhack/encryption.py
--rw-r--r--   0 runner    (1000) runner    (1000)      385 2024-05-10 15:50:41.000000 dreamhack-1.0.7/dreamhack/filepaths.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3819 2024-05-11 23:29:59.000000 dreamhack-1.0.7/dreamhack/gui.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1488 2024-05-10 15:51:14.000000 dreamhack-1.0.7/dreamhack/logging.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1541 2024-05-10 15:51:32.000000 dreamhack-1.0.7/dreamhack/networking.py
--rw-r--r--   0 runner    (1000) runner    (1000)      629 2024-05-10 15:51:48.000000 dreamhack-1.0.7/dreamhack/randoms.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4884 2024-05-12 21:30:05.000000 dreamhack-1.0.7/dreamhack/registry.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5052 2024-05-12 21:45:39.000000 dreamhack-1.0.7/dreamhack/windows.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1637 2024-05-10 15:53:29.000000 dreamhack-1.0.7/dreamhack/zipfiles.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-12 21:50:41.871703 dreamhack-1.0.7/dreamhack.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1859 2024-05-12 21:50:41.000000 dreamhack-1.0.7/dreamhack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      436 2024-05-12 21:50:41.000000 dreamhack-1.0.7/dreamhack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-12 21:50:41.000000 dreamhack-1.0.7/dreamhack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      109 2024-05-12 21:50:41.000000 dreamhack-1.0.7/dreamhack.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-05-12 21:50:41.000000 dreamhack-1.0.7/dreamhack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-12 21:50:41.875703 dreamhack-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     2082 2024-05-12 21:50:37.000000 dreamhack-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 13:04:19.198471 dreamhack-1.0.8/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1957 2024-05-13 13:04:19.194471 dreamhack-1.0.8/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 13:04:19.194471 dreamhack-1.0.8/dreamhack/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1130 2024-05-12 21:49:00.000000 dreamhack-1.0.8/dreamhack/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      916 2024-05-10 15:50:24.000000 dreamhack-1.0.8/dreamhack/colorcodes.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1153 2024-05-11 23:10:11.000000 dreamhack-1.0.8/dreamhack/downloads.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2502 2024-05-10 15:02:31.000000 dreamhack-1.0.8/dreamhack/encryption.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      385 2024-05-10 15:50:41.000000 dreamhack-1.0.8/dreamhack/filepaths.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3819 2024-05-11 23:29:59.000000 dreamhack-1.0.8/dreamhack/gui.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1488 2024-05-10 15:51:14.000000 dreamhack-1.0.8/dreamhack/logging.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1541 2024-05-10 15:51:32.000000 dreamhack-1.0.8/dreamhack/networking.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      629 2024-05-10 15:51:48.000000 dreamhack-1.0.8/dreamhack/randoms.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4884 2024-05-12 21:30:05.000000 dreamhack-1.0.8/dreamhack/registry.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6246 2024-05-13 13:00:58.000000 dreamhack-1.0.8/dreamhack/windows.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1637 2024-05-10 15:53:29.000000 dreamhack-1.0.8/dreamhack/zipfiles.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 13:04:19.194471 dreamhack-1.0.8/dreamhack.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1957 2024-05-13 13:04:18.000000 dreamhack-1.0.8/dreamhack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      436 2024-05-13 13:04:19.000000 dreamhack-1.0.8/dreamhack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-13 13:04:18.000000 dreamhack-1.0.8/dreamhack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      109 2024-05-13 13:04:18.000000 dreamhack-1.0.8/dreamhack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-05-13 13:04:18.000000 dreamhack-1.0.8/dreamhack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-13 13:04:19.198471 dreamhack-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     2217 2024-05-13 13:03:57.000000 dreamhack-1.0.8/setup.py
```

### Comparing `dreamhack-1.0.7/PKG-INFO` & `dreamhack-1.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamhack
-Version: 1.0.7
+Version: 1.0.8
 Summary: The ultimate PyPi package for cyber-security and many other things.
 Author: Jack Burr
 Author-email: BurrJ22@Outlook.com
 Keywords: python,windows,encryption
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: cryptography
@@ -17,71 +17,85 @@
 Requires-Dist: pyautogui
 Requires-Dist: customtkinter
 Requires-Dist: CTkMessagebox
 Requires-Dist: unixreg
 
 The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
-*DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any malicious purposes.
+*DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any malicious purposes. 
 
 RELEASE NOTES: 
 
+v1.0.8: 
+
+- Added new features to GUI and Windows classes 
+
+- Fixed a few bugs 
+
+
+v1.0.7: 
 
-v1.0.7:
 - Added new features to the registry class 
 
 - Added a computer stats class 
 
 - Refresh explorer.exe when registry is edited 
 
 
-v1.0.6:
+v1.0.6: 
+
 - Fixed a critical error with the registry class 
 
 - Added message box function to the gui class 
 
 
-v1.0.5:
+v1.0.5: 
+
 - Added new features to GUI class 
 
 - Added new RegistryEditor class (For Windows only, experimental phase) 
 
 
-v1.0.4:
+v1.0.4: 
+
 - Fixed a few bugs 
 
 - Added a few more features 
 
 
-v1.0.3:
+v1.0.3: 
+
 - Added logging content 
 
 - Added the ability to get the public ip of the current machine 
 
 - Added lots of new features 
 
 - A few bug fixes 
 
 
-v1.0.2:
+v1.0.2: 
+
 - First official stable version, DO NOT USE PREVIOUS VERSIONS 
 
 - Added content to encryption and logging 
 
 - Created networking 
 
 
 
 WARNING: VERSIONS BELOW THIS NOTE ARE UNSTABLE. DO NOT USE THEM.
 
 
-v1.0.1:
+v1.0.1: 
+
 - Fixed critical error from v1.0.0 
 
 - Working on new version 
 
 
-v1.0.0:
+v1.0.0: 
+
 - Initial release 
 
 - NOTE: Encryption and logging are both empty for the first few versions.
```

### Comparing `dreamhack-1.0.7/dreamhack/__init__.py` & `dreamhack-1.0.8/dreamhack/__init__.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.7/dreamhack/colorcodes.py` & `dreamhack-1.0.8/dreamhack/colorcodes.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.7/dreamhack/downloads.py` & `dreamhack-1.0.8/dreamhack/downloads.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.7/dreamhack/encryption.py` & `dreamhack-1.0.8/dreamhack/encryption.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.7/dreamhack/gui.py` & `dreamhack-1.0.8/dreamhack/gui.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.7/dreamhack/logging.py` & `dreamhack-1.0.8/dreamhack/logging.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.7/dreamhack/networking.py` & `dreamhack-1.0.8/dreamhack/networking.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.7/dreamhack/randoms.py` & `dreamhack-1.0.8/dreamhack/randoms.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.7/dreamhack/registry.py` & `dreamhack-1.0.8/dreamhack/registry.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.7/dreamhack/zipfiles.py` & `dreamhack-1.0.8/dreamhack/zipfiles.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.7/dreamhack.egg-info/PKG-INFO` & `dreamhack-1.0.8/dreamhack.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamhack
-Version: 1.0.7
+Version: 1.0.8
 Summary: The ultimate PyPi package for cyber-security and many other things.
 Author: Jack Burr
 Author-email: BurrJ22@Outlook.com
 Keywords: python,windows,encryption
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: cryptography
@@ -17,71 +17,85 @@
 Requires-Dist: pyautogui
 Requires-Dist: customtkinter
 Requires-Dist: CTkMessagebox
 Requires-Dist: unixreg
 
 The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
-*DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any malicious purposes.
+*DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any malicious purposes. 
 
 RELEASE NOTES: 
 
+v1.0.8: 
+
+- Added new features to GUI and Windows classes 
+
+- Fixed a few bugs 
+
+
+v1.0.7: 
 
-v1.0.7:
 - Added new features to the registry class 
 
 - Added a computer stats class 
 
 - Refresh explorer.exe when registry is edited 
 
 
-v1.0.6:
+v1.0.6: 
+
 - Fixed a critical error with the registry class 
 
 - Added message box function to the gui class 
 
 
-v1.0.5:
+v1.0.5: 
+
 - Added new features to GUI class 
 
 - Added new RegistryEditor class (For Windows only, experimental phase) 
 
 
-v1.0.4:
+v1.0.4: 
+
 - Fixed a few bugs 
 
 - Added a few more features 
 
 
-v1.0.3:
+v1.0.3: 
+
 - Added logging content 
 
 - Added the ability to get the public ip of the current machine 
 
 - Added lots of new features 
 
 - A few bug fixes 
 
 
-v1.0.2:
+v1.0.2: 
+
 - First official stable version, DO NOT USE PREVIOUS VERSIONS 
 
 - Added content to encryption and logging 
 
 - Created networking 
 
 
 
 WARNING: VERSIONS BELOW THIS NOTE ARE UNSTABLE. DO NOT USE THEM.
 
 
-v1.0.1:
+v1.0.1: 
+
 - Fixed critical error from v1.0.0 
 
 - Working on new version 
 
 
-v1.0.0:
+v1.0.0: 
+
 - Initial release 
 
 - NOTE: Encryption and logging are both empty for the first few versions.
```

### Comparing `dreamhack-1.0.7/setup.py` & `dreamhack-1.0.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,60 @@
 from setuptools import setup, find_packages
+#type:ignore
 
-VERSION = '1.0.7' 
+VERSION = '1.0.8' 
 DESCRIPTION = 'The ultimate PyPi package for cyber-security and many other things.'
 LONG_DESCRIPTION = '''The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
-*DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any malicious purposes.
+*DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any malicious purposes. 
 
 RELEASE NOTES: \n
+v1.0.8: \n
+- Added new features to GUI and Windows classes \n
+- Fixed a few bugs \n
 
-v1.0.7:
+v1.0.7: \n
 - Added new features to the registry class \n
 - Added a computer stats class \n
 - Refresh explorer.exe when registry is edited \n
 
-v1.0.6:
+v1.0.6: \n
 - Fixed a critical error with the registry class \n
 - Added message box function to the gui class \n
 
-v1.0.5:
+v1.0.5: \n
 - Added new features to GUI class \n
 - Added new RegistryEditor class (For Windows only, experimental phase) \n
 
-v1.0.4:
+v1.0.4: \n
 - Fixed a few bugs \n
 - Added a few more features \n
 
-v1.0.3:
+v1.0.3: \n
 - Added logging content \n
 - Added the ability to get the public ip of the current machine \n
 - Added lots of new features \n
 - A few bug fixes \n
 
-v1.0.2:
+v1.0.2: \n
 - First official stable version, DO NOT USE PREVIOUS VERSIONS \n
 - Added content to encryption and logging \n
 - Created networking \n
 \n
 WARNING: VERSIONS BELOW THIS NOTE ARE UNSTABLE. DO NOT USE THEM.
 \n
-v1.0.1:
+v1.0.1: \n
 - Fixed critical error from v1.0.0 \n
 - Working on new version \n
 
-v1.0.0:
+v1.0.0: \n
 - Initial release \n
 - NOTE: Encryption and logging are both empty for the first few versions. \n
 '''
+#type:ignore
 
 setup(
         name="dreamhack", 
         version=VERSION,
         author="Jack Burr",
         author_email="BurrJ22@Outlook.com",
         description=DESCRIPTION,
```

