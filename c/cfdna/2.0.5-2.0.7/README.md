# Comparing `tmp/cfdna-2.0.5.tar.gz` & `tmp/cfdna-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfdna-2.0.5.tar", max compression
+gzip compressed data, was "cfdna-2.0.7.tar", max compression
```

## Comparing `cfdna-2.0.5.tar` & `cfdna-2.0.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rwxr-xr-x   0        0        0    17895 2022-07-20 16:09:08.000000 cfdna-2.0.5/LICENSE.md
--rwxr-xr-x   0        0        0     1334 2023-11-21 13:51:31.978445 cfdna-2.0.5/README.md
--rw-r--r--   0        0        0     8196 2023-11-21 04:15:35.105678 cfdna-2.0.5/cfdna/.DS_Store
--rwxr-xr-x   0        0        0      638 2023-11-21 13:59:51.763979 cfdna-2.0.5/cfdna/__init__.py
--rwxr-xr-x   0        0        0     2076 2023-11-21 04:10:09.783928 cfdna-2.0.5/cfdna/__main__.py
--rwxr-xr-x   0        0        0       69 2022-07-20 16:09:08.000000 cfdna-2.0.5/cfdna/commandline/__init__.py
--rwxr-xr-x   0        0        0     2270 2023-11-21 04:15:54.236384 cfdna-2.0.5/cfdna/commandline/commands.py
--rwxr-xr-x   0        0        0       64 2022-08-30 19:13:58.000000 cfdna-2.0.5/cfdna/core/__init__.py
--rwxr-xr-x   0        0        0     2918 2023-11-06 18:52:38.951861 cfdna-2.0.5/cfdna/core/core.py
--rw-r--r--   0        0        0     6148 2023-11-06 14:19:28.230169 cfdna-2.0.5/cfdna/io/.DS_Store
--rwxr-xr-x   0        0        0      281 2022-07-20 16:09:09.000000 cfdna-2.0.5/cfdna/io/__init__.py
--rwxr-xr-x   0        0        0      184 2022-07-20 16:09:09.000000 cfdna-2.0.5/cfdna/io/read/__init__.py
--rwxr-xr-x   0        0        0     1762 2023-02-03 15:34:27.663648 cfdna-2.0.5/cfdna/io/read/read_bam.py
--rwxr-xr-x   0        0        0      491 2023-11-06 18:42:33.912191 cfdna-2.0.5/cfdna/io/read/read_h5.py
--rwxr-xr-x   0        0        0      190 2022-07-20 16:09:09.000000 cfdna-2.0.5/cfdna/io/write/__init__.py
--rwxr-xr-x   0        0        0      511 2023-11-06 18:43:44.583371 cfdna-2.0.5/cfdna/io/write/write_h5.py
--rwxr-xr-x   0        0        0      849 2022-07-20 16:09:09.000000 cfdna-2.0.5/cfdna/io/write/write_text.py
--rwxr-xr-x   0        0        0       67 2022-07-20 16:09:08.000000 cfdna-2.0.5/cfdna/plot/__init__.py
--rwxr-xr-x   0        0        0     7663 2022-07-20 16:09:09.000000 cfdna-2.0.5/cfdna/plot/plot_bokeh.py
--rwxr-xr-x   0        0        0      990 2023-11-07 16:01:23.498388 cfdna-2.0.5/cfdna/plot/plot_plt.py
--rwxr-xr-x   0        0        0      391 2022-10-05 14:16:05.000000 cfdna-2.0.5/cfdna/tools/__init__.py
--rwxr-xr-x   0        0        0      167 2023-11-06 18:36:25.971444 cfdna-2.0.5/cfdna/tools/cnv/__init__.py
--rwxr-xr-x   0        0        0     3563 2023-11-06 18:44:12.544286 cfdna-2.0.5/cfdna/tools/cnv/segmentation.py
--rw-r--r--   0        0        0     1301 2023-11-07 17:27:07.399506 cfdna-2.0.5/cfdna/tools/coverage/gene_activity.py
--rwxr-xr-x   0        0        0      165 2022-07-20 16:09:08.000000 cfdna-2.0.5/cfdna/tools/fragmentation/__init__.py
--rwxr-xr-x   0        0        0     2418 2022-08-30 16:29:27.000000 cfdna-2.0.5/cfdna/tools/fragmentation/frag_pattern.py
--rwxr-xr-x   0        0        0      175 2022-07-20 16:09:08.000000 cfdna-2.0.5/cfdna/tools/nucleosome/__init__.py
--rw-r--r--   0        0        0     4281 2022-10-20 20:27:47.000000 cfdna-2.0.5/cfdna/tools/nucleosome/gene_activity.py
--rwxr-xr-x   0        0        0     8696 2022-08-30 16:32:05.000000 cfdna-2.0.5/cfdna/tools/nucleosome/nfr.py
--rw-r--r--   0        0        0     5375 2022-10-21 19:39:37.000000 cfdna-2.0.5/cfdna/tools/nucleosome/relative_window.py
--rwxr-xr-x   0        0        0     4302 2022-10-05 14:44:52.000000 cfdna-2.0.5/cfdna/tools/nucleosome/wps.py
--rw-r--r--   0        0        0     7053 2022-10-05 14:45:53.000000 cfdna-2.0.5/cfdna/tools/nucleosome/wps_functions.py
--rwxr-xr-x   0        0        0      162 2022-07-20 16:09:08.000000 cfdna-2.0.5/cfdna/tools/summarize/__init__.py
--rw-r--r--   0        0        0     3551 2022-08-30 19:26:15.000000 cfdna-2.0.5/cfdna/tools/summarize/multi_sample.py
--rwxr-xr-x   0        0        0     3417 2023-11-06 18:46:14.639312 cfdna-2.0.5/cfdna/tools/summarize/summarize.py
--rwxr-xr-x   0        0        0      143 2022-07-20 16:09:09.000000 cfdna-2.0.5/cfdna/utilities/__init__.py
--rwxr-xr-x   0        0        0     4289 2022-08-30 19:22:16.000000 cfdna-2.0.5/cfdna/utilities/h5_utilities.py
--rw-r--r--   0        0        0     2478 2023-11-21 13:59:45.045238 cfdna-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 cfdna-2.0.5/PKG-INFO
+-rwxr-xr-x   0        0        0    17895 2022-07-20 16:09:08.000000 cfdna-2.0.7/LICENSE.md
+-rwxr-xr-x   0        0        0     1341 2023-11-21 14:09:42.209706 cfdna-2.0.7/README.md
+-rw-r--r--   0        0        0     8196 2024-04-15 19:39:52.737913 cfdna-2.0.7/cfdna/.DS_Store
+-rwxr-xr-x   0        0        0      638 2024-04-16 03:46:52.824792 cfdna-2.0.7/cfdna/__init__.py
+-rwxr-xr-x   0        0        0     4486 2024-04-16 02:05:12.659608 cfdna-2.0.7/cfdna/__main__.py
+-rwxr-xr-x   0        0        0       69 2022-07-20 16:09:08.000000 cfdna-2.0.7/cfdna/commandline/__init__.py
+-rwxr-xr-x   0        0        0     8267 2024-04-16 03:13:23.158743 cfdna-2.0.7/cfdna/commandline/commands.py
+-rwxr-xr-x   0        0        0       64 2022-08-30 19:13:58.000000 cfdna-2.0.7/cfdna/core/__init__.py
+-rwxr-xr-x   0        0        0     2918 2023-11-06 18:52:38.951861 cfdna-2.0.7/cfdna/core/core.py
+-rw-r--r--   0        0        0     6148 2023-11-06 14:19:28.230169 cfdna-2.0.7/cfdna/io/.DS_Store
+-rwxr-xr-x   0        0        0      281 2022-07-20 16:09:09.000000 cfdna-2.0.7/cfdna/io/__init__.py
+-rwxr-xr-x   0        0        0      184 2022-07-20 16:09:09.000000 cfdna-2.0.7/cfdna/io/read/__init__.py
+-rwxr-xr-x   0        0        0     1762 2023-02-03 15:34:27.663648 cfdna-2.0.7/cfdna/io/read/read_bam.py
+-rwxr-xr-x   0        0        0      491 2023-11-06 18:42:33.912191 cfdna-2.0.7/cfdna/io/read/read_h5.py
+-rwxr-xr-x   0        0        0      190 2022-07-20 16:09:09.000000 cfdna-2.0.7/cfdna/io/write/__init__.py
+-rwxr-xr-x   0        0        0      511 2023-11-06 18:43:44.583371 cfdna-2.0.7/cfdna/io/write/write_h5.py
+-rwxr-xr-x   0        0        0      849 2022-07-20 16:09:09.000000 cfdna-2.0.7/cfdna/io/write/write_text.py
+-rwxr-xr-x   0        0        0       67 2022-07-20 16:09:08.000000 cfdna-2.0.7/cfdna/plot/__init__.py
+-rwxr-xr-x   0        0        0     7663 2022-07-20 16:09:09.000000 cfdna-2.0.7/cfdna/plot/plot_bokeh.py
+-rwxr-xr-x   0        0        0      990 2023-11-07 16:01:23.498388 cfdna-2.0.7/cfdna/plot/plot_plt.py
+-rwxr-xr-x   0        0        0      391 2022-10-05 14:16:05.000000 cfdna-2.0.7/cfdna/tools/__init__.py
+-rwxr-xr-x   0        0        0      167 2023-11-06 18:36:25.971444 cfdna-2.0.7/cfdna/tools/cnv/__init__.py
+-rwxr-xr-x   0        0        0     3563 2023-11-06 18:44:12.544286 cfdna-2.0.7/cfdna/tools/cnv/segmentation.py
+-rw-r--r--   0        0        0     1334 2024-03-21 21:01:17.622900 cfdna-2.0.7/cfdna/tools/coverage/gene_activity.py
+-rwxr-xr-x   0        0        0      165 2022-07-20 16:09:08.000000 cfdna-2.0.7/cfdna/tools/fragmentation/__init__.py
+-rwxr-xr-x   0        0        0     2418 2022-08-30 16:29:27.000000 cfdna-2.0.7/cfdna/tools/fragmentation/frag_pattern.py
+-rwxr-xr-x   0        0        0      175 2022-07-20 16:09:08.000000 cfdna-2.0.7/cfdna/tools/nucleosome/__init__.py
+-rw-r--r--   0        0        0     4281 2022-10-20 20:27:47.000000 cfdna-2.0.7/cfdna/tools/nucleosome/gene_activity.py
+-rwxr-xr-x   0        0        0     8696 2022-08-30 16:32:05.000000 cfdna-2.0.7/cfdna/tools/nucleosome/nfr.py
+-rw-r--r--   0        0        0     5375 2022-10-21 19:39:37.000000 cfdna-2.0.7/cfdna/tools/nucleosome/relative_window.py
+-rwxr-xr-x   0        0        0     4302 2022-10-05 14:44:52.000000 cfdna-2.0.7/cfdna/tools/nucleosome/wps.py
+-rw-r--r--   0        0        0     7053 2022-10-05 14:45:53.000000 cfdna-2.0.7/cfdna/tools/nucleosome/wps_functions.py
+-rwxr-xr-x   0        0        0      162 2022-07-20 16:09:08.000000 cfdna-2.0.7/cfdna/tools/summarize/__init__.py
+-rw-r--r--   0        0        0     3551 2022-08-30 19:26:15.000000 cfdna-2.0.7/cfdna/tools/summarize/multi_sample.py
+-rwxr-xr-x   0        0        0     3417 2023-11-06 18:46:14.639312 cfdna-2.0.7/cfdna/tools/summarize/summarize.py
+-rwxr-xr-x   0        0        0      143 2022-07-20 16:09:09.000000 cfdna-2.0.7/cfdna/utilities/__init__.py
+-rwxr-xr-x   0        0        0     4289 2022-08-30 19:22:16.000000 cfdna-2.0.7/cfdna/utilities/h5_utilities.py
+-rw-r--r--   0        0        0     2478 2024-04-16 03:48:10.613356 cfdna-2.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3556 1970-01-01 00:00:00.000000 cfdna-2.0.7/PKG-INFO
```

### Comparing `cfdna-2.0.5/LICENSE.md` & `cfdna-2.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.5/README.md` & `cfdna-2.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     https://continuum.io/downloads
 ```
 
 Create environment and pip install:
 ```
     conda create -n cfdna python=3.11.3
 	conda activate cfdna
