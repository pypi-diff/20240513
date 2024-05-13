# Comparing `tmp/touchpy-0.0.4-py3-none-any.whl.zip` & `tmp/touchpy-0.0.6-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,13 @@
-Zip file size: 1243679 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat   680448 b- defN 24-May-08 18:51 touchpy/TouchEngine.dll
--rw-rw-rw-  2.0 fat       47 b- defN 24-May-13 03:31 touchpy/__init__.py
--rw-rw-rw-  2.0 fat   526848 b- defN 22-Sep-21 18:15 touchpy/cudart64_110.dll
--rw-rw-rw-  2.0 fat   141312 b- defN 24-Apr-06 17:45 touchpy/fmt.dll
--rw-rw-rw-  2.0 fat   258048 b- defN 24-Apr-06 17:57 touchpy/spdlog.dll
--rw-rw-rw-  2.0 fat   920064 b- defN 24-May-13 02:39 touchpy/touchpy.cp310-win_amd64.pyd
--rw-rw-rw-  2.0 fat   920064 b- defN 24-May-13 02:35 touchpy/touchpy.cp311-win_amd64.pyd
--rw-rw-rw-  2.0 fat   919040 b- defN 24-May-13 02:35 touchpy/touchpy.cp312-win_amd64.pyd
--rw-rw-rw-  2.0 fat   920576 b- defN 24-May-13 02:34 touchpy/touchpy.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     4695 b- defN 24-May-13 03:32 touchpy-0.0.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6470 b- defN 24-May-13 03:32 touchpy-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-13 03:32 touchpy-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-May-13 03:32 touchpy-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1150 b- defN 24-May-13 03:32 touchpy-0.0.4.dist-info/RECORD
-14 files, 5298862 bytes uncompressed, 1241799 bytes compressed:  76.6%
+Zip file size: 771171 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat   680448 b- defN 24-May-08 18:51 touchpy-0.0.6.data/purelib/touchpy/TouchEngine.dll
+-rw-rw-rw-  2.0 fat       47 b- defN 24-May-13 17:21 touchpy-0.0.6.data/purelib/touchpy/__init__.py
+-rw-rw-rw-  2.0 fat   526848 b- defN 22-Sep-21 18:15 touchpy-0.0.6.data/purelib/touchpy/cudart64_110.dll
+-rw-rw-rw-  2.0 fat   141312 b- defN 24-Apr-06 17:45 touchpy-0.0.6.data/purelib/touchpy/fmt.dll
+-rw-rw-rw-  2.0 fat   258048 b- defN 24-Apr-06 17:57 touchpy-0.0.6.data/purelib/touchpy/spdlog.dll
+-rw-rw-rw-  2.0 fat   920576 b- defN 24-May-13 20:52 touchpy-0.0.6.data/purelib/touchpy/touchpy.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     4695 b- defN 24-May-13 20:52 touchpy-0.0.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6421 b- defN 24-May-13 20:52 touchpy-0.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-May-13 20:52 touchpy-0.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 24-May-13 20:52 touchpy-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1031 b- defN 24-May-13 20:52 touchpy-0.0.6.dist-info/RECORD
+11 files, 2539534 bytes uncompressed, 769405 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -1,43 +1,34 @@
-Filename: touchpy/TouchEngine.dll
+Filename: touchpy-0.0.6.data/purelib/touchpy/TouchEngine.dll
 Comment: 
 
-Filename: touchpy/__init__.py
+Filename: touchpy-0.0.6.data/purelib/touchpy/__init__.py
 Comment: 
 
-Filename: touchpy/cudart64_110.dll
+Filename: touchpy-0.0.6.data/purelib/touchpy/cudart64_110.dll
 Comment: 
 
-Filename: touchpy/fmt.dll
+Filename: touchpy-0.0.6.data/purelib/touchpy/fmt.dll
 Comment: 
 
-Filename: touchpy/spdlog.dll
+Filename: touchpy-0.0.6.data/purelib/touchpy/spdlog.dll
 Comment: 
 
-Filename: touchpy/touchpy.cp310-win_amd64.pyd
+Filename: touchpy-0.0.6.data/purelib/touchpy/touchpy.cp39-win_amd64.pyd
 Comment: 
 
-Filename: touchpy/touchpy.cp311-win_amd64.pyd
+Filename: touchpy-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: touchpy/touchpy.cp312-win_amd64.pyd
+Filename: touchpy-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: touchpy/touchpy.cp39-win_amd64.pyd
+Filename: touchpy-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: touchpy-0.0.4.dist-info/LICENSE
+Filename: touchpy-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: touchpy-0.0.4.dist-info/METADATA
-Comment: 
-
-Filename: touchpy-0.0.4.dist-info/WHEEL
-Comment: 
-
-Filename: touchpy-0.0.4.dist-info/top_level.txt
-Comment: 
-
-Filename: touchpy-0.0.4.dist-info/RECORD
+Filename: touchpy-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `touchpy/TouchEngine.dll` & `touchpy-0.0.6.data/purelib/touchpy/TouchEngine.dll`

 * *Files identical despite different names*

## Comparing `touchpy/cudart64_110.dll` & `touchpy-0.0.6.data/purelib/touchpy/cudart64_110.dll`

 * *Files identical despite different names*

## Comparing `touchpy/fmt.dll` & `touchpy-0.0.6.data/purelib/touchpy/fmt.dll`

 * *Files identical despite different names*

## Comparing `touchpy/spdlog.dll` & `touchpy-0.0.6.data/purelib/touchpy/spdlog.dll`

 * *Files identical despite different names*

## Comparing `touchpy-0.0.4.dist-info/LICENSE` & `touchpy-0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `touchpy-0.0.4.dist-info/METADATA` & `touchpy-0.0.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: touchpy
-Version: 0.0.4
+Version: 0.0.6
 Summary: Tools to make working with TouchDesigner and Python easier.
 Author-email: Keith Lostracco <keith@intentdev.io>, Idzard Kwadijk <idzard@intentdev.io>
 License: # PolyForm Noncommercial License 1.0.0
         
         <https://polyformproject.org/licenses/noncommercial/1.0.0>
         
         ## Acceptance
@@ -131,15 +131,14 @@
         
         **Your licenses** are all the licenses granted to you for the
         software under these terms.
         
         **Use** means anything you do with the software requiring one
         of your licenses.
         
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: <3.13,>=3.9
 Description-Content-Type: text/markdown
```

