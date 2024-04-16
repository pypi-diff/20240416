# Comparing `tmp/cvxpy-1.4.2.tar.gz` & `tmp/cvxpy-1.4.3-cp312-cp312-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxpy-1.4.2.tar", last modified: Fri Jan 19 02:18:12 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

