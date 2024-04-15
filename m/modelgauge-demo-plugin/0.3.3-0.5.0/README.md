# Comparing `tmp/modelgauge_demo_plugin-0.3.3.tar.gz` & `tmp/modelgauge_demo_plugin-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelgauge_demo_plugin-0.3.3.tar", max compression
+gzip compressed data, was "modelgauge_demo_plugin-0.5.0.tar", max compression
```

## Comparing `modelgauge_demo_plugin-0.3.3.tar` & `modelgauge_demo_plugin-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      321 2024-04-11 19:30:18.206705 modelgauge_demo_plugin-0.3.3/README.md
--rw-r--r--   0        0        0     2132 2024-04-11 19:47:59.766737 modelgauge_demo_plugin-0.3.3/modelgauge/annotators/__pycache__/demo_annotator.cpython-310.pyc
--rw-r--r--   0        0        0     1331 2024-04-11 19:30:18.206705 modelgauge_demo_plugin-0.3.3/modelgauge/annotators/demo_annotator.py
--rw-r--r--   0        0        0     2425 2024-04-11 19:47:59.776737 modelgauge_demo_plugin-0.3.3/modelgauge/suts/__pycache__/demo_01_yes_no_sut.cpython-310.pyc
--rw-r--r--   0        0        0     5501 2024-04-11 19:47:59.778737 modelgauge_demo_plugin-0.3.3/modelgauge/suts/__pycache__/demo_02_secrets_and_options_sut.cpython-310.pyc
--rw-r--r--   0        0        0     2524 2024-04-11 19:47:59.780737 modelgauge_demo_plugin-0.3.3/modelgauge/suts/__pycache__/demo_03_sut_with_args.cpython-310.pyc
--rw-r--r--   0        0        0     1726 2024-04-11 19:30:18.206705 modelgauge_demo_plugin-0.3.3/modelgauge/suts/demo_01_yes_no_sut.py
--rw-r--r--   0        0        0     5599 2024-04-11 19:30:18.206705 modelgauge_demo_plugin-0.3.3/modelgauge/suts/demo_02_secrets_and_options_sut.py
--rw-r--r--   0        0        0     2003 2024-04-11 19:30:18.207705 modelgauge_demo_plugin-0.3.3/modelgauge/suts/demo_03_sut_with_args.py
--rw-r--r--   0        0        0     3187 2024-04-11 19:47:59.762737 modelgauge_demo_plugin-0.3.3/modelgauge/tests/__pycache__/demo_01_simple_qa_test.cpython-310-pytest-7.4.4.pyc
--rw-r--r--   0        0        0     3078 2024-04-12 18:57:05.154892 modelgauge_demo_plugin-0.3.3/modelgauge/tests/__pycache__/demo_01_simple_qa_test.cpython-310.pyc
--rw-r--r--   0        0        0     3478 2024-04-11 19:47:59.763737 modelgauge_demo_plugin-0.3.3/modelgauge/tests/__pycache__/demo_02_unpacking_dependency_test.cpython-310-pytest-7.4.4.pyc
--rw-r--r--   0        0        0     3369 2024-04-12 18:57:05.156892 modelgauge_demo_plugin-0.3.3/modelgauge/tests/__pycache__/demo_02_unpacking_dependency_test.cpython-310.pyc
--rw-r--r--   0        0        0     4213 2024-04-11 19:47:59.764737 modelgauge_demo_plugin-0.3.3/modelgauge/tests/__pycache__/demo_03_paired_prompts_test.cpython-310-pytest-7.4.4.pyc
--rw-r--r--   0        0        0     4104 2024-04-12 18:57:05.157892 modelgauge_demo_plugin-0.3.3/modelgauge/tests/__pycache__/demo_03_paired_prompts_test.cpython-310.pyc
--rw-r--r--   0        0        0     3536 2024-04-11 19:47:59.766737 modelgauge_demo_plugin-0.3.3/modelgauge/tests/__pycache__/demo_04_using_annotation_test.cpython-310-pytest-7.4.4.pyc
--rw-r--r--   0        0        0     3427 2024-04-12 18:57:05.159892 modelgauge_demo_plugin-0.3.3/modelgauge/tests/__pycache__/demo_04_using_annotation_test.cpython-310.pyc
--rw-r--r--   0        0        0     3414 2024-04-11 19:30:18.207705 modelgauge_demo_plugin-0.3.3/modelgauge/tests/demo_01_simple_qa_test.py
--rw-r--r--   0        0        0     3727 2024-04-11 19:30:18.207705 modelgauge_demo_plugin-0.3.3/modelgauge/tests/demo_02_unpacking_dependency_test.py
--rw-r--r--   0        0        0     4784 2024-04-11 19:30:18.207705 modelgauge_demo_plugin-0.3.3/modelgauge/tests/demo_03_paired_prompts_test.py
--rw-r--r--   0        0        0     3120 2024-04-11 19:30:18.207705 modelgauge_demo_plugin-0.3.3/modelgauge/tests/demo_04_using_annotation_test.py
--rw-r--r--   0        0        0        0 2024-04-11 19:30:18.207705 modelgauge_demo_plugin-0.3.3/modelgauge/tests/specifications/README.md
--rw-r--r--   0        0        0       79 2024-04-11 19:30:18.207705 modelgauge_demo_plugin-0.3.3/modelgauge/tests/specifications/demo_01.toml
--rw-r--r--   0        0        0      343 2024-04-12 18:56:17.756891 modelgauge_demo_plugin-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      747 1970-01-01 00:00:00.000000 modelgauge_demo_plugin-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      321 2024-04-11 19:30:18.206705 modelgauge_demo_plugin-0.5.0/README.md
+-rw-r--r--   0        0        0     2135 2024-04-15 22:06:29.094003 modelgauge_demo_plugin-0.5.0/modelgauge/annotators/__pycache__/demo_annotator.cpython-310.pyc
+-rw-r--r--   0        0        0     1334 2024-04-15 22:05:52.196001 modelgauge_demo_plugin-0.5.0/modelgauge/annotators/demo_annotator.py
+-rw-r--r--   0        0        0     2425 2024-04-11 19:47:59.776737 modelgauge_demo_plugin-0.5.0/modelgauge/suts/__pycache__/demo_01_yes_no_sut.cpython-310.pyc
+-rw-r--r--   0        0        0     5501 2024-04-11 19:47:59.778737 modelgauge_demo_plugin-0.5.0/modelgauge/suts/__pycache__/demo_02_secrets_and_options_sut.cpython-310.pyc
+-rw-r--r--   0        0        0     2524 2024-04-11 19:47:59.780737 modelgauge_demo_plugin-0.5.0/modelgauge/suts/__pycache__/demo_03_sut_with_args.cpython-310.pyc
+-rw-r--r--   0        0        0     1726 2024-04-11 19:30:18.206705 modelgauge_demo_plugin-0.5.0/modelgauge/suts/demo_01_yes_no_sut.py
+-rw-r--r--   0        0        0     5599 2024-04-11 19:30:18.206705 modelgauge_demo_plugin-0.5.0/modelgauge/suts/demo_02_secrets_and_options_sut.py
+-rw-r--r--   0        0        0     2003 2024-04-11 19:30:18.207705 modelgauge_demo_plugin-0.5.0/modelgauge/suts/demo_03_sut_with_args.py
+-rw-r--r--   0        0        0     3187 2024-04-11 19:47:59.762737 modelgauge_demo_plugin-0.5.0/modelgauge/tests/__pycache__/demo_01_simple_qa_test.cpython-310-pytest-7.4.4.pyc
+-rw-r--r--   0        0        0     3078 2024-04-12 18:57:05.154892 modelgauge_demo_plugin-0.5.0/modelgauge/tests/__pycache__/demo_01_simple_qa_test.cpython-310.pyc
+-rw-r--r--   0        0        0     3478 2024-04-11 19:47:59.763737 modelgauge_demo_plugin-0.5.0/modelgauge/tests/__pycache__/demo_02_unpacking_dependency_test.cpython-310-pytest-7.4.4.pyc
+-rw-r--r--   0        0        0     3369 2024-04-12 18:57:05.156892 modelgauge_demo_plugin-0.5.0/modelgauge/tests/__pycache__/demo_02_unpacking_dependency_test.cpython-310.pyc
+-rw-r--r--   0        0        0     4213 2024-04-11 19:47:59.764737 modelgauge_demo_plugin-0.5.0/modelgauge/tests/__pycache__/demo_03_paired_prompts_test.cpython-310-pytest-7.4.4.pyc
+-rw-r--r--   0        0        0     4104 2024-04-12 18:57:05.157892 modelgauge_demo_plugin-0.5.0/modelgauge/tests/__pycache__/demo_03_paired_prompts_test.cpython-310.pyc
+-rw-r--r--   0        0        0     3536 2024-04-11 19:47:59.766737 modelgauge_demo_plugin-0.5.0/modelgauge/tests/__pycache__/demo_04_using_annotation_test.cpython-310-pytest-7.4.4.pyc
+-rw-r--r--   0        0        0     3427 2024-04-12 18:57:05.159892 modelgauge_demo_plugin-0.5.0/modelgauge/tests/__pycache__/demo_04_using_annotation_test.cpython-310.pyc
+-rw-r--r--   0        0        0     3414 2024-04-11 19:30:18.207705 modelgauge_demo_plugin-0.5.0/modelgauge/tests/demo_01_simple_qa_test.py
+-rw-r--r--   0        0        0     3727 2024-04-11 19:30:18.207705 modelgauge_demo_plugin-0.5.0/modelgauge/tests/demo_02_unpacking_dependency_test.py
+-rw-r--r--   0        0        0     4784 2024-04-11 19:30:18.207705 modelgauge_demo_plugin-0.5.0/modelgauge/tests/demo_03_paired_prompts_test.py
+-rw-r--r--   0        0        0     3120 2024-04-11 19:30:18.207705 modelgauge_demo_plugin-0.5.0/modelgauge/tests/demo_04_using_annotation_test.py
+-rw-r--r--   0        0        0        0 2024-04-11 19:30:18.207705 modelgauge_demo_plugin-0.5.0/modelgauge/tests/specifications/README.md
+-rw-r--r--   0        0        0       79 2024-04-11 19:30:18.207705 modelgauge_demo_plugin-0.5.0/modelgauge/tests/specifications/demo_01.toml
+-rw-r--r--   0        0        0      343 2024-04-15 22:05:52.196001 modelgauge_demo_plugin-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      747 1970-01-01 00:00:00.000000 modelgauge_demo_plugin-0.5.0/PKG-INFO
```

### Comparing `modelgauge_demo_plugin-0.3.3/modelgauge/annotators/__pycache__/demo_annotator.cpython-310.pyc` & `modelgauge_demo_plugin-0.5.0/modelgauge/annotators/__pycache__/demo_annotator.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 11 19:30:18 2024 UTC, .py size: 1331 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4a3a 1866 3305 0000  o.......J:.f3...
+00000000: 6f0d 0d0a 0000 0000 c0a4 1d66 3605 0000  o..........f6...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 7800 0000 6400  .....@...sx...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6405 6406 8400 6406 6507 8303 5a08 4700  d.d...d.e...Z.G.
 00000070: 6407 6408 8400 6408 6507 8303 5a09 4700  d.d...d.e...Z.G.
