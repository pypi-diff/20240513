# Comparing `tmp/dreamhack-1.0.9.tar.gz` & `tmp/dreamhack-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamhack-1.0.9.tar", last modified: Mon May 13 13:17:54 2024, max compression
+gzip compressed data, was "dreamhack-1.1.0.tar", last modified: Mon May 13 13:41:11 2024, max compression
```

## Comparing `dreamhack-1.0.9.tar` & `dreamhack-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 13:17:54.058823 dreamhack-1.0.9/
--rw-r--r--   0 runner    (1000) runner    (1000)     2096 2024-05-13 13:17:54.058823 dreamhack-1.0.9/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 13:17:54.054823 dreamhack-1.0.9/dreamhack/
--rw-r--r--   0 runner    (1000) runner    (1000)     1496 2024-05-13 13:13:26.000000 dreamhack-1.0.9/dreamhack/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      916 2024-05-10 15:50:24.000000 dreamhack-1.0.9/dreamhack/colorcodes.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1153 2024-05-11 23:10:11.000000 dreamhack-1.0.9/dreamhack/downloads.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2502 2024-05-10 15:02:31.000000 dreamhack-1.0.9/dreamhack/encryption.py
--rw-r--r--   0 runner    (1000) runner    (1000)      385 2024-05-10 15:50:41.000000 dreamhack-1.0.9/dreamhack/filepaths.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3819 2024-05-11 23:29:59.000000 dreamhack-1.0.9/dreamhack/gui.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1488 2024-05-10 15:51:14.000000 dreamhack-1.0.9/dreamhack/logging.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1541 2024-05-10 15:51:32.000000 dreamhack-1.0.9/dreamhack/networking.py
--rw-r--r--   0 runner    (1000) runner    (1000)      629 2024-05-10 15:51:48.000000 dreamhack-1.0.9/dreamhack/randoms.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4884 2024-05-12 21:30:05.000000 dreamhack-1.0.9/dreamhack/registry.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6246 2024-05-13 13:00:58.000000 dreamhack-1.0.9/dreamhack/windows.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1637 2024-05-10 15:53:29.000000 dreamhack-1.0.9/dreamhack/zipfiles.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 13:17:54.054823 dreamhack-1.0.9/dreamhack.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2096 2024-05-13 13:17:53.000000 dreamhack-1.0.9/dreamhack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      436 2024-05-13 13:17:53.000000 dreamhack-1.0.9/dreamhack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-13 13:17:53.000000 dreamhack-1.0.9/dreamhack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      109 2024-05-13 13:17:53.000000 dreamhack-1.0.9/dreamhack.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-05-13 13:17:53.000000 dreamhack-1.0.9/dreamhack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-13 13:17:54.058823 dreamhack-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     2359 2024-05-13 13:17:45.000000 dreamhack-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 13:41:11.108555 dreamhack-1.1.0/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2180 2024-05-13 13:41:11.108555 dreamhack-1.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 13:41:11.076552 dreamhack-1.1.0/dreamhack/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1504 2024-05-13 13:21:37.000000 dreamhack-1.1.0/dreamhack/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      916 2024-05-10 15:50:24.000000 dreamhack-1.1.0/dreamhack/colorcodes.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1153 2024-05-11 23:10:11.000000 dreamhack-1.1.0/dreamhack/downloads.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2502 2024-05-10 15:02:31.000000 dreamhack-1.1.0/dreamhack/encryption.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      385 2024-05-10 15:50:41.000000 dreamhack-1.1.0/dreamhack/filepaths.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3819 2024-05-11 23:29:59.000000 dreamhack-1.1.0/dreamhack/gui.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1488 2024-05-10 15:51:14.000000 dreamhack-1.1.0/dreamhack/logging.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1541 2024-05-10 15:51:32.000000 dreamhack-1.1.0/dreamhack/networking.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      629 2024-05-10 15:51:48.000000 dreamhack-1.1.0/dreamhack/randoms.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4951 2024-05-13 13:39:48.000000 dreamhack-1.1.0/dreamhack/registry.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6246 2024-05-13 13:00:58.000000 dreamhack-1.1.0/dreamhack/windows.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1637 2024-05-10 15:53:29.000000 dreamhack-1.1.0/dreamhack/zipfiles.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 13:41:11.108555 dreamhack-1.1.0/dreamhack.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2180 2024-05-13 13:41:10.000000 dreamhack-1.1.0/dreamhack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      436 2024-05-13 13:41:11.000000 dreamhack-1.1.0/dreamhack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-13 13:41:10.000000 dreamhack-1.1.0/dreamhack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      119 2024-05-13 13:41:10.000000 dreamhack-1.1.0/dreamhack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-05-13 13:41:10.000000 dreamhack-1.1.0/dreamhack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-13 13:41:11.108555 dreamhack-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     2433 2024-05-13 13:40:52.000000 dreamhack-1.1.0/setup.py
```

### Comparing `dreamhack-1.0.9/PKG-INFO` & `dreamhack-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamhack
-Version: 1.0.9
+Version: 1.1.0
 Summary: The ultimate PyPi package for cyber-security and many other things.
 Author: Jack Burr
 Author-email: BurrJ22@Outlook.com
 Keywords: python,windows,encryption
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: cryptography
@@ -14,21 +14,27 @@
 Requires-Dist: requests
 Requires-Dist: public-ip
 Requires-Dist: keyboard
 Requires-Dist: pyautogui
 Requires-Dist: customtkinter
 Requires-Dist: CTkMessagebox
 Requires-Dist: unixreg
