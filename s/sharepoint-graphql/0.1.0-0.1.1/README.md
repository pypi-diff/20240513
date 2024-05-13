# Comparing `tmp/sharepoint_graphql-0.1.0.tar.gz` & `tmp/sharepoint_graphql-0.1.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharepoint_graphql-0.1.0.tar", last modified: Sun May 12 18:28:19 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

