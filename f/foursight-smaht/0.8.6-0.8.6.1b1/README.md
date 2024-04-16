# Comparing `tmp/foursight_smaht-0.8.6.tar.gz` & `tmp/foursight_smaht-0.8.6.1b1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_smaht-0.8.6.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

