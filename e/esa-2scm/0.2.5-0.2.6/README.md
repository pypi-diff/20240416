# Comparing `tmp/esa-2scm-0.2.5.tar.gz` & `tmp/esa-2scm-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esa-2scm-0.2.5.tar", last modified: Sun Apr 14 19:17:04 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
