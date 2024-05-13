# Comparing `tmp/bazel_runfiles-0.31.0-py3-none-any.whl.zip` & `tmp/bazel_runfiles-0.32.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 7177 bytes, number of entries: 5
+Zip file size: 7176 bytes, number of entries: 5
 -rwxrwxrwx  2.0 unx      628 b- defN 80-Jan-01 00:00 runfiles/__init__.py
 -rwxrwxrwx  2.0 unx    15175 b- defN 80-Jan-01 00:00 runfiles/runfiles.py
--rwxrwxrwx  2.0 unx       91 b- defN 80-Jan-01 00:00 bazel_runfiles-0.31.0.dist-info/WHEEL
--rwxrwxrwx  2.0 unx     2641 b- defN 80-Jan-01 00:00 bazel_runfiles-0.31.0.dist-info/METADATA
--rwxrwxrwx  2.0 unx      384 b- defN 80-Jan-01 00:00 bazel_runfiles-0.31.0.dist-info/RECORD
-5 files, 18919 bytes uncompressed, 6465 bytes compressed:  65.8%
+-rwxrwxrwx  2.0 unx       91 b- defN 80-Jan-01 00:00 bazel_runfiles-0.32.0.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx     2641 b- defN 80-Jan-01 00:00 bazel_runfiles-0.32.0.dist-info/METADATA
+-rwxrwxrwx  2.0 unx      384 b- defN 80-Jan-01 00:00 bazel_runfiles-0.32.0.dist-info/RECORD
+5 files, 18919 bytes uncompressed, 6464 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: runfiles/__init__.py
 Comment: 
 
 Filename: runfiles/runfiles.py
 Comment: 
 
-Filename: bazel_runfiles-0.31.0.dist-info/WHEEL
+Filename: bazel_runfiles-0.32.0.dist-info/WHEEL
 Comment: 
 
-Filename: bazel_runfiles-0.31.0.dist-info/METADATA
+Filename: bazel_runfiles-0.32.0.dist-info/METADATA
 Comment: 
 
-Filename: bazel_runfiles-0.31.0.dist-info/RECORD
+Filename: bazel_runfiles-0.32.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `bazel_runfiles-0.31.0.dist-info/METADATA` & `bazel_runfiles-0.32.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: bazel_runfiles
 Home-page: https://github.com/bazelbuild/rules_python
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
-Version: 0.31.0
+Version: 0.32.0
 
 # bazel-runfiles library
 
 This is a Bazel Runfiles lookup library for Bazel-built Python binaries and tests.
 
 Learn about runfiles: read [Runfiles guide](https://bazel.build/extending/rules#runfiles)
 or watch [Fabian's BazelCon talk](https://www.youtube.com/watch?v=5NbgUMH1OGo).
```

