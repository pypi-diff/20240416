# Comparing `tmp/nb_time-1.3.tar.gz` & `tmp/nb_time-1.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\nb_time-1.3.tar", last modified: Wed Mar 20 10:01:46 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

