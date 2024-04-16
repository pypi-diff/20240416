# Comparing `tmp/tacrpy-1.5.0-py3-none-any.whl.zip` & `tmp/tacrpy-1.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,23 @@
-Zip file size: 27517 bytes, number of entries: 20
+Zip file size: 29495 bytes, number of entries: 21
 -rw-r--r--  2.0 unx       40 b- defN 24-Apr-16 08:56 tacrpy/__init__.py
 -rw-r--r--  2.0 unx    15194 b- defN 24-Apr-16 08:56 tacrpy/data_fetcher.py
 -rw-r--r--  2.0 unx     2512 b- defN 24-Apr-16 08:56 tacrpy/data_operations.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-16 08:56 tacrpy/analytics/__init__.py
--rw-r--r--  2.0 unx       26 b- defN 24-Apr-16 08:56 tacrpy/data_fetcher/__init__.py
--rw-r--r--  2.0 unx     9745 b- defN 24-Apr-16 08:56 tacrpy/data_fetcher/googlesheets.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-16 10:06 tacrpy/analytics/__init__.py
+-rw-r--r--  2.0 unx       48 b- defN 24-Apr-16 10:06 tacrpy/data_fetcher/__init__.py
+-rw-r--r--  2.0 unx     9818 b- defN 24-Apr-16 10:06 tacrpy/data_fetcher/googlesheets.py
+-rw-r--r--  2.0 unx     5445 b- defN 24-Apr-16 10:06 tacrpy/data_fetcher/isvavai.py
 -rw-r--r--  2.0 unx      122 b- defN 24-Apr-16 08:56 tacrpy/datahub/__init__.py
 -rw-r--r--  2.0 unx     3425 b- defN 24-Apr-16 08:56 tacrpy/datahub/data_lineage.py
 -rw-r--r--  2.0 unx    16764 b- defN 24-Apr-16 08:56 tacrpy/datahub/datasets.py
 -rw-r--r--  2.0 unx    18442 b- defN 24-Apr-16 08:56 tacrpy/datahub/glossary.py
 -rw-r--r--  2.0 unx     6005 b- defN 24-Apr-16 08:56 tacrpy/datahub/import_checks.py
 -rw-r--r--  2.0 unx     2147 b- defN 24-Apr-16 08:56 tacrpy/datahub/openapi.py
 -rw-r--r--  2.0 unx       74 b- defN 24-Apr-16 08:56 tacrpy/nlp/__init__.py
 -rw-r--r--  2.0 unx    10216 b- defN 24-Apr-16 08:56 tacrpy/nlp/fulltext.py
 -rw-r--r--  2.0 unx     2796 b- defN 24-Apr-16 08:56 tacrpy/nlp/preprocessing.py
 -rw-r--r--  2.0 unx     1535 b- defN 24-Apr-16 08:56 tacrpy/nlp/semantic.py
--rw-r--r--  2.0 unx      550 b- defN 24-Apr-16 08:56 tacrpy-1.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 08:56 tacrpy-1.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-16 08:56 tacrpy-1.5.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1614 b- defN 24-Apr-16 08:56 tacrpy-1.5.0.dist-info/RECORD
-20 files, 91306 bytes uncompressed, 24895 bytes compressed:  72.7%
+-rw-r--r--  2.0 unx      550 b- defN 24-Apr-16 10:06 tacrpy-1.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 10:06 tacrpy-1.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-16 10:06 tacrpy-1.6.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1701 b- defN 24-Apr-16 10:06 tacrpy-1.6.0.dist-info/RECORD
+21 files, 96933 bytes uncompressed, 26737 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -12,14 +12,17 @@
 
 Filename: tacrpy/data_fetcher/__init__.py
 Comment: 
 
 Filename: tacrpy/data_fetcher/googlesheets.py
 Comment: 
 
+Filename: tacrpy/data_fetcher/isvavai.py
+Comment: 
+
 Filename: tacrpy/datahub/__init__.py
 Comment: 
 
 Filename: tacrpy/datahub/data_lineage.py
 Comment: 
 
 Filename: tacrpy/datahub/datasets.py
@@ -42,20 +45,20 @@
 
 Filename: tacrpy/nlp/preprocessing.py
 Comment: 
 
 Filename: tacrpy/nlp/semantic.py
 Comment: 
 
-Filename: tacrpy-1.5.0.dist-info/METADATA
+Filename: tacrpy-1.6.0.dist-info/METADATA
 Comment: 
 
-Filename: tacrpy-1.5.0.dist-info/WHEEL
+Filename: tacrpy-1.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: tacrpy-1.5.0.dist-info/top_level.txt
+Filename: tacrpy-1.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: tacrpy-1.5.0.dist-info/RECORD
+Filename: tacrpy-1.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tacrpy/data_fetcher/__init__.py

```diff
@@ -1 +1,2 @@
-from . import googlesheets
+from . import googlesheets
+from . import isvavai
```

