# Comparing `tmp/destinelab-0.2.tar.gz` & `tmp/destinelab-0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "destinelab-0.2.tar", last modified: Wed May  8 09:10:04 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

