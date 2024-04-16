# Comparing `tmp/carbonplan-0.5.0.tar.gz` & `tmp/carbonplan-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carbonplan-0.5.0.tar", last modified: Sat Feb  5 04:53:08 2022, max compression
+gzip compressed data, was "carbonplan-0.6.0.tar", last modified: Tue Apr 16 19:05:44 2024, max compression
```

## Comparing `carbonplan-0.5.0.tar` & `carbonplan-0.6.0.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2022-02-05 04:53:08.995712 carbonplan-0.5.0/
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2022-02-05 04:53:08.993447 carbonplan-0.5.0/.github/
--rw-r--r--   0 jhamman    (501) staff       (20)      199 2020-08-31 20:06:58.000000 carbonplan-0.5.0/.github/dependabot.yml
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2022-02-05 04:53:08.993606 carbonplan-0.5.0/.github/workflows/
--rw-r--r--   0 jhamman    (501) staff       (20)      998 2022-01-22 00:40:58.000000 carbonplan-0.5.0/.github/workflows/main.yaml
--rw-r--r--   0 jhamman    (501) staff       (20)     1799 2020-08-31 16:44:26.000000 carbonplan-0.5.0/.gitignore
--rw-r--r--   0 jhamman    (501) staff       (20)      959 2022-01-22 00:40:58.000000 carbonplan-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 jhamman    (501) staff       (20)     1067 2020-08-31 16:44:26.000000 carbonplan-0.5.0/LICENSE
--rw-r--r--   0 jhamman    (501) staff       (20)     4012 2022-02-05 04:53:08.995822 carbonplan-0.5.0/PKG-INFO
--rw-r--r--   0 jhamman    (501) staff       (20)     2754 2021-05-13 03:07:17.000000 carbonplan-0.5.0/README.md
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2022-02-05 04:53:08.994631 carbonplan-0.5.0/carbonplan/
--rw-r--r--   0 jhamman    (501) staff       (20)      233 2020-10-19 19:21:46.000000 carbonplan-0.5.0/carbonplan/__init__.py
--rw-r--r--   0 jhamman    (501) staff       (20)      539 2020-10-19 19:58:51.000000 carbonplan-0.5.0/carbonplan/data.py
--rw-r--r--   0 jhamman    (501) staff       (20)      338 2021-05-13 03:01:00.000000 carbonplan-0.5.0/carbonplan/forests_offsets.py
--rw-r--r--   0 jhamman    (501) staff       (20)      327 2021-05-13 02:55:36.000000 carbonplan-0.5.0/carbonplan/forests_risks.py
--rw-r--r--   0 jhamman    (501) staff       (20)      307 2020-10-19 19:57:13.000000 carbonplan-0.5.0/carbonplan/styles.py
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2022-02-05 04:53:08.995483 carbonplan-0.5.0/carbonplan/tests/
--rw-r--r--   0 jhamman    (501) staff       (20)      259 2021-05-13 03:43:54.000000 carbonplan-0.5.0/carbonplan/tests/test_metapackage.py
--rw-r--r--   0 jhamman    (501) staff       (20)      170 2022-01-22 01:10:14.000000 carbonplan-0.5.0/carbonplan/tests/test_watermark.py
--rw-r--r--   0 jhamman    (501) staff       (20)      303 2021-06-22 03:22:49.000000 carbonplan-0.5.0/carbonplan/trace.py
--rw-r--r--   0 jhamman    (501) staff       (20)      500 2022-01-22 01:07:20.000000 carbonplan-0.5.0/carbonplan/watermark.py
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2022-02-05 04:53:08.995242 carbonplan-0.5.0/carbonplan.egg-info/
--rw-r--r--   0 jhamman    (501) staff       (20)     4012 2022-02-05 04:53:08.000000 carbonplan-0.5.0/carbonplan.egg-info/PKG-INFO
--rw-r--r--   0 jhamman    (501) staff       (20)      592 2022-02-05 04:53:08.000000 carbonplan-0.5.0/carbonplan.egg-info/SOURCES.txt
--rw-r--r--   0 jhamman    (501) staff       (20)        1 2022-02-05 04:53:08.000000 carbonplan-0.5.0/carbonplan.egg-info/dependency_links.txt
--rw-r--r--   0 jhamman    (501) staff       (20)      211 2022-02-05 04:53:08.000000 carbonplan-0.5.0/carbonplan.egg-info/requires.txt
--rw-r--r--   0 jhamman    (501) staff       (20)       11 2022-02-05 04:53:08.000000 carbonplan-0.5.0/carbonplan.egg-info/top_level.txt
--rw-r--r--   0 jhamman    (501) staff       (20)       41 2022-01-22 00:44:14.000000 carbonplan-0.5.0/dev-requirements.txt
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2022-02-05 04:53:08.995605 carbonplan-0.5.0/docs/
--rw-r--r--   0 jhamman    (501) staff       (20)      527 2021-09-15 15:12:10.000000 carbonplan-0.5.0/docs/release-procedure.md
--rw-r--r--   0 jhamman    (501) staff       (20)       10 2022-01-22 00:44:20.000000 carbonplan-0.5.0/requirements.txt
--rw-r--r--   0 jhamman    (501) staff       (20)      422 2022-02-05 04:53:08.996115 carbonplan-0.5.0/setup.cfg
--rw-r--r--   0 jhamman    (501) staff       (20)     1644 2022-01-22 00:45:16.000000 carbonplan-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:05:44.196133 carbonplan-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:05:44.192133 carbonplan-0.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-16 19:05:32.000000 carbonplan-0.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:05:44.192133 carbonplan-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-16 19:05:32.000000 carbonplan-0.6.0/.github/workflows/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-16 19:05:32.000000 carbonplan-0.6.0/.github/workflows/pypi-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-16 19:05:32.000000 carbonplan-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-16 19:05:32.000000 carbonplan-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-16 19:05:32.000000 carbonplan-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-16 19:05:44.196133 carbonplan-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-16 19:05:32.000000 carbonplan-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:05:44.192133 carbonplan-0.6.0/carbonplan/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-16 19:05:32.000000 carbonplan-0.6.0/carbonplan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-16 19:05:32.000000 carbonplan-0.6.0/carbonplan/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-16 19:05:32.000000 carbonplan-0.6.0/carbonplan/forests_offsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-16 19:05:32.000000 carbonplan-0.6.0/carbonplan/forests_risks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-16 19:05:32.000000 carbonplan-0.6.0/carbonplan/styles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:05:44.196133 carbonplan-0.6.0/carbonplan/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-16 19:05:32.000000 carbonplan-0.6.0/carbonplan/tests/test_metapackage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-16 19:05:32.000000 carbonplan-0.6.0/carbonplan/tests/test_watermark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-16 19:05:32.000000 carbonplan-0.6.0/carbonplan/trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-16 19:05:32.000000 carbonplan-0.6.0/carbonplan/watermark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:05:44.196133 carbonplan-0.6.0/carbonplan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-16 19:05:44.000000 carbonplan-0.6.0/carbonplan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-16 19:05:44.000000 carbonplan-0.6.0/carbonplan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:05:44.000000 carbonplan-0.6.0/carbonplan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-16 19:05:44.000000 carbonplan-0.6.0/carbonplan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 19:05:44.000000 carbonplan-0.6.0/carbonplan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:05:44.196133 carbonplan-0.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-16 19:05:32.000000 carbonplan-0.6.0/docs/release-procedure.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-16 19:05:32.000000 carbonplan-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:05:44.196133 carbonplan-0.6.0/setup.cfg
```

### Comparing `carbonplan-0.5.0/.gitignore` & `carbonplan-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `carbonplan-0.5.0/LICENSE` & `carbonplan-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `carbonplan-0.5.0/PKG-INFO` & `carbonplan-0.6.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,251 +1,280 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6361 7262  : 2.1.Name: carb
 00000020: 6f6e 706c 616e 0a56 6572 7369 6f6e 3a20  onplan.Version: 
-00000030: 302e 352e 300a 5375 6d6d 6172 793a 2043  0.5.0.Summary: C
+00000030: 302e 362e 300a 5375 6d6d 6172 793a 2043  0.6.0.Summary: C
 00000040: 6172 626f 6e50 6c61 6e20 6e61 6d65 7370  arbonPlan namesp
