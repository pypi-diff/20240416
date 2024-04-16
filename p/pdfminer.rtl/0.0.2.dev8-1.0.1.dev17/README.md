# Comparing `tmp/pdfminer_rtl-0.0.2.dev8.tar.gz` & `tmp/pdfminer.rtl-1.0.1.dev17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfminer_rtl-0.0.2.dev8.tar", last modified: Mon Apr 15 15:08:48 2024, max compression
+gzip compressed data, was "pdfminer.rtl-1.0.1.dev17.tar", last modified: Tue Apr 16 13:49:11 2024, max compression
```

## Comparing `pdfminer_rtl-0.0.2.dev8.tar` & `pdfminer.rtl-1.0.1.dev17.tar`

### file list

```diff
@@ -1,230 +1,232 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 15:08:48.967997 pdfminer_rtl-0.0.2.dev8/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16518 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/CHANGELOG.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2662 2024-04-15 13:22:04.000000 pdfminer_rtl-0.0.2.dev8/CONTRIBUTING.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1093 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      160 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1141 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/Makefile
--rw-r--r--   0 codespace  (1000) codespace  (1000)     3358 2024-04-15 15:08:48.967997 pdfminer_rtl-0.0.2.dev8/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1766 2024-04-15 13:34:22.000000 pdfminer_rtl-0.0.2.dev8/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 15:08:48.863997 pdfminer_rtl-0.0.2.dev8/cmaprsrc/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2917 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/cmaprsrc/README.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)  2046762 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/cmaprsrc/cid2code_Adobe_CNS1.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)  1900416 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/cmaprsrc/cid2code_Adobe_GB1.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)  2681742 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/cmaprsrc/cid2code_Adobe_Japan1.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)  1028252 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/cmaprsrc/cid2code_Adobe_Korea1.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1310 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/noxfile.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 15:08:48.887997 pdfminer_rtl-0.0.2.dev8/pdfminer/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      260 2024-04-15 13:20:38.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3600 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/_saslprep.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      929 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/arcfour.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2097 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/ascii85.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21391 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/ccitt.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 15:08:48.959997 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20532 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/78-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20551 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/78-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19882 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/78-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22969 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/78-RKSJ-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22990 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/78-RKSJ-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19883 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/78-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25942 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/78ms-RKSJ-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25964 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/78ms-RKSJ-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    26305 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/83pv-RKSJ-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    26305 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/83pv-RKSJ-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25732 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/90ms-RKSJ-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25757 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/90ms-RKSJ-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25670 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/90msp-RKSJ-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25688 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/90msp-RKSJ-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24226 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/90pv-RKSJ-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24021 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/90pv-RKSJ-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21027 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/Add-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24275 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/Add-RKSJ-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24079 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/Add-RKSJ-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20874 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/Add-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    42594 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    42549 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    42602 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/B5pc-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    42557 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/B5pc-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    56990 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/CNS-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    56943 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/CNS-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17615 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/CNS1-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17564 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/CNS1-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21723 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/CNS2-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21723 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/CNS2-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    59548 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/ETHK-B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    59481 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/ETHK-B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    43982 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/ETen-B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    43924 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/ETen-B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      320 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/ETenms-B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      438 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/ETenms-B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20429 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20455 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22272 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/Ext-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25721 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/Ext-RKSJ-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25750 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/Ext-RKSJ-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22307 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/Ext-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22118 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GB-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22111 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GB-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21699 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GB-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21694 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GB-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    68254 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBK-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    68199 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBK-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    89917 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBK2K-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    89872 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBK2K-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    68148 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBKp-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    68102 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBKp-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23815 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBT-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23806 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBT-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23339 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBT-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23322 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBT-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23650 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBTpc-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23647 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBTpc-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21945 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBpc-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21956 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBpc-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19781 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    45212 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/HKdla-B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    45167 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/HKdla-B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    44853 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/HKdlb-B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    44816 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/HKdlb-B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    53104 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/HKgccs-B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    53050 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/HKgccs-B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    43667 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/HKm314-B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    43618 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/HKm314-B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    44187 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/HKm471-B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    44144 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/HKm471-B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    59508 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/HKscs-B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    59473 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/HKscs-B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      840 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/Hankaku-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      839 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/Hankaku-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      391 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/Hiragana-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      391 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/Hiragana-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24040 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/KSC-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24078 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/KSC-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23563 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/KSC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    55016 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/KSC-Johab-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    55041 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/KSC-Johab-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23644 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/KSC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    51667 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/KSCms-UHC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    51788 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/KSCms-UHC-HW-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    51821 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/KSCms-UHC-HW-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    51698 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/KSCms-UHC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    27769 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/KSCpc-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    27820 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/KSCpc-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      404 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/Katakana-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      404 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/Katakana-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21708 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/NWP-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21779 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/NWP-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3917 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/README.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23030 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/RKSJ-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23048 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/RKSJ-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      394 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/Roman-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      394 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/Roman-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    67459 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniCNS-UCS2-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    67395 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniCNS-UCS2-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    87819 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniCNS-UTF16-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    87751 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniCNS-UTF16-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    87400 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniCNS-UTF32-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    87327 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniCNS-UTF32-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    82631 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniCNS-UTF8-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    82562 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniCNS-UTF8-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    97445 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniGB-UCS2-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    97441 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniGB-UCS2-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   101459 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniGB-UTF16-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   101331 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniGB-UTF16-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   101490 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniGB-UTF32-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   101357 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniGB-UTF32-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    90500 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniGB-UTF8-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    90368 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniGB-UTF8-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35934 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS-UCS2-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      412 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS-UCS2-HW-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1402 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS-UCS2-HW-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35852 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS-UCS2-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    58054 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS-UTF16-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57928 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS-UTF16-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57910 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS-UTF32-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57780 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS-UTF32-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54764 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS-UTF8-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54684 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS-UTF8-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    58081 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS2004-UTF16-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57960 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS2004-UTF16-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57940 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS2004-UTF32-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57811 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS2004-UTF32-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54829 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS2004-UTF8-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54749 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS2004-UTF8-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57903 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJISX0213-UTF32-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57778 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJISX0213-UTF32-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57930 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJISX02132004-UTF32-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57808 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJISX02132004-UTF32-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    60683 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniKS-UCS2-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    60699 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniKS-UCS2-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    61278 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniKS-UTF16-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    61298 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniKS-UTF16-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    61286 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniKS-UTF32-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    61309 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniKS-UTF32-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54151 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniKS-UTF8-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54172 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniKS-UTF8-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19826 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      505 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/WP-Symbol-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      505 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/WP-Symbol-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   138237 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/to-unicode-Adobe-CNS1.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   204425 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/to-unicode-Adobe-GB1.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   112987 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/to-unicode-Adobe-Japan1.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   120859 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/to-unicode-Adobe-Korea1.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16052 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/cmapdb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35934 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/converter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1654 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/data_structures.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3983 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/encodingdb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   112611 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/fontmetrics.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   130804 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/glyphlist.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7276 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/high_level.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9165 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/image.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11391 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/jbig2.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8531 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/latin_enc.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    39241 2024-04-15 15:08:29.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/layout.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3177 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/lzw.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      821 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/pdfcolor.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8787 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/pdfdevice.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    37267 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/pdfdocument.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    37946 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/pdffont.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34539 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/pdfinterp.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6932 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/pdfpage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5896 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/pdfparser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11965 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/pdftypes.py
--rwxrwxrwx   0 codespace  (1000) codespace  (1000)    19890 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/psparser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/py.typed
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1358 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/runlength.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       15 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/settings.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20804 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/pdfminer/utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 15:08:48.967997 pdfminer_rtl-0.0.2.dev8/pdfminer.rtl.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     3358 2024-04-15 15:08:48.000000 pdfminer_rtl-0.0.2.dev8/pdfminer.rtl.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6909 2024-04-15 15:08:48.000000 pdfminer_rtl-0.0.2.dev8/pdfminer.rtl.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-15 15:08:48.000000 pdfminer_rtl-0.0.2.dev8/pdfminer.rtl.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      206 2024-04-15 15:08:48.000000 pdfminer_rtl-0.0.2.dev8/pdfminer.rtl.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2024-04-15 15:08:48.000000 pdfminer_rtl-0.0.2.dev8/pdfminer.rtl.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-04-15 15:08:48.967997 pdfminer_rtl-0.0.2.dev8/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2104 2024-04-15 13:49:59.000000 pdfminer_rtl-0.0.2.dev8/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 15:08:48.963997 pdfminer_rtl-0.0.2.dev8/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9692 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/tests/test_converter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5420 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/tests/test_encodingdb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      779 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/tests/test_font_size.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7694 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/tests/test_highlevel_extracttext.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5038 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/tests/test_layout.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1809 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/tests/test_pdfdocument.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3972 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/tests/test_pdfencoding.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      604 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/tests/test_pdffont.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4532 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/tests/test_pdfminer_ccitt.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1598 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/tests/test_pdfminer_crypto.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3730 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/tests/test_pdfminer_psparser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      582 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/tests/test_pdfpage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1505 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/tests/test_tools_dumppdf.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5766 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/tests/test_tools_pdf2txt.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3912 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/tests/test_utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 15:08:48.967997 pdfminer_rtl-0.0.2.dev8/tools/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/tools/__init__.py
--rwxrwxrwx   0 codespace  (1000) codespace  (1000)     1646 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/tools/conv_afm.py
--rwxrwxrwx   0 codespace  (1000) codespace  (1000)     6089 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/tools/conv_cmap.py
--rwxrwxrwx   0 codespace  (1000) codespace  (1000)      911 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/tools/conv_glyphlist.py
--rwxrwxrwx   0 codespace  (1000) codespace  (1000)    14316 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/tools/dumppdf.py
--rwxrwxrwx   0 codespace  (1000) codespace  (1000)     9779 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/tools/pdf2txt.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6266 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/tools/pdfdiff.py
--rwxrwxrwx   0 codespace  (1000) codespace  (1000)     2761 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/tools/pdfstats.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1415 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev8/tools/prof.py
+drwxr-xr-x   0 trn        (501) staff       (20)        0 2024-04-16 13:49:11.676719 pdfminer.rtl-1.0.1.dev17/
+-rw-r--r--   0 trn        (501) staff       (20)    16518 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/CHANGELOG.md
+-rw-r--r--   0 trn        (501) staff       (20)     2662 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/CONTRIBUTING.md
+-rw-r--r--   0 trn        (501) staff       (20)     1093 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/LICENSE
+-rw-r--r--   0 trn        (501) staff       (20)      160 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/MANIFEST.in
+-rw-r--r--   0 trn        (501) staff       (20)     1141 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/Makefile
+-rw-r--r--   0 trn        (501) staff       (20)     2860 2024-04-16 13:49:11.676038 pdfminer.rtl-1.0.1.dev17/PKG-INFO
+-rw-r--r--   0 trn        (501) staff       (20)     1766 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/README.md
+drwxr-xr-x   0 trn        (501) staff       (20)        0 2024-04-16 13:49:11.398679 pdfminer.rtl-1.0.1.dev17/cmaprsrc/
+-rw-r--r--   0 trn        (501) staff       (20)     2917 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/cmaprsrc/README.txt
+-rw-r--r--   0 trn        (501) staff       (20)  2046762 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/cmaprsrc/cid2code_Adobe_CNS1.txt
+-rw-r--r--   0 trn        (501) staff       (20)  1900416 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/cmaprsrc/cid2code_Adobe_GB1.txt
+-rw-r--r--   0 trn        (501) staff       (20)  2681742 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/cmaprsrc/cid2code_Adobe_Japan1.txt
+-rw-r--r--   0 trn        (501) staff       (20)  1028252 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/cmaprsrc/cid2code_Adobe_Korea1.txt
+-rw-r--r--   0 trn        (501) staff       (20)     1310 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/noxfile.py
+drwxr-xr-x   0 trn        (501) staff       (20)        0 2024-04-16 13:49:11.422459 pdfminer.rtl-1.0.1.dev17/pdfminer/
+-rw-r--r--   0 trn        (501) staff       (20)      260 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/__init__.py
+-rw-r--r--   0 trn        (501) staff       (20)     3600 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/_saslprep.py
+-rw-r--r--   0 trn        (501) staff       (20)    21819 2024-04-16 13:48:18.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/algorithm.py
+-rw-r--r--   0 trn        (501) staff       (20)      929 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/arcfour.py
+-rw-r--r--   0 trn        (501) staff       (20)     2097 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/ascii85.py
+-rw-r--r--   0 trn        (501) staff       (20)    21391 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/ccitt.py
+drwxr-xr-x   0 trn        (501) staff       (20)        0 2024-04-16 13:49:11.599878 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/
+-rw-r--r--   0 trn        (501) staff       (20)    20532 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/78-EUC-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    20551 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/78-EUC-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    19882 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/78-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    22969 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/78-RKSJ-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    22990 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/78-RKSJ-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    19883 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/78-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    25942 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/78ms-RKSJ-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    25964 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/78ms-RKSJ-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    26305 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/83pv-RKSJ-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    26305 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/83pv-RKSJ-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    25732 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/90ms-RKSJ-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    25757 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/90ms-RKSJ-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    25670 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/90msp-RKSJ-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    25688 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/90msp-RKSJ-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    24226 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/90pv-RKSJ-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    24021 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/90pv-RKSJ-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    21027 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/Add-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    24275 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/Add-RKSJ-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    24079 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/Add-RKSJ-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    20874 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/Add-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    42594 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/B5-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    42549 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/B5-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    42602 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/B5pc-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    42557 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/B5pc-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    56990 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/CNS-EUC-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    56943 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/CNS-EUC-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    17615 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/CNS1-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    17564 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/CNS1-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    21723 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/CNS2-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    21723 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/CNS2-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    59548 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/ETHK-B5-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    59481 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/ETHK-B5-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    43982 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/ETen-B5-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    43924 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/ETen-B5-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)      320 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/ETenms-B5-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)      438 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/ETenms-B5-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    20429 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/EUC-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    20455 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/EUC-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    22272 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/Ext-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    25721 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/Ext-RKSJ-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    25750 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/Ext-RKSJ-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    22307 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/Ext-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    22118 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GB-EUC-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    22111 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GB-EUC-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    21699 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GB-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    21694 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GB-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    68254 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBK-EUC-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    68199 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBK-EUC-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    89917 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBK2K-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    89872 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBK2K-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    68148 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBKp-EUC-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    68102 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBKp-EUC-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    23815 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBT-EUC-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    23806 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBT-EUC-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    23339 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBT-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    23322 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBT-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    23650 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBTpc-EUC-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    23647 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBTpc-EUC-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    21945 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBpc-EUC-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    21956 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBpc-EUC-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    19781 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    45212 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/HKdla-B5-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    45167 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/HKdla-B5-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    44853 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/HKdlb-B5-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    44816 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/HKdlb-B5-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    53104 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/HKgccs-B5-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    53050 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/HKgccs-B5-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    43667 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/HKm314-B5-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    43618 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/HKm314-B5-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    44187 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/HKm471-B5-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    44144 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/HKm471-B5-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    59508 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/HKscs-B5-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    59473 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/HKscs-B5-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)      840 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/Hankaku-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)      839 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/Hankaku-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)      391 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/Hiragana-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)      391 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/Hiragana-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    24040 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/KSC-EUC-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    24078 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/KSC-EUC-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    23563 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/KSC-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    55016 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/KSC-Johab-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    55041 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/KSC-Johab-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    23644 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/KSC-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    51667 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/KSCms-UHC-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    51788 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/KSCms-UHC-HW-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    51821 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/KSCms-UHC-HW-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    51698 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/KSCms-UHC-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    27769 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/KSCpc-EUC-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    27820 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/KSCpc-EUC-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)      404 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/Katakana-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)      404 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/Katakana-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    21708 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/NWP-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    21779 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/NWP-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)     3917 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/README.txt
+-rw-r--r--   0 trn        (501) staff       (20)    23030 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/RKSJ-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    23048 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/RKSJ-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)      394 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/Roman-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)      394 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/Roman-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    67459 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniCNS-UCS2-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    67395 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniCNS-UCS2-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    87819 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniCNS-UTF16-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    87751 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniCNS-UTF16-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    87400 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniCNS-UTF32-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    87327 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniCNS-UTF32-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    82631 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniCNS-UTF8-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    82562 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniCNS-UTF8-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    97445 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniGB-UCS2-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    97441 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniGB-UCS2-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)   101459 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniGB-UTF16-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)   101331 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniGB-UTF16-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)   101490 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniGB-UTF32-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)   101357 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniGB-UTF32-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    90500 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniGB-UTF8-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    90368 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniGB-UTF8-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    35934 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS-UCS2-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)      412 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS-UCS2-HW-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)     1402 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS-UCS2-HW-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    35852 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS-UCS2-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    58054 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS-UTF16-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    57928 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS-UTF16-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    57910 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS-UTF32-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    57780 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS-UTF32-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    54764 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS-UTF8-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    54684 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS-UTF8-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    58081 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS2004-UTF16-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    57960 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS2004-UTF16-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    57940 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS2004-UTF32-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    57811 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS2004-UTF32-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    54829 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS2004-UTF8-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    54749 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS2004-UTF8-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    57903 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJISX0213-UTF32-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    57778 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJISX0213-UTF32-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    57930 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJISX02132004-UTF32-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    57808 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJISX02132004-UTF32-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    60683 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniKS-UCS2-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    60699 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniKS-UCS2-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    61278 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniKS-UTF16-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    61298 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniKS-UTF16-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    61286 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniKS-UTF32-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    61309 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniKS-UTF32-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    54151 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniKS-UTF8-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    54172 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniKS-UTF8-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    19826 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)      505 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/WP-Symbol-H.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)      505 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/WP-Symbol-V.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)   138237 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/to-unicode-Adobe-CNS1.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)   204425 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/to-unicode-Adobe-GB1.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)   112987 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/to-unicode-Adobe-Japan1.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)   120859 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/to-unicode-Adobe-Korea1.pickle.gz
+-rw-r--r--   0 trn        (501) staff       (20)    16052 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/cmapdb.py
+-rw-r--r--   0 trn        (501) staff       (20)    35934 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/converter.py
+-rw-r--r--   0 trn        (501) staff       (20)     1654 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/data_structures.py
+-rw-r--r--   0 trn        (501) staff       (20)     3983 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/encodingdb.py
+-rw-r--r--   0 trn        (501) staff       (20)   112611 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/fontmetrics.py
+-rw-r--r--   0 trn        (501) staff       (20)   130804 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/glyphlist.py
+-rw-r--r--   0 trn        (501) staff       (20)     7276 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/high_level.py
+-rw-r--r--   0 trn        (501) staff       (20)     9165 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/image.py
+-rw-r--r--   0 trn        (501) staff       (20)    11391 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/jbig2.py
+-rw-r--r--   0 trn        (501) staff       (20)     8531 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/latin_enc.py
+-rw-r--r--   0 trn        (501) staff       (20)    39514 2024-04-16 13:48:18.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/layout.py
+-rw-r--r--   0 trn        (501) staff       (20)     3177 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/lzw.py
+-rw-r--r--   0 trn        (501) staff       (20)    22542 2024-04-16 13:48:18.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/mirror.py
+-rw-r--r--   0 trn        (501) staff       (20)      821 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/pdfcolor.py
+-rw-r--r--   0 trn        (501) staff       (20)     8787 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/pdfdevice.py
+-rw-r--r--   0 trn        (501) staff       (20)    37267 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/pdfdocument.py
+-rw-r--r--   0 trn        (501) staff       (20)    37946 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/pdffont.py
+-rw-r--r--   0 trn        (501) staff       (20)    34539 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/pdfinterp.py
+-rw-r--r--   0 trn        (501) staff       (20)     6932 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/pdfpage.py
+-rw-r--r--   0 trn        (501) staff       (20)     5896 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/pdfparser.py
+-rw-r--r--   0 trn        (501) staff       (20)    11965 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/pdftypes.py
+-rwxr-xr-x   0 trn        (501) staff       (20)    19890 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/psparser.py
+-rw-r--r--   0 trn        (501) staff       (20)        0 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/py.typed
+-rw-r--r--   0 trn        (501) staff       (20)     1358 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/runlength.py
+-rw-r--r--   0 trn        (501) staff       (20)       15 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/settings.py
+-rw-r--r--   0 trn        (501) staff       (20)    20804 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/pdfminer/utils.py
+drwxr-xr-x   0 trn        (501) staff       (20)        0 2024-04-16 13:49:11.425338 pdfminer.rtl-1.0.1.dev17/pdfminer.rtl.egg-info/
+-rw-r--r--   0 trn        (501) staff       (20)     2860 2024-04-16 13:49:11.000000 pdfminer.rtl-1.0.1.dev17/pdfminer.rtl.egg-info/PKG-INFO
+-rw-r--r--   0 trn        (501) staff       (20)     6950 2024-04-16 13:49:11.000000 pdfminer.rtl-1.0.1.dev17/pdfminer.rtl.egg-info/SOURCES.txt
+-rw-r--r--   0 trn        (501) staff       (20)        1 2024-04-16 13:49:11.000000 pdfminer.rtl-1.0.1.dev17/pdfminer.rtl.egg-info/dependency_links.txt
+-rw-r--r--   0 trn        (501) staff       (20)      194 2024-04-16 13:49:11.000000 pdfminer.rtl-1.0.1.dev17/pdfminer.rtl.egg-info/requires.txt
+-rw-r--r--   0 trn        (501) staff       (20)        9 2024-04-16 13:49:11.000000 pdfminer.rtl-1.0.1.dev17/pdfminer.rtl.egg-info/top_level.txt
+-rw-r--r--   0 trn        (501) staff       (20)       38 2024-04-16 13:49:11.676863 pdfminer.rtl-1.0.1.dev17/setup.cfg
+-rw-r--r--   0 trn        (501) staff       (20)     2106 2024-04-16 13:48:18.000000 pdfminer.rtl-1.0.1.dev17/setup.py
+drwxr-xr-x   0 trn        (501) staff       (20)        0 2024-04-16 13:49:11.665500 pdfminer.rtl-1.0.1.dev17/tests/
+-rw-r--r--   0 trn        (501) staff       (20)     9692 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/tests/test_converter.py
+-rw-r--r--   0 trn        (501) staff       (20)     5420 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/tests/test_encodingdb.py
+-rw-r--r--   0 trn        (501) staff       (20)      779 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/tests/test_font_size.py
+-rw-r--r--   0 trn        (501) staff       (20)     7694 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/tests/test_highlevel_extracttext.py
+-rw-r--r--   0 trn        (501) staff       (20)     5038 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/tests/test_layout.py
+-rw-r--r--   0 trn        (501) staff       (20)     1809 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/tests/test_pdfdocument.py
+-rw-r--r--   0 trn        (501) staff       (20)     3972 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/tests/test_pdfencoding.py
+-rw-r--r--   0 trn        (501) staff       (20)      604 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/tests/test_pdffont.py
+-rw-r--r--   0 trn        (501) staff       (20)     4532 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/tests/test_pdfminer_ccitt.py
+-rw-r--r--   0 trn        (501) staff       (20)     1598 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/tests/test_pdfminer_crypto.py
+-rw-r--r--   0 trn        (501) staff       (20)     3730 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/tests/test_pdfminer_psparser.py
+-rw-r--r--   0 trn        (501) staff       (20)      582 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/tests/test_pdfpage.py
+-rw-r--r--   0 trn        (501) staff       (20)     1505 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/tests/test_tools_dumppdf.py
+-rw-r--r--   0 trn        (501) staff       (20)     5766 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/tests/test_tools_pdf2txt.py
+-rw-r--r--   0 trn        (501) staff       (20)     3912 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/tests/test_utils.py
+drwxr-xr-x   0 trn        (501) staff       (20)        0 2024-04-16 13:49:11.675170 pdfminer.rtl-1.0.1.dev17/tools/
+-rw-r--r--   0 trn        (501) staff       (20)        0 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/tools/__init__.py
+-rwxr-xr-x   0 trn        (501) staff       (20)     1646 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/tools/conv_afm.py
+-rwxr-xr-x   0 trn        (501) staff       (20)     6089 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/tools/conv_cmap.py
+-rwxr-xr-x   0 trn        (501) staff       (20)      911 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/tools/conv_glyphlist.py
+-rwxr-xr-x   0 trn        (501) staff       (20)    14316 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/tools/dumppdf.py
+-rwxr-xr-x   0 trn        (501) staff       (20)     9779 2024-04-16 11:42:07.000000 pdfminer.rtl-1.0.1.dev17/tools/pdf2txt.py
+-rw-r--r--   0 trn        (501) staff       (20)     6266 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/tools/pdfdiff.py
+-rwxr-xr-x   0 trn        (501) staff       (20)     2761 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/tools/pdfstats.py
+-rw-r--r--   0 trn        (501) staff       (20)     1415 2024-04-15 15:24:38.000000 pdfminer.rtl-1.0.1.dev17/tools/prof.py
```

### Comparing `pdfminer_rtl-0.0.2.dev8/CHANGELOG.md` & `pdfminer.rtl-1.0.1.dev17/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/CONTRIBUTING.md` & `pdfminer.rtl-1.0.1.dev17/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/LICENSE` & `pdfminer.rtl-1.0.1.dev17/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/Makefile` & `pdfminer.rtl-1.0.1.dev17/Makefile`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/PKG-INFO` & `pdfminer.rtl-1.0.1.dev17/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfminer.rtl
-Version: 0.0.2.dev8
+Version: 1.0.1.dev17
 Summary: PDF parser and analyzer
 Home-page: https://github.com/taneron/pdfminerrtl
 Author: Yusuke Shinyama + Philippe Guglielmetti + Taner
 Author-email: pdfminerrtl@rust.8shield.net
 License: MIT
 Keywords: pdf parser,pdf converter,layout analysis,text mining
 Classifier: Programming Language :: Python
@@ -18,30 +18,18 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Text Processing
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: charset-normalizer>=2.0.0
-Requires-Dist: cryptography>=36.0.0
-Requires-Dist: typing_extensions; python_version < "3.8"
-Requires-Dist: importlib_metadata; python_version < "3.8"
-Requires-Dist: python-bidi
 Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: nox; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: mypy==0.931; extra == "dev"
 Provides-Extra: docs
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: sphinx-argparse; extra == "docs"
 Provides-Extra: image
-Requires-Dist: Pillow; extra == "image"
+License-File: LICENSE
 
 pdfminer.rtl
 ============
 
 
 This is a fork of pdfminer.six that attempts to add RTL support with python-bidi. This version is experimental and probably buggy. Please don't rely on it for critical projects.
```

