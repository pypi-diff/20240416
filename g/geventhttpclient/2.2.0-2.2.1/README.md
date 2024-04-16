# Comparing `tmp/geventhttpclient-2.2.0.tar.gz` & `tmp/geventhttpclient-2.2.1-cp311-cp311-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geventhttpclient-2.2.0.tar", last modified: Fri Apr 12 15:24:34 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

