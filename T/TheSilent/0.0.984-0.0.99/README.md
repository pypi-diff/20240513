# Comparing `tmp/thesilent-0.0.984.tar.gz` & `tmp/TheSilent-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thesilent-0.0.984.tar", last modified: Mon May 13 11:04:38 2024, max compression
+gzip compressed data, was "TheSilent-0.0.99.tar", last modified: Mon Jan  9 15:25:09 2023, max compression
```

## Comparing `thesilent-0.0.984.tar` & `TheSilent-0.0.99.tar`

### file list

```diff
@@ -1,23 +1,35 @@
-drwxr-xr-x   0 linux     (1000) linux     (1000)        0 2024-05-13 11:04:38.235991 thesilent-0.0.984/
--rw-r--r--   0 linux     (1000) linux     (1000)      569 2024-05-13 11:04:38.235991 thesilent-0.0.984/PKG-INFO
--rw-rw-r--   0 linux     (1000) linux     (1000)       70 2024-05-13 02:24:43.000000 thesilent-0.0.984/README.md
--rw-rw-r--   0 linux     (1000) linux     (1000)      650 2024-05-13 11:02:48.000000 thesilent-0.0.984/pyproject.toml
--rw-r--r--   0 linux     (1000) linux     (1000)       38 2024-05-13 11:04:38.235991 thesilent-0.0.984/setup.cfg
-drwxr-xr-x   0 linux     (1000) linux     (1000)        0 2024-05-13 11:04:38.235991 thesilent-0.0.984/src/
-drwxr-xr-x   0 linux     (1000) linux     (1000)        0 2024-05-13 11:04:38.235991 thesilent-0.0.984/src/TheSilent/
--rw-rw-r--   0 linux     (1000) linux     (1000)        0 2024-05-13 02:24:43.000000 thesilent-0.0.984/src/TheSilent/__init__.py
--rw-rw-r--   0 linux     (1000) linux     (1000)      167 2024-05-13 02:24:43.000000 thesilent-0.0.984/src/TheSilent/clear.py
--rw-rw-r--   0 linux     (1000) linux     (1000)     5422 2024-05-13 11:04:03.000000 thesilent-0.0.984/src/TheSilent/cobra.py
--rw-rw-r--   0 linux     (1000) linux     (1000)     1468 2024-05-13 02:24:43.000000 thesilent-0.0.984/src/TheSilent/evasion.py
--rw-rw-r--   0 linux     (1000) linux     (1000)     2206 2024-05-13 02:24:43.000000 thesilent-0.0.984/src/TheSilent/fingerprint_scanner.py
--rw-rw-r--   0 linux     (1000) linux     (1000)    80583 2024-05-13 02:24:43.000000 thesilent-0.0.984/src/TheSilent/http_scanners.py
--rw-rw-r--   0 linux     (1000) linux     (1000)     2668 2024-05-13 02:24:43.000000 thesilent-0.0.984/src/TheSilent/kitten_crawler.py
--rw-rw-r--   0 linux     (1000) linux     (1000)    10985 2024-05-13 02:24:43.000000 thesilent-0.0.984/src/TheSilent/parser.py
--rw-rw-r--   0 linux     (1000) linux     (1000)    23369 2024-05-13 02:24:43.000000 thesilent-0.0.984/src/TheSilent/payloads.py
--rw-rw-r--   0 linux     (1000) linux     (1000)     5234 2024-05-13 02:24:43.000000 thesilent-0.0.984/src/TheSilent/puppy_requests.py
--rw-rw-r--   0 linux     (1000) linux     (1000)      646 2024-05-13 02:24:43.000000 thesilent-0.0.984/src/TheSilent/return_user_agent.py
-drwxr-xr-x   0 linux     (1000) linux     (1000)        0 2024-05-13 11:04:38.235991 thesilent-0.0.984/src/TheSilent.egg-info/
--rw-r--r--   0 linux     (1000) linux     (1000)      569 2024-05-13 11:04:38.000000 thesilent-0.0.984/src/TheSilent.egg-info/PKG-INFO
--rw-r--r--   0 linux     (1000) linux     (1000)      486 2024-05-13 11:04:38.000000 thesilent-0.0.984/src/TheSilent.egg-info/SOURCES.txt
--rw-r--r--   0 linux     (1000) linux     (1000)        1 2024-05-13 11:04:38.000000 thesilent-0.0.984/src/TheSilent.egg-info/dependency_links.txt
--rw-r--r--   0 linux     (1000) linux     (1000)       10 2024-05-13 11:04:38.000000 thesilent-0.0.984/src/TheSilent.egg-info/top_level.txt
+drwxr-xr-x   0 linux     (1000) linux     (1000)        0 2023-01-09 15:25:09.786667 TheSilent-0.0.99/
+-rw-r--r--   0 linux     (1000) linux     (1000)      643 2023-01-09 15:25:09.786667 TheSilent-0.0.99/PKG-INFO
+-rw-r--r--   0 linux     (1000) linux     (1000)      101 2023-01-06 01:24:13.000000 TheSilent-0.0.99/README.md
+-rw-r--r--   0 linux     (1000) linux     (1000)      735 2023-01-09 15:05:42.000000 TheSilent-0.0.99/pyproject.toml
+-rw-r--r--   0 linux     (1000) linux     (1000)       38 2023-01-09 15:25:09.786667 TheSilent-0.0.99/setup.cfg
+drwxr-xr-x   0 linux     (1000) linux     (1000)        0 2023-01-09 15:25:09.777667 TheSilent-0.0.99/src/
+drwxr-xr-x   0 linux     (1000) linux     (1000)        0 2023-01-09 15:25:09.785667 TheSilent-0.0.99/src/TheSilent/
+-rw-r--r--   0 linux     (1000) linux     (1000)      762 2023-01-08 22:12:06.000000 TheSilent-0.0.99/src/TheSilent/TheSilent.py
+-rw-r--r--   0 linux     (1000) linux     (1000)        0 2023-01-06 01:24:13.000000 TheSilent-0.0.99/src/TheSilent/__init__.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     1324 2023-01-08 22:09:59.000000 TheSilent-0.0.99/src/TheSilent/arp_void.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     6976 2023-01-08 22:10:13.000000 TheSilent-0.0.99/src/TheSilent/brute_force_hash.py
+-rw-r--r--   0 linux     (1000) linux     (1000)      167 2023-01-08 20:46:15.000000 TheSilent-0.0.99/src/TheSilent/clear.py
+-rw-r--r--   0 linux     (1000) linux     (1000)    17412 2023-01-08 22:10:20.000000 TheSilent-0.0.99/src/TheSilent/dictionary_hash.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     7894 2023-01-08 22:10:23.000000 TheSilent-0.0.99/src/TheSilent/email_scanner.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     1247 2023-01-08 21:08:17.000000 TheSilent-0.0.99/src/TheSilent/form_scanner.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     1812 2023-01-08 22:10:31.000000 TheSilent-0.0.99/src/TheSilent/ftp_cracker.py
+-rw-r--r--   0 linux     (1000) linux     (1000)      781 2023-01-08 22:10:35.000000 TheSilent-0.0.99/src/TheSilent/hex_viewer.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     9590 2023-01-09 15:24:17.000000 TheSilent-0.0.99/src/TheSilent/link_scanner.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     5982 2023-01-08 22:10:47.000000 TheSilent-0.0.99/src/TheSilent/login_cracker.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     5074 2023-01-08 22:10:51.000000 TheSilent-0.0.99/src/TheSilent/nmap.py
+-rw-r--r--   0 linux     (1000) linux     (1000)    19506 2023-01-08 22:10:56.000000 TheSilent-0.0.99/src/TheSilent/packet_sniffer.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     2541 2023-01-08 22:11:02.000000 TheSilent-0.0.99/src/TheSilent/port_scanner.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     1833 2023-01-08 22:11:07.000000 TheSilent-0.0.99/src/TheSilent/secure_overwrite.py
+-rw-r--r--   0 linux     (1000) linux     (1000)      800 2023-01-08 22:11:13.000000 TheSilent-0.0.99/src/TheSilent/security_scanner.py
+-rw-r--r--   0 linux     (1000) linux     (1000)      831 2023-01-08 22:11:18.000000 TheSilent-0.0.99/src/TheSilent/source_code_viewer.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     9363 2023-01-08 22:11:23.000000 TheSilent-0.0.99/src/TheSilent/sql_injection_scanner.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     1307 2023-01-08 22:11:27.000000 TheSilent-0.0.99/src/TheSilent/subdomain_scanner.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     1366 2023-01-08 22:11:32.000000 TheSilent-0.0.99/src/TheSilent/subdomain_takeover.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     7212 2023-01-09 15:19:41.000000 TheSilent-0.0.99/src/TheSilent/xss_scanner.py
+drwxr-xr-x   0 linux     (1000) linux     (1000)        0 2023-01-09 15:25:09.786667 TheSilent-0.0.99/src/TheSilent.egg-info/
+-rw-r--r--   0 linux     (1000) linux     (1000)      643 2023-01-09 15:25:09.000000 TheSilent-0.0.99/src/TheSilent.egg-info/PKG-INFO
+-rw-r--r--   0 linux     (1000) linux     (1000)      883 2023-01-09 15:25:09.000000 TheSilent-0.0.99/src/TheSilent.egg-info/SOURCES.txt
+-rw-r--r--   0 linux     (1000) linux     (1000)        1 2023-01-09 15:25:09.000000 TheSilent-0.0.99/src/TheSilent.egg-info/dependency_links.txt
+-rw-r--r--   0 linux     (1000) linux     (1000)       23 2023-01-09 15:25:09.000000 TheSilent-0.0.99/src/TheSilent.egg-info/requires.txt
+-rw-r--r--   0 linux     (1000) linux     (1000)       10 2023-01-09 15:25:09.000000 TheSilent-0.0.99/src/TheSilent.egg-info/top_level.txt
```

### Comparing `thesilent-0.0.984/PKG-INFO` & `TheSilent-0.0.99/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: TheSilent
-Version: 0.0.984
-Summary: TheSilent contains free and open source hacking and osint tools!
-Author: Michael Mueller
+Version: 0.0.99
+Summary: Python penetration testing, osint, and digital forensics multi tool!
+Author-email: Michael Mueller <michael.j.mueller.pro@gmail.com>
 Project-URL: Homepage, https://github.com/Invizabel/The-Silent
 Project-URL: Bug Tracker, https://github.com/Invizabel/The-Silent/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-﻿# TheSilent contains free and open source hacking and osint tools!
