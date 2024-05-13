# Comparing `tmp/modern_colorthief-0.1.2.tar.gz` & `tmp/modern_colorthief-0.1.3-pp39-pypy39_pp73-manylinux_2_17_armv7l.manylinux2014_armv7l.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modern_colorthief-0.1.2.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