@@ -53,82 +53,82 @@
 00000340: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
 00000350: 0000 0400 0000 4000 0000 7346 0000 0065  ......@...sF...e
 00000360: 005a 0164 005a 0264 015a 0364 0265 0464  .Z.d.Z.d.Z.d.e.d
 00000370: 0365 0566 0464 0464 0584 045a 0664 0665  .e.f.d.d...Z.d.e
 00000380: 0764 0765 0866 0464 0864 0984 045a 0964  .d.e.f.d.d...Z.d
 00000390: 0a65 0864 0765 0a66 0464 0b64 0c84 045a  .e.d.e.f.d.d...Z
 000003a0: 0b64 0d53 0029 0eda 1144 656d 6f59 4261  .d.S.)...DemoYBa
-000003b0: 6441 6e6e 6f74 6174 6f72 610f 0100 0041  dAnnotatora....A
+000003b0: 6441 6e6e 6f74 6174 6f72 6112 0100 0041  dAnnotatora....A
 000003c0: 2064 656d 6f6e 7374 7261 7469 6f6e 2061   demonstration a
 000003d0: 6e6e 6f74 6174 6f72 2074 6861 7420 6469  nnotator that di
 000003e0: 736c 696b 6573 2074 6865 206c 6574 7465  slikes the lette
 000003f0: 7220 592e 0a0a 2020 2020 5265 616c 2041  r Y...    Real A
 00000400: 6e6e 6f74 6174 6f72 7320 6172 6520 696e  nnotators are in
 00000410: 7465 6e64 6564 2074 6f20 646f 2065 7870  tended to do exp
 00000420: 656e 7369 7665 2070 726f 6365 7373 696e  ensive processin
 00000430: 6720 6f6e 2074 6865 2073 7472 696e 672c  g on the string,
 00000440: 0a20 2020 2073 7563 6820 6173 2063 616c  .    such as cal
 00000450: 6c69 6e67 2061 6e6f 7468 6572 206d 6f64  ling another mod
