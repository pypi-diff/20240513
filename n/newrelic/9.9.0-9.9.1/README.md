# Comparing `tmp/newrelic-9.9.0.tar.gz` & `tmp/newrelic-9.9.1-cp37-cp37m-musllinux_1_1_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newrelic-9.9.0.tar", last modified: Thu Apr 18 22:50:51 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

