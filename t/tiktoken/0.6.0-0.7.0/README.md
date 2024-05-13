# Comparing `tmp/tiktoken-0.6.0.tar.gz` & `tmp/tiktoken-0.7.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiktoken-0.6.0.tar", last modified: Fri Feb  9 05:53:29 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

