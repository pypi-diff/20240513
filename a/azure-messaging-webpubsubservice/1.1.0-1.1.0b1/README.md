# Comparing `tmp/azure-messaging-webpubsubservice-1.1.0.tar.gz` & `tmp/azure-messaging-webpubsubservice-1.1.0b1.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-messaging-webpubsubservice-1.1.0.tar", last modified: Mon May 13 07:59:35 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

