# Comparing `tmp/iSwitch-1.0.1.tar.gz` & `tmp/iSwitch-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iSwitch-1.0.1.tar", last modified: Mon May 13 18:39:53 2024, max compression
+gzip compressed data, was "iSwitch-1.0.2.tar", last modified: Mon May 13 19:11:20 2024, max compression
```

## Comparing `iSwitch-1.0.1.tar` & `iSwitch-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-13 18:39:53.434595 iSwitch-1.0.1/
--rw-r--r--   0 mac        (501) staff       (20)     1057 2024-05-11 18:46:44.000000 iSwitch-1.0.1/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)     4880 2024-05-13 18:39:53.434070 iSwitch-1.0.1/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     4528 2024-05-13 17:13:43.000000 iSwitch-1.0.1/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-13 18:39:53.433508 iSwitch-1.0.1/iSwitch.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     4880 2024-05-13 18:39:53.000000 iSwitch-1.0.1/iSwitch.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      276 2024-05-13 18:39:53.000000 iSwitch-1.0.1/iSwitch.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2024-05-13 18:39:53.000000 iSwitch-1.0.1/iSwitch.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       26 2024-05-13 18:39:53.000000 iSwitch-1.0.1/iSwitch.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        8 2024-05-13 18:39:53.000000 iSwitch-1.0.1/iSwitch.egg-info/top_level.txt
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-13 18:39:53.432675 iSwitch-1.0.1/iswitch/
--rw-r--r--   0 mac        (501) staff       (20)      328 2024-05-12 10:01:33.000000 iSwitch-1.0.1/iswitch/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     6560 2024-05-13 16:12:36.000000 iSwitch-1.0.1/iswitch/_client.py
--rw-r--r--   0 mac        (501) staff       (20)     7677 2024-05-12 22:15:34.000000 iSwitch-1.0.1/iswitch/_services.py
--rw-r--r--   0 mac        (501) staff       (20)     7360 2024-05-13 16:09:25.000000 iSwitch-1.0.1/iswitch/_types.py
--rw-r--r--   0 mac        (501) staff       (20)     3247 2024-05-12 10:42:22.000000 iSwitch-1.0.1/iswitch/_utils.py
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-05-13 18:39:53.434706 iSwitch-1.0.1/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      617 2024-05-13 18:39:45.000000 iSwitch-1.0.1/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-13 19:11:20.302528 iSwitch-1.0.2/
+-rw-r--r--   0 mac        (501) staff       (20)     1057 2024-05-11 18:46:44.000000 iSwitch-1.0.2/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)     5119 2024-05-13 19:11:20.301714 iSwitch-1.0.2/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     4767 2024-05-13 19:10:59.000000 iSwitch-1.0.2/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-13 19:11:20.300674 iSwitch-1.0.2/iSwitch.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     5119 2024-05-13 19:11:19.000000 iSwitch-1.0.2/iSwitch.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      276 2024-05-13 19:11:19.000000 iSwitch-1.0.2/iSwitch.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2024-05-13 19:11:19.000000 iSwitch-1.0.2/iSwitch.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       26 2024-05-13 19:11:19.000000 iSwitch-1.0.2/iSwitch.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        8 2024-05-13 19:11:19.000000 iSwitch-1.0.2/iSwitch.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-13 19:11:20.280686 iSwitch-1.0.2/iswitch/
+-rw-r--r--   0 mac        (501) staff       (20)      328 2024-05-12 10:01:33.000000 iSwitch-1.0.2/iswitch/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     6560 2024-05-13 16:12:36.000000 iSwitch-1.0.2/iswitch/_client.py
+-rw-r--r--   0 mac        (501) staff       (20)     7677 2024-05-12 22:15:34.000000 iSwitch-1.0.2/iswitch/_services.py
+-rw-r--r--   0 mac        (501) staff       (20)     7360 2024-05-13 16:09:25.000000 iSwitch-1.0.2/iswitch/_types.py
+-rw-r--r--   0 mac        (501) staff       (20)     3247 2024-05-12 10:42:22.000000 iSwitch-1.0.2/iswitch/_utils.py
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-05-13 19:11:20.302725 iSwitch-1.0.2/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      617 2024-05-13 19:11:14.000000 iSwitch-1.0.2/setup.py
```

### Comparing `iSwitch-1.0.1/LICENSE` & `iSwitch-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iSwitch-1.0.1/PKG-INFO` & `iSwitch-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iSwitch
-Version: 1.0.1
+Version: 1.0.2
 Summary: SwitchPay Python SDK for AllDotPy internal use. 
 Home-page: https://github.com/AllDotPy/iSwitch.git
 Author: #Einswilli
 Author-email: einswilligoeh@email.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
