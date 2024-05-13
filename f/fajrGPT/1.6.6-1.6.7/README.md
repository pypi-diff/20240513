# Comparing `tmp/fajrGPT-1.6.6.tar.gz` & `tmp/fajrGPT-1.6.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fajrGPT-1.6.6.tar", last modified: Wed Jan  3 12:53:05 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