-00000460: 656c 2063 6f6c 6c65 6374 696e 6720 6461  el collecting da
-00000470: 7461 2066 726f 6d20 6875 6d61 6e20 7261  ta from human ra
-00000480: 7465 7273 2e20 466f 720a 2020 2020 7468  ters. For.    th
-00000490: 6520 6465 6d6f 2074 686f 7567 682c 2077  e demo though, w
-000004a0: 6520 7761 6e74 2073 6f6d 6574 6869 6e67  e want something
-000004b0: 2063 6865 6170 2061 6e64 2064 6574 6572   cheap and deter
-000004c0: 6d69 6e69 7374 6963 2e0a 2020 2020 da06  ministic..    ..
-000004d0: 7072 6f6d 7074 da0a 636f 6d70 6c65 7469  prompt..completi
-000004e0: 6f6e 6303 0000 0000 0000 0000 0000 0003  onc.............
-000004f0: 0000 0003 0000 0043 0000 00f3 0c00 0000  .......C........
-00000500: 7400 7c02 6a01 6401 8d01 5300 2902 4e29  t.|.j.d...S.).N)
-00000510: 0172 1200 0000 2902 7211 0000 0072 1200  .r....).r....r..
-00000520: 0000 2903 da04 7365 6c66 7218 0000 0072  ..)...selfr....r
-00000530: 1900 0000 720e 0000 0072 0e00 0000 720f  ....r....r....r.
-00000540: 0000 00da 1174 7261 6e73 6c61 7465 5f72  .....translate_r
-00000550: 6571 7565 7374 1d00 0000 7302 0000 000c  equest....s.....
-00000560: 017a 2344 656d 6f59 4261 6441 6e6e 6f74  .z#DemoYBadAnnot
-00000570: 6174 6f72 2e74 7261 6e73 6c61 7465 5f72  ator.translate_r
-00000580: 6571 7565 7374 da12 616e 6e6f 7461 7469  equest..annotati
-00000590: 6f6e 5f72 6571 7565 7374 da06 7265 7475  on_request..retu
-000005a0: 726e 6302 0000 0000 0000 0000 0000 0004  rnc.............
-000005b0: 0000 0003 0000 0043 0000 0073 2a00 0000  .......C...s*...
-000005c0: 6401 7d02 7c01 6a00 4400 5d0a 7d03 7c03  d.}.|.j.D.].}.|.
-000005d0: 6402 7600 720f 7c02 6403 3700 7d02 7105  d.v.r.|.d.7.}.q.
-000005e0: 7401 7c02 6404 8d01 5300 2905 4e72 0100  t.|.d...S.).Nr..
-000005f0: 0000 3e02 0000 00da 0179 da01 59e9 0100  ..>......y..Y...
-00000600: 0000 2901 7216 0000 0029 0272 1200 0000  ..).r....).r....
-00000610: 7215 0000 0029 0472 1b00 0000 721d 0000  r....).r....r...
-00000620: 0072 1600 0000 da09 6368 6172 6163 7465  .r......characte
-00000630: 7272 0e00 0000 720e 0000 0072 0f00 0000  rr....r....r....
-00000640: da08 616e 6e6f 7461 7465 2000 0000 730c  ..annotate ...s.
-00000650: 0000 0004 010a 0108 0108 0102 800a 017a  ...............z
-00000660: 1a44 656d 6f59 4261 6441 6e6e 6f74 6174  .DemoYBadAnnotat
-00000670: 6f72 2e61 6e6e 6f74 6174 65da 0872 6573  or.annotate..res
-00000680: 706f 6e73 6563 0300 0000 0000 0000 0000  ponsec..........
-00000690: 0000 0300 0000 0300 0000 4300 0000 721a  ..........C...r.
-000006a0: 0000 0029 024e 2901 7207 0000 0029 0272  ...).N).r....).r
-000006b0: 0600 0000 7216 0000 0029 0372 1b00 0000  ....r....).r....
-000006c0: da07 7265 7175 6573 7472 2400 0000 720e  ..requestr$...r.
-000006d0: 0000 0072 0e00 0000 720f 0000 00da 1274  ...r....r......t
-000006e0: 7261 6e73 6c61 7465 5f72 6573 706f 6e73  ranslate_respons
-000006f0: 6527 0000 0073 0200 0000 0c03 7a24 4465  e'...s......z$De
-00000700: 6d6f 5942 6164 416e 6e6f 7461 746f 722e  moYBadAnnotator.
-00000710: 7472 616e 736c 6174 655f 7265 7370 6f6e  translate_respon
-00000720: 7365 4e29 0c72 0800 0000 7209 0000 0072  seN).r....r....r
-00000730: 0a00 0000 720b 0000 0072 0300 0000 7204  ....r....r....r.
-00000740: 0000 0072 1c00 0000 7211 0000 0072 1500  ...r....r....r..
-00000750: 0000 7223 0000 0072 0600 0000 7226 0000  ..r#...r....r&..
-00000760: 0072 0e00 0000 720e 0000 0072 0e00 0000  .r....r....r....
-00000770: 720f 0000 0072 1700 0000 1500 0000 7312  r....r........s.
-00000780: 0000 0008 0004 0112 0712 0302 0702 0102  ................
-00000790: ff02 020e fe72 1700 0000 4e29 0cda 146d  .....r....N)...m
-000007a0: 6f64 656c 6761 7567 652e 616e 6e6f 7461  odelgauge.annota
-000007b0: 746f 7272 0200 0000 da26 6d6f 6465 6c67  torr.....&modelg
-000007c0: 6175 6765 2e73 696e 676c 655f 7475 726e  auge.single_turn
-000007d0: 5f70 726f 6d70 745f 7265 7370 6f6e 7365  _prompt_response
-000007e0: 7203 0000 00da 0e6d 6f64 656c 6761 7567  r......modelgaug
-000007f0: 652e 7375 7472 0400 0000 da08 7079 6461  e.sutr......pyda
-00000800: 6e74 6963 7205 0000 0072 0600 0000 7211  nticr....r....r.
-00000810: 0000 0072 1500 0000 7217 0000 0072 0e00  ...r....r....r..
-00000820: 0000 720e 0000 0072 0e00 0000 720f 0000  ..r....r....r...
-00000830: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00000840: 1000 0000 0c00 0c01 0c01 0c01 1003 1006  ................
-00000850: 1004 1804                                ....
+00000460: 656c 206f 7220 636f 6c6c 6563 7469 6e67  el or collecting
+00000470: 2064 6174 6120 6672 6f6d 2068 756d 616e   data from human
+00000480: 2072 6174 6572 732e 2046 6f72 0a20 2020   raters. For.   
+00000490: 2074 6865 2064 656d 6f20 7468 6f75 6768   the demo though
+000004a0: 2c20 7765 2077 616e 7420 736f 6d65 7468  , we want someth
+000004b0: 696e 6720 6368 6561 7020 616e 6420 6465  ing cheap and de
+000004c0: 7465 726d 696e 6973 7469 632e 0a20 2020  terministic..   
+000004d0: 20da 0670 726f 6d70 74da 0a63 6f6d 706c   ..prompt..compl
+000004e0: 6574 696f 6e63 0300 0000 0000 0000 0000  etionc..........
+000004f0: 0000 0300 0000 0300 0000 4300 0000 f30c  ..........C.....
+00000500: 0000 0074 007c 026a 0164 018d 0153 0029  ...t.|.j.d...S.)
+00000510: 024e 2901 7212 0000 0029 0272 1100 0000  .N).r....).r....
+00000520: 7212 0000 0029 03da 0473 656c 6672 1800  r....)...selfr..
+00000530: 0000 7219 0000 0072 0e00 0000 720e 0000  ..r....r....r...
+00000540: 0072 0f00 0000 da11 7472 616e 736c 6174  .r......translat
+00000550: 655f 7265 7175 6573 741d 0000 0073 0200  e_request....s..
+00000560: 0000 0c01 7a23 4465 6d6f 5942 6164 416e  ....z#DemoYBadAn
+00000570: 6e6f 7461 746f 722e 7472 616e 736c 6174  notator.translat
+00000580: 655f 7265 7175 6573 74da 1261 6e6e 6f74  e_request..annot
+00000590: 6174 696f 6e5f 7265 7175 6573 74da 0672  ation_request..r
+000005a0: 6574 7572 6e63 0200 0000 0000 0000 0000  eturnc..........
+000005b0: 0000 0400 0000 0300 0000 4300 0000 732a  ..........C...s*
+000005c0: 0000 0064 017d 027c 016a 0044 005d 0a7d  ...d.}.|.j.D.].}
+000005d0: 037c 0364 0276 0072 0f7c 0264 0337 007d  .|.d.v.r.|.d.7.}
+000005e0: 0271 0574 017c 0264 048d 0153 0029 054e  .q.t.|.d...S.).N
+000005f0: 7201 0000 003e 0200 0000 da01 79da 0159  r....>......y..Y
+00000600: e901 0000 0029 0172 1600 0000 2902 7212  .....).r....).r.
+00000610: 0000 0072 1500 0000 2904 721b 0000 0072  ...r....).r....r
+00000620: 1d00 0000 7216 0000 00da 0963 6861 7261  ....r......chara
+00000630: 6374 6572 720e 0000 0072 0e00 0000 720f  cterr....r....r.
+00000640: 0000 00da 0861 6e6e 6f74 6174 6520 0000  .....annotate ..
+00000650: 0073 0c00 0000 0401 0a01 0801 0801 0280  .s..............
+00000660: 0a01 7a1a 4465 6d6f 5942 6164 416e 6e6f  ..z.DemoYBadAnno
+00000670: 7461 746f 722e 616e 6e6f 7461 7465 da08  tator.annotate..
+00000680: 7265 7370 6f6e 7365 6303 0000 0000 0000  responsec.......
+00000690: 0000 0000 0003 0000 0003 0000 0043 0000  .............C..
+000006a0: 0072 1a00 0000 2902 4e29 0172 0700 0000  .r....).N).r....
+000006b0: 2902 7206 0000 0072 1600 0000 2903 721b  ).r....r....).r.
+000006c0: 0000 00da 0772 6571 7565 7374 7224 0000  .....requestr$..
+000006d0: 0072 0e00 0000 720e 0000 0072 0f00 0000  .r....r....r....
+000006e0: da12 7472 616e 736c 6174 655f 7265 7370  ..translate_resp
+000006f0: 6f6e 7365 2700 0000 7302 0000 000c 037a  onse'...s......z
+00000700: 2444 656d 6f59 4261 6441 6e6e 6f74 6174  $DemoYBadAnnotat
+00000710: 6f72 2e74 7261 6e73 6c61 7465 5f72 6573  or.translate_res
+00000720: 706f 6e73 654e 290c 7208 0000 0072 0900  ponseN).r....r..
+00000730: 0000 720a 0000 0072 0b00 0000 7203 0000  ..r....r....r...
+00000740: 0072 0400 0000 721c 0000 0072 1100 0000  .r....r....r....
+00000750: 7215 0000 0072 2300 0000 7206 0000 0072  r....r#...r....r
+00000760: 2600 0000 720e 0000 0072 0e00 0000 720e  &...r....r....r.
+00000770: 0000 0072 0f00 0000 7217 0000 0015 0000  ...r....r.......
+00000780: 0073 1200 0000 0800 0401 1207 1203 0207  .s..............
+00000790: 0201 02ff 0202 0efe 7217 0000 004e 290c  ........r....N).
+000007a0: da14 6d6f 6465 6c67 6175 6765 2e61 6e6e  ..modelgauge.ann
+000007b0: 6f74 6174 6f72 7202 0000 00da 266d 6f64  otatorr.....&mod
+000007c0: 656c 6761 7567 652e 7369 6e67 6c65 5f74  elgauge.single_t
+000007d0: 7572 6e5f 7072 6f6d 7074 5f72 6573 706f  urn_prompt_respo
+000007e0: 6e73 6572 0300 0000 da0e 6d6f 6465 6c67  nser......modelg
+000007f0: 6175 6765 2e73 7574 7204 0000 00da 0870  auge.sutr......p
+00000800: 7964 616e 7469 6372 0500 0000 7206 0000  ydanticr....r...
+00000810: 0072 1100 0000 7215 0000 0072 1700 0000  .r....r....r....
+00000820: 720e 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
+00000830: 0f00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000840: 0000 7310 0000 000c 000c 010c 010c 0110  ..s.............
+00000850: 0310 0610 0418 04                        .......
```

### Comparing `modelgauge_demo_plugin-0.3.3/modelgauge/annotators/demo_annotator.py` & `modelgauge_demo_plugin-0.5.0/modelgauge/annotators/demo_annotator.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     score: float
 
 
 class DemoYBadAnnotator(CompletionAnnotator[DemoYBadAnnotation]):
     """A demonstration annotator that dislikes the letter Y.
 
     Real Annotators are intended to do expensive processing on the string,
-    such as calling another model collecting data from human raters. For
+    such as calling another model or collecting data from human raters. For
     the demo though, we want something cheap and deterministic.
     """
 
     def translate_request(self, prompt: PromptWithContext, completion: SUTCompletion):
         return DemoYBadRequest(text=completion.text)
 
     def annotate(self, annotation_request: DemoYBadRequest) -> DemoYBadResponse:
