# Comparing `tmp/opentelemetry_instrumentation_qdrant-0.17.4.tar.gz` & `tmp/opentelemetry_instrumentation_qdrant-0.17.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry_instrumentation_qdrant-0.17.4.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

