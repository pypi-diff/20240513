# Comparing `tmp/algokit_client_generator-1.1.4b2-py3-none-any.whl.zip` & `tmp/algokit_client_generator-1.1.4b3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -4,13 +4,13 @@
 -rw-r--r--  2.0 unx     2550 b- defN 80-Jan-01 00:00 algokit_client_generator/cli.py
 -rw-r--r--  2.0 unx     3208 b- defN 80-Jan-01 00:00 algokit_client_generator/document.py
 -rw-r--r--  2.0 unx    37388 b- defN 80-Jan-01 00:00 algokit_client_generator/generator.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_client_generator/py.typed
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_client_generator/spec.py
 -rw-r--r--  2.0 unx     4507 b- defN 80-Jan-01 00:00 algokit_client_generator/utils.py
 -rw-r--r--  2.0 unx      995 b- defN 80-Jan-01 00:00 algokit_client_generator/writer.py
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_client_generator-1.1.4b2.dist-info/LICENSE
--rw-r--r--  2.0 unx     4800 b- defN 80-Jan-01 00:00 algokit_client_generator-1.1.4b2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_client_generator-1.1.4b2.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 80-Jan-01 00:00 algokit_client_generator-1.1.4b2.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1298 b- defN 16-Jan-01 00:00 algokit_client_generator-1.1.4b2.dist-info/RECORD
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_client_generator-1.1.4b3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4800 b- defN 80-Jan-01 00:00 algokit_client_generator-1.1.4b3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_client_generator-1.1.4b3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       67 b- defN 80-Jan-01 00:00 algokit_client_generator-1.1.4b3.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1298 b- defN 16-Jan-01 00:00 algokit_client_generator-1.1.4b3.dist-info/RECORD
 14 files, 63588 bytes uncompressed, 16325 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: algokit_client_generator/utils.py
 Comment: 
 
 Filename: algokit_client_generator/writer.py
 Comment: 
 
-Filename: algokit_client_generator-1.1.4b2.dist-info/LICENSE
+Filename: algokit_client_generator-1.1.4b3.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_client_generator-1.1.4b2.dist-info/METADATA
+Filename: algokit_client_generator-1.1.4b3.dist-info/METADATA
 Comment: 
 
-Filename: algokit_client_generator-1.1.4b2.dist-info/WHEEL
+Filename: algokit_client_generator-1.1.4b3.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_client_generator-1.1.4b2.dist-info/entry_points.txt
+Filename: algokit_client_generator-1.1.4b3.dist-info/entry_points.txt
 Comment: 
 
-Filename: algokit_client_generator-1.1.4b2.dist-info/RECORD
+Filename: algokit_client_generator-1.1.4b3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `algokit_client_generator-1.1.4b2.dist-info/LICENSE` & `algokit_client_generator-1.1.4b3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_client_generator-1.1.4b2.dist-info/METADATA` & `algokit_client_generator-1.1.4b3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: algokit-client-generator
-Version: 1.1.4b2
+Version: 1.1.4b3
 Summary: Algorand typed client Generator
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: algokit-utils (==2.2.2)
+Requires-Dist: algokit-utils (==2.3.0)
 Description-Content-Type: text/markdown
 
 # AlgoKit Python client generator 
 
 This project generates a type-safe smart contract client in Python for the Algorand Blockchain that wraps the 
 [application client](https://algorandfoundation.github.io/algokit-utils-py/html/apidocs/algokit_utils/algokit_utils.html#algokit_utils.ApplicationClient) in 
 [AlgoKit Utils](https://github.com/algorandfoundation/algokit-utils-py). It does this by reading an [ARC-0032](https://github.com/algorandfoundation/ARCs/blob/main/ARCs/arc-0032.md) application spec file.
```

## Comparing `algokit_client_generator-1.1.4b2.dist-info/RECORD` & `algokit_client_generator-1.1.4b3.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -3,12 +3,12 @@
 algokit_client_generator/cli.py,sha256=XwuLZUhym9ntuHRIayPZsfv2-vTSbEykt3evF7EdVq4,2550
 algokit_client_generator/document.py,sha256=kzoBGG842Zm-XsWFyRe5HOcCJs79CWiKy9RB_blqTE8,3208
 algokit_client_generator/generator.py,sha256=PSArIiBV0Hc-HO9rEnxdycZZ4ebNGrywTCEKxe0LiIs,37388
 algokit_client_generator/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 algokit_client_generator/spec.py,sha256=apgef1qcRbm2akT1ogF23d6HnSncPwnLdrqaVzJAKmo,7466
 algokit_client_generator/utils.py,sha256=XseV85NgM_yW-g3q8Ss4Lzg2v-iHIkHwlc1pxtQIffI,4507
 algokit_client_generator/writer.py,sha256=CynBYWnHlO1E4Ubcpjvzq8kRcgfYCpnO3nEAslBEr-s,995
-algokit_client_generator-1.1.4b2.dist-info/LICENSE,sha256=fkgfhUgPPyK1aS4tK9QOFRl5fWtuFEtkKx4zPQNT1bQ,1076
-algokit_client_generator-1.1.4b2.dist-info/METADATA,sha256=4FuNLF14e_ljccp95AySVcy9tpz4vcw_mAgQBIPiIyc,4800
-algokit_client_generator-1.1.4b2.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-algokit_client_generator-1.1.4b2.dist-info/entry_points.txt,sha256=RnsJToDSJC_LyXvGqv7LNpgkqipw1C7eQsc0bke--A0,67
-algokit_client_generator-1.1.4b2.dist-info/RECORD,,
+algokit_client_generator-1.1.4b3.dist-info/LICENSE,sha256=fkgfhUgPPyK1aS4tK9QOFRl5fWtuFEtkKx4zPQNT1bQ,1076
+algokit_client_generator-1.1.4b3.dist-info/METADATA,sha256=kG4MQtb3RtfO-TbxMNxAQPJ9VSGQ9uMomR5C81lZBlA,4800
+algokit_client_generator-1.1.4b3.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+algokit_client_generator-1.1.4b3.dist-info/entry_points.txt,sha256=RnsJToDSJC_LyXvGqv7LNpgkqipw1C7eQsc0bke--A0,67
+algokit_client_generator-1.1.4b3.dist-info/RECORD,,
```

