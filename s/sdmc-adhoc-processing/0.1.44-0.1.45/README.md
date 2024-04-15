# Comparing `tmp/sdmc_adhoc_processing-0.1.44.tar.gz` & `tmp/sdmc_adhoc_processing-0.1.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdmc_adhoc_processing-0.1.44.tar", last modified: Fri Mar 15 18:44:13 2024, max compression
+gzip compressed data, was "sdmc_adhoc_processing-0.1.45.tar", last modified: Mon Apr 15 19:00:52 2024, max compression
```

## Comparing `sdmc_adhoc_processing-0.1.44.tar` & `sdmc_adhoc_processing-0.1.45.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxrwxr-x   0 bhaddock (80211) staff     (1000)        0 2024-03-15 18:44:13.159915 sdmc_adhoc_processing-0.1.44/
--rw-rw-r--   0 bhaddock (80211) staff     (1000)    35149 2024-03-01 20:01:53.000000 sdmc_adhoc_processing-0.1.44/LICENSE
--rw-r--r--   0 bhaddock (80211) staff     (1000)      619 2024-03-15 18:44:13.154925 sdmc_adhoc_processing-0.1.44/PKG-INFO
--rw-rw-r--   0 bhaddock (80211) staff     (1000)       69 2024-03-01 19:56:23.000000 sdmc_adhoc_processing-0.1.44/README.md
--rw-rw-r--   0 bhaddock (80211) staff     (1000)      997 2024-03-15 18:43:42.000000 sdmc_adhoc_processing-0.1.44/pyproject.toml
--rw-rw-r--   0 bhaddock (80211) staff     (1000)       38 2024-03-15 18:44:13.160915 sdmc_adhoc_processing-0.1.44/setup.cfg
-drwxrwxr-x   0 bhaddock (80211) staff     (1000)        0 2024-03-15 18:44:13.093911 sdmc_adhoc_processing-0.1.44/src/
-drwxrwxr-x   0 bhaddock (80211) staff     (1000)        0 2024-03-15 18:44:13.122919 sdmc_adhoc_processing-0.1.44/src/sdmc_adhoc_processing/
--rw-rw-r--   0 bhaddock (80211) staff     (1000)      245 2024-03-13 22:27:19.000000 sdmc_adhoc_processing-0.1.44/src/sdmc_adhoc_processing/__init__.py
--rw-rw-r--   0 bhaddock (80211) staff     (1000)     2576 2024-03-12 17:50:23.000000 sdmc_adhoc_processing-0.1.44/src/sdmc_adhoc_processing/constants.py
--rwxrwx---   0 bhaddock (80211) staff     (1000)    12880 2024-03-08 23:26:26.000000 sdmc_adhoc_processing-0.1.44/src/sdmc_adhoc_processing/data_dictionary_TEMPLATE.xlsx
--rwxrwx---   0 bhaddock (80211) staff     (1000)     5738 2024-03-13 23:24:18.000000 sdmc_adhoc_processing-0.1.44/src/sdmc_adhoc_processing/generate_dict.py
--rw-rw-r--   0 bhaddock (80211) staff     (1000)     7008 2024-03-12 17:51:56.000000 sdmc_adhoc_processing-0.1.44/src/sdmc_adhoc_processing/process.py
-drwxrwxr-x   0 bhaddock (80211) staff     (1000)        0 2024-03-15 18:44:13.150921 sdmc_adhoc_processing-0.1.44/src/sdmc_adhoc_processing.egg-info/
--rw-r--r--   0 bhaddock (80211) staff     (1000)      619 2024-03-15 18:44:13.000000 sdmc_adhoc_processing-0.1.44/src/sdmc_adhoc_processing.egg-info/PKG-INFO
--rw-rw-r--   0 bhaddock (80211) staff     (1000)      559 2024-03-15 18:44:13.000000 sdmc_adhoc_processing-0.1.44/src/sdmc_adhoc_processing.egg-info/SOURCES.txt
--rw-rw-r--   0 bhaddock (80211) staff     (1000)        1 2024-03-15 18:44:13.000000 sdmc_adhoc_processing-0.1.44/src/sdmc_adhoc_processing.egg-info/dependency_links.txt
--rw-rw-r--   0 bhaddock (80211) staff     (1000)      118 2024-03-15 18:44:13.000000 sdmc_adhoc_processing-0.1.44/src/sdmc_adhoc_processing.egg-info/entry_points.txt
--rw-rw-r--   0 bhaddock (80211) staff     (1000)       23 2024-03-15 18:44:13.000000 sdmc_adhoc_processing-0.1.44/src/sdmc_adhoc_processing.egg-info/requires.txt
--rw-rw-r--   0 bhaddock (80211) staff     (1000)       22 2024-03-15 18:44:13.000000 sdmc_adhoc_processing-0.1.44/src/sdmc_adhoc_processing.egg-info/top_level.txt
-drwxrwxr-x   0 bhaddock (80211) staff     (1000)        0 2024-03-15 18:44:13.146919 sdmc_adhoc_processing-0.1.44/tests/
--rw-rw-r--   0 bhaddock (80211) staff     (1000)      100 2024-03-01 19:54:57.000000 sdmc_adhoc_processing-0.1.44/tests/test_foo.py
+drwxrwxr-x   0 bhaddock (80211) staff     (1000)        0 2024-04-15 19:00:52.346263 sdmc_adhoc_processing-0.1.45/
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)    35149 2024-03-01 20:01:53.000000 sdmc_adhoc_processing-0.1.45/LICENSE
+-rw-r--r--   0 bhaddock (80211) staff     (1000)      619 2024-04-15 19:00:52.343253 sdmc_adhoc_processing-0.1.45/PKG-INFO
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)       69 2024-03-01 19:56:23.000000 sdmc_adhoc_processing-0.1.45/README.md
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)     1037 2024-04-15 19:00:04.000000 sdmc_adhoc_processing-0.1.45/pyproject.toml
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)       38 2024-04-15 19:00:52.347256 sdmc_adhoc_processing-0.1.45/setup.cfg
+drwxrwxr-x   0 bhaddock (80211) staff     (1000)        0 2024-04-15 19:00:52.220278 sdmc_adhoc_processing-0.1.45/src/
+drwxrwxr-x   0 bhaddock (80211) staff     (1000)        0 2024-04-15 19:00:52.296314 sdmc_adhoc_processing-0.1.45/src/sdmc_adhoc_processing/
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)      313 2024-03-15 23:09:53.000000 sdmc_adhoc_processing-0.1.45/src/sdmc_adhoc_processing/__init__.py
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)     3197 2024-04-10 20:42:00.000000 sdmc_adhoc_processing-0.1.45/src/sdmc_adhoc_processing/constants.py
+-rwxrwx---   0 bhaddock (80211) staff     (1000)    12964 2024-03-22 18:48:38.000000 sdmc_adhoc_processing-0.1.45/src/sdmc_adhoc_processing/data_dictionary_TEMPLATE.xlsx
+-rwxrwx---   0 bhaddock (80211) staff     (1000)    10205 2024-03-22 18:52:44.000000 sdmc_adhoc_processing-0.1.45/src/sdmc_adhoc_processing/data_dictionary_nonstandard_vars.xlsx
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)     5333 2024-04-15 18:56:45.000000 sdmc_adhoc_processing-0.1.45/src/sdmc_adhoc_processing/generate_README.py
+-rwxrwx---   0 bhaddock (80211) staff     (1000)     5889 2024-04-15 18:59:57.000000 sdmc_adhoc_processing-0.1.45/src/sdmc_adhoc_processing/generate_dict.py
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)     9237 2024-04-11 19:14:15.000000 sdmc_adhoc_processing-0.1.45/src/sdmc_adhoc_processing/process.py
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)     1264 2024-04-12 21:22:07.000000 sdmc_adhoc_processing-0.1.45/src/sdmc_adhoc_processing/readme_template.md
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)      313 2024-04-10 18:40:18.000000 sdmc_adhoc_processing-0.1.45/src/sdmc_adhoc_processing/utilities.py
+drwxrwxr-x   0 bhaddock (80211) staff     (1000)        0 2024-04-15 19:00:52.336310 sdmc_adhoc_processing-0.1.45/src/sdmc_adhoc_processing.egg-info/
+-rw-r--r--   0 bhaddock (80211) staff     (1000)      619 2024-04-15 19:00:52.000000 sdmc_adhoc_processing-0.1.45/src/sdmc_adhoc_processing.egg-info/PKG-INFO
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)      752 2024-04-15 19:00:52.000000 sdmc_adhoc_processing-0.1.45/src/sdmc_adhoc_processing.egg-info/SOURCES.txt
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)        1 2024-04-15 19:00:52.000000 sdmc_adhoc_processing-0.1.45/src/sdmc_adhoc_processing.egg-info/dependency_links.txt
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)      146 2024-04-15 19:00:52.000000 sdmc_adhoc_processing-0.1.45/src/sdmc_adhoc_processing.egg-info/entry_points.txt
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)       23 2024-04-15 19:00:52.000000 sdmc_adhoc_processing-0.1.45/src/sdmc_adhoc_processing.egg-info/requires.txt
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)       22 2024-04-15 19:00:52.000000 sdmc_adhoc_processing-0.1.45/src/sdmc_adhoc_processing.egg-info/top_level.txt
+drwxrwxr-x   0 bhaddock (80211) staff     (1000)        0 2024-04-15 19:00:52.330262 sdmc_adhoc_processing-0.1.45/tests/
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)      100 2024-03-01 19:54:57.000000 sdmc_adhoc_processing-0.1.45/tests/test_foo.py
```

### Comparing `sdmc_adhoc_processing-0.1.44/LICENSE` & `sdmc_adhoc_processing-0.1.45/LICENSE`

 * *Files identical despite different names*

### Comparing `sdmc_adhoc_processing-0.1.44/PKG-INFO` & `sdmc_adhoc_processing-0.1.45/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdmc_adhoc_processing
-Version: 0.1.44
+Version: 0.1.45
 Summary: Helper utilities for SDMC ad-hoc data processing requests.
 Author-email: Beatrix Haddock <beatrix.haddock@gmail.com>
 Project-URL: Homepage, https://github.com/beatrixh/sdmc-adhoc-processing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `sdmc_adhoc_processing-0.1.44/pyproject.toml` & `sdmc_adhoc_processing-0.1.45/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sdmc_adhoc_processing"
-version = "0.1.44"
+version = "0.1.45"
 authors = [
   { name="Beatrix Haddock", email="beatrix.haddock@gmail.com" },
 ]
 description = "Helper utilities for SDMC ad-hoc data processing requests."
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = ["docutils", "requires <= 0.4"]
@@ -17,14 +17,15 @@
 [project.urls]
 Homepage = "https://github.com/beatrixh/sdmc-adhoc-processing"
 
 [build-system]
 requires = [
   "setuptools",
   "pandas",
+  "numpy",
   "typing",
   "datetime",
   "openpyxl",
   "xlsxwriter"
 ]
 build-backend = "setuptools.build_meta"
 
@@ -34,9 +35,9 @@
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
 "*" = ["*.*"]
 
 [project.scripts]
-hello-world = "sdmc_adhoc_processing:hello_world"
-gen-data-dict = "sdmc_adhoc_processing:gen_data_dict"
+gen-readme = "sdmc_adhoc_processing.generate_README:gen_README"
+gen-data-dict = "sdmc_adhoc_processing.generate_dict:gen_data_dict"
```

### Comparing `sdmc_adhoc_processing-0.1.44/src/sdmc_adhoc_processing/constants.py` & `sdmc_adhoc_processing-0.1.45/src/sdmc_adhoc_processing/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,9 +55,39 @@
     ('BLD', 'LYS'): 'Whole Blood (Lysed)',
     ('VCS', 'FLD'): 'Cervicovaginal Secretions (Fluid)',
     ('VCS', 'MUC'): 'Cervicovaginal Secretions (Mucus)',
     ('VAG', 'SWB'): 'Vaginal Swab',
     ('BLD', 'BLD'): 'Whole Blood',
     ('VCS', "N/A"): 'Cervicovaginal Secretions',
     ('BLD', "N/A"): 'Whole Blood',
-    ('VCS', 'SWB'): 'Cervicovaginal Secretions (Swab)'
+    ('VCS', 'SWB'): 'Cervicovaginal Secretions (Swab)',
+    ('REC', 'BPS'): 'Rectal Biopsy',
+    ('VAG', 'BPS'): 'Vaginal Biopsy',
+    ('CER', 'BPS'): 'Cervical Biopsy',
+    ('REC', 'SEC'): 'Rectal Secretions'
 }
+
+STD_PREFACE_COLS = [
+    'network',
+    'protocol',
+    'specrole',
+    'guspec',
+    'ptid',
+    'visitno',
+    'drawdt',
+    'spectype',
+    'spec_primary',
+    'spec_additive',
+    'spec_derivative',
+    'upload_lab_id',
+    'assay_lab_name',
+    'assay_type',
+    'assay_subtype',
+    'assay_kit',
+    'instrument',
+]
+
+STD_POSTFACE_COLS = [
+    'sdmc_processing_datetime',
+    'sdmc_data_receipt_datetime',
+    'input_file_name'
+]
```

### Comparing `sdmc_adhoc_processing-0.1.44/src/sdmc_adhoc_processing/data_dictionary_TEMPLATE.xlsx` & `sdmc_adhoc_processing-0.1.45/src/sdmc_adhoc_processing/data_dictionary_TEMPLATE.xlsx`

 * *Files 24% similar despite different names*

```diff
@@ -103,75 +103,75 @@
 00000660: d542 53ed ad86 b0b7 37a0 ea93 cf9b 7fd7  .BS.....7.......
 00000670: 96a6 e90d 3f88 394c ecd2 9915 c873 6267  ....?.9L.....sbg
 00000680: d9ae 7cc8 6c21 f5f9 1a55 5368 3969 b062  ..|.l!...USh9i.b
 00000690: 9e72 3a22 795f 646c c0f3 449b bf13 fd7c  .r:"y_dl..D....|
 000006a0: 2d4e 9cc8 5222 3412 f832 cf47 c725 a0f5  -N..R"4..2.G.%..
 000006b0: 7f5a b434 f1cb 9d79 c437 09c3 abc8 f0c9  .Z.4...y.7......
 000006c0: 828b 1fa8 de01 0000 ffff 0300 504b 0304  ............PK..
