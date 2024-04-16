# Comparing `tmp/scratchattach-1.6.2.tar.gz` & `tmp/scratchattach-1.6.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchattach-1.6.2.tar", last modified: Tue Feb 27 20:09:06 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

