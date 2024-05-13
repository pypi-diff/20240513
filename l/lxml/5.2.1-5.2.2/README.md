# Comparing `tmp/lxml-5.2.1.tar.gz` & `tmp/lxml-5.2.2-cp310-cp310-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lxml-5.2.1.tar", last modified: Tue Apr  2 08:30:29 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

