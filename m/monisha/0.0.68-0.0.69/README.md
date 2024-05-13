# Comparing `tmp/monisha-0.0.68.tar.gz` & `tmp/monisha-0.0.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monisha-0.0.68.tar", last modified: Sun May 12 11:28:35 2024, max compression
+gzip compressed data, was "monisha-0.0.69.tar", last modified: Mon May 13 17:33:31 2024, max compression
```

## Comparing `monisha-0.0.68.tar` & `monisha-0.0.69.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:28:35.221935 monisha-0.0.68/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-12 11:28:31.000000 monisha-0.0.68/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:28:35.213935 monisha-0.0.68/Monisha/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:28:35.217935 monisha-0.0.68/Monisha/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function01.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function02.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function03.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function04.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function05.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function06.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function07.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function08.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function09.py
--rw-r--r--   0 runner    (1001) docker     (127)    60666 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function10.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function11.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function12.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function14.py
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function15.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function16.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function17.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function18.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function19.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function20.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:28:35.221935 monisha-0.0.68/Monisha/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/scripts/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/scripts/es.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/scripts/eu.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-12 11:28:35.221935 monisha-0.0.68/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-12 11:28:31.000000 monisha-0.0.68/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:28:35.221935 monisha-0.0.68/monisha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-12 11:28:35.000000 monisha-0.0.68/monisha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-12 11:28:35.000000 monisha-0.0.68/monisha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 11:28:35.000000 monisha-0.0.68/monisha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-12 11:28:35.000000 monisha-0.0.68/monisha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-12 11:28:35.000000 monisha-0.0.68/monisha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 11:28:35.221935 monisha-0.0.68/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-12 11:28:31.000000 monisha-0.0.68/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:33:31.839548 monisha-0.0.69/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-13 17:33:27.000000 monisha-0.0.69/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:33:31.831548 monisha-0.0.69/Monisha/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-13 17:33:27.000000 monisha-0.0.69/Monisha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:33:31.835548 monisha-0.0.69/Monisha/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-13 17:33:27.000000 monisha-0.0.69/Monisha/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-13 17:33:27.000000 monisha-0.0.69/Monisha/functions/function01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-13 17:33:27.000000 monisha-0.0.69/Monisha/functions/function02.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-13 17:33:27.000000 monisha-0.0.69/Monisha/functions/function03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-13 17:33:27.000000 monisha-0.0.69/Monisha/functions/function04.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-13 17:33:27.000000 monisha-0.0.69/Monisha/functions/function05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-13 17:33:27.000000 monisha-0.0.69/Monisha/functions/function06.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-13 17:33:27.000000 monisha-0.0.69/Monisha/functions/function07.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-13 17:33:27.000000 monisha-0.0.69/Monisha/functions/function08.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-13 17:33:27.000000 monisha-0.0.69/Monisha/functions/function09.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60666 2024-05-13 17:33:27.000000 monisha-0.0.69/Monisha/functions/function10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-13 17:33:27.000000 monisha-0.0.69/Monisha/functions/function11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-13 17:33:27.000000 monisha-0.0.69/Monisha/functions/function12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-13 17:33:27.000000 monisha-0.0.69/Monisha/functions/function13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-13 17:33:27.000000 monisha-0.0.69/Monisha/functions/function14.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-13 17:33:27.000000 monisha-0.0.69/Monisha/functions/function15.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-13 17:33:27.000000 monisha-0.0.69/Monisha/functions/function16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-13 17:33:27.000000 monisha-0.0.69/Monisha/functions/function17.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-13 17:33:27.000000 monisha-0.0.69/Monisha/functions/function18.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-13 17:33:27.000000 monisha-0.0.69/Monisha/functions/function19.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-13 17:33:27.000000 monisha-0.0.69/Monisha/functions/function20.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:33:31.835548 monisha-0.0.69/Monisha/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-13 17:33:27.000000 monisha-0.0.69/Monisha/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-13 17:33:27.000000 monisha-0.0.69/Monisha/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-13 17:33:27.000000 monisha-0.0.69/Monisha/scripts/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-13 17:33:27.000000 monisha-0.0.69/Monisha/scripts/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-13 17:33:27.000000 monisha-0.0.69/Monisha/scripts/eu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-13 17:33:31.839548 monisha-0.0.69/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-13 17:33:27.000000 monisha-0.0.69/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:33:31.839548 monisha-0.0.69/monisha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-13 17:33:31.000000 monisha-0.0.69/monisha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-13 17:33:31.000000 monisha-0.0.69/monisha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 17:33:31.000000 monisha-0.0.69/monisha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-13 17:33:31.000000 monisha-0.0.69/monisha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-13 17:33:31.000000 monisha-0.0.69/monisha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 17:33:31.839548 monisha-0.0.69/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-13 17:33:27.000000 monisha-0.0.69/setup.py
```

### Comparing `monisha-0.0.68/LICENSE` & `monisha-0.0.69/LICENSE`

 * *Files identical despite different names*

### Comparing `monisha-0.0.68/Monisha/__init__.py` & `monisha-0.0.69/Monisha/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 appname = "monisha"
-version = "0.0.68"
+version = "0.0.69"
 
 install = ["hachoir",
            "requests",
            "beautifulsoup4"]
 
 DATA01 = "clintonabrahamc@gmail.com"
 DATA02 = ['Natural Language :: English',
```

### Comparing `monisha-0.0.68/Monisha/functions/__init__.py` & `monisha-0.0.69/Monisha/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.68/Monisha/functions/function01.py` & `monisha-0.0.69/Monisha/functions/function01.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.68/Monisha/functions/function02.py` & `monisha-0.0.69/Monisha/functions/function02.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.68/Monisha/functions/function03.py` & `monisha-0.0.69/Monisha/functions/function03.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.68/Monisha/functions/function04.py` & `monisha-0.0.69/Monisha/functions/function04.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.68/Monisha/functions/function06.py` & `monisha-0.0.69/Monisha/functions/function06.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.68/Monisha/functions/function07.py` & `monisha-0.0.69/Monisha/functions/function07.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.68/Monisha/functions/function10.py` & `monisha-0.0.69/Monisha/functions/function10.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.68/Monisha/functions/function14.py` & `monisha-0.0.69/Monisha/functions/function14.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.68/Monisha/functions/function15.py` & `monisha-0.0.69/Monisha/functions/function15.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.68/Monisha/functions/function16.py` & `monisha-0.0.69/Monisha/functions/function16.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.68/Monisha/functions/function17.py` & `monisha-0.0.69/Monisha/functions/function17.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         moonus = mainos + extension if extension else mainos
         return moonus
 
 #=========================================================================
 
     async def get02(filename):
         nameas = str(filename)
-        cnames = os.path.splitext(nameas)[0]
+        finame = os.path.splitext(nameas)[0]
         exexon = os.path.splitext(nameas)[1]
         exoexo = exexon if exexon else ".tmp"
         moonus = finame if finame else "Unknown"
         return SMessages(filename=moonus, extension=exoexo)
 
 #=========================================================================
```

### Comparing `monisha-0.0.68/Monisha/functions/function18.py` & `monisha-0.0.69/Monisha/functions/function18.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.68/Monisha/functions/function19.py` & `monisha-0.0.69/Monisha/functions/function19.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.68/Monisha/functions/function20.py` & `monisha-0.0.69/Monisha/functions/function20.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.68/Monisha/scripts/es.py` & `monisha-0.0.69/Monisha/scripts/es.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.68/PKG-INFO` & `monisha-0.0.69/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.68
+Version: 0.0.69
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.68 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.69 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
```

### Comparing `monisha-0.0.68/monisha.egg-info/PKG-INFO` & `monisha-0.0.69/monisha.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.68
+Version: 0.0.69
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.68 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.69 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
```

### Comparing `monisha-0.0.68/monisha.egg-info/SOURCES.txt` & `monisha-0.0.69/monisha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monisha-0.0.68/setup.py` & `monisha-0.0.69/setup.py`

 * *Files identical despite different names*

