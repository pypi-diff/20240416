# Comparing `tmp/lakeapi2sql-0.8.0.tar.gz` & `tmp/lakeapi2sql-0.8.1-cp310-abi3-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

