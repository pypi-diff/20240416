# Comparing `tmp/financial_datasets-0.1.6.tar.gz` & `tmp/financial_datasets-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "financial_datasets-0.1.6.tar", max compression
+gzip compressed data, was "financial_datasets-0.1.7.tar", max compression
```

## Comparing `financial_datasets-0.1.6.tar` & `financial_datasets-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2024-03-29 00:57:03.662287 financial_datasets-0.1.6/LICENSE
--rw-r--r--   0        0        0     4307 2024-04-10 12:21:55.239116 financial_datasets-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-03-29 00:57:47.261649 financial_datasets-0.1.6/financial_datasets/__init__.py
--rw-r--r--   0        0        0      201 2024-04-03 12:06:00.779549 financial_datasets-0.1.6/financial_datasets/dataset.py
--rw-r--r--   0        0        0      687 2024-04-07 22:00:07.915325 financial_datasets-0.1.6/financial_datasets/filings.py
--rw-r--r--   0        0        0     6616 2024-04-10 12:02:39.104303 financial_datasets-0.1.6/financial_datasets/generator.py
--rw-r--r--   0        0        0     1457 2024-04-10 12:02:30.195140 financial_datasets-0.1.6/financial_datasets/prompts.py
--rw-r--r--   0        0        0      660 2024-04-10 12:22:09.681746 financial_datasets-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     5200 1970-01-01 00:00:00.000000 financial_datasets-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-29 00:57:03.662287 financial_datasets-0.1.7/LICENSE
+-rw-r--r--   0        0        0     4090 2024-04-16 20:09:06.071968 financial_datasets-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-03-29 00:57:47.261649 financial_datasets-0.1.7/financial_datasets/__init__.py
+-rw-r--r--   0        0        0      201 2024-04-03 12:06:00.779549 financial_datasets-0.1.7/financial_datasets/dataset.py
+-rw-r--r--   0        0        0      687 2024-04-07 22:00:07.915325 financial_datasets-0.1.7/financial_datasets/filings.py
+-rw-r--r--   0        0        0     9496 2024-04-16 20:09:06.083652 financial_datasets-0.1.7/financial_datasets/generator.py
+-rw-r--r--   0        0        0     1457 2024-04-10 12:02:30.195140 financial_datasets-0.1.7/financial_datasets/prompts.py
+-rw-r--r--   0        0        0      660 2024-04-16 20:10:01.668688 financial_datasets-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4983 1970-01-01 00:00:00.000000 financial_datasets-0.1.7/PKG-INFO
```

### Comparing `financial_datasets-0.1.6/LICENSE` & `financial_datasets-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `financial_datasets-0.1.6/README.md` & `financial_datasets-0.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,252 +19,238 @@
 00000120: 616c 2074 6578 7473 2e0a 0a5b 215b 5477  al texts...[![Tw
 00000130: 6974 7465 7220 466f 6c6c 6f77 5d28 6874  itter Follow](ht
 00000140: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
 00000150: 732e 696f 2f74 7769 7474 6572 2f66 6f6c  s.io/twitter/fol
 00000160: 6c6f 772f 7669 7261 7474 743f 7374 796c  low/virattt?styl
 00000170: 653d 736f 6369 616c 295d 2868 7474 7073  e=social)](https
 00000180: 3a2f 2f74 7769 7474 6572 2e63 6f6d 2f76  ://twitter.com/v
-00000190: 6972 6174 7474 290a 0a23 2320 4665 6174  irattt)..## Feat
-000001a0: 7572 6573 0a0a 2d20 4765 6e65 7261 7465  ures..- Generate
-000001b0: 2073 796e 7468 6574 6963 2066 696e 616e   synthetic finan
-000001c0: 6369 616c 2064 6174 6173 6574 7320 7573  cial datasets us
-000001d0: 696e 6720 4c4c 4d73 0a2d 2053 7570 706f  ing LLMs.- Suppo
-000001e0: 7274 7320 7661 7269 6f75 7320 5345 4320  rts various SEC 
-000001f0: 6669 6c69 6e67 7320 2831 302d 4b73 2c20  filings (10-Ks, 
-00000200: 3130 2d51 732c 2065 7463 2e29 0a2d 2045  10-Qs, etc.).- E
-00000210: 6173 7920 696e 7465 6772 6174 696f 6e20  asy integration 
-00000220: 7769 7468 2050 7974 686f 6e20 7072 6f6a  with Python proj
-00000230: 6563 7473 0a2d 2043 7573 746f 6d69 7a61  ects.- Customiza
-00000240: 626c 6520 6461 7461 2067 656e 6572 6174  ble data generat
-00000250: 696f 6e20 6f70 7469 6f6e 730a 0a23 2320  ion options..## 
-00000260: 5573 6167 650a 0a2a 2a45 7861 6d70 6c65  Usage..**Example
-00000270: 2067 656e 6572 6174 6564 2064 6174 6173   generated datas
-00000280: 6574 3a2a 2a0a 6060 606a 736f 6e0a 5b0a  et:**.```json.[.
-00000290: 2020 7b0a 2020 2020 2271 7565 7374 696f    {.    "questio
-000002a0: 6e22 3a20 2257 6861 7420 7761 7320 4169  n": "What was Ai
-000002b0: 7262 6e62 2773 2072 6576 656e 7565 2069  rbnb's revenue i
-000002c0: 6e20 3230 3233 3f22 2c0a 2020 2020 2261  n 2023?",.    "a
-000002d0: 6e73 7765 7222 3a20 2224 392e 3920 6269  nswer": "$9.9 bi
-000002e0: 6c6c 696f 6e22 2c0a 2020 2020 2263 6f6e  llion",.    "con
-000002f0: 7465 7874 223a 2022 496e 2032 3032 332c  text": "In 2023,
-00000300: 2072 6576 656e 7565 2069 6e63 7265 6173   revenue increas
-00000310: 6564 2062 7920 3138 2520 746f 2024 392e  ed by 18% to $9.
-00000320: 3920 6269 6c6c 696f 6e20 636f 6d70 6172  9 billion compar
-00000330: 6564 2074 6f20 3230 3232 2c20 7072 696d  ed to 2022, prim
-00000340: 6172 696c 7920 6475 6520 746f 2061 2031  arily due to a 1
-00000350: 3425 2069 6e63 7265 6173 6520 696e 204e  4% increase in N
-00000360: 6967 6874 7320 616e 6420 4578 7065 7269  ights and Experi
-00000370: 656e 6365 7320 426f 6f6b 6564 206f 6620  ences Booked of 
-00000380: 3534 2e35 206d 696c 6c69 6f6e 2063 6f6d  54.5 million com
-00000390: 6269 6e65 6420 7769 7468 2068 6967 6865  bined with highe
-000003a0: 7220 6176 6572 6167 6520 6461 696c 7920  r average daily 
-000003b0: 7261 7465 7320 6472 6976 696e 6720 6120  rates driving a 
-000003c0: 3136 2520 696e 6372 6561 7365 2069 6e20  16% increase in 
-000003d0: 4772 6f73 7320 426f 6f6b 696e 6720 5661  Gross Booking Va
-000003e0: 6c75 6520 6f66 2024 3130 2e30 2062 696c  lue of $10.0 bil
-000003f0: 6c69 6f6e 2e22 0a20 207d 2c0a 2020 7b0a  lion.".  },.  {.
-00000400: 2020 2020 2271 7565 7374 696f 6e22 3a20      "question": 
-00000410: 2242 7920 7768 6174 2070 6572 6365 6e74  "By what percent
-00000420: 6167 6520 6469 6420 4169 7262 6e62 2773  age did Airbnb's
-00000430: 206e 6574 2069 6e63 6f6d 6520 696e 6372   net income incr
-00000440: 6561 7365 2069 6e20 3230 3233 2063 6f6d  ease in 2023 com
-00000450: 7061 7265 6420 746f 2074 6865 2070 7269  pared to the pri
-00000460: 6f72 2079 6561 723f 222c 0a20 2020 2022  or year?",.    "
-00000470: 616e 7377 6572 223a 2022 3135 3325 222c  answer": "153%",
-00000480: 0a20 2020 2022 636f 6e74 6578 7422 3a20  .    "context": 
-00000490: 224e 6574 2069 6e63 6f6d 6520 696e 2032  "Net income in 2
-000004a0: 3032 3320 696e 6372 6561 7365 6420 6279  023 increased by
-000004b0: 2031 3533 2520 746f 2024 342e 3820 6269   153% to $4.8 bi
-000004c0: 6c6c 696f 6e2c 2063 6f6d 7061 7265 6420  llion, compared 
-000004d0: 746f 2074 6865 2070 7269 6f72 2079 6561  to the prior yea
-000004e0: 722c 2064 7269 7665 6e20 6279 206f 7572  r, driven by our
-000004f0: 2072 6576 656e 7565 2067 726f 7774 682c   revenue growth,
-00000500: 2069 6e63 7265 6173 6564 2069 6e74 6572   increased inter
-00000510: 6573 7420 696e 636f 6d65 2c20 6469 7363  est income, disc
-00000520: 6970 6c69 6e65 2069 6e20 6d61 6e61 6769  ipline in managi
-00000530: 6e67 206f 7572 2063 6f73 7420 7374 7275  ng our cost stru
-00000540: 6374 7572 652c 2061 6e64 2074 6865 2072  cture, and the r
-00000550: 656c 6561 7365 206f 6620 6120 706f 7274  elease of a port
-00000560: 696f 6e20 6f66 206f 7572 2076 616c 7561  ion of our valua
-00000570: 7469 6f6e 2061 6c6c 6f77 616e 6365 206f  tion allowance o
-00000580: 6e20 6465 6665 7272 6564 2074 6178 2061  n deferred tax a
-00000590: 7373 6574 7320 6f66 2024 322e 3920 6269  ssets of $2.9 bi
-000005a0: 6c6c 696f 6e2e 220a 2020 7d0a 5d0a 6060  llion.".  }.].``
-000005b0: 600a 0a2a 2a45 7861 6d70 6c65 2023 3120  `..**Example #1 
-000005c0: 2d20 6765 6e65 7261 7465 2066 726f 6d20  - generate from 
-000005d0: 616e 7920 7465 7874 733a 2a2a 0a0a 4d6f  any texts:**..Mo
-000005e0: 7374 2066 6c65 7869 626c 6520 6f70 7469  st flexible opti
-000005f0: 6f6e 2e20 2047 656e 6572 6174 6573 2064  on.  Generates d
-00000600: 6174 6173 6574 2075 7369 6e67 2061 206c  ataset using a l
-00000610: 6973 7420 6f66 2073 7472 696e 6720 6074  ist of string `t
-00000620: 6578 7473 602e 2043 6f6c 6162 2063 6f64  exts`. Colab cod
-00000630: 6520 6578 616d 706c 6520 5b68 6572 655d  e example [here]
-00000640: 2868 7474 7073 3a2f 2f63 6f6c 6162 2e72  (https://colab.r
-00000650: 6573 6561 7263 682e 676f 6f67 6c65 2e63  esearch.google.c
-00000660: 6f6d 2f67 6973 742f 7669 7261 7474 742f  om/gist/virattt/
-00000670: 6639 6235 6130 6165 3832 6363 3063 6161  f9b5a0ae82cc0caa
-00000680: 6235 3764 6635 6465 6463 3239 3237 6339  b57df5dedc2927c9
-00000690: 2f69 6e74 726f 2d66 696e 616e 6369 616c  /intro-financial
-000006a0: 2d64 6174 6173 6574 732e 6970 796e 6229  -datasets.ipynb)
-000006b0: 2e0a 0a60 6060 7079 7468 6f6e 0a66 726f  ...```python.fro
-000006c0: 6d20 6669 6e61 6e63 6961 6c5f 6461 7461  m financial_data
-000006d0: 7365 7473 2e67 656e 6572 6174 6f72 2069  sets.generator i
-000006e0: 6d70 6f72 7420 4461 7461 7365 7447 656e  mport DatasetGen
-000006f0: 6572 6174 6f72 0a0a 7465 7874 7320 3d20  erator..texts = 
-00000700: 2e2e 2e20 2023 204c 6973 7420 6f66 2074  ...  # List of t
-00000710: 6578 7473 2066 726f 6d20 5345 4320 6669  exts from SEC fi
-00000720: 6c69 6e67 0a67 656e 6572 6174 6f72 203d  ling.generator =
-00000730: 2044 6174 6173 6574 4765 6e65 7261 746f   DatasetGenerato
-00000740: 7228 6d6f 6465 6c3d 2267 7074 2d34 2d30  r(model="gpt-4-0
-00000750: 3132 352d 7072 6576 6965 7722 2c20 6170  125-preview", ap
-00000760: 695f 6b65 793d 2279 6f75 722d 6f70 656e  i_key="your-open
-00000770: 6169 2d6b 6579 2229 0a0a 2320 4765 6e65  ai-key")..# Gene
-00000780: 7261 7465 2064 6174 6173 6574 2066 726f  rate dataset fro
-00000790: 6d20 7465 7874 730a 6461 7461 7365 7420  m texts.dataset 
-000007a0: 3d20 6765 6e65 7261 746f 722e 6765 6e65  = generator.gene
-000007b0: 7261 7465 5f66 726f 6d5f 7465 7874 7328  rate_from_texts(
-000007c0: 0a20 2020 7465 7874 733d 7465 7874 732c  .   texts=texts,
-000007d0: 200a 2020 206d 6178 5f71 7565 7374 696f   .   max_questio
-000007e0: 6e73 3d31 3030 2c0a 290a 6060 600a 0a2a  ns=100,.).```..*
-000007f0: 2a45 7861 6d70 6c65 2023 3220 2d20 6765  *Example #2 - ge
-00000800: 6e65 7261 7465 2066 726f 6d20 3130 2d4b  nerate from 10-K
-00000810: 3a2a 2a0a 0a47 656e 6572 6174 6520 6120  :**..Generate a 
-00000820: 6461 7461 7365 7420 7573 696e 6720 6120  dataset using a 
-00000830: 6074 6963 6b65 7260 2061 6e64 2060 7965  `ticker` and `ye
-00000840: 6172 602e 2020 436f 6c61 6220 636f 6465  ar`.  Colab code
-00000850: 2065 7861 6d70 6c65 205b 6865 7265 5d28   example [here](
-00000860: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
-00000870: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
-00000880: 6d2f 6769 7374 2f76 6972 6174 7474 2f37  m/gist/virattt/7
-00000890: 3433 3837 3265 3134 3330 3334 3938 3764  43872e143034987d
-000008a0: 3230 6536 6136 6337 6262 3964 3061 312f  20e6a6c7bb9d0a1/
-000008b0: 696e 7472 6f2d 6669 6e61 6e63 6961 6c2d  intro-financial-
-000008c0: 6461 7461 7365 7473 2e69 7079 6e62 292e  datasets.ipynb).
-000008d0: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
-000008e0: 2066 696e 616e 6369 616c 5f64 6174 6173   financial_datas
-000008f0: 6574 732e 6765 6e65 7261 746f 7220 696d  ets.generator im
-00000900: 706f 7274 2044 6174 6173 6574 4765 6e65  port DatasetGene
-00000910: 7261 746f 720a 0a74 6578 7473 203d 202e  rator..texts = .
-00000920: 2e2e 2020 2320 4c69 7374 206f 6620 7465  ..  # List of te
-00000930: 7874 7320 6672 6f6d 2053 4543 2066 696c  xts from SEC fil
-00000940: 696e 670a 6765 6e65 7261 746f 7220 3d20  ing.generator = 
-00000950: 4461 7461 7365 7447 656e 6572 6174 6f72  DatasetGenerator
-00000960: 286d 6f64 656c 3d22 6770 742d 342d 3031  (model="gpt-4-01
-00000970: 3235 2d70 7265 7669 6577 222c 2061 7069  25-preview", api
-00000980: 5f6b 6579 3d22 796f 7572 2d6f 7065 6e61  _key="your-opena
-00000990: 692d 6b65 7922 290a 0a23 2047 656e 6572  i-key")..# Gener
-000009a0: 6174 6520 6461 7461 7365 7420 6672 6f6d  ate dataset from
-000009b0: 2031 302d 4b0a 6461 7461 7365 7420 3d20   10-K.dataset = 
-000009c0: 6765 6e65 7261 746f 722e 6765 6e65 7261  generator.genera
-000009d0: 7465 5f66 726f 6d5f 3130 4b28 0a20 2020  te_from_10K(.   
-000009e0: 7469 636b 6572 3d22 4141 504c 222c 0a20  ticker="AAPL",. 
-000009f0: 2020 7965 6172 3d32 3032 332c 0a20 2020    year=2023,.   
-00000a00: 6d61 785f 7175 6573 7469 6f6e 733d 3130  max_questions=10
-00000a10: 302c 0a29 0a60 6060 0a0a 2a2a 4578 616d  0,.).```..**Exam
-00000a20: 706c 6520 2333 202d 2067 656e 6572 6174  ple #3 - generat
-00000a30: 6520 6672 6f6d 2050 4446 3a2a 2a0a 0a47  e from PDF:**..G
-00000a40: 656e 6572 6174 6520 6120 6461 7461 7365  enerate a datase
-00000a50: 7420 7573 696e 6720 6120 5044 4620 6075  t using a PDF `u
-00000a60: 726c 6020 6f6e 6c79 2e20 2043 6f6c 6162  rl` only.  Colab
-00000a70: 2063 6f64 6520 6578 616d 706c 6520 5b68   code example [h
-00000a80: 6572 655d 2868 7474 7073 3a2f 2f63 6f6c  ere](https://col
-00000a90: 6162 2e72 6573 6561 7263 682e 676f 6f67  ab.research.goog
-00000aa0: 6c65 2e63 6f6d 2f67 6973 742f 7669 7261  le.com/gist/vira
-00000ab0: 7474 742f 6230 3434 3432 6565 3763 3663  ttt/b04442ee7c6c
-00000ac0: 3064 3062 6233 6339 3337 3161 6632 3238  0d0bb3c9371af228
-00000ad0: 3361 3230 2f69 6e74 726f 2d66 696e 616e  3a20/intro-finan
-00000ae0: 6369 616c 2d64 6174 6173 6574 732e 6970  cial-datasets.ip
-00000af0: 796e 6229 2e0a 0a60 6060 7079 7468 6f6e  ynb)...```python
-00000b00: 0a66 726f 6d20 6669 6e61 6e63 6961 6c5f  .from financial_
-00000b10: 6461 7461 7365 7473 2e67 656e 6572 6174  datasets.generat
-00000b20: 6f72 2069 6d70 6f72 7420 4461 7461 7365  or import Datase
-00000b30: 7447 656e 6572 6174 6f72 0a0a 7465 7874  tGenerator..text
-00000b40: 7320 3d20 2e2e 2e20 2023 204c 6973 7420  s = ...  # List 
-00000b50: 6f66 2074 6578 7473 2066 726f 6d20 5345  of texts from SE
-00000b60: 4320 6669 6c69 6e67 0a67 656e 6572 6174  C filing.generat
-00000b70: 6f72 203d 2044 6174 6173 6574 4765 6e65  or = DatasetGene
-00000b80: 7261 746f 7228 6d6f 6465 6c3d 2267 7074  rator(model="gpt
-00000b90: 2d34 2d30 3132 352d 7072 6576 6965 7722  -4-0125-preview"
-00000ba0: 2c20 6170 695f 6b65 793d 2279 6f75 722d  , api_key="your-
-00000bb0: 6f70 656e 6169 2d6b 6579 2229 0a0a 2320  openai-key")..# 
-00000bc0: 4765 6e65 7261 7465 2064 6174 6173 6574  Generate dataset
-00000bd0: 2066 726f 6d20 5044 4620 7572 6c0a 6461   from PDF url.da
-00000be0: 7461 7365 7420 3d20 6765 6e65 7261 746f  taset = generato
-00000bf0: 722e 6765 6e65 7261 7465 5f66 726f 6d5f  r.generate_from_
-00000c00: 7064 6628 0a20 2020 7572 6c3d 2268 7474  pdf(.   url="htt
-00000c10: 7073 3a2f 2f77 7777 2e62 6572 6b73 6869  ps://www.berkshi
-00000c20: 7265 6861 7468 6177 6179 2e63 6f6d 2f6c  rehathaway.com/l
-00000c30: 6574 7465 7273 2f32 3032 336c 7472 2e70  etters/2023ltr.p
-00000c40: 6466 222c 0a20 2020 6d61 785f 7175 6573  df",.   max_ques
-00000c50: 7469 6f6e 733d 3130 302c 0a29 0a60 6060  tions=100,.).```
-00000c60: 0a0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
-00000c70: 6e0a 0a23 2323 2055 7369 6e67 2070 6970  n..### Using pip
-00000c80: 0a0a 596f 7520 6361 6e20 696e 7374 616c  ..You can instal
-00000c90: 6c20 7468 6520 4669 6e61 6e63 6961 6c20  l the Financial 
-00000ca0: 4461 7461 7365 7473 206c 6962 7261 7279  Datasets library
-00000cb0: 2075 7369 6e67 2070 6970 3a0a 0a60 6060   using pip:..```
-00000cc0: 0a70 6970 2069 6e73 7461 6c6c 2066 696e  .pip install fin
-00000cd0: 616e 6369 616c 2d64 6174 6173 6574 730a  ancial-datasets.
-00000ce0: 6060 600a 0a23 2323 2055 7369 6e67 2050  ```..### Using P
-00000cf0: 6f65 7472 790a 0a49 6620 796f 7520 7072  oetry..If you pr
-00000d00: 6566 6572 2074 6f20 7573 6520 506f 6574  efer to use Poet
-00000d10: 7279 2066 6f72 2064 6570 656e 6465 6e63  ry for dependenc
-00000d20: 7920 6d61 6e61 6765 6d65 6e74 2c20 796f  y management, yo
-00000d30: 7520 6361 6e20 6164 6420 4669 6e61 6e63  u can add Financ
-00000d40: 6961 6c20 4461 7461 7365 7473 2074 6f20  ial Datasets to 
-00000d50: 796f 7572 2070 726f 6a65 6374 3a0a 0a60  your project:..`
-00000d60: 6060 0a70 6f65 7472 7920 6164 6420 6669  ``.poetry add fi
-00000d70: 6e61 6e63 6961 6c2d 6461 7461 7365 7473  nancial-datasets
-00000d80: 0a60 6060 0a0a 2323 2320 4672 6f6d 2074  .```..### From t
-00000d90: 6865 2052 6570 6f73 6974 6f72 790a 0a49  he Repository..I
-00000da0: 6620 796f 7520 7761 6e74 2074 6f20 696e  f you want to in
-00000db0: 7374 616c 6c20 7468 6520 6c69 6272 6172  stall the librar
-00000dc0: 7920 6469 7265 6374 6c79 2066 726f 6d20  y directly from 
-00000dd0: 7468 6520 7265 706f 7369 746f 7279 2c20  the repository, 
-00000de0: 666f 6c6c 6f77 2074 6865 7365 2073 7465  follow these ste
-00000df0: 7073 3a0a 0a31 2e20 436c 6f6e 6520 7468  ps:..1. Clone th
-00000e00: 6520 7265 706f 7369 746f 7279 3a0a 2020  e repository:.  
-00000e10: 2060 6060 0a20 2020 6769 7420 636c 6f6e   ```.   git clon
-00000e20: 6520 6874 7470 733a 2f2f 6769 7468 7562  e https://github
-00000e30: 2e63 6f6d 2f79 6f75 7275 7365 726e 616d  .com/yourusernam
-00000e40: 652f 6669 6e61 6e63 6961 6c2d 6461 7461  e/financial-data
-00000e50: 7365 7473 2e67 6974 0a20 2020 6060 600a  sets.git.   ```.
-00000e60: 0a32 2e20 4e61 7669 6761 7465 2074 6f20  .2. Navigate to 
-00000e70: 7468 6520 7072 6f6a 6563 7420 6469 7265  the project dire
-00000e80: 6374 6f72 793a 0a20 2020 6060 600a 2020  ctory:.   ```.  
-00000e90: 2063 6420 6669 6e61 6e63 6961 6c2d 6461   cd financial-da
-00000ea0: 7461 7365 7473 0a20 2020 6060 600a 2020  tasets.   ```.  
-00000eb0: 200a 332e 2049 6e73 7461 6c6c 2074 6865   .3. Install the
-00000ec0: 2064 6570 656e 6465 6e63 6965 7320 7573   dependencies us
-00000ed0: 696e 6720 506f 6574 7279 3a0a 2020 2060  ing Poetry:.   `
-00000ee0: 6060 0a20 2020 706f 6574 7279 2069 6e73  ``.   poetry ins
-00000ef0: 7461 6c6c 0a20 2020 6060 600a 0a34 2e20  tall.   ```..4. 
-00000f00: 596f 7520 6361 6e20 6e6f 7720 7573 6520  You can now use 
-00000f10: 7468 6520 6c69 6272 6172 7920 696e 2079  the library in y
-00000f20: 6f75 7220 5079 7468 6f6e 2070 726f 6a65  our Python proje
-00000f30: 6374 732e 0a0a 2323 2043 6f6e 7472 6962  cts...## Contrib
-00000f40: 7574 696e 670a 0a43 6f6e 7472 6962 7574  uting..Contribut
-00000f50: 696f 6e73 2061 7265 2077 656c 636f 6d65  ions are welcome
-00000f60: 2120 4966 2079 6f75 2066 696e 6420 616e  ! If you find an
-00000f70: 7920 6973 7375 6573 206f 7220 6861 7665  y issues or have
-00000f80: 2073 7567 6765 7374 696f 6e73 2066 6f72   suggestions for
-00000f90: 2069 6d70 726f 7665 6d65 6e74 732c 200a   improvements, .
-00000fa0: 706c 6561 7365 206f 7065 6e20 616e 2069  please open an i
-00000fb0: 7373 7565 206f 7220 7375 626d 6974 2061  ssue or submit a
-00000fc0: 2070 756c 6c20 7265 7175 6573 742e 0a0a   pull request...
-00000fd0: 2323 204c 6963 656e 7365 0a0a 5468 6973  ## License..This
-00000fe0: 2070 726f 6a65 6374 2069 7320 6c69 6365   project is lice
-00000ff0: 6e73 6564 2075 6e64 6572 2074 6865 205b  nsed under the [
-00001000: 4d49 5420 4c69 6365 6e73 655d 286c 696e  MIT License](lin
-00001010: 6b2d 746f 2d6c 6963 656e 7365 2d66 696c  k-to-license-fil
-00001020: 6529 2e0a 0a23 2320 436f 6e74 7269 6275  e)...## Contribu
-00001030: 746f 7273 0a0a 3c61 2068 7265 663d 2268  tors..<a href="h
-00001040: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001050: 6d2f 7669 7261 7474 742f 6669 6e61 6e63  m/virattt/financ
-00001060: 6961 6c2d 6461 7461 7365 7473 2f67 7261  ial-datasets/gra
-00001070: 7068 732f 636f 6e74 7269 6275 746f 7273  phs/contributors
-00001080: 223e 0a20 203c 696d 6720 7372 633d 2268  ">.  <img src="h
-00001090: 7474 7073 3a2f 2f63 6f6e 7472 6962 2e72  ttps://contrib.r
-000010a0: 6f63 6b73 2f69 6d61 6765 3f72 6570 6f3d  ocks/image?repo=
-000010b0: 7669 7261 7474 742f 6669 6e61 6e63 6961  virattt/financia
-000010c0: 6c2d 6461 7461 7365 7473 2220 2f3e 0a3c  l-datasets" />.<
-000010d0: 2f61 3e                                  /a>
+00000190: 6972 6174 7474 290a 0a23 2320 5573 6167  irattt)..## Usag
+000001a0: 650a 0a2a 2a45 7861 6d70 6c65 2067 656e  e..**Example gen
+000001b0: 6572 6174 6564 2064 6174 6173 6574 3a2a  erated dataset:*
+000001c0: 2a0a 6060 606a 736f 6e0a 5b0a 2020 7b0a  *.```json.[.  {.
+000001d0: 2020 2020 2271 7565 7374 696f 6e22 3a20      "question": 
+000001e0: 2257 6861 7420 7761 7320 4169 7262 6e62  "What was Airbnb
+000001f0: 2773 2072 6576 656e 7565 2069 6e20 3230  's revenue in 20
+00000200: 3233 3f22 2c0a 2020 2020 2261 6e73 7765  23?",.    "answe
+00000210: 7222 3a20 2224 392e 3920 6269 6c6c 696f  r": "$9.9 billio
+00000220: 6e22 2c0a 2020 2020 2263 6f6e 7465 7874  n",.    "context
+00000230: 223a 2022 496e 2032 3032 332c 2072 6576  ": "In 2023, rev
+00000240: 656e 7565 2069 6e63 7265 6173 6564 2062  enue increased b
+00000250: 7920 3138 2520 746f 2024 392e 3920 6269  y 18% to $9.9 bi
+00000260: 6c6c 696f 6e20 636f 6d70 6172 6564 2074  llion compared t
+00000270: 6f20 3230 3232 2c20 7072 696d 6172 696c  o 2022, primaril
+00000280: 7920 6475 6520 746f 2061 2031 3425 2069  y due to a 14% i
+00000290: 6e63 7265 6173 6520 696e 204e 6967 6874  ncrease in Night
+000002a0: 7320 616e 6420 4578 7065 7269 656e 6365  s and Experience
+000002b0: 7320 426f 6f6b 6564 206f 6620 3534 2e35  s Booked of 54.5
+000002c0: 206d 696c 6c69 6f6e 2063 6f6d 6269 6e65   million combine
+000002d0: 6420 7769 7468 2068 6967 6865 7220 6176  d with higher av
+000002e0: 6572 6167 6520 6461 696c 7920 7261 7465  erage daily rate
+000002f0: 7320 6472 6976 696e 6720 6120 3136 2520  s driving a 16% 
+00000300: 696e 6372 6561 7365 2069 6e20 4772 6f73  increase in Gros
+00000310: 7320 426f 6f6b 696e 6720 5661 6c75 6520  s Booking Value 
+00000320: 6f66 2024 3130 2e30 2062 696c 6c69 6f6e  of $10.0 billion
+00000330: 2e22 0a20 207d 2c0a 2020 7b0a 2020 2020  .".  },.  {.    
+00000340: 2271 7565 7374 696f 6e22 3a20 2242 7920  "question": "By 
+00000350: 7768 6174 2070 6572 6365 6e74 6167 6520  what percentage 
+00000360: 6469 6420 4169 7262 6e62 2773 206e 6574  did Airbnb's net
+00000370: 2069 6e63 6f6d 6520 696e 6372 6561 7365   income increase
+00000380: 2069 6e20 3230 3233 2063 6f6d 7061 7265   in 2023 compare
+00000390: 6420 746f 2074 6865 2070 7269 6f72 2079  d to the prior y
+000003a0: 6561 723f 222c 0a20 2020 2022 616e 7377  ear?",.    "answ
+000003b0: 6572 223a 2022 3135 3325 222c 0a20 2020  er": "153%",.   
+000003c0: 2022 636f 6e74 6578 7422 3a20 224e 6574   "context": "Net
+000003d0: 2069 6e63 6f6d 6520 696e 2032 3032 3320   income in 2023 
+000003e0: 696e 6372 6561 7365 6420 6279 2031 3533  increased by 153
+000003f0: 2520 746f 2024 342e 3820 6269 6c6c 696f  % to $4.8 billio
+00000400: 6e2c 2063 6f6d 7061 7265 6420 746f 2074  n, compared to t
+00000410: 6865 2070 7269 6f72 2079 6561 722c 2064  he prior year, d
+00000420: 7269 7665 6e20 6279 206f 7572 2072 6576  riven by our rev
+00000430: 656e 7565 2067 726f 7774 682c 2069 6e63  enue growth, inc
+00000440: 7265 6173 6564 2069 6e74 6572 6573 7420  reased interest 
+00000450: 696e 636f 6d65 2c20 6469 7363 6970 6c69  income, discipli
+00000460: 6e65 2069 6e20 6d61 6e61 6769 6e67 206f  ne in managing o
+00000470: 7572 2063 6f73 7420 7374 7275 6374 7572  ur cost structur
+00000480: 652c 2061 6e64 2074 6865 2072 656c 6561  e, and the relea
+00000490: 7365 206f 6620 6120 706f 7274 696f 6e20  se of a portion 
+000004a0: 6f66 206f 7572 2076 616c 7561 7469 6f6e  of our valuation
+000004b0: 2061 6c6c 6f77 616e 6365 206f 6e20 6465   allowance on de
+000004c0: 6665 7272 6564 2074 6178 2061 7373 6574  ferred tax asset
+000004d0: 7320 6f66 2024 322e 3920 6269 6c6c 696f  s of $2.9 billio
+000004e0: 6e2e 220a 2020 7d0a 5d0a 6060 600a 0a2a  n.".  }.].```..*
+000004f0: 2a45 7861 6d70 6c65 2023 3120 2d20 6765  *Example #1 - ge
+00000500: 6e65 7261 7465 2066 726f 6d20 616e 7920  nerate from any 
+00000510: 7465 7874 2a2a 0a0a 4d6f 7374 2066 6c65  text**..Most fle
+00000520: 7869 626c 6520 6f70 7469 6f6e 2e20 2047  xible option.  G
+00000530: 656e 6572 6174 6573 2064 6174 6173 6574  enerates dataset
+00000540: 2075 7369 6e67 2061 206c 6973 7420 6f66   using a list of
+00000550: 2073 7472 696e 6720 6074 6578 7473 602e   string `texts`.
+00000560: 2043 6f6c 6162 2063 6f64 6520 6578 616d   Colab code exam
+00000570: 706c 6520 5b68 6572 655d 2868 7474 7073  ple [here](https
+00000580: 3a2f 2f63 6f6c 6162 2e72 6573 6561 7263  ://colab.researc
+00000590: 682e 676f 6f67 6c65 2e63 6f6d 2f67 6973  h.google.com/gis
+000005a0: 742f 7669 7261 7474 742f 6639 6235 6130  t/virattt/f9b5a0
+000005b0: 6165 3832 6363 3063 6161 6235 3764 6635  ae82cc0caab57df5
+000005c0: 6465 6463 3239 3237 6339 2f69 6e74 726f  dedc2927c9/intro
+000005d0: 2d66 696e 616e 6369 616c 2d64 6174 6173  -financial-datas
+000005e0: 6574 732e 6970 796e 6229 2e0a 0a60 6060  ets.ipynb)...```
+000005f0: 7079 7468 6f6e 0a66 726f 6d20 6669 6e61  python.from fina
+00000600: 6e63 6961 6c5f 6461 7461 7365 7473 2e67  ncial_datasets.g
+00000610: 656e 6572 6174 6f72 2069 6d70 6f72 7420  enerator import 
+00000620: 4461 7461 7365 7447 656e 6572 6174 6f72  DatasetGenerator
+00000630: 0a0a 2320 596f 7572 206c 6973 7420 6f66  ..# Your list of
+00000640: 2074 6578 7473 0a74 6578 7473 203d 202e   texts.texts = .
+00000650: 2e2e 2020 0a0a 2320 4372 6561 7465 2064  ..  ..# Create d
+00000660: 6174 6173 6574 2067 656e 6572 6174 6f72  ataset generator
+00000670: 0a67 656e 6572 6174 6f72 203d 2044 6174  .generator = Dat
+00000680: 6173 6574 4765 6e65 7261 746f 7228 6d6f  asetGenerator(mo
+00000690: 6465 6c3d 2267 7074 2d34 2d30 3132 352d  del="gpt-4-0125-
+000006a0: 7072 6576 6965 7722 2c20 6170 695f 6b65  preview", api_ke
+000006b0: 793d 2279 6f75 722d 6f70 656e 6169 2d6b  y="your-openai-k
+000006c0: 6579 2229 0a0a 2320 4765 6e65 7261 7465  ey")..# Generate
+000006d0: 2064 6174 6173 6574 2066 726f 6d20 7465   dataset from te
+000006e0: 7874 730a 6461 7461 7365 7420 3d20 6765  xts.dataset = ge
+000006f0: 6e65 7261 746f 722e 6765 6e65 7261 7465  nerator.generate
+00000700: 5f66 726f 6d5f 7465 7874 7328 0a20 2020  _from_texts(.   
+00000710: 7465 7874 733d 7465 7874 732c 200a 2020  texts=texts, .  
+00000720: 206d 6178 5f71 7565 7374 696f 6e73 3d31   max_questions=1
+00000730: 3030 2c0a 290a 6060 600a 0a2a 2a45 7861  00,.).```..**Exa
+00000740: 6d70 6c65 2023 3220 2d20 6765 6e65 7261  mple #2 - genera
+00000750: 7465 2066 726f 6d20 3130 2d4b 2a2a 0a0a  te from 10-K**..
+00000760: 4765 6e65 7261 7465 2061 2064 6174 6173  Generate a datas
+00000770: 6574 2075 7369 6e67 2061 2060 7469 636b  et using a `tick
+00000780: 6572 6020 616e 6420 6079 6561 7260 2e20  er` and `year`. 
+00000790: 2043 6f6c 6162 2063 6f64 6520 6578 616d   Colab code exam
+000007a0: 706c 6520 5b68 6572 655d 2868 7474 7073  ple [here](https
+000007b0: 3a2f 2f63 6f6c 6162 2e72 6573 6561 7263  ://colab.researc
+000007c0: 682e 676f 6f67 6c65 2e63 6f6d 2f67 6973  h.google.com/gis
+000007d0: 742f 7669 7261 7474 742f 3734 3338 3732  t/virattt/743872
+000007e0: 6531 3433 3033 3439 3837 6432 3065 3661  e143034987d20e6a
+000007f0: 3663 3762 6239 6430 6131 2f69 6e74 726f  6c7bb9d0a1/intro
+00000800: 2d66 696e 616e 6369 616c 2d64 6174 6173  -financial-datas
+00000810: 6574 732e 6970 796e 6229 2e0a 0a60 6060  ets.ipynb)...```
+00000820: 7079 7468 6f6e 0a66 726f 6d20 6669 6e61  python.from fina
+00000830: 6e63 6961 6c5f 6461 7461 7365 7473 2e67  ncial_datasets.g
+00000840: 656e 6572 6174 6f72 2069 6d70 6f72 7420  enerator import 
+00000850: 4461 7461 7365 7447 656e 6572 6174 6f72  DatasetGenerator
+00000860: 0a0a 2320 4372 6561 7465 2064 6174 6173  ..# Create datas
+00000870: 6574 2067 656e 6572 6174 6f72 0a67 656e  et generator.gen
+00000880: 6572 6174 6f72 203d 2044 6174 6173 6574  erator = Dataset
+00000890: 4765 6e65 7261 746f 7228 6d6f 6465 6c3d  Generator(model=
+000008a0: 2267 7074 2d34 2d30 3132 352d 7072 6576  "gpt-4-0125-prev
+000008b0: 6965 7722 2c20 6170 695f 6b65 793d 2279  iew", api_key="y
+000008c0: 6f75 722d 6f70 656e 6169 2d6b 6579 2229  our-openai-key")
+000008d0: 0a0a 2320 4765 6e65 7261 7465 2064 6174  ..# Generate dat
+000008e0: 6173 6574 2066 726f 6d20 3130 2d4b 0a64  aset from 10-K.d
+000008f0: 6174 6173 6574 203d 2067 656e 6572 6174  ataset = generat
+00000900: 6f72 2e67 656e 6572 6174 655f 6672 6f6d  or.generate_from
+00000910: 5f31 304b 280a 2020 2074 6963 6b65 723d  _10K(.   ticker=
+00000920: 2241 4150 4c22 2c0a 2020 2079 6561 723d  "AAPL",.   year=
+00000930: 3230 3233 2c0a 2020 206d 6178 5f71 7565  2023,.   max_que
+00000940: 7374 696f 6e73 3d31 3030 2c0a 290a 6060  stions=100,.).``
+00000950: 600a 0a2a 2a45 7861 6d70 6c65 2023 3320  `..**Example #3 
+00000960: 2d20 6765 6e65 7261 7465 2066 726f 6d20  - generate from 
+00000970: 5044 462a 2a0a 0a47 656e 6572 6174 6520  PDF**..Generate 
+00000980: 6120 6461 7461 7365 7420 7573 696e 6720  a dataset using 
+00000990: 6120 5044 4620 6075 726c 6020 6f6e 6c79  a PDF `url` only
+000009a0: 2e20 2043 6f6c 6162 2063 6f64 6520 6578  .  Colab code ex
+000009b0: 616d 706c 6520 5b68 6572 655d 2868 7474  ample [here](htt
+000009c0: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
+000009d0: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f67  rch.google.com/g
+000009e0: 6973 742f 7669 7261 7474 742f 6230 3434  ist/virattt/b044
+000009f0: 3432 6565 3763 3663 3064 3062 6233 6339  42ee7c6c0d0bb3c9
+00000a00: 3337 3161 6632 3238 3361 3230 2f69 6e74  371af2283a20/int
+00000a10: 726f 2d66 696e 616e 6369 616c 2d64 6174  ro-financial-dat
+00000a20: 6173 6574 732e 6970 796e 6229 2e0a 0a60  asets.ipynb)...`
+00000a30: 6060 7079 7468 6f6e 0a66 726f 6d20 6669  ``python.from fi
+00000a40: 6e61 6e63 6961 6c5f 6461 7461 7365 7473  nancial_datasets
+00000a50: 2e67 656e 6572 6174 6f72 2069 6d70 6f72  .generator impor
+00000a60: 7420 4461 7461 7365 7447 656e 6572 6174  t DatasetGenerat
+00000a70: 6f72 0a0a 2320 4372 6561 7465 2064 6174  or..# Create dat
+00000a80: 6173 6574 2067 656e 6572 6174 6f72 0a67  aset generator.g
+00000a90: 656e 6572 6174 6f72 203d 2044 6174 6173  enerator = Datas
+00000aa0: 6574 4765 6e65 7261 746f 7228 6d6f 6465  etGenerator(mode
+00000ab0: 6c3d 2267 7074 2d34 2d30 3132 352d 7072  l="gpt-4-0125-pr
+00000ac0: 6576 6965 7722 2c20 6170 695f 6b65 793d  eview", api_key=
+00000ad0: 2279 6f75 722d 6f70 656e 6169 2d6b 6579  "your-openai-key
+00000ae0: 2229 0a0a 2320 4765 6e65 7261 7465 2064  ")..# Generate d
+00000af0: 6174 6173 6574 2066 726f 6d20 5044 4620  ataset from PDF 
+00000b00: 7572 6c0a 6461 7461 7365 7420 3d20 6765  url.dataset = ge
+00000b10: 6e65 7261 746f 722e 6765 6e65 7261 7465  nerator.generate
+00000b20: 5f66 726f 6d5f 7064 6628 0a20 2020 7572  _from_pdf(.   ur
+00000b30: 6c3d 2268 7474 7073 3a2f 2f77 7777 2e62  l="https://www.b
+00000b40: 6572 6b73 6869 7265 6861 7468 6177 6179  erkshirehathaway
+00000b50: 2e63 6f6d 2f6c 6574 7465 7273 2f32 3032  .com/letters/202
+00000b60: 336c 7472 2e70 6466 222c 0a20 2020 6d61  3ltr.pdf",.   ma
+00000b70: 785f 7175 6573 7469 6f6e 733d 3130 302c  x_questions=100,
+00000b80: 0a29 0a60 6060 0a0a 2323 2049 6e73 7461  .).```..## Insta
+00000b90: 6c6c 6174 696f 6e0a 0a23 2323 2055 7369  llation..### Usi
+00000ba0: 6e67 2070 6970 0a0a 596f 7520 6361 6e20  ng pip..You can 
+00000bb0: 696e 7374 616c 6c20 7468 6520 4669 6e61  install the Fina
+00000bc0: 6e63 6961 6c20 4461 7461 7365 7473 206c  ncial Datasets l
+00000bd0: 6962 7261 7279 2075 7369 6e67 2070 6970  ibrary using pip
+00000be0: 3a0a 0a60 6060 0a70 6970 2069 6e73 7461  :..```.pip insta
+00000bf0: 6c6c 2066 696e 616e 6369 616c 2d64 6174  ll financial-dat
+00000c00: 6173 6574 730a 6060 600a 0a23 2323 2055  asets.```..### U
+00000c10: 7369 6e67 2050 6f65 7472 790a 0a49 6620  sing Poetry..If 
+00000c20: 796f 7520 7072 6566 6572 2074 6f20 7573  you prefer to us
+00000c30: 6520 506f 6574 7279 2066 6f72 2064 6570  e Poetry for dep
+00000c40: 656e 6465 6e63 7920 6d61 6e61 6765 6d65  endency manageme
+00000c50: 6e74 2c20 796f 7520 6361 6e20 6164 6420  nt, you can add 
+00000c60: 4669 6e61 6e63 6961 6c20 4461 7461 7365  Financial Datase
+00000c70: 7473 2074 6f20 796f 7572 2070 726f 6a65  ts to your proje
+00000c80: 6374 3a0a 0a60 6060 0a70 6f65 7472 7920  ct:..```.poetry 
+00000c90: 6164 6420 6669 6e61 6e63 6961 6c2d 6461  add financial-da
+00000ca0: 7461 7365 7473 0a60 6060 0a0a 2323 2320  tasets.```..### 
+00000cb0: 4672 6f6d 2074 6865 2052 6570 6f73 6974  From the Reposit
+00000cc0: 6f72 790a 0a49 6620 796f 7520 7761 6e74  ory..If you want
+00000cd0: 2074 6f20 696e 7374 616c 6c20 7468 6520   to install the 
+00000ce0: 6c69 6272 6172 7920 6469 7265 6374 6c79  library directly
+00000cf0: 2066 726f 6d20 7468 6520 7265 706f 7369   from the reposi
+00000d00: 746f 7279 2c20 666f 6c6c 6f77 2074 6865  tory, follow the
+00000d10: 7365 2073 7465 7073 3a0a 0a31 2e20 436c  se steps:..1. Cl
+00000d20: 6f6e 6520 7468 6520 7265 706f 7369 746f  one the reposito
+00000d30: 7279 3a0a 2020 2060 6060 0a20 2020 6769  ry:.   ```.   gi
+00000d40: 7420 636c 6f6e 6520 6874 7470 733a 2f2f  t clone https://
+00000d50: 6769 7468 7562 2e63 6f6d 2f79 6f75 7275  github.com/youru
+00000d60: 7365 726e 616d 652f 6669 6e61 6e63 6961  sername/financia
+00000d70: 6c2d 6461 7461 7365 7473 2e67 6974 0a20  l-datasets.git. 
+00000d80: 2020 6060 600a 0a32 2e20 4e61 7669 6761    ```..2. Naviga
+00000d90: 7465 2074 6f20 7468 6520 7072 6f6a 6563  te to the projec
+00000da0: 7420 6469 7265 6374 6f72 793a 0a20 2020  t directory:.   
+00000db0: 6060 600a 2020 2063 6420 6669 6e61 6e63  ```.   cd financ
+00000dc0: 6961 6c2d 6461 7461 7365 7473 0a20 2020  ial-datasets.   
+00000dd0: 6060 600a 2020 200a 332e 2049 6e73 7461  ```.   .3. Insta
+00000de0: 6c6c 2074 6865 2064 6570 656e 6465 6e63  ll the dependenc
+00000df0: 6965 7320 7573 696e 6720 506f 6574 7279  ies using Poetry
+00000e00: 3a0a 2020 2060 6060 0a20 2020 706f 6574  :.   ```.   poet
+00000e10: 7279 2069 6e73 7461 6c6c 0a20 2020 6060  ry install.   ``
+00000e20: 600a 0a34 2e20 596f 7520 6361 6e20 6e6f  `..4. You can no
+00000e30: 7720 7573 6520 7468 6520 6c69 6272 6172  w use the librar
+00000e40: 7920 696e 2079 6f75 7220 5079 7468 6f6e  y in your Python
+00000e50: 2070 726f 6a65 6374 732e 0a0a 2323 2043   projects...## C
+00000e60: 6f6e 7472 6962 7574 696e 670a 0a43 6f6e  ontributing..Con
+00000e70: 7472 6962 7574 696f 6e73 2061 7265 2077  tributions are w
+00000e80: 656c 636f 6d65 2120 4966 2079 6f75 2066  elcome! If you f
+00000e90: 696e 6420 616e 7920 6973 7375 6573 206f  ind any issues o
+00000ea0: 7220 6861 7665 2073 7567 6765 7374 696f  r have suggestio
+00000eb0: 6e73 2066 6f72 2069 6d70 726f 7665 6d65  ns for improveme
+00000ec0: 6e74 732c 200a 706c 6561 7365 206f 7065  nts, .please ope
+00000ed0: 6e20 616e 2069 7373 7565 206f 7220 7375  n an issue or su
+00000ee0: 626d 6974 2061 2070 756c 6c20 7265 7175  bmit a pull requ
+00000ef0: 6573 742e 0a0a 2323 204c 6963 656e 7365  est...## License
+00000f00: 0a0a 5468 6973 2070 726f 6a65 6374 2069  ..This project i
+00000f10: 7320 6c69 6365 6e73 6564 2075 6e64 6572  s licensed under
+00000f20: 2074 6865 205b 4d49 5420 4c69 6365 6e73   the [MIT Licens
+00000f30: 655d 286c 696e 6b2d 746f 2d6c 6963 656e  e](link-to-licen
+00000f40: 7365 2d66 696c 6529 2e0a 0a23 2320 436f  se-file)...## Co
+00000f50: 6e74 7269 6275 746f 7273 0a0a 3c61 2068  ntributors..<a h
+00000f60: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00000f70: 6875 622e 636f 6d2f 7669 7261 7474 742f  hub.com/virattt/
+00000f80: 6669 6e61 6e63 6961 6c2d 6461 7461 7365  financial-datase
+00000f90: 7473 2f67 7261 7068 732f 636f 6e74 7269  ts/graphs/contri
+00000fa0: 6275 746f 7273 223e 0a20 203c 696d 6720  butors">.  <img 
+00000fb0: 7372 633d 2268 7474 7073 3a2f 2f63 6f6e  src="https://con
+00000fc0: 7472 6962 2e72 6f63 6b73 2f69 6d61 6765  trib.rocks/image
+00000fd0: 3f72 6570 6f3d 7669 7261 7474 742f 6669  ?repo=virattt/fi
+00000fe0: 6e61 6e63 6961 6c2d 6461 7461 7365 7473  nancial-datasets
+00000ff0: 2220 2f3e 0a3c 2f61 3e0a                 " />.</a>.
```

### Comparing `financial_datasets-0.1.6/financial_datasets/filings.py` & `financial_datasets-0.1.7/financial_datasets/filings.py`

 * *Files identical despite different names*

### Comparing `financial_datasets-0.1.6/financial_datasets/generator.py` & `financial_datasets-0.1.7/financial_datasets/generator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 import time
 from io import BytesIO
 from typing import List
 
 import requests
 from PyPDF2 import PdfReader
-from edgar import Company, set_identity
+from edgar import Company, set_identity, get_filings
 from instructor import patch
 from langchain_text_splitters import TokenTextSplitter
 from openai import OpenAI
 from tqdm import tqdm
 
 from financial_datasets.dataset import DatasetItem, Dataset
 from financial_datasets.filings import filter_filings
@@ -169,14 +169,87 @@
 
         # Remove any newline characters
         items = [item.replace("\n", " ") for item in items]
 
         # Remove any sequence of 3 or more '-' or '.' characters
         pattern1 = r'-{3,}|\.{3,}'
         items = [re.sub(pattern1, '', item) for item in items]
+
+        # Remove any sequence of 2 or more '+' characters
+        pattern2 = r'\+{2,}'
+        items = [re.sub(pattern2, '', item) for item in items]
+
+        # Chunk Items to prevent exceeding the context window of models at the question generation step.
+        chunk_size = 8192
+        chunk_overlap = 128
+        token_splitter = TokenTextSplitter(chunk_size=chunk_size, chunk_overlap=chunk_overlap)
+        texts = []  # List to hold the chunked items
+        for item in items:
+            chunks = token_splitter.split_text(item)
+            texts.extend(chunks)
+
+        # Generate questions from the extracted text
+        return self.generate_from_texts(texts=texts, max_questions=max_questions)
+
+    def generate_from_10Q(
+        self,
+        ticker: str,
+        year: int,
+        quarter: int,
+        max_questions=10,
+        sec_identity=default_sec_identity,
+    ) -> Dataset:
+        """
+        Generate questions from a specific SEC filing for a given ticker.
+
+        :param ticker: The stock ticker symbol.
+        :param year: The year of the filing.
+        :param quarter: The quarter of the filing.
+        :param max_questions: Maximum number of questions to generate.
+        :param sec_identity: The identity to use when making requests to the SEC API.
+        :return: Dataset containing the generated questions.
+        """
+
+        # Tell the SEC who is making the request
+        set_identity(sec_identity)
+
+        if not ticker:
+            raise ValueError("Ticker symbol is required.")
+
+        if not year:
+            raise ValueError("Year is required.")
+
+        # Get all 10-Q filings for the given year and quarter
+        filings = get_filings(year, quarter, form="10-Q")
+
+        # Create a Company object
+        company = Company(ticker)
+
+        # Filter the filings to find the one for the company
+        filing = next((f for f in filings if f.cik == company.cik), None)
+        if not filing:
+            raise ValueError(f"No 10-Q filing found for {ticker} in {year} Q{quarter}.")
+
+        # Get the filing entities for the company
+        company_filings = company.get_filings(form="10-Q", filing_date=filing.filing_date)
+        if not company_filings:
+            raise ValueError(f"No 10-Q filing found for {ticker} in {year} Q{quarter}.")
+
+        # Get the exact 10-Q filing for the company
+        company_filing = company_filings[0].obj()
+
+        # Extract the items from the filing
+        items = [company_filing[item] for item in company_filing.items if len(company_filing[item]) > 200]  # Ignore short items like "Item 6. Reserved"
+
+        # Remove any newline characters
+        items = [item.replace("\n", " ") for item in items]
+
+        # Remove any sequence of 3 or more '-' or '.' characters
+        pattern1 = r'-{3,}|\.{3,}'
+        items = [re.sub(pattern1, '', item) for item in items]
 
         # Remove any sequence of 2 or more '+' characters
         pattern2 = r'\+{2,}'
         items = [re.sub(pattern2, '', item) for item in items]
 
         # Chunk Items to prevent exceeding the context window of models at the question generation step.
         chunk_size = 8192
```

### Comparing `financial_datasets-0.1.6/financial_datasets/prompts.py` & `financial_datasets-0.1.7/financial_datasets/prompts.py`

 * *Files identical despite different names*

### Comparing `financial_datasets-0.1.6/pyproject.toml` & `financial_datasets-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "financial-datasets"
-version = "0.1.6"
+version = "0.1.7"
 description = "Financial datasets for LLMs"
 authors = ["Virat Singh <virat@virat.ai>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "financial_datasets"}]
 
 [tool.poetry.dependencies]
```

### Comparing `financial_datasets-0.1.6/PKG-INFO` & `financial_datasets-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: financial-datasets
-Version: 0.1.6
+Version: 0.1.7
 Summary: Financial datasets for LLMs
 License: MIT
 Author: Virat Singh
 Author-email: virat@virat.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -29,21 +29,14 @@
 that lets you create question & answer financial datasets
 using Large Language Models (LLMs). With this library,
 you can easily generate realistic financial datasets from a 10-K, 
 10-Q, PDF, and other financial texts.
 
 [![Twitter Follow](https://img.shields.io/twitter/follow/virattt?style=social)](https://twitter.com/virattt)
 
-## Features
-
-- Generate synthetic financial datasets using LLMs
-- Supports various SEC filings (10-Ks, 10-Qs, etc.)
-- Easy integration with Python projects
-- Customizable data generation options
-
 ## Usage
 
 **Example generated dataset:**
 ```json
 [
   {
     "question": "What was Airbnb's revenue in 2023?",
@@ -54,57 +47,60 @@
     "question": "By what percentage did Airbnb's net income increase in 2023 compared to the prior year?",
     "answer": "153%",
     "context": "Net income in 2023 increased by 153% to $4.8 billion, compared to the prior year, driven by our revenue growth, increased interest income, discipline in managing our cost structure, and the release of a portion of our valuation allowance on deferred tax assets of $2.9 billion."
   }
 ]
 ```
 
-**Example #1 - generate from any texts:**
+**Example #1 - generate from any text**
 
 Most flexible option.  Generates dataset using a list of string `texts`. Colab code example [here](https://colab.research.google.com/gist/virattt/f9b5a0ae82cc0caab57df5dedc2927c9/intro-financial-datasets.ipynb).
 
 ```python
 from financial_datasets.generator import DatasetGenerator
 
-texts = ...  # List of texts from SEC filing
+# Your list of texts
+texts = ...  
+
+# Create dataset generator
 generator = DatasetGenerator(model="gpt-4-0125-preview", api_key="your-openai-key")
 
 # Generate dataset from texts
 dataset = generator.generate_from_texts(
    texts=texts, 
    max_questions=100,
 )
 ```
 
-**Example #2 - generate from 10-K:**
+**Example #2 - generate from 10-K**
 
 Generate a dataset using a `ticker` and `year`.  Colab code example [here](https://colab.research.google.com/gist/virattt/743872e143034987d20e6a6c7bb9d0a1/intro-financial-datasets.ipynb).
 
 ```python
 from financial_datasets.generator import DatasetGenerator
 
-texts = ...  # List of texts from SEC filing
+# Create dataset generator
 generator = DatasetGenerator(model="gpt-4-0125-preview", api_key="your-openai-key")
 
 # Generate dataset from 10-K
 dataset = generator.generate_from_10K(
    ticker="AAPL",
    year=2023,
    max_questions=100,
 )
 ```
 
-**Example #3 - generate from PDF:**
+**Example #3 - generate from PDF**
 
 Generate a dataset using a PDF `url` only.  Colab code example [here](https://colab.research.google.com/gist/virattt/b04442ee7c6c0d0bb3c9371af2283a20/intro-financial-datasets.ipynb).
 
 ```python
 from financial_datasets.generator import DatasetGenerator
 
-texts = ...  # List of texts from SEC filing
+# Create dataset generator
 generator = DatasetGenerator(model="gpt-4-0125-preview", api_key="your-openai-key")
 
 # Generate dataset from PDF url
 dataset = generator.generate_from_pdf(
    url="https://www.berkshirehathaway.com/letters/2023ltr.pdf",
    max_questions=100,
 )
@@ -159,7 +155,8 @@
 This project is licensed under the [MIT License](link-to-license-file).
 
 ## Contributors
 
 <a href="https://github.com/virattt/financial-datasets/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=virattt/financial-datasets" />
 </a>
+
```