-	pip install cfdna
+	pip install cfdna==2.0.5
 ```
 
 Dependencies can be installed by:
 
 ```
     pip install -r requirements.txt
 ```
```

### Comparing `cfdna-2.0.5/cfdna/.DS_Store` & `cfdna-2.0.7/cfdna/.DS_Store`

 * *Files 14% similar despite different names*

```diff
@@ -253,102 +253,102 @@
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0000 0000 000c 0000 000b  ................
 00001010: 0063 006f 006d 006d 0061 006e 0064 006c  .c.o.m.m.a.n.d.l
 00001020: 0069 006e 0065 6277 7370 626c 6f62 0000  .i.n.ebwspblob..
-00001030: 00b7 6270 6c69 7374 3030 d601 0203 0405  ..bplist00......
+00001030: 00b8 6270 6c69 7374 3030 d601 0203 0405  ..bplist00......
 00001040: 0607 0807 080b 085d 5368 6f77 5374 6174  .......]ShowStat
 00001050: 7573 4261 725b 5368 6f77 546f 6f6c 6261  usBar[ShowToolba
 00001060: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
 00001070: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
 00001080: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
 00001090: 735b 5368 6f77 5369 6465 6261 7208 0908  s[ShowSidebar...
-000010a0: 095f 1017 7b7b 3434 2c20 3338 377d 2c20  ._..{{44, 387}, 
-000010b0: 7b39 3230 2c20 3434 367d 7d09 0815 232f  {920, 446}}...#/
-000010c0: 3b52 5f6b 6c6d 6e6f 8900 0000 0000 0001  ;R_klmno........
-000010d0: 0100 0000 0000 0000 0d00 0000 0000 0000  ................
-000010e0: 0000 0000 0000 0000 8a00 0000 0b00 6300  ..............c.
-000010f0: 6f00 6d00 6d00 6100 6e00 6400 6c00 6900  o.m.m.a.n.d.l.i.
-00001100: 6e00 6576 5372 6e6c 6f6e 6700 0000 0100  n.evSrnlong.....
-00001110: 0000 0400 6300 6f00 7200 6562 7773 7062  ....c.o.r.ebwspb
-00001120: 6c6f 6200 0000 b762 706c 6973 7430 30d6  lob....bplist00.
-00001130: 0102 0304 0506 0708 0708 0b08 5d53 686f  ............]Sho
-00001140: 7753 7461 7475 7342 6172 5b53 686f 7754  wStatusBar[ShowT
-00001150: 6f6f 6c62 6172 5b53 686f 7754 6162 5669  oolbar[ShowTabVi
-00001160: 6577 5f10 1443 6f6e 7461 696e 6572 5368  ew_..ContainerSh
-00001170: 6f77 5369 6465 6261 725c 5769 6e64 6f77  owSidebar\Window
-00001180: 426f 756e 6473 5b53 686f 7753 6964 6562  Bounds[ShowSideb
-00001190: 6172 0809 0809 5f10 177b 7b34 342c 2033  ar...._..{{44, 3
-000011a0: 3934 7d2c 207b 3932 302c 2034 3436 7d7d  94}, {920, 446}}
-000011b0: 0908 1523 2f3b 525f 6b6c 6d6e 6f89 0000  ...#/;R_klmno...
-000011c0: 0000 0000 0101 0000 0000 0000 000d 0000  ................
-000011d0: 0000 0000 0000 0000 0000 0000 008a 0000  ................
-000011e0: 0004 0063 006f 0072 0065 7653 726e 6c6f  ...c.o.r.evSrnlo
-000011f0: 6e67 0000 0001 0000 0002 0069 006f 6277  ng.........i.obw
-00001200: 7370 626c 6f62 0000 00b7 6270 6c69 7374  spblob....bplist
-00001210: 3030 d601 0203 0405 0607 0807 080b 085d  00.............]
-00001220: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
-00001230: 6f77 546f 6f6c 6261 725b 5368 6f77 5461  owToolbar[ShowTa
-00001240: 6256 6965 775f 1014 436f 6e74 6169 6e65  bView_..Containe
-00001250: 7253 686f 7753 6964 6562 6172 5c57 696e  rShowSidebar\Win
-00001260: 646f 7742 6f75 6e64 735b 5368 6f77 5369  dowBounds[ShowSi
-00001270: 6465 6261 7208 0908 095f 1017 7b7b 3434  debar...._..{{44
-00001280: 2c20 3339 347d 2c20 7b39 3230 2c20 3434  , 394}, {920, 44
-00001290: 367d 7d09 0815 232f 3b52 5f6b 6c6d 6e6f  6}}...#/;R_klmno
-000012a0: 8900 0000 0000 0001 0100 0000 0000 0000  ................
-000012b0: 0d00 0000 0000 0000 0000 0000 0000 0000  ................
-000012c0: 8a00 0000 0200 6900 6f76 5372 6e6c 6f6e  ......i.ovSrnlon
-000012d0: 6700 0000 0100 0000 0400 7000 6c00 6f00  g.........p.l.o.
-000012e0: 7462 7773 7062 6c6f 6200 0000 b762 706c  tbwspblob....bpl
-000012f0: 6973 7430 30d6 0102 0304 0506 0708 0708  ist00...........
-00001300: 0b08 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
-00001310: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
-00001320: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
-00001330: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
-00001340: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
-00001350: 7753 6964 6562 6172 0809 0809 5f10 177b  wSidebar...._..{
-00001360: 7b34 342c 2033 3934 7d2c 207b 3932 302c  {44, 394}, {920,
-00001370: 2034 3436 7d7d 0908 1523 2f3b 525f 6b6c   446}}...#/;R_kl
-00001380: 6d6e 6f89 0000 0000 0000 0101 0000 0000  mno.............
-00001390: 0000 000d 0000 0000 0000 0000 0000 0000  ................
-000013a0: 0000 008a 0000 0004 0070 006c 006f 0074  .........p.l.o.t
-000013b0: 7653 726e 6c6f 6e67 0000 0001 0000 0005  vSrnlong........
-000013c0: 0074 006f 006f 006c 0073 6277 7370 626c  .t.o.o.l.sbwspbl
-000013d0: 6f62 0000 00b7 6270 6c69 7374 3030 d601  ob....bplist00..
-000013e0: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
-000013f0: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
-00001400: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
-00001410: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
-00001420: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
-00001430: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00001440: 7208 0908 095f 1017 7b7b 3434 2c20 3338  r...._..{{44, 38
-00001450: 377d 2c20 7b39 3230 2c20 3434 367d 7d09  7}, {920, 446}}.
-00001460: 0815 232f 3b52 5f6b 6c6d 6e6f 8900 0000  ..#/;R_klmno....
-00001470: 0000 0001 0100 0000 0000 0000 0d00 0000  ................
-00001480: 0000 0000 0000 0000 0000 0000 8a00 0000  ................
-00001490: 0500 7400 6f00 6f00 6c00 7376 5372 6e6c  ..t.o.o.l.svSrnl
-000014a0: 6f6e 6700 0000 0100 0000 0900 7500 7400  ong.........u.t.
-000014b0: 6900 6c00 6900 7400 6900 6500 7362 7773  i.l.i.t.i.e.sbws
-000014c0: 7062 6c6f 6200 0000 b762 706c 6973 7430  pblob....bplist0
-000014d0: 30d6 0102 0304 0506 0708 0708 0b08 5d53  0.............]S
-000014e0: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
-000014f0: 7754 6f6f 6c62 6172 5b53 686f 7754 6162  wToolbar[ShowTab
-00001500: 5669 6577 5f10 1443 6f6e 7461 696e 6572  View_..Container
-00001510: 5368 6f77 5369 6465 6261 725c 5769 6e64  ShowSidebar\Wind
-00001520: 6f77 426f 756e 6473 5b53 686f 7753 6964  owBounds[ShowSid
-00001530: 6562 6172 0809 0809 5f10 177b 7b34 342c  ebar...._..{{44,
-00001540: 2033 3934 7d2c 207b 3932 302c 2034 3436   394}, {920, 446
-00001550: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f89  }}...#/;R_klmno.
-00001560: 0000 0000 0000 0101 0000 0000 0000 000d  ................
-00001570: 0000 0000 0000 0000 0000 0000 0000 008a  ................
-00001580: 0000 0009 0075 0074 0069 006c 0069 0074  .....u.t.i.l.i.t
-00001590: 0069 0065 0073 7653 726e 6c6f 6e67 0000  .i.e.svSrnlong..
-000015a0: 0001 0000 0000 0000 0000 0000 0000 0000  ................
+000010a0: 095f 1018 7b7b 3335 372c 2034 3330 7d2c  ._..{{357, 430},
+000010b0: 207b 3932 302c 2034 3336 7d7d 0908 1523   {920, 436}}...#
+000010c0: 2f3b 525f 6b6c 6d6e 6f8a 0000 0000 0000  /;R_klmno.......
+000010d0: 0101 0000 0000 0000 000d 0000 0000 0000  ................
+000010e0: 0000 0000 0000 0000 008b 0000 000b 0063  ...............c
+000010f0: 006f 006d 006d 0061 006e 0064 006c 0069  .o.m.m.a.n.d.l.i
+00001100: 006e 0065 7653 726e 6c6f 6e67 0000 0001  .n.evSrnlong....
+00001110: 0000 0004 0063 006f 0072 0065 6277 7370  .....c.o.r.ebwsp
+00001120: 626c 6f62 0000 00b7 6270 6c69 7374 3030  blob....bplist00
+00001130: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
+00001140: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
+00001150: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
+00001160: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
+00001170: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
+00001180: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
+00001190: 6261 7208 0908 095f 1017 7b7b 3137 2c20  bar...._..{{17, 
+000011a0: 3430 357d 2c20 7b37 3836 2c20 3434 367d  405}, {786, 446}
+000011b0: 7d09 0815 232f 3b52 5f6b 6c6d 6e6f 8900  }...#/;R_klmno..
+000011c0: 0000 0000 0001 0100 0000 0000 0000 0d00  ................
+000011d0: 0000 0000 0000 0000 0000 0000 0000 8a00  ................
+000011e0: 0000 0400 6300 6f00 7200 6576 5372 6e6c  ....c.o.r.evSrnl
+000011f0: 6f6e 6700 0000 0100 0000 0200 6900 6f62  ong.........i.ob
+00001200: 7773 7062 6c6f 6200 0000 b762 706c 6973  wspblob....bplis
+00001210: 7430 30d6 0102 0304 0506 0708 0708 0b08  t00.............
+00001220: 5d53 686f 7753 7461 7475 7342 6172 5b53  ]ShowStatusBar[S
+00001230: 686f 7754 6f6f 6c62 6172 5b53 686f 7754  howToolbar[ShowT
+00001240: 6162 5669 6577 5f10 1443 6f6e 7461 696e  abView_..Contain
+00001250: 6572 5368 6f77 5369 6465 6261 725c 5769  erShowSidebar\Wi
+00001260: 6e64 6f77 426f 756e 6473 5b53 686f 7753  ndowBounds[ShowS
+00001270: 6964 6562 6172 0809 0809 5f10 177b 7b34  idebar...._..{{4
+00001280: 342c 2033 3934 7d2c 207b 3932 302c 2034  4, 394}, {920, 4
+00001290: 3436 7d7d 0908 1523 2f3b 525f 6b6c 6d6e  46}}...#/;R_klmn
+000012a0: 6f89 0000 0000 0000 0101 0000 0000 0000  o...............
+000012b0: 000d 0000 0000 0000 0000 0000 0000 0000  ................
+000012c0: 008a 0000 0002 0069 006f 7653 726e 6c6f  .......i.ovSrnlo
+000012d0: 6e67 0000 0001 0000 0004 0070 006c 006f  ng.........p.l.o
+000012e0: 0074 6277 7370 626c 6f62 0000 00b8 6270  .tbwspblob....bp
+000012f0: 6c69 7374 3030 d601 0203 0405 0607 0807  list00..........
+00001300: 080b 085d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
+00001310: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
+00001320: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
+00001330: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
+00001340: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
+00001350: 6f77 5369 6465 6261 7208 0908 095f 1018  owSidebar...._..
+00001360: 7b7b 3239 392c 2033 3635 7d2c 207b 3932  {{299, 365}, {92
+00001370: 302c 2034 3336 7d7d 0908 1523 2f3b 525f  0, 436}}...#/;R_
+00001380: 6b6c 6d6e 6f8a 0000 0000 0000 0101 0000  klmno...........
+00001390: 0000 0000 000d 0000 0000 0000 0000 0000  ................
+000013a0: 0000 0000 008b 0000 0004 0070 006c 006f  ...........p.l.o
+000013b0: 0074 7653 726e 6c6f 6e67 0000 0001 0000  .tvSrnlong......
+000013c0: 0005 0074 006f 006f 006c 0073 6277 7370  ...t.o.o.l.sbwsp
+000013d0: 626c 6f62 0000 00b8 6270 6c69 7374 3030  blob....bplist00
+000013e0: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
+000013f0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
+00001400: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
+00001410: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
+00001420: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
+00001430: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
+00001440: 6261 7208 0908 095f 1018 7b7b 3135 352c  bar...._..{{155,
+00001450: 2033 3634 7d2c 207b 3932 302c 2034 3336   364}, {920, 436
+00001460: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
+00001470: 0000 0000 0000 0101 0000 0000 0000 000d  ................
+00001480: 0000 0000 0000 0000 0000 0000 0000 008b  ................
+00001490: 0000 0005 0074 006f 006f 006c 0073 7653  .....t.o.o.l.svS
+000014a0: 726e 6c6f 6e67 0000 0001 0000 0009 0075  rnlong.........u
+000014b0: 0074 0069 006c 0069 0074 0069 0065 0073  .t.i.l.i.t.i.e.s
+000014c0: 6277 7370 626c 6f62 0000 00b7 6270 6c69  bwspblob....bpli
+000014d0: 7374 3030 d601 0203 0405 0607 0807 080b  st00............
+000014e0: 085d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
+000014f0: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
+00001500: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+00001510: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+00001520: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+00001530: 5369 6465 6261 7208 0908 095f 1017 7b7b  Sidebar...._..{{
+00001540: 3434 2c20 3339 347d 2c20 7b39 3230 2c20  44, 394}, {920, 
+00001550: 3434 367d 7d09 0815 232f 3b52 5f6b 6c6d  446}}...#/;R_klm
+00001560: 6e6f 8900 0000 0000 0001 0100 0000 0000  no..............
+00001570: 0000 0d00 0000 0000 0000 0000 0000 0000  ................
+00001580: 0000 8a00 0000 0900 7500 7400 6900 6c00  ........u.t.i.l.
+00001590: 6900 7400 6900 6500 7376 5372 6e6c 6f6e  i.t.i.e.svSrnlon
+000015a0: 6700 0000 0100 0000 0000 0000 0000 0000  g...............
 000015b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -457,26 +457,26 @@
 00001c80: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001c90: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 00001ca0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 00001cb0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
 00001cc0: 0000 0000 0101 0000 0000 0000 0102 0000  ................
 00001cd0: 0000 0000 0104 0000 0000 0000 0108 0000  ................
 00001ce0: 0000 0000 0110 0000 0000 0000 0120 0000  ............. ..
-00001cf0: 0000 0000 0140 0000 0000 0000 0054 6162  .....@.......Tab
-00001d00: 5669 6577 5f10 1443 6f6e 7461 696e 6572  View_..Container
-00001d10: 5368 6f77 5369 6465 6261 725c 5769 6e64  ShowSidebar\Wind
-00001d20: 6f77 426f 756e 6473 5b53 686f 7753 6964  owBounds[ShowSid
-00001d30: 6562 6172 0809 0809 5f10 177b 7b34 342c  ebar...._..{{44,
-00001d40: 2033 3934 7d2c 207b 3932 302c 2034 3436   394}, {920, 446
-00001d50: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f89  }}...#/;R_klmno.
-00001d60: 0000 0000 0000 0101 0000 0000 0000 000d  ................
-00001d70: 0000 0000 0000 0000 0000 0000 0000 008a  ................
-00001d80: 0000 0009 0075 0074 0069 006c 0069 0074  .....u.t.i.l.i.t
-00001d90: 0069 0065 0073 7653 726e 6c6f 6e67 0000  .i.e.svSrnlong..
-00001da0: 0001 0000 0000 0000 0000 0000 0000 0000  ................
+00001cf0: 0000 0000 0140 0000 0000 0000 0068 6f77  .....@.......how
+00001d00: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+00001d10: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+00001d20: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+00001d30: 5369 6465 6261 7208 0908 095f 1017 7b7b  Sidebar...._..{{
+00001d40: 3434 2c20 3339 347d 2c20 7b39 3230 2c20  44, 394}, {920, 
+00001d50: 3434 367d 7d09 0815 232f 3b52 5f6b 6c6d  446}}...#/;R_klm
+00001d60: 6e6f 8900 0000 0000 0001 0100 0000 0000  no..............
+00001d70: 0000 0d00 0000 0000 0000 0000 0000 0000  ................
+00001d80: 0000 8a00 0000 0900 7500 7400 6900 6c00  ........u.t.i.l.
+00001d90: 6900 7400 6900 6500 7376 5372 6e6c 6f6e  i.t.i.e.svSrnlon
+00001da0: 6700 0000 0100 0000 0000 0000 0000 0000  g...............
 00001db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `cfdna-2.0.5/cfdna/__init__.py` & `cfdna-2.0.7/cfdna/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from . import commandline as cmd
 from . import tools as tl
 
 from ngsfragments import Fragments
 
 
 # This is extracted automatically by the top-level setup.py.
