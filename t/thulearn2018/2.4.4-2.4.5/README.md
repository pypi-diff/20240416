# Comparing `tmp/thulearn2018-2.4.4.tar.gz` & `tmp/thulearn2018-2.4.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thulearn2018-2.4.4.tar", last modified: Tue Apr 16 09:02:15 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

