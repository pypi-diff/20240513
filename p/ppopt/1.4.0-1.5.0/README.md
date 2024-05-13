# Comparing `tmp/ppopt-1.4.0.tar.gz` & `tmp/ppopt-1.5.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ppopt-1.4.0.tar", last modified: Wed Jan 24 22:53:51 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