```

### Comparing `modelgauge_demo_plugin-0.3.3/modelgauge/suts/__pycache__/demo_01_yes_no_sut.cpython-310.pyc` & `modelgauge_demo_plugin-0.5.0/modelgauge/suts/__pycache__/demo_01_yes_no_sut.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `modelgauge_demo_plugin-0.3.3/modelgauge/suts/__pycache__/demo_02_secrets_and_options_sut.cpython-310.pyc` & `modelgauge_demo_plugin-0.5.0/modelgauge/suts/__pycache__/demo_02_secrets_and_options_sut.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `modelgauge_demo_plugin-0.3.3/modelgauge/suts/__pycache__/demo_03_sut_with_args.cpython-310.pyc` & `modelgauge_demo_plugin-0.5.0/modelgauge/suts/__pycache__/demo_03_sut_with_args.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `modelgauge_demo_plugin-0.3.3/modelgauge/suts/demo_01_yes_no_sut.py` & `modelgauge_demo_plugin-0.5.0/modelgauge/suts/demo_01_yes_no_sut.py`

 * *Files identical despite different names*

### Comparing `modelgauge_demo_plugin-0.3.3/modelgauge/suts/demo_02_secrets_and_options_sut.py` & `modelgauge_demo_plugin-0.5.0/modelgauge/suts/demo_02_secrets_and_options_sut.py`

 * *Files identical despite different names*