-00000050: 6163 6520 7061 636b 6167 650a 486f 6d65  ace package.Home
-00000060: 2d70 6167 653a 2068 7474 7073 3a2f 2f67  -page: https://g
-00000070: 6974 6875 622e 636f 6d2f 6361 7262 6f6e  ithub.com/carbon
-00000080: 706c 616e 2f63 6172 626f 6e70 6c61 6e2d  plan/carbonplan-
-00000090: 7079 7468 6f6e 0a4d 6169 6e74 6169 6e65  python.Maintaine
-000000a0: 723a 204a 6f65 2048 616d 6d61 6e0a 4d61  r: Joe Hamman.Ma
-000000b0: 696e 7461 696e 6572 2d65 6d61 696c 3a20  intainer-email: 
-000000c0: 6a6f 6540 6361 7262 6f6e 706c 616e 2e6f  joe@carbonplan.o
-000000d0: 7267 0a4c 6963 656e 7365 3a20 4d49 540a  rg.License: MIT.
-000000e0: 4465 7363 7269 7074 696f 6e3a 203c 696d  Description: <im
-000000f0: 670a 2020 2020 2020 2020 2020 7372 633d  g.          src=
-00000100: 2768 7474 7073 3a2f 2f63 6172 626f 6e70  'https://carbonp
-00000110: 6c61 6e2d 6173 7365 7473 2e73 332e 616d  lan-assets.s3.am
-00000120: 617a 6f6e 6177 732e 636f 6d2f 6d6f 6e6f  azonaws.com/mono
-00000130: 6772 616d 2f64 6172 6b2d 736d 616c 6c2e  gram/dark-small.
-00000140: 706e 6727 0a20 2020 2020 2020 2020 2068  png'.          h
-00000150: 6569 6768 743d 2734 3827 0a20 2020 2020  eight='48'.     
-00000160: 2020 202f 3e0a 2020 2020 2020 2020 0a20     />.        . 
-00000170: 2020 2020 2020 2023 2063 6172 626f 6e70         # carbonp
-00000180: 6c61 6e20 2f20 6361 7262 6f6e 706c 616e  lan / carbonplan
-00000190: 2d70 7974 686f 6e0a 2020 2020 2020 2020  -python.        
-000001a0: 0a20 2020 2020 2020 202a 2a6e 616d 6573  .        **names
-000001b0: 7061 6365 2070 6163 6b61 6765 2066 6f72  pace package for
-000001c0: 2070 7974 686f 6e20 7574 696c 6974 6965   python utilitie
-000001d0: 7320 616e 6420 7375 6270 726f 6a65 6374  s and subproject
-000001e0: 732a 2a0a 2020 2020 2020 2020 0a20 2020  s**.        .   
-000001f0: 2020 2020 205b 215b 4349 5d28 6874 7470       [![CI](http
-00000200: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
-00000210: 6172 626f 6e70 6c61 6e2f 6361 7262 6f6e  arbonplan/carbon
-00000220: 706c 616e 2d70 7974 686f 6e2f 6163 7469  plan-python/acti
-00000230: 6f6e 732f 776f 726b 666c 6f77 732f 6d61  ons/workflows/ma
-00000240: 696e 2e79 616d 6c2f 6261 6467 652e 7376  in.yaml/badge.sv
-00000250: 6729 5d28 6874 7470 733a 2f2f 6769 7468  g)](https://gith
-00000260: 7562 2e63 6f6d 2f63 6172 626f 6e70 6c61  ub.com/carbonpla
-00000270: 6e2f 6361 7262 6f6e 706c 616e 2d70 7974  n/carbonplan-pyt
-00000280: 686f 6e2f 6163 7469 6f6e 732f 776f 726b  hon/actions/work
-00000290: 666c 6f77 732f 6d61 696e 2e79 616d 6c29  flows/main.yaml)
-000002a0: 0a20 2020 2020 2020 2021 5b4d 4954 204c  .        ![MIT L
-000002b0: 6963 656e 7365 5d5b 5d0a 2020 2020 2020  icense][].      
-000002c0: 2020 5b21 5b50 7950 4920 7665 7273 696f    [![PyPI versio
-000002d0: 6e5d 2868 7474 7073 3a2f 2f62 6164 6765  n](https://badge
-000002e0: 2e66 7572 792e 696f 2f70 792f 6361 7262  .fury.io/py/carb
-000002f0: 6f6e 706c 616e 2e73 7667 295d 2868 7474  onplan.svg)](htt
-00000300: 7073 3a2f 2f62 6164 6765 2e66 7572 792e  ps://badge.fury.
-00000310: 696f 2f70 792f 6361 7262 6f6e 706c 616e  io/py/carbonplan
-00000320: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-00000330: 2020 205b 6769 7468 7562 2d62 6164 6765     [github-badge
-00000340: 5d3a 2068 7474 7073 3a2f 2f62 6164 6765  ]: https://badge
-00000350: 6e2e 6e65 742f 6261 6467 652f 2d2f 6769  n.net/badge/-/gi
-00000360: 7468 7562 3f69 636f 6e3d 6769 7468 7562  thub?icon=github
-00000370: 266c 6162 656c 0a20 2020 2020 2020 205b  &label.        [
-00000380: 6d69 7420 6c69 6365 6e73 655d 3a20 6874  mit license]: ht
-00000390: 7470 733a 2f2f 6261 6467 656e 2e6e 6574  tps://badgen.net
-000003a0: 2f62 6164 6765 2f6c 6963 656e 7365 2f4d  /badge/license/M
-000003b0: 4954 2f62 6c75 650a 2020 2020 2020 2020  IT/blue.        
-000003c0: 0a20 2020 2020 2020 2054 6869 7320 7265  .        This re
-000003d0: 706f 7369 746f 7279 2069 6e63 6c75 6465  pository include
-000003e0: 7320 7468 6520 6063 6172 626f 6e70 6c61  s the `carbonpla
-000003f0: 6e60 206e 616d 6573 7061 6365 2050 7974  n` namespace Pyt
-00000400: 686f 6e20 7061 636b 6167 652e 2054 6865  hon package. The
-00000410: 2070 6163 6b61 6765 2069 7473 656c 6620   package itself 
-00000420: 696e 636c 7564 6573 2076 6572 7920 6c69  includes very li
-00000430: 7474 6c65 206f 6620 7375 6273 7461 6e63  ttle of substanc
-00000440: 652c 2061 6e64 2069 7320 6469 7374 7269  e, and is distri
-00000450: 6275 7465 6420 746f 2061 6374 2061 7320  buted to act as 
-00000460: 7468 6520 746f 702d 6c65 7665 6c20 6e61  the top-level na
-00000470: 6d65 7370 6163 6520 666f 7220 6f74 6865  mespace for othe
-00000480: 7220 5079 7468 6f6e 2070 6163 6b61 6765  r Python package
-00000490: 7320 6465 7665 6c6f 7065 6420 6279 2043  s developed by C
-000004a0: 6172 626f 6e50 6c61 6e2e 204f 7468 6572  arbonPlan. Other
-000004b0: 2070 6163 6b61 6765 7320 696e 636c 7564   packages includ
-000004c0: 653a 0a20 2020 2020 2020 200a 2020 2020  e:.        .    
-000004d0: 2020 2020 7c20 5061 636b 6167 6520 2020      | Package   
-000004e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000004f0: 7c20 496d 706f 7274 2020 2020 2020 2020  | Import        
-00000500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000510: 2020 2020 207c 2047 6974 4875 6220 5265       | GitHub Re
-00000520: 706f 2020 2020 2020 2020 2020 2020 2020  po              
-00000530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000570: 2020 2020 7c0a 2020 2020 2020 2020 7c20      |.        | 
-00000580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000590: 2d2d 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d  --------- | ----
-000005a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000005b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c  -------------- |
-000005c0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
-000005d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000005e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000005f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000600: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c0a  ------------- |.
-00000620: 2020 2020 2020 2020 7c20 6361 7262 6f6e          | carbon
-00000630: 706c 616e 2d64 6174 6120 2020 2020 2020  plan-data       
-00000640: 2020 2020 7c20 6069 6d70 6f72 7420 6361      | `import ca
-00000650: 7262 6f6e 706c 616e 2e64 6174 6160 2020  rbonplan.data`  
-00000660: 2020 2020 2020 2020 207c 205b 6874 7470           | [http
-00000670: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
-00000680: 6172 626f 6e70 6c61 6e2f 6461 7461 5d28  arbonplan/data](
-00000690: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000006a0: 6f6d 2f63 6172 626f 6e70 6c61 6e2f 6461  om/carbonplan/da
-000006b0: 7461 2920 2020 2020 2020 2020 2020 2020  ta)             
-000006c0: 2020 2020 2020 2020 7c0a 2020 2020 2020          |.      
-000006d0: 2020 7c20 6361 7262 6f6e 706c 616e 2d66    | carbonplan-f
-000006e0: 6f72 6573 742d 6f66 6673 6574 7320 7c20  orest-offsets | 
-000006f0: 6069 6d70 6f72 7420 6361 7262 6f6e 706c  `import carbonpl
-00000700: 616e 2e66 6f72 6573 745f 6f66 6673 6574  an.forest_offset
-00000710: 7360 207c 205b 6874 7470 733a 2f2f 6769  s` | [https://gi
-00000720: 7468 7562 2e63 6f6d 2f63 6172 626f 6e70  thub.com/carbonp
-00000730: 6c61 6e2f 666f 7265 7374 2d6f 6666 7365  lan/forest-offse
-00000740: 7473 5d28 6874 7470 733a 2f2f 6769 7468  ts](https://gith
-00000750: 7562 2e63 6f6d 2f63 6172 626f 6e70 6c61  ub.com/carbonpla
-00000760: 6e2f 666f 7265 7374 2d6f 6666 7365 7473  n/forest-offsets
-00000770: 2920 7c0a 2020 2020 2020 2020 7c20 6361  ) |.        | ca
-00000780: 7262 6f6e 706c 616e 2d66 6f72 6573 742d  rbonplan-forest-
-00000790: 7269 736b 7320 2020 7c20 6069 6d70 6f72  risks   | `impor
-000007a0: 7420 6361 7262 6f6e 706c 616e 2e66 6f72  t carbonplan.for
-000007b0: 6573 745f 7269 736b 7360 2020 207c 205b  est_risks`   | [
-000007c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000007d0: 6f6d 2f63 6172 626f 6e70 6c61 6e2f 666f  om/carbonplan/fo
-000007e0: 7265 7374 2d72 6973 6b73 5d28 6874 7470  rest-risks](http
-000007f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
-00000800: 6172 626f 6e70 6c61 6e2f 666f 7265 7374  arbonplan/forest
-00000810: 2d72 6973 6b73 2920 2020 2020 7c0a 2020  -risks)     |.  
-00000820: 2020 2020 2020 7c20 6361 7262 6f6e 706c        | carbonpl
-00000830: 616e 2d73 7479 6c65 7320 2020 2020 2020  an-styles       
-00000840: 2020 7c20 6069 6d70 6f72 7420 6361 7262    | `import carb
-00000850: 6f6e 706c 616e 2e73 7479 6c65 7360 2020  onplan.styles`  
-00000860: 2020 2020 2020 207c 205b 6874 7470 733a         | [https:
-00000870: 2f2f 6769 7468 7562 2e63 6f6d 2f63 6172  //github.com/car
-00000880: 626f 6e70 6c61 6e2f 7374 796c 6573 5d28  bonplan/styles](
-00000890: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000008a0: 6f6d 2f63 6172 626f 6e70 6c61 6e2f 7374  om/carbonplan/st
-000008b0: 796c 6573 2920 2020 2020 2020 2020 2020  yles)           
-000008c0: 2020 2020 2020 7c0a 2020 2020 2020 2020        |.        
-000008d0: 0a20 2020 2020 2020 2023 2320 696e 7374  .        ## inst
-000008e0: 616c 6c0a 2020 2020 2020 2020 0a20 2020  all.        .   
-000008f0: 2020 2020 2060 6060 7368 656c 6c0a 2020       ```shell.  
-00000900: 2020 2020 2020 7069 7020 696e 7374 616c        pip instal
-00000910: 6c20 6361 7262 6f6e 706c 616e 5b61 6c6c  l carbonplan[all
-00000920: 5d0a 2020 2020 2020 2020 2320 6f72 2069  ].        # or i
-00000930: 6e64 6976 6964 7561 6c20 7375 6220 7061  ndividual sub pa
-00000940: 636b 6167 6573 0a20 2020 2020 2020 2070  ckages.        p
-00000950: 6970 2069 6e73 7461 6c6c 2063 6172 626f  ip install carbo
-00000960: 6e70 6c61 6e5b 7374 796c 6573 5d0a 2020  nplan[styles].  
-00000970: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
-00000980: 2020 0a20 2020 2020 2020 2023 2320 7573    .        ## us
-00000990: 6167 650a 2020 2020 2020 2020 0a20 2020  age.        .   
-000009a0: 2020 2020 2060 6060 7079 7468 6f6e 0a20       ```python. 
-000009b0: 2020 2020 2020 2066 726f 6d20 6361 7262         from carb
-000009c0: 6f6e 706c 616e 2e73 7479 6c65 732e 6d70  onplan.styles.mp
-000009d0: 6c20 696d 706f 7274 2073 6574 5f74 6865  l import set_the
-000009e0: 6d65 0a20 2020 2020 2020 2023 2074 6869  me.        # thi
-000009f0: 7320 6973 2074 6865 2073 616d 6520 7468  s is the same th
-00000a00: 696e 6773 2061 730a 2020 2020 2020 2020  ings as.        
-00000a10: 6672 6f6d 2063 6172 626f 6e70 6c61 6e5f  from carbonplan_
-00000a20: 7374 796c 6573 2e6d 706c 2069 6d70 6f72  styles.mpl impor
-00000a30: 7420 7365 745f 7468 656d 650a 2020 2020  t set_theme.    
-00000a40: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
-00000a50: 0a20 2020 2020 2020 2023 2320 6c69 6365  .        ## lice
-00000a60: 6e73 650a 2020 2020 2020 2020 0a20 2020  nse.        .   
-00000a70: 2020 2020 2041 6c6c 2074 6865 2063 6f64       All the cod
-00000a80: 6520 696e 2074 6869 7320 7265 706f 7369  e in this reposi
-00000a90: 746f 7279 2069 7320 5b4d 4954 5d28 6874  tory is [MIT](ht
-00000aa0: 7470 733a 2f2f 6368 6f6f 7365 616c 6963  tps://choosealic
-00000ab0: 656e 7365 2e63 6f6d 2f6c 6963 656e 7365  ense.com/license
-00000ac0: 732f 6d69 742f 2920 6c69 6365 6e73 6564  s/mit/) licensed
-00000ad0: 2e20 5765 2069 6e63 6c75 6465 2061 7474  . We include att
-00000ae0: 7269 6275 7469 6f6e 2066 6f72 2074 6869  ribution for thi
-00000af0: 7320 636f 6e74 656e 742c 2061 6e64 2077  s content, and w
-00000b00: 6520 706c 6561 7365 2072 6571 7565 7374  e please request
-00000b10: 2074 6861 7420 796f 7520 616c 736f 206d   that you also m
-00000b20: 6169 6e74 6169 6e20 7468 6174 2061 7474  aintain that att
-00000b30: 7269 6275 7469 6f6e 2069 6620 7573 696e  ribution if usin
-00000b40: 6720 7468 6973 2064 6174 612e 0a20 2020  g this data..   
-00000b50: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
-00000b60: 2061 626f 7574 2075 730a 2020 2020 2020   about us.      
-00000b70: 2020 0a20 2020 2020 2020 2043 6172 626f    .        Carbo
-00000b80: 6e50 6c61 6e20 6973 2061 206e 6f6e 2d70  nPlan is a non-p
-00000b90: 726f 6669 7420 6f72 6761 6e69 7a61 7469  rofit organizati
-00000ba0: 6f6e 2074 6861 7420 7573 6573 2064 6174  on that uses dat
-00000bb0: 6120 616e 6420 7363 6965 6e63 6520 666f  a and science fo
-00000bc0: 7220 636c 696d 6174 6520 6163 7469 6f6e  r climate action
-00000bd0: 2e20 5765 2061 696d 2074 6f20 696d 7072  . We aim to impr
-00000be0: 6f76 6520 7468 6520 7472 616e 7370 6172  ove the transpar
-00000bf0: 656e 6379 2061 6e64 2073 6369 656e 7469  ency and scienti
-00000c00: 6669 6320 696e 7465 6772 6974 7920 6f66  fic integrity of
-00000c10: 2063 6172 626f 6e20 7265 6d6f 7661 6c20   carbon removal 
-00000c20: 616e 6420 636c 696d 6174 6520 736f 6c75  and climate solu
-00000c30: 7469 6f6e 7320 7468 726f 7567 6820 6f70  tions through op
-00000c40: 656e 2064 6174 6120 616e 6420 746f 6f6c  en data and tool
-00000c50: 732e 2046 696e 6420 6f75 7420 6d6f 7265  s. Find out more
-00000c60: 2061 7420 5b63 6172 626f 6e70 6c61 6e2e   at [carbonplan.
-00000c70: 6f72 675d 2868 7474 7073 3a2f 2f63 6172  org](https://car
-00000c80: 626f 6e70 6c61 6e2e 6f72 672f 2920 6f72  bonplan.org/) or
-00000c90: 2067 6574 2069 6e20 746f 7563 6820 6279   get in touch by
-00000ca0: 205b 6f70 656e 696e 6720 616e 2069 7373   [opening an iss
-00000cb0: 7565 5d28 6874 7470 733a 2f2f 6769 7468  ue](https://gith
-00000cc0: 7562 2e63 6f6d 2f63 6172 626f 6e70 6c61  ub.com/carbonpla
-00000cd0: 6e2f 6361 7262 6f6e 706c 616e 2d70 7974  n/carbonplan-pyt
-00000ce0: 686f 6e2f 6973 7375 6573 2f6e 6577 2920  hon/issues/new) 
-00000cf0: 6f72 205b 7365 6e64 696e 6720 7573 2061  or [sending us a
-00000d00: 6e20 656d 6169 6c5d 286d 6169 6c74 6f3a  n email](mailto:
-00000d10: 6865 6c6c 6f40 6361 7262 6f6e 706c 616e  hello@carbonplan
-00000d20: 2e6f 7267 292e 0a20 2020 2020 2020 200a  .org)..        .
-00000d30: 506c 6174 666f 726d 3a20 554e 4b4e 4f57  Platform: UNKNOW
-00000d40: 4e0a 436c 6173 7369 6669 6572 3a20 4465  N.Classifier: De
-00000d50: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
-00000d60: 203a 3a20 3220 2d20 5072 652d 416c 7068   :: 2 - Pre-Alph
-00000d70: 610a 436c 6173 7369 6669 6572 3a20 4c69  a.Classifier: Li
-00000d80: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
-00000d90: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
-00000da0: 656e 7365 0a43 6c61 7373 6966 6965 723a  ense.Classifier:
-00000db0: 204f 7065 7261 7469 6e67 2053 7973 7465   Operating Syste
-00000dc0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
-00000dd0: 656e 740a 436c 6173 7369 6669 6572 3a20  ent.Classifier: 
-00000de0: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
-00000df0: 6520 3a3a 2053 6369 656e 6365 2f52 6573  e :: Science/Res
-00000e00: 6561 7263 680a 436c 6173 7369 6669 6572  earch.Classifier
-00000e10: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000e20: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000e30: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000e40: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000e50: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000e60: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000e70: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000e80: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000e90: 2e38 0a43 6c61 7373 6966 6965 723a 2050  .8.Classifier: P
-00000ea0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000eb0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000ec0: 2033 2e39 0a43 6c61 7373 6966 6965 723a   3.9.Classifier:
-00000ed0: 2054 6f70 6963 203a 3a20 5363 6965 6e74   Topic :: Scient
-00000ee0: 6966 6963 2f45 6e67 696e 6565 7269 6e67  ific/Engineering
-00000ef0: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
-00000f00: 3a20 3e3d 332e 380a 4465 7363 7269 7074  : >=3.8.Descript
-00000f10: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
-00000f20: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
-00000f30: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-00000f40: 616c 6c0a 5072 6f76 6964 6573 2d45 7874  all.Provides-Ext
-00000f50: 7261 3a20 6461 7461 0a50 726f 7669 6465  ra: data.Provide
-00000f60: 732d 4578 7472 613a 2066 6f72 6573 742d  s-Extra: forest-
-00000f70: 6f66 6673 6574 730a 5072 6f76 6964 6573  offsets.Provides
-00000f80: 2d45 7874 7261 3a20 666f 7265 7374 2d72  -Extra: forest-r
-00000f90: 6973 6b73 0a50 726f 7669 6465 732d 4578  isks.Provides-Ex
-00000fa0: 7472 613a 2073 7479 6c65 730a            tra: styles.
+00000050: 6163 6520 7061 636b 6167 650a 4175 7468  ace package.Auth
+00000060: 6f72 2d65 6d61 696c 3a20 4361 7262 6f6e  or-email: Carbon
+00000070: 506c 616e 203c 7465 6368 4063 6172 626f  Plan <tech@carbo
+00000080: 6e70 6c61 6e2e 6f72 673e 0a4c 6963 656e  nplan.org>.Licen
+00000090: 7365 3a20 4d49 540a 5072 6f6a 6563 742d  se: MIT.Project-
+000000a0: 5552 4c3a 2072 6570 6f73 6974 6f72 792c  URL: repository,
+000000b0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+000000c0: 636f 6d2f 6361 7262 6f6e 706c 616e 2f63  com/carbonplan/c
+000000d0: 6172 626f 6e70 6c61 6e2d 7079 7468 6f6e  arbonplan-python
+000000e0: 0a43 6c61 7373 6966 6965 723a 2044 6576  .Classifier: Dev
+000000f0: 656c 6f70 6d65 6e74 2053 7461 7475 7320  elopment Status 
+00000100: 3a3a 2032 202d 2050 7265 2d41 6c70 6861  :: 2 - Pre-Alpha
+00000110: 0a43 6c61 7373 6966 6965 723a 204c 6963  .Classifier: Lic
+00000120: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+00000130: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
+00000140: 6e73 650a 436c 6173 7369 6669 6572 3a20  nse.Classifier: 
+00000150: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+00000160: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
+00000170: 6e74 0a43 6c61 7373 6966 6965 723a 2049  nt.Classifier: I
+00000180: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
+00000190: 203a 3a20 5363 6965 6e63 652f 5265 7365   :: Science/Rese
+000001a0: 6172 6368 0a43 6c61 7373 6966 6965 723a  arch.Classifier:
+000001b0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+000001c0: 6775 6167 6520 3a3a 2050 7974 686f 6e0a  guage :: Python.
+000001d0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+000001e0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000001f0: 203a 3a20 5079 7468 6f6e 203a 3a20 330a   :: Python :: 3.
+00000200: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000210: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000220: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000230: 390a 436c 6173 7369 6669 6572 3a20 5072  9.Classifier: Pr
+00000240: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000250: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000260: 332e 3130 0a43 6c61 7373 6966 6965 723a  3.10.Classifier:
+00000270: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000280: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000290: 3a3a 2033 2e31 310a 436c 6173 7369 6669  :: 3.11.Classifi
+000002a0: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+000002b0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000002c0: 6f6e 203a 3a20 332e 3132 0a43 6c61 7373  on :: 3.12.Class
+000002d0: 6966 6965 723a 2054 6f70 6963 203a 3a20  ifier: Topic :: 
+000002e0: 5363 6965 6e74 6966 6963 2f45 6e67 696e  Scientific/Engin
+000002f0: 6565 7269 6e67 0a52 6571 7569 7265 732d  eering.Requires-
+00000300: 5079 7468 6f6e 3a20 3e3d 332e 390a 4465  Python: >=3.9.De
+00000310: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
+00000320: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
+00000330: 6b64 6f77 6e0a 4c69 6365 6e73 652d 4669  kdown.License-Fi
+00000340: 6c65 3a20 4c49 4345 4e53 450a 5265 7175  le: LICENSE.Requ
+00000350: 6972 6573 2d44 6973 743a 2077 6174 6572  ires-Dist: water
+00000360: 6d61 726b 0a50 726f 7669 6465 732d 4578  mark.Provides-Ex
+00000370: 7472 613a 2064 6576 0a52 6571 7569 7265  tra: dev.Require
+00000380: 732d 4469 7374 3a20 7079 7465 7374 3b20  s-Dist: pytest; 
+00000390: 6578 7472 6120 3d3d 2022 6465 7622 0a52  extra == "dev".R
+000003a0: 6571 7569 7265 732d 4469 7374 3a20 6361  equires-Dist: ca
+000003b0: 7262 6f6e 706c 616e 2d64 6174 613b 2065  rbonplan-data; e
+000003c0: 7874 7261 203d 3d20 2264 6576 220a 5265  xtra == "dev".Re
+000003d0: 7175 6972 6573 2d44 6973 743a 2063 6172  quires-Dist: car
+000003e0: 626f 6e70 6c61 6e2d 7374 796c 6573 3b20  bonplan-styles; 
+000003f0: 6578 7472 6120 3d3d 2022 6465 7622 0a50  extra == "dev".P
+00000400: 726f 7669 6465 732d 4578 7472 613a 2061  rovides-Extra: a
+00000410: 6c6c 0a52 6571 7569 7265 732d 4469 7374  ll.Requires-Dist
+00000420: 3a20 6361 7262 6f6e 706c 616e 2d64 6174  : carbonplan-dat
+00000430: 613b 2065 7874 7261 203d 3d20 2261 6c6c  a; extra == "all
+00000440: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000450: 2063 6172 626f 6e70 6c61 6e2d 7374 796c   carbonplan-styl
+00000460: 6573 3b20 6578 7472 6120 3d3d 2022 616c  es; extra == "al
+00000470: 6c22 0a52 6571 7569 7265 732d 4469 7374  l".Requires-Dist
+00000480: 3a20 6361 7262 6f6e 706c 616e 2d66 6f72  : carbonplan-for
+00000490: 6573 742d 6f66 6673 6574 733b 2065 7874  est-offsets; ext
+000004a0: 7261 203d 3d20 2261 6c6c 220a 5265 7175  ra == "all".Requ
+000004b0: 6972 6573 2d44 6973 743a 2063 6172 626f  ires-Dist: carbo
+000004c0: 6e70 6c61 6e2d 666f 7265 7374 2d72 6973  nplan-forest-ris
+000004d0: 6b73 3b20 6578 7472 6120 3d3d 2022 616c  ks; extra == "al
+000004e0: 6c22 0a50 726f 7669 6465 732d 4578 7472  l".Provides-Extr
+000004f0: 613a 2064 6174 610a 5265 7175 6972 6573  a: data.Requires
+00000500: 2d44 6973 743a 2063 6172 626f 6e70 6c61  -Dist: carbonpla
+00000510: 6e2d 6461 7461 3b20 6578 7472 6120 3d3d  n-data; extra ==
+00000520: 2022 6461 7461 220a 5072 6f76 6964 6573   "data".Provides
+00000530: 2d45 7874 7261 3a20 7374 796c 6573 0a52  -Extra: styles.R
+00000540: 6571 7569 7265 732d 4469 7374 3a20 6361  equires-Dist: ca
+00000550: 7262 6f6e 706c 616e 2d73 7479 6c65 733b  rbonplan-styles;
+00000560: 2065 7874 7261 203d 3d20 2273 7479 6c65   extra == "style
+00000570: 7322 0a50 726f 7669 6465 732d 4578 7472  s".Provides-Extr
+00000580: 613a 2066 6f72 6573 742d 6f66 6673 6574  a: forest-offset
+00000590: 730a 5265 7175 6972 6573 2d44 6973 743a  s.Requires-Dist:
+000005a0: 2063 6172 626f 6e70 6c61 6e2d 666f 7265   carbonplan-fore
+000005b0: 7374 2d6f 6666 7365 7473 3b20 6578 7472  st-offsets; extr
+000005c0: 6120 3d3d 2022 666f 7265 7374 2d6f 6666  a == "forest-off
+000005d0: 7365 7473 220a 5072 6f76 6964 6573 2d45  sets".Provides-E
+000005e0: 7874 7261 3a20 666f 7265 7374 2d72 6973  xtra: forest-ris
+000005f0: 6b73 0a52 6571 7569 7265 732d 4469 7374  ks.Requires-Dist
+00000600: 3a20 6361 7262 6f6e 706c 616e 2d66 6f72  : carbonplan-for
+00000610: 6573 742d 7269 736b 733b 2065 7874 7261  est-risks; extra
+00000620: 203d 3d20 2266 6f72 6573 742d 7269 736b   == "forest-risk
+00000630: 7322 0a0a 3c70 2061 6c69 676e 3d22 6c65  s"..<p align="le
+00000640: 6674 2220 3e0a 3c61 2068 7265 663d 2768  ft" >.<a href='h
+00000650: 7474 7073 3a2f 2f63 6172 626f 6e70 6c61  ttps://carbonpla
+00000660: 6e2e 6f72 6727 3e0a 3c70 6963 7475 7265  n.org'>.<picture
+00000670: 3e0a 2020 3c73 6f75 7263 6520 6d65 6469  >.  <source medi
+00000680: 613d 2228 7072 6566 6572 732d 636f 6c6f  a="(prefers-colo
+00000690: 722d 7363 6865 6d65 3a20 6461 726b 2922  r-scheme: dark)"
+000006a0: 2073 7263 7365 743d 2268 7474 7073 3a2f   srcset="https:/
+000006b0: 2f63 6172 626f 6e70 6c61 6e2d 6173 7365  /carbonplan-asse
+000006c0: 7473 2e73 332e 616d 617a 6f6e 6177 732e  ts.s3.amazonaws.
+000006d0: 636f 6d2f 6d6f 6e6f 6772 616d 2f6c 6967  com/monogram/lig
+000006e0: 6874 2d73 6d61 6c6c 2e70 6e67 223e 0a20  ht-small.png">. 
+000006f0: 203c 696d 6720 616c 743d 2243 6172 626f   <img alt="Carbo
+00000700: 6e50 6c61 6e20 6d6f 6e6f 6772 616d 2e22  nPlan monogram."
+00000710: 2068 6569 6768 743d 2234 3822 2073 7263   height="48" src
+00000720: 3d22 6874 7470 733a 2f2f 6361 7262 6f6e  ="https://carbon
+00000730: 706c 616e 2d61 7373 6574 732e 7333 2e61  plan-assets.s3.a
+00000740: 6d61 7a6f 6e61 7773 2e63 6f6d 2f6d 6f6e  mazonaws.com/mon
+00000750: 6f67 7261 6d2f 6461 726b 2d73 6d61 6c6c  ogram/dark-small
+00000760: 2e70 6e67 223e 0a3c 2f70 6963 7475 7265  .png">.</picture
+00000770: 3e0a 3c2f 613e 0a3c 2f70 3e0a 0a23 2063  >.</a>.</p>..# c
+00000780: 6172 626f 6e70 6c61 6e20 2f20 6361 7262  arbonplan / carb
+00000790: 6f6e 706c 616e 2d70 7974 686f 6e0a 0a2a  onplan-python..*
+000007a0: 2a6e 616d 6573 7061 6365 2070 6163 6b61  *namespace packa
+000007b0: 6765 2066 6f72 2070 7974 686f 6e20 7574  ge for python ut
+000007c0: 696c 6974 6965 7320 616e 6420 7375 6270  ilities and subp
+000007d0: 726f 6a65 6374 732a 2a0a 0a5b 215b 4349  rojects**..[![CI
+000007e0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000007f0: 2e63 6f6d 2f63 6172 626f 6e70 6c61 6e2f  .com/carbonplan/
+00000800: 6361 7262 6f6e 706c 616e 2d70 7974 686f  carbonplan-pytho
+00000810: 6e2f 6163 7469 6f6e 732f 776f 726b 666c  n/actions/workfl
+00000820: 6f77 732f 6d61 696e 2e79 616d 6c2f 6261  ows/main.yaml/ba
+00000830: 6467 652e 7376 6729 5d28 6874 7470 733a  dge.svg)](https:
+00000840: 2f2f 6769 7468 7562 2e63 6f6d 2f63 6172  //github.com/car
+00000850: 626f 6e70 6c61 6e2f 6361 7262 6f6e 706c  bonplan/carbonpl
+00000860: 616e 2d70 7974 686f 6e2f 6163 7469 6f6e  an-python/action
+00000870: 732f 776f 726b 666c 6f77 732f 6d61 696e  s/workflows/main
+00000880: 2e79 616d 6c29 0a21 5b50 7950 495d 2868  .yaml).![PyPI](h
+00000890: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000008a0: 6473 2e69 6f2f 7079 7069 2f76 2f63 6172  ds.io/pypi/v/car
+000008b0: 626f 6e70 6c61 6e29 0a5b 215b 4c69 6365  bonplan).[![Lice
+000008c0: 6e73 653a 204d 4954 5d28 6874 7470 733a  nse: MIT](https:
+000008d0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000008e0: 2f62 6164 6765 2f4c 6963 656e 7365 2d4d  /badge/License-M
+000008f0: 4954 2d62 6c75 652e 7376 6729 5d28 6874  IT-blue.svg)](ht
+00000900: 7470 733a 2f2f 6f70 656e 736f 7572 6365  tps://opensource
+00000910: 2e6f 7267 2f6c 6963 656e 7365 732f 4d49  .org/licenses/MI
+00000920: 5429 0a0a 5468 6973 2072 6570 6f73 6974  T)..This reposit
+00000930: 6f72 7920 696e 636c 7564 6573 2074 6865  ory includes the
+00000940: 2060 6361 7262 6f6e 706c 616e 6020 6e61   `carbonplan` na
+00000950: 6d65 7370 6163 6520 5079 7468 6f6e 2070  mespace Python p
+00000960: 6163 6b61 6765 2e20 5468 6520 7061 636b  ackage. The pack
+00000970: 6167 6520 6974 7365 6c66 2069 6e63 6c75  age itself inclu
+00000980: 6465 7320 7665 7279 206c 6974 746c 6520  des very little 
+00000990: 6f66 2073 7562 7374 616e 6365 2c20 616e  of substance, an
+000009a0: 6420 6973 2064 6973 7472 6962 7574 6564  d is distributed
+000009b0: 2074 6f20 6163 7420 6173 2074 6865 2074   to act as the t
+000009c0: 6f70 2d6c 6576 656c 206e 616d 6573 7061  op-level namespa
+000009d0: 6365 2066 6f72 206f 7468 6572 2050 7974  ce for other Pyt
+000009e0: 686f 6e20 7061 636b 6167 6573 2064 6576  hon packages dev
+000009f0: 656c 6f70 6564 2062 7920 4361 7262 6f6e  eloped by Carbon
+00000a00: 506c 616e 2e20 4f74 6865 7220 7061 636b  Plan. Other pack
+00000a10: 6167 6573 2069 6e63 6c75 6465 3a0a 0a7c  ages include:..|
+00000a20: 2050 6163 6b61 6765 2020 2020 2020 2020   Package        
+00000a30: 2020 2020 2020 2020 2020 207c 2049 6d70             | Imp
+00000a40: 6f72 7420 2020 2020 2020 2020 2020 2020  ort             
+00000a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a60: 7c20 4769 7448 7562 2052 6570 6f20 2020  | GitHub Repo   
+00000a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ab0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00000ac0: 0a7c 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .| -------------
+00000ad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c 202d  ------------ | -
+00000ae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000af0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b00: 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  - | ------------
+00000b10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b60: 207c 0a7c 2063 6172 626f 6e70 6c61 6e2d   |.| carbonplan-
+00000b70: 6461 7461 2020 2020 2020 2020 2020 207c  data           |
+00000b80: 2060 696d 706f 7274 2063 6172 626f 6e70   `import carbonp
+00000b90: 6c61 6e2e 6461 7461 6020 2020 2020 2020  lan.data`       
+00000ba0: 2020 2020 7c20 5b68 7474 7073 3a2f 2f67      | [https://g
+00000bb0: 6974 6875 622e 636f 6d2f 6361 7262 6f6e  ithub.com/carbon
+00000bc0: 706c 616e 2f64 6174 615d 2868 7474 7073  plan/data](https
+00000bd0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6361  ://github.com/ca
+00000be0: 7262 6f6e 706c 616e 2f64 6174 6129 2020  rbonplan/data)  
+00000bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c00: 2020 207c 0a7c 2063 6172 626f 6e70 6c61     |.| carbonpla
+00000c10: 6e2d 666f 7265 7374 2d6f 6666 7365 7473  n-forest-offsets
+00000c20: 207c 2060 696d 706f 7274 2063 6172 626f   | `import carbo
+00000c30: 6e70 6c61 6e2e 666f 7265 7374 5f6f 6666  nplan.forest_off
+00000c40: 7365 7473 6020 7c20 5b68 7474 7073 3a2f  sets` | [https:/
+00000c50: 2f67 6974 6875 622e 636f 6d2f 6361 7262  /github.com/carb
+00000c60: 6f6e 706c 616e 2f66 6f72 6573 742d 6f66  onplan/forest-of
+00000c70: 6673 6574 735d 2868 7474 7073 3a2f 2f67  fsets](https://g
+00000c80: 6974 6875 622e 636f 6d2f 6361 7262 6f6e  ithub.com/carbon
+00000c90: 706c 616e 2f66 6f72 6573 742d 6f66 6673  plan/forest-offs
+00000ca0: 6574 7329 207c 0a7c 2063 6172 626f 6e70  ets) |.| carbonp
+00000cb0: 6c61 6e2d 666f 7265 7374 2d72 6973 6b73  lan-forest-risks
+00000cc0: 2020 207c 2060 696d 706f 7274 2063 6172     | `import car
+00000cd0: 626f 6e70 6c61 6e2e 666f 7265 7374 5f72  bonplan.forest_r
+00000ce0: 6973 6b73 6020 2020 7c20 5b68 7474 7073  isks`   | [https
+00000cf0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6361  ://github.com/ca
+00000d00: 7262 6f6e 706c 616e 2f66 6f72 6573 742d  rbonplan/forest-
+00000d10: 7269 736b 735d 2868 7474 7073 3a2f 2f67  risks](https://g
+00000d20: 6974 6875 622e 636f 6d2f 6361 7262 6f6e  ithub.com/carbon
+00000d30: 706c 616e 2f66 6f72 6573 742d 7269 736b  plan/forest-risk
+00000d40: 7329 2020 2020 207c 0a7c 2063 6172 626f  s)     |.| carbo
+00000d50: 6e70 6c61 6e2d 7374 796c 6573 2020 2020  nplan-styles    
+00000d60: 2020 2020 207c 2060 696d 706f 7274 2063       | `import c
+00000d70: 6172 626f 6e70 6c61 6e2e 7374 796c 6573  arbonplan.styles
+00000d80: 6020 2020 2020 2020 2020 7c20 5b68 7474  `         | [htt
+00000d90: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000da0: 6361 7262 6f6e 706c 616e 2f73 7479 6c65  carbonplan/style
+00000db0: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
+00000dc0: 622e 636f 6d2f 6361 7262 6f6e 706c 616e  b.com/carbonplan
+00000dd0: 2f73 7479 6c65 7329 2020 2020 2020 2020  /styles)        
+00000de0: 2020 2020 2020 2020 207c 0a0a 2323 2069           |..## i
+00000df0: 6e73 7461 6c6c 0a0a 6060 6073 6865 6c6c  nstall..```shell
+00000e00: 0a70 6970 2069 6e73 7461 6c6c 2063 6172  .pip install car
+00000e10: 626f 6e70 6c61 6e5b 616c 6c5d 0a23 206f  bonplan[all].# o
+00000e20: 7220 696e 6469 7669 6475 616c 2073 7562  r individual sub
+00000e30: 2070 6163 6b61 6765 730a 7069 7020 696e   packages.pip in
+00000e40: 7374 616c 6c20 6361 7262 6f6e 706c 616e  stall carbonplan
+00000e50: 5b73 7479 6c65 735d 0a60 6060 0a0a 2323  [styles].```..##
+00000e60: 2075 7361 6765 0a0a 6060 6070 7974 686f   usage..```pytho
+00000e70: 6e0a 6672 6f6d 2063 6172 626f 6e70 6c61  n.from carbonpla
+00000e80: 6e2e 7374 796c 6573 2e6d 706c 2069 6d70  n.styles.mpl imp
+00000e90: 6f72 7420 7365 745f 7468 656d 650a 2320  ort set_theme.# 
+00000ea0: 7468 6973 2069 7320 7468 6520 7361 6d65  this is the same
+00000eb0: 2074 6869 6e67 7320 6173 0a66 726f 6d20   things as.from 
+00000ec0: 6361 7262 6f6e 706c 616e 5f73 7479 6c65  carbonplan_style
+00000ed0: 732e 6d70 6c20 696d 706f 7274 2073 6574  s.mpl import set
+00000ee0: 5f74 6865 6d65 0a60 6060 0a0a 2323 206c  _theme.```..## l
+00000ef0: 6963 656e 7365 0a0a 416c 6c20 7468 6520  icense..All the 
+00000f00: 636f 6465 2069 6e20 7468 6973 2072 6570  code in this rep
+00000f10: 6f73 6974 6f72 7920 6973 205b 4d49 545d  ository is [MIT]
+00000f20: 2868 7474 7073 3a2f 2f63 686f 6f73 6561  (https://choosea
+00000f30: 6c69 6365 6e73 652e 636f 6d2f 6c69 6365  license.com/lice
+00000f40: 6e73 6573 2f6d 6974 2f29 2d6c 6963 656e  nses/mit/)-licen
+00000f50: 7365 642e 2057 6520 696e 636c 7564 6520  sed. We include 
+00000f60: 6174 7472 6962 7574 696f 6e20 666f 7220  attribution for 
+00000f70: 7468 6973 2063 6f6e 7465 6e74 2c20 616e  this content, an
+00000f80: 6420 7765 2070 6c65 6173 6520 7265 7175  d we please requ
+00000f90: 6573 7420 7468 6174 2079 6f75 2061 6c73  est that you als
+00000fa0: 6f20 6d61 696e 7461 696e 2074 6861 7420  o maintain that 
+00000fb0: 6174 7472 6962 7574 696f 6e20 6966 2075  attribution if u
+00000fc0: 7369 6e67 2074 6869 7320 6461 7461 2e0a  sing this data..
+00000fd0: 0a23 2320 6162 6f75 7420 7573 0a0a 4361  .## about us..Ca
+00000fe0: 7262 6f6e 506c 616e 2069 7320 6120 6e6f  rbonPlan is a no
+00000ff0: 6e70 726f 6669 7420 6f72 6761 6e69 7a61  nprofit organiza
+00001000: 7469 6f6e 2074 6861 7420 7573 6573 2064  tion that uses d
+00001010: 6174 6120 616e 6420 7363 6965 6e63 6520  ata and science 
+00001020: 666f 7220 636c 696d 6174 6520 6163 7469  for climate acti
+00001030: 6f6e 2e20 5765 2061 696d 2074 6f20 696d  on. We aim to im
+00001040: 7072 6f76 6520 7468 6520 7472 616e 7370  prove the transp
+00001050: 6172 656e 6379 2061 6e64 2073 6369 656e  arency and scien
+00001060: 7469 6669 6320 696e 7465 6772 6974 7920  tific integrity 
+00001070: 6f66 2063 6c69 6d61 7465 2073 6f6c 7574  of climate solut
+00001080: 696f 6e73 2077 6974 6820 6f70 656e 2064  ions with open d
+00001090: 6174 6120 616e 6420 746f 6f6c 732e 2046  ata and tools. F
+000010a0: 696e 6420 6f75 7420 6d6f 7265 2061 7420  ind out more at 
+000010b0: 5b63 6172 626f 6e70 6c61 6e2e 6f72 675d  [carbonplan.org]
+000010c0: 2868 7474 7073 3a2f 2f63 6172 626f 6e70  (https://carbonp
+000010d0: 6c61 6e2e 6f72 672f 2920 6f72 2067 6574  lan.org/) or get
+000010e0: 2069 6e20 746f 7563 6820 6279 205b 6f70   in touch by [op
+000010f0: 656e 696e 6720 616e 2069 7373 7565 5d28  ening an issue](
+00001100: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001110: 6f6d 2f63 6172 626f 6e70 6c61 6e2f 6361  om/carbonplan/ca
+00001120: 7262 6f6e 706c 616e 2d70 7974 686f 6e2f  rbonplan-python/
+00001130: 6973 7375 6573 2f6e 6577 2920 6f72 205b  issues/new) or [
+00001140: 7365 6e64 696e 6720 7573 2061 6e20 656d  sending us an em
+00001150: 6169 6c5d 286d 6169 6c74 6f3a 6865 6c6c  ail](mailto:hell
+00001160: 6f40 6361 7262 6f6e 706c 616e 2e6f 7267  o@carbonplan.org
+00001170: 292e 0a                                  )..
```

### Comparing `carbonplan-0.5.0/README.md` & `carbonplan-0.6.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,173 +1,180 @@
-00000000: 3c69 6d67 0a20 2073 7263 3d27 6874 7470  <img.  src='http
-00000010: 733a 2f2f 6361 7262 6f6e 706c 616e 2d61  s://carbonplan-a
-00000020: 7373 6574 732e 7333 2e61 6d61 7a6f 6e61  ssets.s3.amazona
-00000030: 7773 2e63 6f6d 2f6d 6f6e 6f67 7261 6d2f  ws.com/monogram/
-00000040: 6461 726b 2d73 6d61 6c6c 2e70 6e67 270a  dark-small.png'.
-00000050: 2020 6865 6967 6874 3d27 3438 270a 2f3e    height='48'./>
-00000060: 0a0a 2320 6361 7262 6f6e 706c 616e 202f  ..# carbonplan /
-00000070: 2063 6172 626f 6e70 6c61 6e2d 7079 7468   carbonplan-pyth
-00000080: 6f6e 0a0a 2a2a 6e61 6d65 7370 6163 6520  on..**namespace 
-00000090: 7061 636b 6167 6520 666f 7220 7079 7468  package for pyth
-000000a0: 6f6e 2075 7469 6c69 7469 6573 2061 6e64  on utilities and
-000000b0: 2073 7562 7072 6f6a 6563 7473 2a2a 0a0a   subprojects**..
-000000c0: 5b21 5b43 495d 2868 7474 7073 3a2f 2f67  [![CI](https://g
-000000d0: 6974 6875 622e 636f 6d2f 6361 7262 6f6e  ithub.com/carbon
-000000e0: 706c 616e 2f63 6172 626f 6e70 6c61 6e2d  plan/carbonplan-
-000000f0: 7079 7468 6f6e 2f61 6374 696f 6e73 2f77  python/actions/w
-00000100: 6f72 6b66 6c6f 7773 2f6d 6169 6e2e 7961  orkflows/main.ya
-00000110: 6d6c 2f62 6164 6765 2e73 7667 295d 2868  ml/badge.svg)](h
-00000120: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000130: 6d2f 6361 7262 6f6e 706c 616e 2f63 6172  m/carbonplan/car
-00000140: 626f 6e70 6c61 6e2d 7079 7468 6f6e 2f61  bonplan-python/a
-00000150: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
-00000160: 2f6d 6169 6e2e 7961 6d6c 290a 215b 4d49  /main.yaml).![MI
-00000170: 5420 4c69 6365 6e73 655d 5b5d 0a5b 215b  T License][].[![
-00000180: 5079 5049 2076 6572 7369 6f6e 5d28 6874  PyPI version](ht
-00000190: 7470 733a 2f2f 6261 6467 652e 6675 7279  tps://badge.fury
-000001a0: 2e69 6f2f 7079 2f63 6172 626f 6e70 6c61  .io/py/carbonpla
-000001b0: 6e2e 7376 6729 5d28 6874 7470 733a 2f2f  n.svg)](https://
-000001c0: 6261 6467 652e 6675 7279 2e69 6f2f 7079  badge.fury.io/py
-000001d0: 2f63 6172 626f 6e70 6c61 6e29 0a0a 5b67  /carbonplan)..[g
-000001e0: 6974 6875 622d 6261 6467 655d 3a20 6874  ithub-badge]: ht
-000001f0: 7470 733a 2f2f 6261 6467 656e 2e6e 6574  tps://badgen.net
-00000200: 2f62 6164 6765 2f2d 2f67 6974 6875 623f  /badge/-/github?
-00000210: 6963 6f6e 3d67 6974 6875 6226 6c61 6265  icon=github&labe
-00000220: 6c0a 5b6d 6974 206c 6963 656e 7365 5d3a  l.[mit license]:
-00000230: 2068 7474 7073 3a2f 2f62 6164 6765 6e2e   https://badgen.
-00000240: 6e65 742f 6261 6467 652f 6c69 6365 6e73  net/badge/licens
-00000250: 652f 4d49 542f 626c 7565 0a0a 5468 6973  e/MIT/blue..This
-00000260: 2072 6570 6f73 6974 6f72 7920 696e 636c   repository incl
-00000270: 7564 6573 2074 6865 2060 6361 7262 6f6e  udes the `carbon
-00000280: 706c 616e 6020 6e61 6d65 7370 6163 6520  plan` namespace 
-00000290: 5079 7468 6f6e 2070 6163 6b61 6765 2e20  Python package. 
-000002a0: 5468 6520 7061 636b 6167 6520 6974 7365  The package itse
-000002b0: 6c66 2069 6e63 6c75 6465 7320 7665 7279  lf includes very
-000002c0: 206c 6974 746c 6520 6f66 2073 7562 7374   little of subst
-000002d0: 616e 6365 2c20 616e 6420 6973 2064 6973  ance, and is dis
-000002e0: 7472 6962 7574 6564 2074 6f20 6163 7420  tributed to act 
-000002f0: 6173 2074 6865 2074 6f70 2d6c 6576 656c  as the top-level
-00000300: 206e 616d 6573 7061 6365 2066 6f72 206f   namespace for o
-00000310: 7468 6572 2050 7974 686f 6e20 7061 636b  ther Python pack
-00000320: 6167 6573 2064 6576 656c 6f70 6564 2062  ages developed b
-00000330: 7920 4361 7262 6f6e 506c 616e 2e20 4f74  y CarbonPlan. Ot
-00000340: 6865 7220 7061 636b 6167 6573 2069 6e63  her packages inc
-00000350: 6c75 6465 3a0a 0a7c 2050 6163 6b61 6765  lude:..| Package
-00000360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000370: 2020 207c 2049 6d70 6f72 7420 2020 2020     | Import     
-00000380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000390: 2020 2020 2020 2020 7c20 4769 7448 7562          | GitHub
-000003a0: 2052 6570 6f20 2020 2020 2020 2020 2020   Repo           
-000003b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003f0: 2020 2020 2020 207c 0a7c 202d 2d2d 2d2d         |.| -----
-00000400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000410: 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d 2d2d  ---- | ---------
-00000420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000430: 2d2d 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d  --------- | ----
-00000440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000450: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000470: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000490: 2d2d 2d2d 2d2d 2d2d 207c 0a7c 2063 6172  -------- |.| car
-000004a0: 626f 6e70 6c61 6e2d 6461 7461 2020 2020  bonplan-data    
-000004b0: 2020 2020 2020 207c 2060 696d 706f 7274         | `import
-000004c0: 2063 6172 626f 6e70 6c61 6e2e 6461 7461   carbonplan.data
-000004d0: 6020 2020 2020 2020 2020 2020 7c20 5b68  `           | [h
-000004e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000004f0: 6d2f 6361 7262 6f6e 706c 616e 2f64 6174  m/carbonplan/dat
-00000500: 615d 2868 7474 7073 3a2f 2f67 6974 6875  a](https://githu
-00000510: 622e 636f 6d2f 6361 7262 6f6e 706c 616e  b.com/carbonplan
-00000520: 2f64 6174 6129 2020 2020 2020 2020 2020  /data)          
-00000530: 2020 2020 2020 2020 2020 207c 0a7c 2063             |.| c
-00000540: 6172 626f 6e70 6c61 6e2d 666f 7265 7374  arbonplan-forest
-00000550: 2d6f 6666 7365 7473 207c 2060 696d 706f  -offsets | `impo
-00000560: 7274 2063 6172 626f 6e70 6c61 6e2e 666f  rt carbonplan.fo
-00000570: 7265 7374 5f6f 6666 7365 7473 6020 7c20  rest_offsets` | 
-00000580: 5b68 7474 7073 3a2f 2f67 6974 6875 622e  [https://github.
-00000590: 636f 6d2f 6361 7262 6f6e 706c 616e 2f66  com/carbonplan/f
-000005a0: 6f72 6573 742d 6f66 6673 6574 735d 2868  orest-offsets](h
-000005b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000005c0: 6d2f 6361 7262 6f6e 706c 616e 2f66 6f72  m/carbonplan/for
-000005d0: 6573 742d 6f66 6673 6574 7329 207c 0a7c  est-offsets) |.|
-000005e0: 2063 6172 626f 6e70 6c61 6e2d 666f 7265   carbonplan-fore
-000005f0: 7374 2d72 6973 6b73 2020 207c 2060 696d  st-risks   | `im
-00000600: 706f 7274 2063 6172 626f 6e70 6c61 6e2e  port carbonplan.
-00000610: 666f 7265 7374 5f72 6973 6b73 6020 2020  forest_risks`   
-00000620: 7c20 5b68 7474 7073 3a2f 2f67 6974 6875  | [https://githu
-00000630: 622e 636f 6d2f 6361 7262 6f6e 706c 616e  b.com/carbonplan
-00000640: 2f66 6f72 6573 742d 7269 736b 735d 2868  /forest-risks](h
-00000650: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000660: 6d2f 6361 7262 6f6e 706c 616e 2f66 6f72  m/carbonplan/for
-00000670: 6573 742d 7269 736b 7329 2020 2020 207c  est-risks)     |
-00000680: 0a7c 2063 6172 626f 6e70 6c61 6e2d 7374  .| carbonplan-st
-00000690: 796c 6573 2020 2020 2020 2020 207c 2060  yles         | `
-000006a0: 696d 706f 7274 2063 6172 626f 6e70 6c61  import carbonpla
-000006b0: 6e2e 7374 796c 6573 6020 2020 2020 2020  n.styles`       
-000006c0: 2020 7c20 5b68 7474 7073 3a2f 2f67 6974    | [https://git
-000006d0: 6875 622e 636f 6d2f 6361 7262 6f6e 706c  hub.com/carbonpl
-000006e0: 616e 2f73 7479 6c65 735d 2868 7474 7073  an/styles](https
-000006f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6361  ://github.com/ca
-00000700: 7262 6f6e 706c 616e 2f73 7479 6c65 7329  rbonplan/styles)
-00000710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000720: 207c 0a0a 2323 2069 6e73 7461 6c6c 0a0a   |..## install..
-00000730: 6060 6073 6865 6c6c 0a70 6970 2069 6e73  ```shell.pip ins
-00000740: 7461 6c6c 2063 6172 626f 6e70 6c61 6e5b  tall carbonplan[
-00000750: 616c 6c5d 0a23 206f 7220 696e 6469 7669  all].# or indivi
-00000760: 6475 616c 2073 7562 2070 6163 6b61 6765  dual sub package
-00000770: 730a 7069 7020 696e 7374 616c 6c20 6361  s.pip install ca
-00000780: 7262 6f6e 706c 616e 5b73 7479 6c65 735d  rbonplan[styles]
-00000790: 0a60 6060 0a0a 2323 2075 7361 6765 0a0a  .```..## usage..
-000007a0: 6060 6070 7974 686f 6e0a 6672 6f6d 2063  ```python.from c
-000007b0: 6172 626f 6e70 6c61 6e2e 7374 796c 6573  arbonplan.styles
-000007c0: 2e6d 706c 2069 6d70 6f72 7420 7365 745f  .mpl import set_
-000007d0: 7468 656d 650a 2320 7468 6973 2069 7320  theme.# this is 
-000007e0: 7468 6520 7361 6d65 2074 6869 6e67 7320  the same things 
-000007f0: 6173 0a66 726f 6d20 6361 7262 6f6e 706c  as.from carbonpl
-00000800: 616e 5f73 7479 6c65 732e 6d70 6c20 696d  an_styles.mpl im
-00000810: 706f 7274 2073 6574 5f74 6865 6d65 0a60  port set_theme.`
-00000820: 6060 0a0a 2323 206c 6963 656e 7365 0a0a  ``..## license..
-00000830: 416c 6c20 7468 6520 636f 6465 2069 6e20  All the code in 
-00000840: 7468 6973 2072 6570 6f73 6974 6f72 7920  this repository 
-00000850: 6973 205b 4d49 545d 2868 7474 7073 3a2f  is [MIT](https:/
-00000860: 2f63 686f 6f73 6561 6c69 6365 6e73 652e  /choosealicense.
-00000870: 636f 6d2f 6c69 6365 6e73 6573 2f6d 6974  com/licenses/mit
-00000880: 2f29 206c 6963 656e 7365 642e 2057 6520  /) licensed. We 
-00000890: 696e 636c 7564 6520 6174 7472 6962 7574  include attribut
-000008a0: 696f 6e20 666f 7220 7468 6973 2063 6f6e  ion for this con
-000008b0: 7465 6e74 2c20 616e 6420 7765 2070 6c65  tent, and we ple
-000008c0: 6173 6520 7265 7175 6573 7420 7468 6174  ase request that
-000008d0: 2079 6f75 2061 6c73 6f20 6d61 696e 7461   you also mainta
-000008e0: 696e 2074 6861 7420 6174 7472 6962 7574  in that attribut
-000008f0: 696f 6e20 6966 2075 7369 6e67 2074 6869  ion if using thi
-00000900: 7320 6461 7461 2e0a 0a23 2320 6162 6f75  s data...## abou
-00000910: 7420 7573 0a0a 4361 7262 6f6e 506c 616e  t us..CarbonPlan
-00000920: 2069 7320 6120 6e6f 6e2d 7072 6f66 6974   is a non-profit
-00000930: 206f 7267 616e 697a 6174 696f 6e20 7468   organization th
-00000940: 6174 2075 7365 7320 6461 7461 2061 6e64  at uses data and
-00000950: 2073 6369 656e 6365 2066 6f72 2063 6c69   science for cli
-00000960: 6d61 7465 2061 6374 696f 6e2e 2057 6520  mate action. We 
-00000970: 6169 6d20 746f 2069 6d70 726f 7665 2074  aim to improve t
-00000980: 6865 2074 7261 6e73 7061 7265 6e63 7920  he transparency 
-00000990: 616e 6420 7363 6965 6e74 6966 6963 2069  and scientific i
-000009a0: 6e74 6567 7269 7479 206f 6620 6361 7262  ntegrity of carb
-000009b0: 6f6e 2072 656d 6f76 616c 2061 6e64 2063  on removal and c
-000009c0: 6c69 6d61 7465 2073 6f6c 7574 696f 6e73  limate solutions
-000009d0: 2074 6872 6f75 6768 206f 7065 6e20 6461   through open da
-000009e0: 7461 2061 6e64 2074 6f6f 6c73 2e20 4669  ta and tools. Fi
-000009f0: 6e64 206f 7574 206d 6f72 6520 6174 205b  nd out more at [
-00000a00: 6361 7262 6f6e 706c 616e 2e6f 7267 5d28  carbonplan.org](
-00000a10: 6874 7470 733a 2f2f 6361 7262 6f6e 706c  https://carbonpl
-00000a20: 616e 2e6f 7267 2f29 206f 7220 6765 7420  an.org/) or get 
-00000a30: 696e 2074 6f75 6368 2062 7920 5b6f 7065  in touch by [ope
-00000a40: 6e69 6e67 2061 6e20 6973 7375 655d 2868  ning an issue](h
-00000a50: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000a60: 6d2f 6361 7262 6f6e 706c 616e 2f63 6172  m/carbonplan/car
-00000a70: 626f 6e70 6c61 6e2d 7079 7468 6f6e 2f69  bonplan-python/i
-00000a80: 7373 7565 732f 6e65 7729 206f 7220 5b73  ssues/new) or [s
-00000a90: 656e 6469 6e67 2075 7320 616e 2065 6d61  ending us an ema
-00000aa0: 696c 5d28 6d61 696c 746f 3a68 656c 6c6f  il](mailto:hello
-00000ab0: 4063 6172 626f 6e70 6c61 6e2e 6f72 6729  @carbonplan.org)
-00000ac0: 2e0a                                     ..
+00000000: 3c70 2061 6c69 676e 3d22 6c65 6674 2220  <p align="left" 
+00000010: 3e0a 3c61 2068 7265 663d 2768 7474 7073  >.<a href='https
+00000020: 3a2f 2f63 6172 626f 6e70 6c61 6e2e 6f72  ://carbonplan.or
+00000030: 6727 3e0a 3c70 6963 7475 7265 3e0a 2020  g'>.<picture>.  
+00000040: 3c73 6f75 7263 6520 6d65 6469 613d 2228  <source media="(
+00000050: 7072 6566 6572 732d 636f 6c6f 722d 7363  prefers-color-sc
+00000060: 6865 6d65 3a20 6461 726b 2922 2073 7263  heme: dark)" src
+00000070: 7365 743d 2268 7474 7073 3a2f 2f63 6172  set="https://car
+00000080: 626f 6e70 6c61 6e2d 6173 7365 7473 2e73  bonplan-assets.s
+00000090: 332e 616d 617a 6f6e 6177 732e 636f 6d2f  3.amazonaws.com/
+000000a0: 6d6f 6e6f 6772 616d 2f6c 6967 6874 2d73  monogram/light-s
+000000b0: 6d61 6c6c 2e70 6e67 223e 0a20 203c 696d  mall.png">.  <im
+000000c0: 6720 616c 743d 2243 6172 626f 6e50 6c61  g alt="CarbonPla
+000000d0: 6e20 6d6f 6e6f 6772 616d 2e22 2068 6569  n monogram." hei
+000000e0: 6768 743d 2234 3822 2073 7263 3d22 6874  ght="48" src="ht
+000000f0: 7470 733a 2f2f 6361 7262 6f6e 706c 616e  tps://carbonplan
+00000100: 2d61 7373 6574 732e 7333 2e61 6d61 7a6f  -assets.s3.amazo
+00000110: 6e61 7773 2e63 6f6d 2f6d 6f6e 6f67 7261  naws.com/monogra
+00000120: 6d2f 6461 726b 2d73 6d61 6c6c 2e70 6e67  m/dark-small.png
+00000130: 223e 0a3c 2f70 6963 7475 7265 3e0a 3c2f  ">.</picture>.</
+00000140: 613e 0a3c 2f70 3e0a 0a23 2063 6172 626f  a>.</p>..# carbo
+00000150: 6e70 6c61 6e20 2f20 6361 7262 6f6e 706c  nplan / carbonpl
+00000160: 616e 2d70 7974 686f 6e0a 0a2a 2a6e 616d  an-python..**nam
+00000170: 6573 7061 6365 2070 6163 6b61 6765 2066  espace package f
+00000180: 6f72 2070 7974 686f 6e20 7574 696c 6974  or python utilit
+00000190: 6965 7320 616e 6420 7375 6270 726f 6a65  ies and subproje
+000001a0: 6374 732a 2a0a 0a5b 215b 4349 5d28 6874  cts**..[![CI](ht
+000001b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000001c0: 2f63 6172 626f 6e70 6c61 6e2f 6361 7262  /carbonplan/carb
+000001d0: 6f6e 706c 616e 2d70 7974 686f 6e2f 6163  onplan-python/ac
+000001e0: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
+000001f0: 6d61 696e 2e79 616d 6c2f 6261 6467 652e  main.yaml/badge.
+00000200: 7376 6729 5d28 6874 7470 733a 2f2f 6769  svg)](https://gi
+00000210: 7468 7562 2e63 6f6d 2f63 6172 626f 6e70  thub.com/carbonp
+00000220: 6c61 6e2f 6361 7262 6f6e 706c 616e 2d70  lan/carbonplan-p
+00000230: 7974 686f 6e2f 6163 7469 6f6e 732f 776f  ython/actions/wo
+00000240: 726b 666c 6f77 732f 6d61 696e 2e79 616d  rkflows/main.yam
+00000250: 6c29 0a21 5b50 7950 495d 2868 7474 7073  l).![PyPI](https
+00000260: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000270: 6f2f 7079 7069 2f76 2f63 6172 626f 6e70  o/pypi/v/carbonp
+00000280: 6c61 6e29 0a5b 215b 4c69 6365 6e73 653a  lan).[![License:
+00000290: 204d 4954 5d28 6874 7470 733a 2f2f 696d   MIT](https://im
+000002a0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+000002b0: 6765 2f4c 6963 656e 7365 2d4d 4954 2d62  ge/License-MIT-b
+000002c0: 6c75 652e 7376 6729 5d28 6874 7470 733a  lue.svg)](https:
+000002d0: 2f2f 6f70 656e 736f 7572 6365 2e6f 7267  //opensource.org
+000002e0: 2f6c 6963 656e 7365 732f 4d49 5429 0a0a  /licenses/MIT)..
+000002f0: 5468 6973 2072 6570 6f73 6974 6f72 7920  This repository 
+00000300: 696e 636c 7564 6573 2074 6865 2060 6361  includes the `ca
+00000310: 7262 6f6e 706c 616e 6020 6e61 6d65 7370  rbonplan` namesp
+00000320: 6163 6520 5079 7468 6f6e 2070 6163 6b61  ace Python packa
+00000330: 6765 2e20 5468 6520 7061 636b 6167 6520  ge. The package 
+00000340: 6974 7365 6c66 2069 6e63 6c75 6465 7320  itself includes 
+00000350: 7665 7279 206c 6974 746c 6520 6f66 2073  very little of s
+00000360: 7562 7374 616e 6365 2c20 616e 6420 6973  ubstance, and is
+00000370: 2064 6973 7472 6962 7574 6564 2074 6f20   distributed to 
+00000380: 6163 7420 6173 2074 6865 2074 6f70 2d6c  act as the top-l
+00000390: 6576 656c 206e 616d 6573 7061 6365 2066  evel namespace f
+000003a0: 6f72 206f 7468 6572 2050 7974 686f 6e20  or other Python 
+000003b0: 7061 636b 6167 6573 2064 6576 656c 6f70  packages develop
+000003c0: 6564 2062 7920 4361 7262 6f6e 506c 616e  ed by CarbonPlan
+000003d0: 2e20 4f74 6865 7220 7061 636b 6167 6573  . Other packages
+000003e0: 2069 6e63 6c75 6465 3a0a 0a7c 2050 6163   include:..| Pac
+000003f0: 6b61 6765 2020 2020 2020 2020 2020 2020  kage            
+00000400: 2020 2020 2020 207c 2049 6d70 6f72 7420         | Import 
+00000410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000420: 2020 2020 2020 2020 2020 2020 7c20 4769              | Gi
+00000430: 7448 7562 2052 6570 6f20 2020 2020 2020  tHub Repo       
+00000440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000480: 2020 2020 2020 2020 2020 207c 0a7c 202d             |.| -
+00000490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000004a0: 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d  -------- | -----
+000004b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000004c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c20  ------------- | 
+000004d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000004e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000004f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c 0a7c  ------------ |.|
+00000530: 2063 6172 626f 6e70 6c61 6e2d 6461 7461   carbonplan-data
+00000540: 2020 2020 2020 2020 2020 207c 2060 696d             | `im
+00000550: 706f 7274 2063 6172 626f 6e70 6c61 6e2e  port carbonplan.
+00000560: 6461 7461 6020 2020 2020 2020 2020 2020  data`           
+00000570: 7c20 5b68 7474 7073 3a2f 2f67 6974 6875  | [https://githu
+00000580: 622e 636f 6d2f 6361 7262 6f6e 706c 616e  b.com/carbonplan
+00000590: 2f64 6174 615d 2868 7474 7073 3a2f 2f67  /data](https://g
+000005a0: 6974 6875 622e 636f 6d2f 6361 7262 6f6e  ithub.com/carbon
+000005b0: 706c 616e 2f64 6174 6129 2020 2020 2020  plan/data)      
+000005c0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000005d0: 0a7c 2063 6172 626f 6e70 6c61 6e2d 666f  .| carbonplan-fo
+000005e0: 7265 7374 2d6f 6666 7365 7473 207c 2060  rest-offsets | `
+000005f0: 696d 706f 7274 2063 6172 626f 6e70 6c61  import carbonpla
+00000600: 6e2e 666f 7265 7374 5f6f 6666 7365 7473  n.forest_offsets
+00000610: 6020 7c20 5b68 7474 7073 3a2f 2f67 6974  ` | [https://git
+00000620: 6875 622e 636f 6d2f 6361 7262 6f6e 706c  hub.com/carbonpl
+00000630: 616e 2f66 6f72 6573 742d 6f66 6673 6574  an/forest-offset
+00000640: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
+00000650: 622e 636f 6d2f 6361 7262 6f6e 706c 616e  b.com/carbonplan
+00000660: 2f66 6f72 6573 742d 6f66 6673 6574 7329  /forest-offsets)
+00000670: 207c 0a7c 2063 6172 626f 6e70 6c61 6e2d   |.| carbonplan-
+00000680: 666f 7265 7374 2d72 6973 6b73 2020 207c  forest-risks   |
+00000690: 2060 696d 706f 7274 2063 6172 626f 6e70   `import carbonp
+000006a0: 6c61 6e2e 666f 7265 7374 5f72 6973 6b73  lan.forest_risks
+000006b0: 6020 2020 7c20 5b68 7474 7073 3a2f 2f67  `   | [https://g
+000006c0: 6974 6875 622e 636f 6d2f 6361 7262 6f6e  ithub.com/carbon
+000006d0: 706c 616e 2f66 6f72 6573 742d 7269 736b  plan/forest-risk
+000006e0: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
+000006f0: 622e 636f 6d2f 6361 7262 6f6e 706c 616e  b.com/carbonplan
+00000700: 2f66 6f72 6573 742d 7269 736b 7329 2020  /forest-risks)  
+00000710: 2020 207c 0a7c 2063 6172 626f 6e70 6c61     |.| carbonpla
+00000720: 6e2d 7374 796c 6573 2020 2020 2020 2020  n-styles        
+00000730: 207c 2060 696d 706f 7274 2063 6172 626f   | `import carbo
+00000740: 6e70 6c61 6e2e 7374 796c 6573 6020 2020  nplan.styles`   
+00000750: 2020 2020 2020 7c20 5b68 7474 7073 3a2f        | [https:/
+00000760: 2f67 6974 6875 622e 636f 6d2f 6361 7262  /github.com/carb
+00000770: 6f6e 706c 616e 2f73 7479 6c65 735d 2868  onplan/styles](h
+00000780: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000790: 6d2f 6361 7262 6f6e 706c 616e 2f73 7479  m/carbonplan/sty
+000007a0: 6c65 7329 2020 2020 2020 2020 2020 2020  les)            
+000007b0: 2020 2020 207c 0a0a 2323 2069 6e73 7461       |..## insta
+000007c0: 6c6c 0a0a 6060 6073 6865 6c6c 0a70 6970  ll..```shell.pip
+000007d0: 2069 6e73 7461 6c6c 2063 6172 626f 6e70   install carbonp
+000007e0: 6c61 6e5b 616c 6c5d 0a23 206f 7220 696e  lan[all].# or in
+000007f0: 6469 7669 6475 616c 2073 7562 2070 6163  dividual sub pac
+00000800: 6b61 6765 730a 7069 7020 696e 7374 616c  kages.pip instal
+00000810: 6c20 6361 7262 6f6e 706c 616e 5b73 7479  l carbonplan[sty
+00000820: 6c65 735d 0a60 6060 0a0a 2323 2075 7361  les].```..## usa
+00000830: 6765 0a0a 6060 6070 7974 686f 6e0a 6672  ge..```python.fr
+00000840: 6f6d 2063 6172 626f 6e70 6c61 6e2e 7374  om carbonplan.st
+00000850: 796c 6573 2e6d 706c 2069 6d70 6f72 7420  yles.mpl import 
+00000860: 7365 745f 7468 656d 650a 2320 7468 6973  set_theme.# this
+00000870: 2069 7320 7468 6520 7361 6d65 2074 6869   is the same thi
+00000880: 6e67 7320 6173 0a66 726f 6d20 6361 7262  ngs as.from carb
+00000890: 6f6e 706c 616e 5f73 7479 6c65 732e 6d70  onplan_styles.mp
+000008a0: 6c20 696d 706f 7274 2073 6574 5f74 6865  l import set_the
+000008b0: 6d65 0a60 6060 0a0a 2323 206c 6963 656e  me.```..## licen
+000008c0: 7365 0a0a 416c 6c20 7468 6520 636f 6465  se..All the code
+000008d0: 2069 6e20 7468 6973 2072 6570 6f73 6974   in this reposit
+000008e0: 6f72 7920 6973 205b 4d49 545d 2868 7474  ory is [MIT](htt
+000008f0: 7073 3a2f 2f63 686f 6f73 6561 6c69 6365  ps://choosealice
+00000900: 6e73 652e 636f 6d2f 6c69 6365 6e73 6573  nse.com/licenses
+00000910: 2f6d 6974 2f29 2d6c 6963 656e 7365 642e  /mit/)-licensed.
+00000920: 2057 6520 696e 636c 7564 6520 6174 7472   We include attr
+00000930: 6962 7574 696f 6e20 666f 7220 7468 6973  ibution for this
+00000940: 2063 6f6e 7465 6e74 2c20 616e 6420 7765   content, and we
+00000950: 2070 6c65 6173 6520 7265 7175 6573 7420   please request 
+00000960: 7468 6174 2079 6f75 2061 6c73 6f20 6d61  that you also ma
+00000970: 696e 7461 696e 2074 6861 7420 6174 7472  intain that attr
+00000980: 6962 7574 696f 6e20 6966 2075 7369 6e67  ibution if using
+00000990: 2074 6869 7320 6461 7461 2e0a 0a23 2320   this data...## 
+000009a0: 6162 6f75 7420 7573 0a0a 4361 7262 6f6e  about us..Carbon
+000009b0: 506c 616e 2069 7320 6120 6e6f 6e70 726f  Plan is a nonpro
+000009c0: 6669 7420 6f72 6761 6e69 7a61 7469 6f6e  fit organization
+000009d0: 2074 6861 7420 7573 6573 2064 6174 6120   that uses data 
+000009e0: 616e 6420 7363 6965 6e63 6520 666f 7220  and science for 
+000009f0: 636c 696d 6174 6520 6163 7469 6f6e 2e20  climate action. 
+00000a00: 5765 2061 696d 2074 6f20 696d 7072 6f76  We aim to improv
+00000a10: 6520 7468 6520 7472 616e 7370 6172 656e  e the transparen
+00000a20: 6379 2061 6e64 2073 6369 656e 7469 6669  cy and scientifi
+00000a30: 6320 696e 7465 6772 6974 7920 6f66 2063  c integrity of c
+00000a40: 6c69 6d61 7465 2073 6f6c 7574 696f 6e73  limate solutions
+00000a50: 2077 6974 6820 6f70 656e 2064 6174 6120   with open data 
+00000a60: 616e 6420 746f 6f6c 732e 2046 696e 6420  and tools. Find 
+00000a70: 6f75 7420 6d6f 7265 2061 7420 5b63 6172  out more at [car
+00000a80: 626f 6e70 6c61 6e2e 6f72 675d 2868 7474  bonplan.org](htt
+00000a90: 7073 3a2f 2f63 6172 626f 6e70 6c61 6e2e  ps://carbonplan.
+00000aa0: 6f72 672f 2920 6f72 2067 6574 2069 6e20  org/) or get in 
+00000ab0: 746f 7563 6820 6279 205b 6f70 656e 696e  touch by [openin
+00000ac0: 6720 616e 2069 7373 7565 5d28 6874 7470  g an issue](http
+00000ad0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
+00000ae0: 6172 626f 6e70 6c61 6e2f 6361 7262 6f6e  arbonplan/carbon
+00000af0: 706c 616e 2d70 7974 686f 6e2f 6973 7375  plan-python/issu
+00000b00: 6573 2f6e 6577 2920 6f72 205b 7365 6e64  es/new) or [send
+00000b10: 696e 6720 7573 2061 6e20 656d 6169 6c5d  ing us an email]
+00000b20: 286d 6169 6c74 6f3a 6865 6c6c 6f40 6361  (mailto:hello@ca
+00000b30: 7262 6f6e 706c 616e 2e6f 7267 292e 0a    rbonplan.org)..
```

### Comparing `carbonplan-0.5.0/carbonplan/data.py` & `carbonplan-0.6.0/carbonplan/data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa
 import warnings
 
 try:
     with warnings.catch_warnings():
