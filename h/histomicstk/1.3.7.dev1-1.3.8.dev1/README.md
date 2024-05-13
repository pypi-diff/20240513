# Comparing `tmp/histomicstk-1.3.7.dev1.tar.gz` & `tmp/histomicstk-1.3.8.dev1-cp311-cp311-macosx_10_12_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histomicstk-1.3.7.dev1.tar", last modified: Thu Apr 11 17:32:54 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

