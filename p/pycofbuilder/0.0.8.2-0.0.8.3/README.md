# Comparing `tmp/pycofbuilder-0.0.8.2.tar.gz` & `tmp/pycofbuilder-0.0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycofbuilder-0.0.8.2.tar", last modified: Wed Mar 13 21:29:45 2024, max compression
+gzip compressed data, was "pycofbuilder-0.0.8.3.tar", last modified: Tue Apr 16 17:58:19 2024, max compression
```

## Comparing `pycofbuilder-0.0.8.2.tar` & `pycofbuilder-0.0.8.3.tar`

### file list

```diff
@@ -1,164 +1,167 @@
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-03-13 21:29:45.587297 pycofbuilder-0.0.8.2/
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1081 2023-10-06 15:52:45.000000 pycofbuilder-0.0.8.2/LICENSE
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      202 2024-03-05 14:34:09.000000 pycofbuilder-0.0.8.2/MANIFEST.in
--rw-r--r--   0 felipe    (1001) felipe    (1001)     8983 2024-03-13 21:29:45.587297 pycofbuilder-0.0.8.2/PKG-INFO
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     6345 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.2/README.md
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1009 2024-03-13 21:22:48.000000 pycofbuilder-0.0.8.2/pyproject.toml
--rw-rw-r--   0 felipe    (1001) felipe    (1001)       38 2024-03-13 21:29:45.587297 pycofbuilder-0.0.8.2/setup.cfg
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1445 2024-03-13 21:23:06.000000 pycofbuilder-0.0.8.2/setup.py
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-03-13 21:29:45.527295 pycofbuilder-0.0.8.2/src/
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-03-13 21:29:45.539296 pycofbuilder-0.0.8.2/src/pycofbuilder/
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1043 2024-03-13 21:23:08.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/__init__.py
--rwxrwxr-x   0 felipe    (1001) felipe    (1001)    26417 2024-03-13 21:20:11.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/building_block.py
--rw-rw-r--   0 felipe    (1001) felipe    (1001)    15250 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/cjson.py
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-03-13 21:29:45.551296 pycofbuilder-0.0.8.2/src/pycofbuilder/data/
--rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/__init__.py
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-03-13 21:29:45.551296 pycofbuilder-0.0.8.2/src/pycofbuilder/data/__pycache__/
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      175 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     6843 2024-03-13 20:45:45.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/__pycache__/topology.cpython-311.pyc
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-03-13 21:29:45.555296 pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      627 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/BOH2.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      612 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/Br.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      859 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/CH2CN.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      720 2024-01-10 16:37:07.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/CH3.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      999 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/CHNNH2.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      867 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/CHO.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1465 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/COCHCHOH.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1116 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/CONHNH2.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      873 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/COOH.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      613 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/Cl.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      608 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/NH2.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      741 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/NHOH.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      609 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/O.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      893 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/OH2.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/__init__.py
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-03-13 21:29:45.555296 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-03-13 21:29:45.559296 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/D4/
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3679 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/D4/ADAM.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     5816 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/D4/SBFE.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)    14640 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/D4/TDAT.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     9212 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/D4/TKAT.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)    11916 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/D4/TKDM.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     6483 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/D4/TTPM.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/D4/__init__.py
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-03-13 21:29:45.559296 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/H6/
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     8080 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/H6/HECO.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     9885 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/H6/HEXB.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)    15793 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/H6/HPCO.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/H6/__init__.py
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-03-13 21:29:45.567296 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2906 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/2BPD.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2970 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/3BPD.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3746 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/3IDT.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3727 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/4IDT.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3608 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/ANTR.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2446 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/BBTZ.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2708 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/BDFN.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2714 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/BDTP.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1898 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/BENZ.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3215 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/BPNY.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     4995 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/BPYB.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2455 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/BTPH.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     5259 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/DFFE.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2965 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/DHPI.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2967 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/DHSI.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3645 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/DPBY.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3495 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/DPDA.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3730 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/DPEL.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3395 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/DPEY.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      620 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/HDZN.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     4689 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/IITT.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3715 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/INDE.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     4498 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/INFL.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2630 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/INTO.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2705 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/NAPT.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3457 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/NDTP.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     4125 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/PHEN.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     5243 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/PTCD.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3860 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/PYEN.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3659 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/PYRN.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3400 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/PYTO.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     4191 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/TIDA.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     6343 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/TIEN.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     4772 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/TPDI.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     4501 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/TPNY.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1942 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/TTPH.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/__init__.py
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-03-13 21:29:45.571297 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/S4/
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2684 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/S4/CoBTC.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2684 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/S4/CuBTC.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1428 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/S4/NiBTC.gjf
--rw-rw-r--   0 felipe    (1001) felipe    (1001)    10913 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/S4/PHPR.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     5215 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/S4/PORP.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     7719 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/S4/PTCA.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2684 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/S4/ZnBTC.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/S4/__init__.py
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-03-13 21:29:45.579297 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1892 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/BENZ.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1851 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/BRZN.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3087 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/BTTP.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     4953 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/DBA1.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     5680 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/DBA2.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     5710 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/DICZ.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     8873 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/STAR.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     9549 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/STAR1.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     9612 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/TBBZ.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1492 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/TOTB.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     4789 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/TPAM.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     5790 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/TPBZ.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     4180 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/TPNY.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     6011 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/TPOB.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     5689 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/TPTA.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     5389 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/TPTZ.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1477 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/TRZN.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/__init__.py
--rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/__init__.py
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-03-13 21:29:45.587297 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      615 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/Br.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1030 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/CF3.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      987 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/CH3.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      878 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/CHO.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      878 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/CHS.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      723 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/CN.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      999 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/COOH.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      617 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/Cl.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2696 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/DMPE.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2008 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/EEPO.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2145 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/EMEPO.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1248 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/EPO.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      610 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/F.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      614 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/H.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      609 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/I.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1630 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/MEPO.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      844 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/NH2.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      735 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/NO.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      886 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/NO2.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      609 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/O.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1391 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/OCOCH3.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1762 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/OEEPO.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1503 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/OEt.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      728 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/OH.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1129 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/OMe.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1883 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/OProp.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1881 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/Ph.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      726 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/SH.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1009 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/SO2H.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1143 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/SO3H.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/__init__.py
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2117 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/tBu.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)    66018 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/periodic_table.json
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     8037 2024-03-13 20:45:37.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/data/topology.py
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1910 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/exceptions.py
--rw-rw-r--   0 felipe    (1001) felipe    (1001)   178980 2024-03-13 21:21:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/framework.py
--rw-rw-r--   0 felipe    (1001) felipe    (1001)    47784 2024-03-12 17:46:14.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/io_tools.py
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2492 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/logger.py
--rw-rw-r--   0 felipe    (1001) felipe    (1001)    32273 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.2/src/pycofbuilder/tools.py
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-03-13 21:29:45.543296 pycofbuilder-0.0.8.2/src/pycofbuilder.egg-info/
--rw-r--r--   0 felipe    (1001) felipe    (1001)     8983 2024-03-13 21:29:45.000000 pycofbuilder-0.0.8.2/src/pycofbuilder.egg-info/PKG-INFO
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     5877 2024-03-13 21:29:45.000000 pycofbuilder-0.0.8.2/src/pycofbuilder.egg-info/SOURCES.txt
--rw-rw-r--   0 felipe    (1001) felipe    (1001)        1 2024-03-13 21:29:45.000000 pycofbuilder-0.0.8.2/src/pycofbuilder.egg-info/dependency_links.txt
--rw-rw-r--   0 felipe    (1001) felipe    (1001)       95 2024-03-13 21:29:45.000000 pycofbuilder-0.0.8.2/src/pycofbuilder.egg-info/requires.txt
--rw-rw-r--   0 felipe    (1001) felipe    (1001)       13 2024-03-13 21:29:45.000000 pycofbuilder-0.0.8.2/src/pycofbuilder.egg-info/top_level.txt
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-03-13 21:29:45.587297 pycofbuilder-0.0.8.2/tests/
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      266 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.2/tests/test_advanced.py
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      258 2023-10-06 15:52:45.000000 pycofbuilder-0.0.8.2/tests/test_basic.py
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.497946 pycofbuilder-0.0.8.3/
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1081 2023-10-06 15:52:45.000000 pycofbuilder-0.0.8.3/LICENSE
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      202 2024-03-05 14:34:09.000000 pycofbuilder-0.0.8.3/MANIFEST.in
+-rw-r--r--   0 felipe    (1001) felipe    (1001)     8983 2024-04-16 17:58:19.497946 pycofbuilder-0.0.8.3/PKG-INFO
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     6345 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.3/README.md
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1009 2024-04-16 14:15:54.000000 pycofbuilder-0.0.8.3/pyproject.toml
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)       38 2024-04-16 17:58:19.497946 pycofbuilder-0.0.8.3/setup.cfg
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1445 2024-04-16 14:15:43.000000 pycofbuilder-0.0.8.3/setup.py
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.445945 pycofbuilder-0.0.8.3/src/
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.461946 pycofbuilder-0.0.8.3/src/pycofbuilder/
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1043 2024-04-16 14:14:35.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/__init__.py
+-rwxrwxr-x   0 felipe    (1001) felipe    (1001)    26448 2024-04-16 16:05:38.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/building_block.py
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)    15250 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/cjson.py
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.465946 pycofbuilder-0.0.8.3/src/pycofbuilder/data/
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/__init__.py
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.465946 pycofbuilder-0.0.8.3/src/pycofbuilder/data/__pycache__/
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      175 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     6651 2024-04-16 17:25:24.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/__pycache__/topology.cpython-311.pyc
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.469946 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      627 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/BOH2.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      612 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/Br.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      859 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/CH2CN.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      720 2024-01-10 16:37:07.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/CH3.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      999 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/CHNNH2.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      867 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/CHO.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1465 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/COCHCHOH.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1116 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/CONHNH2.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      873 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/COOH.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      613 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/Cl.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      608 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/NH2.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      741 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/NHOH.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      609 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/O.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      893 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/OH2.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/__init__.py
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.469946 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.469946 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3679 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/ADAM.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     5816 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/SBFE.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)    14640 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/TDAT.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     9212 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/TKAT.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)    11916 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/TKDM.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     6483 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/TTPM.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/__init__.py
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.473946 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/H6/
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     8080 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/H6/HECO.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     9885 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/H6/HEXB.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)    15793 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/H6/HPCO.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/H6/__init__.py
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.477946 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2906 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/2BPD.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2970 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/3BPD.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3746 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/3IDT.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3727 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/4IDT.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3608 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/ANTR.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2446 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BBTZ.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2708 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BDFN.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2714 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BDTP.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1898 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BENZ.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3215 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BPNY.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     4995 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BPYB.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2455 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BTPH.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3098 2024-04-16 13:59:02.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DFDB.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     5259 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DFFE.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2965 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DHPI.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2967 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DHSI.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3645 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DPBY.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3495 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DPDA.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3730 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DPEL.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3395 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DPEY.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      620 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/HDZN.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     4689 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/IITT.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3715 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/INDE.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     4498 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/INFL.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2630 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/INTO.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2705 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/NAPT.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3457 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/NDTP.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     4125 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/PHEN.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     5243 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/PTCD.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3860 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/PYEN.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3659 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/PYRN.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3400 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/PYTO.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     4191 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/TIDA.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     6343 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/TIEN.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     4772 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/TPDI.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     4501 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/TPNY.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1942 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/TTPH.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/__init__.py
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.477946 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/R4/
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     7553 2024-04-16 14:05:34.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/R4/TPDT.cjson
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.477946 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2684 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/CoBTC.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2684 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/CuBTC.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1428 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/NiBTC.gjf
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)    10913 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/PHPR.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     5215 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/PORP.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     7719 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/PTCA.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2684 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/ZnBTC.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/__init__.py
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.485946 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1892 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/BENZ.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1851 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/BRZN.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3087 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/BTTP.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     4953 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/DBA1.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     5680 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/DBA2.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     5710 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/DICZ.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     8873 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/STAR.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     9549 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/STAR1.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     9612 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TBBZ.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1492 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TOTB.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     4789 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TPAM.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     5790 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TPBZ.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     4180 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TPNY.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     6011 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TPOB.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     5689 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TPTA.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     5389 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TPTZ.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1477 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TRZN.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/__init__.py
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/__init__.py
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.493946 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      615 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/Br.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1030 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/CF3.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      987 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/CH3.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      878 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/CHO.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      878 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/CHS.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      723 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/CN.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      999 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/COOH.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      617 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/Cl.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2696 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/DMPE.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2008 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/EEPO.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2145 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/EMEPO.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1248 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/EPO.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      610 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/F.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      614 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/H.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      609 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/I.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1630 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/MEPO.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      844 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/NH2.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      735 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/NO.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      886 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/NO2.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      609 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/O.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1391 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/OCOCH3.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1762 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/OEEPO.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1503 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/OEt.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      728 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/OH.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1129 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/OMe.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1883 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/OProp.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1881 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/Ph.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      726 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/SH.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1009 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/SO2H.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1143 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/SO3H.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/__init__.py
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2117 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/tBu.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)    66018 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/periodic_table.json
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     7993 2024-04-16 17:23:55.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/topology.py
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1910 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/exceptions.py
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)   179874 2024-04-16 17:48:27.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/framework.py
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)    47784 2024-03-12 17:46:14.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/io_tools.py
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2492 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/logger.py
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)    32273 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/tools.py
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.465946 pycofbuilder-0.0.8.3/src/pycofbuilder.egg-info/
+-rw-r--r--   0 felipe    (1001) felipe    (1001)     8983 2024-04-16 17:58:19.000000 pycofbuilder-0.0.8.3/src/pycofbuilder.egg-info/PKG-INFO
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     5959 2024-04-16 17:58:19.000000 pycofbuilder-0.0.8.3/src/pycofbuilder.egg-info/SOURCES.txt
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)        1 2024-04-16 17:58:19.000000 pycofbuilder-0.0.8.3/src/pycofbuilder.egg-info/dependency_links.txt
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)       95 2024-04-16 17:58:19.000000 pycofbuilder-0.0.8.3/src/pycofbuilder.egg-info/requires.txt
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)       13 2024-04-16 17:58:19.000000 pycofbuilder-0.0.8.3/src/pycofbuilder.egg-info/top_level.txt
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.497946 pycofbuilder-0.0.8.3/tests/
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      266 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.3/tests/test_advanced.py
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      258 2023-10-06 15:52:45.000000 pycofbuilder-0.0.8.3/tests/test_basic.py
```

### Comparing `pycofbuilder-0.0.8.2/LICENSE` & `pycofbuilder-0.0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/PKG-INFO` & `pycofbuilder-0.0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycofbuilder
-Version: 0.0.8.2
+Version: 0.0.8.3
 Summary: A package for Covalent Organic Frameworks sturcture creation based on the reticular approach.
 Home-page: https://github.com/lipelopesoliveira/pyCOFBuilder
 Author: Felipe Lopes Oliveira
 Author-email: Felipe Lopes <felipe.lopes@nano.ufrj.br>
 License: MIT License
         
         Copyright (c) 2023, Felipe Lopes de Oliveira
```

### Comparing `pycofbuilder-0.0.8.2/README.md` & `pycofbuilder-0.0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/pyproject.toml` & `pycofbuilder-0.0.8.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pyproject.toml
 
 [project]
 name = "pycofbuilder"
-version = '0.0.8.2'
+version = '0.0.8.3'
 authors = [
   { name="Felipe Lopes", email="felipe.lopes@nano.ufrj.br" },
 ]
 description = 'A package for Covalent Organic Frameworks sturcture creation based on the reticular approach.'
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pycofbuilder-0.0.8.2/setup.py` & `pycofbuilder-0.0.8.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 with open('LICENSE') as f:
     license = f.read()
 
 
