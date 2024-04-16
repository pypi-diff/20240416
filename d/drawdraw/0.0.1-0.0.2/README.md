# Comparing `tmp/drawdraw-0.0.1-py3-none-any.whl.zip` & `tmp/drawdraw-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1797 bytes, number of entries: 6
--rw-r--r--  2.0 unx     1010 b- defN 24-Apr-16 05:43 grcalc/app.py
--rw-r--r--  2.0 unx       17 b- defN 24-Apr-16 05:44 drawdraw-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      186 b- defN 24-Apr-16 05:44 drawdraw-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 05:44 drawdraw-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-16 05:44 drawdraw-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      457 b- defN 24-Apr-16 05:44 drawdraw-0.0.1.dist-info/RECORD
-6 files, 1769 bytes uncompressed, 965 bytes compressed:  45.4%
+Zip file size: 1555 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      354 b- defN 24-Apr-16 06:18 grcalc/app.py
+-rw-r--r--  2.0 unx       17 b- defN 24-Apr-16 06:19 drawdraw-0.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      186 b- defN 24-Apr-16 06:19 drawdraw-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 06:19 drawdraw-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-16 06:19 drawdraw-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      456 b- defN 24-Apr-16 06:19 drawdraw-0.0.2.dist-info/RECORD
+6 files, 1112 bytes uncompressed, 723 bytes compressed:  35.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: grcalc/app.py
 Comment: 
 
-Filename: drawdraw-0.0.1.dist-info/LICENSE
+Filename: drawdraw-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: drawdraw-0.0.1.dist-info/METADATA
+Filename: drawdraw-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: drawdraw-0.0.1.dist-info/WHEEL
+Filename: drawdraw-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: drawdraw-0.0.1.dist-info/top_level.txt
+Filename: drawdraw-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: drawdraw-0.0.1.dist-info/RECORD
+Filename: drawdraw-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## grcalc/app.py

```diff
@@ -1,28 +1,15 @@
 
 import numpy as np
 import matplotlib.pyplot as plt
 
 def scatter_plot(x_data, y_data, x_label='', y_label='', title=''):
-   """주어진 x와 y 데이터에 대한 산점도를 그리는 함수
-    :param x데이터: x 축 데이터 (리스트 또는 배열)
-    :param y데이터: y 축 데이터 (리스트 또는 배열)
-    :param x축레이블: x 축 레이블 (기본값: '')
-    :param y축레이블: y 축 레이블 (기본값: '')
-    :param 제목: 그래프 제목 (기본값: '')
-    """
     plt.scatter(x_data, y_data)
     plt.xlabel(x_label)
     plt.ylabel(y_label)
     plt.title(title)
     plt.show()
 
 def box_plot(data, labels=None, title=''):
-    """
-    주어진 데이터에 대한 상자 그림을 그리는 함수
-    :param data: 상자 그림을 그릴 데이터 리스트의 리스트
-    :param labels: 각 상자에 대한 레이블 (기본값: None)
-    :param title: 그래프 제목 (기본값: '')
-    """
     plt.boxplot(data, labels=labels)
     plt.title(title)
     plt.show()
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

