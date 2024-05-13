# Comparing `tmp/yuag-0.0.69.tar.gz` & `tmp/yuag-0.0.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuag-0.0.69.tar", last modified: Wed May  8 20:56:15 2024, max compression
+gzip compressed data, was "yuag-0.0.70.tar", last modified: Mon May 13 12:00:34 2024, max compression
```

## Comparing `yuag-0.0.69.tar` & `yuag-0.0.70.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 20:56:15.486237 yuag-0.0.69/
--rw-rw-rw-   0        0        0       52 2024-05-08 20:56:15.480245 yuag-0.0.69/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-08 20:56:15.486237 yuag-0.0.69/setup.cfg
--rw-rw-rw-   0        0        0      249 2024-05-08 20:56:07.000000 yuag-0.0.69/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 20:56:15.455256 yuag-0.0.69/yuag/
--rw-rw-rw-   0        0        0     2853 2024-05-08 20:47:05.000000 yuag-0.0.69/yuag/__init__.py
--rw-rw-rw-   0        0        0    43228 2024-05-08 20:49:00.000000 yuag-0.0.69/yuag/yuag.py
-drwxrwxrwx   0        0        0        0 2024-05-08 20:56:15.478242 yuag-0.0.69/yuag.egg-info/
--rw-rw-rw-   0        0        0       52 2024-05-08 20:56:15.000000 yuag-0.0.69/yuag.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2024-05-08 20:56:15.000000 yuag-0.0.69/yuag.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 20:56:15.000000 yuag-0.0.69/yuag.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-08 20:56:15.000000 yuag-0.0.69/yuag.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 12:00:34.861420 yuag-0.0.70/
+-rw-rw-rw-   0        0        0       52 2024-05-13 12:00:34.859418 yuag-0.0.70/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-13 12:00:34.861420 yuag-0.0.70/setup.cfg
+-rw-rw-rw-   0        0        0      249 2024-05-13 11:59:29.000000 yuag-0.0.70/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 12:00:34.846426 yuag-0.0.70/yuag/
+-rw-rw-rw-   0        0        0     2873 2024-05-13 11:58:51.000000 yuag-0.0.70/yuag/__init__.py
+-rw-rw-rw-   0        0        0    44696 2024-05-13 11:58:39.000000 yuag-0.0.70/yuag/yuag.py
+drwxrwxrwx   0        0        0        0 2024-05-13 12:00:34.858420 yuag-0.0.70/yuag.egg-info/
+-rw-rw-rw-   0        0        0       52 2024-05-13 12:00:34.000000 yuag-0.0.70/yuag.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      150 2024-05-13 12:00:34.000000 yuag-0.0.70/yuag.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 12:00:34.000000 yuag-0.0.70/yuag.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-13 12:00:34.000000 yuag-0.0.70/yuag.egg-info/top_level.txt
```

### Comparing `yuag-0.0.69/yuag/__init__.py` & `yuag-0.0.70/yuag/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 -----------------
 ```
 wait()
 clear()
 detect_lang()
 rangeNum()
 python_path()
+check_lib_status()
 ```
 \n\n
 
 دوال للملفات:
 -----------------
 ```
 filesIn()
```

### Comparing `yuag-0.0.69/yuag/yuag.py` & `yuag-0.0.70/yuag/yuag.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,21 +78,64 @@
 
         return res
 
 def python_path():
     """
     اللهم صل على سيدنا محمد ﷺ\n
     ارجاع قيمة مسار بايثون، مثل:
-    `C:\Python\python.exe`
+    `C:\\Python\\python.exe`
     """
     
     import sys
 
     return sys.executable
 
+def check_lib_status(lib_to_check: str|list, installed_lib_return = "installed", builtIn_return = "built-in", notFound_return = "not found"):
+    """
+    اللهم صل على سيدنا محمد ﷺ\n
+    التأكد من وجود أي مكتبة أو أكثر من مكتبة في بايثون\n\n
+
+    مكتبة واحدة:
+    ------------
+    ```
+    lib_to_check = "إسم المكتبة"
+    ==> "installed"
+    ```
+
+    أكثر من مكتبة:
+    ------------
+    ```
+    lib_to_check = ["lib1", "lib2", "lib3"]
+    ==>
+    [
+        {"lib name": "lib1", "lib status": "not found"},
+        {"lib name": "lib2", "lib status": "installed"},
+        {"lib name": "lib3", "lib status": "built-in"}
+    ]
+    ```
+    """
+
+    py_path = python_path().split("python.exe")[0] + "Lib" # C\Python312\Lib
+
+    def check_one(lib):
+        if lib in filesIn(py_path + "\\site-packages"): # تم تنزيل المكتبة
+            return installed_lib_return
+        elif lib in filesIn(py_path): # المكتبة أساسية في بايثون
+            return builtIn_return
+        else: # المكتبة غير موجودة
+            return notFound_return
+    
+    if type(lib_to_check) == str:
+        return check_one(lib_to_check)
+    elif type(lib_to_check) == list:
+        res = []
+        for lib in lib_to_check: res.append({"lib name": lib, "lib status": check_one(lib)})
+        
+        return res
+
 # file defs
 def filesIn(folder_path: str = "./"):
     import os
 
     return os.listdir(folder_path)
 
 def rename_file(file_path: str, new_name: str):
```