-VERSION = '0.0.8.2'
+VERSION = '0.0.8.3'
 DESCRIPTION = 'A package for Covalent Organic Frameworks sturcture assembly.'
 
 setup(
     name='pyCOFBuilder',
     version=VERSION,
     description=DESCRIPTION,
     long_description=open('README.md').read(),
```

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/__init__.py` & `pycofbuilder-0.0.8.3/src/pycofbuilder/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,10 +39,10 @@
     'Logger'
     ]
 
 _ROOT = os.path.abspath(os.path.dirname(__file__))
 
 __author__ = "Felipe Lopes de Oliveira"
 __license__ = "MIT"
-__version__ = '0.0.8.2'
+__version__ = '0.0.8.3'
 __email__ = "felipe.lopes@nano.ufrj.br"
 __status__ = "Development"
```

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/building_block.py` & `pycofbuilder-0.0.8.3/src/pycofbuilder/building_block.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
         self.core = kwargs.get('core', None)
         self.conector = kwargs.get('conector', None)
         self.funcGroups = kwargs.get('funcGroups', None)
 
         self.available_symmetry = ['L2',
                                    'T3',
-                                   'S4', 'D4',  # 'R4'
+                                   'S4', 'D4', 'R4',
                                    'H6',  # 'O6', 'P6'
                                    # 'C8', 'A8', 'E8'
                                    # 'B12', 'I12', 'U12', 'X12'
                                    ]
 
         # Check if bb_out_path exists and try to create it if not
         if self.save_bb != '':
@@ -655,15 +655,15 @@
         funcGroups = name[3:]
 
         BB_dict = self.get_available_core()
 
         if symm in self.available_symmetry:
             symm_check = True
         else:
-            print('ERROR!: Building Block symmetry must be L2, T3, S4, or H6.')
+            print('ERROR!: Building Block symmetry be one of the following:', ','.join(self.available_symmetry))
             symm_check = False
 
         if core in BB_dict[symm]:
             core_check = True
         else:
             print(f'ERROR!: {core} not available!')
             print(f'Available cores with {symm} symmetry are {BB_dict[symm]}')
```

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/cjson.py` & `pycofbuilder-0.0.8.3/src/pycofbuilder/cjson.py`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/__pycache__/topology.cpython-311.pyc` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/__pycache__/topology.cpython-311.pyc`

 * *Files 22% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x7110f265 (Wed Mar 13 20:45:37 2024 UTC)
-files sz: 8037
+moddate:  0x2bb41e66 (Tue Apr 16 17:23:55 2024 UTC)
+files sz: 7993
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 29
    flags     : 0
    code
       0x970064005a00640164026c015a026403020065026a0300000000000000
@@ -23,90 +23,85 @@
       0065026a0500000000000000006408a6010000ab01000000000000000064
       087a0b000064016703640b640a9c0267026401020065026a050000000000
       0000006408a6010000ab010000000000000000640d7a0b00006401670364
       01640a9c02640e640f020065026a0500000000000000006408a6010000ab
       0100000000000000007a05000064107a0b0000640167036407640a9c0264
       11640f020065026a0500000000000000006408a6010000ab010000000000
       0000007a05000064107a0b0000640167036412640a9c026703640c9c0a64
-      03020065026a0500000000000000006403a6010000ab0100000000000000
-      007a0b00006403020065026a0500000000000000006403a6010000ab0100
-      000000000000007a0b000064056406640664066413640167006409a20164
-      14640a9c0267006415a2016414640a9c0267026700640c9c0a6413020065
-      026a0500000000000000006403a6010000ab0100000000000000007a0b00
-      006413020065026a0500000000000000006403a6010000ab010000000000
-      0000007a0b000064056406640664066413640367006409a2016416640a9c
-      0267006415a2016416640a9c02670267006417a2016414640a9c02670064
-      18a2016419640a9c026700641aa201641b640a9c026700641ca201641d64
-      0a9c026704640c9c0a6403020065026a030000000000000000020065026a
-      0400000000000000006404a6010000ab010000000000000000a6010000ab
-      0100000000000000007a0500006403020065026a03000000000000000002
-      0065026a0400000000000000006404a6010000ab010000000000000000a6
-      010000ab0100000000000000007a0500006405640664066407640d640867
-      006409a2016401640a9c0267016401020065026a05000000000000000064
-      08a6010000ab01000000000000000064087a0b000064016703641e640a9c
-      02641f020065026a0500000000000000006408a6010000ab010000000000
-      000000640d7a0b0000640167036401640a9c026702640c9c0a6403640364
-      05640664066407640d640167006409a2016404640a9c0267016411020065
-      026a0500000000000000006408a6010000ab01000000000000000064137a
-      0b0000640167036404640a9c0267006420a2016406640a9c02640e020065
-      026a0500000000000000006408a6010000ab01000000000000000064137a
-      0b0000640167036421640a9c026703640c9c0a6413641364056406640664
-      07641364016411020065026a0500000000000000006408a6010000ab0100
-      0000000000000064137a0b0000640167036404640a9c0267006420a20164
-      22640a9c02640e020065026a0500000000000000006408a6010000ab0100
-      0000000000000064137a0b0000640167036421640a9c0267036700640c9c
-      0a641364136405640664066407641364036411020065026a050000000000
-      0000006408a6010000ab01000000000000000064137a0b00006401670364
-      04640a9c0267006420a2016422640a9c02640e020065026a050000000000
-      0000006408a6010000ab01000000000000000064137a0b00006401670364
-      21640a9c0267036423020065026a0500000000000000006408a6010000ab
-      01000000000000000064247a0b0000640167036421640a9c026425640802
-      0065026a0500000000000000006408a6010000ab0100000000000000007a
-      05000064247a0b0000640167036421640a9c026426020065026a05000000
-      00000000006408a6010000ab01000000000000000064247a0b0000640167
-      036404640a9c026427020065026a0500000000000000006408a6010000ab
-      01000000000000000064247a0b0000640167036404640a9c02641f020065
-      026a0500000000000000006408a6010000ab01000000000000000064137a
-      0b0000640167036406640a9c026401020065026a05000000000000000064
-      08a6010000ab01000000000000000064137a0b0000640167036406640a9c
-      026706640c9c0a6428642864056406640664076413640364116408020065
-      026a0500000000000000006408a6010000ab0100000000000000007a0500
-      0064107a0b0000640167036429640a9c0267006420a2016414640a9c0264
-      0e6408020065026a0500000000000000006408a6010000ab010000000000
-      0000007a05000064107a0b000064016703642a640a9c0267036700640c9c
-      0a6403640364056406640664076413640364116408020065026a05000000
-      00000000006408a6010000ab0100000000000000007a05000064107a0b00
-      00640167036429640a9c0267006420a2016414640a9c02640e6408020065
-      026a0500000000000000006408a6010000ab0100000000000000007a0500
-      0064107a0b000064016703642a640a9c026703642b642c020065026a0500
-      000000000000006408a6010000ab0100000000000000007a050000642d7a
-      0b0000640167036421640a9c02642e642c020065026a0500000000000000
-      006408a6010000ab0100000000000000007a050000642d7a0b0000640167
-      036404640a9c02641f642f020065026a0500000000000000006408a60100
-      00ab0100000000000000007a05000064307a0b0000640167036406640a9c
-      0264016431020065026a0500000000000000006408a6010000ab01000000
-      00000000007a05000064307a0b0000640167036406640a9c026432643302
-      0065026a0500000000000000006408a6010000ab0100000000000000007a
-      050000642d7a0b0000640167036421640a9c0264346433020065026a0500
-      000000000000006408a6010000ab0100000000000000007a050000642d7a
-      0b0000640167036404640a9c026706640c9c0a6428642864286435643564
-      3567006436a20167006437a20167006438a20167036413641367006409a2
-      0164396700643aa201643b9c036700643ca201643d6700643ea201643b9c
-      0367026700643f9c0b64286428642864356435643567006436a201670064
-      37a20167006438a20167036413640367006409a20164406700643aa20164
-      3b9c036700643ca20164416700643ea201643b9c03670267006442a20164
-      436700643aa201643b9c0367006444a201644567006446a201643b9c0367
-      006447a201644867006449a201643b9c036700644aa20164456700644ba2
-      01643b9c036704643f9c0b6428642864286406640664066700644ca20167
-      00644da2016700644ea20167036413640867006420a201644f67006450a2
-      01643b9c0367006451a201645267006453a201643b9c0367006454a20164
-      1667006455a201643b9c03670367006456a20164046700643aa201643b9c
-      0367006457a201640167006458a201643b9c0367006459a2016401670064
-      5aa201643b9c036700645ba201645c6700643aa201643b9c036704643f9c
-      0b645d9c0d5a0664025300
+      13641364056406640664066414640167006409a2016415640a9c02670064
+      16a2016415640a9c0267026700640c9c0a64136413640564066406640664
+      14640367006409a2016417640a9c0267006416a2016417640a9c02670267
+      006418a2016415640a9c0267006419a201641a640a9c026700641ba20164
+      1c640a9c026700641da201641e640a9c026704640c9c0a6403020065026a
+      030000000000000000020065026a0400000000000000006404a6010000ab
+      010000000000000000a6010000ab0100000000000000007a050000640302
+      0065026a030000000000000000020065026a0400000000000000006404a6
+      010000ab010000000000000000a6010000ab0100000000000000007a0500
+      006405640664066407640d640867006409a2016401640a9c026701640102
+      0065026a0500000000000000006408a6010000ab01000000000000000064
+      087a0b000064016703641f640a9c026420020065026a0500000000000000
+      006408a6010000ab010000000000000000640d7a0b000064016703640164
+      0a9c026702640c9c0a640364036405640664066407640d640167006409a2
+      016404640a9c0267016411020065026a0500000000000000006408a60100
+      00ab01000000000000000064147a0b0000640167036404640a9c02670064
+      21a2016406640a9c02640e020065026a0500000000000000006408a60100
+      00ab01000000000000000064147a0b0000640167036422640a9c02670364
+      0c9c0a641464146405640664066407641464016411020065026a05000000
+      00000000006408a6010000ab01000000000000000064147a0b0000640167
+      036404640a9c0267006421a2016423640a9c02640e020065026a05000000
+      00000000006408a6010000ab01000000000000000064147a0b0000640167
+      036422640a9c0267036700640c9c0a641464146405640664066407641464
+      036411020065026a0500000000000000006408a6010000ab010000000000
+      00000064147a0b0000640167036404640a9c0267006421a2016423640a9c
+      02640e020065026a0500000000000000006408a6010000ab010000000000
+      00000064147a0b0000640167036422640a9c0267036424020065026a0500
+      000000000000006408a6010000ab01000000000000000064257a0b000064
+      0167036422640a9c0264266408020065026a0500000000000000006408a6
+      010000ab0100000000000000007a05000064257a0b000064016703642264
+      0a9c026427020065026a0500000000000000006408a6010000ab01000000
+      000000000064257a0b0000640167036404640a9c026428020065026a0500
+      000000000000006408a6010000ab01000000000000000064257a0b000064
+      0167036404640a9c026420020065026a0500000000000000006408a60100
+      00ab01000000000000000064147a0b0000640167036406640a9c02640102
+      0065026a0500000000000000006408a6010000ab01000000000000000064
+      147a0b0000640167036406640a9c026706640c9c0a641364136405640664
+      0664076414640364116408020065026a0500000000000000006408a60100
+      00ab0100000000000000007a05000064107a0b0000640167036429640a9c
+      0267006421a2016415640a9c02640e6408020065026a0500000000000000
+      006408a6010000ab0100000000000000007a05000064107a0b0000640167
+      03642a640a9c0267036700640c9c0a640364036405640664066407641464
+      0364116408020065026a0500000000000000006408a6010000ab01000000
+      00000000007a05000064107a0b0000640167036429640a9c0267006421a2
+      016415640a9c02640e6408020065026a0500000000000000006408a60100
+      00ab0100000000000000007a05000064107a0b000064016703642a640a9c
+      026703642b642c020065026a0500000000000000006408a6010000ab0100
+      000000000000007a050000642d7a0b0000640167036422640a9c02642e64
+      2c020065026a0500000000000000006408a6010000ab0100000000000000
+      007a050000642d7a0b0000640167036404640a9c026420642f020065026a
+      0500000000000000006408a6010000ab0100000000000000007a05000064
+      307a0b0000640167036406640a9c0264016431020065026a050000000000
+      0000006408a6010000ab0100000000000000007a05000064307a0b000064
+      0167036406640a9c0264326433020065026a0500000000000000006408a6
+      010000ab0100000000000000007a050000642d7a0b000064016703642264
+      0a9c0264346433020065026a0500000000000000006408a6010000ab0100
+      000000000000007a050000642d7a0b0000640167036404640a9c02670664
+      0c9c0a64136413641364356435643567006436a20167006437a201670064
+      38a20167036414641467006409a20164396700643aa201643b9c03670064
+      3ca201643d6700643ea201643b9c0367026700643f9c0b64136413641364
+      356435643567006436a20167006437a20167006438a20167036414640367
+      006409a20164406700643aa201643b9c036700643ca20164416700643ea2
+      01643b9c03670267006442a20164436700643aa201643b9c0367006444a2
+      01644567006446a201643b9c0367006447a201644867006449a201643b9c
+      036700644aa20164456700644ba201643b9c036704643f9c0b6413641364
+      136406640664066700644ca2016700644da2016700644ea2016703641464
+      0867006421a201644f67006450a201643b9c0367006451a2016452670064
+      53a201643b9c0367006454a201641767006455a201643b9c036703670064
+      56a20164046700643aa201643b9c0367006457a201640167006458a20164
+      3b9c0367006459a20164016700645aa201643b9c036700645ba201645c67
+      00643aa201643b9c036704643f9c0b645d9c0d5a0664025300
      0           0 RESUME                   0
    
      5           2 LOAD_CONST               0 ('\nThe dictionary containing the definitions nets for a Framework buiding\n')
                  4 STORE_NAME               0 (__doc__)
    
      9           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (None)
@@ -300,994 +295,966 @@
                590 BUILD_CONST_KEY_MAP      2
    
     40         592 BUILD_LIST               3
    
     27         594 LOAD_CONST              12 (('a', 'b', 'c', 'alpha', 'beta', 'gamma', 'vertice_connectivity', 'edge_connectivity', 'vertices', 'edges'))
                596 BUILD_CONST_KEY_MAP     10
    
-    47         598 LOAD_CONST               3 (2)
-               600 PUSH_NULL
-               602 LOAD_NAME                2 (np)
-               604 LOAD_ATTR                5 (sqrt)
-               614 LOAD_CONST               3 (2)
-               616 PRECALL                  1
-               620 CALL                     1
-               630 BINARY_OP               11 (/)
-   
-    48         634 LOAD_CONST               3 (2)
-               636 PUSH_NULL
-               638 LOAD_NAME                2 (np)
-               640 LOAD_ATTR                5 (sqrt)
-               650 LOAD_CONST               3 (2)
-               652 PRECALL                  1
-               656 CALL                     1
-               666 BINARY_OP               11 (/)
-   
-    49         670 LOAD_CONST               5 (3.6)
-   
-    50         672 LOAD_CONST               6 (90)
-   
-    51         674 LOAD_CONST               6 (90)
-   
-    52         676 LOAD_CONST               6 (90)
-   
-    53         678 LOAD_CONST              19 (4)
-   
-    54         680 LOAD_CONST               1 (0)
-   
-    56         682 BUILD_LIST               0
-               684 LOAD_CONST               9 ((0, 0, 0))
-               686 LIST_EXTEND              1
-               688 LOAD_CONST              20 (45)
-               690 LOAD_CONST              10 (('position', 'angle'))
-               692 BUILD_CONST_KEY_MAP      2
-   
-    57         694 BUILD_LIST               0
-               696 LOAD_CONST              21 ((0.5, 0.5, 0))
-               698 LIST_EXTEND              1
-               700 LOAD_CONST              20 (45)
-               702 LOAD_CONST              10 (('position', 'angle'))
-               704 BUILD_CONST_KEY_MAP      2
-   
-    55         706 BUILD_LIST               2
-   
-    59         708 BUILD_LIST               0
-   
-    46         710 LOAD_CONST              12 (('a', 'b', 'c', 'alpha', 'beta', 'gamma', 'vertice_connectivity', 'edge_connectivity', 'vertices', 'edges'))
-               712 BUILD_CONST_KEY_MAP     10
-   
-    62         714 LOAD_CONST              19 (4)
-               716 PUSH_NULL
-               718 LOAD_NAME                2 (np)
-               720 LOAD_ATTR                5 (sqrt)
-               730 LOAD_CONST               3 (2)
-               732 PRECALL                  1
-               736 CALL                     1
-               746 BINARY_OP               11 (/)
-   
-    63         750 LOAD_CONST              19 (4)
-               752 PUSH_NULL
-               754 LOAD_NAME                2 (np)
-               756 LOAD_ATTR                5 (sqrt)
-               766 LOAD_CONST               3 (2)
-               768 PRECALL                  1
-               772 CALL                     1
-               782 BINARY_OP               11 (/)
-   
-    64         786 LOAD_CONST               5 (3.6)
-   
-    65         788 LOAD_CONST               6 (90)
-   
-    66         790 LOAD_CONST               6 (90)
-   
-    67         792 LOAD_CONST               6 (90)
-   
-    68         794 LOAD_CONST              19 (4)
-   
-    69         796 LOAD_CONST               3 (2)
-   
-    71         798 BUILD_LIST               0
-               800 LOAD_CONST               9 ((0, 0, 0))
-               802 LIST_EXTEND              1
-               804 LOAD_CONST              22 (-45)
-               806 LOAD_CONST              10 (('position', 'angle'))
-               808 BUILD_CONST_KEY_MAP      2
-   
-    72         810 BUILD_LIST               0
-               812 LOAD_CONST              21 ((0.5, 0.5, 0))
-               814 LIST_EXTEND              1
-               816 LOAD_CONST              22 (-45)
-               818 LOAD_CONST              10 (('position', 'angle'))
-               820 BUILD_CONST_KEY_MAP      2
-   
-    70         822 BUILD_LIST               2
-   
-    75         824 BUILD_LIST               0
-               826 LOAD_CONST              23 ((0.25, 0.25, 0))
-               828 LIST_EXTEND              1
-               830 LOAD_CONST              20 (45)
-               832 LOAD_CONST              10 (('position', 'angle'))
-               834 BUILD_CONST_KEY_MAP      2
-   
-    76         836 BUILD_LIST               0
-               838 LOAD_CONST              24 ((0.75, 0.25, 0))
-               840 LIST_EXTEND              1
-               842 LOAD_CONST              25 (135)
-               844 LOAD_CONST              10 (('position', 'angle'))
-               846 BUILD_CONST_KEY_MAP      2
-   
-    77         848 BUILD_LIST               0
-               850 LOAD_CONST              26 ((0.75, 0.75, 0))
-               852 LIST_EXTEND              1
-               854 LOAD_CONST              27 (225)
-               856 LOAD_CONST              10 (('position', 'angle'))
-               858 BUILD_CONST_KEY_MAP      2
-   
-    78         860 BUILD_LIST               0
-               862 LOAD_CONST              28 ((0.25, 0.75, 0))
-               864 LIST_EXTEND              1
-               866 LOAD_CONST              29 (315)
-               868 LOAD_CONST              10 (('position', 'angle'))
-               870 BUILD_CONST_KEY_MAP      2
-   
-    74         872 BUILD_LIST               4
-   
-    61         874 LOAD_CONST              12 (('a', 'b', 'c', 'alpha', 'beta', 'gamma', 'vertice_connectivity', 'edge_connectivity', 'vertices', 'edges'))
-               876 BUILD_CONST_KEY_MAP     10
-   
-    82         878 LOAD_CONST               3 (2)
-               880 PUSH_NULL
-               882 LOAD_NAME                2 (np)
-               884 LOAD_ATTR                3 (cos)
-               894 PUSH_NULL
-               896 LOAD_NAME                2 (np)
-               898 LOAD_ATTR                4 (radians)
-               908 LOAD_CONST               4 (30)
-               910 PRECALL                  1
-               914 CALL                     1
-               924 PRECALL                  1
-               928 CALL                     1
-               938 BINARY_OP                5 (*)
-   
-    83         942 LOAD_CONST               3 (2)
-               944 PUSH_NULL
-               946 LOAD_NAME                2 (np)
-               948 LOAD_ATTR                3 (cos)
-               958 PUSH_NULL
-               960 LOAD_NAME                2 (np)
-               962 LOAD_ATTR                4 (radians)
-               972 LOAD_CONST               4 (30)
-               974 PRECALL                  1
-               978 CALL                     1
-               988 PRECALL                  1
-               992 CALL                     1
-              1002 BINARY_OP                5 (*)
-   
-    84        1006 LOAD_CONST               5 (3.6)
-   
-    85        1008 LOAD_CONST               6 (90)
-   
-    86        1010 LOAD_CONST               6 (90)
-   
-    87        1012 LOAD_CONST               7 (120)
-   
-    88        1014 LOAD_CONST              13 (6)
-   
-    89        1016 LOAD_CONST               8 (3)
-   
-    91        1018 BUILD_LIST               0
-              1020 LOAD_CONST               9 ((0, 0, 0))
-              1022 LIST_EXTEND              1
-              1024 LOAD_CONST               1 (0)
-              1026 LOAD_CONST              10 (('position', 'angle'))
-              1028 BUILD_CONST_KEY_MAP      2
-   
-    90        1030 BUILD_LIST               1
-   
-    94        1032 LOAD_CONST               1 (0)
-              1034 PUSH_NULL
-              1036 LOAD_NAME                2 (np)
-              1038 LOAD_ATTR                5 (sqrt)
-              1048 LOAD_CONST               8 (3)
-              1050 PRECALL                  1
-              1054 CALL                     1
-              1064 LOAD_CONST               8 (3)
-              1066 BINARY_OP               11 (/)
-              1070 LOAD_CONST               1 (0)
-              1072 BUILD_LIST               3
-              1074 LOAD_CONST              30 (-180)
-              1076 LOAD_CONST              10 (('position', 'angle'))
-              1078 BUILD_CONST_KEY_MAP      2
-   
-    95        1080 LOAD_CONST              31 (0.5)
-              1082 PUSH_NULL
-              1084 LOAD_NAME                2 (np)
-              1086 LOAD_ATTR                5 (sqrt)
-              1096 LOAD_CONST               8 (3)
-              1098 PRECALL                  1
-              1102 CALL                     1
-              1112 LOAD_CONST              13 (6)
-              1114 BINARY_OP               11 (/)
-              1118 LOAD_CONST               1 (0)
-              1120 BUILD_LIST               3
-              1122 LOAD_CONST               1 (0)
-              1124 LOAD_CONST              10 (('position', 'angle'))
-              1126 BUILD_CONST_KEY_MAP      2
-   
-    93        1128 BUILD_LIST               2
-   
-    81        1130 LOAD_CONST              12 (('a', 'b', 'c', 'alpha', 'beta', 'gamma', 'vertice_connectivity', 'edge_connectivity', 'vertices', 'edges'))
-              1132 BUILD_CONST_KEY_MAP     10
-   
-    99        1134 LOAD_CONST               3 (2)
-   
-   100        1136 LOAD_CONST               3 (2)
-   
-   101        1138 LOAD_CONST               5 (3.6)
-   
-   102        1140 LOAD_CONST               6 (90)
-   
-   103        1142 LOAD_CONST               6 (90)
-   
-   104        1144 LOAD_CONST               7 (120)
-   
-   105        1146 LOAD_CONST              13 (6)
-   
-   106        1148 LOAD_CONST               1 (0)
-   
-   108        1150 BUILD_LIST               0
-              1152 LOAD_CONST               9 ((0, 0, 0))
-              1154 LIST_EXTEND              1
-              1156 LOAD_CONST               4 (30)
-              1158 LOAD_CONST              10 (('position', 'angle'))
-              1160 BUILD_CONST_KEY_MAP      2
-   
-   107        1162 BUILD_LIST               1
-   
-   111        1164 LOAD_CONST              17 (0.25)
-              1166 PUSH_NULL
-              1168 LOAD_NAME                2 (np)
-              1170 LOAD_ATTR                5 (sqrt)
-              1180 LOAD_CONST               8 (3)
-              1182 PRECALL                  1
-              1186 CALL                     1
-              1196 LOAD_CONST              19 (4)
-              1198 BINARY_OP               11 (/)
-              1202 LOAD_CONST               1 (0)
-              1204 BUILD_LIST               3
-              1206 LOAD_CONST               4 (30)
-              1208 LOAD_CONST              10 (('position', 'angle'))
-              1210 BUILD_CONST_KEY_MAP      2
-   
-   112        1212 BUILD_LIST               0
-              1214 LOAD_CONST              32 ((0.5, 0, 0))
-              1216 LIST_EXTEND              1
-              1218 LOAD_CONST               6 (90)
-              1220 LOAD_CONST              10 (('position', 'angle'))
-              1222 BUILD_CONST_KEY_MAP      2
-   
-   113        1224 LOAD_CONST              14 (-0.25)
-              1226 PUSH_NULL
-              1228 LOAD_NAME                2 (np)
-              1230 LOAD_ATTR                5 (sqrt)
-              1240 LOAD_CONST               8 (3)
-              1242 PRECALL                  1
-              1246 CALL                     1
-              1256 LOAD_CONST              19 (4)
-              1258 BINARY_OP               11 (/)
-              1262 LOAD_CONST               1 (0)
-              1264 BUILD_LIST               3
-              1266 LOAD_CONST              33 (-30)
-              1268 LOAD_CONST              10 (('position', 'angle'))
-              1270 BUILD_CONST_KEY_MAP      2
-   
-   110        1272 BUILD_LIST               3
-   
-    98        1274 LOAD_CONST              12 (('a', 'b', 'c', 'alpha', 'beta', 'gamma', 'vertice_connectivity', 'edge_connectivity', 'vertices', 'edges'))
-              1276 BUILD_CONST_KEY_MAP     10
-   
-   117        1278 LOAD_CONST              19 (4)
-   
-   118        1280 LOAD_CONST              19 (4)
-   
-   119        1282 LOAD_CONST               5 (3.6)
-   
-   120        1284 LOAD_CONST               6 (90)
-   
-   121        1286 LOAD_CONST               6 (90)
-   
-   122        1288 LOAD_CONST               7 (120)
-   
-   123        1290 LOAD_CONST              19 (4)
-   
-   124        1292 LOAD_CONST               1 (0)
-   
-   126        1294 LOAD_CONST              17 (0.25)
-              1296 PUSH_NULL
-              1298 LOAD_NAME                2 (np)
-              1300 LOAD_ATTR                5 (sqrt)
-              1310 LOAD_CONST               8 (3)
-              1312 PRECALL                  1
-              1316 CALL                     1
-              1326 LOAD_CONST              19 (4)
-              1328 BINARY_OP               11 (/)
-              1332 LOAD_CONST               1 (0)
-              1334 BUILD_LIST               3
-              1336 LOAD_CONST               4 (30)
-              1338 LOAD_CONST              10 (('position', 'angle'))
-              1340 BUILD_CONST_KEY_MAP      2
-   
-   127        1342 BUILD_LIST               0
-              1344 LOAD_CONST              32 ((0.5, 0, 0))
-              1346 LIST_EXTEND              1
-              1348 LOAD_CONST              34 (-90)
-              1350 LOAD_CONST              10 (('position', 'angle'))
-              1352 BUILD_CONST_KEY_MAP      2
-   
-   128        1354 LOAD_CONST              14 (-0.25)
-              1356 PUSH_NULL
-              1358 LOAD_NAME                2 (np)
-              1360 LOAD_ATTR                5 (sqrt)
-              1370 LOAD_CONST               8 (3)
-              1372 PRECALL                  1
-              1376 CALL                     1
-              1386 LOAD_CONST              19 (4)
-              1388 BINARY_OP               11 (/)
-              1392 LOAD_CONST               1 (0)
-              1394 BUILD_LIST               3
-              1396 LOAD_CONST              33 (-30)
-              1398 LOAD_CONST              10 (('position', 'angle'))
-              1400 BUILD_CONST_KEY_MAP      2
-   
-   125        1402 BUILD_LIST               3
-   
-   130        1404 BUILD_LIST               0
-   
-   116        1406 LOAD_CONST              12 (('a', 'b', 'c', 'alpha', 'beta', 'gamma', 'vertice_connectivity', 'edge_connectivity', 'vertices', 'edges'))
-              1408 BUILD_CONST_KEY_MAP     10
-   
-   133        1410 LOAD_CONST              19 (4)
-   
-   134        1412 LOAD_CONST              19 (4)
-   
-   135        1414 LOAD_CONST               5 (3.6)
-   
-   136        1416 LOAD_CONST               6 (90)
-   
-   137        1418 LOAD_CONST               6 (90)
-   
-   138        1420 LOAD_CONST               7 (120)
-   
-   139        1422 LOAD_CONST              19 (4)
-   
-   140        1424 LOAD_CONST               3 (2)
-   
-   142        1426 LOAD_CONST              17 (0.25)
-              1428 PUSH_NULL
-              1430 LOAD_NAME                2 (np)
-              1432 LOAD_ATTR                5 (sqrt)
-              1442 LOAD_CONST               8 (3)
-              1444 PRECALL                  1
-              1448 CALL                     1
-              1458 LOAD_CONST              19 (4)
-              1460 BINARY_OP               11 (/)
-              1464 LOAD_CONST               1 (0)
-              1466 BUILD_LIST               3
-              1468 LOAD_CONST               4 (30)
-              1470 LOAD_CONST              10 (('position', 'angle'))
-              1472 BUILD_CONST_KEY_MAP      2
-   
-   143        1474 BUILD_LIST               0
-              1476 LOAD_CONST              32 ((0.5, 0, 0))
-              1478 LIST_EXTEND              1
-              1480 LOAD_CONST              34 (-90)
-              1482 LOAD_CONST              10 (('position', 'angle'))
-              1484 BUILD_CONST_KEY_MAP      2
-   
-   144        1486 LOAD_CONST              14 (-0.25)
-              1488 PUSH_NULL
-              1490 LOAD_NAME                2 (np)
-              1492 LOAD_ATTR                5 (sqrt)
-              1502 LOAD_CONST               8 (3)
-              1504 PRECALL                  1
-              1508 CALL                     1
-              1518 LOAD_CONST              19 (4)
-              1520 BINARY_OP               11 (/)
-              1524 LOAD_CONST               1 (0)
-              1526 BUILD_LIST               3
-              1528 LOAD_CONST              33 (-30)
-              1530 LOAD_CONST              10 (('position', 'angle'))
-              1532 BUILD_CONST_KEY_MAP      2
-   
-   141        1534 BUILD_LIST               3
-   
-   147        1536 LOAD_CONST              35 (0.375)
-              1538 PUSH_NULL
-              1540 LOAD_NAME                2 (np)
-              1542 LOAD_ATTR                5 (sqrt)
-              1552 LOAD_CONST               8 (3)
-              1554 PRECALL                  1
-              1558 CALL                     1
-              1568 LOAD_CONST              36 (8)
-              1570 BINARY_OP               11 (/)
-              1574 LOAD_CONST               1 (0)
-              1576 BUILD_LIST               3
-              1578 LOAD_CONST              33 (-30)
-              1580 LOAD_CONST              10 (('position', 'angle'))
-              1582 BUILD_CONST_KEY_MAP      2
-   
-   148        1584 LOAD_CONST              37 (0.125)
-              1586 LOAD_CONST               8 (3)
-              1588 PUSH_NULL
-              1590 LOAD_NAME                2 (np)
-              1592 LOAD_ATTR                5 (sqrt)
-              1602 LOAD_CONST               8 (3)
-              1604 PRECALL                  1
-              1608 CALL                     1
-              1618 BINARY_OP                5 (*)
-              1622 LOAD_CONST              36 (8)
-              1624 BINARY_OP               11 (/)
-              1628 LOAD_CONST               1 (0)
-              1630 BUILD_LIST               3
-              1632 LOAD_CONST              33 (-30)
-              1634 LOAD_CONST              10 (('position', 'angle'))
-              1636 BUILD_CONST_KEY_MAP      2
-   
-   149        1638 LOAD_CONST              38 (0.625)
-              1640 PUSH_NULL
-              1642 LOAD_NAME                2 (np)
-              1644 LOAD_ATTR                5 (sqrt)
-              1654 LOAD_CONST               8 (3)
-              1656 PRECALL                  1
-              1660 CALL                     1
-              1670 LOAD_CONST              36 (8)
-              1672 BINARY_OP               11 (/)
-              1676 LOAD_CONST               1 (0)
-              1678 BUILD_LIST               3
-              1680 LOAD_CONST               4 (30)
-              1682 LOAD_CONST              10 (('position', 'angle'))
-              1684 BUILD_CONST_KEY_MAP      2
-   
-   150        1686 LOAD_CONST              39 (-0.125)
-              1688 PUSH_NULL
-              1690 LOAD_NAME                2 (np)
-              1692 LOAD_ATTR                5 (sqrt)
-              1702 LOAD_CONST               8 (3)
-              1704 PRECALL                  1
-              1708 CALL                     1
-              1718 LOAD_CONST              36 (8)
-              1720 BINARY_OP               11 (/)
-              1724 LOAD_CONST               1 (0)
-              1726 BUILD_LIST               3
-              1728 LOAD_CONST               4 (30)
-              1730 LOAD_CONST              10 (('position', 'angle'))
-              1732 BUILD_CONST_KEY_MAP      2
-   
-   151        1734 LOAD_CONST              31 (0.5)
-              1736 PUSH_NULL
-              1738 LOAD_NAME                2 (np)
-              1740 LOAD_ATTR                5 (sqrt)
-              1750 LOAD_CONST               8 (3)
-              1752 PRECALL                  1
-              1756 CALL                     1
-              1766 LOAD_CONST              19 (4)
-              1768 BINARY_OP               11 (/)
-              1772 LOAD_CONST               1 (0)
-              1774 BUILD_LIST               3
-              1776 LOAD_CONST               6 (90)
+    47         598 LOAD_CONST              19 (1)
+   
+    48         600 LOAD_CONST              19 (1)
+   
+    49         602 LOAD_CONST               5 (3.6)
+   
+    50         604 LOAD_CONST               6 (90)
+   
+    51         606 LOAD_CONST               6 (90)
+   
+    52         608 LOAD_CONST               6 (90)
+   
+    53         610 LOAD_CONST              20 (4)
+   
+    54         612 LOAD_CONST               1 (0)
+   
+    56         614 BUILD_LIST               0
+               616 LOAD_CONST               9 ((0, 0, 0))
+               618 LIST_EXTEND              1
+               620 LOAD_CONST              21 (45)
+               622 LOAD_CONST              10 (('position', 'angle'))
+               624 BUILD_CONST_KEY_MAP      2
+   
+    57         626 BUILD_LIST               0
+               628 LOAD_CONST              22 ((0.5, 0.5, 0))
+               630 LIST_EXTEND              1
+               632 LOAD_CONST              21 (45)
+               634 LOAD_CONST              10 (('position', 'angle'))
+               636 BUILD_CONST_KEY_MAP      2
+   
+    55         638 BUILD_LIST               2
+   
+    59         640 BUILD_LIST               0
+   
+    46         642 LOAD_CONST              12 (('a', 'b', 'c', 'alpha', 'beta', 'gamma', 'vertice_connectivity', 'edge_connectivity', 'vertices', 'edges'))
+               644 BUILD_CONST_KEY_MAP     10
+   
+    62         646 LOAD_CONST              19 (1)
+   
+    63         648 LOAD_CONST              19 (1)
+   
+    64         650 LOAD_CONST               5 (3.6)
+   
+    65         652 LOAD_CONST               6 (90)
+   
+    66         654 LOAD_CONST               6 (90)
+   
+    67         656 LOAD_CONST               6 (90)
+   
+    68         658 LOAD_CONST              20 (4)
+   
+    69         660 LOAD_CONST               3 (2)
+   
+    71         662 BUILD_LIST               0
+               664 LOAD_CONST               9 ((0, 0, 0))
+               666 LIST_EXTEND              1
+               668 LOAD_CONST              23 (-45)
+               670 LOAD_CONST              10 (('position', 'angle'))
+               672 BUILD_CONST_KEY_MAP      2
+   
+    72         674 BUILD_LIST               0
+               676 LOAD_CONST              22 ((0.5, 0.5, 0))
+               678 LIST_EXTEND              1
+               680 LOAD_CONST              23 (-45)
+               682 LOAD_CONST              10 (('position', 'angle'))
+               684 BUILD_CONST_KEY_MAP      2
+   
+    70         686 BUILD_LIST               2
+   
+    75         688 BUILD_LIST               0
+               690 LOAD_CONST              24 ((0.25, 0.25, 0))
+               692 LIST_EXTEND              1
+               694 LOAD_CONST              21 (45)
+               696 LOAD_CONST              10 (('position', 'angle'))
+               698 BUILD_CONST_KEY_MAP      2
+   
+    76         700 BUILD_LIST               0
+               702 LOAD_CONST              25 ((0.75, 0.25, 0))
+               704 LIST_EXTEND              1
+               706 LOAD_CONST              26 (135)
+               708 LOAD_CONST              10 (('position', 'angle'))
+               710 BUILD_CONST_KEY_MAP      2
+   
+    77         712 BUILD_LIST               0
+               714 LOAD_CONST              27 ((0.75, 0.75, 0))
+               716 LIST_EXTEND              1
+               718 LOAD_CONST              28 (225)
+               720 LOAD_CONST              10 (('position', 'angle'))
+               722 BUILD_CONST_KEY_MAP      2
+   
+    78         724 BUILD_LIST               0
+               726 LOAD_CONST              29 ((0.25, 0.75, 0))
+               728 LIST_EXTEND              1
+               730 LOAD_CONST              30 (315)
+               732 LOAD_CONST              10 (('position', 'angle'))
+               734 BUILD_CONST_KEY_MAP      2
+   
+    74         736 BUILD_LIST               4
+   
+    61         738 LOAD_CONST              12 (('a', 'b', 'c', 'alpha', 'beta', 'gamma', 'vertice_connectivity', 'edge_connectivity', 'vertices', 'edges'))
+               740 BUILD_CONST_KEY_MAP     10
+   
+    82         742 LOAD_CONST               3 (2)
+               744 PUSH_NULL
+               746 LOAD_NAME                2 (np)
+               748 LOAD_ATTR                3 (cos)
+               758 PUSH_NULL
+               760 LOAD_NAME                2 (np)
+               762 LOAD_ATTR                4 (radians)
+               772 LOAD_CONST               4 (30)
+               774 PRECALL                  1
+               778 CALL                     1
+               788 PRECALL                  1
+               792 CALL                     1
+               802 BINARY_OP                5 (*)
+   
+    83         806 LOAD_CONST               3 (2)
+               808 PUSH_NULL
+               810 LOAD_NAME                2 (np)
+               812 LOAD_ATTR                3 (cos)
+               822 PUSH_NULL
+               824 LOAD_NAME                2 (np)
+               826 LOAD_ATTR                4 (radians)
+               836 LOAD_CONST               4 (30)
+               838 PRECALL                  1
+               842 CALL                     1
+               852 PRECALL                  1
+               856 CALL                     1
+               866 BINARY_OP                5 (*)
+   
+    84         870 LOAD_CONST               5 (3.6)
+   
+    85         872 LOAD_CONST               6 (90)
+   
+    86         874 LOAD_CONST               6 (90)
+   
+    87         876 LOAD_CONST               7 (120)
+   
+    88         878 LOAD_CONST              13 (6)
+   
+    89         880 LOAD_CONST               8 (3)
+   
+    91         882 BUILD_LIST               0
+               884 LOAD_CONST               9 ((0, 0, 0))
+               886 LIST_EXTEND              1
+               888 LOAD_CONST               1 (0)
+               890 LOAD_CONST              10 (('position', 'angle'))
+               892 BUILD_CONST_KEY_MAP      2
+   
+    90         894 BUILD_LIST               1
+   
+    94         896 LOAD_CONST               1 (0)
+               898 PUSH_NULL
+               900 LOAD_NAME                2 (np)
+               902 LOAD_ATTR                5 (sqrt)
+               912 LOAD_CONST               8 (3)
+               914 PRECALL                  1
+               918 CALL                     1
+               928 LOAD_CONST               8 (3)
+               930 BINARY_OP               11 (/)
+               934 LOAD_CONST               1 (0)
+               936 BUILD_LIST               3
+               938 LOAD_CONST              31 (-180)
+               940 LOAD_CONST              10 (('position', 'angle'))
+               942 BUILD_CONST_KEY_MAP      2
+   
+    95         944 LOAD_CONST              32 (0.5)
+               946 PUSH_NULL
+               948 LOAD_NAME                2 (np)
+               950 LOAD_ATTR                5 (sqrt)
+               960 LOAD_CONST               8 (3)
+               962 PRECALL                  1
+               966 CALL                     1
+               976 LOAD_CONST              13 (6)
+               978 BINARY_OP               11 (/)
+               982 LOAD_CONST               1 (0)
+               984 BUILD_LIST               3
+               986 LOAD_CONST               1 (0)
+               988 LOAD_CONST              10 (('position', 'angle'))
+               990 BUILD_CONST_KEY_MAP      2
+   
+    93         992 BUILD_LIST               2
+   
+    81         994 LOAD_CONST              12 (('a', 'b', 'c', 'alpha', 'beta', 'gamma', 'vertice_connectivity', 'edge_connectivity', 'vertices', 'edges'))
+               996 BUILD_CONST_KEY_MAP     10
+   
+    99         998 LOAD_CONST               3 (2)
+   
+   100        1000 LOAD_CONST               3 (2)
+   
+   101        1002 LOAD_CONST               5 (3.6)
+   
+   102        1004 LOAD_CONST               6 (90)
+   
+   103        1006 LOAD_CONST               6 (90)
+   
+   104        1008 LOAD_CONST               7 (120)
+   
+   105        1010 LOAD_CONST              13 (6)
+   
+   106        1012 LOAD_CONST               1 (0)
+   
+   108        1014 BUILD_LIST               0
+              1016 LOAD_CONST               9 ((0, 0, 0))
+              1018 LIST_EXTEND              1
+              1020 LOAD_CONST               4 (30)
+              1022 LOAD_CONST              10 (('position', 'angle'))
+              1024 BUILD_CONST_KEY_MAP      2
+   
+   107        1026 BUILD_LIST               1
+   
+   111        1028 LOAD_CONST              17 (0.25)
+              1030 PUSH_NULL
+              1032 LOAD_NAME                2 (np)
+              1034 LOAD_ATTR                5 (sqrt)
+              1044 LOAD_CONST               8 (3)
+              1046 PRECALL                  1
+              1050 CALL                     1
+              1060 LOAD_CONST              20 (4)
+              1062 BINARY_OP               11 (/)
+              1066 LOAD_CONST               1 (0)
+              1068 BUILD_LIST               3
+              1070 LOAD_CONST               4 (30)
+              1072 LOAD_CONST              10 (('position', 'angle'))
+              1074 BUILD_CONST_KEY_MAP      2
+   
+   112        1076 BUILD_LIST               0
+              1078 LOAD_CONST              33 ((0.5, 0, 0))
+              1080 LIST_EXTEND              1
+              1082 LOAD_CONST               6 (90)
+              1084 LOAD_CONST              10 (('position', 'angle'))
+              1086 BUILD_CONST_KEY_MAP      2
+   
+   113        1088 LOAD_CONST              14 (-0.25)
+              1090 PUSH_NULL
+              1092 LOAD_NAME                2 (np)
+              1094 LOAD_ATTR                5 (sqrt)
+              1104 LOAD_CONST               8 (3)
+              1106 PRECALL                  1
+              1110 CALL                     1
+              1120 LOAD_CONST              20 (4)
+              1122 BINARY_OP               11 (/)
+              1126 LOAD_CONST               1 (0)
+              1128 BUILD_LIST               3
+              1130 LOAD_CONST              34 (-30)
+              1132 LOAD_CONST              10 (('position', 'angle'))
+              1134 BUILD_CONST_KEY_MAP      2
+   
+   110        1136 BUILD_LIST               3
+   
+    98        1138 LOAD_CONST              12 (('a', 'b', 'c', 'alpha', 'beta', 'gamma', 'vertice_connectivity', 'edge_connectivity', 'vertices', 'edges'))
+              1140 BUILD_CONST_KEY_MAP     10
+   
+   117        1142 LOAD_CONST              20 (4)
+   
+   118        1144 LOAD_CONST              20 (4)
+   
+   119        1146 LOAD_CONST               5 (3.6)
+   
+   120        1148 LOAD_CONST               6 (90)
+   
+   121        1150 LOAD_CONST               6 (90)
+   
+   122        1152 LOAD_CONST               7 (120)
+   
+   123        1154 LOAD_CONST              20 (4)
+   
+   124        1156 LOAD_CONST               1 (0)
+   
+   126        1158 LOAD_CONST              17 (0.25)
+              1160 PUSH_NULL
+              1162 LOAD_NAME                2 (np)
+              1164 LOAD_ATTR                5 (sqrt)
+              1174 LOAD_CONST               8 (3)
+              1176 PRECALL                  1
+              1180 CALL                     1
+              1190 LOAD_CONST              20 (4)
+              1192 BINARY_OP               11 (/)
+              1196 LOAD_CONST               1 (0)
+              1198 BUILD_LIST               3
+              1200 LOAD_CONST               4 (30)
+              1202 LOAD_CONST              10 (('position', 'angle'))
+              1204 BUILD_CONST_KEY_MAP      2
+   
+   127        1206 BUILD_LIST               0
+              1208 LOAD_CONST              33 ((0.5, 0, 0))
+              1210 LIST_EXTEND              1
+              1212 LOAD_CONST              35 (-90)
+              1214 LOAD_CONST              10 (('position', 'angle'))
+              1216 BUILD_CONST_KEY_MAP      2
+   
+   128        1218 LOAD_CONST              14 (-0.25)
+              1220 PUSH_NULL
+              1222 LOAD_NAME                2 (np)
+              1224 LOAD_ATTR                5 (sqrt)
+              1234 LOAD_CONST               8 (3)
+              1236 PRECALL                  1
+              1240 CALL                     1
+              1250 LOAD_CONST              20 (4)
+              1252 BINARY_OP               11 (/)
+              1256 LOAD_CONST               1 (0)
+              1258 BUILD_LIST               3
+              1260 LOAD_CONST              34 (-30)
+              1262 LOAD_CONST              10 (('position', 'angle'))
+              1264 BUILD_CONST_KEY_MAP      2
+   
+   125        1266 BUILD_LIST               3
+   
+   130        1268 BUILD_LIST               0
+   
+   116        1270 LOAD_CONST              12 (('a', 'b', 'c', 'alpha', 'beta', 'gamma', 'vertice_connectivity', 'edge_connectivity', 'vertices', 'edges'))
+              1272 BUILD_CONST_KEY_MAP     10
+   
+   133        1274 LOAD_CONST              20 (4)
+   
+   134        1276 LOAD_CONST              20 (4)
+   
+   135        1278 LOAD_CONST               5 (3.6)
+   
+   136        1280 LOAD_CONST               6 (90)
+   
+   137        1282 LOAD_CONST               6 (90)
+   
+   138        1284 LOAD_CONST               7 (120)
+   
+   139        1286 LOAD_CONST              20 (4)
+   
+   140        1288 LOAD_CONST               3 (2)
+   
+   142        1290 LOAD_CONST              17 (0.25)
+              1292 PUSH_NULL
+              1294 LOAD_NAME                2 (np)
+              1296 LOAD_ATTR                5 (sqrt)
+              1306 LOAD_CONST               8 (3)
+              1308 PRECALL                  1
+              1312 CALL                     1
+              1322 LOAD_CONST              20 (4)
+              1324 BINARY_OP               11 (/)
+              1328 LOAD_CONST               1 (0)
+              1330 BUILD_LIST               3
+              1332 LOAD_CONST               4 (30)
+              1334 LOAD_CONST              10 (('position', 'angle'))
+              1336 BUILD_CONST_KEY_MAP      2
+   
+   143        1338 BUILD_LIST               0
+              1340 LOAD_CONST              33 ((0.5, 0, 0))
+              1342 LIST_EXTEND              1
+              1344 LOAD_CONST              35 (-90)
+              1346 LOAD_CONST              10 (('position', 'angle'))
+              1348 BUILD_CONST_KEY_MAP      2
+   
+   144        1350 LOAD_CONST              14 (-0.25)
+              1352 PUSH_NULL
+              1354 LOAD_NAME                2 (np)
+              1356 LOAD_ATTR                5 (sqrt)
+              1366 LOAD_CONST               8 (3)
+              1368 PRECALL                  1
+              1372 CALL                     1
+              1382 LOAD_CONST              20 (4)
+              1384 BINARY_OP               11 (/)
+              1388 LOAD_CONST               1 (0)
+              1390 BUILD_LIST               3
+              1392 LOAD_CONST              34 (-30)
+              1394 LOAD_CONST              10 (('position', 'angle'))
+              1396 BUILD_CONST_KEY_MAP      2
+   
+   141        1398 BUILD_LIST               3
+   
+   147        1400 LOAD_CONST              36 (0.375)
+              1402 PUSH_NULL
+              1404 LOAD_NAME                2 (np)
+              1406 LOAD_ATTR                5 (sqrt)
+              1416 LOAD_CONST               8 (3)
+              1418 PRECALL                  1
+              1422 CALL                     1
+              1432 LOAD_CONST              37 (8)
+              1434 BINARY_OP               11 (/)
+              1438 LOAD_CONST               1 (0)
+              1440 BUILD_LIST               3
+              1442 LOAD_CONST              34 (-30)
+              1444 LOAD_CONST              10 (('position', 'angle'))
+              1446 BUILD_CONST_KEY_MAP      2
+   
+   148        1448 LOAD_CONST              38 (0.125)
+              1450 LOAD_CONST               8 (3)
+              1452 PUSH_NULL
+              1454 LOAD_NAME                2 (np)
+              1456 LOAD_ATTR                5 (sqrt)
+              1466 LOAD_CONST               8 (3)
+              1468 PRECALL                  1
+              1472 CALL                     1
+              1482 BINARY_OP                5 (*)
+              1486 LOAD_CONST              37 (8)
+              1488 BINARY_OP               11 (/)
+              1492 LOAD_CONST               1 (0)
+              1494 BUILD_LIST               3
+              1496 LOAD_CONST              34 (-30)
+              1498 LOAD_CONST              10 (('position', 'angle'))
+              1500 BUILD_CONST_KEY_MAP      2
+   
+   149        1502 LOAD_CONST              39 (0.625)
+              1504 PUSH_NULL
+              1506 LOAD_NAME                2 (np)
+              1508 LOAD_ATTR                5 (sqrt)
+              1518 LOAD_CONST               8 (3)
+              1520 PRECALL                  1
+              1524 CALL                     1
+              1534 LOAD_CONST              37 (8)
+              1536 BINARY_OP               11 (/)
+              1540 LOAD_CONST               1 (0)
+              1542 BUILD_LIST               3
+              1544 LOAD_CONST               4 (30)
+              1546 LOAD_CONST              10 (('position', 'angle'))
+              1548 BUILD_CONST_KEY_MAP      2
+   
+   150        1550 LOAD_CONST              40 (-0.125)
+              1552 PUSH_NULL
+              1554 LOAD_NAME                2 (np)
+              1556 LOAD_ATTR                5 (sqrt)
+              1566 LOAD_CONST               8 (3)
+              1568 PRECALL                  1
+              1572 CALL                     1
+              1582 LOAD_CONST              37 (8)
+              1584 BINARY_OP               11 (/)
+              1588 LOAD_CONST               1 (0)
+              1590 BUILD_LIST               3
+              1592 LOAD_CONST               4 (30)
+              1594 LOAD_CONST              10 (('position', 'angle'))
+              1596 BUILD_CONST_KEY_MAP      2
+   
+   151        1598 LOAD_CONST              32 (0.5)
+              1600 PUSH_NULL
+              1602 LOAD_NAME                2 (np)
+              1604 LOAD_ATTR                5 (sqrt)
+              1614 LOAD_CONST               8 (3)
+              1616 PRECALL                  1
+              1620 CALL                     1
+              1630 LOAD_CONST              20 (4)
+              1632 BINARY_OP               11 (/)
+              1636 LOAD_CONST               1 (0)
+              1638 BUILD_LIST               3
+              1640 LOAD_CONST               6 (90)
+              1642 LOAD_CONST              10 (('position', 'angle'))
+              1644 BUILD_CONST_KEY_MAP      2
+   
+   152        1646 LOAD_CONST               1 (0)
+              1648 PUSH_NULL
+              1650 LOAD_NAME                2 (np)
+              1652 LOAD_ATTR                5 (sqrt)
+              1662 LOAD_CONST               8 (3)
+              1664 PRECALL                  1
+              1668 CALL                     1
+              1678 LOAD_CONST              20 (4)
+              1680 BINARY_OP               11 (/)
+              1684 LOAD_CONST               1 (0)
+              1686 BUILD_LIST               3
+              1688 LOAD_CONST               6 (90)
+              1690 LOAD_CONST              10 (('position', 'angle'))
+              1692 BUILD_CONST_KEY_MAP      2
+   
+   146        1694 BUILD_LIST               6
+   
+   132        1696 LOAD_CONST              12 (('a', 'b', 'c', 'alpha', 'beta', 'gamma', 'vertice_connectivity', 'edge_connectivity', 'vertices', 'edges'))
+              1698 BUILD_CONST_KEY_MAP     10
+   
+   156        1700 LOAD_CONST              19 (1)
+   
+   157        1702 LOAD_CONST              19 (1)
+   
+   158        1704 LOAD_CONST               5 (3.6)
+   
+   159        1706 LOAD_CONST               6 (90)
+   
+   160        1708 LOAD_CONST               6 (90)
+   
+   161        1710 LOAD_CONST               7 (120)
+   
+   162        1712 LOAD_CONST              20 (4)
+   
+   163        1714 LOAD_CONST               3 (2)
+   
+   165        1716 LOAD_CONST              17 (0.25)
+              1718 LOAD_CONST               8 (3)
+              1720 PUSH_NULL
+              1722 LOAD_NAME                2 (np)
+              1724 LOAD_ATTR                5 (sqrt)
+              1734 LOAD_CONST               8 (3)
+              1736 PRECALL                  1
+              1740 CALL                     1
+              1750 BINARY_OP                5 (*)
+              1754 LOAD_CONST              16 (12)
+              1756 BINARY_OP               11 (/)
+              1760 LOAD_CONST               1 (0)
+              1762 BUILD_LIST               3
+              1764 LOAD_CONST              41 (-15)
+              1766 LOAD_CONST              10 (('position', 'angle'))
+              1768 BUILD_CONST_KEY_MAP      2
+   
+   166        1770 BUILD_LIST               0
+              1772 LOAD_CONST              33 ((0.5, 0, 0))
+              1774 LIST_EXTEND              1
+              1776 LOAD_CONST              21 (45)
               1778 LOAD_CONST              10 (('position', 'angle'))
               1780 BUILD_CONST_KEY_MAP      2
    
-   152        1782 LOAD_CONST               1 (0)
-              1784 PUSH_NULL
-              1786 LOAD_NAME                2 (np)
-              1788 LOAD_ATTR                5 (sqrt)
-              1798 LOAD_CONST               8 (3)
-              1800 PRECALL                  1
-              1804 CALL                     1
-              1814 LOAD_CONST              19 (4)
-              1816 BINARY_OP               11 (/)
-              1820 LOAD_CONST               1 (0)
-              1822 BUILD_LIST               3
-              1824 LOAD_CONST               6 (90)
-              1826 LOAD_CONST              10 (('position', 'angle'))
-              1828 BUILD_CONST_KEY_MAP      2
-   
-   146        1830 BUILD_LIST               6
-   
-   132        1832 LOAD_CONST              12 (('a', 'b', 'c', 'alpha', 'beta', 'gamma', 'vertice_connectivity', 'edge_connectivity', 'vertices', 'edges'))
-              1834 BUILD_CONST_KEY_MAP     10
-   
-   156        1836 LOAD_CONST              40 (1)
-   
-   157        1838 LOAD_CONST              40 (1)
-   
-   158        1840 LOAD_CONST               5 (3.6)
-   
-   159        1842 LOAD_CONST               6 (90)
-   
-   160        1844 LOAD_CONST               6 (90)
-   
-   161        1846 LOAD_CONST               7 (120)
-   
-   162        1848 LOAD_CONST              19 (4)
-   
-   163        1850 LOAD_CONST               3 (2)
-   
-   165        1852 LOAD_CONST              17 (0.25)
-              1854 LOAD_CONST               8 (3)
-              1856 PUSH_NULL
-              1858 LOAD_NAME                2 (np)
-              1860 LOAD_ATTR                5 (sqrt)
-              1870 LOAD_CONST               8 (3)
-              1872 PRECALL                  1
-              1876 CALL                     1
-              1886 BINARY_OP                5 (*)
-              1890 LOAD_CONST              16 (12)
-              1892 BINARY_OP               11 (/)
-              1896 LOAD_CONST               1 (0)
-              1898 BUILD_LIST               3
-              1900 LOAD_CONST              41 (-15)
-              1902 LOAD_CONST              10 (('position', 'angle'))
-              1904 BUILD_CONST_KEY_MAP      2
-   
-   166        1906 BUILD_LIST               0
-              1908 LOAD_CONST              32 ((0.5, 0, 0))
-              1910 LIST_EXTEND              1
-              1912 LOAD_CONST              20 (45)
-              1914 LOAD_CONST              10 (('position', 'angle'))
-              1916 BUILD_CONST_KEY_MAP      2
-   
-   167        1918 LOAD_CONST              14 (-0.25)
-              1920 LOAD_CONST               8 (3)
-              1922 PUSH_NULL
-              1924 LOAD_NAME                2 (np)
-              1926 LOAD_ATTR                5 (sqrt)
-              1936 LOAD_CONST               8 (3)
-              1938 PRECALL                  1
-              1942 CALL                     1
-              1952 BINARY_OP                5 (*)
-              1956 LOAD_CONST              16 (12)
-              1958 BINARY_OP               11 (/)
-              1962 LOAD_CONST               1 (0)
-              1964 BUILD_LIST               3
-              1966 LOAD_CONST              42 (15)
-              1968 LOAD_CONST              10 (('position', 'angle'))
-              1970 BUILD_CONST_KEY_MAP      2
-   
-   164        1972 BUILD_LIST               3
-   
-   169        1974 BUILD_LIST               0
-   
-   155        1976 LOAD_CONST              12 (('a', 'b', 'c', 'alpha', 'beta', 'gamma', 'vertice_connectivity', 'edge_connectivity', 'vertices', 'edges'))
-              1978 BUILD_CONST_KEY_MAP     10
-   
-   172        1980 LOAD_CONST               3 (2)
-   
-   173        1982 LOAD_CONST               3 (2)
-   
-   174        1984 LOAD_CONST               5 (3.6)
-   
-   175        1986 LOAD_CONST               6 (90)
-   
-   176        1988 LOAD_CONST               6 (90)
-   
-   177        1990 LOAD_CONST               7 (120)
-   
-   178        1992 LOAD_CONST              19 (4)
-   
-   179        1994 LOAD_CONST               3 (2)
-   
-   181        1996 LOAD_CONST              17 (0.25)
-              1998 LOAD_CONST               8 (3)
-              2000 PUSH_NULL
-              2002 LOAD_NAME                2 (np)
-              2004 LOAD_ATTR                5 (sqrt)
-              2014 LOAD_CONST               8 (3)
-              2016 PRECALL                  1
-              2020 CALL                     1
-              2030 BINARY_OP                5 (*)
-              2034 LOAD_CONST              16 (12)
-              2036 BINARY_OP               11 (/)
-              2040 LOAD_CONST               1 (0)
-              2042 BUILD_LIST               3
-              2044 LOAD_CONST              41 (-15)
-              2046 LOAD_CONST              10 (('position', 'angle'))
-              2048 BUILD_CONST_KEY_MAP      2
-   
-   182        2050 BUILD_LIST               0
-              2052 LOAD_CONST              32 ((0.5, 0, 0))
-              2054 LIST_EXTEND              1
-              2056 LOAD_CONST              20 (45)
-              2058 LOAD_CONST              10 (('position', 'angle'))
-              2060 BUILD_CONST_KEY_MAP      2
-   
-   183        2062 LOAD_CONST              14 (-0.25)
-              2064 LOAD_CONST               8 (3)
-              2066 PUSH_NULL
-              2068 LOAD_NAME                2 (np)
-              2070 LOAD_ATTR                5 (sqrt)
-              2080 LOAD_CONST               8 (3)
-              2082 PRECALL                  1
-              2086 CALL                     1
-              2096 BINARY_OP                5 (*)
-              2100 LOAD_CONST              16 (12)
-              2102 BINARY_OP               11 (/)
-              2106 LOAD_CONST               1 (0)
-              2108 BUILD_LIST               3
-              2110 LOAD_CONST              42 (15)
-              2112 LOAD_CONST              10 (('position', 'angle'))
-              2114 BUILD_CONST_KEY_MAP      2
-   
-   180        2116 BUILD_LIST               3
-   
-   186        2118 LOAD_CONST              43 (0.34375)
-              2120 LOAD_CONST              44 (7)
-              2122 PUSH_NULL
-              2124 LOAD_NAME                2 (np)
-              2126 LOAD_ATTR                5 (sqrt)
-              2136 LOAD_CONST               8 (3)
-              2138 PRECALL                  1
-              2142 CALL                     1
-              2152 BINARY_OP                5 (*)
-              2156 LOAD_CONST              45 (64)
-              2158 BINARY_OP               11 (/)
-              2162 LOAD_CONST               1 (0)
-              2164 BUILD_LIST               3
-              2166 LOAD_CONST              33 (-30)
-              2168 LOAD_CONST              10 (('position', 'angle'))
-              2170 BUILD_CONST_KEY_MAP      2
-   
-   187        2172 LOAD_CONST              46 (0.6640625)
-              2174 LOAD_CONST              44 (7)
-              2176 PUSH_NULL
-              2178 LOAD_NAME                2 (np)
-              2180 LOAD_ATTR                5 (sqrt)
-              2190 LOAD_CONST               8 (3)
-              2192 PRECALL                  1
-              2196 CALL                     1
-              2206 BINARY_OP                5 (*)
-              2210 LOAD_CONST              45 (64)
-              2212 BINARY_OP               11 (/)
-              2216 LOAD_CONST               1 (0)
-              2218 BUILD_LIST               3
-              2220 LOAD_CONST               4 (30)
-              2222 LOAD_CONST              10 (('position', 'angle'))
-              2224 BUILD_CONST_KEY_MAP      2
-   
-   188        2226 LOAD_CONST              31 (0.5)
-              2228 LOAD_CONST              47 (35)
-              2230 PUSH_NULL
-              2232 LOAD_NAME                2 (np)
-              2234 LOAD_ATTR                5 (sqrt)
-              2244 LOAD_CONST               8 (3)
-              2246 PRECALL                  1
-              2250 CALL                     1
-              2260 BINARY_OP                5 (*)
-              2264 LOAD_CONST              48 (128)
-              2266 BINARY_OP               11 (/)
-              2270 LOAD_CONST               1 (0)
-              2272 BUILD_LIST               3
-              2274 LOAD_CONST               6 (90)
-              2276 LOAD_CONST              10 (('position', 'angle'))
-              2278 BUILD_CONST_KEY_MAP      2
-   
-   189        2280 LOAD_CONST               1 (0)
-              2282 LOAD_CONST              49 (29)
-              2284 PUSH_NULL
-              2286 LOAD_NAME                2 (np)
-              2288 LOAD_ATTR                5 (sqrt)
-              2298 LOAD_CONST               8 (3)
-              2300 PRECALL                  1
-              2304 CALL                     1
-              2314 BINARY_OP                5 (*)
-              2318 LOAD_CONST              48 (128)
-              2320 BINARY_OP               11 (/)
-              2324 LOAD_CONST               1 (0)
-              2326 BUILD_LIST               3
-              2328 LOAD_CONST               6 (90)
-              2330 LOAD_CONST              10 (('position', 'angle'))
-              2332 BUILD_CONST_KEY_MAP      2
-   
-   190        2334 LOAD_CONST              50 (0.1640625)
-              2336 LOAD_CONST              51 (25)
-              2338 PUSH_NULL
-              2340 LOAD_NAME                2 (np)
-              2342 LOAD_ATTR                5 (sqrt)
-              2352 LOAD_CONST               8 (3)
-              2354 PRECALL                  1
-              2358 CALL                     1
-              2368 BINARY_OP                5 (*)
-              2372 LOAD_CONST              45 (64)
-              2374 BINARY_OP               11 (/)
-              2378 LOAD_CONST               1 (0)
-              2380 BUILD_LIST               3
-              2382 LOAD_CONST              33 (-30)
-              2384 LOAD_CONST              10 (('position', 'angle'))
-              2386 BUILD_CONST_KEY_MAP      2
-   
-   191        2388 LOAD_CONST              52 (-0.1640625)
-              2390 LOAD_CONST              51 (25)
-              2392 PUSH_NULL
-              2394 LOAD_NAME                2 (np)
-              2396 LOAD_ATTR                5 (sqrt)
-              2406 LOAD_CONST               8 (3)
-              2408 PRECALL                  1
-              2412 CALL                     1
-              2422 BINARY_OP                5 (*)
-              2426 LOAD_CONST              45 (64)
-              2428 BINARY_OP               11 (/)
-              2432 LOAD_CONST               1 (0)
-              2434 BUILD_LIST               3
-              2436 LOAD_CONST               4 (30)
-              2438 LOAD_CONST              10 (('position', 'angle'))
-              2440 BUILD_CONST_KEY_MAP      2
-   
-   185        2442 BUILD_LIST               6
-   
-   171        2444 LOAD_CONST              12 (('a', 'b', 'c', 'alpha', 'beta', 'gamma', 'vertice_connectivity', 'edge_connectivity', 'vertices', 'edges'))
-              2446 BUILD_CONST_KEY_MAP     10
-   
-   195        2448 LOAD_CONST              40 (1)
-   
-   196        2450 LOAD_CONST              40 (1)
-   
-   197        2452 LOAD_CONST              40 (1)
-   
-   198        2454 LOAD_CONST              53 (60)
-   
-   199        2456 LOAD_CONST              53 (60)
-   
-   200        2458 LOAD_CONST              53 (60)
-   
-   201        2460 BUILD_LIST               0
-              2462 LOAD_CONST              54 ((0, 1, 1))
-              2464 LIST_EXTEND              1
-              2466 BUILD_LIST               0
-              2468 LOAD_CONST              55 ((1, 0, 1))
-              2470 LIST_EXTEND              1
-              2472 BUILD_LIST               0
-              2474 LOAD_CONST              56 ((1, 1, 0))
-              2476 LIST_EXTEND              1
-              2478 BUILD_LIST               3
+   167        1782 LOAD_CONST              14 (-0.25)
+              1784 LOAD_CONST               8 (3)
+              1786 PUSH_NULL
+              1788 LOAD_NAME                2 (np)
+              1790 LOAD_ATTR                5 (sqrt)
+              1800 LOAD_CONST               8 (3)
+              1802 PRECALL                  1
+              1806 CALL                     1
+              1816 BINARY_OP                5 (*)
+              1820 LOAD_CONST              16 (12)
+              1822 BINARY_OP               11 (/)
+              1826 LOAD_CONST               1 (0)
+              1828 BUILD_LIST               3
+              1830 LOAD_CONST              42 (15)
+              1832 LOAD_CONST              10 (('position', 'angle'))
+              1834 BUILD_CONST_KEY_MAP      2
+   
+   164        1836 BUILD_LIST               3
+   
+   169        1838 BUILD_LIST               0
+   
+   155        1840 LOAD_CONST              12 (('a', 'b', 'c', 'alpha', 'beta', 'gamma', 'vertice_connectivity', 'edge_connectivity', 'vertices', 'edges'))
+              1842 BUILD_CONST_KEY_MAP     10
+   
+   172        1844 LOAD_CONST               3 (2)
+   
+   173        1846 LOAD_CONST               3 (2)
+   
+   174        1848 LOAD_CONST               5 (3.6)
+   
+   175        1850 LOAD_CONST               6 (90)
+   
+   176        1852 LOAD_CONST               6 (90)
+   
+   177        1854 LOAD_CONST               7 (120)
+   
+   178        1856 LOAD_CONST              20 (4)
+   
+   179        1858 LOAD_CONST               3 (2)
+   
+   181        1860 LOAD_CONST              17 (0.25)
+              1862 LOAD_CONST               8 (3)
+              1864 PUSH_NULL
+              1866 LOAD_NAME                2 (np)
+              1868 LOAD_ATTR                5 (sqrt)
+              1878 LOAD_CONST               8 (3)
+              1880 PRECALL                  1
+              1884 CALL                     1
+              1894 BINARY_OP                5 (*)
+              1898 LOAD_CONST              16 (12)
+              1900 BINARY_OP               11 (/)
+              1904 LOAD_CONST               1 (0)
+              1906 BUILD_LIST               3
+              1908 LOAD_CONST              41 (-15)
+              1910 LOAD_CONST              10 (('position', 'angle'))
+              1912 BUILD_CONST_KEY_MAP      2
+   
+   182        1914 BUILD_LIST               0
+              1916 LOAD_CONST              33 ((0.5, 0, 0))
+              1918 LIST_EXTEND              1
+              1920 LOAD_CONST              21 (45)
+              1922 LOAD_CONST              10 (('position', 'angle'))
+              1924 BUILD_CONST_KEY_MAP      2
+   
+   183        1926 LOAD_CONST              14 (-0.25)
+              1928 LOAD_CONST               8 (3)
+              1930 PUSH_NULL
+              1932 LOAD_NAME                2 (np)
+              1934 LOAD_ATTR                5 (sqrt)
+              1944 LOAD_CONST               8 (3)
+              1946 PRECALL                  1
+              1950 CALL                     1
+              1960 BINARY_OP                5 (*)
+              1964 LOAD_CONST              16 (12)
+              1966 BINARY_OP               11 (/)
+              1970 LOAD_CONST               1 (0)
+              1972 BUILD_LIST               3
+              1974 LOAD_CONST              42 (15)
+              1976 LOAD_CONST              10 (('position', 'angle'))
+              1978 BUILD_CONST_KEY_MAP      2
+   
+   180        1980 BUILD_LIST               3
+   
+   186        1982 LOAD_CONST              43 (0.34375)
+              1984 LOAD_CONST              44 (7)
+              1986 PUSH_NULL
+              1988 LOAD_NAME                2 (np)
+              1990 LOAD_ATTR                5 (sqrt)
+              2000 LOAD_CONST               8 (3)
+              2002 PRECALL                  1
+              2006 CALL                     1
+              2016 BINARY_OP                5 (*)
+              2020 LOAD_CONST              45 (64)
+              2022 BINARY_OP               11 (/)
+              2026 LOAD_CONST               1 (0)
+              2028 BUILD_LIST               3
+              2030 LOAD_CONST              34 (-30)
+              2032 LOAD_CONST              10 (('position', 'angle'))
+              2034 BUILD_CONST_KEY_MAP      2
+   
+   187        2036 LOAD_CONST              46 (0.6640625)
+              2038 LOAD_CONST              44 (7)
+              2040 PUSH_NULL
+              2042 LOAD_NAME                2 (np)
+              2044 LOAD_ATTR                5 (sqrt)
+              2054 LOAD_CONST               8 (3)
+              2056 PRECALL                  1
+              2060 CALL                     1
+              2070 BINARY_OP                5 (*)
+              2074 LOAD_CONST              45 (64)
+              2076 BINARY_OP               11 (/)
+              2080 LOAD_CONST               1 (0)
+              2082 BUILD_LIST               3
+              2084 LOAD_CONST               4 (30)
+              2086 LOAD_CONST              10 (('position', 'angle'))
+              2088 BUILD_CONST_KEY_MAP      2
+   
+   188        2090 LOAD_CONST              32 (0.5)
+              2092 LOAD_CONST              47 (35)
+              2094 PUSH_NULL
+              2096 LOAD_NAME                2 (np)
+              2098 LOAD_ATTR                5 (sqrt)
+              2108 LOAD_CONST               8 (3)
+              2110 PRECALL                  1
+              2114 CALL                     1
+              2124 BINARY_OP                5 (*)
+              2128 LOAD_CONST              48 (128)
+              2130 BINARY_OP               11 (/)
+              2134 LOAD_CONST               1 (0)
+              2136 BUILD_LIST               3
+              2138 LOAD_CONST               6 (90)
+              2140 LOAD_CONST              10 (('position', 'angle'))
+              2142 BUILD_CONST_KEY_MAP      2
+   
+   189        2144 LOAD_CONST               1 (0)
+              2146 LOAD_CONST              49 (29)
+              2148 PUSH_NULL
+              2150 LOAD_NAME                2 (np)
+              2152 LOAD_ATTR                5 (sqrt)
+              2162 LOAD_CONST               8 (3)
+              2164 PRECALL                  1
+              2168 CALL                     1
+              2178 BINARY_OP                5 (*)
+              2182 LOAD_CONST              48 (128)
+              2184 BINARY_OP               11 (/)
+              2188 LOAD_CONST               1 (0)
+              2190 BUILD_LIST               3
+              2192 LOAD_CONST               6 (90)
+              2194 LOAD_CONST              10 (('position', 'angle'))
+              2196 BUILD_CONST_KEY_MAP      2
+   
+   190        2198 LOAD_CONST              50 (0.1640625)
+              2200 LOAD_CONST              51 (25)
+              2202 PUSH_NULL
+              2204 LOAD_NAME                2 (np)
+              2206 LOAD_ATTR                5 (sqrt)
+              2216 LOAD_CONST               8 (3)
+              2218 PRECALL                  1
+              2222 CALL                     1
+              2232 BINARY_OP                5 (*)
+              2236 LOAD_CONST              45 (64)
+              2238 BINARY_OP               11 (/)
+              2242 LOAD_CONST               1 (0)
+              2244 BUILD_LIST               3
+              2246 LOAD_CONST              34 (-30)
+              2248 LOAD_CONST              10 (('position', 'angle'))
+              2250 BUILD_CONST_KEY_MAP      2
+   
+   191        2252 LOAD_CONST              52 (-0.1640625)
+              2254 LOAD_CONST              51 (25)
+              2256 PUSH_NULL
+              2258 LOAD_NAME                2 (np)
+              2260 LOAD_ATTR                5 (sqrt)
+              2270 LOAD_CONST               8 (3)
+              2272 PRECALL                  1
+              2276 CALL                     1
+              2286 BINARY_OP                5 (*)
+              2290 LOAD_CONST              45 (64)
+              2292 BINARY_OP               11 (/)
+              2296 LOAD_CONST               1 (0)
+              2298 BUILD_LIST               3
+              2300 LOAD_CONST               4 (30)
+              2302 LOAD_CONST              10 (('position', 'angle'))
+              2304 BUILD_CONST_KEY_MAP      2
+   
+   185        2306 BUILD_LIST               6
+   
+   171        2308 LOAD_CONST              12 (('a', 'b', 'c', 'alpha', 'beta', 'gamma', 'vertice_connectivity', 'edge_connectivity', 'vertices', 'edges'))
+              2310 BUILD_CONST_KEY_MAP     10
+   
+   195        2312 LOAD_CONST              19 (1)
+   
+   196        2314 LOAD_CONST              19 (1)
+   
+   197        2316 LOAD_CONST              19 (1)
+   
+   198        2318 LOAD_CONST              53 (60)
+   
+   199        2320 LOAD_CONST              53 (60)
+   
+   200        2322 LOAD_CONST              53 (60)
+   
+   201        2324 BUILD_LIST               0
+              2326 LOAD_CONST              54 ((0, 1, 1))
+              2328 LIST_EXTEND              1
+              2330 BUILD_LIST               0
+              2332 LOAD_CONST              55 ((1, 0, 1))
+              2334 LIST_EXTEND              1
+              2336 BUILD_LIST               0
+              2338 LOAD_CONST              56 ((1, 1, 0))
+              2340 LIST_EXTEND              1
+              2342 BUILD_LIST               3
+   
+   202        2344 LOAD_CONST              20 (4)
+   
+   203        2346 LOAD_CONST              20 (4)
+   
+   205        2348 BUILD_LIST               0
+              2350 LOAD_CONST               9 ((0, 0, 0))
+              2352 LIST_EXTEND              1
+              2354 LOAD_CONST              57 (55)
+              2356 BUILD_LIST               0
+              2358 LOAD_CONST              58 ((1, 1, 1))
+              2360 LIST_EXTEND              1
+              2362 LOAD_CONST              59 (('position', 'angle', 'align_v'))
+              2364 BUILD_CONST_KEY_MAP      3
+   
+   206        2366 BUILD_LIST               0
+              2368 LOAD_CONST              60 ((0.25, 0.25, 0.25))
+              2370 LIST_EXTEND              1
+              2372 LOAD_CONST              61 (-55)
+              2374 BUILD_LIST               0
+              2376 LOAD_CONST              62 ((-1, -1, -1))
+              2378 LIST_EXTEND              1
+              2380 LOAD_CONST              59 (('position', 'angle', 'align_v'))
+              2382 BUILD_CONST_KEY_MAP      3
+   
+   204        2384 BUILD_LIST               2
+   
+   208        2386 BUILD_LIST               0
+   
+   194        2388 LOAD_CONST              63 (('a', 'b', 'c', 'alpha', 'beta', 'gamma', 'lattice', 'vertice_connectivity', 'edge_connectivity', 'vertices', 'edges'))
+              2390 BUILD_CONST_KEY_MAP     11
+   
+   211        2392 LOAD_CONST              19 (1)
+   
+   212        2394 LOAD_CONST              19 (1)
+   
+   213        2396 LOAD_CONST              19 (1)
+   
+   214        2398 LOAD_CONST              53 (60)
+   
+   215        2400 LOAD_CONST              53 (60)
+   
+   216        2402 LOAD_CONST              53 (60)
+   
+   217        2404 BUILD_LIST               0
+              2406 LOAD_CONST              54 ((0, 1, 1))
+              2408 LIST_EXTEND              1
+              2410 BUILD_LIST               0
+              2412 LOAD_CONST              55 ((1, 0, 1))
+              2414 LIST_EXTEND              1
+              2416 BUILD_LIST               0
+              2418 LOAD_CONST              56 ((1, 1, 0))
+              2420 LIST_EXTEND              1
+              2422 BUILD_LIST               3
+   
+   218        2424 LOAD_CONST              20 (4)
+   
+   219        2426 LOAD_CONST               3 (2)
+   
+   221        2428 BUILD_LIST               0
+              2430 LOAD_CONST               9 ((0, 0, 0))
+              2432 LIST_EXTEND              1
+              2434 LOAD_CONST              64 (-7.5)
+              2436 BUILD_LIST               0
+              2438 LOAD_CONST              58 ((1, 1, 1))
+              2440 LIST_EXTEND              1
+              2442 LOAD_CONST              59 (('position', 'angle', 'align_v'))
+              2444 BUILD_CONST_KEY_MAP      3
+   
+   222        2446 BUILD_LIST               0
+              2448 LOAD_CONST              60 ((0.25, 0.25, 0.25))
+              2450 LIST_EXTEND              1
+              2452 LOAD_CONST              65 (7.5)
+              2454 BUILD_LIST               0
+              2456 LOAD_CONST              62 ((-1, -1, -1))
+              2458 LIST_EXTEND              1
+              2460 LOAD_CONST              59 (('position', 'angle', 'align_v'))
+              2462 BUILD_CONST_KEY_MAP      3
    
-   202        2480 LOAD_CONST              19 (4)
+   220        2464 BUILD_LIST               2
    
-   203        2482 LOAD_CONST              19 (4)
+   225        2466 BUILD_LIST               0
+              2468 LOAD_CONST              66 ((0.125, 0.125, 0.125))
+              2470 LIST_EXTEND              1
+              2472 LOAD_CONST              67 (-8.8)
+              2474 BUILD_LIST               0
+              2476 LOAD_CONST              58 ((1, 1, 1))
+              2478 LIST_EXTEND              1
+              2480 LOAD_CONST              59 (('position', 'angle', 'align_v'))
+              2482 BUILD_CONST_KEY_MAP      3
    
-   205        2484 BUILD_LIST               0
-              2486 LOAD_CONST               9 ((0, 0, 0))
+   226        2484 BUILD_LIST               0
+              2486 LOAD_CONST              68 ((0.125, 0.375, 0.375))
               2488 LIST_EXTEND              1
-              2490 LOAD_CONST              57 (55)
+              2490 LOAD_CONST              69 (16)
               2492 BUILD_LIST               0
-              2494 LOAD_CONST              58 ((1, 1, 1))
+              2494 LOAD_CONST              70 ((-0.25, 0.25, 0.25))
               2496 LIST_EXTEND              1
               2498 LOAD_CONST              59 (('position', 'angle', 'align_v'))
               2500 BUILD_CONST_KEY_MAP      3
    
-   206        2502 BUILD_LIST               0
-              2504 LOAD_CONST              60 ((0.25, 0.25, 0.25))
+   227        2502 BUILD_LIST               0
+              2504 LOAD_CONST              71 ((0.375, 0.125, 0.375))
               2506 LIST_EXTEND              1
-              2508 LOAD_CONST              61 (-55)
+              2508 LOAD_CONST              72 (-78)
               2510 BUILD_LIST               0
-              2512 LOAD_CONST              62 ((-1, -1, -1))
+              2512 LOAD_CONST              73 ((0.25, -0.25, 0.25))
               2514 LIST_EXTEND              1
               2516 LOAD_CONST              59 (('position', 'angle', 'align_v'))
               2518 BUILD_CONST_KEY_MAP      3
    
-   204        2520 BUILD_LIST               2
-   
-   208        2522 BUILD_LIST               0
+   228        2520 BUILD_LIST               0
+              2522 LOAD_CONST              74 ((0.375, 0.375, 0.125))
+              2524 LIST_EXTEND              1
+              2526 LOAD_CONST              69 (16)
+              2528 BUILD_LIST               0
+              2530 LOAD_CONST              75 ((0.25, 0.25, -0.25))
+              2532 LIST_EXTEND              1
+              2534 LOAD_CONST              59 (('position', 'angle', 'align_v'))
+              2536 BUILD_CONST_KEY_MAP      3
+   
+   224        2538 BUILD_LIST               4
+   
+   210        2540 LOAD_CONST              63 (('a', 'b', 'c', 'alpha', 'beta', 'gamma', 'lattice', 'vertice_connectivity', 'edge_connectivity', 'vertices', 'edges'))
+              2542 BUILD_CONST_KEY_MAP     11
+   
+   232        2544 LOAD_CONST              19 (1)
+   
+   233        2546 LOAD_CONST              19 (1)
+   
+   234        2548 LOAD_CONST              19 (1)
+   
+   235        2550 LOAD_CONST               6 (90)
+   
+   236        2552 LOAD_CONST               6 (90)
+   
+   237        2554 LOAD_CONST               6 (90)
+   
+   238        2556 BUILD_LIST               0
+              2558 LOAD_CONST              76 ((1, 0, 0))
+              2560 LIST_EXTEND              1
+              2562 BUILD_LIST               0
+              2564 LOAD_CONST              77 ((0, 1, 0))
+              2566 LIST_EXTEND              1
+              2568 BUILD_LIST               0
+              2570 LOAD_CONST              78 ((0, 0, 1))
+              2572 LIST_EXTEND              1
+              2574 BUILD_LIST               3
+   
+   239        2576 LOAD_CONST              20 (4)
+   
+   240        2578 LOAD_CONST               8 (3)
+   
+   242        2580 BUILD_LIST               0
+              2582 LOAD_CONST              33 ((0.5, 0, 0))
+              2584 LIST_EXTEND              1
+              2586 LOAD_CONST              79 (-10)
+              2588 BUILD_LIST               0
+              2590 LOAD_CONST              80 ((-1, 1, 1))
+              2592 LIST_EXTEND              1
+              2594 LOAD_CONST              59 (('position', 'angle', 'align_v'))
+              2596 BUILD_CONST_KEY_MAP      3
+   
+   243        2598 BUILD_LIST               0
+              2600 LOAD_CONST              81 ((0, 0.5, 0))
+              2602 LIST_EXTEND              1
+              2604 LOAD_CONST              82 (40)
+              2606 BUILD_LIST               0
+              2608 LOAD_CONST              83 ((1, -1, 1))
+              2610 LIST_EXTEND              1
+              2612 LOAD_CONST              59 (('position', 'angle', 'align_v'))
+              2614 BUILD_CONST_KEY_MAP      3
+   
+   244        2616 BUILD_LIST               0
+              2618 LOAD_CONST              84 ((0, 0, 0.5))
+              2620 LIST_EXTEND              1
+              2622 LOAD_CONST              23 (-45)
+              2624 BUILD_LIST               0
+              2626 LOAD_CONST              85 ((1, 1, -1))
+              2628 LIST_EXTEND              1
+              2630 LOAD_CONST              59 (('position', 'angle', 'align_v'))
+              2632 BUILD_CONST_KEY_MAP      3
+   
+   241        2634 BUILD_LIST               3
+   
+   247        2636 BUILD_LIST               0
+              2638 LOAD_CONST              86 ((0.16666666666666666, 0.16666666666666666, 0.16666666666666666))
+              2640 LIST_EXTEND              1
+              2642 LOAD_CONST               4 (30)
+              2644 BUILD_LIST               0
+              2646 LOAD_CONST              58 ((1, 1, 1))
+              2648 LIST_EXTEND              1
+              2650 LOAD_CONST              59 (('position', 'angle', 'align_v'))
+              2652 BUILD_CONST_KEY_MAP      3
+   
+   248        2654 BUILD_LIST               0
+              2656 LOAD_CONST              87 ((0.16666666666666666, 0.8333333333333334, 0.8333333333333334))
+              2658 LIST_EXTEND              1
+              2660 LOAD_CONST               1 (0)
+              2662 BUILD_LIST               0
+              2664 LOAD_CONST              88 ((0.5, 1, 1))
+              2666 LIST_EXTEND              1
+              2668 LOAD_CONST              59 (('position', 'angle', 'align_v'))
+              2670 BUILD_CONST_KEY_MAP      3
+   
+   249        2672 BUILD_LIST               0
+              2674 LOAD_CONST              89 ((0.8333333333333334, 0.16666666666666666, 0.8333333333333334))
+              2676 LIST_EXTEND              1
+              2678 LOAD_CONST               1 (0)
+              2680 BUILD_LIST               0
+              2682 LOAD_CONST              90 ((1, 0.5, 1))
+              2684 LIST_EXTEND              1
+              2686 LOAD_CONST              59 (('position', 'angle', 'align_v'))
+              2688 BUILD_CONST_KEY_MAP      3
+   
+   250        2690 BUILD_LIST               0
+              2692 LOAD_CONST              91 ((0.8333333333333334, 0.8333333333333334, 0.16666666666666666))
+              2694 LIST_EXTEND              1
+              2696 LOAD_CONST              92 (10)
+              2698 BUILD_LIST               0
+              2700 LOAD_CONST              58 ((1, 1, 1))
+              2702 LIST_EXTEND              1
+              2704 LOAD_CONST              59 (('position', 'angle', 'align_v'))
+              2706 BUILD_CONST_KEY_MAP      3
    
-   194        2524 LOAD_CONST              63 (('a', 'b', 'c', 'alpha', 'beta', 'gamma', 'lattice', 'vertice_connectivity', 'edge_connectivity', 'vertices', 'edges'))
-              2526 BUILD_CONST_KEY_MAP     11
+   246        2708 BUILD_LIST               4
    
-   211        2528 LOAD_CONST              40 (1)
+   231        2710 LOAD_CONST              63 (('a', 'b', 'c', 'alpha', 'beta', 'gamma', 'lattice', 'vertice_connectivity', 'edge_connectivity', 'vertices', 'edges'))
+              2712 BUILD_CONST_KEY_MAP     11
    
-   212        2530 LOAD_CONST              40 (1)
-   
-   213        2532 LOAD_CONST              40 (1)
-   
-   214        2534 LOAD_CONST              53 (60)
-   
-   215        2536 LOAD_CONST              53 (60)
-   
-   216        2538 LOAD_CONST              53 (60)
-   
-   217        2540 BUILD_LIST               0
-              2542 LOAD_CONST              54 ((0, 1, 1))
-              2544 LIST_EXTEND              1
-              2546 BUILD_LIST               0
-              2548 LOAD_CONST              55 ((1, 0, 1))
-              2550 LIST_EXTEND              1
-              2552 BUILD_LIST               0
-              2554 LOAD_CONST              56 ((1, 1, 0))
-              2556 LIST_EXTEND              1
-              2558 BUILD_LIST               3
-   
-   218        2560 LOAD_CONST              19 (4)
-   
-   219        2562 LOAD_CONST               3 (2)
-   
-   221        2564 BUILD_LIST               0
-              2566 LOAD_CONST               9 ((0, 0, 0))
-              2568 LIST_EXTEND              1
-              2570 LOAD_CONST              64 (-7.5)
-              2572 BUILD_LIST               0
-              2574 LOAD_CONST              58 ((1, 1, 1))
-              2576 LIST_EXTEND              1
-              2578 LOAD_CONST              59 (('position', 'angle', 'align_v'))
-              2580 BUILD_CONST_KEY_MAP      3
-   
-   222        2582 BUILD_LIST               0
-              2584 LOAD_CONST              60 ((0.25, 0.25, 0.25))
-              2586 LIST_EXTEND              1
-              2588 LOAD_CONST              65 (7.5)
-              2590 BUILD_LIST               0
-              2592 LOAD_CONST              62 ((-1, -1, -1))
-              2594 LIST_EXTEND              1
-              2596 LOAD_CONST              59 (('position', 'angle', 'align_v'))
-              2598 BUILD_CONST_KEY_MAP      3
-   
-   220        2600 BUILD_LIST               2
-   
-   225        2602 BUILD_LIST               0
-              2604 LOAD_CONST              66 ((0.125, 0.125, 0.125))
-              2606 LIST_EXTEND              1
-              2608 LOAD_CONST              67 (-8.8)
-              2610 BUILD_LIST               0
-              2612 LOAD_CONST              58 ((1, 1, 1))
-              2614 LIST_EXTEND              1
-              2616 LOAD_CONST              59 (('position', 'angle', 'align_v'))
-              2618 BUILD_CONST_KEY_MAP      3
-   
-   226        2620 BUILD_LIST               0
-              2622 LOAD_CONST              68 ((0.125, 0.375, 0.375))
-              2624 LIST_EXTEND              1
-              2626 LOAD_CONST              69 (16)
-              2628 BUILD_LIST               0
-              2630 LOAD_CONST              70 ((-0.25, 0.25, 0.25))
-              2632 LIST_EXTEND              1
-              2634 LOAD_CONST              59 (('position', 'angle', 'align_v'))
-              2636 BUILD_CONST_KEY_MAP      3
-   
-   227        2638 BUILD_LIST               0
-              2640 LOAD_CONST              71 ((0.375, 0.125, 0.375))
-              2642 LIST_EXTEND              1
-              2644 LOAD_CONST              72 (-78)
-              2646 BUILD_LIST               0
-              2648 LOAD_CONST              73 ((0.25, -0.25, 0.25))
-              2650 LIST_EXTEND              1
-              2652 LOAD_CONST              59 (('position', 'angle', 'align_v'))
-              2654 BUILD_CONST_KEY_MAP      3
-   
-   228        2656 BUILD_LIST               0
-              2658 LOAD_CONST              74 ((0.375, 0.375, 0.125))
-              2660 LIST_EXTEND              1
-              2662 LOAD_CONST              69 (16)
-              2664 BUILD_LIST               0
-              2666 LOAD_CONST              75 ((0.25, 0.25, -0.25))
-              2668 LIST_EXTEND              1
-              2670 LOAD_CONST              59 (('position', 'angle', 'align_v'))
-              2672 BUILD_CONST_KEY_MAP      3
-   
-   224        2674 BUILD_LIST               4
-   
-   210        2676 LOAD_CONST              63 (('a', 'b', 'c', 'alpha', 'beta', 'gamma', 'lattice', 'vertice_connectivity', 'edge_connectivity', 'vertices', 'edges'))
-              2678 BUILD_CONST_KEY_MAP     11
-   
-   232        2680 LOAD_CONST              40 (1)
-   
-   233        2682 LOAD_CONST              40 (1)
-   
-   234        2684 LOAD_CONST              40 (1)
-   
-   235        2686 LOAD_CONST               6 (90)
-   
-   236        2688 LOAD_CONST               6 (90)
-   
-   237        2690 LOAD_CONST               6 (90)
-   
-   238        2692 BUILD_LIST               0
-              2694 LOAD_CONST              76 ((1, 0, 0))
-              2696 LIST_EXTEND              1
-              2698 BUILD_LIST               0
-              2700 LOAD_CONST              77 ((0, 1, 0))
-              2702 LIST_EXTEND              1
-              2704 BUILD_LIST               0
-              2706 LOAD_CONST              78 ((0, 0, 1))
-              2708 LIST_EXTEND              1
-              2710 BUILD_LIST               3
-   
-   239        2712 LOAD_CONST              19 (4)
-   
-   240        2714 LOAD_CONST               8 (3)
-   
-   242        2716 BUILD_LIST               0
-              2718 LOAD_CONST              32 ((0.5, 0, 0))
-              2720 LIST_EXTEND              1
-              2722 LOAD_CONST              79 (-10)
-              2724 BUILD_LIST               0
-              2726 LOAD_CONST              80 ((-1, 1, 1))
-              2728 LIST_EXTEND              1
-              2730 LOAD_CONST              59 (('position', 'angle', 'align_v'))
-              2732 BUILD_CONST_KEY_MAP      3
-   
-   243        2734 BUILD_LIST               0
-              2736 LOAD_CONST              81 ((0, 0.5, 0))
-              2738 LIST_EXTEND              1
-              2740 LOAD_CONST              82 (40)
-              2742 BUILD_LIST               0
-              2744 LOAD_CONST              83 ((1, -1, 1))
-              2746 LIST_EXTEND              1
-              2748 LOAD_CONST              59 (('position', 'angle', 'align_v'))
-              2750 BUILD_CONST_KEY_MAP      3
-   
-   244        2752 BUILD_LIST               0
-              2754 LOAD_CONST              84 ((0, 0, 0.5))
-              2756 LIST_EXTEND              1
-              2758 LOAD_CONST              22 (-45)
-              2760 BUILD_LIST               0
-              2762 LOAD_CONST              85 ((1, 1, -1))
-              2764 LIST_EXTEND              1
-              2766 LOAD_CONST              59 (('position', 'angle', 'align_v'))
-              2768 BUILD_CONST_KEY_MAP      3
-   
-   241        2770 BUILD_LIST               3
-   
-   247        2772 BUILD_LIST               0
-              2774 LOAD_CONST              86 ((0.16666666666666666, 0.16666666666666666, 0.16666666666666666))
-              2776 LIST_EXTEND              1
-              2778 LOAD_CONST               4 (30)
-              2780 BUILD_LIST               0
-              2782 LOAD_CONST              58 ((1, 1, 1))
-              2784 LIST_EXTEND              1
-              2786 LOAD_CONST              59 (('position', 'angle', 'align_v'))
-              2788 BUILD_CONST_KEY_MAP      3
-   
-   248        2790 BUILD_LIST               0
-              2792 LOAD_CONST              87 ((0.16666666666666666, 0.8333333333333334, 0.8333333333333334))
-              2794 LIST_EXTEND              1
-              2796 LOAD_CONST               1 (0)
-              2798 BUILD_LIST               0
-              2800 LOAD_CONST              88 ((0.5, 1, 1))
-              2802 LIST_EXTEND              1
-              2804 LOAD_CONST              59 (('position', 'angle', 'align_v'))
-              2806 BUILD_CONST_KEY_MAP      3
-   
-   249        2808 BUILD_LIST               0
-              2810 LOAD_CONST              89 ((0.8333333333333334, 0.16666666666666666, 0.8333333333333334))
-              2812 LIST_EXTEND              1
-              2814 LOAD_CONST               1 (0)
-              2816 BUILD_LIST               0
-              2818 LOAD_CONST              90 ((1, 0.5, 1))
-              2820 LIST_EXTEND              1
-              2822 LOAD_CONST              59 (('position', 'angle', 'align_v'))
-              2824 BUILD_CONST_KEY_MAP      3
-   
-   250        2826 BUILD_LIST               0
-              2828 LOAD_CONST              91 ((0.8333333333333334, 0.8333333333333334, 0.16666666666666666))
-              2830 LIST_EXTEND              1
-              2832 LOAD_CONST              92 (10)
-              2834 BUILD_LIST               0
-              2836 LOAD_CONST              58 ((1, 1, 1))
-              2838 LIST_EXTEND              1
-              2840 LOAD_CONST              59 (('position', 'angle', 'align_v'))
-              2842 BUILD_CONST_KEY_MAP      3
-   
-   246        2844 BUILD_LIST               4
-   
-   231        2846 LOAD_CONST              63 (('a', 'b', 'c', 'alpha', 'beta', 'gamma', 'lattice', 'vertice_connectivity', 'edge_connectivity', 'vertices', 'edges'))
-              2848 BUILD_CONST_KEY_MAP     11
-   
-    11        2850 LOAD_CONST              93 (('HCB', 'HCB_A', 'SQL', 'SQL_A', 'KGD', 'HXL_A', 'KGM', 'KGM_A', 'FXT', 'FXT_A', 'DIA', 'DIA_A', 'BOR'))
-              2852 BUILD_CONST_KEY_MAP     13
-              2854 STORE_NAME               6 (TOPOLOGY_DICT)
-              2856 LOAD_CONST               2 (None)
-              2858 RETURN_VALUE
+    11        2714 LOAD_CONST              93 (('HCB', 'HCB_A', 'SQL', 'SQL_A', 'KGD', 'HXL_A', 'KGM', 'KGM_A', 'FXT', 'FXT_A', 'DIA', 'DIA_A', 'BOR'))
+              2716 BUILD_CONST_KEY_MAP     13
+              2718 STORE_NAME               6 (TOPOLOGY_DICT)
+              2720 LOAD_CONST               2 (None)
+              2722 RETURN_VALUE
    consts
       '\nThe dictionary containing the definitions nets for a Framework buiding\n'
       0
       None
       2
       30
       3.6
@@ -1300,14 +1267,15 @@
       ('a', 'b', 'c', 'alpha', 'beta', 'gamma', 'vertice_connectivity', 'edge_connectivity', 'vertices', 'edges')
       6
       -0.25
       5
       12
       0.25
       240
+      1
       4
       45
       (0.5, 0.5, 0)
       -45
       (0.25, 0.25, 0)
       (0.75, 0.25, 0)
       135
@@ -1321,15 +1289,14 @@
       -30
       -90
       0.375
       8
       0.125
       0.625
       -0.125
-      1
       -15
       15
       0.34375
       7
       64
       0.6640625
       35
@@ -1385,16 +1352,16 @@
    cellvars   ()
    filename   '/home/felipe/Github/pyCOFBuilder/src/pycofbuilder/data/topology.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020504040804400140010201020102010201020102020c0130fe02
       0402f30410460146010201020102010201020102020c0130fe0205300136
-      0136fd02f30414240124010201020102010201020102020c010cfe020402
-      f30410240124010201020102010201020102020c010cfe02050c010c010c
+      0136fd02f30414020102010201020102010201020102020c010cfe020402
+      f30410020102010201020102010201020102020c010cfe02050c010c010c
       010cfc02f30415400140010201020102010201020102020cff0204300130
       fe02f40412020102010201020102010201020102020cff020430010c0130
       fd02f404130201020102010201020102010201020230010c0130fd020502
       f204110201020102010201020102010201020230010c0130fd0206300136
       0130013001300130fa02f204180201020102010201020102010201020236
       010c0136fd020502f204110201020102010201020102010201020236010c
       0136fd02063601360136013601360136fa02f20418020102010201020102
```

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/BOH2.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/BOH2.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/Br.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/Br.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/CH2CN.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/CH2CN.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/CH3.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/CH3.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/CHNNH2.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/CHNNH2.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/CHO.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/CHO.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/COCHCHOH.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/COCHCHOH.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/CONHNH2.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/CONHNH2.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/COOH.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/COOH.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/Cl.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/Cl.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/NH2.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/NH2.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/NHOH.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/NHOH.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/O.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/O.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/conector/OH2.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/OH2.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/D4/ADAM.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/ADAM.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/D4/SBFE.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/SBFE.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/D4/TDAT.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/TDAT.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/D4/TKAT.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/TKAT.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/D4/TKDM.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/TKDM.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/D4/TTPM.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/TTPM.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/H6/HECO.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/H6/HECO.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/H6/HEXB.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/H6/HEXB.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/H6/HPCO.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/H6/HPCO.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/2BPD.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/2BPD.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/3BPD.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/3BPD.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/3IDT.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/3IDT.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/4IDT.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/4IDT.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/ANTR.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/ANTR.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/BBTZ.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BBTZ.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/BDFN.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BDFN.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/BDTP.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BDTP.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/BENZ.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BENZ.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/BPNY.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BPNY.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/BPYB.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BPYB.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/BTPH.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BTPH.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/DFFE.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DFFE.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/DHPI.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DHPI.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/DHSI.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DHSI.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/DPBY.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DPBY.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/DPDA.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DPDA.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/DPEL.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DPEL.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/DPEY.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DPEY.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/HDZN.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/HDZN.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/IITT.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/IITT.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/INDE.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/INDE.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/INFL.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/INFL.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/INTO.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/INTO.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/NAPT.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/NAPT.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/NDTP.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/NDTP.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/PHEN.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/PHEN.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/PTCD.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/PTCD.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/PYEN.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/PYEN.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/PYRN.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/PYRN.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/PYTO.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/PYTO.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/TIDA.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/TIDA.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/TIEN.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/TIEN.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/TPDI.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/TPDI.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/TPNY.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/TPNY.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/L2/TTPH.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/TTPH.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/S4/CoBTC.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/CoBTC.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/S4/CuBTC.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/CuBTC.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/S4/NiBTC.gjf` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/NiBTC.gjf`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/S4/PHPR.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/PHPR.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/S4/PORP.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/PORP.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/S4/PTCA.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/PTCA.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/S4/ZnBTC.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/ZnBTC.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/BENZ.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/BENZ.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/BRZN.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/BRZN.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/BTTP.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/BTTP.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/DBA1.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/DBA1.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/DBA2.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/DBA2.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/DICZ.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/DICZ.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/STAR.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/STAR.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/STAR1.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/STAR1.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/TBBZ.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TBBZ.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/TOTB.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TOTB.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/TPAM.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TPAM.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/TPBZ.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TPBZ.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/TPNY.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TPNY.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/TPOB.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TPOB.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/TPTA.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TPTA.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/TPTZ.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TPTZ.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/core/T3/TRZN.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TRZN.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/Br.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/Br.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/CF3.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/CF3.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/CH3.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/CH3.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/CHO.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/CHO.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/CHS.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/CHS.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/CN.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/CN.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/COOH.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/COOH.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/Cl.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/Cl.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/DMPE.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/DMPE.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/EEPO.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/EEPO.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/EMEPO.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/EMEPO.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/EPO.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/EPO.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/F.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/F.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/H.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/H.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/I.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/I.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/MEPO.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/MEPO.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/NH2.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/NH2.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/NO.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/NO.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/NO2.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/NO2.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/O.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/O.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/OCOCH3.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/OCOCH3.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/OEEPO.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/OEEPO.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/OEt.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/OEt.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/OH.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/OH.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/OMe.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/OMe.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/OProp.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/OProp.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/Ph.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/Ph.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/SH.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/SH.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/SO2H.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/SO2H.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/SO3H.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/SO3H.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/func_groups/tBu.cjson` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/tBu.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/periodic_table.json` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/periodic_table.json`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/data/topology.py` & `pycofbuilder-0.0.8.3/src/pycofbuilder/data/topology.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,31 +40,31 @@
         'edges': [
             {'position': [0, np.sqrt(3)/6, 0], 'angle': 0},
             {'position': [-1/4, 5*np.sqrt(3)/12, 0], 'angle': 120},
             {'position': [1/4, 5*np.sqrt(3)/12, 0], 'angle': 240}
             ]
         },
     'SQL': {
-        'a': 2/np.sqrt(2),
-        'b': 2/np.sqrt(2),
+        'a': 1,
+        'b': 1,
         'c': 3.6,
         'alpha': 90,
         'beta': 90,
         'gamma': 90,
         'vertice_connectivity': 4,
         'edge_connectivity': 0,
         'vertices': [
             {'position': [0, 0, 0], 'angle': 45},
             {'position': [1/2, 1/2, 0], 'angle': 45}
             ],
         'edges': []
         },
     'SQL_A': {
-        'a': 4/np.sqrt(2),
-        'b': 4/np.sqrt(2),
+        'a': 1,
+        'b': 1,
         'c': 3.6,
         'alpha': 90,
         'beta': 90,
         'gamma': 90,
         'vertice_connectivity': 4,
         'edge_connectivity': 2,
         'vertices': [
```

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/exceptions.py` & `pycofbuilder-0.0.8.3/src/pycofbuilder/exceptions.py`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/framework.py` & `pycofbuilder-0.0.8.3/src/pycofbuilder/framework.py`

 * *Files 2% similar despite different names*

```diff
@@ -378,15 +378,15 @@
             site_properties={'source': self.atom_labels}
         )
 
         self.bonds = get_bonds(structure, self.bond_threshold)
 
         return result
 
-    def save(self, 
+    def save(self,
              fmt: str = 'cif',
              supercell: list = [1, 1, 1],
              save_dir=None,
              primitive=False,
              save_bonds=True) -> None:
         '''
         Save the structure in a specif file format.
@@ -1281,16 +1281,16 @@
                 str(self.lattice_type),
                 str(self.hall[0:2]),
                 str(self.space_group),
                 str(self.space_group_n),
                 len(symm_op)]
 
     def create_sql_structure(self,
-                             BB_S4_A: str,
-                             BB_S4_B: str,
+                             BB_A: str,
+                             BB_B: str,
                              stacking: str = 'AA',
                              slab: float = 10.0,
                              shift_vector: list = [1.0, 1.0, 0],
                              tilt_angle: float = 5.0):
         """Creates a COF with SQL network.
 
         The SQL net is composed of two tetrapodal building blocks.
@@ -1321,60 +1321,69 @@
                 3. hall symbol of the cristaline structure,
                 4. space group,
                 5. number of the space group,
                 6. number of operation symmetry
         """
 
         connectivity_error = 'Building block {} must present connectivity {} not {}'
-        if BB_S4_A.connectivity != 4:
-            self.logger.error(connectivity_error.format('A', 4, BB_S4_A.connectivity))
-            raise BBConnectivityError(4, BB_S4_A.connectivity)
-        if BB_S4_B.connectivity != 4:
-            self.logger.error(connectivity_error.format('B', 4, BB_S4_B.connectivity))
-            raise BBConnectivityError(4, BB_S4_B.connectivity)
+        if BB_A.connectivity != 4:
+            self.logger.error(connectivity_error.format('A', 4, BB_A.connectivity))
+            raise BBConnectivityError(4, BB_A.connectivity)
+        if BB_B.connectivity != 4:
+            self.logger.error(connectivity_error.format('B', 4, BB_B.connectivity))
+            raise BBConnectivityError(4, BB_B.connectivity)
 
-        self.name = f'{BB_S4_A.name}-{BB_S4_B.name}-SQL-{stacking}'
+        self.name = f'{BB_A.name}-{BB_B.name}-SQL-{stacking}'
         self.topology = 'SQL'
         self.staking = stacking
         self.dimension = 2
 
-        self.charge = BB_S4_A.charge + BB_S4_B.charge
-        self.chirality = BB_S4_A.chirality or BB_S4_B.chirality
+        self.charge = BB_A.charge + BB_B.charge
+        self.chirality = BB_A.chirality or BB_B.chirality
 
         self.logger.debug(f'Starting the creation of {self.name}')
 
+        # Get the positions of the "X" atoms
+        _, X_A = BB_A.get_X_points()
+        _, X_B = BB_B.get_X_points()
+
+        # Calculate the alpha angle for the rotation of the building blocks
+        alpha_A = -np.arctan2(X_A[0][1] - X_A[-1][1], X_A[0][0] - X_A[-1][0])
+        alpha_B = -np.arctan2(X_B[0][1] - X_B[-1][1], X_B[0][0] - X_B[-1][0])
+
         # Detect the bond atom from the connection groups type
-        bond_atom = get_bond_atom(BB_S4_A.conector, BB_S4_B.conector)
+        bond_atom = get_bond_atom(BB_A.conector, BB_B.conector)
 
         self.logger.debug('{} detected as bond atom for groups {} and {}'.format(bond_atom,
-                                                                                 BB_S4_A.conector,
-                                                                                 BB_S4_B.conector))
+                                                                                 BB_A.conector,
+                                                                                 BB_B.conector))
 
         # Replace "X" the building block
-        BB_S4_A.replace_X(bond_atom)
+        BB_A.replace_X(bond_atom)
 
         # Remove the "X" atoms from the the building block
-        BB_S4_A.remove_X()
-        BB_S4_B.remove_X()
+        BB_A.remove_X()
+        BB_B.remove_X()
 
         # Get the topology information
         topology_info = TOPOLOGY_DICT[self.topology]
 
         # Measure the base size of the building blocks
-        size = BB_S4_A.size[0] + BB_S4_B.size[0]
+        size_A = (np.abs(BB_A.size[0] * np.sin(alpha_A)) + np.abs(BB_B.size[0] * np.cos(alpha_B))) * 2
+        size_B = (np.abs(BB_A.size[0] * np.cos(alpha_A)) + np.abs(BB_B.size[0] * np.cos(alpha_B))) * 2
 
         # Calculate the delta size to add to the c parameter
-        delta_a = abs(max(np.transpose(BB_S4_A.atom_pos)[2])) + abs(min(np.transpose(BB_S4_B.atom_pos)[2]))
-        delta_b = abs(max(np.transpose(BB_S4_A.atom_pos)[2])) + abs(min(np.transpose(BB_S4_B.atom_pos)[2]))
+        delta_a = abs(max(np.transpose(BB_A.atom_pos)[2])) + abs(min(np.transpose(BB_B.atom_pos)[2]))
+        delta_b = abs(max(np.transpose(BB_A.atom_pos)[2])) + abs(min(np.transpose(BB_B.atom_pos)[2]))
 
         delta_max = max([delta_a, delta_b])
 
         # Calculate the cell parameters
-        a = topology_info['a'] * size
-        b = topology_info['b'] * size
+        a = topology_info['a'] * size_A
+        b = topology_info['b'] * size_B
         c = topology_info['c'] + delta_max
         alpha = topology_info['alpha']
         beta = topology_info['beta']
         gamma = topology_info['gamma']
 
         if self.stacking == 'A':
             c = slab
@@ -1385,36 +1394,34 @@
 
         # Create the structure
         self.atom_types = []
         self.atom_labels = []
         self.atom_pos = []
 
         # Add the first building block to the structure
-        vertice_data = topology_info['vertices'][0]
-        self.atom_types += BB_S4_A.atom_types
-        vertice_pos = np.array(vertice_data['position'])*a
+        self.atom_types += BB_A.atom_types
+        vertice_pos = np.array([0, 0, 0])
 
-        R_Matrix = R.from_euler('z', vertice_data['angle'], degrees=True).as_matrix()
+        R_Matrix = R.from_euler('z', -alpha_A, degrees=False).as_matrix()
 
-        rotated_pos = np.dot(BB_S4_A.atom_pos, R_Matrix) + vertice_pos
+        rotated_pos = np.dot(BB_A.atom_pos, R_Matrix)
         self.atom_pos += rotated_pos.tolist()
 
-        self.atom_labels += ['C1' if i == 'C' else i for i in BB_S4_A.atom_labels]
+        self.atom_labels += ['C1' if i == 'C' else i for i in BB_A.atom_labels]
 
         # Add the second building block to the structure
-        vertice_data = topology_info['vertices'][1]
-        self.atom_types += BB_S4_B.atom_types
-        vertice_pos = np.array(vertice_data['position'])*a
+        self.atom_types += BB_B.atom_types
+        vertice_pos = np.array([a/2, b/2, 0])
 
-        R_Matrix = R.from_euler('z', vertice_data['angle'], degrees=True).as_matrix()
+        R_Matrix = R.from_euler('z', -alpha_B, degrees=False).as_matrix()
 
-        rotated_pos = np.dot(BB_S4_B.atom_pos, R_Matrix) + vertice_pos
+        rotated_pos = np.dot(BB_B.atom_pos, R_Matrix) + vertice_pos
         self.atom_pos += rotated_pos.tolist()
 
-        self.atom_labels += ['C2' if i == 'C' else i for i in BB_S4_B.atom_labels]
+        self.atom_labels += ['C2' if i == 'C' else i for i in BB_B.atom_labels]
 
         StartingFramework = Structure(
             self.cellMatrix,
             self.atom_types,
             self.atom_pos,
             coords_are_cartesian=True,
             site_properties={'source': self.atom_labels}
@@ -1748,14 +1755,20 @@
         self.dimension = 2
 
         self.charge = BB_S4.charge + BB_L2.charge
         self.chirality = BB_S4.chirality or BB_L2.chirality
 
         self.logger.debug(f'Starting the creation of {self.name}')
 
+        # Get the position of the "X" atoms
+        _, X_S4 = BB_S4.get_X_points()
+
+        # Calculate the alpha angle for the rotation of the building blocks
+        alpha_S4 = -np.arctan2(X_S4[0][1] - X_S4[-1][1], X_S4[0][0] - X_S4[-1][0])
+
         # Detect the bond atom from the connection groups type
         bond_atom = get_bond_atom(BB_S4.conector, BB_L2.conector)
 
         self.logger.debug('{} detected as bond atom for groups {} and {}'.format(bond_atom,
                                                                                  BB_S4.conector,
                                                                                  BB_L2.conector))
 
@@ -1766,25 +1779,26 @@
         BB_S4.remove_X()
         BB_L2.remove_X()
 
         # Get the topology information
         topology_info = TOPOLOGY_DICT[self.topology]
 
         # Measure the base size of the building blocks
-        size = BB_S4.size[0] + BB_L2.size[0]
+        size_A = ((BB_S4.size[0] + BB_L2.size[0]) * np.abs(np.sin(alpha_S4))) * 4
+        size_B = ((BB_S4.size[0] + BB_L2.size[0]) * np.abs(np.cos(alpha_S4))) * 4
 
         # Calculate the delta size to add to the c parameter
         delta_a = abs(max(np.transpose(BB_S4.atom_pos)[2])) + abs(min(np.transpose(BB_S4.atom_pos)[2]))
         delta_b = abs(max(np.transpose(BB_L2.atom_pos)[2])) + abs(min(np.transpose(BB_L2.atom_pos)[2]))
 
         delta_max = max([delta_a, delta_b])
 
         # Calculate the cell parameters
-        a = topology_info['a'] * size
-        b = topology_info['b'] * size
+        a = topology_info['a'] * size_A
+        b = topology_info['b'] * size_B
         c = topology_info['c'] + delta_max
         alpha = topology_info['alpha']
         beta = topology_info['beta']
         gamma = topology_info['gamma']
 
         if self.stacking == 'A':
             c = slab
@@ -1797,29 +1811,31 @@
         self.atom_types = []
         self.atom_labels = []
         self.atom_pos = []
 
         # Add the building blocks to the structure
         for vertice_data in topology_info['vertices']:
             self.atom_types += BB_S4.atom_types
-            vertice_pos = np.array(vertice_data['position'])*a
+            vertice_pos = np.array(vertice_data['position']) * np.array([a, b, c])
 
-            R_Matrix = R.from_euler('z', vertice_data['angle'], degrees=True).as_matrix()
+            R_Matrix = R.from_euler('z', -alpha_S4, degrees=False).as_matrix()
 
             rotated_pos = np.dot(BB_S4.atom_pos, R_Matrix) + vertice_pos
             self.atom_pos += rotated_pos.tolist()
 
             self.atom_labels += ['C1' if i == 'C' else i for i in BB_S4.atom_labels]
 
+        L2_angle_list = [-alpha_S4, alpha_S4, -alpha_S4, alpha_S4]
+
         # Add the building blocks to the structure
-        for edge_data in topology_info['edges']:
+        for i, edge_data in enumerate(topology_info['edges']):
             self.atom_types += BB_L2.atom_types
-            edge_pos = np.array(edge_data['position'])*a
+            edge_pos = np.array(edge_data['position']) * np.array([a, b, c])
 
-            R_Matrix = R.from_euler('z', edge_data['angle'], degrees=True).as_matrix()
+            R_Matrix = R.from_euler('z', L2_angle_list[i], degrees=False).as_matrix()
 
             rotated_pos = np.dot(BB_L2.atom_pos, R_Matrix) + edge_pos
             self.atom_pos += rotated_pos.tolist()
 
             self.atom_labels += ['C2' if i == 'C' else i for i in BB_L2.atom_labels]
 
         StartingFramework = Structure(
@@ -2923,31 +2939,31 @@
                 str(self.lattice_type),
                 str(self.hall[0:2]),
                 str(self.space_group),
                 str(self.space_group_n),
                 len(symm_op)]
 
     def create_fxt_structure(self,
-                             BB_S4_A: str,
-                             BB_S4_B: str,
+                             BB_R4_A: str,
+                             BB_R4_B: str,
                              stacking: str = 'AA',
                              print_result: bool = True,
                              slab: float = 10.0,
                              shift_vector: list = [1.0, 1.0, 0],
                              tilt_angle: float = 5.0):
         """Creates a COF with FXT network.
 
         The FXT net is composed of two tetrapodal building blocks.
 
         Parameters
         ----------
-        BB_S4_A : BuildingBlock, required
-            The BuildingBlock object of the tetrapodal Buiding Block A
-        BB_S4_B : BuildingBlock, required
-            The BuildingBlock object of the tetrapodal Buiding Block B
+        BB_R4_A : BuildingBlock, required
+            The BuildingBlock object of the rectangular tetrapodal Buiding Block A
+        BB_R4_B : BuildingBlock, required
+            The BuildingBlock object of the rectangular tetrapodal Buiding Block B
         stacking : str, optional
             The stacking pattern of the COF layers (default is 'AA')
         print_result : bool, optional
             Parameter for the control for printing the result (default is True)
         slab : float, optional
             Default parameter for the interlayer slab (default is 10.0)
         shift_vector: list, optional
@@ -2964,54 +2980,58 @@
                 3. hall symbol of the cristaline structure,
                 4. space group,
                 5. number of the space group,
                 6. number of operation symmetry
         """
 
         connectivity_error = 'Building block {} must present connectivity {} not {}'
-        if BB_S4_A.connectivity != 4:
-            self.logger.error(connectivity_error.format('A', 4, BB_S4_A.connectivity))
-            raise BBConnectivityError(4, BB_S4_A.connectivity)
-        if BB_S4_B.connectivity != 4:
-            self.logger.error(connectivity_error.format('B', 4, BB_S4_B.connectivity))
-            raise BBConnectivityError(4, BB_S4_B.connectivity)
+        if BB_R4_A.connectivity != 4:
+            self.logger.error(connectivity_error.format('A', 4, BB_R4_A.connectivity))
+            raise BBConnectivityError(4, BB_R4_A.connectivity)
+        if BB_R4_B.connectivity != 4:
+            self.logger.error(connectivity_error.format('B', 4, BB_R4_B.connectivity))
+            raise BBConnectivityError(4, BB_R4_B.connectivity)
 
-        self.name = f'{BB_S4_A.name}-{BB_S4_B.name}-FXT-{stacking}'
+        self.name = f'{BB_R4_A.name}-{BB_R4_B.name}-FXT-{stacking}'
         self.topology = 'FXT'
         self.staking = stacking
         self.dimension = 2
 
-        self.charge = BB_S4_A.charge + BB_S4_B.charge
-        self.chirality = BB_S4_A.chirality or BB_S4_B.chirality
+        self.charge = BB_R4_A.charge + BB_R4_B.charge
+        self.chirality = BB_R4_A.chirality or BB_R4_B.chirality
 
         self.logger.debug(f'Starting the creation of {self.name}')
 
         # Detect the bond atom from the connection groups type
-        bond_atom = get_bond_atom(BB_S4_A.conector, BB_S4_B.conector)
+        bond_atom = get_bond_atom(BB_R4_A.conector, BB_R4_B.conector)
 
         self.logger.debug('{} detected as bond atom for groups {} and {}'.format(bond_atom,
-                                                                                 BB_S4_A.conector,
-                                                                                 BB_S4_B.conector))
+                                                                                 BB_R4_A.conector,
+                                                                                 BB_R4_B.conector))
+
+        # Get the position of the X atom in the building blocks
+        BB_R4_A.get_X_points(bond_atom)
+        BB_R4_B.get_X_points(bond_atom)
 
         # Replace "X" the building block
-        BB_S4_A.replace_X(bond_atom)
+        BB_R4_A.replace_X(bond_atom)
 
         # Remove the "X" atoms from the the building block
-        BB_S4_A.remove_X()
-        BB_S4_B.remove_X()
+        BB_R4_A.remove_X()
+        BB_R4_B.remove_X()
 
         # Get the topology information
         topology_info = TOPOLOGY_DICT[self.topology]
 
         # Measure the base size of the building blocks
-        size = 2 * (BB_S4_A.size[0] + BB_S4_B.size[0])
+        size = 2 * (BB_R4_A.size[0] + BB_R4_B.size[0])
 
         # Calculate the delta size to add to the c parameter
-        delta_a = abs(max(np.transpose(BB_S4_A.atom_pos)[2])) + abs(min(np.transpose(BB_S4_B.atom_pos)[2]))
-        delta_b = abs(max(np.transpose(BB_S4_A.atom_pos)[2])) + abs(min(np.transpose(BB_S4_B.atom_pos)[2]))
+        delta_a = abs(max(np.transpose(BB_R4_A.atom_pos)[2])) + abs(min(np.transpose(BB_R4_B.atom_pos)[2]))
+        delta_b = abs(max(np.transpose(BB_R4_A.atom_pos)[2])) + abs(min(np.transpose(BB_R4_B.atom_pos)[2]))
 
         delta_max = max([delta_a, delta_b])
 
         # Calculate the cell parameters
         a = topology_info['a'] * size
         b = topology_info['b'] * size
         c = topology_info['c'] + delta_max
@@ -3029,35 +3049,35 @@
         # Create the structure
         self.atom_types = []
         self.atom_labels = []
         self.atom_pos = []
 
         # Add the first building block to the structure
         vertice_data = topology_info['vertices'][0]
-        self.atom_types += BB_S4_A.atom_types
+        self.atom_types += BB_R4_A.atom_types
         vertice_pos = np.array(vertice_data['position'])*a
 
         R_Matrix = R.from_euler('z', vertice_data['angle'], degrees=True).as_matrix()
 
-        rotated_pos = np.dot(BB_S4_A.atom_pos, R_Matrix) + vertice_pos
+        rotated_pos = np.dot(BB_R4_A.atom_pos, R_Matrix) + vertice_pos
         self.atom_pos += rotated_pos.tolist()
 
-        self.atom_labels += ['C1' if i == 'C' else i for i in BB_S4_A.atom_labels]
+        self.atom_labels += ['C1' if i == 'C' else i for i in BB_R4_A.atom_labels]
 
         # Add the second building block to the structure
         for vertice_data in topology_info['vertices'][1:]:
-            self.atom_types += BB_S4_B.atom_types
+            self.atom_types += BB_R4_B.atom_types
             vertice_pos = np.array(vertice_data['position'])*a
 
             R_Matrix = R.from_euler('z', vertice_data['angle'], degrees=True).as_matrix()
 
-            rotated_pos = np.dot(BB_S4_B.atom_pos, R_Matrix) + vertice_pos
+            rotated_pos = np.dot(BB_R4_B.atom_pos, R_Matrix) + vertice_pos
             self.atom_pos += rotated_pos.tolist()
 
-            self.atom_labels += ['C2' if i == 'C' else i for i in BB_S4_B.atom_labels]
+            self.atom_labels += ['C2' if i == 'C' else i for i in BB_R4_B.atom_labels]
 
         StartingFramework = Structure(
             self.cellMatrix,
             self.atom_types,
             self.atom_pos,
             coords_are_cartesian=True,
             site_properties={'source': self.atom_labels}
```

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/io_tools.py` & `pycofbuilder-0.0.8.3/src/pycofbuilder/io_tools.py`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/logger.py` & `pycofbuilder-0.0.8.3/src/pycofbuilder/logger.py`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder/tools.py` & `pycofbuilder-0.0.8.3/src/pycofbuilder/tools.py`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder.egg-info/PKG-INFO` & `pycofbuilder-0.0.8.3/src/pycofbuilder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycofbuilder
-Version: 0.0.8.2
+Version: 0.0.8.3
 Summary: A package for Covalent Organic Frameworks sturcture creation based on the reticular approach.
 Home-page: https://github.com/lipelopesoliveira/pyCOFBuilder
 Author: Felipe Lopes Oliveira
 Author-email: Felipe Lopes <felipe.lopes@nano.ufrj.br>
 License: MIT License
         
         Copyright (c) 2023, Felipe Lopes de Oliveira
```

### Comparing `pycofbuilder-0.0.8.2/src/pycofbuilder.egg-info/SOURCES.txt` & `pycofbuilder-0.0.8.3/src/pycofbuilder.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 src/pycofbuilder/data/core/L2/BBTZ.cjson
 src/pycofbuilder/data/core/L2/BDFN.cjson
 src/pycofbuilder/data/core/L2/BDTP.cjson
 src/pycofbuilder/data/core/L2/BENZ.cjson
 src/pycofbuilder/data/core/L2/BPNY.cjson
 src/pycofbuilder/data/core/L2/BPYB.cjson
 src/pycofbuilder/data/core/L2/BTPH.cjson
+src/pycofbuilder/data/core/L2/DFDB.cjson
 src/pycofbuilder/data/core/L2/DFFE.cjson
 src/pycofbuilder/data/core/L2/DHPI.cjson
 src/pycofbuilder/data/core/L2/DHSI.cjson
 src/pycofbuilder/data/core/L2/DPBY.cjson
 src/pycofbuilder/data/core/L2/DPDA.cjson
 src/pycofbuilder/data/core/L2/DPEL.cjson
 src/pycofbuilder/data/core/L2/DPEY.cjson
@@ -81,14 +82,15 @@
 src/pycofbuilder/data/core/L2/PYTO.cjson
 src/pycofbuilder/data/core/L2/TIDA.cjson
 src/pycofbuilder/data/core/L2/TIEN.cjson
 src/pycofbuilder/data/core/L2/TPDI.cjson
 src/pycofbuilder/data/core/L2/TPNY.cjson
 src/pycofbuilder/data/core/L2/TTPH.cjson
 src/pycofbuilder/data/core/L2/__init__.py
+src/pycofbuilder/data/core/R4/TPDT.cjson
 src/pycofbuilder/data/core/S4/CoBTC.cjson
 src/pycofbuilder/data/core/S4/CuBTC.cjson
 src/pycofbuilder/data/core/S4/NiBTC.gjf
 src/pycofbuilder/data/core/S4/PHPR.cjson
 src/pycofbuilder/data/core/S4/PORP.cjson
 src/pycofbuilder/data/core/S4/PTCA.cjson
 src/pycofbuilder/data/core/S4/ZnBTC.cjson
```

