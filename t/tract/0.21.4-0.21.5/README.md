# Comparing `tmp/tract-0.21.4.tar.gz` & `tmp/tract-0.21.5-pp37-pypy37_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tract-0.21.4.tar", last modified: Tue Apr 23 11:20:54 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

