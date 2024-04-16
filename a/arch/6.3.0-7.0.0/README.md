# Comparing `tmp/arch-6.3.0.tar.gz` & `tmp/arch-7.0.0-cp39-cp39-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arch-6.3.0.tar", last modified: Fri Jan  5 08:37:23 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