### Comparing `modelgauge_demo_plugin-0.3.3/modelgauge/suts/demo_03_sut_with_args.py` & `modelgauge_demo_plugin-0.5.0/modelgauge/suts/demo_03_sut_with_args.py`

 * *Files identical despite different names*

### Comparing `modelgauge_demo_plugin-0.3.3/modelgauge/tests/__pycache__/demo_01_simple_qa_test.cpython-310-pytest-7.4.4.pyc` & `modelgauge_demo_plugin-0.5.0/modelgauge/tests/__pycache__/demo_01_simple_qa_test.cpython-310-pytest-7.4.4.pyc`

 * *Files identical despite different names*

### Comparing `modelgauge_demo_plugin-0.3.3/modelgauge/tests/__pycache__/demo_01_simple_qa_test.cpython-310.pyc` & `modelgauge_demo_plugin-0.5.0/modelgauge/tests/__pycache__/demo_01_simple_qa_test.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `modelgauge_demo_plugin-0.3.3/modelgauge/tests/__pycache__/demo_02_unpacking_dependency_test.cpython-310-pytest-7.4.4.pyc` & `modelgauge_demo_plugin-0.5.0/modelgauge/tests/__pycache__/demo_02_unpacking_dependency_test.cpython-310-pytest-7.4.4.pyc`

 * *Files identical despite different names*

