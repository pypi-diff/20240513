# Comparing `tmp/dnfjson-0.2.0rc1.tar.gz` & `tmp/dnfjson-0.3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnfjson-0.2.0rc1.tar", last modified: Tue Nov 16 11:27:28 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