@@ -198,7 +198,13 @@
         }
     }
 )
 
 # Do Authentication
 response = Client.authenticate()        # Will raise a ResponseError with response message.
 ```
+<br>
+<p align = 'center'>
+    <img src='dotpy_blue_transparent.png?raw=true' height = '60'></img>
+</p>
+<p align = 'center'>Made with ❤️ By DotPy</p>
+<!-- <p height='60' align = 'center'>© 2024 DotPy, Inc. All rights reserved.</p> -->
```

### Comparing `iSwitch-1.0.1/README.md` & `iSwitch-1.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -184,8 +184,14 @@
             'password':'WRONG-PASSWORD',
         }
     }
 )
 
 # Do Authentication
 response = Client.authenticate()        # Will raise a ResponseError with response message.
-```
+```
+<br>
+<p align = 'center'>
+    <img src='dotpy_blue_transparent.png?raw=true' height = '60'></img>
+</p>
+<p align = 'center'>Made with ❤️ By DotPy</p>
+<!-- <p height='60' align = 'center'>© 2024 DotPy, Inc. All rights reserved.</p> -->
```

### Comparing `iSwitch-1.0.1/iSwitch.egg-info/PKG-INFO` & `iSwitch-1.0.2/iSwitch.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iSwitch
-Version: 1.0.1
+Version: 1.0.2
 Summary: SwitchPay Python SDK for AllDotPy internal use. 
 Home-page: https://github.com/AllDotPy/iSwitch.git
 Author: #Einswilli
 Author-email: einswilligoeh@email.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
@@ -198,7 +198,13 @@
         }
     }
 )
 
 # Do Authentication
 response = Client.authenticate()        # Will raise a ResponseError with response message.
 ```
+<br>
+<p align = 'center'>
+    <img src='dotpy_blue_transparent.png?raw=true' height = '60'></img>
+</p>
+<p align = 'center'>Made with ❤️ By DotPy</p>
+<!-- <p height='60' align = 'center'>© 2024 DotPy, Inc. All rights reserved.</p> -->
```

### Comparing `iSwitch-1.0.1/iswitch/_client.py` & `iSwitch-1.0.2/iswitch/_client.py`

 * *Files identical despite different names*

### Comparing `iSwitch-1.0.1/iswitch/_services.py` & `iSwitch-1.0.2/iswitch/_services.py`

 * *Files identical despite different names*

### Comparing `iSwitch-1.0.1/iswitch/_types.py` & `iSwitch-1.0.2/iswitch/_types.py`

 * *Files identical despite different names*

### Comparing `iSwitch-1.0.1/iswitch/_utils.py` & `iSwitch-1.0.2/iswitch/_utils.py`

 * *Files identical despite different names*

### Comparing `iSwitch-1.0.1/setup.py` & `iSwitch-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # LOADING DOCUMENTATION
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name = 'iSwitch',
-    version = '1.0.1',
+    version = '1.0.2',
     packages = find_packages(),
     install_requires = [
         'httpx',
         'simplejson',
         'colorlog'
     ],
     long_description=long_description,
```

