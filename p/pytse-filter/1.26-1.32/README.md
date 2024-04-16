# Comparing `tmp/pytse_filter-1.26.tar.gz` & `tmp/pytse_filter-1.32-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytse_filter-1.26.tar", last modified: Wed Apr 10 09:54:32 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