-__version__ = '2.0.5'
+__version__ = '2.0.7'
 
 __author__ = "Kyle S. Smith"
 
 __doc__ = """\
 
 API
 ======
```

### Comparing `cfdna-2.0.5/cfdna/__main__.py` & `cfdna-2.0.7/cfdna/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import argparse
-from .commandline.commands import CNV_calling
+from .commandline.commands import CNV_calling, GeneActivity
 
 
 if __name__ == "__main__":
 
     parser = argparse.ArgumentParser()
     subparsers = parser.add_subparsers()
 
@@ -17,15 +17,38 @@
     parser_cnv.add_argument("--proportion", type=float, help="Proportion of fragments to use (default: 1.0)", default=1.0)
     parser_cnv.add_argument("--n_frags", type=int, help="Estimate of number of fragments to use (default: ALL)", default=0)
     parser_cnv.add_argument("--min_length", type=int, help="Minimum length to consider (default: 1)", default=1)
     parser_cnv.add_argument("--max_length", type=int, help="Maximum length to consider (default: 1000)", default=1000)
     parser_cnv.add_argument("--mapq", type=int, help="Mapping quality cutoff (default: 25)", default=25)
     parser_cnv.add_argument("--segs", help="Whether to write seg files (default: False)", default=False, action="store_true")
     parser_cnv.add_argument("--nthreads", type=int, help="Number of threads to use (default=1)", default=1)
+    parser_cnv.add_argument("--cache", help="Name of h5 file to append results to", default="")
     parser_cnv.add_argument("--single", help="Whether to reads are single ended (default: False)", default=False, action="store_true")
-    parser_cnv.add_argument("--qcfail", help="Whether to to remove qcfail flag (default: False)", default=False, action="store_true")
+    parser_cnv.add_argument("--qcfail", help="Whether to remove qcfail flag (default: False)", default=False, action="store_true")
+    parser_cnv.add_argument("--use_normal", help="Whether to correct using normal profiles (default: False)", default=False, action="store_true")
+    parser_cnv.add_argument("--add_wps", help="Whether to add a WPS plot for TSSs (default: False)", default=False, action="store_true")
+    parser_cnv.add_argument("--add_sex", help="Whether to keep sex chromosomes (default: False)", default=False, action="store_true")
+    parser_cnv.add_argument("--clonal", help="Whether to predict clonality (default: False)", default=False, action="store_true")
+    parser_cnv.add_argument("--anno_file", help="Whether to write text file with predictioned metrics (default: False)", default=False, action="store_true")
+    parser_cnv.add_argument("--anno_segs", help="Whether to annotated seg file (default: False)", default=False, action="store_true")
     parser_cnv.add_argument("--verbose", help="Whether to be verbose (default: False)", default=False, action="store_true")
     parser_cnv.set_defaults(func=CNV_calling)
 
+    # Call Gebe activity
+    parser_gene = subparsers.add_parser("geneActivity", help="Write gene activity")
+    parser_gene.add_argument("--bam", help="BAM file", required=True, nargs='*')
+    parser_gene.add_argument("--prefix", help="Prefix for ouput files", default="")
+    parser_gene.add_argument("--genome", help="Version of genome to use (default=hg19)", default="hg19")
+    parser_gene.add_argument("--feature", help="Feature to use (default=gene)", default="gene")
+    parser_gene.add_argument("--min_length", type=int, help="Minimum length to consider (default: 120)", default=120)
+    parser_gene.add_argument("--max_length", type=int, help="Maximum length to consider (default: 220)", default=220)
+    parser_gene.add_argument("--mapq", type=int, help="Mapping quality cutoff (default: 25)", default=25)
+    parser_gene.add_argument("--nthreads", type=int, help="Number of threads to use (default=1)", default=1)
+    parser_gene.add_argument("--cache", help="Name of h5 file to append results to", default="")
+    parser_gene.add_argument("--single", help="Whether to reads are single ended (default: False)", default=False, action="store_true")
+    parser_gene.add_argument("--qcfail", help="Whether to remove qcfail flag (default: False)", default=False, action="store_true")
+    parser_gene.add_argument("--verbose", help="Whether to be verbose (default: False)", default=False, action="store_true")
+    parser_gene.set_defaults(func=GeneActivity)
+
     args = parser.parse_args()
 
     args.func(args)
```

### Comparing `cfdna-2.0.5/cfdna/core/core.py` & `cfdna-2.0.7/cfdna/core/core.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.5/cfdna/io/.DS_Store` & `cfdna-2.0.7/cfdna/io/.DS_Store`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.5/cfdna/io/read/read_bam.py` & `cfdna-2.0.7/cfdna/io/read/read_bam.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.5/cfdna/io/write/write_text.py` & `cfdna-2.0.7/cfdna/io/write/write_text.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.5/cfdna/plot/plot_bokeh.py` & `cfdna-2.0.7/cfdna/plot/plot_bokeh.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.5/cfdna/plot/plot_plt.py` & `cfdna-2.0.7/cfdna/plot/plot_plt.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.5/cfdna/tools/cnv/segmentation.py` & `cfdna-2.0.7/cfdna/tools/cnv/segmentation.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.5/cfdna/tools/coverage/gene_activity.py` & `cfdna-2.0.7/cfdna/tools/coverage/gene_activity.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,27 +5,28 @@
 
 def gene_activity(frags: Fragments,
                   cfdna_object: cfDNA,
                   genome_version: str = "hg19",
                   feature: str = "gene",
                   min_length: int = 120,
                   max_length: int = 220,
-                  verbose: bool = False):
+                  verbose: bool = False) -> cfDNA:
     """
     """
 
     # Get gene activity
     gene_activity = ngs.metrics.gene_activity(frags,
                                             genome_version=genome_version,
                                             feature=feature,
                                             min_length=min_length,
                                             max_length=max_length,
                                             verbose=verbose)
-    gene_activity = ngs.metric.correct_gene_activity(frags,
+    gene_activity = ngs.metrics.correct_gene_activity(frags,
                                                      gene_activity,
                                                      correct_cnv = False,
                                                      genome_version = genome_version,
                                                      feature = feature,
                                                      verbose = verbose)
 
     cfdna_object.add_values("gene_activity", gene_activity)
 
+    return cfdna_object
```

### Comparing `cfdna-2.0.5/cfdna/tools/fragmentation/frag_pattern.py` & `cfdna-2.0.7/cfdna/tools/fragmentation/frag_pattern.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.5/cfdna/tools/nucleosome/gene_activity.py` & `cfdna-2.0.7/cfdna/tools/nucleosome/gene_activity.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.5/cfdna/tools/nucleosome/nfr.py` & `cfdna-2.0.7/cfdna/tools/nucleosome/nfr.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.5/cfdna/tools/nucleosome/relative_window.py` & `cfdna-2.0.7/cfdna/tools/nucleosome/relative_window.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.5/cfdna/tools/nucleosome/wps.py` & `cfdna-2.0.7/cfdna/tools/nucleosome/wps.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.5/cfdna/tools/nucleosome/wps_functions.py` & `cfdna-2.0.7/cfdna/tools/nucleosome/wps_functions.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.5/cfdna/tools/summarize/multi_sample.py` & `cfdna-2.0.7/cfdna/tools/summarize/multi_sample.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.5/cfdna/tools/summarize/summarize.py` & `cfdna-2.0.7/cfdna/tools/summarize/summarize.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.5/cfdna/utilities/h5_utilities.py` & `cfdna-2.0.7/cfdna/utilities/h5_utilities.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.5/pyproject.toml` & `cfdna-2.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cfdna"
-version = "2.0.5"
+version = "2.0.7"
 description = "Python package for fragment manipulation for cfDNA"
 authors = ["Kyle S. Smith <kyle.smith@stjude.org>"]
 maintainers = ["Kyle S. Smith <kyle.smith@stjude.org>"]
 repository = "https://github.com/kylessmith/cfdna"
 documentation = "https://www.biosciencestack.com/static/cfdna/docs/index.html"
 keywords = ["cython", "interval", "cfdna", "c"]
 readme = 'README.md'
@@ -27,43 +27,43 @@
 packages = [{ include = "cfdna" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.23.5"
 cython = "^0.29.32"
 pandas = "^1.5.2"
-ailist = "^2.1.0"
+ailist = "^2.1.2"
 linear_segment = "^1.1.0"
 pysam = "^0.21.0"
-intervalframe = "^1.1.3"
+intervalframe = "^1.1.5"
 matplotlib = "^3.7.1"
 bokeh = "^3.1.0"
 scipy = "^1.9.1"
 statsmodels = "^0.13.5"
 seaborn = "^0.12.2"
 projectframe = "^1.0.0"
 hmmCNV = "^1.0.1"
 scikit-learn = "^1.2.2"
-ngsfragments = "^2.1.1"
-genome_info = "^1.0.2"
+ngsfragments = "^2.1.5"
+genome_info = "^1.0.4"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0",
             "cython>=0.29.32",
             "numpy>=1.23.5",
             "pandas>=1.5.2",
             "setuptools>=65.5.0",
-            "ailist>=2.1.0",
+            "ailist>=2.1.2",
             "pysam>=0.20.0",
-            "genome_info>=1.0.2",
-            "intervalframe>=1.1.3",
-            "ngsfragments>=2.1.1"]
+            "genome_info>=1.0.4",
+            "intervalframe>=1.1.5",
+            "ngsfragments>=2.1.5"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.build]
 generate-setup-file = false
 #script = "build.py"
 
 [tool.cibuildwheel]
```

### Comparing `cfdna-2.0.5/PKG-INFO` & `cfdna-2.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfdna
-Version: 2.0.5
+Version: 2.0.7
 Summary: Python package for fragment manipulation for cfDNA
 Home-page: https://github.com/kylessmith/cfdna
 License: GPL-2.0-or-later
 Keywords: cython,interval,cfdna,c
 Author: Kyle S. Smith
 Author-email: kyle.smith@stjude.org
 Maintainer: Kyle S. Smith
@@ -24,23 +24,23 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: ailist (>=2.1.0,<3.0.0)
+Requires-Dist: ailist (>=2.1.2,<3.0.0)
 Requires-Dist: bokeh (>=3.1.0,<4.0.0)
 Requires-Dist: cython (>=0.29.32,<0.30.0)
-Requires-Dist: genome_info (>=1.0.2,<2.0.0)
+Requires-Dist: genome_info (>=1.0.4,<2.0.0)
 Requires-Dist: hmmCNV (>=1.0.1,<2.0.0)
-Requires-Dist: intervalframe (>=1.1.3,<2.0.0)
+Requires-Dist: intervalframe (>=1.1.5,<2.0.0)
 Requires-Dist: linear_segment (>=1.1.0,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: ngsfragments (>=2.1.1,<3.0.0)
+Requires-Dist: ngsfragments (>=2.1.5,<3.0.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: pandas (>=1.5.2,<2.0.0)
 Requires-Dist: projectframe (>=1.0.0,<2.0.0)
 Requires-Dist: pysam (>=0.21.0,<0.22.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: scipy (>=1.9.1,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
@@ -67,15 +67,15 @@
     https://continuum.io/downloads
 ```
 
 Create environment and pip install:
 ```
     conda create -n cfdna python=3.11.3
 	conda activate cfdna
-	pip install cfdna
+	pip install cfdna==2.0.5
 ```
 
 Dependencies can be installed by:
 
 ```
     pip install -r requirements.txt
 ```
```