-        warnings.filterwarnings('ignore', category=DeprecationWarning, module='intake')
-        warnings.filterwarnings('ignore', category=PendingDeprecationWarning, module='intake')
+        warnings.filterwarnings("ignore", category=DeprecationWarning, module="intake")
+        warnings.filterwarnings("ignore", category=PendingDeprecationWarning, module="intake")
         from carbonplan_data import *
 except ImportError as e:
     msg = (
         "CarbonPlan's Data package is not installed.\n\n"
-        'Please install the carbonplan-data package:\n\n'
+        "Please install the carbonplan-data package:\n\n"
         '  python -m pip install "carbonplan-data"'
     )
     raise ImportError(msg) from e
```

### Comparing `carbonplan-0.5.0/carbonplan.egg-info/PKG-INFO` & `carbonplan-0.6.0/carbonplan.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,251 +1,280 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6361 7262  : 2.1.Name: carb
 00000020: 6f6e 706c 616e 0a56 6572 7369 6f6e 3a20  onplan.Version: 
-00000030: 302e 352e 300a 5375 6d6d 6172 793a 2043  0.5.0.Summary: C
+00000030: 302e 362e 300a 5375 6d6d 6172 793a 2043  0.6.0.Summary: C
 00000040: 6172 626f 6e50 6c61 6e20 6e61 6d65 7370  arbonPlan namesp