+Requires-Dist: pypiwin32
 
 The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
 *DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any malicious purposes. 
 
 RELEASE NOTES: 
 
+v1.1.0: 
+
+- Fixed a winreg error with setting the value 
+
+
 v1.0.9: 
 
 - Fixed minor error with functions not showing up in registry class 
 
 - Added function to get current version of this package
```

### Comparing `dreamhack-1.0.9/dreamhack/__init__.py` & `dreamhack-1.1.0/dreamhack/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   return os.getcwd()
 
 def get_package_version():
   import pkg_resources
   try:
       return pkg_resources.get_distribution('dreamhack').version
   except pkg_resources.DistributionNotFound:
-      return "Package not found"
+      return "Package version not found"
 
 
 def install(package):
   try:
     install_ = subprocess.check_call([sys.executable, "-m", "pip", "install", package])
   except Exception as e:
     raise e
```

### Comparing `dreamhack-1.0.9/dreamhack/colorcodes.py` & `dreamhack-1.1.0/dreamhack/colorcodes.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.9/dreamhack/downloads.py` & `dreamhack-1.1.0/dreamhack/downloads.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.9/dreamhack/encryption.py` & `dreamhack-1.1.0/dreamhack/encryption.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.9/dreamhack/gui.py` & `dreamhack-1.1.0/dreamhack/gui.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.9/dreamhack/logging.py` & `dreamhack-1.1.0/dreamhack/logging.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.9/dreamhack/networking.py` & `dreamhack-1.1.0/dreamhack/networking.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.9/dreamhack/randoms.py` & `dreamhack-1.1.0/dreamhack/randoms.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.9/dreamhack/registry.py` & `dreamhack-1.1.0/dreamhack/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,19 +40,22 @@
 
   @staticmethod
   def set(key_path_class, value_name, value, ALL_ACCESS=False):
     key_path_class.build()
     import platform
     if platform.system() ==  'Windows':
       import winreg
+      WINDOWS = True
     else:
       import unixreg as winreg #type:ignore
+      WINDOWS = False
     if type(value) is int: #type:ignore
       value_type = winreg.REG_DWORD #type:ignore
-      value = str(value)
+      if not WINDOWS:
+        value = str(value)
     else:
       value_type = winreg.REG_SZ #type:ignore
       try:
         value = str(value)
       except Exception:
         raise Exception('Invalid value') #type:ignore
     try:
```

### Comparing `dreamhack-1.0.9/dreamhack/windows.py` & `dreamhack-1.1.0/dreamhack/windows.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.9/dreamhack/zipfiles.py` & `dreamhack-1.1.0/dreamhack/zipfiles.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.9/dreamhack.egg-info/PKG-INFO` & `dreamhack-1.1.0/dreamhack.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamhack
-Version: 1.0.9
+Version: 1.1.0
 Summary: The ultimate PyPi package for cyber-security and many other things.
 Author: Jack Burr
 Author-email: BurrJ22@Outlook.com
 Keywords: python,windows,encryption
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: cryptography
@@ -14,21 +14,27 @@
 Requires-Dist: requests
 Requires-Dist: public-ip
 Requires-Dist: keyboard
 Requires-Dist: pyautogui
 Requires-Dist: customtkinter
 Requires-Dist: CTkMessagebox
 Requires-Dist: unixreg
+Requires-Dist: pypiwin32
 
 The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
 *DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any malicious purposes. 
 
 RELEASE NOTES: 
 
+v1.1.0: 
+
+- Fixed a winreg error with setting the value 
+
+
 v1.0.9: 
 
 - Fixed minor error with functions not showing up in registry class 
 
 - Added function to get current version of this package
```

### Comparing `dreamhack-1.0.9/setup.py` & `dreamhack-1.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from setuptools import setup, find_packages
 #type:ignore
 
-VERSION = '1.0.9' 
+VERSION = '1.1.0' 
 DESCRIPTION = 'The ultimate PyPi package for cyber-security and many other things.'
 LONG_DESCRIPTION = '''The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
 *DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any malicious purposes. 
 
 RELEASE NOTES: \n
+v1.1.0: \n
+- Fixed a winreg error with setting the value \n
+
 v1.0.9: \n
 - Fixed minor error with functions not showing up in registry class \n
 - Added function to get current version of this package \n
 
 v1.0.8: \n
 - Added new features to GUI and Windows classes \n
 - Fixed a few bugs \n
@@ -60,14 +63,14 @@
         name="dreamhack", 
         version=VERSION,
         author="Jack Burr",
         author_email="BurrJ22@Outlook.com",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=['cryptography', 'tqdm', 'setuptools', 'pyuac', 'requests', 'public-ip', 'keyboard', 'pyautogui', 'customtkinter', 'CTkMessagebox', 'unixreg'],  #type:ignore
+        install_requires=['cryptography', 'tqdm', 'setuptools', 'pyuac', 'requests', 'public-ip', 'keyboard', 'pyautogui', 'customtkinter', 'CTkMessagebox', 'unixreg', 'pypiwin32'],  #type:ignore
         keywords=['python', 'windows', 'encryption'],
         classifiers= [
             "Programming Language :: Python :: 3",
             "Operating System :: Microsoft :: Windows",
         ]
 )
```

