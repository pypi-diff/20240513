# Comparing `tmp/qcfinancial-0.8.2-cp39-cp39-win_amd64.whl.zip` & `tmp/qcfinancial-0.8.3-cp39-cp39-macosx_14_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 525580 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat  1613312 b- defN 24-Apr-14 12:43 qcfinancial.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      588 b- defN 24-Apr-14 12:43 qcfinancial-0.8.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-14 12:43 qcfinancial-0.8.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-14 12:43 qcfinancial-0.8.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      404 b- defN 24-Apr-14 12:43 qcfinancial-0.8.2.dist-info/RECORD
-5 files, 1614416 bytes uncompressed, 524830 bytes compressed:  67.5%
+Zip file size: 584350 bytes, number of entries: 5
+-rwxr-xr-x  2.0 unx  1759344 b- defN 24-May-13 17:46 qcfinancial.cpython-39-darwin.so
+-rw-r--r--  2.0 unx      568 b- defN 24-May-13 17:46 qcfinancial-0.8.3.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 24-May-13 17:46 qcfinancial-0.8.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-May-13 17:46 qcfinancial-0.8.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      406 b- defN 24-May-13 17:46 qcfinancial-0.8.3.dist-info/RECORD
+5 files, 1760438 bytes uncompressed, 583596 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: qcfinancial.cp39-win_amd64.pyd
+Filename: qcfinancial.cpython-39-darwin.so
 Comment: 
 
-Filename: qcfinancial-0.8.2.dist-info/METADATA
+Filename: qcfinancial-0.8.3.dist-info/METADATA
 Comment: 
 
-Filename: qcfinancial-0.8.2.dist-info/WHEEL
+Filename: qcfinancial-0.8.3.dist-info/WHEEL
 Comment: 
 
-Filename: qcfinancial-0.8.2.dist-info/top_level.txt
+Filename: qcfinancial-0.8.3.dist-info/top_level.txt
 Comment: 
 
-Filename: qcfinancial-0.8.2.dist-info/RECORD
+Filename: qcfinancial-0.8.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `qcfinancial-0.8.2.dist-info/METADATA` & `qcfinancial-0.8.3.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1
-Name: qcfinancial
-Version: 0.8.2
-Summary: A Library for Valuation of Linear Interest Rate and FX Derivatives
-Home-page: UNKNOWN
-Author: Alvaro Diaz V.
-Author-email: alvaro@efaa.cl
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Requires-Dist: pytest >=6.0 ; extra == 'test'
-
-# Derivative Valuation Engine
-Librería para la valorización de derivados lineales de tasa de interés y tipo de cambio.
-
-Library for the valuation of linear interest rate and fx rate derivatives.
-
-
+Metadata-Version: 2.1
+Name: qcfinancial
+Version: 0.8.3
+Summary: A Library for Valuation of Linear Interest Rate and FX Derivatives
+Home-page: UNKNOWN
+Author: Alvaro Diaz V.
+Author-email: alvaro@efaa.cl
+License: UNKNOWN
+Platform: UNKNOWN
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Requires-Dist: pytest >=6.0 ; extra == 'test'
+
+# Derivative Valuation Engine
+Librería para la valorización de derivados lineales de tasa de interés y tipo de cambio.
+
+Library for the valuation of linear interest rate and fx rate derivatives.
+
+
```