### Comparing `pdfminer_rtl-0.0.2.dev8/README.md` & `pdfminer.rtl-1.0.1.dev17/README.md`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/cmaprsrc/README.txt` & `pdfminer.rtl-1.0.1.dev17/cmaprsrc/README.txt`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/cmaprsrc/cid2code_Adobe_CNS1.txt` & `pdfminer.rtl-1.0.1.dev17/cmaprsrc/cid2code_Adobe_CNS1.txt`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/cmaprsrc/cid2code_Adobe_GB1.txt` & `pdfminer.rtl-1.0.1.dev17/cmaprsrc/cid2code_Adobe_GB1.txt`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/cmaprsrc/cid2code_Adobe_Japan1.txt` & `pdfminer.rtl-1.0.1.dev17/cmaprsrc/cid2code_Adobe_Japan1.txt`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/cmaprsrc/cid2code_Adobe_Korea1.txt` & `pdfminer.rtl-1.0.1.dev17/cmaprsrc/cid2code_Adobe_Korea1.txt`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/noxfile.py` & `pdfminer.rtl-1.0.1.dev17/noxfile.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/_saslprep.py` & `pdfminer.rtl-1.0.1.dev17/pdfminer/_saslprep.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/arcfour.py` & `pdfminer.rtl-1.0.1.dev17/pdfminer/arcfour.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/ascii85.py` & `pdfminer.rtl-1.0.1.dev17/pdfminer/ascii85.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/ccitt.py` & `pdfminer.rtl-1.0.1.dev17/pdfminer/ccitt.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/78-EUC-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/78-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/78-EUC-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/78-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/78-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/78-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/78-RKSJ-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/78-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/78-RKSJ-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/78-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/78-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/78-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/78ms-RKSJ-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/78ms-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/78ms-RKSJ-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/78ms-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/83pv-RKSJ-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/83pv-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/83pv-RKSJ-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/83pv-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/90ms-RKSJ-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/90ms-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/90ms-RKSJ-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/90ms-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/90msp-RKSJ-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/90msp-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/90msp-RKSJ-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/90msp-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/90pv-RKSJ-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/90pv-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/90pv-RKSJ-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/90pv-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/Add-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/Add-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/Add-RKSJ-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/Add-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/Add-RKSJ-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/Add-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/Add-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/Add-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/B5-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/B5-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/B5pc-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/B5pc-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/B5pc-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/B5pc-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/CNS-EUC-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/CNS-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/CNS-EUC-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/CNS-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/CNS1-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/CNS1-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/CNS1-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/CNS1-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/CNS2-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/CNS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/CNS2-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/CNS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/ETHK-B5-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/ETHK-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/ETHK-B5-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/ETHK-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/ETen-B5-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/ETen-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/ETen-B5-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/ETen-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/EUC-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/EUC-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/Ext-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/Ext-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/Ext-RKSJ-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/Ext-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/Ext-RKSJ-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/Ext-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/Ext-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/Ext-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GB-EUC-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GB-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GB-EUC-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GB-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GB-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GB-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GB-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GB-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBK-EUC-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBK-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBK-EUC-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBK-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBK2K-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBK2K-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBK2K-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBK2K-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBKp-EUC-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBKp-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBKp-EUC-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBKp-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBT-EUC-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBT-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBT-EUC-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBT-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBT-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBT-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBT-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBT-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBTpc-EUC-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBTpc-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBTpc-EUC-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBTpc-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBpc-EUC-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBpc-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/GBpc-EUC-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/GBpc-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/HKdla-B5-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/HKdla-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/HKdla-B5-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/HKdla-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/HKdlb-B5-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/HKdlb-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/HKdlb-B5-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/HKdlb-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/HKgccs-B5-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/HKgccs-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/HKgccs-B5-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/HKgccs-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/HKm314-B5-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/HKm314-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/HKm314-B5-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/HKm314-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/HKm471-B5-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/HKm471-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/HKm471-B5-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/HKm471-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/HKscs-B5-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/HKscs-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/HKscs-B5-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/HKscs-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/Hankaku-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/Hankaku-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/Hankaku-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/Hankaku-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/KSC-EUC-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/KSC-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/KSC-EUC-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/KSC-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/KSC-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/KSC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/KSC-Johab-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/KSC-Johab-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/KSC-Johab-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/KSC-Johab-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/KSC-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/KSC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/KSCms-UHC-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/KSCms-UHC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/KSCms-UHC-HW-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/KSCms-UHC-HW-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/KSCms-UHC-HW-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/KSCms-UHC-HW-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/KSCms-UHC-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/KSCms-UHC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/KSCpc-EUC-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/KSCpc-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/KSCpc-EUC-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/KSCpc-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/NWP-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/NWP-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/NWP-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/NWP-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/README.txt` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/README.txt`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/RKSJ-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/RKSJ-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniCNS-UCS2-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniCNS-UCS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniCNS-UCS2-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniCNS-UCS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniCNS-UTF16-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniCNS-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniCNS-UTF16-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniCNS-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniCNS-UTF32-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniCNS-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniCNS-UTF32-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniCNS-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniCNS-UTF8-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniCNS-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniCNS-UTF8-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniCNS-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniGB-UCS2-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniGB-UCS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniGB-UCS2-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniGB-UCS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniGB-UTF16-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniGB-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniGB-UTF16-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniGB-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniGB-UTF32-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniGB-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniGB-UTF32-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniGB-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniGB-UTF8-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniGB-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniGB-UTF8-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniGB-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS-UCS2-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS-UCS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS-UCS2-HW-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS-UCS2-HW-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS-UCS2-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS-UCS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS-UTF16-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS-UTF16-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS-UTF32-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS-UTF32-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS-UTF8-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS-UTF8-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS2004-UTF16-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS2004-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS2004-UTF16-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS2004-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS2004-UTF32-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS2004-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS2004-UTF32-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS2004-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS2004-UTF8-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS2004-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJIS2004-UTF8-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJIS2004-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJISX0213-UTF32-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJISX0213-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJISX0213-UTF32-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJISX0213-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJISX02132004-UTF32-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJISX02132004-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniJISX02132004-UTF32-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniJISX02132004-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniKS-UCS2-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniKS-UCS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniKS-UCS2-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniKS-UCS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniKS-UTF16-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniKS-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniKS-UTF16-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniKS-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniKS-UTF32-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniKS-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniKS-UTF32-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniKS-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniKS-UTF8-H.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniKS-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/UniKS-UTF8-V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/UniKS-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/V.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/to-unicode-Adobe-CNS1.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/to-unicode-Adobe-CNS1.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/to-unicode-Adobe-GB1.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/to-unicode-Adobe-GB1.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/to-unicode-Adobe-Japan1.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/to-unicode-Adobe-Japan1.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmap/to-unicode-Adobe-Korea1.pickle.gz` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmap/to-unicode-Adobe-Korea1.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/cmapdb.py` & `pdfminer.rtl-1.0.1.dev17/pdfminer/cmapdb.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/converter.py` & `pdfminer.rtl-1.0.1.dev17/pdfminer/converter.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/data_structures.py` & `pdfminer.rtl-1.0.1.dev17/pdfminer/data_structures.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/encodingdb.py` & `pdfminer.rtl-1.0.1.dev17/pdfminer/encodingdb.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/fontmetrics.py` & `pdfminer.rtl-1.0.1.dev17/pdfminer/fontmetrics.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/glyphlist.py` & `pdfminer.rtl-1.0.1.dev17/pdfminer/glyphlist.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/high_level.py` & `pdfminer.rtl-1.0.1.dev17/pdfminer/high_level.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/image.py` & `pdfminer.rtl-1.0.1.dev17/pdfminer/image.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/jbig2.py` & `pdfminer.rtl-1.0.1.dev17/pdfminer/jbig2.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/latin_enc.py` & `pdfminer.rtl-1.0.1.dev17/pdfminer/latin_enc.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/layout.py` & `pdfminer.rtl-1.0.1.dev17/pdfminer/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import heapq
 import logging
 import unicodedata as UD
