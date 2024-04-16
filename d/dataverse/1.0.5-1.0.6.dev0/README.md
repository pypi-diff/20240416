# Comparing `tmp/dataverse-1.0.5.tar.gz` & `tmp/dataverse-1.0.6.dev0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataverse-1.0.5.tar", last modified: Thu Apr  4 08:18:45 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

