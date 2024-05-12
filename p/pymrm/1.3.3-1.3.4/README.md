# Comparing `tmp/pymrm-1.3.3.tar.gz` & `tmp/pymrm-1.3.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymrm-1.3.3.tar", last modified: Wed May  8 20:40:06 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