+# The-Silent
+# Python penetration testing, osint, and digital forensics multi tool!
+# In Development
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `thesilent-0.0.984/pyproject.toml` & `TheSilent-0.0.99/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TheSilent"
-version = "0.0.984"
+version = "0.0.99"
 authors = [
-  { name="Michael Mueller"},
+  { name="Michael Mueller", email="michael.j.mueller.pro@gmail.com" },
 ]
-description = "TheSilent contains free and open source hacking and osint tools!"
+description = "Python penetration testing, osint, and digital forensics multi tool!"
 readme = "README.md"
 license = { file="LICENSE.txt" }
-requires-python = ">=3.8"
+requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-    ]
+    "numpy",
+    "requests",
+    "urllib3",
+]
 
 [project.urls]
 "Homepage" = "https://github.com/Invizabel/The-Silent"
 "Bug Tracker" = "https://github.com/Invizabel/The-Silent/issues"
```

### Comparing `thesilent-0.0.984/src/TheSilent.egg-info/PKG-INFO` & `TheSilent-0.0.99/src/TheSilent.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: TheSilent
-Version: 0.0.984
-Summary: TheSilent contains free and open source hacking and osint tools!
-Author: Michael Mueller
+Version: 0.0.99
+Summary: Python penetration testing, osint, and digital forensics multi tool!
+Author-email: Michael Mueller <michael.j.mueller.pro@gmail.com>
 Project-URL: Homepage, https://github.com/Invizabel/The-Silent
 Project-URL: Bug Tracker, https://github.com/Invizabel/The-Silent/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-﻿# TheSilent contains free and open source hacking and osint tools!
+# The-Silent
+# Python penetration testing, osint, and digital forensics multi tool!
+# In Development
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

