# Comparing `tmp/open2fa-1.4.1-py3-none-any.whl.zip` & `tmp/open2fa-1.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 20678 bytes, number of entries: 17
+Zip file size: 20672 bytes, number of entries: 17
 -rw-r--r--  2.0 unx      113 b- defN 24-Feb-12 01:03 open2fa/__init__.py
 -rw-r--r--  2.0 unx    10069 b- defN 24-Mar-25 23:32 open2fa/cli.py
 -rw-r--r--  2.0 unx     4747 b- defN 24-Apr-27 23:38 open2fa/cli_utils.py
 -rw-r--r--  2.0 unx     4334 b- defN 24-Mar-24 22:21 open2fa/common.py
 -rw-r--r--  2.0 unx      660 b- defN 24-Apr-11 22:49 open2fa/config.py
 -rw-r--r--  2.0 unx      923 b- defN 24-Mar-21 19:32 open2fa/ex.py
 -rw-r--r--  2.0 unx    17991 b- defN 24-Apr-28 22:53 open2fa/main.py
 -rw-r--r--  2.0 unx     1814 b- defN 24-Apr-28 22:58 open2fa/msgs.py
 -rw-r--r--  2.0 unx     2248 b- defN 24-Apr-16 18:10 open2fa/totp.py
 -rw-r--r--  2.0 unx     2139 b- defN 24-Mar-21 19:36 open2fa/utils.py
--rw-r--r--  2.0 unx       22 b- defN 24-May-03 02:32 open2fa/version.py
--rw-r--r--  2.0 unx     1068 b- defN 24-May-03 02:34 open2fa-1.4.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    11097 b- defN 24-May-03 02:34 open2fa-1.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-03 02:34 open2fa-1.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 24-May-03 02:34 open2fa-1.4.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 24-May-03 02:34 open2fa-1.4.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1284 b- defN 24-May-03 02:34 open2fa-1.4.1.dist-info/RECORD
-17 files, 58661 bytes uncompressed, 18608 bytes compressed:  68.3%
+-rw-r--r--  2.0 unx       22 b- defN 24-May-13 05:50 open2fa/version.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-13 08:19 open2fa-1.4.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    11088 b- defN 24-May-13 08:19 open2fa-1.4.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-13 08:19 open2fa-1.4.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 24-May-13 08:19 open2fa-1.4.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 24-May-13 08:19 open2fa-1.4.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1284 b- defN 24-May-13 08:19 open2fa-1.4.2.dist-info/RECORD
+17 files, 58652 bytes uncompressed, 18602 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: open2fa/utils.py
 Comment: 
 
 Filename: open2fa/version.py
 Comment: 
 
-Filename: open2fa-1.4.1.dist-info/LICENSE
+Filename: open2fa-1.4.2.dist-info/LICENSE
 Comment: 
 
-Filename: open2fa-1.4.1.dist-info/METADATA
+Filename: open2fa-1.4.2.dist-info/METADATA
 Comment: 
 
-Filename: open2fa-1.4.1.dist-info/WHEEL
+Filename: open2fa-1.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: open2fa-1.4.1.dist-info/entry_points.txt
+Filename: open2fa-1.4.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: open2fa-1.4.1.dist-info/top_level.txt
+Filename: open2fa-1.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: open2fa-1.4.1.dist-info/RECORD
+Filename: open2fa-1.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## open2fa/version.py

```diff
@@ -1 +1 @@
-__version__ = "1.4.1"
+__version__ = "1.4.2"
```

## Comparing `open2fa-1.4.1.dist-info/LICENSE` & `open2fa-1.4.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `open2fa-1.4.1.dist-info/METADATA` & `open2fa-1.4.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open2fa
-Version: 1.4.1
+Version: 1.4.2
 Summary: A 2FA CLI tool for generating 2FA codes using TOTP secrets, with an optional SECURE remote api, and an optional web ui enabling 2FA code generation from any device
 Author-email: Cary Carter <ccarterdev@gmail.com>
 Project-URL: Homepage, https://open2fa.liberfy.ai
 Project-URL: Repository, https://github.com/cc-d/open2fa
 Project-URL: Issues, https://github.com/cc-d/open2fa/issues
 Project-URL: Server, https://github.com/cc-d/open2fa-server
 Project-URL: Documentation, https://github.com/cc-d/open2fa
@@ -17,17 +17,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
-Requires-Dist: logfunc <=2.4.3
+Requires-Dist: logfunc <3.0.0
 Requires-Dist: cryptography <=41.0.7
-Requires-Dist: pyshared <1.6.0,>=1.5.8
+Requires-Dist: pyshared <1.6.0
 Requires-Dist: base58 ==2.1.1
 Provides-Extra: dev
 Requires-Dist: pytest ; extra == 'dev'
 Requires-Dist: pytest-cov ; extra == 'dev'
 Requires-Dist: pytest-mock ; extra == 'dev'
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: isort ; extra == 'dev'
```

