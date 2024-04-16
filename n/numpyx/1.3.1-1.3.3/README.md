# Comparing `tmp/numpyx-1.3.1.tar.gz` & `tmp/numpyx-1.3.3-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpyx-1.3.1.tar", last modified: Wed Apr 12 12:29:20 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

