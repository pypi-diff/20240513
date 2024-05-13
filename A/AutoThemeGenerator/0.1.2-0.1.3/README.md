# Comparing `tmp/autothemegenerator-0.1.2.tar.gz` & `tmp/AutoThemeGenerator-0.1.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autothemegenerator-0.1.2.tar", last modified: Wed May  8 14:51:03 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

