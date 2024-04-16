# Comparing `tmp/MyRecursion-0.0.1-py3-none-any.whl.zip` & `tmp/MyRecursion-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1328 bytes, number of entries: 5
--rw-r--r--  2.0 unx      160 b- defN 24-Apr-10 07:05 myrecursion/recursion.py
--rw-r--r--  2.0 unx      200 b- defN 24-Apr-10 07:08 MyRecursion-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 07:08 MyRecursion-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-Apr-10 07:08 MyRecursion-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      393 b- defN 24-Apr-10 07:08 MyRecursion-0.0.1.dist-info/RECORD
-5 files, 857 bytes uncompressed, 590 bytes compressed:  31.2%
+Zip file size: 1341 bytes, number of entries: 5
+-rw-r--r--  2.0 unx      161 b- defN 24-Apr-16 03:07 myrecursion/recursion.py
+-rw-r--r--  2.0 unx      217 b- defN 24-Apr-16 03:09 MyRecursion-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 03:09 MyRecursion-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-Apr-16 03:09 MyRecursion-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      393 b- defN 24-Apr-16 03:09 MyRecursion-0.0.3.dist-info/RECORD
+5 files, 875 bytes uncompressed, 603 bytes compressed:  31.1%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: myrecursion/recursion.py
 Comment: 
 
-Filename: MyRecursion-0.0.1.dist-info/METADATA
+Filename: MyRecursion-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: MyRecursion-0.0.1.dist-info/WHEEL
+Filename: MyRecursion-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: MyRecursion-0.0.1.dist-info/top_level.txt
+Filename: MyRecursion-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: MyRecursion-0.0.1.dist-info/RECORD
+Filename: MyRecursion-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## myrecursion/recursion.py

```diff
@@ -1,7 +1,8 @@
+
 def factorial(n):
   if n == 1: return 1
   return n * factorial(n-1)
 
 def fibonachi(n):
   if n == 1 or n == 2: return 1
   return fibonachi(n-2) + fibonachi(n-1)
```

