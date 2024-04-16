# Comparing `tmp/gaea_tracker-1.2.0.4-py3-none-any.whl.zip` & `tmp/gaea_tracker-1.2.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5897 bytes, number of entries: 8
+Zip file size: 5908 bytes, number of entries: 8
 -rw-r--r--  2.0 unx      213 b- defN 24-Apr-16 05:21 gaea_tracker/__init__.py
 -rw-r--r--  2.0 unx     1654 b- defN 24-Apr-16 05:21 gaea_tracker/aim_tracker.py
 -rw-r--r--  2.0 unx     7798 b- defN 24-Apr-16 05:21 gaea_tracker/experiment_tracker.py
 -rw-r--r--  2.0 unx     1459 b- defN 24-Apr-16 05:21 gaea_tracker/mlflow_tracker.py
--rw-r--r--  2.0 unx     1745 b- defN 24-Apr-16 05:21 gaea_tracker-1.2.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 05:21 gaea_tracker-1.2.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-Apr-16 05:21 gaea_tracker-1.2.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      668 b- defN 24-Apr-16 05:21 gaea_tracker-1.2.0.4.dist-info/RECORD
-8 files, 13642 bytes uncompressed, 4725 bytes compressed:  65.4%
+-rw-r--r--  2.0 unx     1770 b- defN 24-Apr-16 05:24 gaea_tracker-1.2.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 05:24 gaea_tracker-1.2.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-Apr-16 05:24 gaea_tracker-1.2.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      668 b- defN 24-Apr-16 05:24 gaea_tracker-1.2.0.5.dist-info/RECORD
+8 files, 13667 bytes uncompressed, 4736 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: gaea_tracker/experiment_tracker.py
 Comment: 
 
 Filename: gaea_tracker/mlflow_tracker.py
 Comment: 
 
-Filename: gaea_tracker-1.2.0.4.dist-info/METADATA
+Filename: gaea_tracker-1.2.0.5.dist-info/METADATA
 Comment: 
 
-Filename: gaea_tracker-1.2.0.4.dist-info/WHEEL
+Filename: gaea_tracker-1.2.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: gaea_tracker-1.2.0.4.dist-info/top_level.txt
+Filename: gaea_tracker-1.2.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: gaea_tracker-1.2.0.4.dist-info/RECORD
+Filename: gaea_tracker-1.2.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `gaea_tracker-1.2.0.4.dist-info/METADATA` & `gaea_tracker-1.2.0.5.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: gaea-tracker
-Version: 1.2.0.4
+Version: 1.2.0.5
 Summary: A common tracker library.
 Home-page: https://console.cloud.baidu-int.com/devops/icode/repos/baidu/mlops/gaea-operator/tree/master
 Author: liuyawen03
 Author-email: liuyawen03@baidu.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: windmill-train
 Requires-Dist: aim (==3.17.5)
+Requires-Dist: bcelogger
 
 Gaea Operator
 ===
 工业模型训练通用算子
 
 快速开始
 ---
```

## Comparing `gaea_tracker-1.2.0.4.dist-info/RECORD` & `gaea_tracker-1.2.0.5.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 gaea_tracker/__init__.py,sha256=W_LJdwsPO-i_I_labqmA9UtINpc16H_xrUMtH3BgJrg,213
 gaea_tracker/aim_tracker.py,sha256=B8WcwJPQC6hKy-NMeZOYY6rQ4-cER_2j0zrxdPcNlxQ,1654
 gaea_tracker/experiment_tracker.py,sha256=QojIx4sZjL6Trlla3rtqFObeCE8F-cfzmxMcTuXN3wk,7798
 gaea_tracker/mlflow_tracker.py,sha256=iSHBX25D1K5Ss1Jnhyq_2q9KAeizhOz_LTXIVcU3OXE,1459
-gaea_tracker-1.2.0.4.dist-info/METADATA,sha256=sXqEtgpKRW1QeufuDVlNzqB58LyNO1q5VCbAvELJHhU,1745
-gaea_tracker-1.2.0.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-gaea_tracker-1.2.0.4.dist-info/top_level.txt,sha256=puBG5QOAqx9ZaALXFt41yG0oBynhWzrKEJOMgH__hYw,13
-gaea_tracker-1.2.0.4.dist-info/RECORD,,
+gaea_tracker-1.2.0.5.dist-info/METADATA,sha256=PUsefwAZjbqD5174hbSfWD-GUyjvGfOlyhqM7dUIuIg,1770
+gaea_tracker-1.2.0.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+gaea_tracker-1.2.0.5.dist-info/top_level.txt,sha256=puBG5QOAqx9ZaALXFt41yG0oBynhWzrKEJOMgH__hYw,13
+gaea_tracker-1.2.0.5.dist-info/RECORD,,
```

