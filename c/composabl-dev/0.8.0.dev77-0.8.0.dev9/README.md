# Comparing `tmp/composabl_dev-0.8.0.dev77-cp311-cp311-macosx_11_0_arm64.whl.zip` & `tmp/composabl_dev-0.8.0.dev9-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,13 @@
-Zip file size: 25416 bytes, number of entries: 8
--rwxr-xr-x  2.0 unx    55832 b- defN 24-May-13 04:34 composabl/core.cpython-311-darwin.so
--rwxr-xr-x  2.0 unx    56016 b- defN 24-May-13 04:34 composabl/__init__.cpython-311-darwin.so
--rwxr-xr-x  2.0 unx    55816 b- defN 24-May-13 04:34 composabl/ray.cpython-311-darwin.so
--rw-rw-r--  2.0 unx      747 b- defN 24-May-13 04:34 composabl_dev-0.8.0.dev77.dist-info/RECORD
--rw-r--r--  2.0 unx      110 b- defN 24-May-13 04:34 composabl_dev-0.8.0.dev77.dist-info/WHEEL
--rw-r--r--  2.0 unx       56 b- defN 24-May-13 04:34 composabl_dev-0.8.0.dev77.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 24-May-13 04:34 composabl_dev-0.8.0.dev77.dist-info/top_level.txt
--rw-r--r--  2.0 unx     1829 b- defN 24-May-13 04:34 composabl_dev-0.8.0.dev77.dist-info/METADATA
-8 files, 170416 bytes uncompressed, 24108 bytes compressed:  85.9%
+Zip file size: 106007 bytes, number of entries: 11
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-02 14:40 composabl/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-02 14:40 composabl_dev.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-02 14:40 composabl_dev-0.8.0.dev9.dist-info/
+-rwxr-xr-x  2.0 unx    93456 b- defN 24-Apr-02 14:40 composabl/ray.cpython-311-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx    93456 b- defN 24-Apr-02 14:40 composabl/core.cpython-311-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx    94456 b- defN 24-Apr-02 14:40 composabl/__init__.cpython-311-x86_64-linux-gnu.so
+-rw-rw-r--  2.0 unx      772 b- defN 24-Apr-02 14:40 composabl_dev-0.8.0.dev9.dist-info/RECORD
+-rw-r--r--  2.0 unx       56 b- defN 24-Apr-02 14:40 composabl_dev-0.8.0.dev9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx     1825 b- defN 24-Apr-02 14:40 composabl_dev-0.8.0.dev9.dist-info/METADATA
+-rw-r--r--  2.0 unx      225 b- defN 24-Apr-02 14:40 composabl_dev-0.8.0.dev9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-Apr-02 14:40 composabl_dev-0.8.0.dev9.dist-info/top_level.txt
+11 files, 284256 bytes uncompressed, 104293 bytes compressed:  63.3%
```

## zipnote {}

```diff
@@ -1,25 +1,34 @@
-Filename: composabl/core.cpython-311-darwin.so
+Filename: composabl/
 Comment: 
 
-Filename: composabl/__init__.cpython-311-darwin.so
+Filename: composabl_dev.libs/
 Comment: 
 
-Filename: composabl/ray.cpython-311-darwin.so
+Filename: composabl_dev-0.8.0.dev9.dist-info/
 Comment: 
 
-Filename: composabl_dev-0.8.0.dev77.dist-info/RECORD
+Filename: composabl/ray.cpython-311-x86_64-linux-gnu.so
 Comment: 
 
-Filename: composabl_dev-0.8.0.dev77.dist-info/WHEEL
+Filename: composabl/core.cpython-311-x86_64-linux-gnu.so
 Comment: 
 
-Filename: composabl_dev-0.8.0.dev77.dist-info/entry_points.txt
+Filename: composabl/__init__.cpython-311-x86_64-linux-gnu.so
 Comment: 
 
-Filename: composabl_dev-0.8.0.dev77.dist-info/top_level.txt
+Filename: composabl_dev-0.8.0.dev9.dist-info/RECORD
 Comment: 
 
-Filename: composabl_dev-0.8.0.dev77.dist-info/METADATA
+Filename: composabl_dev-0.8.0.dev9.dist-info/entry_points.txt
+Comment: 
+
+Filename: composabl_dev-0.8.0.dev9.dist-info/METADATA
+Comment: 
+
+Filename: composabl_dev-0.8.0.dev9.dist-info/WHEEL
+Comment: 
+
+Filename: composabl_dev-0.8.0.dev9.dist-info/top_level.txt
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## Comparing `composabl_dev-0.8.0.dev77.dist-info/METADATA` & `composabl_dev-0.8.0.dev9.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: composabl-dev
-Version: 0.8.0.dev77
-Summary: a distributed trainer to be able to train agents across a cluster of machines
+Version: 0.8.0.dev9
+Summary: a distributed runtime to be able to train agents across a cluster of machines
 Author-email: Xavier Geerinck <xavier@composabl.io>, Hunter Park <hunter@composabl.io>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: composabl-core-dev >=0.8.0.dev77
-Requires-Dist: composabl-train-dev >=0.8.0.dev77
-Requires-Dist: composabl-cli-dev >=0.8.0.dev77
+Requires-Dist: composabl-core-dev >=0.8.0.dev9
+Requires-Dist: composabl-train-dev >=0.8.0.dev9
+Requires-Dist: composabl-cli-dev >=0.8.0.dev9
 
 # Composabl
 
 Composabl helps you build Autonomous Agents! Through an easy SDK you get access to outscaled simulator training tools.
 
 ## Licenses / Seats
```

