# Comparing `tmp/otp_generate-0.0.5.tar.gz` & `tmp/otp_generate-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otp_generate-0.0.5.tar", last modified: Fri May 10 14:09:41 2024, max compression
+gzip compressed data, was "otp_generate-0.0.6.tar", last modified: Mon May 13 05:22:07 2024, max compression
```

## Comparing `otp_generate-0.0.5.tar` & `otp_generate-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 marimuthu  (1000) marimuthu  (1000)        0 2024-05-10 14:09:41.795063 otp_generate-0.0.5/
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)     1083 2024-05-08 11:06:07.000000 otp_generate-0.0.5/LICENSE
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)     3382 2024-05-10 14:09:41.795063 otp_generate-0.0.5/PKG-INFO
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)     2708 2024-05-10 13:31:35.000000 otp_generate-0.0.5/README.md
-drwxr-xr-x   0 marimuthu  (1000) marimuthu  (1000)        0 2024-05-10 14:09:41.794063 otp_generate-0.0.5/otp_generate/
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       46 2024-05-10 07:45:12.000000 otp_generate-0.0.5/otp_generate/__init__.py
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)     1404 2024-05-10 13:23:26.000000 otp_generate-0.0.5/otp_generate/main.py
-drwxr-xr-x   0 marimuthu  (1000) marimuthu  (1000)        0 2024-05-10 14:09:41.795063 otp_generate-0.0.5/otp_generate.egg-info/
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)     3382 2024-05-10 14:09:41.000000 otp_generate-0.0.5/otp_generate.egg-info/PKG-INFO
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)      255 2024-05-10 14:09:41.000000 otp_generate-0.0.5/otp_generate.egg-info/SOURCES.txt
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)        1 2024-05-10 14:09:41.000000 otp_generate-0.0.5/otp_generate.egg-info/dependency_links.txt
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       61 2024-05-10 14:09:41.000000 otp_generate-0.0.5/otp_generate.egg-info/entry_points.txt
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       13 2024-05-10 14:09:41.000000 otp_generate-0.0.5/otp_generate.egg-info/top_level.txt
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       38 2024-05-10 14:09:41.795063 otp_generate-0.0.5/setup.cfg
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)     1222 2024-05-10 14:09:19.000000 otp_generate-0.0.5/setup.py
+drwxr-xr-x   0 marimuthu  (1000) marimuthu  (1000)        0 2024-05-13 05:22:07.698094 otp_generate-0.0.6/
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)     1083 2024-05-08 11:06:07.000000 otp_generate-0.0.6/LICENSE
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)     3380 2024-05-13 05:22:07.698094 otp_generate-0.0.6/PKG-INFO
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)     2706 2024-05-13 05:06:00.000000 otp_generate-0.0.6/README.md
+drwxr-xr-x   0 marimuthu  (1000) marimuthu  (1000)        0 2024-05-13 05:22:07.697095 otp_generate-0.0.6/otp_generate/
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       46 2024-05-10 07:45:12.000000 otp_generate-0.0.6/otp_generate/__init__.py
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)     1404 2024-05-10 13:23:26.000000 otp_generate-0.0.6/otp_generate/main.py
+drwxr-xr-x   0 marimuthu  (1000) marimuthu  (1000)        0 2024-05-13 05:22:07.698094 otp_generate-0.0.6/otp_generate.egg-info/
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)     3380 2024-05-13 05:22:07.000000 otp_generate-0.0.6/otp_generate.egg-info/PKG-INFO
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)      255 2024-05-13 05:22:07.000000 otp_generate-0.0.6/otp_generate.egg-info/SOURCES.txt
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)        1 2024-05-13 05:22:07.000000 otp_generate-0.0.6/otp_generate.egg-info/dependency_links.txt
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       61 2024-05-13 05:22:07.000000 otp_generate-0.0.6/otp_generate.egg-info/entry_points.txt
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       13 2024-05-13 05:22:07.000000 otp_generate-0.0.6/otp_generate.egg-info/top_level.txt
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       38 2024-05-13 05:22:07.699094 otp_generate-0.0.6/setup.cfg
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)     1222 2024-05-13 05:21:32.000000 otp_generate-0.0.6/setup.py
```

### Comparing `otp_generate-0.0.5/LICENSE` & `otp_generate-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `otp_generate-0.0.5/PKG-INFO` & `otp_generate-0.0.6/otp_generate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: otp_generate
-Version: 0.0.5
+Name: otp-generate
+Version: 0.0.6
 Summary: A simple otp generate package
 Home-page: https://github.com/MariMuthu15/otp-generate-package
 Author: Marimuthu
 Author-email: mahimari555@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -41,18 +41,18 @@
 
 Create 6 digits otp. OTP will change 2 minutes once based on your_own_secret_key.
     
     from otp_generate import generate_otp
         
     otp = generate_otp('your_own_secret_key')
     print(otp)
-To change interval time pass the value in seconds.
+To change interval time pass the value in minutes.
         
     from otp_generate import generate_otp
-    otp = generate_otp('your_own_secret', interval=120)
+    otp = generate_otp('your_own_secret', interval=5)
 To get 7 or 8 length otp.
         
     from otp_generate import generate_otp
     otp = generate_otp('your_own_secret', length=7)
 To get hashed OTP. Mixed of char and numbers
         
     from otp_generate import generate_otp
```