## tacrpy/data_fetcher/googlesheets.py

```diff
@@ -1,7 +1,9 @@
+"""Modul na načítání dat, které jsou uložené na Google disku."""
+
 import pandas as pd
 
 from google.colab import auth
 auth.authenticate_user()
 
 import gspread
 from google.auth import default
```

## Comparing `tacrpy-1.5.0.dist-info/METADATA` & `tacrpy-1.6.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tacrpy
-Version: 1.5.0
+Version: 1.6.0
 Summary: Analytická knihovna pro potřeby TA ČR
 Home-page: UNKNOWN
 Author: david.sulc
 Author-email: sulda.str@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://data.tacr.cz/tacrpy/docs/index.html
 Platform: UNKNOWN
```

## Comparing `tacrpy-1.5.0.dist-info/RECORD` & `tacrpy-1.6.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 tacrpy/__init__.py,sha256=C-E8DD7BR3WaN0cFJthjKdBBDiIWifZr0EVPP6MoEuY,40
 tacrpy/data_fetcher.py,sha256=y1mCudKY_gAsTp1S2j-oFs5r_J58dd9i71x08DHCh1c,15194
 tacrpy/data_operations.py,sha256=YTHOwrEZLEJyAiiskkcRbNSy3zt2MnQLsPwjobDRrgw,2512
 tacrpy/analytics/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tacrpy/data_fetcher/__init__.py,sha256=OZbxjOpn-pijTRmwR8v8nCJK7W7ZbVmUhGX51N2fUFg,26
-tacrpy/data_fetcher/googlesheets.py,sha256=2cw7QXH5SUR7L9eukq7_B_doQkDwwH7FjltvwVKKPjU,9745
+tacrpy/data_fetcher/__init__.py,sha256=trnojglpHFTLTQAnAGSnO4CBeSUe7pSYpUCzeXzUL8k,48
+tacrpy/data_fetcher/googlesheets.py,sha256=NUFZ31EudNfZllR-h4kLOPEMvDPUzYtWICo6pOKovlc,9818
+tacrpy/data_fetcher/isvavai.py,sha256=g6lhXYH_tFvbvSws6fyCAGQtWjM7c0aXsB5fI8k9dXA,5445
 tacrpy/datahub/__init__.py,sha256=0zK9D2SShhdxCfHDh0sPiQxn__YxVjB7d6cEIS2U4g4,122
 tacrpy/datahub/data_lineage.py,sha256=-QqvyihMHUZ5hiSghye2BjObs_A5JuJbjlFiyA4FrG8,3425
 tacrpy/datahub/datasets.py,sha256=bXiyrVA39VDgPZAhw6XfP9hOGyGsNMr5tL2uMKU5fYQ,16764
 tacrpy/datahub/glossary.py,sha256=Xzdsvdx7qsse_YlsQVI9vvFVxmyq0uAMIiXnkr_0-GU,18442
 tacrpy/datahub/import_checks.py,sha256=y32k1r33eFJ0g-oyal4u6-vhvtEUMipP0ESN7hNuYZE,6005
 tacrpy/datahub/openapi.py,sha256=M8ewVDiywa2UT5G4Wz0Q6YUxl4oxrbf9fFv2QeDYgQ4,2147
 tacrpy/nlp/__init__.py,sha256=JB3slGG7y69kNkWTpmEqqJLp7gVhiUhYVPJ078fulyQ,74
 tacrpy/nlp/fulltext.py,sha256=ObMEgqd2J6d5rB2IYVeoHFYIqMOMky61xL7FvOVA2ko,10216
 tacrpy/nlp/preprocessing.py,sha256=woSTEB5MJafzCvyI4dDaI_RJRVU03k6CHaj-K9LDpII,2796
 tacrpy/nlp/semantic.py,sha256=I2u8Pm6XBRiZyhmCFueMuq_kP7kXa8YNwupjou7uZ-I,1535
-tacrpy-1.5.0.dist-info/METADATA,sha256=zXs7oHR1lqw1jRUNsCopUi0nGccDV81c5jNSjuSQedI,550
-tacrpy-1.5.0.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-tacrpy-1.5.0.dist-info/top_level.txt,sha256=BqpXuN5c5p-Kf_Qv8U1hT8dbV6NhdnLZ7QQa4wAvBH4,7
-tacrpy-1.5.0.dist-info/RECORD,,
+tacrpy-1.6.0.dist-info/METADATA,sha256=CHu7j3RtgbjR-Tgi0igADuMgWffvdtB6-cp_j9nUZSI,550
+tacrpy-1.6.0.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+tacrpy-1.6.0.dist-info/top_level.txt,sha256=BqpXuN5c5p-Kf_Qv8U1hT8dbV6NhdnLZ7QQa4wAvBH4,7
+tacrpy-1.6.0.dist-info/RECORD,,
```