### Comparing `modelgauge_demo_plugin-0.3.3/modelgauge/tests/__pycache__/demo_02_unpacking_dependency_test.cpython-310.pyc` & `modelgauge_demo_plugin-0.5.0/modelgauge/tests/__pycache__/demo_02_unpacking_dependency_test.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `modelgauge_demo_plugin-0.3.3/modelgauge/tests/__pycache__/demo_03_paired_prompts_test.cpython-310-pytest-7.4.4.pyc` & `modelgauge_demo_plugin-0.5.0/modelgauge/tests/__pycache__/demo_03_paired_prompts_test.cpython-310-pytest-7.4.4.pyc`

 * *Files identical despite different names*

### Comparing `modelgauge_demo_plugin-0.3.3/modelgauge/tests/__pycache__/demo_03_paired_prompts_test.cpython-310.pyc` & `modelgauge_demo_plugin-0.5.0/modelgauge/tests/__pycache__/demo_03_paired_prompts_test.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `modelgauge_demo_plugin-0.3.3/modelgauge/tests/__pycache__/demo_04_using_annotation_test.cpython-310-pytest-7.4.4.pyc` & `modelgauge_demo_plugin-0.5.0/modelgauge/tests/__pycache__/demo_04_using_annotation_test.cpython-310-pytest-7.4.4.pyc`

 * *Files identical despite different names*