### Comparing `otp_generate-0.0.5/README.md` & `otp_generate-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 
 Create 6 digits otp. OTP will change 2 minutes once based on your_own_secret_key.
     
     from otp_generate import generate_otp
         
     otp = generate_otp('your_own_secret_key')
     print(otp)
-To change interval time pass the value in seconds.
+To change interval time pass the value in minutes.
         
     from otp_generate import generate_otp
-    otp = generate_otp('your_own_secret', interval=120)
+    otp = generate_otp('your_own_secret', interval=5)
 To get 7 or 8 length otp.
         
     from otp_generate import generate_otp
     otp = generate_otp('your_own_secret', length=7)
 To get hashed OTP. Mixed of char and numbers
         
     from otp_generate import generate_otp
```

### Comparing `otp_generate-0.0.5/otp_generate/main.py` & `otp_generate-0.0.6/otp_generate/main.py`

 * *Files identical despite different names*

### Comparing `otp_generate-0.0.5/otp_generate.egg-info/PKG-INFO` & `otp_generate-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: otp-generate
-Version: 0.0.5
+Name: otp_generate
+Version: 0.0.6
 Summary: A simple otp generate package
 Home-page: https://github.com/MariMuthu15/otp-generate-package
 Author: Marimuthu
 Author-email: mahimari555@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -41,18 +41,18 @@
 
 Create 6 digits otp. OTP will change 2 minutes once based on your_own_secret_key.
     
     from otp_generate import generate_otp
         
     otp = generate_otp('your_own_secret_key')
     print(otp)
-To change interval time pass the value in seconds.
+To change interval time pass the value in minutes.
         
     from otp_generate import generate_otp
-    otp = generate_otp('your_own_secret', interval=120)
+    otp = generate_otp('your_own_secret', interval=5)
 To get 7 or 8 length otp.
         
     from otp_generate import generate_otp
     otp = generate_otp('your_own_secret', length=7)
 To get hashed OTP. Mixed of char and numbers
         
     from otp_generate import generate_otp
```

### Comparing `otp_generate-0.0.5/setup.py` & `otp_generate-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 working_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(working_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='otp_generate',  # name of package which will be package dir below project
-    version='0.0.5',
+    version='0.0.6',
     url='https://github.com/MariMuthu15/otp-generate-package',
     author='Marimuthu',
     author_email='mahimari555@gmail.com',
     description='A simple otp generate package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