-import bidi.algorithm as BA
+
 import re
 from typing import (
     Dict,
     Generic,
     Iterable,
     Iterator,
     List,
@@ -32,33 +32,38 @@
 from .utils import apply_matrix_pt
 from .utils import bbox2str
 from .utils import fsplit
 from .utils import get_bound
 from .utils import matrix2str
 from .utils import uniq
 
+# import bidi.algorithm as BA
+# import algorithm as BA
+from .algorithm import MIRRORED, get_empty_storage, explicit_embed_and_overrides, resolve_weak_types, resolve_neutral_types, resolve_implicit_levels,reorder_resolved_levels
+
+
 logger = logging.getLogger(__name__)
 
 def debug_string_formats(s):
     # Convert string to bytes
     bytes_data = s.encode()
 
     # Print bytes
-    logger.debug("Bytes:", bytes_data)
+    print("Bytes:", bytes_data)
 
     # Print as hexadecimal
-    logger.debug("Hexadecimal:", bytes_data.hex())
+    print("Hexadecimal:", bytes_data.hex())
 
     # Print bytes as binary
     binary_representation = ' '.join(format(byte, '08b') for byte in bytes_data)
-    logger.debug("Binary:", binary_representation)
+    print("Binary:", binary_representation)
 
     # Print ASCII values
     ascii_values = ' '.join(str(ord(char)) for char in s)
-    logger.debug("ASCII Values:", ascii_values)
+    print("ASCII Values:", ascii_values)
 
 class IndexAssigner:
     def __init__(self, index: int = 0) -> None:
         self.index = index
 
     def run(self, obj: "LTItem") -> None:
         if isinstance(obj, LTTextBox):
@@ -580,36 +585,41 @@
         See: http://unicode.org/reports/tr9/#L4
         """
         for _ch in storage['chars']:
             unichar = _ch['ch']._text
             if len(unichar) == 1 and \
                     UD.mirrored(unichar) and \
                     self._embedding_direction(_ch['level']) == 'R':
-                _ch['ch']._text = BA.MIRRORED.get(unichar, unichar)
+                _ch['ch']._text = MIRRORED.get(unichar, unichar)
 
     def bidi_textline(self):
         """Reorder Char in Textlines"""
-        storage = BA.get_empty_storage()
-        weirdtext = self.get_text()
-
-
-        text = self.removeWeirdChars(weirdtext)
+        storage = get_empty_storage()
+        # weirdtext = self.get_text()
+        # text = self.removeWeirdChars(weirdtext)
+        text = self.get_text()
         
         logger.debug(f"Current bidi line {text}")
-        debug_string_formats(text)
+        # debug_string_formats(text)
+
+
+        # see if script has debug flag or argument
+        debug = False
+
 
         base_level = self.get_base_level(text)
         storage['base_level'] = base_level
         storage['base_dir'] = ('L', 'R')[base_level]
         self.get_embedding_levels(self._objs, storage)
-        BA.explicit_embed_and_overrides(storage)
-        BA.resolve_weak_types(storage)
-        BA.resolve_neutral_types(storage, False)
-        BA.resolve_implicit_levels(storage, False)
-        BA.reorder_resolved_levels(storage, False)
+       
+        explicit_embed_and_overrides(storage)
+        resolve_weak_types(storage)
+        resolve_neutral_types(storage, debug)
+        resolve_implicit_levels(storage, debug)
+        reorder_resolved_levels(storage, debug)
         self.apply_mirroring(storage)
         self._objs = [_ch['ch'] for _ch in storage['chars']]
         return
     
     # for fixing the bidi assertion in resolve_implicit_levels() bug https://github.com/alihoseiny/word_cloud_fa/issues/3
     def removeWeirdChars(self,text):
         weridPatterns = re.compile("["
```

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/lzw.py` & `pdfminer.rtl-1.0.1.dev17/pdfminer/lzw.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/pdfcolor.py` & `pdfminer.rtl-1.0.1.dev17/pdfminer/pdfcolor.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/pdfdevice.py` & `pdfminer.rtl-1.0.1.dev17/pdfminer/pdfdevice.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/pdfdocument.py` & `pdfminer.rtl-1.0.1.dev17/pdfminer/pdfdocument.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/pdffont.py` & `pdfminer.rtl-1.0.1.dev17/pdfminer/pdffont.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/pdfinterp.py` & `pdfminer.rtl-1.0.1.dev17/pdfminer/pdfinterp.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/pdfpage.py` & `pdfminer.rtl-1.0.1.dev17/pdfminer/pdfpage.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/pdfparser.py` & `pdfminer.rtl-1.0.1.dev17/pdfminer/pdfparser.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/pdftypes.py` & `pdfminer.rtl-1.0.1.dev17/pdfminer/pdftypes.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/psparser.py` & `pdfminer.rtl-1.0.1.dev17/pdfminer/psparser.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/runlength.py` & `pdfminer.rtl-1.0.1.dev17/pdfminer/runlength.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer/utils.py` & `pdfminer.rtl-1.0.1.dev17/pdfminer/utils.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer.rtl.egg-info/PKG-INFO` & `pdfminer.rtl-1.0.1.dev17/pdfminer.rtl.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfminer.rtl
-Version: 0.0.2.dev8
+Version: 1.0.1.dev17
 Summary: PDF parser and analyzer
 Home-page: https://github.com/taneron/pdfminerrtl
 Author: Yusuke Shinyama + Philippe Guglielmetti + Taner
 Author-email: pdfminerrtl@rust.8shield.net
 License: MIT
 Keywords: pdf parser,pdf converter,layout analysis,text mining
 Classifier: Programming Language :: Python
@@ -18,30 +18,18 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Text Processing
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: charset-normalizer>=2.0.0
-Requires-Dist: cryptography>=36.0.0
-Requires-Dist: typing_extensions; python_version < "3.8"
-Requires-Dist: importlib_metadata; python_version < "3.8"
-Requires-Dist: python-bidi
 Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: nox; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: mypy==0.931; extra == "dev"
 Provides-Extra: docs
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: sphinx-argparse; extra == "docs"
 Provides-Extra: image
-Requires-Dist: Pillow; extra == "image"
+License-File: LICENSE
 
 pdfminer.rtl
 ============
 
 
 This is a fork of pdfminer.six that attempts to add RTL support with python-bidi. This version is experimental and probably buggy. Please don't rely on it for critical projects.
```

### Comparing `pdfminer_rtl-0.0.2.dev8/pdfminer.rtl.egg-info/SOURCES.txt` & `pdfminer.rtl-1.0.1.dev17/pdfminer.rtl.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 cmaprsrc/README.txt
 cmaprsrc/cid2code_Adobe_CNS1.txt
 cmaprsrc/cid2code_Adobe_GB1.txt
 cmaprsrc/cid2code_Adobe_Japan1.txt
 cmaprsrc/cid2code_Adobe_Korea1.txt
 pdfminer/__init__.py
 pdfminer/_saslprep.py
+pdfminer/algorithm.py
 pdfminer/arcfour.py
 pdfminer/ascii85.py
 pdfminer/ccitt.py
 pdfminer/cmapdb.py
 pdfminer/converter.py
 pdfminer/data_structures.py
 pdfminer/encodingdb.py
@@ -24,14 +25,15 @@
 pdfminer/glyphlist.py
 pdfminer/high_level.py
 pdfminer/image.py
 pdfminer/jbig2.py
 pdfminer/latin_enc.py
 pdfminer/layout.py
 pdfminer/lzw.py
+pdfminer/mirror.py
 pdfminer/pdfcolor.py
 pdfminer/pdfdevice.py
 pdfminer/pdfdocument.py
 pdfminer/pdffont.py
 pdfminer/pdfinterp.py
 pdfminer/pdfpage.py
 pdfminer/pdfparser.py
```

### Comparing `pdfminer_rtl-0.0.2.dev8/setup.py` & `pdfminer.rtl-1.0.1.dev17/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     packages=["pdfminer"],
     package_data={"pdfminer": ["cmap/*.pickle.gz", "py.typed"]},
     install_requires=[
         "charset-normalizer >= 2.0.0",
         "cryptography >= 36.0.0",
         'typing_extensions; python_version < "3.8"',
         'importlib_metadata; python_version < "3.8"',
-        'python-bidi',
+        # 'python-bidi',
     ],
     extras_require={
         "dev": ["pytest", "nox", "black", "mypy == 0.931"],
         "docs": ["sphinx", "sphinx-argparse"],
         "image": ["Pillow"],
     },
     description="PDF parser and analyzer",
```

### Comparing `pdfminer_rtl-0.0.2.dev8/tests/test_converter.py` & `pdfminer.rtl-1.0.1.dev17/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/tests/test_encodingdb.py` & `pdfminer.rtl-1.0.1.dev17/tests/test_encodingdb.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/tests/test_font_size.py` & `pdfminer.rtl-1.0.1.dev17/tests/test_font_size.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/tests/test_highlevel_extracttext.py` & `pdfminer.rtl-1.0.1.dev17/tests/test_highlevel_extracttext.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/tests/test_layout.py` & `pdfminer.rtl-1.0.1.dev17/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/tests/test_pdfdocument.py` & `pdfminer.rtl-1.0.1.dev17/tests/test_pdfdocument.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/tests/test_pdfencoding.py` & `pdfminer.rtl-1.0.1.dev17/tests/test_pdfencoding.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/tests/test_pdffont.py` & `pdfminer.rtl-1.0.1.dev17/tests/test_pdffont.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/tests/test_pdfminer_ccitt.py` & `pdfminer.rtl-1.0.1.dev17/tests/test_pdfminer_ccitt.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/tests/test_pdfminer_crypto.py` & `pdfminer.rtl-1.0.1.dev17/tests/test_pdfminer_crypto.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/tests/test_pdfminer_psparser.py` & `pdfminer.rtl-1.0.1.dev17/tests/test_pdfminer_psparser.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/tests/test_pdfpage.py` & `pdfminer.rtl-1.0.1.dev17/tests/test_pdfpage.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/tests/test_tools_dumppdf.py` & `pdfminer.rtl-1.0.1.dev17/tests/test_tools_dumppdf.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/tests/test_tools_pdf2txt.py` & `pdfminer.rtl-1.0.1.dev17/tests/test_tools_pdf2txt.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/tests/test_utils.py` & `pdfminer.rtl-1.0.1.dev17/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/tools/conv_afm.py` & `pdfminer.rtl-1.0.1.dev17/tools/conv_afm.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/tools/conv_cmap.py` & `pdfminer.rtl-1.0.1.dev17/tools/conv_cmap.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/tools/conv_glyphlist.py` & `pdfminer.rtl-1.0.1.dev17/tools/conv_glyphlist.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/tools/dumppdf.py` & `pdfminer.rtl-1.0.1.dev17/tools/dumppdf.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/tools/pdf2txt.py` & `pdfminer.rtl-1.0.1.dev17/tools/pdf2txt.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/tools/pdfdiff.py` & `pdfminer.rtl-1.0.1.dev17/tools/pdfdiff.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/tools/pdfstats.py` & `pdfminer.rtl-1.0.1.dev17/tools/pdfstats.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev8/tools/prof.py` & `pdfminer.rtl-1.0.1.dev17/tools/prof.py`

 * *Files identical despite different names*

