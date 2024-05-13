# Comparing `tmp/wlkata_mirobot_Virtual-1.1.3.tar.gz` & `tmp/wlkata_mirobot_Virtual-1.1.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wlkata_mirobot_Virtual-1.1.3.tar", last modified: Mon May 13 02:50:17 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