-000006d0: 1400 0600 0800 0000 2100 c97e 6f47 5803  ........!..~oGX.
-000006e0: 0000 6208 0000 0f00 0000 786c 2f77 6f72  ..b.......xl/wor
-000006f0: 6b62 6f6f 6b2e 786d 6ca4 565d 6fa3 3814  kbook.xml.V]o.8.
-00000700: 7d5f 69fe 03f2 3b05 2740 1b54 3a0a 2168  }_i...;.'@.T:.!h
-00000710: 2a35 55d5 66da 5929 52e4 8029 5601 b3b6  *5U.f.Y)R..)V...
-00000720: 6912 8de6 bfcf 3584 6432 59ad b21d 94d8  i.....5.d2Y.....
-00000730: f8fa 72b8 1fe7 38b9 febc 290b e39d 0ac9  ..r...8...).....
-00000740: 7815 207c 6123 8356 094f 59f5 1aa0 aff3  x. |a#.V.OY.....
-00000750: d8bc 4286 54a4 4a49 c12b 1aa0 2d95 e8f3  ..B.T.JI.+..-...
-00000760: cda7 bfae d75c bcad 387f 3300 a092 01ca  .....\..8.3.....
-00000770: 95aa 7dcb 9249 4e4b 222f 784d 2bd8 c9b8  ..}..INK"/xM+...
-00000780: 2889 82a5 78b5 642d 2849 654e a92a 0b6b  (...x.d-(IeN.*.k
-00000790: 60db 9e55 1256 a10e c117 e760 f02c 6309  `..U.V.....`.,c.
-000007a0: 8d78 d294 b452 1d88 a005 5110 becc 592d  .x...R....Q...Y-
-000007b0: 7bb4 3239 07ae 24e2 ada9 cd84 9735 40ac  {.29..$......5@.
-000007c0: 58c1 d4b6 0545 4699 f8b7 af15 1764 5540  X....EF......dU@
-000007d0: da1b ec1a 1b01 1f0f bed8 8661 d0bf 09b6  ...........a....
-000007e0: 4e5e 55b2 4470 c933 7501 d056 17f4 49fe  N^U.Dp.3u..V..I.
-000007f0: d8b6 303e 2ac1 e6b4 06e7 2139 96a0 ef4c  ..0>*.....!9...L
-00000800: f770 1f95 f03e 1895 b7c7 f20e 60d8 fe63  .p...>......`..c
-00000810: 340c d46a b9e2 43f1 3e88 e6ee 631b a09b  4..j..C.>...c...
-00000820: eb8c 15f4 b9a3 ae41 eafa 9e94 ba53 0532  .......A.....S.2
-00000830: 0a22 d534 658a a601 ba84 255f d323 8368  .".4e.....%_.#.h
-00000840: eab0 6105 ec0e bccb 2146 d6cd 9ece 0fc2  ..a.....!F......
-00000850: 4869 469a 42cd 81c8 3d3c 28c3 f346 0357  HiF.B...=<(..F.W
-00000860: 7b02 31c6 85a2 a222 8a4e 78a5 8087 bbbc  {.1....".Nx.....
-00000870: fe94 732d f624 e7c0 70e3 91fe d330 4141  ..s-.$..p....0AA
-00000880: 58c0 2fc8 1546 92f8 6425 1f88 ca8d 4614  X./..F..d%....F.
-00000890: 01ba f717 efaa 5a14 64b5 788a 6693 25dc  ......Z.d.x.f.%.
-000008a0: c884 817a e902 d427 3a4d 2cd2 9d56 e442  ...z...':M,..V.B
-000008b0: d1b2 06a5 50b9 2052 92ed 7ebd 0493 02bd  ....P. R..~.....
-000008c0: 2f7e 6134 3995 cfff e034 4974 a12c a854  /~a49....4It.,.T
-000008d0: 974d 77ff 7bd5 2029 e1f7 bc7d 50c2 80fb  .Mw.{. )...}P...
-000008e0: dbe8 0e7a f744 dea1 93c0 973e f85b 6815  ...z.D.....>.[h.
-000008f0: 1e2e ab44 f878 f97d 1c47 e371 184d cda1  ...D.x.}.G.q.M..
-00000900: 77e9 9a4e 389a 98a3 418c 4d7b 389c 784e  w..N8...A.M{8.xN
-00000910: 145d 85de e407 2423 3c3f e1a4 51f9 8e24  .]....$#<?..Q..$
-00000920: 1a3a 400e 30e2 646b 4636 fd0e b6fd 86a5  .:@.0.dkF6......
-00000930: 8730 bedb bbcb d4f3 6f43 bff7 4327 ac8f  .0......oC..C'..
-00000940: c367 46d7 f240 27bd 3436 2fac 4af9 3a40  .gF..@'.46/.J.:@
-00000950: 2676 5d07 d2da 1e0c 1e9c 83c8 58b7 0e2f  &v].........X../
-00000960: 2c55 3924 ea38 07db 17ca 5e73 881a bb9e  ,U9$.8....^s....
-00000970: 3682 7474 7401 3a8a 2aea a28a e132 f570  6.ttt.:.*....2.p
-00000980: 1495 f54b 58ed e10b e1b5 b351 b582 4905  ...KX......Q..I.
-00000990: c9d4 3225 8a2c 5396 e883 9488 2d1c fafa  ..2%.,S.....-...
-000009a0: 9c6e eb8e 0ce1 eb57 8adb b495 8ad5 a324  .n.....W.......$
-000009b0: a448 402f 7a6a 1d47 d81e 8c74 21e8 46dd  .H@/zj.G...t!.F.
-000009c0: 49d5 ce40 5506 d186 ee55 680f 4703 d389  I..@U....Uh.G...
-000009d0: 716c 3a78 649b 61e8 39a6 1bc5 43f7 1247  ql:xd.a.9...C..G
-000009e0: 93a9 1beb 96e9 df12 7fa3 11b3 0f1e 1157  ...............W
-000009f0: 56fb 3425 aa01 f968 e5b4 6b5f 8ff1 ceba  V.4%...h..k_....
-00000a00: 3766 9d61 5789 2386 fb8f 914e 65f7 f47f  7f.aW.#....Ne...
-00000a10: 393e 8176 0a7a a673 fc7c a6e3 e47e 369f  9>.v.z.s.|...~6.
-00000a20: 9de9 7b37 9d2f 5fe2 739d c7b3 301a 9fef  ..{7./_.s...0...
-00000a30: 3f7e 7c1c ff3d 9f7e eb5f 61fd 6b41 2de8  ?~|..=.~._a.kA-.
-00000a40: 39c8 bcef bcd5 ff3d b8f9 0900 00ff ff03  9......=........
-00000a50: 0050 4b03 0414 0006 0008 0000 0021 0081  .PK..........!..
-00000a60: 3e94 97f3 0000 00ba 0200 001a 0008 0178  >..............x
-00000a70: 6c2f 5f72 656c 732f 776f 726b 626f 6f6b  l/_rels/workbook
-00000a80: 2e78 6d6c 2e72 656c 7320 a204 0128 a000  .xml.rels ...(..
-00000a90: 0100 0000 0000 0000 0000 0000 0000 0000  ................
+000006d0: 1400 0600 0800 0000 2100 25bf 56fe 5f03  ........!.%.V._.
+000006e0: 0000 5308 0000 0f00 0000 786c 2f77 6f72  ..S.......xl/wor
+000006f0: 6b62 6f6f 6b2e 786d 6ca4 566d 6f9b 3a14  kbook.xml.Vmo.:.
+00000700: fe7e a5fd 07e4 ef14 cc5b 1254 3a25 10b4  .~.......[.T:%..
+00000710: 4acd 5665 69bb 4991 2207 4cb1 0a98 6b4c  J.Vei.I.".L...kL
+00000720: 936a dafd edf7 9884 7459 a629 eb50 6263  .j......tY.).Pbc
+00000730: fbf0 f839 e73c c770 f97e 5b16 da33 150d  ...9.<.p.~[..3..
+00000740: e355 80f0 8589 345a 253c 65d5 6380 ee16  .U....4Z%<e.c...
+00000750: b13e 445a 2349 9592 8257 3440 2fb4 41ef  .>DZ#I...W4@/.A.
+00000760: afde fd73 b9e1 e269 cdf9 9306 0055 13a0  ...s...i.....U..
+00000770: 5cca da37 8c26 c969 499a 0b5e d30a 5632  \..7.&.iI..^..V2
+00000780: 2e4a 2261 281e 8da6 1694 a44d 4ea9 2c0b  .J"a(......MN.,.
+00000790: c332 4dcf 2809 abd0 0ec1 17e7 60f0 2c63  .2M.(.......`.,c
+000007a0: 098d 78d2 96b4 923b 1041 0b22 817e 93b3  ..x....;.A.".~..
+000007b0: bae9 d1ca e41c b892 88a7 b6d6 135e d600  .............^..
+000007c0: b166 0593 2f1d 28d2 cac4 bf7e acb8 20eb  .f../.(....~.. .
+000007d0: 02dc de62 57db 0af8 79f0 c726 3456 bf13  ...bW...y..&4V..
+000007e0: 2c9d 6c55 b244 f086 67f2 02a0 8d1d e913  ,.lU.D..g.......
+000007f0: ffb1 6960 7c14 82ed 690c ce43 720c 419f  ..i`|...i..Cr.A.
+00000800: 99ca e181 95f0 dec8 ca3b 6079 af60 d8fc  .........;`y.`..
+00000810: 6b34 0cd2 eab4 e243 f0de 88e6 1eb8 59e8  k4.....C......Y.
+00000820: ea32 6305 bddf 4957 2375 fd91 942a 5305  .2c...IW#u...*S.
+00000830: d20a d2c8 69ca 244d 0334 8021 dfd0 a309  ....i.$M.4.!....
+00000840: d1d6 9396 15b0 6a79 031b 23e3 ea20 e75b  ......jy..#.. .[
+00000850: a1a5 3423 6d21 1720 e41e 1e2a c3f3 4696  ..4#m!. ...*..F.
+00000860: ab2c 4118 e342 5251 1149 435e 49d0 e1de  .,A..BRQ.IC^I...
+00000870: afbf d55c 871d e61c 14ae cde9 bf2d 1314  ...\.........-..
+00000880: 0a0b f405 be42 4b12 9fac 9b5b 2273 ad15  .....BK....["s..
+00000890: 4580 427f 79d7 80fb cb75 4ed2 9427 4fcb  E.B.y....uN..'O.
+000008a0: e853 7837 9bfe 8797 33be 265f 8063 b96c  .Sx7....3.&_.c.l
+000008b0: 2016 f972 4e4b 2e69 0cf1 6a96 d8b6 0723   ..rNK.i..j....#
+000008c0: 6b65 afec e50f 1226 a7f5 f207 2226 898a  ke.....&...."&..
+000008d0: 8c01 a1d9 d1df ddff 1c26 f042 f8bd 506f  .........&.B..Po
+000008e0: a5d0 e0fe 3aba 8164 7d26 cf90 3a10 08b8  ....:..d}&..:...
+000008f0: d155 f635 e406 dbab 2a11 3e5e 7d8b ccc1  .U.5....*.>^}...
+00000900: c831 4d47 0fc3 a1ab 3b91 37d4 c75e e8e9  .1MG....;.7..^..
+00000910: b1e7 626f 62d9 aeeb 8dbe 8333 c2f3 134e  ..bob......3...N
+00000920: 5a99 ef55 a1a0 03e4 8004 4e96 6664 dbaf  Z..U......N.fd..
+00000930: 60d3 6f59 fa4a e39b b9bf 74d5 ffd4 f46b  `.oY.J....t....k
+00000940: df95 c3ea fcbb 6774 d3bc ea47 0db5 ed03  ......gt...G....
+00000950: ab52 be09 908e 5dd7 01b7 5e5e 273c 38f8  .R....]...^^'<8.
+00000960: 90b6 e90c 1e58 2a73 10a1 3518 bafd dc07  .....X*s..5.....
+00000970: ca1e 7360 8d5d 4f19 42ad 2876 013a 6215  ..s`.]O.B.(v.:b.
+00000980: ed58 c570 e9aa 3962 65fc 40ab 3b6d 815e  .X.p..9be.@.;m.^
+00000990: d76b 5557 21a9 2099 5ca5 4492 55ca 1275  .kUW!. .\.D.U..u
+000009a0: 7212 f102 a7bc 3a98 bbb8 234d f86a 4b71  r.....:...#M.jKq
+000009b0: 9d76 b561 f428 0929 1228 10d5 7586 236c  .v.a.(.).(..u.#l
+000009c0: 5a23 1508 ba95 378d ec7a d026 03b6 1377  Z#....7..z.&...w
+000009d0: 3831 ed91 a53b 318e 7507 8f4c 7d32 f11c  81...;1.u..L}2..
+000009e0: dd8d 62db 1de0 289c bab1 4a99 7a79 f85b  ..b...(...J.zy.[
+000009f0: 8598 bdf1 4c18 1add d394 c816 ea45 954a  ....L........E.J
+00000a00: 37f6 551b ef67 0f93 d96e 621f 8923 85fb  7.U..g...nb..#..
+00000a10: f348 b9b2 7ffa 7786 9fe1 e558 d033 8de3  .H....w....X.3..
+00000a20: fb33 0dc3 8fb3 c5ec 4cdb 9be9 62f5 109f  .3......L...b...
+00000a30: 6b3c 9e4d a2f1 f9f6 e3f9 7cfc 7531 fdd2  k<.M......|.u1..
+00000a40: 6f61 fc32 a006 e41c cabc cfbc d17f 0f5c  oa.2...........\
+00000a50: fd0f 0000 ffff 0300 504b 0304 1400 0600  ........PK......
+00000a60: 0800 0000 2100 813e 9497 f300 0000 ba02  ....!..>........
+00000a70: 0000 1a00 0801 786c 2f5f 7265 6c73 2f77  ......xl/_rels/w
+00000a80: 6f72 6b62 6f6f 6b2e 786d 6c2e 7265 6c73  orkbook.xml.rels
+00000a90: 20a2 0401 28a0 0001 0000 0000 0000 0000   ...(...........
 00000aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -179,627 +179,633 @@
 00000b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b90: 00ac 524d 4bc4 3010 bd0b fe87 3077 9b76  ..RMK.0.....0w.v
-00000ba0: 1511 d974 2f22 ec55 eb0f 08c9 b429 db26  ...t/".U.....).&
-00000bb0: 2133 7ef4 df1b 2aba 5d58 d64b 2f03 6f86  !3~...*.]X.K/.o.
-00000bc0: 79ef cdc7 76f7 350e e203 13f5 c12b a88a  y...v.5......+..
-00000bd0: 1204 7a13 6cef 3b05 6fcd f3cd 0308 62ed  ..z.l.;.o.....b.
-00000be0: ad1e 8247 0513 12ec eaeb abed 0b0e 9a73  ...G...........s
-00000bf0: 13b9 3e92 c82c 9e14 38e6 f828 2519 87a3  ..>..,..8..(%...
-00000c00: a622 44f4 b9d2 8634 6ace 3075 326a 73d0  ."D....4j.0u2js.
-00000c10: 1dca 4d59 decb b4e4 80fa 8453 ecad 82b4  ..MY.......S....
-00000c20: b7b7 209a 2966 e5ff b943 dbf6 069f 8279  .. .)f...C.....y
-00000c30: 1fd1 f319 0949 3c0d 7900 d1e8 d421 2bf8  .....I<.y....!+.
-00000c40: c145 f608 f2bc fc66 4d79 ce6b c1a3 fa0c  .E.....fMy.k....
-00000c50: e51c ab4b 1eaa 353d 7c86 7420 87c8 471f  ...K..5=|.t ..G.
-00000c60: 7f29 9273 e5a2 99bb 55ef e174 42fb ca29  .).s....U..tB..)
-00000c70: bfdb f22c cbf4 ef66 e4c9 c7d5 df00 0000  ...,...f........
-00000c80: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
-00000c90: 2100 116d 0f68 b405 0000 2416 0000 1800  !..m.h....$.....
-00000ca0: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
-00000cb0: 7368 6565 7431 2e78 6d6c 9c93 db8e da30  sheet1.xml.....0
-00000cc0: 1086 ef2b f51d 22df 13e7 4496 20c2 aaea  ...+.."...D. ...
-00000cd0: 0a75 6faa aadb c3b5 7126 c422 8e53 db9c  .uo.....q&.".S..
-00000ce0: 5af5 dd77 6c8e 2a15 428b 82c7 89f3 7fff  Z..wl.*.B.......
-00000cf0: 8c3d 993c 6e65 1bac 411b a1ba 92c4 6144  .=.<ne..A.....aD
-00000d00: 02e8 b8aa 44b7 28c9 f76f b3c1 8804 c6b2  ....D.(..o......
-00000d10: ae62 adea a024 3b30 e471 fafe dd64 a3f4  .b...$;0.q...d..
-00000d20: d234 0036 4042 674a d258 db8f 2935 bc01  .4.6@BgJ.X..)5..
-00000d30: c94c a87a e870 a556 5a32 8bb7 7a41 4daf  .L.z.p.VZ2..zAM.
-00000d40: 8155 5e24 5b9a 4451 4e25 131d d913 c6fa  .U^$[.DQN%......
-00000d50: 1e86 aa6b c1e1 49f1 9584 ceee 211a 5a66  ...k..I.....!.Zf
-00000d60: 317f d388 de1c 6992 df83 934c 2f57 fd80  1.....i....L/W..
-00000d70: 2bd9 2362 2e5a 6177 1e4a 02c9 c7cf 8b4e  +.#b.Zaw.J.....N
-00000d80: 6936 6fb1 ee6d 9c31 1e6c 355e 09fe d3a3  i6o..m.1.l5^....
-00000d90: 8d7f 7ee5 2405 d7ca a8da 8648 a6fb 9caf  ..~.$......H....
-00000da0: cb2f 6841 193f 91ae ebbf 0b13 6754 c35a  ./hA.?......gT.Z
-00000db0: b803 3ca3 92b7 a514 0f4f ace4 0c4b df08  ..<......O...K..
-00000dc0: cb4f 30b7 5d7a bc12 5549 fe44 87df 0063  .O0.]z..UI.D...c
-00000dd0: ec86 e83c 1cd7 fe92 e9a4 1278 c2ae aa40  ...<.......x...@
-00000de0: 435d 920f f178 9624 844e 27be 817e 08d8  C]...x.$.N'..~..
-00000df0: 988b 7960 d9fc 055a e016 d024 26c1 6fa5  ..y`...Z...$&.o.
-00000e00: e40b 672d 7c76 1dd8 e2b3 087b db75 ed5c  ..g-|v.....{.u.\
-00000e10: a9a5 933f e38b 111a 192f 7346 8c5b b186  ...?...../sF.[..
-00000e20: 8fd0 e2eb b338 c7ce ffe5 bddd 1c8d e9c9  .....8..........
-00000e30: f972 7ecc 62e6 3bfd 8b0e 2aa8 d9aa b55f  .r~.b.;...*...._
-00000e40: d5e6 1388 4563 d13a 0b87 b803 ae85 c6d5  ....Ec.:........
-00000e50: ee09 0cc7 de45 f330 1d3a 2e57 2d42 700c  .....E.0.:.W-Bp.
-00000e60: a470 1f21 f61e dbfa b811 956d 4a92 1461  .p.!.......mJ..a
-00000e70: 9217 c334 4e10 c357 c62a f973 bf12 1ff4  ...4N..W.*.s....
-00000e80: 7b25 9e99 5762 3c28 d334 8c46 c528 4b1f  {%..Wb<(.4.F.(K.
-00000e90: 5069 ecce b532 f26f 30f0 a83c 233b 338a  Pi...2.o0..<#;3.
-00000ea0: 0bc6 0d25 3a78 25c6 63de 59f8 90e4 c3dc  ...%:x%.c.Y.....
-00000eb0: a57d 30c7 d46e 2070 cb3d 02e3 b980 7f11  .}0..n p.=......
-00000ec0: ffcd 9ffa 4d7c 0500 00ff ff00 0000 ffff  ....M|..........
-00000ed0: 9c58 d18e da30 10fc 1594 0f38 b063 87bb  .X...0.....8.c..
-00000ee0: 1341 6a82 f90f 4491 eee5 8e8a d06b fbf7  .Aj...D......k..
-00000ef0: 5ddb 496c cf9a 1078 43c9 78bc b35e ef6c  ].Il...xC.x..^.l
-00000f00: d874 1fa7 d375 77b8 1eb6 9bcb f9cf e252  .t...uw........R
-00000f10: 17a2 5874 bf0e 5f1d fd7a af8a c55f a10e  ..Xt.._..z..._..
-00000f20: c7f7 9fff 76a7 ee78 faba d6c5 eaa5 d4c5  ....v..x........
-00000f30: 7673 b4d8 1f16 5c17 65b1 a017 1d3d fdde  vs....\.e....=..
-00000f40: ae36 cbef ed66 79ec 118d 47a8 0821 5244  .6...fy...G..!RD
-00000f50: cb39 648a d871 84aa 5288 f110 1d6d 53a6  .9d..q..R....mS.
-00000f60: 883d 0f44 8d88 2569 1f13 201f 4900 8147  .=.D..%i.. .I..G
-00000f70: e91a a45b 2297 cf11 5142 d86d bcbc bc11  ...["...QB.m....
-00000f80: 0f65 77fe 81c4 4701 9b35 9628 8d67 0d47  .ew...G..5.(.g.G
-00000f90: e111 6f71 1641 d42e de40 871d 920c d269  ..oq.A...@.....i
-00000fa0: cf8f 3829 0d08 a8b1 4c75 4165 38a6 50be  ..8)....LuAe8.P.
-00000fb0: 41cc f1fa 2885 ae3e cdb0 7e49 2519 9f31  A...(..>..~I%..1
-00000fc0: 154a 1ce1 07d1 4b92 3d5d ec71 7541 148d  .J....K.=].quA..
-00000fd0: 25ac 8bd7 3873 7013 5a0f 8993 ab81 c578  %...8sp.Z......x
-00000fe0: 8858 1518 2f65 607e 46e3 7489 5054 2e23  .X../e`~F.t.PT.#
-00000ff0: 8d65 4a03 5570 535a 0f99 ac02 0ed1 70ad  .eJ.UpSZ......p.
-00001000: 8d87 64b4 ac9f c93d 2d1a 4b40 e045 b38c  ..d....=-.K@.E..
-00001010: 907c 6821 ad87 4c6a e210 0d2c c643 329a  .|h!..Lj...,.C2.
-00001020: e8e0 e79f 4f5c 2502 2fa9 6502 2d78 4b3d  ....O\%./.e.-xK=
-00001030: 24d6 a2f0 9672 8886 5336 1e92 d142 c4f3  $....r..S6...B..
-00001040: b5c4 5108 ecfd 9629 bdbd 2536 7f0f 99d4  ..Q....)..%6....
-00001050: 9281 4046 8c87 64b4 d0a3 47dc 8cd0 a1ca  ..@F..d...G.....
-00001060: 20d4 c671 a572 14de f11e 3359 6719 8c7a   ..q.r....3Yg..z
-00001070: 453b b371 53af e69d 403c e6cf 840e 8aa0  E;.qS...@<......
-00001080: 9c1b c705 8a98 3b7b df9c 56c4 310a 5b5b  ......;{..V.1.[[
-00001090: bf57 4ed1 4386 2b62 cb14 50d4 8d7d 0b25  .WN.C.+b..P..}.%
-000010a0: a7b0 15f4 9869 459e 2769 d670 d6a6 e7c9  .....iE.'i.p....
-000010b0: 2902 cbb6 f6a2 ca17 eaee 77a6 a9c4 5cd1  ).........w...\.
-000010c0: 0b05 f76f 09f7 beb5 9830 6db0 1188 3354  ...o.....0m...3T
-000010d0: 4155 6290 023c 7cb6 84d8 8e35 9475 e358  AUb..<|....5.u.X
-000010e0: d311 44e2 4864 3141 02d8 d73e c370 5302  ..D.Hd1A...>.pS.
-000010f0: 98fc 9ddc c7ee 2e59 ee7b 678e 4203 6dad  .......Y.{g.B.m.
-00001100: 4886 cf1b b39c 0023 a75a a51a 3bfe eeae  H......#.Z..;...
-00001110: e7cf fdf9 f279 20e5 7499 ee84 cadd b762  .....y .t......b
-00001120: cd6a f079 9a24 9cf1 b76e 6bb7 ddcd ec9a  .j.y.$...nk.....
-00001130: 1ee3 4bda 2ddb f78f 5ed9 4822 c0c7 9f93  ..K.-...^.H"....
-00001140: c24d 57b2 2ee5 31c9 10c8 929f f177 281d  .MW...1......w(.
-00001150: e302 ae8b b555 d26b 1b06 071c b704 f8f9  .....U.k........
-00001160: 73da b809 574c 9bc7 5463 4cc6 6d9d 4639  s...WL..TcL.m.F9
-00001170: 8c04 2c4a 70ea e7a2 e4f6 5ab1 ae3a 18f9  ..,Jp.....Z..:..
-00001180: 9039 23fc 9338 97fe 09af 1309 166c 3b89  .9#..8.......l;.
-00001190: 2649 d335 6e57 8599 1f03 729c f069 8525  &I.5nW....r..i.%
-000011a0: 9130 08b0 a37d 8641 de68 8512 1c77 dec7  .0...}.A.h...w..
-000011b0: 825d 1504 e014 ee38 4100 7ed8 240c 2860  .].....8A.~.$.(`
-000011c0: 97bc d5d8 2633 fc32 b488 f473 17ec 77a6  ....&3.2...s..w.
-000011d0: bcc4 86b1 cf4b fee9 ab20 c4d6 62c2 6802  .....K... ..b.h.
-000011e0: e277 c95b 1d6c ce87 be0c 7f5b fc07 0000  .w.[.l.....[....
-000011f0: ffff 0000 00ff ff34 8dc1 0ac2 3010 447f  .......4....0.D.
-00001200: 25ec 0758 4544 90a6 770f 9efc 8295 6c93  %..XED..w.....l.
-00001210: 45cd 86ed 88bf 6f2b e436 6f78 cc8c 8db3  E.....o+.6ox....
-00001220: dcd8 b3d6 25bc 6446 a4fd ee4c c135 979e  ....%.dF...L.5..
-00001230: 61ed df9e 283c 0cb0 77a7 229c c437 3a52  a...(<..w."..7:R
-00001240: 98cd d061 98c6 6df7 2ef8 b460 ae52 c150  ...a..m....`.R.P
-00001250: ab91 9a39 9c15 ebc3 4553 24bf a603 adfa  ...9....ES$.....
-00001260: f035 7f2e 4504 d30f 0000 ffff 0300 504b  .5..E.........PK
-00001270: 0304 1400 0600 0800 0000 2100 c117 10be  ..........!.....
-00001280: 4e07 0000 c620 0000 1300 0000 786c 2f74  N.... ......xl/t
-00001290: 6865 6d65 2f74 6865 6d65 312e 786d 6cec  heme/theme1.xml.
-000012a0: 59cd 8b1b 3714 bf17 fa3f 0c73 77fc 35e3  Y...7....?.sw.5.
-000012b0: 8f25 dee0 cf6c 93dd 2464 9d94 1cb5 b6ec  .%...l..$d......
-000012c0: 5156 3332 92bc 1b13 0225 39f5 5228 a4a5  QV32.....%9.R(..
-000012d0: 9742 6f3d 94d2 4003 0dbd f48f 0924 b4e9  .Bo=..@......$..
-000012e0: 1fd1 27cd d823 ade5 249b 6c4a 5a76 0d8b  ..'..#..$.lJZv..
-000012f0: 47fe bda7 a7f7 9e7e 7af3 74f1 d2bd 987a  G......~z.t....z
-00001300: 4798 0bc2 9296 5fbe 50f2 3d9c 8cd8 9824  G....._.P.=....$
-00001310: d396 7f6b 3828 347c 4f48 948c 1165 096e  ...k8(4|OH...e.n
-00001320: f90b 2cfc 4bdb 9f7e 7211 6dc9 08c7 d803  ..,.K..~r.m.....
-00001330: f944 6ca1 961f 4939 db2a 16c5 0886 91b8  .Dl...I9.*......
-00001340: c066 3881 df26 8cc7 48c2 239f 16c7 1c1d  .f8..&..H.#.....
-00001350: 83de 9816 2ba5 52ad 1823 92f8 5e82 6250  ....+.R..#..^.bP
-00001360: 7b7d 3221 23ec 0d95 4a7f 7ba9 bc4f e131  {}2!#...J.{..O.1
-00001370: 9142 0d8c 28df 57aa b125 a1b1 e3c3 b242  .B..(.W..%.....B
-00001380: 8885 e852 ee1d 21da f261 9e31 3b1e e27b  ...R..!..a.1;..{
-00001390: d2f7 2812 127e 68f9 25fd e717 b72f 16d1  ..(..~h.%..../..
-000013a0: 5626 44e5 0659 436e a0ff 32b9 4c60 7c58  V&D..YCn..2.L`|X
-000013b0: d173 f2e9 c16a d220 0883 5a7b a55f 03a8  .s...j. ..Z{._..
-000013c0: 5cc7 f5eb fd5a bfb6 d2a7 0168 3482 95a6  \....Z.....h4...
-000013d0: b6d8 3aeb 956e 9061 0d50 fad5 a1bb 57ef  ..:..n.a.P....W.
-000013e0: 55cb 16de d05f 5db3 b91d aa8f 85d7 a054  U...._]........T
-000013f0: 7fb0 861f 0cba e045 0baf 4129 3e5c c387  .......E..A)>\..
-00001400: 9d66 a767 ebd7 a014 5f5b c3d7 4bed 5e50  .f.g...._[..K.^P
-00001410: b7f4 6b50 4449 72b8 862e 85b5 6a77 b9da  ..kPDIr.....jw..
-00001420: 1564 c2e8 8e13 de0c 8341 bd92 29cf 5190  .d.......A..).Q.
-00001430: 0dab ec52 534c 5822 37e5 5a8c ee32 3e00  ...RSLX"7.Z..2>.
-00001440: 8002 5224 49e2 c9c5 0c4f d008 b2b8 8b28  ..R$I....O.....(
-00001450: 39e0 c4db 25d3 0812 6f86 1226 60b8 5429  9...%...o..&`.T)
-00001460: 0d4a 55f8 af3e 81fe a623 8ab6 3032 a495  .JU..>...#..02..
-00001470: 5d60 8958 1b52 f678 62c4 c94c b6fc 2ba0  ]`.X.R.xb..L..+.
-00001480: d537 202f 9e3d 7bfe f0e9 f387 bf3d 7ff4  .7 /.={......=..
-00001490: e8f9 c35f b2b9 b52a 4b6e 0725 5353 eed5  ..._...*Kn.%SS..
-000014a0: 8f5f fffd fd17 de5f bffe f0ea f137 e9d4  ._....._.....7..
-000014b0: 27f1 c2c4 bffc f9cb 97bf fff1 3af5 b0e2  '...........:...
-000014c0: dc15 2fbe 7df2 f2e9 9317 df7d f5e7 4f8f  ../.}......}..O.
-000014d0: 1dda db1c 1d98 f021 89b1 f0ae e163 ef26  .......!.....c.&
-000014e0: 8b61 810e fbf1 013f 9dc4 3042 c492 4011  .a.....?..0B..@.
-000014f0: e876 a8ee cbc8 025e 5b20 eac2 75b0 edc2  .v.....^[ ..u...
-00001500: db1c 58c6 05bc 3cbf 6bd9 ba1f f1b9 248e  ..X...<.k.....$.
-00001510: 99af 46b1 05dc 638c 7618 773a e0aa 9acb  ..F...c.v.w:....
-00001520: f0f0 709e 4cdd 93f3 b989 bb89 d091 6bee  ..p.L.........k.
-00001530: 2e4a ac00 f7e7 33a0 57e2 52d9 8db0 65e6  .J....3.W.R...e.
-00001540: 0d8a 1289 a638 c1d2 53bf b143 8c1d abbb  .....8..S..C....
-00001550: 4388 e5d7 3d32 e24c b089 f4ee 10af 8388  C...=2.L........
-00001560: d325 4372 6025 522e b443 6288 cbc2 6520  .%Cr`%R..Cb...e 
-00001570: 84da f2cd de6d afc3 a86b d53d 7c64 2361  .....m...k.=|d#a
-00001580: 5b20 ea30 7e88 a9e5 c6cb 682e 51ec 5239  [ .0~.....h.Q.R9
-00001590: 4431 351d be8b 64e4 3272 7fc1 4726 ae2f  D15...d.2r..G&./
-000015a0: 2444 7a8a 29f3 fa63 2c84 4be6 3a87 f51a  $Dz.)..c,.K.:...
-000015b0: 41bf 0a0c e30e fb1e 5dc4 3692 4b72 e8d2  A.......].6.Kr..
-000015c0: b98b 1833 913d 76d8 8d50 3c73 da4c 92c8  ...3.=v..P<s.L..
-000015d0: c47e 260e 2145 9177 8349 177c 8fd9 3b44  .~&.!E.w.I.|..;D
-000015e0: 3d43 1c50 b231 dcb7 09b6 c2fd 6622 b805  =C.P.1......f"..
-000015f0: e46a 9a94 2788 fa65 ce1d b1bc 8c99 bd1f  .j..'..e........
-00001600: 1774 82b0 8b65 da3c b6d8 b5cd 8933 3b3a  .t...e.<.....3;:
-00001610: f3a9 95da bb18 5374 8cc6 187b b73e 7358  ......St...{.>sX
-00001620: d061 33cb e7b9 d157 2260 951d ec4a ac2b  .a3....W"`...J.+
-00001630: c8ce 55f5 9c60 0165 92aa 6bd6 2972 9708  ..U..`.e..k.)r..
-00001640: 2b65 f7f1 946d b067 6f71 8278 1628 8911  +e...m.goq.x.(..
-00001650: dfa4 f91a 44dd 4a5d 38e5 9c54 7a9d 8e0e  ....D.J]8..Tz...
-00001660: 4de0 3502 e51f e48b d329 d705 e830 92bb  M.5......)...0..
-00001670: bf49 eb8d 0859 6797 7a16 ee7c 5d70 2b7e  .I...Yg.z..|]p+~
-00001680: 6fb3 c760 5fde 3ded be04 197c 6a19 20f6  o..`_.=....|j. .
-00001690: b7f6 cd10 516b 823c 6186 080a 0c17 dd82  ....Qk.<a.......
-000016a0: 8815 fe5c 449d ab5a 6cee 949b d89b 360f  ...\D..Zl.....6.
-000016b0: 0314 4656 bd13 93e4 8dc5 cf89 b227 fc77  ..FV.........'.w
-000016c0: ca1e 7701 7306 058f 5bf1 fb94 3a9b 2865  ..w.s...[...:.(e
-000016d0: e744 81b3 09f7 1f2c 6b7a 689e dcc0 7092  .D.....,kzh...p.
-000016e0: ac73 d679 5573 5ed5 f8ff fbaa 66d3 5e3e  .s.yUs^.....f.^>
-000016f0: af65 ce6b 99f3 5ac6 f5f6 f541 6a99 bc7c  .e.k..Z....Aj..|
-00001700: 81ca 26ef f2e8 9e4f bcb1 e533 2194 eecb  ..&....O...3!...
-00001710: 05c5 bb42 777d 04bc d18c 0730 a8db 51ba  ...Bw}.....0..Q.
-00001720: 27b9 6a01 ce22 f89a 3598 2cdc 9423 2de3  '.j.."..5.,..#-.
-00001730: 7126 3f27 32da 8fd0 0c5a 4365 ddc0 9c8a  q&?'2....ZCe....
-00001740: 4cf5 5478 3326 a063 a487 752b 159f d0ad  L.Tx3&.c..u+....
-00001750: fb4e f378 8f8d d34e 67b9 acba 9aa9 0b05  .N.x...Ng.......
-00001760: 92f9 7829 5c8d 4397 4aa6 e85a 3def dead  ..x)\.C.J..Z=...
-00001770: d4eb 7ee8 5477 5997 0628 d9d3 1861 4c66  ..~.TwY..(...aLf
-00001780: 1b51 7518 515f 0e42 145e 6784 5ed9 9958  .Qu.Q_.B.^g.^..X
-00001790: d174 58d1 50ea 97a1 5a46 71e5 0a30 6d15  .tX.P...ZFq..0m.
-000017a0: 1578 e5f6 e045 bde5 8741 da41 8666 1c94  .x...E...A.A.f..
-000017b0: e763 15a7 b499 bc8c ae0a ce99 467a 9333  .c..........Fz.3
-000017c0: a999 0150 622f 3320 8f74 53d9 ba71 796a  ...Pb/3 .tS..qyj
-000017d0: 7569 aabd 45a4 2d23 8c74 b38d 30d2 3082  ui..E.-#.t..0.0.
-000017e0: 17e1 2c3b cd96 fb59 c6ba 9987 d432 4fb9  ..,;...Y.....2O.
-000017f0: 62b9 1b72 33ea 8d0f 116b 4522 27b8 8126  b..r3....kE"'..&
-00001800: 2653 d0c4 3b6e f9b5 6a08 b72a 2334 6bf9  &S..;n..j..*#4k.
-00001810: 13e8 18c3 d778 06b9 23d4 5b17 a253 b876  .....x..#.[..S.v
-00001820: 1949 9e6e f877 6196 1917 b287 4494 3a5c  .I.n.wa.....D.:\
-00001830: 934e ca06 3191 987b 94c4 2d5f 2d7f 950d  .N..1..{..-_-...
-00001840: 34d1 1ca2 6d2b 5780 103e 5ae3 9a40 2b1f  4...m+W..>Z..@+.
-00001850: 9b71 1074 3bc8 7832 c123 6986 dd18 519e  .q.t;.x2.#i...Q.
-00001860: 4e1f 81e1 53ae 70fe aac5 df1d ac24 d91c  N...S.p......$..
-00001870: c2bd 1f8d 8fbd 033a e737 11a4 5858 2f2b  .......:.7..XX/+
-00001880: 078e 8980 8b83 72ea cd31 819b b015 91e5  ......r..1......
-00001890: f977 e260 ca68 d7bc 8ad2 3994 8e23 3a8b  .w.`.h....9..#:.
-000018a0: 5076 a298 649e c235 89ae ccd1 4f2b 1f18  Pv..d..5....O+..
-000018b0: 4fd9 9ac1 a1eb 2e3c 98aa 03f6 bd4f dd37  O......<.....O.7
-000018c0: 1fd5 ca73 0669 e667 a6c5 2aea d474 93e9  ...s.i.g..*..t..
-000018d0: 873b e40d abf2 43d4 b22a a56e fd4e 2d72  .;....C..*.n.N-r
-000018e0: ae6b 2eb9 0e12 d579 4abc e1d4 7d8b 03c1  .k.....yJ...}...
-000018f0: 302d 9fcc 324d 59bc 4ec3 8ab3 b351 dbb4  0-..2MY.N....Q..
-00001900: 332c 080c 4fd4 36f8 6d75 4638 3df1 ae27  3,..O.6.muF8=..'
-00001910: 3fc8 9dcc 5a75 402c eb4a 9df8 faca dcbc  ?...Zu@,.J......
-00001920: d566 0777 813c 7a70 7f38 a752 e850 426f  .f.w.<zp.8.R.PBo
-00001930: 9723 28fa d21b c894 3660 8bdc 9359 8d08  .#(.....6`...Y..
-00001940: dfbc 3927 2dff 7e29 6c07 dd4a d82d 941a  ..9'-.~)l..J.-..
-00001950: 61bf 1054 8352 a111 b6ab 8576 1856 cbfd  a..T.R.....v.V..
-00001960: b05c ea75 2a0f e060 9151 5c0e d3eb fa01  .\.u*..`.Q\.....
-00001970: 5c61 d045 7669 afc7 d72e eee3 e52d cd85  \a.Evi.......-..
-00001980: 118b 8b4c 5fcc 17b5 e1fa e2be 5cd9 7c71  ...L_.......\.|q
-00001990: ef11 209d fbb5 caa0 596d 766a 8566 b53d  .. .....Ymvj.f.=
-000019a0: 2804 bd4e a3d0 ecd6 3a85 5ead 5bef 0d7a  (..N....:.^.[..z
-000019b0: ddb0 d11c 3cf0 bd23 0d0e dad5 6e50 eb37  ....<..#....nP.7
-000019c0: 0ab5 72b7 5b08 6a25 657e a359 a807 954a  ..r.[.j%e~.Y...J
-000019d0: 3ba8 b71b fda0 fd20 2b63 60e5 297d 64be  ;...... +c`.)}d.
-000019e0: 00f7 6abb b6ff 0100 00ff ff03 0050 4b03  ..j..........PK.
-000019f0: 0414 0006 0008 0000 0021 0013 7c8b 5bf1  .........!..|.[.
-00001a00: 0800 0076 4600 000d 0000 0078 6c2f 7374  ...vF......xl/st
-00001a10: 796c 6573 2e78 6d6c c45c 596f e336 107e  yles.xml.\Yo.6.~
-00001a20: 2fd0 ff20 08e8 a3a3 dbb6 02db 45ec 44ed  /.. ........E.D.
-00001a30: 02db 6d81 4dd1 beca b2ec a8d1 6148 f2d6  ..m.M.......aH..
-00001a40: 69d1 ffde 19ea 20e9 934e 6413 c16e 2cc5  i..... ..Nd..n,.
-00001a50: fce6 fa38 438e 8ed1 8fdb 2456 be85 7911  ...8C.....$V..y.
-00001a60: 65e9 5835 ee74 5509 d320 5b44 e96a acfe  e.X5.tU.. [D.j..
-00001a70: feec f586 aa52 947e baf0 e32c 0dc7 ea5b  .....R.~...,...[
-00001a80: 58a8 3f4e beff 6e54 946f 71f8 f525 0c4b  X.?N..nT.oq..%.K
-00001a90: 0520 d262 acbe 94e5 fa5e d38a e025 4cfc  . .b.....^...%L.
-00001aa0: e22e 5b87 29fc 6599 e589 5fc2 61be d28a  ..[.).e..._.a...
-00001ab0: 751e fa8b 0207 25b1 66ea 7a5f 4bfc 2855  u.....%.f.z_K.(U
-00001ac0: 2b84 fb24 1001 49fc fc75 b3ee 0559 b2f6  +..$..I..u...Y..
-00001ad0: cb68 1ec5 51f9 46b0 5425 09ee 3fad d22c  .h..Q.F.T%..?..,
-00001ae0: f7e7 31a8 ba35 6c3f 50b6 463f 3795 6dde  ..1..5l?P.F?7.m.
-00001af0: 0821 67f7 e424 5190 6745 b62c ef00 57cb  .!g..$Q.gE.,..W.
-00001b00: 96cb 2808 f7d5 7535 57f3 038a 04c8 ef43  ..(...u5W......C
-00001b10: 321c 4d37 39db b7f9 3b91 6c2d 0fbf 4518  2.M79...;.l-..E.
-00001b20: 3e75 325a 6669 5928 41b6 494b 08a6 0b9a  >u2ZfiY(A.IK....
-00001b30: a20f ee5f d3ec efd4 c3bf c1d9 fa6b 9351  ..._.........k.Q
-00001b40: f18f f2cd 8fe1 8ca1 6a93 5190 c559 ae94  ........j.Q..Y..
-00001b50: 103b 701d 3993 fa49 587d 63e6 c7d1 3c8f  .;p.9..IX}c...<.
-00001b60: f06b 4b3f 89e2 b7ea b489 2748 b8eb ef25  .kK?......'H...%
-00001b70: 1138 1f4f 6aa8 48a5 8e04 39c3 3d7b 2c3c  .8.Oj.H...9.={,<
-00001b80: b367 8ff2 395a bd94 e7ad f2ff 3a60 d51c  .g..9Z......:`..
-00001b90: 6d6f 3ce8 084a 7ca7 0739 59c4 162e 5a87  mo<..J|..9Y...Z.
-00001ba0: adeb 42d6 3e33 3a95 7588 81f9 6a3e 563d  ..B.>3:.u...j>V=
-00001bb0: 0f72 83a1 eb07 c3d6 210d 6b61 ee4c 0779  .r......!.ka.L.y
-00001bc0: 3713 e60c 6e66 99e5 59de a053 cb38 2e32  7...nf..Y..S.8.2
-00001bd0: fca8 5d89 022d af4b 579e 11e8 3d0c 1e6f  ..]..-.KW...=..o
-00001be0: e6ce ee85 1db3 ae4e c4b7 9a01 38e1 baf5  .......N....8...
-00001bf0: 62c4 e6c7 7d9e 0c3c fcb9 054f 6e5c d2ae  b...}..<...On\..
-00001c00: 18b1 8f17 6452 970b 28cc 511c b7eb 04cb  ....dR..(.Q.....
-00001c10: c625 019c 998c 6045 5586 79ea c181 527f  .%....`EU.y...R.
-00001c20: 7e7e 5bc3 8220 85c5 1f06 4bab be77 e6db  ~~[.. ....K..w..
-00001c30: abdc 7f33 4c52 14c5 0614 591c 2d50 8bd5  ...3LR....Y.-P..
-00001c40: 8c2c 43ea 6432 eb3f 79b3 2722 97d1 4c54  .,C.d2.?y.'"..LT
-00001c50: 8b23 a09e 371b 5c01 f469 eace bad7 74e6  .#..7.\..i....t.
-00001c60: ba5d 839a 1efc 740c fae0 e04f e7e6 43a8  .]....t....O..C.
-00001c70: 3af3 699d 06ec ae94 6cf1 9432 c2d5 b67e  :.i.....l..2...~
-00001c80: 3770 5d77 68f4 87c3 a16b 5b86 6d13 27cf  7p]wh....k[.m.'.
-00001c90: 6b46 47e9 22dc 868b b1da efcc 4dfb 1a38  kFG.".......M..8
-00001ca0: a081 6b0d ddbe 098a e8f6 9088 baa9 0616  ..k.............
-00001cb0: 2830 709c a163 b8a6 0dff 48e2 bfbe 065d  (0p..c....H....]
-00001cc0: fbd4 5165 4795 d140 5254 190d 2445 95ac  ..QeG..@RT..$E..
-00001cd0: 5bb5 0e32 7f3d 53fa d2a3 ca68 2029 aa8c  [..2.=S....h )..
-00001ce0: 0692 a23a e838 030f a447 95d1 4052 5419  ...:.8...G..@RT.
-00001cf0: 0d24 4595 f45c 3a9c abd0 7694 5c57 190d  .$E..\:...v.\W..
-00001d00: 2445 95d1 4052 543b 5b7c d619 183a 9292  $E..@RT;[|...:..
-00001d10: a3ca 6820 29aa 8c06 92a2 0a3d fe2a 0a3d  ..h )......=.*.=
-00001d20: fdce b071 d56a 0f6c 7d60 3b66 ffd8 82ed  ...q.j.l}`;f....
-00001d30: f8b2 996c f060 4b39 cff2 055c 4668 9bcf  ...l.`K9...\Fh..
-00001d40: 3a6c e7aa 7393 511c 2e4b d83c e6d8 6e85  :l..s.Q..K.<..n.
-00001d50: df65 b686 ffe7 5959 42af 7d32 5a44 fe2a  .e....YYB.}2ZD.*
-00001d60: 4bfd 18b7 97cd 0881 9170 5902 ae40 8cd5  K........pY..@..
-00001d70: f225 0a5e 4118 d712 adf4 ad44 5c4b 424b  .%.^A......D\KBK
-00001d80: e51d 1792 fad6 91e8 245c 449b 64df ba56  ........$\D.d..V
-00001d90: f641 0a81 1bd1 b7e7 0d67 7c88 970f 2a17  .A.......g|...*.
-00001da0: d69b 6fda a1d1 307e 75f8 0447 9050 9348  ..o...0~u..G.P.H
-00001db0: 0b0e 004e 3494 101c d185 8db4 5b29 6a23  ...N4.......[)j#
-00001dc0: 3342 cc46 6680 a08d cc88 8e58 b4c8 3670  3B.Ff......X..6p
-00001dd0: 456c 37c0 9e37 d475 b241 bb98 2f87 014f  El7..7.u.A../..O
-00001de0: 7bf3 ec98 7d7f 9e1d 72c0 a367 c774 c19b  {...}...r..g.t..
-00001df0: a989 3f64 a20b ce0d 6684 186f 9801 82bc  ..?d....f..o....
-00001e00: 6146 bc8f 3707 271e d737 39ef 6fee eba7  aF..7.'..79.o...
-00001e10: d4a8 533d 548e 208c e3af 98cb ff5c b6e5  ..S=T. ......\..
-00001e20: 039a 2793 d176 a9a4 9bc4 4bca 4fd0 3781  ..'..v....K.O.7.
-00001e30: a285 1715 9b8f d0a1 ac3f 56a5 a23a 8012  .........?V..:..
-00001e40: 726c 9009 e30f 0f52 fcf5 3a7e fbb2 49e6  rl.....R..:~..I.
-00001e50: 61ee 91ab d544 1a39 8b9d 507a 3425 358e  a....D.9..Pz4%5.
-00001e60: 1e3f c4d1 2a4d 42d2 fe51 2b98 dff2 ac0c  .?..*MB..Q+.....
-00001e70: 8392 5c4d 27ad e063 fa58 47f4 316a 2011  ..\M'..c.XG.1j .
-00001e80: 7d3e 22df 3e22 1ffc 24ec 8f8f c887 f6c2  }>".>"..$.......
-00001e90: c178 805f a4ca 079e 49e1 036c cc1b 7f40  .x._....I..l...@
-00001ea0: 0858 529f d2a7 4b46 c226 b2d1 0082 2043  .XR...KF.&.... C
-00001eb0: 03d8 f034 1a00 3d65 6800 8bf3 4603 2028  ...4..=eh...F. (
-00001ec0: d500 d439 c18a 8fcc 0303 135b 9d98 8003  ...9.......[....
-00001ed0: 5424 c8bf 9648 c831 0745 5ed1 ca63 e917  T$...H.1.E^..c..
-00001ee0: 4cbe c974 3798 7c0b 44a7 6e86 836b b9f9  L..t7.|.D.n..k..
-00001ef0: 588a 9595 6298 b0c3 4ca3 2e80 8353 3180  X...b...L....S1.
-00001f00: aadb 4dc9 338e e57c 690e 6192 2ee8 403d  ..M.3..|i.a...@=
-00001f10: 0269 e036 ac64 722e c894 91f1 1852 602a  .i.6.dr......R`*
-00001f20: 92ad 02a8 235b 0549 e5d7 60b8 80d9 4ab6  ....#[.I..`...J.
-00001f30: 1b24 5560 968f 5c09 3e9d 24ba 5c08 b12a  .$U`..\.>.$.\..*
-00001f40: 7025 f986 2ab0 64e0 ea95 1c37 70f5 428e  p%..*.d....7p.B.
-00001f50: 0af2 f3a3 292b 3f32 6480 06ad eccc 60ca  ....)+?2d.....`.
-00001f60: 4a90 cc0e 497e 7e34 65e5 4796 0cf2 13a4  J...I~~4e.G.....
-00001f70: 292b 4132 6490 9f1f 4d59 f991 2583 fc04  )+A2d...MY..%...
-00001f80: 69c9 5f40 5af2 f3a3 75e5 fca8 b10d d3aa  i._@Z...u.......
-00001f90: 7dca 744e e169 8ef7 744e 95ed f26c 0b95  }.tN.i..tN...l..
-00001fa0: e954 ec06 ba19 5d6d 9b98 7e08 6a03 4f8f  .T....]m..~.j.O.
-00001fb0: 546d 52e5 efdc 5f3f 875b 7c38 8534 cfb7  TmR..._?.[|8.4..
-00001fc0: cb1d 5d6d 6cc0 9c6d f3b6 ca1e daa5 11e4  ..]ml..m........
-00001fd0: 635d 5783 d9f1 59bb 4584 3702 9f97 413d  c]W...Y.E.7...A=
-00001fe0: 2b19 5523 f8ba d85d 3aef 0243 f94e 736b  +.U#...]:..C.Nsk
-00001ff0: f0c5 e633 ddbb d3f4 38ec d94e ad17 d6a5  ...3....8..N....
-00002000: 23e3 85a7 46c3 a38f 5a8b 022f 9d27 c738  #...F...Z../.'.8
-00002010: dcc9 a4db 9b26 244d 4162 622e f0f0 9777  .....&$MAbb....w
-00002020: da34 a6e0 8ded 63d5 d47f 507a ca43 10c0  .4....c...Pz.C..
-00002030: 0515 6061 351b f121 b6f9 268a e186 05cc  ..`a5..!..&.....
-00002040: 4f58 6182 4d01 17b7 a7d5 c93a 939c c282  OXa.M......:....
-00002050: 745c 6199 38e1 192c 58c1 5d8a 0508 3516  t\a.8..,X.]...5.
-00002060: 2e3a 182c 20dc a558 20be c222 358b 62c1  .:., ..X .."5.b.
-00002070: b5af 8bb1 6021 5863 e192 90c1 827c 77a9  ....`!Xc.....|w.
-00002080: 5e30 a4c6 e27d ef08 fade 3e14 47b2 7762  ^0...}....>.G.wb
-00002090: fc05 0116 d18b c5a2 71c4 a537 8305 265f  ........q..7..&_
-000020a0: 8a45 e388 2b37 060b 4cbe 148b c611 0b3f  .E..+7..L......?
-000020b0: e37b 1072 2916 8d23 aeab 192c a0db a558  .{.r)..#...,...X
-000020c0: 6d1c 6d4c c714 cb11 f47d ff60 1c71 7dc5  m.mL.....}.`.q}.
-000020d0: f84b 90ab 2c16 8d23 cf55 4b90 ab2c 168d  .K..,..#.UK..,..
-000020e0: 23cf 5534 59c4 5f2c 168d 239f 276c c13c  #.U4Y._,..#.'l.<
-000020f0: c162 d138 f279 c216 cc13 2c16 8d23 ef7b  .b.8.y....,..#.{
-00002100: 47d0 f7bb 1995 67bc 29c8 f80a 85c6 8ee7  G.....g.).......
-00002110: 3aae a544 fc5d a1d0 a8f1 2cb7 0459 5ea1  :..D.]....,..Y^.
-00002120: d078 f1fc b605 f95d a1d0 48f1 59c5 16cc  .x.....]..H.Y...
-00002130: 2a15 0acd 99bc 77b1 b48a f865 ea2f 9aac  *.....w....e./..
-00002140: cb13 c614 7409 3ca2 1d6c 6278 201e 9e03  ....t.<..lbx ...
-00002150: 6f4a 274f 176c db88 a832 7b09 8357 6506  oJ'O.l...2{..We.
-00002160: 3765 b440 fc7c c032 2a02 f4b4 5dc7 7eea  7e.@.|.2*...].~.
-00002170: 9759 fea6 e0a2 bf85 e383 ee08 c2fd 9465  .Y.............e
-00002180: ad8f 7804 ec41 8828 f433 bc7c 00de 6ba0  ..x..A.(.3.|..k.
-00002190: b48b 0b9e c3b8 64be 04a6 9d0b bc7b b08f  ......d......{..
-000021a0: 7f09 4c3b 1978 fe19 8299 a231 aa9d 0d7c  ..L;.x.....1...|
-000021b0: 52c5 f593 8836 9fd2 f5a6 8d10 9f4b b174  R....6.......K.t
-000021c0: 8b40 7c8e d2d7 70c1 3387 f730 f6cc 4490  .@|...p.3..0..D.
-000021d0: be84 9b32 f75b feed 242c 41c7 7cc1 5b79  ...2.[..$,A.|.[y
-000021e0: 5a0c 3e45 903b 7376 d78c 5fe0 ce9d 96a3  Z.>E.;sv.._.....
-000021f0: 3b5e 1474 c1af 9b92 7123 b99e 466b 25b6  ;^.t....q#..Fk%.
-00002200: 6e45 ac7f 8e4a b859 af99 c45c b9c5 2ba8  nE...J.Y...\..+.
-00002210: 4210 5949 4d47 4232 251b 9ecb 14c2 f8c3  B.YIMGB2%.......
-00002220: cf53 9c2d dcd4 dde1 e811 8b68 8702 56ff  .S.-.......h..V.
-00002230: 8b2d bdad 8bf8 bdc4 d773 901b beda fd00  .-.......s......
-00002240: b877 112e fd4d 5c3e b77f 1cab f4f3 2fe4  .w...M\>....../.
-00002250: 3658 2053 fdad dfa2 6f59 4920 c62a fd4c  6X S....oYI .*.L
-00002260: 5ee7 00b3 18ee 0283 74f3 b980 7b56 e1b7  ^.......t...{V..
-00002270: b2c9 a3b1 faef d374 e03e 3e79 666f a84f  .......t.>>yfo.O
-00002280: 873d db0a 9d9e eb4c 1f7b 8e3d 9b3e 3e7a  .=.....L.{.=.>>z
-00002290: ae6e eab3 ff98 9784 7ce0 1521 e49d 26d0  .n......|..!..&.
-000022a0: d830 ecfb 2286 1789 e4b5 b1b5 f25f e9b9  .0.."........_..
-000022b0: b1ca 1c54 ea93 be08 a8cd eaee 9a7d fdc1  ...T.........}..
-000022c0: 31f4 9e67 e946 cfee fbc3 deb0 6f39 3dcf  1..g.F......o9=.
-000022d0: 31cc c7be 3d7d 723c 87d1 dd79 e7ab 4474  1...=}r<...y..Dt
-000022e0: cd30 aa97 92a0 f2ce 7d19 2561 1ca5 4dac  .0......}.%a..M.
-000022f0: 9a08 b167 2148 7078 c208 ad89 8446 5f18  ...g!Hpx.....F_.
-00002300: 33f9 1f00 00ff ff03 0050 4b03 0414 0006  3........PK.....
-00002310: 0008 0000 0021 00b3 7cd6 e18a 0300 0030  .....!..|......0
-00002320: 0a00 0014 0000 0078 6c2f 7368 6172 6564  .......xl/shared
-00002330: 5374 7269 6e67 732e 786d 6c8c 56db 4e1b  Strings.xml.V.N.
-00002340: 3110 7daf d47f 18ed 1348 85d0 aaa2 5594  1.}......H....U.
-00002350: 0451 a20a 2482 10a1 95fa b472 d64e 6275  .Q..$......r.Nbu
-00002360: 7da9 3dbb 90bf efd8 de96 b2de 50f2 92c4  }.=.........P...
-00002370: 333b 379f 7366 2767 8faa 8656 382f 8d9e  3;7.sf'g...V8/..
-00002380: 16ef 8f4f 0a10 ba32 5cea cdb4 f876 fff5  ...O...2\....v..
-00002390: e873 011e 99e6 ac36 5a4c 8b9d f0c5 d9ec  .s.....6ZL......
-000023a0: ed9b 89f7 08f4 acf6 d362 8b68 c7a3 91af  .........b.h....
-000023b0: b642 317f 6cac d064 591b a718 d25f b719  .B1.l..dY...._..
-000023c0: 79eb 04e3 7e2b 04aa 7af4 e1e4 e474 a498  y...~+..z....t..
-000023d0: d405 54a6 d138 2d3e 5196 46cb 5f8d b848  ..T..8->Q.F._..H
-000023e0: 07a7 1f8b d9c4 cbd9 0467 2d73 92ad 6a51  .........g-s..jQ
-000023f0: 6aa6 c464 84b3 c928 1892 918b b5d4 12a9  j..d...(........
-00002400: f8be c59b c655 99bf 7864 cad6 d9b1 3628  .....U..xd....6(
-00002410: 7c3f 8216 f860 dccf feb1 7506 4d65 eafe  |?...`....u.Me..
-00002420: f96d 770e ba51 2be1 fae6 73ef d90e 7067  .mw..Q+...s...pg
-00002430: b3e4 9bc6 5b51 65f5 d3d9 9077 f02d ad93  ....[Qe....w.-..
-00002440: 8ab9 ddd0 3325 e39c 06d2 6669 e283 5c38  ....3%....fi..\8
-00002450: d9b2 21b3 45c9 fbf1 5ae9 256a 930d ddb1  ..!.E...Z.%j....
-00002460: 078e 43c9 9dc9 672b b56d b05c cb3d 3778  ..C...g+.m.\.=7x
-00002470: ceb9 e0b0 dac1 72be b8e8 c7bc f206 3843  ......r.......8C
-00002480: 0109 4c7d f38d 41d0 a212 345a 276b 9aee  ..L}..A...4Z'k..
-00002490: 5624 f7f0 a366 2ba8 0876 48e1 3b03 3b86  V$...f+..vH.;.;.
-000024a0: 1031 053b ee47 93da a36b 94d0 796b 5c85  .1.;.G...k..yk\.
-000024b0: 999b 9089 8851 8692 50e6 68f4 c18f 8cac  .....Q..P.h.....
-000024c0: 7454 95b4 b8d7 7379 7179 7e77 0b57 f350  tT....syqy~w.W.P
-000024d0: 0c34 b636 2c50 2e14 9d35 49b0 07b3 0616  .4.6,P...5I.....
-000024e0: 0134 e010 0de5 1056 12e6 f6f7 7547 d715  .4.....V....uG..
-000024f0: 4207 6850 3b19 876e 1203 8e28 83dc 689a  B.hP;..n...(..h.
-00002500: 63e2 28f8 4822 909c 6625 d732 07fb b20b  c.(.H"..f%.2....
-00002510: 3888 f7ef 0155 1d4b e0c0 0a07 7f28 d51d  8....U.K.....(..
-00002520: d220 0e49 199c 13de 1a1d e782 a64b da9f  . .I.........K..
-00002530: 4e37 c86b baec 6f71 8a70 6f72 6e06 6cc1  N7.k..oq.porn.l.
-00002540: 1756 fddc 38d2 170e 0bba 4052 953a e3fc  .V..8.....@R.:..
-00002550: 42b8 0df5 b976 46c1 f57c b1dc 07cc 6e32  B....vF..|....n2
-00002560: 1034 09d8 6ae5 442b 8956 b90c 2dd3 a848  .4..j.D+.V..-..H
-00002570: 2f6a e233 39c0 3ce0 f9e0 077d 8e16 8ba3  /j.39.<....}....
-00002580: f9fc b0df 5274 20c5 8500 31a0 271e b6b2  ....Rt ...1.'...
-00002590: da46 7e64 80f6 0281 6693 3c70 2b3d 7019  .F~d....f.<p+=p.
-000025a0: d390 3a80 136b 12f6 7f73 dd5f 5e8e 178b  ..:..k...s._^...
-000025b0: f172 9925 bd08 4c09 e585 a424 f8ca 0660  .r.%..L....$...`
-000025c0: 04de 44fe 065a b1d7 457a 76f7 63b8 1d96  ..D..Z..Ezv.c...
-000025d0: aa9e 17a9 c0a0 68f5 dce6 7be5 eb96 3994  ......h...{...9.
-000025e0: 95b4 4ce3 0bb8 fc4a 2a94 eeec 2fa1 6263  ..L....J*.../.bc
-000025f0: 8980 4128 0cfc 074a b184 d740 248a 4127  ..A(...J...@$.A'
-00002600: 1a25 17c8 640e b708 b1b4 a9c6 c402 a948  .%..d..........H
-00002610: 81de 0189 744b 3ffa b818 727e d187 36c1  ....tK?...r~..6.
-00002620: ffc2 bc26 153e a2cd 77c3 b36a 5ac9 5b96  ...&.>..w..jZ.[.
-00002630: 6dc4 672e 3c2c 0d45 cd85 6fde 7d67 1bec  m.g.<,.E..o.}g..
-00002640: 8e5e 1312 fbc2 c200 4563 0b17 34a4 8971  .^......Ec..4..q
-00002650: 6974 42ff e218 6a8f 0dcf 32a5 2b2f 494f  itB...j...2.+/IO
-00002660: cbbc b924 a9c1 36f4 d2b1 6c56 4a62 d82b  ...$..6...lVJb.+
-00002670: b4b6 8614 9bde 2688 3a8c a8d9 eda1 f8e7  ......&.:.......
-00002680: 0964 694d 3120 baea 8115 46f2 4aa2 e29f  .diM1 ....F.J...
-00002690: 3f4d 3a19 f656 b7cc 6281 fdae 53d5 be59  ?M:..V..b...S..Y
-000026a0: 0ded 82a7 2d50 faa8 7df9 5e0f fd7a b3c6  ....-P..}.^..z..
-000026b0: 07e6 44d9 bd13 3ee5 18d1 1bdf ec37 0000  ..D...>......7..
-000026c0: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
-000026d0: 0021 003b 6d32 4bc1 0000 0042 0100 0023  .!.;m2K....B...#
-000026e0: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
-000026f0: 2f5f 7265 6c73 2f73 6865 6574 312e 786d  /_rels/sheet1.xm
-00002700: 6c2e 7265 6c73 848f c18a c230 1445 f703  l.rels.....0.E..
-00002710: fe43 787b 93d6 850c 4353 3722 b855 e703  .Cx{....CS7".U..
-00002720: 62fa da06 db97 90f7 14fd 7bb3 1c65 c0e5  b.........{..e..
-00002730: e570 cfe5 369b fb3c a91b 660e 912c d4ba  .p..6..<..f..,..
-00002740: 0285 e463 1768 b0f0 7bda 2dbf 41b1 38ea  ...c.h..{.-.A.8.
-00002750: dc14 092d 3c90 61d3 2ebe 9a03 4e4e 4a89  ...-<.a.....NNJ.
-00002760: c790 5815 0bb1 8551 24fd 18c3 7ec4 d9b1  ..X....Q$...~...
-00002770: 8e09 a990 3ee6 d949 8979 30c9 f98b 1bd0  ....>..I.y0.....
-00002780: acaa 6a6d f25f 07b4 2f4e b5ef 2ce4 7d57  ..jm._../N..,.}W
-00002790: 833a 3d52 59fe ec8e 7d1f 3c6e a3bf ce48  .:=RY...}.<n...H
-000027a0: f2cf 8449 3990 603e a248 39c8 45ed f280  ...I9.`>.H9.E...
-000027b0: 6241 eb77 f69e 6b7d 0e04 a66d cccb f3f6  bA.w..k}...m....
-000027c0: 0900 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
-000027d0: 0000 0021 00cf e047 b4c2 0100 002c 1500  ...!...G.....,..
-000027e0: 0027 0000 0078 6c2f 7072 696e 7465 7253  .'...xl/printerS
-000027f0: 6574 7469 6e67 732f 7072 696e 7465 7253  ettings/printerS
-00002800: 6574 7469 6e67 7331 2e62 696e ec54 cd4a  ettings1.bin.T.J
-00002810: dc50 183d 33b1 ede8 a60e 14dc 7451 a42b  .P.=3.......tQ.+
-00002820: 71e8 0c93 a9dd 5599 a476 4ad2 8424 33b8  q.....U..vJ..$3.
-00002830: 7131 7452 088c c990 4444 a582 f81a 3e48  q1tR....DD....>H
-00002840: 972e 5df6 01ba 7621 c507 70a3 e7a6 33d8  ..]...v!..p...3.
-00002850: 96a1 8ce0 46f8 eee5 bbdf cf3d 3937 f790  ....F......=97..
-00002860: 7c36 227c 418a 0419 ed2b 72bc 82cb 3c42  |6"|A....+r...<B
-00002870: 5cc4 39ab aa62 e003 a68d d29c f6f4 27dc  \.9..b........'.
-00002880: 17da 9b12 d4bc 5c48 2a03 fae7 d82a 97e9  ......\H*....*..
-00002890: b7ca 1a57 0b21 d972 aee9 5496 fb15 4b63  ...W.!.r..T...Kc
-000028a0: b8f2 659a f237 1c9b 1d5f ff93 c9e8 7cee  ..e..7..._....|.
-000028b0: 2ee3 1caf b5d5 eafb edc3 a3ff 9df2 a4d8  ................
-000028c0: 9c2f b81e e015 85e2 112a 30f9 ae66 79f5  ./.......*0..fy.
-000028d0: 7382 7c3b f8a4 b08b f88e 43d4 f10e 3aff  s.|;......C...:.
-000028e0: 923a 1a5c 3750 8389 b768 b256 a319 58e3  .:.\7P...h.V..X.
-000028f0: ac11 d364 dd64 5467 ae33 6fd0 b799 35d1  ...d.dTg.3o...5.
-00002900: 2ab2 6f64 f44c dfb0 2c74 e328 0d33 15b9  *.od.L..,t.(.3..
-00002910: fd51 98fa d141 08cb 0c02 d383 9346 619c  .Q...A.......Fa.
-00002920: f7f3 2889 e13a 5ee0 6d74 0278 6196 0c77  ..(..:^.mt.xa..w
-00002930: 8b1a 4367 a4a2 06da c930 49ed 6410 fe8e  ..Cg.....0I.d...
-00002940: febe dd6a 15e8 e986 3db9 fbe9 c268 f925  ...j....=....h.%
-00002950: 21bf 681a edba e454 f48b 3dfb e4ea d9c7  !.h....T..=.....
-00002960: a5b3 d6f1 0fd6 acf1 1e2a 775c 0aab f295  .........*w\....
-00002970: b157 f93a ada7 f245 f0fe 09fb cc2e 76d8  .W.:...E......v.
-00002980: 0354 67e9 b2df a86e e0a2 cf28 c31e f753  .Tg....n...(...S
-00002990: 0c08 fe17 e970 2f9e 11db 26c7 3e46 e4f7  .....p/...&.>F..
-000029a0: f984 3a4f 75b2 9c35 19a2 8028 200a 8802  ..:Ou..5...( ...
-000029b0: a280 2820 0a88 02a2 8028 200a 8802 a280  ..( .....( .....
-000029c0: 2820 0acc a2c0 2d00 0000 ffff 0300 504b  ( ....-.......PK
-000029d0: 0304 1400 0600 0800 0000 2100 cb95 14e3  ..........!.....
-000029e0: 4e01 0000 7102 0000 1100 0801 646f 6350  N...q.......docP
-000029f0: 726f 7073 2f63 6f72 652e 786d 6c20 a204  rops/core.xml ..
-00002a00: 0128 a000 0100 0000 0000 0000 0000 0000  .(..............
-00002a10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002a20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002a30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002a40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002a50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000b90: 0000 0000 0000 0000 ac52 4d4b c430 10bd  .........RMK.0..
+00000ba0: 0bfe 8730 779b 7615 11d9 742f 22ec 55eb  ...0w.v...t/".U.
+00000bb0: 0f08 c9b4 29db 2621 337e f4df 1b2a ba5d  ....).&!3~...*.]
+00000bc0: 58d6 4b2f 036f 8679 efcd c776 f735 0ee2  X.K/.o.y...v.5..
+00000bd0: 0313 f5c1 2ba8 8a12 047a 136c ef3b 056f  ....+....z.l.;.o
+00000be0: cdf3 cd03 0862 edad 1e82 4705 1312 ecea  .....b....G.....
+00000bf0: ebab ed0b 0e9a 7313 b93e 92c8 2c9e 1438  ......s..>..,..8
+00000c00: e6f8 2825 1987 a3a6 2244 f4b9 d286 346a  ..(%...."D....4j
+00000c10: ce30 7532 6a73 d01d ca4d 59de cbb4 e480  .0u2js...MY.....
+00000c20: fa84 53ec ad82 b4b7 b720 9a29 66e5 ffb9  ..S...... .)f...
+00000c30: 43db f606 9f82 791f d1f3 1909 493c 0d79  C.....y.....I<.y
+00000c40: 00d1 e8d4 212b f8c1 45f6 08f2 bcfc 664d  ....!+..E.....fM
+00000c50: 79ce 6bc1 a3fa 0ce5 1cab 4b1e aa35 3d7c  y.k.......K..5=|
+00000c60: 8674 2087 c847 1f7f 2992 73e5 a299 bb55  .t ..G..).s....U
+00000c70: efe1 7442 fbca 29bf dbf2 2ccb f4ef 66e4  ..tB..)...,...f.
+00000c80: c9c7 d5df 0000 00ff ff03 0050 4b03 0414  ...........PK...
+00000c90: 0006 0008 0000 0021 00bd c503 36ea 0500  .......!....6...
+00000ca0: 00a5 1700 0018 0000 0078 6c2f 776f 726b  .........xl/work
+00000cb0: 7368 6565 7473 2f73 6865 6574 312e 786d  sheets/sheet1.xm
+00000cc0: 6c9c 93db 8e9b 3010 86ef 2bf5 1d90 ef83  l.....0...+.....
+00000cd0: 3985 0d28 6455 ed2a eade 5455 b787 6bc7  9..(dU.*..TU..k.
+00000ce0: 0cc1 0ac6 a9ed 9c5a f5dd 3b76 8e6a aa28  .......Z..;v.j.(
+00000cf0: 5a04 1e83 99ef 9fc1 3fe3 c7ad ec82 3568  Z.......?.....5h
+00000d00: 2354 5f91 388c 4800 3d57 b5e8 e715 f9f6  #T_.8.H.=W......
+00000d10: 753a 1891 c058 d6d7 ac53 3d54 6407 863c  u:...X...S=Td..<
+00000d20: 4ede bf1b 6f94 5e98 16c0 0648 e84d 455a  N...o.^....H.MEZ
+00000d30: 6b97 25a5 86b7 2099 09d5 127a 5c69 9496  k.%... ....z\i..
+00000d40: cce2 ad9e 53b3 d4c0 6a9f 243b 9a44 514e  ....S...j.$;.DQN
+00000d50: 2513 3dd9 134a 7d0f 4335 8de0 f0ac f84a  %.=..J}.C5.....J
+00000d60: 426f f710 0d1d b358 bf69 c5d2 1c69 92df  Bo.....X.i...i..
+00000d70: 8393 4c2f 56cb 0157 7289 8899 e884 dd79  ..L/V..Wr......y
+00000d80: 2809 242f 5fe6 bdd2 6cd6 61df db38 633c  (.$/_...l.a..8c<
+00000d90: d86a 3c13 bcd2 a38c 7f7e a524 05d7 caa8  .j<......~.$....
+00000da0: c686 48a6 fb9a afdb 2f68 4119 3f91 aefb  ..H...../hA.?...
+00000db0: bf0b 1367 54c3 5ab8 0d3c a392 b795 140f  ...gT.Z..<......
+00000dc0: 4fac e40c 4bdf 08cb 4f30 f7b9 74b9 1275  O...K...O0..t..u
+00000dd0: 457e 4787 6380 3176 4374 1e8e 6b7f c864  E~G.c.1vCt..k..d
+00000de0: 5c0b dc61 d755 a0a1 a9c8 87b8 9c26 19a1  \..a.U.......&..
+00000df0: 93b1 37d0 7701 1b73 310f 2c9b bd42 07dc  ..7.w..s1.,..B..
+00000e00: 028a c424 f8a5 947c e5ac 834f ce81 1d3e  ...$...|...O...>
+00000e10: 8bd0 dbce b533 a516 2efd 055f 8c50 c8f8  .....3....._.P..
+00000e20: 3427 c4b8 156b 7882 0e5f 7f1a a2f1 7f7a  4'...kx.._.....z
+00000e30: 699c a22c 3de9 5ece 8f35 4cbd cf3f eba0  i..,=.^..5L..?..
+00000e40: 8686 ad3a fb45 6d3e 8298 b716 85b3 1059  ...:.Em>.......Y
+00000e50: de28 65bd 7b06 c3d1 b928 1da6 9ecb 5587  .(e.{....(....U.
+00000e60: 101c 0329 dc2f 88ce 635b 1f37 a2b6 6d45  ...)./..c[.7..mE
+00000e70: 9222 4cf2 6298 c609 62f8 ca58 257f ec57  ."L.b...b..X%..W
+00000e80: 6257 d729 1377 cc67 623c 64a6 6918 8d8a  bW.).w.gb<d.i...
+00000e90: 5196 3eb8 66ec ce19 19f9 3718 b851 9e91  Q.>.f.....7..Q..
+00000ea0: 9d19 c505 e346 262a f84c 8cc7 bab3 f021  .....F&*.L.....!
+00000eb0: c987 b92b fb20 8ea5 dd40 e407 04c6 7303  ...+. ...@....s.
+00000ec0: ff22 fe5b 3ff5 1ff1 2f00 0000 ffff 0000  .".[?.../.......
+00000ed0: 00ff ff9c 585b 8ee2 3010 bc0a ca01 06ec  ....X[..0.......
+00000ee0: 3c98 1911 a44d 48ee 8158 a4f9 9961 45d8  <....MH..X...aE.
+00000ef0: d9dd db6f fb41 dcae 3621 f087 9c72 bbaa  ...o.A..6!...r..
+00000f00: dd76 b5d9 0c1f c7e3 65b7 bfec b79b f3e9  .v......e.......
+00000f10: cfe2 5c67 2a5b 0cbf f65f 03fd 7aaf b2c5  ..\g*[..._..z...
+00000f20: 5f55 ec0f ef3f ffed 8ec3 e1f8 75a9 b3d5  _U...?......u...
+00000f30: 4b5e 66db cdc1 607f 1870 9de5 d982 3e0c  K^f...`..p....>.
+00000f40: 34fa bd5d 6d96 dfdb cdf2 e011 8d43 140c  4..]m........C..
+00000f50: a162 442b 63e8 18b1 9388 a28a 219d 8394  .bD+c.......!...
+00000f60: 6c99 3c46 f492 4831 2296 a47d 4c80 7e24  l.<F..H1"..}L.~$
+00000f70: 0104 1ea5 9720 dd04 b2f9 1c11 39d0 6ef9  ..... ......9.n.
+00000f80: f4fc 061f caee fc0d e15b 018b 3526 50cc  .........[..5&P.
+00000f90: 670d 5be1 106f 3c8b 206a c717 28c3 0a51  g.[..o<. j..(..Q
+00000fa0: 0669 b7e7 338e 4a03 0835 2652 9d51 198e  .i..3.J..5&R.Q..
+00000fb0: 29d4 6fc0 99cf 6729 b4f5 d95d e72f a924  ).o...g)...]./.$
+00000fc0: f91e 53a1 7086 1f14 5e93 ece9 62e7 d505  ..S.p...^...b...
+00000fd0: 2c1a 13b0 ce5e 79e6 e024 b40e c293 5b42  ,....^y..$....[B
+00000fe0: 94ce 41d4 2a43 be94 81f9 19e5 e952 a1a8  ..A.*C.......R..
+00000ff0: 6c46 1a13 2926 5ac0 4969 1d64 b20a 24a4  lF..)&Z.Ii.d..$.
+00001000: 8463 dd39 4842 cbfa 99dc d3a4 b104 141e  .c.9HB..........
+00001010: 3413 1192 0f57 48eb 2093 9a24 a484 289d  4....WH. ..$..(.
+00001020: 8324 34d1 c6cf df1f 5e25 0a0f a989 045a  .$4.....^%.....Z
+00001030: f094 3a08 d752 e029 9590 1276 b973 9084  ..:..R.)...v.s..
+00001040: 160a 3c5f 0b67 a1f0 ee37 91e2 d39b e3e5  ..<_.g...7......
+00001050: ef20 935a 1210 c848 e720 092d 34f4 889b  . .Z...H. .-4...
+00001060: 113a 5419 506d 6cac 584e 8167 dc63 26eb  .:T.Pml.XN.g.c&.
+00001070: 2c81 295e d1ce 0c6f baab e54d a01e f367  ,.)^...o...M...g
+00001080: 4207 4550 ce8d 8d05 8a84 3b3b df9c 5624  B.EP......;;..V$
+00001090: 3105 5e6d 7ead 94a2 870c 5771 cb54 50d4  1.^m~.....Wq.TP.
+000010a0: 8df9 0a25 57e0 55e0 31d3 8a5c 9ce8 b286  ...%W.U.1..\....
+000010b0: bdee 7c9c 9422 b06c 632f 45fe 42b7 fb9d  ..|..".lc/E.B...
+000010c0: 6e2a 3257 f442 25fd 5bc3 b96f 0d26 741b  n*2W.B%.[..o.&t.
+000010d0: a205 9211 aaa0 2a32 4805 1e3e 5b02 b7e3  ......*2H..>[...
+000010e0: 12ca bab1 51e3 1644 634b 6430 4102 d857  ....Q..DcKd0A..W
+000010f0: 9f88 7053 0298 fc9d dc73 77d7 22f7 de99  ..pS.....sw."...
+00001100: 1935 d0d6 aaa8 f9bc d1cb 2930 72aa 55aa  .5........)0r.U.
+00001110: b1c3 efe1 72fa ec4f e7cf 3d29 a7c3 7487  ....r..O..=)..t.
+00001120: aa74 df4a 5c56 579f a74e c21a 7f6b 97b6  .t.J\VW..N...k..
+00001130: cbdd cc6e e731 aea4 edb4 de0f bd8a 9644  ...n.1.........D
+00001140: 818f 3f27 459a 6e85 1d8b 5dc8 5862 9092  ..?'E.n...].Xb..
+00001150: 7073 98d5 f959 9194 6b9f 80dd 9502 fb7e  ps...Y..k......~
+00001160: 4e8a f45c 2d2e 5c87 89fa 5951 4732 8e68  N..\-.\...YQG2.h
+00001170: 6b2d e13a 5b8f 29e9 fd48 629b c0ce 9fd3  k-.:[.)..Hb.....
+00001180: 263d b812 daae 6e7f dda6 4eb9 11ce d28d  &=....n...N.....
+00001190: 4896 1a7c fa29 9636 485c e115 1a84 c754  H..|.).6H\.....T
+000011a0: 63e6 3a3f c258 fa91 044b f0de e758 4ab3  c.:?.X...K...XJ.
+000011b0: acc4 cbd1 6178 9d54 f8e2 d50e c379 bb91  ....ax.T.....y..
+000011c0: 046f 7058 7399 9754 66d3 d78c e64e ab45  .opXs..Tf....N.E
+000011d0: 2213 af5b 2ce5 2882 828e a037 5fe1 3daa  "..[,.(....7_.=.
+000011e0: 6fb8 914e 18ea fdf7 9a99 15de 8d78 add8  o..N.........x..
+000011f0: 98f0 3cc7 b765 1401 05ec a2af 253a 5522  ..<..e......%:U"
+00001200: be0e b774 fc8f 43c2 6c67 c88b 5ece 68b5  ...t..C.lg..^.h.
+00001210: da3d 7d79 ff57 00c5 d660 4277 08e2 77d1  .=}y.W...`Bw..w.
+00001220: d732 94a8 a3be 0cff 1cfd 0700 00ff ff00  .2..............
+00001230: 0000 ffff 348d c10a c230 1044 7f25 ec07  ....4....0.D.%..
+00001240: 5845 4490 a677 0f9e fc82 956c 9345 cd86  XED..w.....l.E..
+00001250: ed88 bf6f 2be4 366f 78cc 8c8d b3dc d8b3  ...o+.6ox.......
+00001260: d625 bc64 46a4 fdee 4cc1 3597 9e61 eddf  .%.dF...L.5..a..
+00001270: 9e28 3c0c b077 a722 9cc4 373a 5298 cdd0  .(<..w."..7:R...
+00001280: 6198 c66d f72e f8b4 60ae 52c1 50ab 919a  a..m....`.R.P...
+00001290: 399c 15eb c345 5324 bfa6 03ad faf0 357f  9....ES$......5.
+000012a0: 2e45 04d3 0f00 00ff ff03 0050 4b03 0414  .E.........PK...
+000012b0: 0006 0008 0000 0021 00c1 1710 be4e 0700  .......!.....N..
+000012c0: 00c6 2000 0013 0000 0078 6c2f 7468 656d  .. ......xl/them
+000012d0: 652f 7468 656d 6531 2e78 6d6c ec59 cd8b  e/theme1.xml.Y..
+000012e0: 1b37 14bf 17fa 3f0c 7377 fc35 e38f 25de  .7....?.sw.5..%.
+000012f0: e0cf 6c93 dd24 649d 941c b5b6 ec51 5633  ..l..$d......QV3
+00001300: 3292 bc1b 1302 2539 f552 28a4 a597 426f  2.....%9.R(...Bo
+00001310: 3d94 d240 030d bdf4 8f09 24b4 e91f d127  =..@......$....'
+00001320: cdd8 23ad e524 9b6c 4a5a 760d 8b47 febd  ..#..$.lJZv..G..
+00001330: a7a7 f79e 7e7a f374 f1d2 bd98 7a47 980b  ....~z.t....zG..
+00001340: c292 965f be50 f23d 9c8c d898 24d3 967f  ..._.P.=....$...
+00001350: 6b38 2834 7c4f 4894 8c11 6509 6ef9 0b2c  k8(4|OH...e.n..,
+00001360: fc4b db9f 7e72 116d c908 c7d8 03f9 446c  .K..~r.m......Dl
+00001370: a196 1f49 39db 2a16 c508 8691 b8c0 6638  ...I9.*.......f8
+00001380: 81df 268c c748 c223 9f16 c71c 1d83 de98  ..&..H.#........
+00001390: 162b a552 ad18 2392 f85e 8262 507b 7d32  .+.R..#..^.bP{}2
+000013a0: 2123 ec0d 954a 7f7b a9bc 4fe1 3191 420d  !#...J.{..O.1.B.
+000013b0: 8c28 df57 aab1 25a1 b1e3 c3b2 4288 85e8  .(.W..%.....B...
+000013c0: 52ee 1d21 daf2 619e 313b 1ee2 7bd2 f728  R..!..a.1;..{..(
+000013d0: 1212 7e68 f925 fde7 17b7 2f16 d156 2644  ..~h.%..../..V&D
+000013e0: e506 5943 6ea0 ff32 b94c 607c 58d1 73f2  ..YCn..2.L`|X.s.
+000013f0: e9c1 6ad2 2008 835a 7ba5 5f03 a85c c7f5  ..j. ..Z{._..\..
+00001400: ebfd 5abf b6d2 a701 6834 8295 a6b6 d83a  ..Z.....h4.....:
+00001410: eb95 6e90 610d 50fa d5a1 bb57 ef55 cb16  ..n.a.P....W.U..
+00001420: ded0 5f5d b3b9 1daa 8f85 d7a0 547f b086  .._]........T...
+00001430: 1f0c bae0 450b af41 293e 5cc3 879d 66a7  ....E..A)>\...f.
+00001440: 67eb d7a0 145f 5bc3 d74b ed5e 50b7 f46b  g...._[..K.^P..k
+00001450: 5044 4972 b886 2e85 b56a 77b9 da15 64c2  PDIr.....jw...d.
+00001460: e88e 13de 0c83 41bd 9229 cf51 900d abec  ......A..).Q....
+00001470: 5253 4c58 2237 e55a 8cee 323e 0080 0252  RSLX"7.Z..2>...R
+00001480: 2449 e2c9 c50c 4fd0 08b2 b88b 2839 e0c4  $I....O.....(9..
+00001490: db25 d308 126f 8612 2660 b854 290d 4a55  .%...o..&`.T).JU
+000014a0: f8af 3e81 fea6 238a b630 32a4 955d 6089  ..>...#..02..]`.
+000014b0: 581b 52f6 7862 c4c9 4cb6 fc2b a0d5 3720  X.R.xb..L..+..7 
+000014c0: 2f9e 3d7b fef0 e9f3 87bf 3d7f f4e8 f9c3  /.={......=.....
+000014d0: 5fb2 b9b5 2a4b 6e07 2553 53ee d58f 5fff  _...*Kn.%SS..._.
+000014e0: fdfd 17de 5fbf fef0 eaf1 37e9 d427 f1c2  ...._.....7..'..
+000014f0: c4bf fcf9 cb97 bfff f13a f5b0 e2dc 152f  .........:...../
+00001500: be7d f2f2 e993 17df 7df5 e74f 8f1d dadb  .}......}..O....
+00001510: 1c1d 98f0 2189 b1f0 aee1 63ef 268b 6181  ....!.....c.&.a.
+00001520: 0efb f101 3f9d c430 42c4 9240 11e8 76a8  ....?..0B..@..v.
+00001530: eecb c802 5e5b 20ea c275 b0ed c2db 1c58  ....^[ ..u.....X
+00001540: c605 bc3c bf6b d9ba 1ff1 b924 8e99 af46  ...<.k.....$...F
+00001550: b105 dc63 8c76 1877 3ae0 aa9a cbf0 f070  ...c.v.w:......p
+00001560: 9e4c dd93 f3b9 89bb 89d0 916b ee2e 4aac  .L.........k..J.
+00001570: 00f7 e733 a057 e252 d98d b065 e60d 8a12  ...3.W.R...e....
+00001580: 89a6 38c1 d253 bfb1 438c 1dab bb43 88e5  ..8..S..C....C..
+00001590: d73d 32e2 4cb0 89f4 ee10 af83 88d3 2543  .=2.L.........%C
+000015a0: 7260 2552 2eb4 4362 88cb c265 2084 daf2  r`%R..Cb...e ...
+000015b0: cdde 6daf c3a8 6bd5 3d7c 6423 615b 20ea  ..m...k.=|d#a[ .
+000015c0: 307e 88a9 e5c6 cb68 2e51 ec52 3944 3135  0~.....h.Q.R9D15
+000015d0: 1dbe 8b64 e432 727f c147 26ae 2f24 447a  ...d.2r..G&./$Dz
+000015e0: 8a29 f3fa 632c 844b e63a 87f5 1a41 bf0a  .)..c,.K.:...A..
+000015f0: 0ce3 0efb 1e5d c436 924b 72e8 d2b9 8b18  .....].6.Kr.....
+00001600: 3391 3d76 d88d 503c 73da 4c92 c8c4 7e26  3.=v..P<s.L...~&
+00001610: 0e21 4591 7783 4917 7c8f d93b 443d 431c  .!E.w.I.|..;D=C.
+00001620: 50b2 31dc b709 b6c2 fd66 22b8 05e4 6a9a  P.1......f"...j.
+00001630: 9427 88fa 65ce 1db1 bc8c 99bd 1f17 7482  .'..e.........t.
+00001640: b08b 65da 3cb6 d8b5 cd89 333b 3af3 a995  ..e.<.....3;:...
+00001650: dabb 1853 748c c618 7bb7 3e73 58d0 6133  ...St...{.>sX.a3
+00001660: cbe7 b9d1 5722 6095 1dec 4aac 2bc8 ce55  ....W"`...J.+..U
+00001670: f59c 6001 6592 aa6b d629 7297 082b 65f7  ..`.e..k.)r..+e.
+00001680: f194 6db0 676f 7182 7816 2889 11df a4f9  ..m.goq.x.(.....
+00001690: 1a44 dd4a 5d38 e59c 547a 9d8e 0e4d e035  .D.J]8..Tz...M.5
+000016a0: 02e5 1fe4 8bd3 29d7 05e8 3092 bbbf 49eb  ......)...0...I.
+000016b0: 8d08 5967 977a 16ee 7c5d 702b 7e6f b3c7  ..Yg.z..|]p+~o..
+000016c0: 605f de3d edbe 0419 7c6a 1920 f6b7 f6cd  `_.=....|j. ....
+000016d0: 1051 6b82 3c61 8608 0a0c 17dd 8288 15fe  .Qk.<a..........
+000016e0: 5c44 9dab 5a6c ee94 9bd8 9b36 0f03 1446  \D..Zl.....6...F
+000016f0: 56bd 1393 e48d c5cf 89b2 27fc 77ca 1e77  V.........'.w..w
+00001700: 0173 0605 8f5b f1fb 943a 9b28 65e7 4481  .s...[...:.(e.D.
+00001710: b309 f71f 2c6b 7a68 9edc c070 92ac 73d6  ....,kzh...p..s.
+00001720: 7955 735e d5f8 fffb aa66 d35e 3eaf 65ce  yUs^.....f.^>.e.
+00001730: 6b99 f35a c6f5 f6f5 416a 99bc 7c81 ca26  k..Z....Aj..|..&
+00001740: eff2 e89e 4fbc b1e5 3321 94ee cb05 c5bb  ....O...3!......
+00001750: 4277 7d04 bcd1 8c07 30a8 db51 ba27 b96a  Bw}.....0..Q.'.j
+00001760: 01ce 22f8 9a35 982c dc94 232d e371 263f  .."..5.,..#-.q&?
+00001770: 2732 da8f d00c 5a43 65dd c09c 8a4c f554  '2....ZCe....L.T
+00001780: 7833 26a0 63a4 8775 2b15 9fd0 adfb 4ef3  x3&.c..u+.....N.
+00001790: 788f 8dd3 4e67 b9ac ba9a a90b 0592 f978  x...Ng.........x
+000017a0: 295c 8d43 974a a6e8 5a3d efde add4 eb7e  )\.C.J..Z=.....~
+000017b0: e854 7759 9706 28d9 d318 614c 661b 5175  .TwY..(...aLf.Qu
+000017c0: 1851 5f0e 4214 5e67 845e d999 58d1 7458  .Q_.B.^g.^..X.tX
+000017d0: d150 ea97 a15a 4671 e50a 306d 1515 78e5  .P...ZFq..0m..x.
+000017e0: f6e0 45bd e587 41da 4186 661c 94e7 6315  ..E...A.A.f...c.
+000017f0: a7b4 99bc 8cae 0ace 9946 7a93 33a9 9901  .........Fz.3...
+00001800: 5062 2f33 208f 7453 d9ba 7179 6a75 69aa  Pb/3 .tS..qyjui.
+00001810: bd45 a42d 238c 74b3 8d30 d230 8217 e12c  .E.-#.t..0.0...,
+00001820: 3bcd 96fb 59c6 ba99 87d4 324f b962 b91b  ;...Y.....2O.b..
+00001830: 7233 ea8d 0f11 6b45 2227 b881 2626 53d0  r3....kE"'..&&S.
+00001840: c43b 6ef9 b56a 08b7 2a23 346b f913 e818  .;n..j..*#4k....
+00001850: c3d7 7806 b923 d45b 17a2 53b8 7619 499e  ..x..#.[..S.v.I.
+00001860: 6ef8 7761 9619 17b2 8744 943a 5c93 4eca  n.wa.....D.:\.N.
+00001870: 0631 9198 7b94 c42d 5f2d 7f95 0d34 d11c  .1..{..-_-...4..
+00001880: a26d 2b57 8010 3e5a e39a 402b 1f9b 7110  .m+W..>Z..@+..q.
+00001890: 743b c878 32c1 2369 86dd 1851 9e4e 1f81  t;.x2.#i...Q.N..
+000018a0: e153 ae70 feaa c5df 1dac 24d9 1cc2 bd1f  .S.p......$.....
+000018b0: 8d8f bd03 3ae7 3711 a458 582f 2b07 8e89  ....:.7..XX/+...
+000018c0: 808b 8372 eacd 3181 9bb0 1591 e5f9 77e2  ...r..1.......w.
+000018d0: 60ca 68d7 bc8a d239 948e 233a 8b50 76a2  `.h....9..#:.Pv.
+000018e0: 9864 9ec2 3589 aecc d14f 2b1f 184f d99a  .d..5....O+..O..
+000018f0: c1a1 eb2e 3c98 aa03 f6bd 4fdd 371f d5ca  ....<.....O.7...
+00001900: 7306 69e6 67a6 c52a ead4 7493 e987 3be4  s.i.g..*..t...;.
+00001910: 0dab f243 d4b2 2aa5 6efd 4e2d 72ae 6b2e  ...C..*.n.N-r.k.
+00001920: b90e 12d5 794a bce1 d47d 8b03 c130 2d9f  ....yJ...}...0-.
+00001930: cc32 4d59 bc4e c38a b3b3 51db b433 2c08  .2MY.N....Q..3,.
+00001940: 0c4f d436 f86d 7546 383d f1ae 273f c89d  .O.6.muF8=..'?..
+00001950: cc5a 7540 2ceb 4a9d f8fa cadc bcd5 6607  .Zu@,.J.......f.
+00001960: 7781 3c7a 707f 38a7 52e8 5042 6f97 2328  w.<zp.8.R.PBo.#(
+00001970: fad2 1bc8 9436 608b dc93 598d 08df bc39  .....6`...Y....9
+00001980: 272d ff7e 296c 07dd 4ad8 2d94 1a61 bf10  '-.~)l..J.-..a..
+00001990: 5483 52a1 11b6 ab85 7618 56cb fdb0 5cea  T.R.....v.V...\.
+000019a0: 752a 0fe0 6091 515c 0ed3 ebfa 015c 61d0  u*..`.Q\.....\a.
+000019b0: 4576 69af c7d7 2eee e3e5 2dcd 8511 8b8b  Evi.......-.....
+000019c0: 4c5f cc17 b5e1 fae2 be5c d97c 71ef 1120  L_.......\.|q.. 
+000019d0: 9dfb b5ca a059 6d76 6a85 66b5 3d28 04bd  .....Ymvj.f.=(..
+000019e0: 4ea3 d0ec d63a 855e ad5b ef0d 7add b0d1  N....:.^.[..z...
+000019f0: 1c3c f0bd 230d 0eda d56e 50eb 370a b572  .<..#....nP.7..r
+00001a00: b75b 086a 2565 7ea3 59a8 0795 4a3b a8b7  .[.j%e~.Y...J;..
+00001a10: 1bfd a0fd 202b 6360 e529 7d64 be00 f76a  .... +c`.)}d...j
+00001a20: bbb6 ff01 0000 ffff 0300 504b 0304 1400  ..........PK....
+00001a30: 0600 0800 0000 2100 137c 8b5b f108 0000  ......!..|.[....
+00001a40: 7646 0000 0d00 0000 786c 2f73 7479 6c65  vF......xl/style
+00001a50: 732e 786d 6cc4 5c59 6fe3 3610 7e2f d0ff  s.xml.\Yo.6.~/..
+00001a60: 2008 e8a3 a3db b602 db45 ec44 ed02 db6d   ........E.D...m
+00001a70: 814d d1be cab2 eca8 d161 48f2 d669 d1ff  .M.......aH..i..
+00001a80: de19 ea20 e993 4e64 13c1 6e2c c5fc e6fa  ... ..Nd..n,....
+00001a90: 3843 8e8e d18f db24 56be 8579 1165 e958  8C.....$V..y.e.X
+00001aa0: 35ee 7455 09d3 205b 44e9 6aac fefe ecf5  5.tU.. [D.j.....
+00001ab0: 86aa 5294 7eba f0e3 2c0d c7ea 5b58 a83f  ..R.~...,...[X.?
+00001ac0: 4ebe ff6e 5494 6f71 f8f5 250c 4b05 20d2  N..nT.oq..%.K. .
+00001ad0: 62ac be94 e5fa 5ed3 8ae0 254c fce2 2e5b  b.....^...%L...[
+00001ae0: 8729 fc65 99e5 895f c261 bed2 8a75 1efa  .).e..._.a...u..
+00001af0: 8b02 0725 b166 ea7a 5f4b fc28 552b 84fb  ...%.f.z_K.(U+..
+00001b00: 2410 0149 fcfc 75b3 ee05 59b2 f6cb 681e  $..I..u...Y...h.
+00001b10: c551 f946 b054 2509 ee3f add2 2cf7 e731  .Q.F.T%..?..,..1
+00001b20: a8ba 356c 3f50 b646 3f37 956d de08 2167  ..5l?P.F?7.m..!g
+00001b30: f7e4 2451 9067 45b6 2cef 0057 cb96 cb28  ..$Q.gE.,..W...(
+00001b40: 08f7 d575 3557 f303 8a04 c8ef 4332 1c4d  ...u5W......C2.M
+00001b50: 3739 dbb7 f93b 916c 2d0f bf45 183e 7532  79...;.l-..E.>u2
+00001b60: 5a66 6959 2841 b649 4b08 a60b 9aa2 0fee  ZfiY(A.IK.......
+00001b70: 5fd3 ecef d4c3 bfc1 d9fa 6b93 51f1 8ff2  _.........k.Q...
+00001b80: cd8f e18c a16a 9351 90c5 59ae 9410 3b70  .....j.Q..Y...;p
+00001b90: 1d39 93fa 4958 7d63 e6c7 d13c 8ff0 6b4b  .9..IX}c...<..kK
+00001ba0: 3f89 e2b7 eab4 8927 48b8 ebef 2511 381f  ?......'H...%.8.
+00001bb0: 4f6a a848 a58e 0439 c33d 7b2c 3cb3 678f  Oj.H...9.={,<.g.
+00001bc0: f239 5abd 94e7 adf2 ff3a 60d5 1c6d 6f3c  .9Z......:`..mo<
+00001bd0: e808 4a7c a707 3959 c416 2e5a 87ad eb42  ..J|..9Y...Z...B
+00001be0: d63e 333a 9575 8881 f96a 3e56 3d0f 7283  .>3:.u...j>V=.r.
+00001bf0: a1eb 07c3 d621 0d6b 61ee 4c07 7937 13e6  .....!.ka.L.y7..
+00001c00: 0c6e 6699 e559 dea0 53cb 382e 32fc a85d  .nf..Y..S.8.2..]
+00001c10: 8902 2daf 4b57 9e11 e83d 0c1e 6fe6 ceee  ..-.KW...=..o...
+00001c20: 851d b3ae 4ec4 b79a 0138 e1ba f562 c4e6  ....N....8...b..
+00001c30: c77d 9e0c 3cfc b905 4f6e 5cd2 ae18 b18f  .}..<...On\.....
+00001c40: 1764 5297 0b28 cc51 1cb7 eb04 cbc6 2501  .dR..(.Q......%.
+00001c50: 9c99 8c60 4555 8679 eac1 8152 7f7e 7e5b  ...`EU.y...R.~~[
+00001c60: c382 2085 c51f 064b abbe 77e6 dbab dc7f  .. ....K..w.....
+00001c70: 334c 5214 c506 1459 1c2d 508b d58c 2c43  3LR....Y.-P...,C
+00001c80: ea64 32eb 3f79 b327 2297 d14c 548b 23a0  .d2.?y.'"..LT.#.
+00001c90: 9e37 1b5c 01f4 69ea ceba d774 e6ba 5d83  .7.\..i....t..].
+00001ca0: 9a1e fc74 0cfa e0e0 4fe7 e643 a83a f369  ...t....O..C.:.i
+00001cb0: 9d06 ecae 946c f194 32c2 d5b6 7e37 705d  .....l..2...~7p]
+00001cc0: 7768 f487 c3a1 6b5b 866d 1327 cf6b 4647  wh....k[.m.'.kFG
+00001cd0: e922 dc86 8bb1 daef cc4d fb1a 38a0 816b  .".......M..8..k
+00001ce0: 0ddd be09 8ae8 f690 88ba a906 1628 3070  .............(0p
+00001cf0: 9ca1 63b8 a60d ff48 e2bf be06 5dfb d451  ..c....H....]..Q
+00001d00: 6547 95d1 4052 5419 0d24 4595 ac5b b50e  eG..@RT..$E..[..
+00001d10: 327f 3d53 fad2 a3ca 6820 29aa 8c06 92a2  2.=S....h ).....
+00001d20: 3ae8 3803 0fa4 4795 d140 5254 190d 2445  :.8...G..@RT..$E
+00001d30: 95f4 5c3a 9cab d076 945c 5719 0d24 4595  ..\:...v.\W..$E.
+00001d40: d140 5254 3b5b 7cd6 1918 3a92 92a3 ca68  .@RT;[|...:....h
+00001d50: 2029 aa8c 0692 a20a 3dfe 2a0a 3dfd ceb0   )......=.*.=...
+00001d60: 71d5 6a0f 6c7d 603b 66ff d882 edf8 b299  q.j.l}`;f.......
+00001d70: 6cf0 604b 39cf f205 5c46 689b cf3a 6ce7  l.`K9...\Fh..:l.
+00001d80: aa73 9351 1c2e 4bd8 3ce6 d86e 85df 65b6  .s.Q..K.<..n..e.
+00001d90: 86ff e759 5942 af7d 325a 44fe 2a4b fd18  ...YYB.}2ZD.*K..
+00001da0: b797 cd08 8191 7059 02ae 408c d5f2 250a  ......pY..@...%.
+00001db0: 5e41 18d7 12ad f4ad 445c 4b42 4be5 1d17  ^A......D\KBK...
+00001dc0: 92fa d691 e824 5c44 9b64 dfba 56f6 410a  .....$\D.d..V.A.
+00001dd0: 811b d1b7 e70d 677c 8897 0f2a 17d6 9b6f  ......g|...*...o
+00001de0: daa1 d130 7e75 f804 4790 5093 480b 0e00  ...0~u..G.P.H...
+00001df0: 4e34 9410 1cd1 858d b45b 296a 2333 42cc  N4.......[)j#3B.
+00001e00: 4666 80a0 8dcc 888e 58b4 c836 7045 6c37  Ff......X..6pEl7
+00001e10: c09e 37d4 75b2 41bb 982f 8701 4f7b f3ec  ..7.u.A../..O{..
+00001e20: 987d 7f9e 1d72 c0a3 67c7 74c1 9ba9 893f  .}...r..g.t....?
+00001e30: 64a2 0bce 0d66 8418 6f98 0182 bc61 46bc  d....f..o....aF.
+00001e40: 8f37 0727 1ed7 3739 ef6f eeeb a7d4 a853  .7.'..79.o.....S
+00001e50: 3d54 8e20 8ce3 af98 cbff 5cb6 e503 9a27  =T. ......\....'
+00001e60: 93d1 76a9 a49b c44b ca4f d037 81a2 8517  ..v....K.O.7....
+00001e70: 159b 8fd0 a1ac 3f56 a5a2 3a80 1272 6c90  ......?V..:..rl.
+00001e80: 09e3 0f0f 52fc f53a 7efb b249 e661 ee91  ....R..:~..I.a..
+00001e90: abd5 441a 398b 9d50 7a34 2535 8e1e 3fc4  ..D.9..Pz4%5..?.
+00001ea0: d12a 4d42 d2fe 512b 98df f2ac 0c83 925c  .*MB..Q+.......\
+00001eb0: 4d27 ade0 63fa 5847 f431 6a20 117d 3e22  M'..c.XG.1j .}>"
+00001ec0: df3e 221f fc24 ec8f 8fc8 87f6 c2c1 7880  .>"..$........x.
+00001ed0: 5fa4 ca07 9e49 e103 6ccc 1b7f 4008 5852  _....I..l...@.XR
+00001ee0: 9fd2 a74b 46c2 26b2 d100 8220 4303 d8f0  ...KF.&.... C...
+00001ef0: 341a 003d 6568 008b f346 0320 28d5 00d4  4..=eh...F. (...
+00001f00: 39c1 8a8f cc03 0313 5b9d 9880 0354 24c8  9.......[....T$.
+00001f10: bf96 48c8 3107 455e d1ca 63e9 174c bec9  ..H.1.E^..c..L..
+00001f20: 7437 987c 0b44 a76e 8683 6bb9 f958 8a95  t7.|.D.n..k..X..
+00001f30: 9562 98b0 c34c a32e 8083 5331 80aa db4d  .b...L....S1...M
+00001f40: c933 8ee5 7c69 0e61 922e e840 3d02 69e0  .3..|i.a...@=.i.
+00001f50: 36ac 6472 2ec8 9491 f118 5260 2a92 ad02  6.dr......R`*...
+00001f60: a823 5b05 49e5 d760 b880 d94a b61b 2455  .#[.I..`...J..$U
+00001f70: 6096 8f5c 093e 9d24 ba5c 08b1 2a70 25f9  `..\.>.$.\..*p%.
+00001f80: 862a b064 e0ea 951c 3770 f542 8e0a f2f3  .*.d....7p.B....
+00001f90: a329 2b3f 3264 8006 adec cc60 ca4a 90cc  .)+?2d.....`.J..
+00001fa0: 0e49 7e7e 3465 e547 960c f213 a429 2b41  .I~~4e.G.....)+A
+00001fb0: 3264 909f 1f4d 59f9 9125 83fc 0469 c95f  2d...MY..%...i._
+00001fc0: 405a f2f3 a375 e5fc a8b1 0dd3 aa7d ca74  @Z...u.......}.t
+00001fd0: 4ee1 698e f774 4e95 edf2 6c0b 95e9 54ec  N.i..tN...l...T.
+00001fe0: 06ba 195d 6d9b 987e 086a 034f 8f54 6d52  ...]m..~.j.O.TmR
+00001ff0: e5ef dc5f 3f87 5b7c 3885 34cf b7cb 1d5d  ..._?.[|8.4....]
+00002000: 6d6c c09c 6df3 b6ca 1eda a511 e463 5d57  ml..m........c]W
+00002010: 83d9 f159 bb45 8437 029f 9741 3d2b 1955  ...Y.E.7...A=+.U
+00002020: 23f8 bad8 5d3a ef02 43f9 4e73 6bf0 c5e6  #...]:..C.Nsk...
+00002030: 33dd bbd3 f438 ecd9 4ead 17d6 a523 e385  3....8..N....#..
+00002040: a746 c3a3 8f5a 8b02 2f9d 27c7 38dc c9a4  .F...Z../.'.8...
+00002050: db9b 2624 4d41 6262 2ef0 f097 77da 34a6  ..&$MAbb....w.4.
+00002060: e08d ed63 d5d4 7f50 7aca 4310 c005 1560  ...c...Pz.C....`
+00002070: 6135 1bf1 21b6 f926 8ae1 8605 cc4f 5861  a5..!..&.....OXa
+00002080: 824d 0117 b7a7 d5c9 3a93 9cc2 8274 5c61  .M......:....t\a
+00002090: 9938 e119 2c58 c15d 8a05 0835 162e 3a18  .8..,X.]...5..:.
+000020a0: 2c20 dca5 5820 bec2 2235 8b62 c1b5 af8b  , ..X .."5.b....
+000020b0: b160 2158 63e1 9290 c182 7c77 a95e 30a4  .`!Xc.....|w.^0.
+000020c0: c6e2 7def 08fa de3e 1447 b277 62fc 0501  ..}....>.G.wb...
+000020d0: 16d1 8bc5 a271 c4a5 3783 0526 5f8a 45e3  .....q..7..&_.E.
+000020e0: 882b 3706 0b4c be14 8bc6 110b 3fe3 7b10  .+7..L......?.{.
+000020f0: 7229 168d 23ae ab19 2ca0 dba5 586d 1c6d  r)..#...,...Xm.m
+00002100: 4cc7 14cb 11f4 7dff 601c 717d c5f8 4b90  L.....}.`.q}..K.
+00002110: ab2c 168d 23cf 554b 90ab 2c16 8d23 cf55  .,..#.UK..,..#.U
+00002120: 3459 c45f 2c16 8d23 9f27 6cc1 3cc1 62d1  4Y._,..#.'l.<.b.
+00002130: 38f2 79c2 16cc 132c 168d 23ef 7b47 d0f7  8.y....,..#.{G..
+00002140: bb19 9567 bc29 c8f8 0a85 c68e e73a aea5  ...g.).......:..
+00002150: 44fc 5da1 d0a8 f12c b704 595e a1d0 78f1  D.]....,..Y^..x.
+00002160: fcb6 05f9 5da1 d048 f159 c516 cc2a 150a  ....]..H.Y...*..
+00002170: cd99 bc77 b1b4 8af8 65ea 2f9a accb 13c6  ...w....e./.....
+00002180: 1474 093c a21d 6c62 7820 1e9e 036f 4a27  .t.<..lbx ...oJ'
+00002190: 4f17 6cdb 88a8 327b 0983 5765 0637 65b4  O.l...2{..We.7e.
+000021a0: 40fc 7cc0 322a 02f4 b45d c77e ea97 59fe  @.|.2*...].~..Y.
+000021b0: a6e0 a2bf 85e3 83ee 08c2 fd94 65ad 8f78  ............e..x
+000021c0: 04ec 4188 28f4 33bc 7c00 de6b a0b4 8b0b  ..A.(.3.|..k....
+000021d0: 9ec3 b864 be04 a69d 0bbc 7bb0 8f7f 094c  ...d......{....L
+000021e0: 3b19 78fe 1982 99a2 31aa 9d0d 7c52 c5f5  ;.x.....1...|R..
+000021f0: 9388 369f d2f5 a68d 109f 4bb1 748b 407c  ..6.......K.t.@|
+00002200: 8ed2 d770 c133 87f7 30f6 cc44 90be 849b  ...p.3..0..D....
+00002210: 32f7 5bfe ed24 2c41 c77c c15b 795a 0c3e  2.[..$,A.|.[yZ.>
+00002220: 4590 3b73 76d7 8c5f e0ce 9d96 a33b 5e14  E.;sv.._.....;^.
+00002230: 74c1 af9b 9271 23b9 9e46 6b25 b66e 45ac  t....q#..Fk%.nE.
+00002240: 7f8e 4ab8 59af 99c4 5cb9 c52b a842 1059  ..J.Y...\..+.B.Y
+00002250: 494d 4742 3225 1b9e cb14 c2f8 c3cf 539c  IMGB2%........S.
+00002260: 2ddc d4dd e1e8 118b 6887 0256 ff8b 2dbd  -.......h..V..-.
+00002270: ad8b f8bd c4d7 7390 1bbe dafd 00b8 7711  ......s.......w.
+00002280: 2efd 4d5c 3eb7 7f1c abf4 f32f e436 5820  ..M\>....../.6X 
+00002290: 53fd addf a26f 5949 20c6 2afd 4c5e e700  S....oYI .*.L^..
+000022a0: b318 ee02 8374 f3b9 807b 56e1 b7b2 c9a3  .....t...{V.....
+000022b0: b1fa efd3 74e0 3e3e 7966 6fa8 4f87 3ddb  ....t.>>yfo.O.=.
+000022c0: 0a9d 9eeb 4c1f 7b8e 3d9b 3e3e 7aae 6eea  ....L.{.=.>>z.n.
+000022d0: b3ff 9897 847c e015 21e4 9d26 d0d8 30ec  .....|..!..&..0.
+000022e0: fb22 8617 89e4 b5b1 b5f2 5fe9 b9b1 ca1c  ."........_.....
+000022f0: 54ea 93be 08a8 cdea ee9a 7dfd c131 f49e  T.........}..1..
+00002300: 67e9 46cf eefb c3de b06f 393d cf31 ccc7  g.F......o9=.1..
+00002310: be3d 7d72 3c87 d1dd 79e7 ab44 74cd 30aa  .=}r<...y..Dt.0.
+00002320: 9792 a0f2 ce7d 1925 611c a54d ac9a 08b1  .....}.%a..M....
+00002330: 6721 4870 78c2 08ad 8984 465f 1833 f91f  g!Hpx.....F_.3..
+00002340: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
+00002350: 0000 2100 9e63 0ab8 a203 0000 960a 0000  ..!..c..........
+00002360: 1400 0000 786c 2f73 6861 7265 6453 7472  ....xl/sharedStr
+00002370: 696e 6773 2e78 6d6c 8c56 4d6f db38 10bd  ings.xml.VMo.8..
+00002380: 2fb0 ff61 a053 0a6c e26c 0f6d 60d8 2eb2  /..a.S.l.l.m`...
+00002390: 318a 14a8 8b20 4e0a ec49 a045 da26 2291  1.... N..I.E.&".
+000023a0: 2c39 52e2 7fdf 1952 bb69 4439 8d2f b639  ,9R....R.iD9./.9
+000023b0: 43ce 07df 7bc3 d9a7 a7a6 864e f9a0 ad99  C...{......N....
+000023c0: 177f 9f9d 17a0 4c65 a536 bb79 717f f7f9  ......Le.6.yq...
+000023d0: f4a2 8080 c248 515b a3e6 c541 85e2 d3e2  .....HQ[...A....
+000023e0: cf3f 6621 20d0 5e13 e6c5 1ed1 4d27 9350  .?f! .^.....M'.P
+000023f0: ed55 23c2 9975 ca90 656b 7d23 90fe fadd  .U#..u..ek}#....
+00002400: 2438 af84 0c7b a5b0 a927 efcf cf3f 4c1a  $8...{...'...?L.
+00002410: a14d 0195 6d0d ce8b 8bf7 05b4 46ff 68d5  .M..m.......F.h.
+00002420: 555a f8f0 b158 cc82 5ecc 70d1 09af c5a6  UZ...X..^.p.....
+00002430: 56a5 118d 9a4d 7031 9bb0 2119 a5da 6aa3  V....Mp1..!...j.
+00002440: 9192 1f5a 826d 7d95 f9ab 27d1 b83a 5b36  ...Z.m}...'..:[6
+00002450: 1655 189e 6014 3e5a ff30 5c76 dea2 ad6c  .U..`.>Z.0\v...l
+00002460: 3d5c bfe9 d7c1 b4cd 46f9 a1f9 3204 7100  =\......F...2.q.
+00002470: 3cb8 2cf8 ae0d 4e55 59fe b436 e6cd bea5  <.,...NUY..6....
+00002480: f3ba 11fe 30b6 a714 5252 43ba 2c4c dc28  ....0...RRC.,L.(
+00002490: 95d7 9d18 333b d472 785e a783 4663 b3a6  ....3;.rx^..Fc..
+000024a0: 7bf1 2871 2cb8 b779 6fb5 712d 965b 7de4  {.(q,..yo.q-.[}.
+000024b0: 062f a554 1236 0758 2f57 57c3 33bf 040b  ./.T.6.X/WW.3...
+000024c0: 52a0 8204 a6a1 f99b 4530 aa52 d45a af6b  R.......E0.R.Z.k
+000024d0: eaee 5e25 77fe 518b 0d54 043b a4e3 7b83  ..^%w.Q..T.;..{.
+000024e0: 3803 3e31 1d76 363c 4d9b 80be 6d94 c94b  8.>1.v6<M...m..K
+000024f0: 930d f7dc 7224 2246 c929 a1ce d118 d88f  ....r$"F.)......
+00002500: 8ca2 f494 9576 78d4 737d 757d 797b 035f  .....vx.s}u}y{._
+00002510: 969c 0cb4 aeb6 8229 c749 6745 12ec c16e  .......).IgE...n
+00002520: 4144 008d 3844 4339 8695 84b9 e375 ddd2  AD..8DC9.....u..
+00002530: 75f1 d10c 0d2a 27e3 d0b7 c480 538a a077  u....*'.....S..w
+00002540: 86fa 9838 0a21 9208 b4a4 5ee9 adce c1be  ...8.!....^.....
+00002550: ee0f 1cc5 fb77 4655 cf12 3871 cac3 7f94  .....wFU..8q....
+00002560: ea17 a911 ef48 19bc 57c1 5913 fb82 b60f  .....H..W.Y.....
+00002570: 3aec 4edf c8af 74d9 f7b1 8b70 6773 6e32  :.N...t....pgsn2
+00002580: b6e0 1f51 3dec 3ce9 8b84 155d 20a9 4a9d  ...Q=.<....] .J.
+00002590: 717e a5fc 8eea dc7a dbc0 d7e5 6a7d 0c98  q~.....z....j}..
+000025a0: 7d67 8035 09c4 66e3 55a7 8956 b90c ad53  }g.5..f.U..V...S
+000025b0: ab48 2f6a e233 39c0 92f1 7cf2 2f7d 4e57  .H/j.39...|./}NW
+000025c0: abd3 e5f2 ddb0 a4e8 408a 0b0c 31a0 1d8f  ........@...1...
+000025d0: 7b5d ed23 3f32 4007 8540 bd49 1eb8 d701  {].#?2@..@.I....
+000025e0: a48e 6148 1dc0 ab2d 09fb afb1 eeae afa7  ..aH...-........
+000025f0: abd5 74bd ce82 5e31 5338 3d0e 4a82 df38  ..t...^1S8=.J..8
+00002600: 0606 f326 f297 6925 de76 d28b bb9f c2cd  ...&..i%.v......
+00002610: b854 0dbc 4805 4645 6be0 b63c 2a5f 37c2  .T..H.FEk..<*_7.
+00002620: a3ae b413 065f c1e5 6752 a174 67ff 132a  ....._..gR.tg..*
+00002630: 1696 08c8 4261 e137 508a 29bc 0522 510c  ....Ba.7P.).."Q.
+00002640: 7ad1 28a5 42a1 73b8 4588 a549 3525 16e8  z.(.B.s.E..I5%..
+00002650: 8614 e82f 2091 eee8 c710 1763 ceaf fad0  .../ ......c....
+00002660: 24f8 dd31 6f09 854f e8f2 d9f0 229b 4ecb  $..1o..O....".N.
+00002670: 4e64 13f1 858b e4a1 d150 71fc 2dfb ef6c  Nd.......Pq.-..l
+00002680: 82dd d233 21b1 8f07 0634 d436 bea0 314d  ...3!....4.6..1M
+00002690: 8c43 a317 fa57 db50 076c 6516 295d 7949  .C...W.P.le.)]yI
+000026a0: 7a5a e6c5 2549 65db d8a3 63dd 6e1a 8d3c  zZ..%Ie...c.n..<
+000026b0: 5768 6c8d 2936 bd26 883a 82a8 d9cf a1f8  Whl.)6.&.:......
+000026c0: e719 6469 4c09 20ba 9a91 1146 f24a a212  ..diL. ....F.J..
+000026d0: 5eee 269d e4b9 d50f b398 e0b0 ea94 7568  ^.&...........uh
+000026e0: 3763 b3e0 790a 9421 6a5f 3ed7 b9de 60b7  7c..y..!j_>...`.
+000026f0: f828 bc2a fb37 e178 8c23 7026 c16e 6b2c  .(.*.7.x.#p&.nk,
+00002700: 694a 60a6 acf7 bc98 ab7a daf2 1c65 42ef  iJ`......z...eB.
+00002710: cac5 4f00 0000 ffff 0300 504b 0304 1400  ..O.......PK....
+00002720: 0600 0800 0000 2100 3b6d 324b c100 0000  ......!.;m2K....
+00002730: 4201 0000 2300 0000 786c 2f77 6f72 6b73  B...#...xl/works
+00002740: 6865 6574 732f 5f72 656c 732f 7368 6565  heets/_rels/shee
+00002750: 7431 2e78 6d6c 2e72 656c 7384 8fc1 8ac2  t1.xml.rels.....
+00002760: 3014 45f7 03fe 4378 7b93 d685 0c43 5337  0.E...Cx{....CS7
+00002770: 22b8 55e7 0362 fada 06db 9790 f714 fd7b  ".U..b.........{
+00002780: b31c 65c0 e5e5 70cf e536 9bfb 3ca9 1b66  ..e...p..6..<..f
+00002790: 0e91 2cd4 ba02 85e4 6317 68b0 f07b da2d  ..,.....c.h..{.-
+000027a0: bf41 b138 eadc 1409 2d3c 9061 d32e be9a  .A.8....-<.a....
+000027b0: 034e 4e4a 89c7 9058 150b b185 5124 fd18  .NNJ...X....Q$..
+000027c0: c37e c4d9 b18e 09a9 903e e6d9 4989 7930  .~.......>..I.y0
+000027d0: c9f9 8b1b d0ac aa6a 6df2 5f07 b42f 4eb5  .......jm._../N.
+000027e0: ef2c e47d 5783 3a3d 5259 feec 8e7d 1f3c  .,.}W.:=RY...}.<
+000027f0: 6ea3 bfce 48f2 cf84 4939 9060 3ea2 4839  n...H...I9.`>.H9
+00002800: c845 edf2 8062 41eb 77f6 9e6b 7d0e 04a6  .E...bA.w..k}...
+00002810: 6dcc cbf3 f609 0000 ffff 0300 504b 0304  m...........PK..
+00002820: 1400 0600 0800 0000 2100 cfe0 47b4 c201  ........!...G...
+00002830: 0000 2c15 0000 2700 0000 786c 2f70 7269  ..,...'...xl/pri
+00002840: 6e74 6572 5365 7474 696e 6773 2f70 7269  nterSettings/pri
+00002850: 6e74 6572 5365 7474 696e 6773 312e 6269  nterSettings1.bi
+00002860: 6eec 54cd 4adc 5018 3d33 b1ed e8a6 0e14  n.T.J.P.=3......
+00002870: dc74 51a4 2b71 e80c 93a9 dd55 99a4 764a  .tQ.+q.....U..vJ
+00002880: d284 2433 b871 3174 5208 8cc9 9044 44a5  ..$3.q1tR....DD.
+00002890: 82f8 1a3e 4897 2e5d f601 ba76 21c5 0770  ...>H..]...v!..p
+000028a0: a3e7 a633 d896 a18c e046 f8ee e5bb dfcf  ...3.....F......
+000028b0: 3d39 37f7 907c 3622 7c41 8a04 19ed 2b72  =97..|6"|A....+r
+000028c0: bc82 cb3c 425c c439 abaa 62e0 03a6 8dd2  ...<B\.9..b.....
+000028d0: 9cf6 f427 dc17 da9b 12d4 bc5c 482a 03fa  ...'.......\H*..
+000028e0: e7d8 2a97 e9b7 ca1a 570b 21d9 72ae e954  ..*.....W.!.r..T
+000028f0: 96fb 154b 63b8 f265 9af2 371c 9b1d 5fff  ...Kc..e..7..._.
+00002900: 93c9 e87c ee2e e31c afb5 d5ea fbed c3a3  ...|............
+00002910: ff9d f2a4 d89c 2fb8 1ee0 1585 e211 2a30  ....../.......*0
+00002920: f9ae 6679 f573 827c 3bf8 a4b0 8bf8 8e43  ..fy.s.|;......C
+00002930: d4f1 0e3a ff92 3a1a 5c37 5083 89b7 68b2  ...:..:.\7P...h.
+00002940: 56a3 1958 e3ac 11d3 64dd 6454 67ae 336f  V..X....d.dTg.3o
+00002950: d0b7 9935 d12a b26f 64f4 4cdf b02c 74e3  ...5.*.od.L..,t.
+00002960: 280d 3315 b9fd 5198 fad1 4108 cb0c 02d3  (.3...Q...A.....
+00002970: 8393 4661 9cf7 f328 89e1 3a5e e06d 7402  ..Fa...(..:^.mt.
+00002980: 7861 960c 778b 1a43 67a4 a206 dac9 3049  xa..w..Cg.....0I
+00002990: ed64 10fe 8efe bedd 6a15 e8e9 863d b9fb  .d......j....=..
+000029a0: e9c2 68f9 2521 bf68 1aed bae4 54f4 8b3d  ..h.%!.h....T..=
+000029b0: fbe4 ead9 c7a5 b3d6 f10f d6ac f11e 2a77  ..............*w
+000029c0: 5c0a abf2 95b1 57f9 3aad a7f2 45f0 fe09  \.....W.:...E...
+000029d0: fbcc 2e76 d803 5467 e9b2 dfa8 6ee0 a2cf  ...v..Tg....n...
+000029e0: 28c3 1ef7 530c 08fe 17e9 702f 9e11 db26  (...S.....p/...&
+000029f0: c73e 46e4 f7f9 843a 4f75 b29c 3519 a280  .>F....:Ou..5...
+00002a00: 2820 0a88 02a2 8028 200a 8802 a280 2820  ( .....( .....( 
+00002a10: 0a88 02a2 8028 200a cca2 c02d 0000 00ff  .....( ....-....
+00002a20: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
+00002a30: 0011 f2fe 2d4d 0100 0071 0200 0011 0008  ....-M...q......
+00002a40: 0164 6f63 5072 6f70 732f 636f 7265 2e78  .docProps/core.x
+00002a50: 6d6c 20a2 0401 28a0 0001 0000 0000 0000  ml ...(.........
 00002a60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002a80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002b00: 0000 0000 0084 9251 4bc3 3014 85df 05ff  .......QK.0.....
-00002b10: 43c9 b35d d2ce 9511 da0e a60c 1f1c 0856  C..]...........V
-00002b20: 14df 4272 b785 3569 49a2 ddfe bd69 bbd5  ..Br..5iI....i..
-00002b30: ca06 3e26 e7dc 2fe7 5c92 2e0e aa0c bec1  ..>&../.\.......
-00002b40: 5859 e90c 4513 8202 d0bc 1252 6f33 f456  XY..E......Ro3.V
-00002b50: acc2 390a ac63 5ab0 b2d2 90a1 2358 b4c8  ..9..cZ.....#X..
-00002b60: 6f6f 525e 535e 1978 3155 0dc6 49b0 8127  ooR^S^.x1U..I..'
-00002b70: 694b 799d a19d 7335 c5d8 f21d 2866 27de  iKy...s5....(f'.
-00002b80: a1bd b8a9 8c62 ce1f cd16 d78c efd9 1670  .....b.........p
-00002b90: 4c48 8215 3826 9863 b805 86f5 4044 27a4  LH..8&.c....@D'.
-00002ba0: e003 b2fe 3265 0710 1c43 090a b4b3 389a  ....2e...C....8.
-00002bb0: 44f8 d7eb c028 7b75 a053 464e 25dd b1f6  D....({u.SFN%...
-00002bc0: 9d4e 71c7 6cc1 7b71 701f ac1c 8c4d d34c  .Nq.l.{qp....M.L
-00002bd0: 9a69 17c3 e78f f0c7 faf9 b5ab 1a4a ddee  .i...........J..
-00002be0: 8a03 ca53 c129 37c0 5c65 f227 2644 c5f7  ...S.)7.\e.'&D..
-00002bf0: 77c1 d29f 8d3c a478 24b6 8b2c 9975 6bbf  w....<.x$..,.uk.
-00002c00: f38d 04b1 3c5e f15f 7a3c bfab d33f 0222  ....<^._z<...?."
-00002c10: f001 695f e7ac bc4f 1f1e 8b15 ca63 12df  ..i_...O.....c..
-00002c20: 8724 0ea3 a420 8446 118d 93cf 36c2 9ff9  .$... .F....6...
-00002c30: 3670 7fa1 4e41 fe25 4e43 9214 714c 6709  6p..NA.%NC..qLg.
-00002c40: 9dcd 47c4 3320 4ff1 c527 c97f 0000 00ff  ..G.3 O..'......
-00002c50: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
-00002c60: 00d0 b93e a68b 0100 000d 0300 0010 0008  ...>............
-00002c70: 0164 6f63 5072 6f70 732f 6170 702e 786d  .docProps/app.xm
-00002c80: 6c20 a204 0128 a000 0100 0000 0000 0000  l ...(..........
-00002c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002ca0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002cb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002cc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002cd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002b50: 0000 0000 0000 0000 0000 8492 5f4b c330  ............_K.0
+00002b60: 14c5 df05 bf43 c9b3 6dfa 678c 11da 0ea6  .....C..m.g.....
+00002b70: 0c1f 1c08 5614 df42 72b7 85b5 4948 a2dd  ....V..Br...IH..
+00002b80: bebd 693b 6b65 031f 9373 ee2f e75c 922f  ..i;ke...s./.\./
+00002b90: 8f4d 1d7c 81b1 42c9 0225 518c 0290 4c71  .M.|..B..%Q...Lq
+00002ba0: 2177 057a add6 e102 05d6 51c9 69ad 2414  !w.z......Q.i.$.
+00002bb0: e804 162d cbdb 9b9c 69c2 9481 67a3 3418  ...-....i...g.4.
+00002bc0: 27c0 069e 242d 61ba 407b e734 c1d8 b23d  '...$-a.@{.4...=
+00002bd0: 34d4 46de 21bd b855 a6a1 ce1f cd0e 6bca  4.F.!..U......k.
+00002be0: 0e74 0738 8de3 396e c051 4e1d c51d 30d4  .t.8..9n.QN...0.
+00002bf0: 2311 9d91 9c8d 48fd 69ea 1ec0 1986 1a1a  #.....H.i.......
+00002c00: 90ce e224 4af0 afd7 8169 ecd5 815e 9938  ...$J....i...^.8
+00002c10: 1be1 4eda 773a c79d b239 1bc4 d17d b462  ..N.w:...9...}.b
+00002c20: 34b6 6d1b b559 1fc3 e74f f0fb e6e9 a5af  4.m..Y...O......
+00002c30: 1a0a d9ed 8a01 2a73 ce08 3340 9d32 e523  ......*s..3@.2.#
+00002c40: e55c b1c3 5db0 f267 238e 399e 88dd 226b  .\..]..g#.9..."k
+00002c50: 6add c6ef 7c2b 80af 4e57 fc97 1ecf efeb  j...|+..NW......
+00002c60: 0c8f 000f 7c40 32d4 f951 deb2 fb87 6a8d  ....|@2..Q....j.
+00002c70: ca34 4e67 619c 86c9 bc8a 6392 2424 9d7f  .4Nga.....c.$$..
+00002c80: 7411 fecc 7781 878b e61c e45f 6216 a669  t...w......_b..i
+00002c90: 952c c86c 41b2 29f1 0750 e6f8 e293 94df  .,.lA.)..P......
+00002ca0: 0000 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
+00002cb0: 0000 0021 00d0 b93e a68b 0100 000d 0300  ...!...>........
+00002cc0: 0010 0008 0164 6f63 5072 6f70 732f 6170  .....docProps/ap
+00002cd0: 702e 786d 6c20 a204 0128 a000 0100 0000  p.xml ...(......
 00002ce0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002d00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002d80: 0000 0000 0000 0000 009c 924f 4f1b 3110  ...........OO.1.
-00002d90: c5ef 48fd 0e2b df89 3714 2114 798d 2a68  ..H..+..7.!.y.*h
-00002da0: c581 aa91 92d0 239a dab3 590b c75e 7986  ......#...Y..^y.
-00002db0: 55c2 a7c7 bb2b c2a6 f4d4 dbfc 797a fef9  U....+......yz..
-00002dc0: d9ea 66bf f345 8789 5c0c 9598 cf4a 5160  ..f..E..\....JQ`
-00002dd0: 30d1 bab0 adc4 66fd e3fc 5a14 c410 2cf8  0.....f...Z...,.
-00002de0: 18b0 1207 2471 a3bf 9ca9 658a 2d26 7648  ....$q....e.-&vH
-00002df0: 45b6 0854 8986 b95d 4849 a6c1 1dd0 2caf  E..T...]HI....,.
-00002e00: 43de d431 ed80 739b b632 d6b5 3378 17cd  C..1..s..2..3x..
-00002e10: cb0e 03cb 8bb2 bc92 b867 0c16 ed79 7b34  .........g...y{4
-00002e20: 14a3 e3a2 e3ff 35b5 d1f4 7cf4 b83e b419  ......5...|..>..
-00002e30: 58ab 6f6d eb9d 01ce b7d4 3f9d 4991 62cd  X.om......?.I.b.
-00002e40: c5f7 bd41 afe4 74a9 32dd 0acd 4b72 7cd0  ...A..t.2...Kr|.
-00002e50: a592 d356 ad0c 78bc cdc6 ba06 4fa8 e4c7  ...V..x.....O...
-00002e60: 40dd 23f4 a12d c125 d2aa e345 8786 632a  @.#..-.%...E..c*
-00002e70: c8bd e6d8 2e44 f107 087b 9c4a 7490 1c04  .....D...{.Jt...
-00002e80: ce58 bd6c 6c86 dab7 c449 ff8e e999 1a44  .X.ll....I.....D
-00002e90: 2625 b360 1c0e e554 3bad dda5 9e0f 825c  &%.`...T;......\
-00002ea0: 9c0a 7b83 1124 2f4e 11d7 8e3d d2af 7a09  ..{..$/N...=..z.
-00002eb0: 89ff 413c 9f12 0f0c 23ef 8863 13d4 fc64  ..A<....#..c...d
-00002ec0: 81e1 c93a d3c7 0ae9 f009 7748 201f fcd7  ...:......wH ...
-00002ed0: 510f 2e3c d3a6 5dc7 3b60 7c8f f274 a856  Q..<..].;`|..t.V
-00002ee0: 0d24 b439 fd63 d4c7 81ba cf29 26df 9bdc  .$.9.c.....)&...
-00002ef0: 3610 b668 df35 9f17 fdc3 3f8e bf5b cfaf  6..h.5....?..[..
-00002f00: 66e5 d732 bfe9 64a6 e4c7 3fd6 6f00 0000  f..2..d...?.o...
-00002f10: ffff 0300 504b 0102 2d00 1400 0600 0800  ....PK..-.......
-00002f20: 0000 2100 4137 82cf 6e01 0000 0405 0000  ..!.A7..n.......
-00002f30: 1300 0000 0000 0000 0000 0000 0000 0000  ................
-00002f40: 0000 5b43 6f6e 7465 6e74 5f54 7970 6573  ..[Content_Types
-00002f50: 5d2e 786d 6c50 4b01 022d 0014 0006 0008  ].xmlPK..-......
-00002f60: 0000 0021 00b5 5530 23f4 0000 004c 0200  ...!..U0#....L..
-00002f70: 000b 0000 0000 0000 0000 0000 0000 00a7  ................
-00002f80: 0300 005f 7265 6c73 2f2e 7265 6c73 504b  ..._rels/.relsPK
-00002f90: 0102 2d00 1400 0600 0800 0000 2100 c97e  ..-.........!..~
-00002fa0: 6f47 5803 0000 6208 0000 0f00 0000 0000  oGX...b.........
-00002fb0: 0000 0000 0000 0000 cc06 0000 786c 2f77  ............xl/w
-00002fc0: 6f72 6b62 6f6f 6b2e 786d 6c50 4b01 022d  orkbook.xmlPK..-
-00002fd0: 0014 0006 0008 0000 0021 0081 3e94 97f3  .........!..>...
-00002fe0: 0000 00ba 0200 001a 0000 0000 0000 0000  ................
-00002ff0: 0000 0000 0051 0a00 0078 6c2f 5f72 656c  .....Q...xl/_rel
-00003000: 732f 776f 726b 626f 6f6b 2e78 6d6c 2e72  s/workbook.xml.r
-00003010: 656c 7350 4b01 022d 0014 0006 0008 0000  elsPK..-........
-00003020: 0021 0011 6d0f 68b4 0500 0024 1600 0018  .!..m.h....$....
-00003030: 0000 0000 0000 0000 0000 0000 0084 0c00  ................
-00003040: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
-00003050: 6865 6574 312e 786d 6c50 4b01 022d 0014  heet1.xmlPK..-..
-00003060: 0006 0008 0000 0021 00c1 1710 be4e 0700  .......!.....N..
-00003070: 00c6 2000 0013 0000 0000 0000 0000 0000  .. .............
-00003080: 0000 006e 1200 0078 6c2f 7468 656d 652f  ...n...xl/theme/
-00003090: 7468 656d 6531 2e78 6d6c 504b 0102 2d00  theme1.xmlPK..-.
-000030a0: 1400 0600 0800 0000 2100 137c 8b5b f108  ........!..|.[..
-000030b0: 0000 7646 0000 0d00 0000 0000 0000 0000  ..vF............
-000030c0: 0000 0000 ed19 0000 786c 2f73 7479 6c65  ........xl/style
-000030d0: 732e 786d 6c50 4b01 022d 0014 0006 0008  s.xmlPK..-......
-000030e0: 0000 0021 00b3 7cd6 e18a 0300 0030 0a00  ...!..|......0..
-000030f0: 0014 0000 0000 0000 0000 0000 0000 0009  ................
-00003100: 2300 0078 6c2f 7368 6172 6564 5374 7269  #..xl/sharedStri
-00003110: 6e67 732e 786d 6c50 4b01 022d 0014 0006  ngs.xmlPK..-....
-00003120: 0008 0000 0021 003b 6d32 4bc1 0000 0042  .....!.;m2K....B
-00003130: 0100 0023 0000 0000 0000 0000 0000 0000  ...#............
-00003140: 00c5 2600 0078 6c2f 776f 726b 7368 6565  ..&..xl/workshee
-00003150: 7473 2f5f 7265 6c73 2f73 6865 6574 312e  ts/_rels/sheet1.
-00003160: 786d 6c2e 7265 6c73 504b 0102 2d00 1400  xml.relsPK..-...
-00003170: 0600 0800 0000 2100 cfe0 47b4 c201 0000  ......!...G.....
-00003180: 2c15 0000 2700 0000 0000 0000 0000 0000  ,...'...........
-00003190: 0000 c727 0000 786c 2f70 7269 6e74 6572  ...'..xl/printer
-000031a0: 5365 7474 696e 6773 2f70 7269 6e74 6572  Settings/printer
-000031b0: 5365 7474 696e 6773 312e 6269 6e50 4b01  Settings1.binPK.
-000031c0: 022d 0014 0006 0008 0000 0021 00cb 9514  .-.........!....
-000031d0: e34e 0100 0071 0200 0011 0000 0000 0000  .N...q..........
-000031e0: 0000 0000 0000 00ce 2900 0064 6f63 5072  ........)..docPr
-000031f0: 6f70 732f 636f 7265 2e78 6d6c 504b 0102  ops/core.xmlPK..
-00003200: 2d00 1400 0600 0800 0000 2100 d0b9 3ea6  -.........!...>.
-00003210: 8b01 0000 0d03 0000 1000 0000 0000 0000  ................
-00003220: 0000 0000 0000 532c 0000 646f 6350 726f  ......S,..docPro
-00003230: 7073 2f61 7070 2e78 6d6c 504b 0506 0000  ps/app.xmlPK....
-00003240: 0000 0c00 0c00 2603 0000 142f 0000 0000  ......&..../....
+00002d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002dd0: 0000 0000 0000 0000 0000 0000 009c 924f  ...............O
+00002de0: 4f1b 3110 c5ef 48fd 0e2b df89 3714 2114  O.1...H..+..7.!.
+00002df0: 798d 2a68 c581 aa91 92d0 239a dab3 590b  y.*h......#...Y.
+00002e00: c75e 7986 55c2 a7c7 bb2b c2a6 f4d4 dbfc  .^y.U....+......
+00002e10: 797a fef9 d9ea 66bf f345 8789 5c0c 9598  yz....f..E..\...
+00002e20: cf4a 5160 30d1 bab0 adc4 66fd e3fc 5a14  .JQ`0.....f...Z.
+00002e30: c410 2cf8 18b0 1207 2471 a3bf 9ca9 658a  ..,.....$q....e.
+00002e40: 2d26 7648 45b6 0854 8986 b95d 4849 a6c1  -&vHE..T...]HI..
+00002e50: 1dd0 2caf 43de d431 ed80 739b b632 d6b5  ..,.C..1..s..2..
+00002e60: 3378 17cd cb0e 03cb 8bb2 bc92 b867 0c16  3x...........g..
+00002e70: ed79 7b34 14a3 e3a2 e3ff 35b5 d1f4 7cf4  .y{4......5...|.
+00002e80: b83e b419 58ab 6f6d eb9d 01ce b7d4 3f9d  .>..X.om......?.
+00002e90: 4991 62cd c5f7 bd41 afe4 74a9 32dd 0acd  I.b....A..t.2...
+00002ea0: 4b72 7cd0 a592 d356 ad0c 78bc cdc6 ba06  Kr|....V..x.....
+00002eb0: 4fa8 e4c7 40dd 23f4 a12d c125 d2aa e345  O...@.#..-.%...E
+00002ec0: 8786 632a c8bd e6d8 2e44 f107 087b 9c4a  ..c*.....D...{.J
+00002ed0: 7490 1c04 ce58 bd6c 6c86 dab7 c449 ff8e  t....X.ll....I..
+00002ee0: e999 1a44 2625 b360 1c0e e554 3bad dda5  ...D&%.`...T;...
+00002ef0: 9e0f 825c 9c0a 7b83 1124 2f4e 11d7 8e3d  ...\..{..$/N...=
+00002f00: d2af 7a09 89ff 413c 9f12 0f0c 23ef 8863  ..z...A<....#..c
+00002f10: 13d4 fc64 81e1 c93a d3c7 0ae9 f009 7748  ...d...:......wH
+00002f20: 201f fcd7 510f 2e3c d3a6 5dc7 3b60 7c8f   ...Q..<..].;`|.
+00002f30: f274 a856 0d24 b439 fd63 d4c7 81ba cf29  .t.V.$.9.c.....)
+00002f40: 26df 9bdc 3610 b668 df35 9f17 fdc3 3f8e  &...6..h.5....?.
+00002f50: bf5b cfaf 66e5 d732 bfe9 64a6 e4c7 3fd6  .[..f..2..d...?.
+00002f60: 6f00 0000 ffff 0300 504b 0102 2d00 1400  o.......PK..-...
+00002f70: 0600 0800 0000 2100 4137 82cf 6e01 0000  ......!.A7..n...
+00002f80: 0405 0000 1300 0000 0000 0000 0000 0000  ................
+00002f90: 0000 0000 0000 5b43 6f6e 7465 6e74 5f54  ......[Content_T
+00002fa0: 7970 6573 5d2e 786d 6c50 4b01 022d 0014  ypes].xmlPK..-..
+00002fb0: 0006 0008 0000 0021 00b5 5530 23f4 0000  .......!..U0#...
+00002fc0: 004c 0200 000b 0000 0000 0000 0000 0000  .L..............
+00002fd0: 0000 00a7 0300 005f 7265 6c73 2f2e 7265  ......._rels/.re
+00002fe0: 6c73 504b 0102 2d00 1400 0600 0800 0000  lsPK..-.........
+00002ff0: 2100 25bf 56fe 5f03 0000 5308 0000 0f00  !.%.V._...S.....
+00003000: 0000 0000 0000 0000 0000 0000 cc06 0000  ................
+00003010: 786c 2f77 6f72 6b62 6f6f 6b2e 786d 6c50  xl/workbook.xmlP
+00003020: 4b01 022d 0014 0006 0008 0000 0021 0081  K..-.........!..
+00003030: 3e94 97f3 0000 00ba 0200 001a 0000 0000  >...............
+00003040: 0000 0000 0000 0000 0058 0a00 0078 6c2f  .........X...xl/
+00003050: 5f72 656c 732f 776f 726b 626f 6f6b 2e78  _rels/workbook.x
+00003060: 6d6c 2e72 656c 7350 4b01 022d 0014 0006  ml.relsPK..-....
+00003070: 0008 0000 0021 00bd c503 36ea 0500 00a5  .....!....6.....
+00003080: 1700 0018 0000 0000 0000 0000 0000 0000  ................
+00003090: 008b 0c00 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
+000030a0: 7473 2f73 6865 6574 312e 786d 6c50 4b01  ts/sheet1.xmlPK.
+000030b0: 022d 0014 0006 0008 0000 0021 00c1 1710  .-.........!....
+000030c0: be4e 0700 00c6 2000 0013 0000 0000 0000  .N.... .........
+000030d0: 0000 0000 0000 00ab 1200 0078 6c2f 7468  ...........xl/th
+000030e0: 656d 652f 7468 656d 6531 2e78 6d6c 504b  eme/theme1.xmlPK
+000030f0: 0102 2d00 1400 0600 0800 0000 2100 137c  ..-.........!..|
+00003100: 8b5b f108 0000 7646 0000 0d00 0000 0000  .[....vF........
+00003110: 0000 0000 0000 0000 2a1a 0000 786c 2f73  ........*...xl/s
+00003120: 7479 6c65 732e 786d 6c50 4b01 022d 0014  tyles.xmlPK..-..
+00003130: 0006 0008 0000 0021 009e 630a b8a2 0300  .......!..c.....
+00003140: 0096 0a00 0014 0000 0000 0000 0000 0000  ................
+00003150: 0000 0046 2300 0078 6c2f 7368 6172 6564  ...F#..xl/shared
+00003160: 5374 7269 6e67 732e 786d 6c50 4b01 022d  Strings.xmlPK..-
+00003170: 0014 0006 0008 0000 0021 003b 6d32 4bc1  .........!.;m2K.
+00003180: 0000 0042 0100 0023 0000 0000 0000 0000  ...B...#........
+00003190: 0000 0000 001a 2700 0078 6c2f 776f 726b  ......'..xl/work
+000031a0: 7368 6565 7473 2f5f 7265 6c73 2f73 6865  sheets/_rels/she
+000031b0: 6574 312e 786d 6c2e 7265 6c73 504b 0102  et1.xml.relsPK..
+000031c0: 2d00 1400 0600 0800 0000 2100 cfe0 47b4  -.........!...G.
+000031d0: c201 0000 2c15 0000 2700 0000 0000 0000  ....,...'.......
+000031e0: 0000 0000 0000 1c28 0000 786c 2f70 7269  .......(..xl/pri
+000031f0: 6e74 6572 5365 7474 696e 6773 2f70 7269  nterSettings/pri
+00003200: 6e74 6572 5365 7474 696e 6773 312e 6269  nterSettings1.bi
+00003210: 6e50 4b01 022d 0014 0006 0008 0000 0021  nPK..-.........!
+00003220: 0011 f2fe 2d4d 0100 0071 0200 0011 0000  ....-M...q......
+00003230: 0000 0000 0000 0000 0000 0023 2a00 0064  ...........#*..d
+00003240: 6f63 5072 6f70 732f 636f 7265 2e78 6d6c  ocProps/core.xml
+00003250: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
+00003260: d0b9 3ea6 8b01 0000 0d03 0000 1000 0000  ..>.............
+00003270: 0000 0000 0000 0000 0000 a72c 0000 646f  ...........,..do
+00003280: 6350 726f 7073 2f61 7070 2e78 6d6c 504b  cProps/app.xmlPK
+00003290: 0506 0000 0000 0c00 0c00 2603 0000 682f  ..........&...h/
+000032a0: 0000 0000                                ....
```

### Comparing `sdmc_adhoc_processing-0.1.44/src/sdmc_adhoc_processing/generate_dict.py` & `sdmc_adhoc_processing-0.1.45/src/sdmc_adhoc_processing/generate_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,20 @@
 # build data dict ------------------------------------------------------------##
 template_dict = pd.read_excel(template_dict_path)
 template_vars = list(template_dict.variable_name)
 
 processed_data = pd.read_csv(processed_data_path, sep="\t")
 processed_data_vars = list(processed_data.columns)
 
+def gen_data_dict():
+    if os.path.exists(output_dir + data_dict_fname):
+        edit_existing_dict()
+    else:
+        build_brand_new_dict()
+
 def save_dict(dict_to_save):
     writer = pd.ExcelWriter(
         output_dir + data_dict_fname,
         engine='xlsxwriter'
     )
     dict_to_save.to_excel(writer, sheet_name="Sheet1", index=False)
     workbook = writer.book
```

### Comparing `sdmc_adhoc_processing-0.1.44/src/sdmc_adhoc_processing/process.py` & `sdmc_adhoc_processing-0.1.45/src/sdmc_adhoc_processing/process.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,69 @@
 import pandas as pd
+import numpy as np
 import os
 from typing import List, Union
 import datetime
 from sdmc_adhoc_processing import constants
 
+def standard_processing(
+    input_data: pd.DataFrame,
+    input_data_path: str,
+    guspec_col: str,
+    network: str,
+    metadata_dict: dict,
+    ldms: pd.DataFrame,
+    ldms_usecols: List[str] = constants.STANDARD_COLS,
+    ) -> pd.DataFrame:
+    """
+    INPUTS
+    ------
+    input_data: pd.DataFrame, long/desired format,
+    input_data_path: str, filepath to the input data
+    guspec_col: str, name of the global identifier (guspec) in input_data
+    network: str, either "hvtn" or "covpn"
+    metadata_dict: dict; keys are column names, values are column values
+    ldms: pd.DataFrame, should contain guspec + all other desired vars to merge
+    ldms_usecols: columns to merge on from ldms.
+
+    OUTPUTS
+    -------
+    data formatted with the following merged on:
+    - ldms columns
+    - metadata from "metadata_dict"
+    - sdmc processing info
+
+    sorted in standard order
+    """
+
+    dh = DataHandler(
+    input_data = input_data,
+    guspec_col = guspec_col,
+    network = network.lower()
+    )
+    dh.ldms = ldms.copy()
+
+    # merge ldms
+    dh.add_ldms(cols = ldms_usecols,
+                incl_spec_type=True,
+                map_drawdt=True,
+                relabel=True,
+                enforce_typing=True)
+
+    dh.add_metadata(metadata_dict)
+    dh.add_sdmc_processing_info(input_data_path=input_data_path)
+
+    if guspec_col!="guspec":
+        dh.processed_data = dh.processed_data.drop(columns=guspec_col)
+
+    reorder = dh.reorder_cols(dh.processed_data.columns)
+
+    return dh.processed_data[reorder]
+
+
 class DataHandler:
     def __init__(
         self,
         input_data: pd.DataFrame,
         guspec_col: str,
         network: str,
         input_data_path: str = None,
@@ -72,15 +128,16 @@
             return "MISSING FROM MAP"
 
     def add_ldms(
         self,
         cols: List[str],
         incl_spec_type: bool = True,
         map_drawdt: bool = True,
-        relabel: bool = True
+        relabel: bool = True,
+        enforce_typing = True
     ):
         """
         Merge self.ldms onto self.processed_data
         Optionally add spec_type and drawdt columns
         Optionally relabel with standard relabelling names
         """
         if not cols:
@@ -106,30 +163,32 @@
 
         if map_drawdt:
             ldms["drawdt"] = ldms.apply(
                 lambda x: datetime.date(x.drawdy, x.drawdm, x.drawdd).isoformat(), axis=1
             )
             ldms = ldms.drop(columns=["drawdy", "drawdm", "drawdd"])
 
+        if enforce_typing:
+            for col in ['txtpid', 'lstudy']:
+                if col in ldms.columns:
+                    ldms[col] = ldms[col].astype(int).astype("string")
+            if 'vidval' in ldms.columns:
+                ldms.vidval = ldms.vidval.astype("string")
+
         if relabel:
             ldms = ldms.rename(columns=constants.LDMS_RELABEL_DICT)
 
         # merge ldms on
         self.processed_data = self.processed_data.merge(
             ldms,
             left_on=self.guspec_col,
             right_on="guspec",
             how="left"
         )
 
-    def enfornce_ldms_typing():
-        for col in ['ptid', 'protocol']:
-            if col in self.processed_data.columns:
-                self.processed_data[col] = self.processed_data[col].astype(int).astype(str)
-
     def add_metadata(self, metadata: dict):
         """
         INPUT: dictionary of column names and values.
         INPUT EXAMPLE: {"upload_lab_id": "DG",
                         "assay_lab_name": "Geraghty Lab (FHCRC)",
                         "instrument": "Illumina NGS"}
         FUNCTION: adds corresponding columns to self.processed_data
@@ -173,7 +232,23 @@
 
         # if these columns are already in processed_data, drop and replace
         already_exists = set(sdmc_metadata.columns).intersection(self.processed_data.columns)
         self.processed_data = self.processed_data.drop(columns=already_exists)
 
         # add processing metadata columns
         self.processed_data = self.processed_data.merge(sdmc_metadata, how="cross")
+
+    def reorder_cols(self, input_cols: List[str]) -> List[str]:
+        usecols = []
+        for col in constants.STD_PREFACE_COLS:
+            if col in input_cols:
+                usecols += [col]
+        for col in np.sort(list(set(input_cols).difference(
+        constants.STD_PREFACE_COLS + constants.STD_POSTFACE_COLS
+        ))):
+            usecols += [col]
+
+        for col in constants.STD_POSTFACE_COLS:
+            if col in input_cols:
+                usecols += [col]
+
+        return usecols
```

### Comparing `sdmc_adhoc_processing-0.1.44/src/sdmc_adhoc_processing.egg-info/PKG-INFO` & `sdmc_adhoc_processing-0.1.45/src/sdmc_adhoc_processing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdmc_adhoc_processing
-Version: 0.1.44
+Version: 0.1.45
 Summary: Helper utilities for SDMC ad-hoc data processing requests.
 Author-email: Beatrix Haddock <beatrix.haddock@gmail.com>
 Project-URL: Homepage, https://github.com/beatrixh/sdmc-adhoc-processing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `sdmc_adhoc_processing-0.1.44/src/sdmc_adhoc_processing.egg-info/SOURCES.txt` & `sdmc_adhoc_processing-0.1.45/src/sdmc_adhoc_processing.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 LICENSE
 README.md
 pyproject.toml
 src/sdmc_adhoc_processing/__init__.py
 src/sdmc_adhoc_processing/constants.py
 src/sdmc_adhoc_processing/data_dictionary_TEMPLATE.xlsx
+src/sdmc_adhoc_processing/data_dictionary_nonstandard_vars.xlsx
+src/sdmc_adhoc_processing/generate_README.py
 src/sdmc_adhoc_processing/generate_dict.py
 src/sdmc_adhoc_processing/process.py
+src/sdmc_adhoc_processing/readme_template.md
+src/sdmc_adhoc_processing/utilities.py
 src/sdmc_adhoc_processing.egg-info/PKG-INFO
 src/sdmc_adhoc_processing.egg-info/SOURCES.txt
 src/sdmc_adhoc_processing.egg-info/dependency_links.txt
 src/sdmc_adhoc_processing.egg-info/entry_points.txt
 src/sdmc_adhoc_processing.egg-info/requires.txt
 src/sdmc_adhoc_processing.egg-info/top_level.txt
 tests/test_foo.py
```

