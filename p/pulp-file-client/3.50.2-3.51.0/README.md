# Comparing `tmp/pulp_file-client-3.50.2.tar.gz` & `tmp/pulp_file_client-3.51.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp_file-client-3.50.2.tar", last modified: Tue Apr  9 18:35:44 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