-00000050: 6163 6520 7061 636b 6167 650a 486f 6d65  ace package.Home
-00000060: 2d70 6167 653a 2068 7474 7073 3a2f 2f67  -page: https://g
-00000070: 6974 6875 622e 636f 6d2f 6361 7262 6f6e  ithub.com/carbon
-00000080: 706c 616e 2f63 6172 626f 6e70 6c61 6e2d  plan/carbonplan-
-00000090: 7079 7468 6f6e 0a4d 6169 6e74 6169 6e65  python.Maintaine
-000000a0: 723a 204a 6f65 2048 616d 6d61 6e0a 4d61  r: Joe Hamman.Ma
-000000b0: 696e 7461 696e 6572 2d65 6d61 696c 3a20  intainer-email: 
-000000c0: 6a6f 6540 6361 7262 6f6e 706c 616e 2e6f  joe@carbonplan.o
-000000d0: 7267 0a4c 6963 656e 7365 3a20 4d49 540a  rg.License: MIT.
-000000e0: 4465 7363 7269 7074 696f 6e3a 203c 696d  Description: <im
-000000f0: 670a 2020 2020 2020 2020 2020 7372 633d  g.          src=
-00000100: 2768 7474 7073 3a2f 2f63 6172 626f 6e70  'https://carbonp
-00000110: 6c61 6e2d 6173 7365 7473 2e73 332e 616d  lan-assets.s3.am
-00000120: 617a 6f6e 6177 732e 636f 6d2f 6d6f 6e6f  azonaws.com/mono
-00000130: 6772 616d 2f64 6172 6b2d 736d 616c 6c2e  gram/dark-small.
-00000140: 706e 6727 0a20 2020 2020 2020 2020 2068  png'.          h
-00000150: 6569 6768 743d 2734 3827 0a20 2020 2020  eight='48'.     
-00000160: 2020 202f 3e0a 2020 2020 2020 2020 0a20     />.        . 
-00000170: 2020 2020 2020 2023 2063 6172 626f 6e70         # carbonp
-00000180: 6c61 6e20 2f20 6361 7262 6f6e 706c 616e  lan / carbonplan
-00000190: 2d70 7974 686f 6e0a 2020 2020 2020 2020  -python.        
-000001a0: 0a20 2020 2020 2020 202a 2a6e 616d 6573  .        **names
-000001b0: 7061 6365 2070 6163 6b61 6765 2066 6f72  pace package for
-000001c0: 2070 7974 686f 6e20 7574 696c 6974 6965   python utilitie
-000001d0: 7320 616e 6420 7375 6270 726f 6a65 6374  s and subproject
-000001e0: 732a 2a0a 2020 2020 2020 2020 0a20 2020  s**.        .   
-000001f0: 2020 2020 205b 215b 4349 5d28 6874 7470       [![CI](http
-00000200: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
-00000210: 6172 626f 6e70 6c61 6e2f 6361 7262 6f6e  arbonplan/carbon
-00000220: 706c 616e 2d70 7974 686f 6e2f 6163 7469  plan-python/acti
-00000230: 6f6e 732f 776f 726b 666c 6f77 732f 6d61  ons/workflows/ma
-00000240: 696e 2e79 616d 6c2f 6261 6467 652e 7376  in.yaml/badge.sv
-00000250: 6729 5d28 6874 7470 733a 2f2f 6769 7468  g)](https://gith
-00000260: 7562 2e63 6f6d 2f63 6172 626f 6e70 6c61  ub.com/carbonpla
-00000270: 6e2f 6361 7262 6f6e 706c 616e 2d70 7974  n/carbonplan-pyt
-00000280: 686f 6e2f 6163 7469 6f6e 732f 776f 726b  hon/actions/work
-00000290: 666c 6f77 732f 6d61 696e 2e79 616d 6c29  flows/main.yaml)
-000002a0: 0a20 2020 2020 2020 2021 5b4d 4954 204c  .        ![MIT L
-000002b0: 6963 656e 7365 5d5b 5d0a 2020 2020 2020  icense][].      
-000002c0: 2020 5b21 5b50 7950 4920 7665 7273 696f    [![PyPI versio
-000002d0: 6e5d 2868 7474 7073 3a2f 2f62 6164 6765  n](https://badge
-000002e0: 2e66 7572 792e 696f 2f70 792f 6361 7262  .fury.io/py/carb
-000002f0: 6f6e 706c 616e 2e73 7667 295d 2868 7474  onplan.svg)](htt
-00000300: 7073 3a2f 2f62 6164 6765 2e66 7572 792e  ps://badge.fury.
-00000310: 696f 2f70 792f 6361 7262 6f6e 706c 616e  io/py/carbonplan
-00000320: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-00000330: 2020 205b 6769 7468 7562 2d62 6164 6765     [github-badge
-00000340: 5d3a 2068 7474 7073 3a2f 2f62 6164 6765  ]: https://badge
-00000350: 6e2e 6e65 742f 6261 6467 652f 2d2f 6769  n.net/badge/-/gi
-00000360: 7468 7562 3f69 636f 6e3d 6769 7468 7562  thub?icon=github
-00000370: 266c 6162 656c 0a20 2020 2020 2020 205b  &label.        [
-00000380: 6d69 7420 6c69 6365 6e73 655d 3a20 6874  mit license]: ht
-00000390: 7470 733a 2f2f 6261 6467 656e 2e6e 6574  tps://badgen.net
-000003a0: 2f62 6164 6765 2f6c 6963 656e 7365 2f4d  /badge/license/M
-000003b0: 4954 2f62 6c75 650a 2020 2020 2020 2020  IT/blue.        
-000003c0: 0a20 2020 2020 2020 2054 6869 7320 7265  .        This re
-000003d0: 706f 7369 746f 7279 2069 6e63 6c75 6465  pository include
-000003e0: 7320 7468 6520 6063 6172 626f 6e70 6c61  s the `carbonpla
-000003f0: 6e60 206e 616d 6573 7061 6365 2050 7974  n` namespace Pyt
-00000400: 686f 6e20 7061 636b 6167 652e 2054 6865  hon package. The
-00000410: 2070 6163 6b61 6765 2069 7473 656c 6620   package itself 
-00000420: 696e 636c 7564 6573 2076 6572 7920 6c69  includes very li
-00000430: 7474 6c65 206f 6620 7375 6273 7461 6e63  ttle of substanc
-00000440: 652c 2061 6e64 2069 7320 6469 7374 7269  e, and is distri
-00000450: 6275 7465 6420 746f 2061 6374 2061 7320  buted to act as 
-00000460: 7468 6520 746f 702d 6c65 7665 6c20 6e61  the top-level na
-00000470: 6d65 7370 6163 6520 666f 7220 6f74 6865  mespace for othe
-00000480: 7220 5079 7468 6f6e 2070 6163 6b61 6765  r Python package
-00000490: 7320 6465 7665 6c6f 7065 6420 6279 2043  s developed by C
-000004a0: 6172 626f 6e50 6c61 6e2e 204f 7468 6572  arbonPlan. Other
-000004b0: 2070 6163 6b61 6765 7320 696e 636c 7564   packages includ
-000004c0: 653a 0a20 2020 2020 2020 200a 2020 2020  e:.        .    
-000004d0: 2020 2020 7c20 5061 636b 6167 6520 2020      | Package   
-000004e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000004f0: 7c20 496d 706f 7274 2020 2020 2020 2020  | Import        
-00000500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000510: 2020 2020 207c 2047 6974 4875 6220 5265       | GitHub Re
-00000520: 706f 2020 2020 2020 2020 2020 2020 2020  po              
-00000530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000570: 2020 2020 7c0a 2020 2020 2020 2020 7c20      |.        | 
-00000580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000590: 2d2d 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d  --------- | ----
-000005a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000005b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c  -------------- |
-000005c0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
-000005d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000005e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000005f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000600: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c0a  ------------- |.
-00000620: 2020 2020 2020 2020 7c20 6361 7262 6f6e          | carbon
-00000630: 706c 616e 2d64 6174 6120 2020 2020 2020  plan-data       
-00000640: 2020 2020 7c20 6069 6d70 6f72 7420 6361      | `import ca
-00000650: 7262 6f6e 706c 616e 2e64 6174 6160 2020  rbonplan.data`  
-00000660: 2020 2020 2020 2020 207c 205b 6874 7470           | [http
-00000670: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
-00000680: 6172 626f 6e70 6c61 6e2f 6461 7461 5d28  arbonplan/data](
-00000690: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000006a0: 6f6d 2f63 6172 626f 6e70 6c61 6e2f 6461  om/carbonplan/da
-000006b0: 7461 2920 2020 2020 2020 2020 2020 2020  ta)             
-000006c0: 2020 2020 2020 2020 7c0a 2020 2020 2020          |.      
-000006d0: 2020 7c20 6361 7262 6f6e 706c 616e 2d66    | carbonplan-f
-000006e0: 6f72 6573 742d 6f66 6673 6574 7320 7c20  orest-offsets | 
-000006f0: 6069 6d70 6f72 7420 6361 7262 6f6e 706c  `import carbonpl
-00000700: 616e 2e66 6f72 6573 745f 6f66 6673 6574  an.forest_offset
-00000710: 7360 207c 205b 6874 7470 733a 2f2f 6769  s` | [https://gi
-00000720: 7468 7562 2e63 6f6d 2f63 6172 626f 6e70  thub.com/carbonp
-00000730: 6c61 6e2f 666f 7265 7374 2d6f 6666 7365  lan/forest-offse
-00000740: 7473 5d28 6874 7470 733a 2f2f 6769 7468  ts](https://gith
-00000750: 7562 2e63 6f6d 2f63 6172 626f 6e70 6c61  ub.com/carbonpla
-00000760: 6e2f 666f 7265 7374 2d6f 6666 7365 7473  n/forest-offsets
-00000770: 2920 7c0a 2020 2020 2020 2020 7c20 6361  ) |.        | ca
-00000780: 7262 6f6e 706c 616e 2d66 6f72 6573 742d  rbonplan-forest-
-00000790: 7269 736b 7320 2020 7c20 6069 6d70 6f72  risks   | `impor
-000007a0: 7420 6361 7262 6f6e 706c 616e 2e66 6f72  t carbonplan.for
-000007b0: 6573 745f 7269 736b 7360 2020 207c 205b  est_risks`   | [
-000007c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000007d0: 6f6d 2f63 6172 626f 6e70 6c61 6e2f 666f  om/carbonplan/fo
-000007e0: 7265 7374 2d72 6973 6b73 5d28 6874 7470  rest-risks](http
-000007f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
-00000800: 6172 626f 6e70 6c61 6e2f 666f 7265 7374  arbonplan/forest
-00000810: 2d72 6973 6b73 2920 2020 2020 7c0a 2020  -risks)     |.  
-00000820: 2020 2020 2020 7c20 6361 7262 6f6e 706c        | carbonpl
-00000830: 616e 2d73 7479 6c65 7320 2020 2020 2020  an-styles       
-00000840: 2020 7c20 6069 6d70 6f72 7420 6361 7262    | `import carb
-00000850: 6f6e 706c 616e 2e73 7479 6c65 7360 2020  onplan.styles`  
-00000860: 2020 2020 2020 207c 205b 6874 7470 733a         | [https:
-00000870: 2f2f 6769 7468 7562 2e63 6f6d 2f63 6172  //github.com/car
-00000880: 626f 6e70 6c61 6e2f 7374 796c 6573 5d28  bonplan/styles](
-00000890: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000008a0: 6f6d 2f63 6172 626f 6e70 6c61 6e2f 7374  om/carbonplan/st
-000008b0: 796c 6573 2920 2020 2020 2020 2020 2020  yles)           
-000008c0: 2020 2020 2020 7c0a 2020 2020 2020 2020        |.        
-000008d0: 0a20 2020 2020 2020 2023 2320 696e 7374  .        ## inst
-000008e0: 616c 6c0a 2020 2020 2020 2020 0a20 2020  all.        .   
-000008f0: 2020 2020 2060 6060 7368 656c 6c0a 2020       ```shell.  
-00000900: 2020 2020 2020 7069 7020 696e 7374 616c        pip instal
-00000910: 6c20 6361 7262 6f6e 706c 616e 5b61 6c6c  l carbonplan[all
-00000920: 5d0a 2020 2020 2020 2020 2320 6f72 2069  ].        # or i
-00000930: 6e64 6976 6964 7561 6c20 7375 6220 7061  ndividual sub pa
-00000940: 636b 6167 6573 0a20 2020 2020 2020 2070  ckages.        p
-00000950: 6970 2069 6e73 7461 6c6c 2063 6172 626f  ip install carbo
-00000960: 6e70 6c61 6e5b 7374 796c 6573 5d0a 2020  nplan[styles].  
-00000970: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
-00000980: 2020 0a20 2020 2020 2020 2023 2320 7573    .        ## us
-00000990: 6167 650a 2020 2020 2020 2020 0a20 2020  age.        .   
-000009a0: 2020 2020 2060 6060 7079 7468 6f6e 0a20       ```python. 
-000009b0: 2020 2020 2020 2066 726f 6d20 6361 7262         from carb
-000009c0: 6f6e 706c 616e 2e73 7479 6c65 732e 6d70  onplan.styles.mp
-000009d0: 6c20 696d 706f 7274 2073 6574 5f74 6865  l import set_the
-000009e0: 6d65 0a20 2020 2020 2020 2023 2074 6869  me.        # thi
-000009f0: 7320 6973 2074 6865 2073 616d 6520 7468  s is the same th
-00000a00: 696e 6773 2061 730a 2020 2020 2020 2020  ings as.        
-00000a10: 6672 6f6d 2063 6172 626f 6e70 6c61 6e5f  from carbonplan_
-00000a20: 7374 796c 6573 2e6d 706c 2069 6d70 6f72  styles.mpl impor
-00000a30: 7420 7365 745f 7468 656d 650a 2020 2020  t set_theme.    
-00000a40: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
-00000a50: 0a20 2020 2020 2020 2023 2320 6c69 6365  .        ## lice
-00000a60: 6e73 650a 2020 2020 2020 2020 0a20 2020  nse.        .   
-00000a70: 2020 2020 2041 6c6c 2074 6865 2063 6f64       All the cod
-00000a80: 6520 696e 2074 6869 7320 7265 706f 7369  e in this reposi
-00000a90: 746f 7279 2069 7320 5b4d 4954 5d28 6874  tory is [MIT](ht
-00000aa0: 7470 733a 2f2f 6368 6f6f 7365 616c 6963  tps://choosealic
-00000ab0: 656e 7365 2e63 6f6d 2f6c 6963 656e 7365  ense.com/license
-00000ac0: 732f 6d69 742f 2920 6c69 6365 6e73 6564  s/mit/) licensed
-00000ad0: 2e20 5765 2069 6e63 6c75 6465 2061 7474  . We include att
-00000ae0: 7269 6275 7469 6f6e 2066 6f72 2074 6869  ribution for thi
-00000af0: 7320 636f 6e74 656e 742c 2061 6e64 2077  s content, and w
-00000b00: 6520 706c 6561 7365 2072 6571 7565 7374  e please request
-00000b10: 2074 6861 7420 796f 7520 616c 736f 206d   that you also m
-00000b20: 6169 6e74 6169 6e20 7468 6174 2061 7474  aintain that att
-00000b30: 7269 6275 7469 6f6e 2069 6620 7573 696e  ribution if usin
-00000b40: 6720 7468 6973 2064 6174 612e 0a20 2020  g this data..   
-00000b50: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
-00000b60: 2061 626f 7574 2075 730a 2020 2020 2020   about us.      
-00000b70: 2020 0a20 2020 2020 2020 2043 6172 626f    .        Carbo
-00000b80: 6e50 6c61 6e20 6973 2061 206e 6f6e 2d70  nPlan is a non-p
-00000b90: 726f 6669 7420 6f72 6761 6e69 7a61 7469  rofit organizati
-00000ba0: 6f6e 2074 6861 7420 7573 6573 2064 6174  on that uses dat
-00000bb0: 6120 616e 6420 7363 6965 6e63 6520 666f  a and science fo
-00000bc0: 7220 636c 696d 6174 6520 6163 7469 6f6e  r climate action
-00000bd0: 2e20 5765 2061 696d 2074 6f20 696d 7072  . We aim to impr
-00000be0: 6f76 6520 7468 6520 7472 616e 7370 6172  ove the transpar
-00000bf0: 656e 6379 2061 6e64 2073 6369 656e 7469  ency and scienti
-00000c00: 6669 6320 696e 7465 6772 6974 7920 6f66  fic integrity of
-00000c10: 2063 6172 626f 6e20 7265 6d6f 7661 6c20   carbon removal 
-00000c20: 616e 6420 636c 696d 6174 6520 736f 6c75  and climate solu
-00000c30: 7469 6f6e 7320 7468 726f 7567 6820 6f70  tions through op
-00000c40: 656e 2064 6174 6120 616e 6420 746f 6f6c  en data and tool
-00000c50: 732e 2046 696e 6420 6f75 7420 6d6f 7265  s. Find out more
-00000c60: 2061 7420 5b63 6172 626f 6e70 6c61 6e2e   at [carbonplan.
-00000c70: 6f72 675d 2868 7474 7073 3a2f 2f63 6172  org](https://car
-00000c80: 626f 6e70 6c61 6e2e 6f72 672f 2920 6f72  bonplan.org/) or
-00000c90: 2067 6574 2069 6e20 746f 7563 6820 6279   get in touch by
-00000ca0: 205b 6f70 656e 696e 6720 616e 2069 7373   [opening an iss
-00000cb0: 7565 5d28 6874 7470 733a 2f2f 6769 7468  ue](https://gith
-00000cc0: 7562 2e63 6f6d 2f63 6172 626f 6e70 6c61  ub.com/carbonpla
-00000cd0: 6e2f 6361 7262 6f6e 706c 616e 2d70 7974  n/carbonplan-pyt
-00000ce0: 686f 6e2f 6973 7375 6573 2f6e 6577 2920  hon/issues/new) 
-00000cf0: 6f72 205b 7365 6e64 696e 6720 7573 2061  or [sending us a
-00000d00: 6e20 656d 6169 6c5d 286d 6169 6c74 6f3a  n email](mailto:
-00000d10: 6865 6c6c 6f40 6361 7262 6f6e 706c 616e  hello@carbonplan
-00000d20: 2e6f 7267 292e 0a20 2020 2020 2020 200a  .org)..        .
-00000d30: 506c 6174 666f 726d 3a20 554e 4b4e 4f57  Platform: UNKNOW
-00000d40: 4e0a 436c 6173 7369 6669 6572 3a20 4465  N.Classifier: De
-00000d50: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
-00000d60: 203a 3a20 3220 2d20 5072 652d 416c 7068   :: 2 - Pre-Alph
-00000d70: 610a 436c 6173 7369 6669 6572 3a20 4c69  a.Classifier: Li
-00000d80: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
-00000d90: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
-00000da0: 656e 7365 0a43 6c61 7373 6966 6965 723a  ense.Classifier:
-00000db0: 204f 7065 7261 7469 6e67 2053 7973 7465   Operating Syste
-00000dc0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
-00000dd0: 656e 740a 436c 6173 7369 6669 6572 3a20  ent.Classifier: 
-00000de0: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
-00000df0: 6520 3a3a 2053 6369 656e 6365 2f52 6573  e :: Science/Res
-00000e00: 6561 7263 680a 436c 6173 7369 6669 6572  earch.Classifier
-00000e10: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000e20: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000e30: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000e40: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000e50: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000e60: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000e70: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000e80: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000e90: 2e38 0a43 6c61 7373 6966 6965 723a 2050  .8.Classifier: P
-00000ea0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000eb0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000ec0: 2033 2e39 0a43 6c61 7373 6966 6965 723a   3.9.Classifier:
-00000ed0: 2054 6f70 6963 203a 3a20 5363 6965 6e74   Topic :: Scient
-00000ee0: 6966 6963 2f45 6e67 696e 6565 7269 6e67  ific/Engineering
-00000ef0: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
-00000f00: 3a20 3e3d 332e 380a 4465 7363 7269 7074  : >=3.8.Descript
-00000f10: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
-00000f20: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
-00000f30: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-00000f40: 616c 6c0a 5072 6f76 6964 6573 2d45 7874  all.Provides-Ext
-00000f50: 7261 3a20 6461 7461 0a50 726f 7669 6465  ra: data.Provide
-00000f60: 732d 4578 7472 613a 2066 6f72 6573 742d  s-Extra: forest-
-00000f70: 6f66 6673 6574 730a 5072 6f76 6964 6573  offsets.Provides
-00000f80: 2d45 7874 7261 3a20 666f 7265 7374 2d72  -Extra: forest-r
-00000f90: 6973 6b73 0a50 726f 7669 6465 732d 4578  isks.Provides-Ex
-00000fa0: 7472 613a 2073 7479 6c65 730a            tra: styles.
+00000050: 6163 6520 7061 636b 6167 650a 4175 7468  ace package.Auth
+00000060: 6f72 2d65 6d61 696c 3a20 4361 7262 6f6e  or-email: Carbon
+00000070: 506c 616e 203c 7465 6368 4063 6172 626f  Plan <tech@carbo
+00000080: 6e70 6c61 6e2e 6f72 673e 0a4c 6963 656e  nplan.org>.Licen
+00000090: 7365 3a20 4d49 540a 5072 6f6a 6563 742d  se: MIT.Project-
+000000a0: 5552 4c3a 2072 6570 6f73 6974 6f72 792c  URL: repository,
+000000b0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+000000c0: 636f 6d2f 6361 7262 6f6e 706c 616e 2f63  com/carbonplan/c
+000000d0: 6172 626f 6e70 6c61 6e2d 7079 7468 6f6e  arbonplan-python
+000000e0: 0a43 6c61 7373 6966 6965 723a 2044 6576  .Classifier: Dev
+000000f0: 656c 6f70 6d65 6e74 2053 7461 7475 7320  elopment Status 
+00000100: 3a3a 2032 202d 2050 7265 2d41 6c70 6861  :: 2 - Pre-Alpha
+00000110: 0a43 6c61 7373 6966 6965 723a 204c 6963  .Classifier: Lic
+00000120: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+00000130: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
+00000140: 6e73 650a 436c 6173 7369 6669 6572 3a20  nse.Classifier: 
+00000150: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+00000160: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
+00000170: 6e74 0a43 6c61 7373 6966 6965 723a 2049  nt.Classifier: I
+00000180: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
+00000190: 203a 3a20 5363 6965 6e63 652f 5265 7365   :: Science/Rese
+000001a0: 6172 6368 0a43 6c61 7373 6966 6965 723a  arch.Classifier:
+000001b0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+000001c0: 6775 6167 6520 3a3a 2050 7974 686f 6e0a  guage :: Python.
+000001d0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+000001e0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000001f0: 203a 3a20 5079 7468 6f6e 203a 3a20 330a   :: Python :: 3.
+00000200: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000210: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000220: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000230: 390a 436c 6173 7369 6669 6572 3a20 5072  9.Classifier: Pr
+00000240: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000250: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000260: 332e 3130 0a43 6c61 7373 6966 6965 723a  3.10.Classifier:
+00000270: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000280: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000290: 3a3a 2033 2e31 310a 436c 6173 7369 6669  :: 3.11.Classifi
+000002a0: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+000002b0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000002c0: 6f6e 203a 3a20 332e 3132 0a43 6c61 7373  on :: 3.12.Class
+000002d0: 6966 6965 723a 2054 6f70 6963 203a 3a20  ifier: Topic :: 
+000002e0: 5363 6965 6e74 6966 6963 2f45 6e67 696e  Scientific/Engin
+000002f0: 6565 7269 6e67 0a52 6571 7569 7265 732d  eering.Requires-
+00000300: 5079 7468 6f6e 3a20 3e3d 332e 390a 4465  Python: >=3.9.De
+00000310: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
+00000320: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
+00000330: 6b64 6f77 6e0a 4c69 6365 6e73 652d 4669  kdown.License-Fi
+00000340: 6c65 3a20 4c49 4345 4e53 450a 5265 7175  le: LICENSE.Requ
+00000350: 6972 6573 2d44 6973 743a 2077 6174 6572  ires-Dist: water
+00000360: 6d61 726b 0a50 726f 7669 6465 732d 4578  mark.Provides-Ex
+00000370: 7472 613a 2064 6576 0a52 6571 7569 7265  tra: dev.Require
+00000380: 732d 4469 7374 3a20 7079 7465 7374 3b20  s-Dist: pytest; 
+00000390: 6578 7472 6120 3d3d 2022 6465 7622 0a52  extra == "dev".R
+000003a0: 6571 7569 7265 732d 4469 7374 3a20 6361  equires-Dist: ca
+000003b0: 7262 6f6e 706c 616e 2d64 6174 613b 2065  rbonplan-data; e
+000003c0: 7874 7261 203d 3d20 2264 6576 220a 5265  xtra == "dev".Re
+000003d0: 7175 6972 6573 2d44 6973 743a 2063 6172  quires-Dist: car
+000003e0: 626f 6e70 6c61 6e2d 7374 796c 6573 3b20  bonplan-styles; 
+000003f0: 6578 7472 6120 3d3d 2022 6465 7622 0a50  extra == "dev".P
+00000400: 726f 7669 6465 732d 4578 7472 613a 2061  rovides-Extra: a
+00000410: 6c6c 0a52 6571 7569 7265 732d 4469 7374  ll.Requires-Dist
+00000420: 3a20 6361 7262 6f6e 706c 616e 2d64 6174  : carbonplan-dat
+00000430: 613b 2065 7874 7261 203d 3d20 2261 6c6c  a; extra == "all
+00000440: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000450: 2063 6172 626f 6e70 6c61 6e2d 7374 796c   carbonplan-styl
+00000460: 6573 3b20 6578 7472 6120 3d3d 2022 616c  es; extra == "al
+00000470: 6c22 0a52 6571 7569 7265 732d 4469 7374  l".Requires-Dist
+00000480: 3a20 6361 7262 6f6e 706c 616e 2d66 6f72  : carbonplan-for
+00000490: 6573 742d 6f66 6673 6574 733b 2065 7874  est-offsets; ext
+000004a0: 7261 203d 3d20 2261 6c6c 220a 5265 7175  ra == "all".Requ
+000004b0: 6972 6573 2d44 6973 743a 2063 6172 626f  ires-Dist: carbo
+000004c0: 6e70 6c61 6e2d 666f 7265 7374 2d72 6973  nplan-forest-ris
+000004d0: 6b73 3b20 6578 7472 6120 3d3d 2022 616c  ks; extra == "al
+000004e0: 6c22 0a50 726f 7669 6465 732d 4578 7472  l".Provides-Extr
+000004f0: 613a 2064 6174 610a 5265 7175 6972 6573  a: data.Requires
+00000500: 2d44 6973 743a 2063 6172 626f 6e70 6c61  -Dist: carbonpla
+00000510: 6e2d 6461 7461 3b20 6578 7472 6120 3d3d  n-data; extra ==
+00000520: 2022 6461 7461 220a 5072 6f76 6964 6573   "data".Provides
+00000530: 2d45 7874 7261 3a20 7374 796c 6573 0a52  -Extra: styles.R
+00000540: 6571 7569 7265 732d 4469 7374 3a20 6361  equires-Dist: ca
+00000550: 7262 6f6e 706c 616e 2d73 7479 6c65 733b  rbonplan-styles;
+00000560: 2065 7874 7261 203d 3d20 2273 7479 6c65   extra == "style
+00000570: 7322 0a50 726f 7669 6465 732d 4578 7472  s".Provides-Extr
+00000580: 613a 2066 6f72 6573 742d 6f66 6673 6574  a: forest-offset
+00000590: 730a 5265 7175 6972 6573 2d44 6973 743a  s.Requires-Dist:
+000005a0: 2063 6172 626f 6e70 6c61 6e2d 666f 7265   carbonplan-fore
+000005b0: 7374 2d6f 6666 7365 7473 3b20 6578 7472  st-offsets; extr
+000005c0: 6120 3d3d 2022 666f 7265 7374 2d6f 6666  a == "forest-off
+000005d0: 7365 7473 220a 5072 6f76 6964 6573 2d45  sets".Provides-E
+000005e0: 7874 7261 3a20 666f 7265 7374 2d72 6973  xtra: forest-ris
+000005f0: 6b73 0a52 6571 7569 7265 732d 4469 7374  ks.Requires-Dist
+00000600: 3a20 6361 7262 6f6e 706c 616e 2d66 6f72  : carbonplan-for
+00000610: 6573 742d 7269 736b 733b 2065 7874 7261  est-risks; extra
+00000620: 203d 3d20 2266 6f72 6573 742d 7269 736b   == "forest-risk
+00000630: 7322 0a0a 3c70 2061 6c69 676e 3d22 6c65  s"..<p align="le
+00000640: 6674 2220 3e0a 3c61 2068 7265 663d 2768  ft" >.<a href='h
+00000650: 7474 7073 3a2f 2f63 6172 626f 6e70 6c61  ttps://carbonpla
+00000660: 6e2e 6f72 6727 3e0a 3c70 6963 7475 7265  n.org'>.<picture
+00000670: 3e0a 2020 3c73 6f75 7263 6520 6d65 6469  >.  <source medi
+00000680: 613d 2228 7072 6566 6572 732d 636f 6c6f  a="(prefers-colo
+00000690: 722d 7363 6865 6d65 3a20 6461 726b 2922  r-scheme: dark)"
+000006a0: 2073 7263 7365 743d 2268 7474 7073 3a2f   srcset="https:/
+000006b0: 2f63 6172 626f 6e70 6c61 6e2d 6173 7365  /carbonplan-asse
+000006c0: 7473 2e73 332e 616d 617a 6f6e 6177 732e  ts.s3.amazonaws.
+000006d0: 636f 6d2f 6d6f 6e6f 6772 616d 2f6c 6967  com/monogram/lig
+000006e0: 6874 2d73 6d61 6c6c 2e70 6e67 223e 0a20  ht-small.png">. 
+000006f0: 203c 696d 6720 616c 743d 2243 6172 626f   <img alt="Carbo
+00000700: 6e50 6c61 6e20 6d6f 6e6f 6772 616d 2e22  nPlan monogram."
+00000710: 2068 6569 6768 743d 2234 3822 2073 7263   height="48" src
+00000720: 3d22 6874 7470 733a 2f2f 6361 7262 6f6e  ="https://carbon
+00000730: 706c 616e 2d61 7373 6574 732e 7333 2e61  plan-assets.s3.a
+00000740: 6d61 7a6f 6e61 7773 2e63 6f6d 2f6d 6f6e  mazonaws.com/mon
+00000750: 6f67 7261 6d2f 6461 726b 2d73 6d61 6c6c  ogram/dark-small
+00000760: 2e70 6e67 223e 0a3c 2f70 6963 7475 7265  .png">.</picture
+00000770: 3e0a 3c2f 613e 0a3c 2f70 3e0a 0a23 2063  >.</a>.</p>..# c
+00000780: 6172 626f 6e70 6c61 6e20 2f20 6361 7262  arbonplan / carb
+00000790: 6f6e 706c 616e 2d70 7974 686f 6e0a 0a2a  onplan-python..*
+000007a0: 2a6e 616d 6573 7061 6365 2070 6163 6b61  *namespace packa
+000007b0: 6765 2066 6f72 2070 7974 686f 6e20 7574  ge for python ut
+000007c0: 696c 6974 6965 7320 616e 6420 7375 6270  ilities and subp
+000007d0: 726f 6a65 6374 732a 2a0a 0a5b 215b 4349  rojects**..[![CI
+000007e0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000007f0: 2e63 6f6d 2f63 6172 626f 6e70 6c61 6e2f  .com/carbonplan/
+00000800: 6361 7262 6f6e 706c 616e 2d70 7974 686f  carbonplan-pytho
+00000810: 6e2f 6163 7469 6f6e 732f 776f 726b 666c  n/actions/workfl
+00000820: 6f77 732f 6d61 696e 2e79 616d 6c2f 6261  ows/main.yaml/ba
+00000830: 6467 652e 7376 6729 5d28 6874 7470 733a  dge.svg)](https:
+00000840: 2f2f 6769 7468 7562 2e63 6f6d 2f63 6172  //github.com/car
+00000850: 626f 6e70 6c61 6e2f 6361 7262 6f6e 706c  bonplan/carbonpl
+00000860: 616e 2d70 7974 686f 6e2f 6163 7469 6f6e  an-python/action
+00000870: 732f 776f 726b 666c 6f77 732f 6d61 696e  s/workflows/main
+00000880: 2e79 616d 6c29 0a21 5b50 7950 495d 2868  .yaml).![PyPI](h
+00000890: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000008a0: 6473 2e69 6f2f 7079 7069 2f76 2f63 6172  ds.io/pypi/v/car
+000008b0: 626f 6e70 6c61 6e29 0a5b 215b 4c69 6365  bonplan).[![Lice
+000008c0: 6e73 653a 204d 4954 5d28 6874 7470 733a  nse: MIT](https:
+000008d0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000008e0: 2f62 6164 6765 2f4c 6963 656e 7365 2d4d  /badge/License-M
+000008f0: 4954 2d62 6c75 652e 7376 6729 5d28 6874  IT-blue.svg)](ht
+00000900: 7470 733a 2f2f 6f70 656e 736f 7572 6365  tps://opensource
+00000910: 2e6f 7267 2f6c 6963 656e 7365 732f 4d49  .org/licenses/MI
+00000920: 5429 0a0a 5468 6973 2072 6570 6f73 6974  T)..This reposit
+00000930: 6f72 7920 696e 636c 7564 6573 2074 6865  ory includes the
+00000940: 2060 6361 7262 6f6e 706c 616e 6020 6e61   `carbonplan` na
+00000950: 6d65 7370 6163 6520 5079 7468 6f6e 2070  mespace Python p
+00000960: 6163 6b61 6765 2e20 5468 6520 7061 636b  ackage. The pack
+00000970: 6167 6520 6974 7365 6c66 2069 6e63 6c75  age itself inclu
+00000980: 6465 7320 7665 7279 206c 6974 746c 6520  des very little 
+00000990: 6f66 2073 7562 7374 616e 6365 2c20 616e  of substance, an
+000009a0: 6420 6973 2064 6973 7472 6962 7574 6564  d is distributed
+000009b0: 2074 6f20 6163 7420 6173 2074 6865 2074   to act as the t
+000009c0: 6f70 2d6c 6576 656c 206e 616d 6573 7061  op-level namespa
+000009d0: 6365 2066 6f72 206f 7468 6572 2050 7974  ce for other Pyt
+000009e0: 686f 6e20 7061 636b 6167 6573 2064 6576  hon packages dev
+000009f0: 656c 6f70 6564 2062 7920 4361 7262 6f6e  eloped by Carbon
+00000a00: 506c 616e 2e20 4f74 6865 7220 7061 636b  Plan. Other pack
+00000a10: 6167 6573 2069 6e63 6c75 6465 3a0a 0a7c  ages include:..|
+00000a20: 2050 6163 6b61 6765 2020 2020 2020 2020   Package        
+00000a30: 2020 2020 2020 2020 2020 207c 2049 6d70             | Imp
+00000a40: 6f72 7420 2020 2020 2020 2020 2020 2020  ort             
+00000a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a60: 7c20 4769 7448 7562 2052 6570 6f20 2020  | GitHub Repo   
+00000a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ab0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00000ac0: 0a7c 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .| -------------
+00000ad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c 202d  ------------ | -
+00000ae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000af0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b00: 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  - | ------------
+00000b10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b60: 207c 0a7c 2063 6172 626f 6e70 6c61 6e2d   |.| carbonplan-
+00000b70: 6461 7461 2020 2020 2020 2020 2020 207c  data           |
+00000b80: 2060 696d 706f 7274 2063 6172 626f 6e70   `import carbonp
+00000b90: 6c61 6e2e 6461 7461 6020 2020 2020 2020  lan.data`       
+00000ba0: 2020 2020 7c20 5b68 7474 7073 3a2f 2f67      | [https://g
+00000bb0: 6974 6875 622e 636f 6d2f 6361 7262 6f6e  ithub.com/carbon
+00000bc0: 706c 616e 2f64 6174 615d 2868 7474 7073  plan/data](https
+00000bd0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6361  ://github.com/ca
+00000be0: 7262 6f6e 706c 616e 2f64 6174 6129 2020  rbonplan/data)  
+00000bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c00: 2020 207c 0a7c 2063 6172 626f 6e70 6c61     |.| carbonpla
+00000c10: 6e2d 666f 7265 7374 2d6f 6666 7365 7473  n-forest-offsets
+00000c20: 207c 2060 696d 706f 7274 2063 6172 626f   | `import carbo
+00000c30: 6e70 6c61 6e2e 666f 7265 7374 5f6f 6666  nplan.forest_off
+00000c40: 7365 7473 6020 7c20 5b68 7474 7073 3a2f  sets` | [https:/
+00000c50: 2f67 6974 6875 622e 636f 6d2f 6361 7262  /github.com/carb
+00000c60: 6f6e 706c 616e 2f66 6f72 6573 742d 6f66  onplan/forest-of
+00000c70: 6673 6574 735d 2868 7474 7073 3a2f 2f67  fsets](https://g
+00000c80: 6974 6875 622e 636f 6d2f 6361 7262 6f6e  ithub.com/carbon
+00000c90: 706c 616e 2f66 6f72 6573 742d 6f66 6673  plan/forest-offs
+00000ca0: 6574 7329 207c 0a7c 2063 6172 626f 6e70  ets) |.| carbonp
+00000cb0: 6c61 6e2d 666f 7265 7374 2d72 6973 6b73  lan-forest-risks
+00000cc0: 2020 207c 2060 696d 706f 7274 2063 6172     | `import car
+00000cd0: 626f 6e70 6c61 6e2e 666f 7265 7374 5f72  bonplan.forest_r
+00000ce0: 6973 6b73 6020 2020 7c20 5b68 7474 7073  isks`   | [https
+00000cf0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6361  ://github.com/ca
+00000d00: 7262 6f6e 706c 616e 2f66 6f72 6573 742d  rbonplan/forest-
+00000d10: 7269 736b 735d 2868 7474 7073 3a2f 2f67  risks](https://g
+00000d20: 6974 6875 622e 636f 6d2f 6361 7262 6f6e  ithub.com/carbon
+00000d30: 706c 616e 2f66 6f72 6573 742d 7269 736b  plan/forest-risk
+00000d40: 7329 2020 2020 207c 0a7c 2063 6172 626f  s)     |.| carbo
+00000d50: 6e70 6c61 6e2d 7374 796c 6573 2020 2020  nplan-styles    
+00000d60: 2020 2020 207c 2060 696d 706f 7274 2063       | `import c
+00000d70: 6172 626f 6e70 6c61 6e2e 7374 796c 6573  arbonplan.styles
+00000d80: 6020 2020 2020 2020 2020 7c20 5b68 7474  `         | [htt
+00000d90: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000da0: 6361 7262 6f6e 706c 616e 2f73 7479 6c65  carbonplan/style
+00000db0: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
+00000dc0: 622e 636f 6d2f 6361 7262 6f6e 706c 616e  b.com/carbonplan
+00000dd0: 2f73 7479 6c65 7329 2020 2020 2020 2020  /styles)        
+00000de0: 2020 2020 2020 2020 207c 0a0a 2323 2069           |..## i
+00000df0: 6e73 7461 6c6c 0a0a 6060 6073 6865 6c6c  nstall..```shell
+00000e00: 0a70 6970 2069 6e73 7461 6c6c 2063 6172  .pip install car
+00000e10: 626f 6e70 6c61 6e5b 616c 6c5d 0a23 206f  bonplan[all].# o
+00000e20: 7220 696e 6469 7669 6475 616c 2073 7562  r individual sub
+00000e30: 2070 6163 6b61 6765 730a 7069 7020 696e   packages.pip in
+00000e40: 7374 616c 6c20 6361 7262 6f6e 706c 616e  stall carbonplan
+00000e50: 5b73 7479 6c65 735d 0a60 6060 0a0a 2323  [styles].```..##
+00000e60: 2075 7361 6765 0a0a 6060 6070 7974 686f   usage..```pytho
+00000e70: 6e0a 6672 6f6d 2063 6172 626f 6e70 6c61  n.from carbonpla
+00000e80: 6e2e 7374 796c 6573 2e6d 706c 2069 6d70  n.styles.mpl imp
+00000e90: 6f72 7420 7365 745f 7468 656d 650a 2320  ort set_theme.# 
+00000ea0: 7468 6973 2069 7320 7468 6520 7361 6d65  this is the same
+00000eb0: 2074 6869 6e67 7320 6173 0a66 726f 6d20   things as.from 
+00000ec0: 6361 7262 6f6e 706c 616e 5f73 7479 6c65  carbonplan_style
+00000ed0: 732e 6d70 6c20 696d 706f 7274 2073 6574  s.mpl import set
+00000ee0: 5f74 6865 6d65 0a60 6060 0a0a 2323 206c  _theme.```..## l
+00000ef0: 6963 656e 7365 0a0a 416c 6c20 7468 6520  icense..All the 
+00000f00: 636f 6465 2069 6e20 7468 6973 2072 6570  code in this rep
+00000f10: 6f73 6974 6f72 7920 6973 205b 4d49 545d  ository is [MIT]
+00000f20: 2868 7474 7073 3a2f 2f63 686f 6f73 6561  (https://choosea
+00000f30: 6c69 6365 6e73 652e 636f 6d2f 6c69 6365  license.com/lice
+00000f40: 6e73 6573 2f6d 6974 2f29 2d6c 6963 656e  nses/mit/)-licen
+00000f50: 7365 642e 2057 6520 696e 636c 7564 6520  sed. We include 
+00000f60: 6174 7472 6962 7574 696f 6e20 666f 7220  attribution for 
+00000f70: 7468 6973 2063 6f6e 7465 6e74 2c20 616e  this content, an
+00000f80: 6420 7765 2070 6c65 6173 6520 7265 7175  d we please requ
+00000f90: 6573 7420 7468 6174 2079 6f75 2061 6c73  est that you als
+00000fa0: 6f20 6d61 696e 7461 696e 2074 6861 7420  o maintain that 
+00000fb0: 6174 7472 6962 7574 696f 6e20 6966 2075  attribution if u
+00000fc0: 7369 6e67 2074 6869 7320 6461 7461 2e0a  sing this data..
+00000fd0: 0a23 2320 6162 6f75 7420 7573 0a0a 4361  .## about us..Ca
+00000fe0: 7262 6f6e 506c 616e 2069 7320 6120 6e6f  rbonPlan is a no
+00000ff0: 6e70 726f 6669 7420 6f72 6761 6e69 7a61  nprofit organiza
+00001000: 7469 6f6e 2074 6861 7420 7573 6573 2064  tion that uses d
+00001010: 6174 6120 616e 6420 7363 6965 6e63 6520  ata and science 
+00001020: 666f 7220 636c 696d 6174 6520 6163 7469  for climate acti
+00001030: 6f6e 2e20 5765 2061 696d 2074 6f20 696d  on. We aim to im
+00001040: 7072 6f76 6520 7468 6520 7472 616e 7370  prove the transp
+00001050: 6172 656e 6379 2061 6e64 2073 6369 656e  arency and scien
+00001060: 7469 6669 6320 696e 7465 6772 6974 7920  tific integrity 
+00001070: 6f66 2063 6c69 6d61 7465 2073 6f6c 7574  of climate solut
+00001080: 696f 6e73 2077 6974 6820 6f70 656e 2064  ions with open d
+00001090: 6174 6120 616e 6420 746f 6f6c 732e 2046  ata and tools. F
+000010a0: 696e 6420 6f75 7420 6d6f 7265 2061 7420  ind out more at 
+000010b0: 5b63 6172 626f 6e70 6c61 6e2e 6f72 675d  [carbonplan.org]
+000010c0: 2868 7474 7073 3a2f 2f63 6172 626f 6e70  (https://carbonp
+000010d0: 6c61 6e2e 6f72 672f 2920 6f72 2067 6574  lan.org/) or get
+000010e0: 2069 6e20 746f 7563 6820 6279 205b 6f70   in touch by [op
+000010f0: 656e 696e 6720 616e 2069 7373 7565 5d28  ening an issue](
+00001100: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001110: 6f6d 2f63 6172 626f 6e70 6c61 6e2f 6361  om/carbonplan/ca
+00001120: 7262 6f6e 706c 616e 2d70 7974 686f 6e2f  rbonplan-python/
+00001130: 6973 7375 6573 2f6e 6577 2920 6f72 205b  issues/new) or [
+00001140: 7365 6e64 696e 6720 7573 2061 6e20 656d  sending us an em
+00001150: 6169 6c5d 286d 6169 6c74 6f3a 6865 6c6c  ail](mailto:hell
+00001160: 6f40 6361 7262 6f6e 706c 616e 2e6f 7267  o@carbonplan.org
+00001170: 292e 0a                                  )..
```

### Comparing `carbonplan-0.5.0/carbonplan.egg-info/SOURCES.txt` & `carbonplan-0.6.0/carbonplan.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.md
-dev-requirements.txt
-requirements.txt
-setup.cfg
-setup.py
+pyproject.toml
 .github/dependabot.yml
 .github/workflows/main.yaml
