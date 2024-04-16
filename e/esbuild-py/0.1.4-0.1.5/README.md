# Comparing `tmp/esbuild_py-0.1.4.tar.gz` & `tmp/esbuild_py-0.1.5-cp39-cp39-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esbuild_py-0.1.4.tar", last modified: Mon Apr 15 17:34:32 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