### Comparing `modelgauge_demo_plugin-0.3.3/modelgauge/tests/__pycache__/demo_04_using_annotation_test.cpython-310.pyc` & `modelgauge_demo_plugin-0.5.0/modelgauge/tests/__pycache__/demo_04_using_annotation_test.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `modelgauge_demo_plugin-0.3.3/modelgauge/tests/demo_01_simple_qa_test.py` & `modelgauge_demo_plugin-0.5.0/modelgauge/tests/demo_01_simple_qa_test.py`

 * *Files identical despite different names*

### Comparing `modelgauge_demo_plugin-0.3.3/modelgauge/tests/demo_02_unpacking_dependency_test.py` & `modelgauge_demo_plugin-0.5.0/modelgauge/tests/demo_02_unpacking_dependency_test.py`

 * *Files identical despite different names*

### Comparing `modelgauge_demo_plugin-0.3.3/modelgauge/tests/demo_03_paired_prompts_test.py` & `modelgauge_demo_plugin-0.5.0/modelgauge/tests/demo_03_paired_prompts_test.py`

 * *Files identical despite different names*

### Comparing `modelgauge_demo_plugin-0.3.3/modelgauge/tests/demo_04_using_annotation_test.py` & `modelgauge_demo_plugin-0.5.0/modelgauge/tests/demo_04_using_annotation_test.py`

 * *Files identical despite different names*

### Comparing `modelgauge_demo_plugin-0.3.3/PKG-INFO` & `modelgauge_demo_plugin-0.5.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelgauge-demo-plugin
-Version: 0.3.3
+Version: 0.5.0
 Summary: 
 Author: MLCommons AI Safety
 Author-email: ai-safety-engineering@mlcommons.org
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

