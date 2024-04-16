# Comparing `tmp/lenstr-0.1-py3-none-any.whl.zip` & `tmp/lenstr-0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 1844 bytes, number of entries: 7
+Zip file size: 1846 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-12 11:29 my_backend/__init__.py
 -rw-rw-rw-  2.0 fat      599 b- defN 24-Apr-12 11:42 my_backend/main.py
--rw-rw-rw-  2.0 fat      124 b- defN 24-Apr-16 07:26 lenstr-0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-16 07:26 lenstr-0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       51 b- defN 24-Apr-16 07:26 lenstr-0.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       11 b- defN 24-Apr-16 07:26 lenstr-0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      527 b- defN 24-Apr-16 07:26 lenstr-0.1.dist-info/RECORD
-7 files, 1404 bytes uncompressed, 904 bytes compressed:  35.6%
+-rw-rw-rw-  2.0 fat      124 b- defN 24-Apr-16 07:30 lenstr-0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-16 07:30 lenstr-0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       51 b- defN 24-Apr-16 07:30 lenstr-0.2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       11 b- defN 24-Apr-16 07:30 lenstr-0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      527 b- defN 24-Apr-16 07:30 lenstr-0.2.dist-info/RECORD
+7 files, 1404 bytes uncompressed, 906 bytes compressed:  35.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: my_backend/__init__.py
 Comment: 
 
 Filename: my_backend/main.py
 Comment: 
 
-Filename: lenstr-0.1.dist-info/METADATA
+Filename: lenstr-0.2.dist-info/METADATA
 Comment: 
 
-Filename: lenstr-0.1.dist-info/WHEEL
+Filename: lenstr-0.2.dist-info/WHEEL
 Comment: 
 
-Filename: lenstr-0.1.dist-info/entry_points.txt
+Filename: lenstr-0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: lenstr-0.1.dist-info/top_level.txt
+Filename: lenstr-0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: lenstr-0.1.dist-info/RECORD
+Filename: lenstr-0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `lenstr-0.1.dist-info/RECORD` & `lenstr-0.2.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 my_backend/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 my_backend/main.py,sha256=SQZQ7opNMaFYVJvTJlnZr3KfN8MjnD98S0AswdrDxrA,599
-lenstr-0.1.dist-info/METADATA,sha256=RPo0Oxkt1sPgbKJ51IK1eIvQki4slIAkCxcOSO8_S0I,124
-lenstr-0.1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-lenstr-0.1.dist-info/entry_points.txt,sha256=sNbkqNZUDUjCA0ve3mBozBZ5grV15i-0mzZeCBmx5_g,51
-lenstr-0.1.dist-info/top_level.txt,sha256=F1S16ahqCvvWwiydwib_MPy4CM3AW-k619hgnd-zVuM,11
-lenstr-0.1.dist-info/RECORD,,
+lenstr-0.2.dist-info/METADATA,sha256=RE3gkJpImCCdhovLSlxJ5KGNqLW0-5qEOrg6I1TjBiY,124
+lenstr-0.2.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+lenstr-0.2.dist-info/entry_points.txt,sha256=sNbkqNZUDUjCA0ve3mBozBZ5grV15i-0mzZeCBmx5_g,51
+lenstr-0.2.dist-info/top_level.txt,sha256=F1S16ahqCvvWwiydwib_MPy4CM3AW-k619hgnd-zVuM,11
+lenstr-0.2.dist-info/RECORD,,
```

