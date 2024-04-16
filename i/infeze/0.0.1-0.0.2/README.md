# Comparing `tmp/infeze-0.0.1-py3-none-any.whl.zip` & `tmp/infeze-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,10 @@
-Zip file size: 1479 bytes, number of entries: 6
+Zip file size: 6781 bytes, number of entries: 8
 -rw-rw-r--  2.0 unx       75 b- defN 24-Apr-10 23:42 infeze/__init__.py
--rw-rw-r--  2.0 unx       23 b- defN 24-Mar-11 07:57 infeze/_version.py
--rw-rw-r--  2.0 unx      249 b- defN 24-Apr-10 23:49 infeze-0.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-10 23:49 infeze-0.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 24-Apr-10 23:49 infeze-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      438 b- defN 24-Apr-10 23:49 infeze-0.0.1.dist-info/RECORD
-6 files, 884 bytes uncompressed, 681 bytes compressed:  23.0%
+-rw-rw-r--  2.0 unx       23 b- defN 24-Apr-16 06:13 infeze/_version.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-16 06:07 infeze/py.typed
+-rw-rw-r--  2.0 unx    25172 b- defN 24-Apr-16 02:32 infeze/backports/langchain/tongyi.py
+-rw-rw-r--  2.0 unx      322 b- defN 24-Apr-16 06:15 infeze-0.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-16 06:15 infeze-0.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 24-Apr-16 06:15 infeze-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      601 b- defN 24-Apr-16 06:15 infeze-0.0.2.dist-info/RECORD
+8 files, 26292 bytes uncompressed, 5729 bytes compressed:  78.2%
```

## zipnote {}

```diff
@@ -1,19 +1,25 @@
 Filename: infeze/__init__.py
 Comment: 
 
 Filename: infeze/_version.py
 Comment: 
 
-Filename: infeze-0.0.1.dist-info/METADATA
+Filename: infeze/py.typed
 Comment: 
 
-Filename: infeze-0.0.1.dist-info/WHEEL
+Filename: infeze/backports/langchain/tongyi.py
 Comment: 
 
-Filename: infeze-0.0.1.dist-info/top_level.txt
+Filename: infeze-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: infeze-0.0.1.dist-info/RECORD
+Filename: infeze-0.0.2.dist-info/WHEEL
+Comment: 
+
+Filename: infeze-0.0.2.dist-info/top_level.txt
+Comment: 
+
+Filename: infeze-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## infeze/_version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.0.1"
+__version__ = "0.0.2"
```

