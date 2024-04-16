# Comparing `tmp/dall_alsa-0.0.1.tar.gz` & `tmp/Dall_ALSA-0.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dall_alsa-0.0.1.tar", last modified: Tue Apr 16 12:03:18 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