+.github/workflows/pypi-release.yaml
 carbonplan/__init__.py
 carbonplan/data.py
 carbonplan/forests_offsets.py
 carbonplan/forests_risks.py
 carbonplan/styles.py
 carbonplan/trace.py
 carbonplan/watermark.py
```

### Comparing `carbonplan-0.5.0/setup.py` & `carbonplan-0.6.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,104 @@
-import os
-
-from setuptools import find_packages, setup
+[build-system]
+requires = ["setuptools>=64", "setuptools-scm[toml]>=6.2", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "carbonplan"
+description = "CarbonPlan namespace package"
+readme = "README.md"
+license = { text = "MIT" }
+authors = [{ name = "CarbonPlan", email = "tech@carbonplan.org" }]
+requires-python = ">=3.9"
+classifiers = [
+    "Development Status :: 2 - Pre-Alpha",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Intended Audience :: Science/Research",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Topic :: Scientific/Engineering",
+]
+dynamic = ["version"]
 
-with open('requirements.txt') as f:
-    install_requires = f.read().strip().split('\n')
+dependencies = [
+    "watermark"
+]
 
-if os.path.exists('README.md'):
-    with open('README.md') as f:
-        long_description = f.read()
-else:
-    long_description = ''
-
-
-CLASSIFIERS = [
-    'Development Status :: 2 - Pre-Alpha',
-    'License :: OSI Approved :: MIT License',
-    'Operating System :: OS Independent',
-    'Intended Audience :: Science/Research',
-    'Programming Language :: Python',
-    'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
-    'Topic :: Scientific/Engineering',
+[project.optional-dependencies]
+dev = ["pytest", "carbonplan-data", "carbonplan-styles"]
+all = ["carbonplan-data", "carbonplan-styles", "carbonplan-forest-offsets", "carbonplan-forest-risks"]
+data = ["carbonplan-data"]
+styles = ["carbonplan-styles"]
+forest-offsets = ["carbonplan-forest-offsets"]
+forest-risks = ["carbonplan-forest-risks"]
+
+[project.urls]
+repository = "https://github.com/carbonplan/carbonplan-python"
+
+[tool.setuptools.packages.find]
+include = ["carbonplan*"]
+
+[tool.setuptools_scm]
+local_scheme = "node-and-date"
+fallback_version = "999"
+
+
+[tool.black]
+line-length = 100
+target-version = ['py39']
+skip-string-normalization = true
+
+
+[tool.ruff]
+line-length = 100
+target-version = "py39"
+builtins = ["ellipsis"]
+# Exclude a variety of commonly ignored directories.
+exclude = [
+    ".bzr",
+    ".direnv",
+    ".eggs",
+    ".git",
+    ".hg",
+    ".mypy_cache",
+    ".nox",
+    ".pants.d",
+    ".ruff_cache",
+    ".svn",
+    ".tox",
+    ".venv",
+    "__pypackages__",
+    "_build",
+    "buck-out",
+    "build",
+    "dist",
+    "node_modules",
+    "venv",
 ]
+per-file-ignores = {}
+# E402: module level import not at top of file
+# E501: line too long - let black worry about that
+# E731: do not assign a lambda expression, use a def
+ignore = ["E402", "E501", "E731"]
+select = [
+    # Pyflakes
+    "F",
+    # Pycodestyle
+    "E",
+    "W",
+    # isort
+    "I",
+    # Pyupgrade
+    "UP",
+]
+
+
+[tool.ruff.mccabe]
+max-complexity = 18
 
-extras_require = {
-    'all': ['carbonplan-data', 'carbonplan-styles', 'carbonplan-forest-risks'],
-    'data': ['carbonplan-data'],
-    'forest-offsets': ['carbonplan-forest-offsets'],
-    'forest-risks': ['carbonplan-forest-risks'],
-    'styles': ['carbonplan-styles'],
-}
-
-setup(
-    name='carbonplan',
-    description='CarbonPlan namespace package',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    python_requires='>=3.8',
-    maintainer='Joe Hamman',
-    maintainer_email='joe@carbonplan.org',
-    url='https://github.com/carbonplan/carbonplan-python',
-    license='MIT',
-    packages=find_packages(exclude=('tests',)),
-    install_requires=install_requires,
-    extras_require=extras_require,
-    classifiers=CLASSIFIERS,
-    use_scm_version={"version_scheme": "post-release", "local_scheme": "node-and-timestamp"},
-    setup_requires=["setuptools_scm", "setuptools>=30.3.0", "setuptools_scm_git_archive"],
-)
+[tool.ruff.isort]
+known-first-party = ["carbonplan"]
```

