# Comparing `tmp/ownotp-0.1.0.tar.gz` & `tmp/ownotp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ownotp-0.1.0.tar", last modified: Fri May 10 12:52:23 2024, max compression
+gzip compressed data, was "ownotp-0.1.1.tar", last modified: Mon May 13 07:02:55 2024, max compression
```

## Comparing `ownotp-0.1.0.tar` & `ownotp-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:23.362504 ownotp-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-10 12:52:19.000000 ownotp-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-10 12:52:23.362504 ownotp-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-10 12:52:19.000000 ownotp-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:23.362504 ownotp-0.1.0/ownotp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:19.000000 ownotp-0.1.0/ownotp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-10 12:52:19.000000 ownotp-0.1.0/ownotp/otp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:23.362504 ownotp-0.1.0/ownotp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-10 12:52:23.000000 ownotp-0.1.0/ownotp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-10 12:52:23.000000 ownotp-0.1.0/ownotp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:52:23.000000 ownotp-0.1.0/ownotp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 12:52:23.000000 ownotp-0.1.0/ownotp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 12:52:23.362504 ownotp-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-10 12:52:19.000000 ownotp-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:23.362504 ownotp-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-10 12:52:19.000000 ownotp-0.1.0/tests/test_otp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:02:55.646977 ownotp-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-13 07:02:49.000000 ownotp-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-13 07:02:55.646977 ownotp-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-13 07:02:49.000000 ownotp-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:02:55.646977 ownotp-0.1.1/ownotp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:02:49.000000 ownotp-0.1.1/ownotp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-13 07:02:49.000000 ownotp-0.1.1/ownotp/otp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:02:55.646977 ownotp-0.1.1/ownotp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-13 07:02:55.000000 ownotp-0.1.1/ownotp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-13 07:02:55.000000 ownotp-0.1.1/ownotp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 07:02:55.000000 ownotp-0.1.1/ownotp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 07:02:55.000000 ownotp-0.1.1/ownotp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 07:02:55.646977 ownotp-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-13 07:02:49.000000 ownotp-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:02:55.646977 ownotp-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-13 07:02:49.000000 ownotp-0.1.1/tests/test_otp.py
```

### Comparing `ownotp-0.1.0/LICENSE` & `ownotp-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ownotp-0.1.0/PKG-INFO` & `ownotp-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ownotp
-Version: 0.1.0
+Version: 0.1.1
 Summary: Generate a time-based OTP using SHA-256 hashing algorithm
 Home-page: https://github.com/karthiksenniyappan/ownotp
 Author: karthiksenniyappan
 Author-email: karthiksenniyappan76@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,18 @@
 print(otp)
 ```
 To change interval time pass the value in seconds.
 ```python
 from ownotp.otp import generate_otp
 otp = generate_otp('your_own_secret', interval=120)
 ```
-To get 7 or 8 length otp.
+
+To generate different length OTP.
+
+Note: Minium 4 and Maximum 8 length will support. If condition not satisfied default length will take to generate OTP.
 ```python
 from ownotp.otp import generate_otp
 otp = generate_otp('your_own_secret', length=7)
 ```
 To get hashed OTP. Mixed of char and numbers
 ```python
 from ownotp.otp import generate_otp
```

### Comparing `ownotp-0.1.0/README.md` & `ownotp-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,18 @@
 print(otp)
 ```
 To change interval time pass the value in seconds.
 ```python
 from ownotp.otp import generate_otp
 otp = generate_otp('your_own_secret', interval=120)
 ```
-To get 7 or 8 length otp.
+
+To generate different length OTP.
+
+Note: Minium 4 and Maximum 8 length will support. If condition not satisfied default length will take to generate OTP.
 ```python
 from ownotp.otp import generate_otp
 otp = generate_otp('your_own_secret', length=7)
 ```
 To get hashed OTP. Mixed of char and numbers
 ```python
 from ownotp.otp import generate_otp
```

### Comparing `ownotp-0.1.0/ownotp/otp.py` & `ownotp-0.1.1/ownotp/otp.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,18 +5,29 @@
 def generate_otp(secret_key, interval=120, length=6, only_digits=True):
     """
     Generate a time-based OTP using SHA-256 hashing algorithm.
 
     Args:
     secret_key (str): Secret key used for hashing.
     interval (int): Time interval in seconds for OTP validity. Default is 120 seconds (2 minutes).
-    length (int): Length of OTP. Default is 6 (6 digits). Maximum 8 digits.
+    length (int): Length of OTP. Default is 6 (6 digits). Maximum 8 digits. Minimum 4 digits.
+    only_digits (bool): If True, only digits are used for OTP. Default is True.
 
     Returns:
     str: Generated OTP.
     """
-    length = length if length < 9 else 6
+    # Validating the length. Maximum 8 is allowed. 6 will assign if count gave more than 8.
+    length = length if 9 > length > 3 else 6
+
+    # Getting current time based on interval. This will use for generate one OTP based on secret at particular interval.
     current_time = int(time.time() / interval)
+
+    # Generating hash
     otp_hash = hashlib.sha256((str(current_time) + secret_key).encode()).hexdigest()
+
+    # Getting only digits from hash
     otp_numeric = ''.join(char for char in otp_hash if char.isdigit())
+
+    # Digit or mixed OTP based on only_digits
     otp = otp_numeric[:length] if only_digits else otp_hash[:length]  # Return the first 6 characters as the OTP
+    
     return otp
```

### Comparing `ownotp-0.1.0/ownotp.egg-info/PKG-INFO` & `ownotp-0.1.1/ownotp.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ownotp
-Version: 0.1.0
+Version: 0.1.1
 Summary: Generate a time-based OTP using SHA-256 hashing algorithm
 Home-page: https://github.com/karthiksenniyappan/ownotp
 Author: karthiksenniyappan
 Author-email: karthiksenniyappan76@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,18 @@
 print(otp)
 ```
 To change interval time pass the value in seconds.
 ```python
 from ownotp.otp import generate_otp
 otp = generate_otp('your_own_secret', interval=120)
 ```
-To get 7 or 8 length otp.
+
+To generate different length OTP.
+
+Note: Minium 4 and Maximum 8 length will support. If condition not satisfied default length will take to generate OTP.
 ```python
 from ownotp.otp import generate_otp
 otp = generate_otp('your_own_secret', length=7)
 ```
 To get hashed OTP. Mixed of char and numbers
 ```python
 from ownotp.otp import generate_otp
```

### Comparing `ownotp-0.1.0/setup.py` & `ownotp-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='ownotp',
-    version='0.1.0',
+    version='0.1.1',
     author='karthiksenniyappan',
     author_email='karthiksenniyappan76@gmail.com',
     description="Generate a time-based OTP using SHA-256 hashing algorithm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/karthiksenniyappan/ownotp",
     packages=['ownotp'],
```

### Comparing `ownotp-0.1.0/tests/test_otp.py` & `ownotp-0.1.1/tests/test_otp.py`

 * *Files identical despite different names*

