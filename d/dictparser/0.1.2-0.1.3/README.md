# Comparing `tmp/dictparser-0.1.2-py3-none-any.whl.zip` & `tmp/dictparser-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5342 bytes, number of entries: 9
+Zip file size: 5370 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      575 b- defN 24-May-09 22:01 dictparser/__init__.py
 -rw-r--r--  2.0 unx     7257 b- defN 24-May-12 15:31 dictparser/engine.py
 -rw-r--r--  2.0 unx     1375 b- defN 24-May-09 21:44 dictparser/pylint.py
 -rw-r--r--  2.0 unx      377 b- defN 24-May-09 21:50 dictparser/types.py
--rw-r--r--  2.0 unx      891 b- defN 24-May-12 15:32 dictparser-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      571 b- defN 24-May-12 15:32 dictparser-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-12 15:32 dictparser-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-May-12 15:32 dictparser-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      706 b- defN 24-May-12 15:32 dictparser-0.1.2.dist-info/RECORD
-9 files, 11855 bytes uncompressed, 4126 bytes compressed:  65.2%
+-rw-r--r--  2.0 unx      891 b- defN 24-May-12 15:53 dictparser-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      623 b- defN 24-May-12 15:53 dictparser-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-12 15:53 dictparser-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-May-12 15:53 dictparser-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      706 b- defN 24-May-12 15:53 dictparser-0.1.3.dist-info/RECORD
+9 files, 11907 bytes uncompressed, 4154 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: dictparser/pylint.py
 Comment: 
 
 Filename: dictparser/types.py
 Comment: 
 
-Filename: dictparser-0.1.2.dist-info/LICENSE
+Filename: dictparser-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: dictparser-0.1.2.dist-info/METADATA
+Filename: dictparser-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: dictparser-0.1.2.dist-info/WHEEL
+Filename: dictparser-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: dictparser-0.1.2.dist-info/top_level.txt
+Filename: dictparser-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: dictparser-0.1.2.dist-info/RECORD
+Filename: dictparser-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `dictparser-0.1.2.dist-info/LICENSE` & `dictparser-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dictparser-0.1.2.dist-info/METADATA` & `dictparser-0.1.3.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: dictparser
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Class serialization/deserializeation library
 Project-URL: Homepage, https://github.com/tgoncalves87/dictparser
 Project-URL: Issues, https://github.com/tgoncalves87/dictparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT No Attribution License (MIT-0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml
+Requires-Dist: dataclasses ; python_version < "3.7"
 
 A Class serialization/deserializeation library
```

