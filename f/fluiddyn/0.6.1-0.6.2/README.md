# Comparing `tmp/fluiddyn-0.6.1.tar.gz` & `tmp/fluiddyn-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluiddyn-0.6.1.tar", last modified: Tue Apr  2 13:10:35 2024, max compression
+gzip compressed data, was "fluiddyn-0.6.2.tar", last modified: Tue Apr 16 08:16:57 2024, max compression
```

## Comparing `fluiddyn-0.6.1.tar` & `fluiddyn-0.6.2.tar`

### file list

```diff
@@ -1,119 +1,119 @@
--rw-r--r--   0        0        0      314 2024-02-17 22:43:56.129004 fluiddyn-0.6.1/AUTHORS.md
--rw-r--r--   0        0        0    21394 2024-02-17 22:43:56.129004 fluiddyn-0.6.1/LICENSE.txt
--rw-r--r--   0        0        0     5322 2024-02-17 22:43:56.133004 fluiddyn-0.6.1/README.rst
--rw-r--r--   0        0        0     1136 2024-02-17 22:43:56.161004 fluiddyn-0.6.1/fluiddoc/__init__.py
--rw-r--r--   0        0        0     4408 2024-02-17 22:43:56.161004 fluiddyn-0.6.1/fluiddoc/fluiddocset.py
--rw-r--r--   0        0        0     2344 2024-02-17 22:43:56.161004 fluiddyn-0.6.1/fluiddoc/fluidnbstripout.py
--rw-r--r--   0        0        0     3096 2024-02-17 22:43:56.161004 fluiddyn-0.6.1/fluiddoc/ipynb_maker.py
--rw-r--r--   0        0        0     5174 2024-02-17 22:43:56.161004 fluiddyn-0.6.1/fluiddoc/mathmacro.py
--rw-r--r--   0        0        0     1127 2024-02-17 22:43:56.161004 fluiddyn-0.6.1/fluiddyn/__init__.py
--rw-r--r--   0        0        0      343 2024-02-17 22:43:56.165003 fluiddyn-0.6.1/fluiddyn/_version.py
--rw-r--r--   0        0        0      144 2024-02-17 22:43:56.165003 fluiddyn-0.6.1/fluiddyn/calcul/__init__.py
--rw-r--r--   0        0        0    18805 2024-02-17 22:43:56.165003 fluiddyn-0.6.1/fluiddyn/calcul/easypyfft.py
--rw-r--r--   0        0        0     4223 2024-02-17 22:43:56.165003 fluiddyn-0.6.1/fluiddyn/calcul/setofvariables.py
--rw-r--r--   0        0        0     5250 2024-02-17 22:43:56.165003 fluiddyn-0.6.1/fluiddyn/calcul/signal.py
--rw-r--r--   0        0        0    24798 2024-02-17 22:43:56.169003 fluiddyn-0.6.1/fluiddyn/calcul/sphericalharmo.py
--rw-r--r--   0        0        0        0 2024-02-17 22:43:56.169003 fluiddyn-0.6.1/fluiddyn/calcul/test/__init__.py
--rw-r--r--   0        0        0     5783 2024-02-17 22:43:56.169003 fluiddyn-0.6.1/fluiddyn/calcul/test/test_easypyfft.py
--rw-r--r--   0        0        0      330 2024-02-17 22:43:56.169003 fluiddyn-0.6.1/fluiddyn/calcul/test/test_setofvariables.py
--rw-r--r--   0        0        0      660 2024-02-17 22:43:56.169003 fluiddyn-0.6.1/fluiddyn/calcul/test/test_signal.py
--rw-r--r--   0        0        0      895 2024-02-17 22:43:56.173003 fluiddyn-0.6.1/fluiddyn/calcul/test/test_sphericalharmo.py
--rw-r--r--   0        0        0     2887 2024-02-17 22:43:56.173003 fluiddyn-0.6.1/fluiddyn/clusters/__init__.py
--rw-r--r--   0        0        0      875 2024-02-17 22:43:56.173003 fluiddyn-0.6.1/fluiddyn/clusters/azzurra.py
--rw-r--r--   0        0        0      995 2024-02-17 22:43:56.173003 fluiddyn-0.6.1/fluiddyn/clusters/ciment.py
--rw-r--r--   0        0        0     1274 2024-02-17 22:43:56.173003 fluiddyn-0.6.1/fluiddyn/clusters/cines.py
--rw-r--r--   0        0        0      834 2024-02-17 22:43:56.173003 fluiddyn-0.6.1/fluiddyn/clusters/idris.py
--rw-r--r--   0        0        0     1045 2024-03-26 14:13:20.514828 fluiddyn-0.6.1/fluiddyn/clusters/legi.py
--rw-r--r--   0        0        0      716 2024-02-17 22:43:56.177003 fluiddyn-0.6.1/fluiddyn/clusters/licallo.py
--rw-r--r--   0        0        0     8102 2024-02-17 22:43:56.177003 fluiddyn-0.6.1/fluiddyn/clusters/local.py
--rw-r--r--   0        0        0     9408 2024-02-17 22:43:56.177003 fluiddyn-0.6.1/fluiddyn/clusters/oar.py
--rw-r--r--   0        0        0     8351 2024-02-17 22:43:56.177003 fluiddyn-0.6.1/fluiddyn/clusters/pbs.py
--rw-r--r--   0        0        0    16542 2024-02-17 22:43:56.181003 fluiddyn-0.6.1/fluiddyn/clusters/slurm.py
--rw-r--r--   0        0        0     4178 2024-02-17 22:43:56.181003 fluiddyn-0.6.1/fluiddyn/clusters/snic.py
--rw-r--r--   0        0        0        0 2024-02-17 22:43:56.181003 fluiddyn-0.6.1/fluiddyn/clusters/test/__init__.py
--rw-r--r--   0        0        0     1026 2024-02-17 22:43:56.181003 fluiddyn-0.6.1/fluiddyn/clusters/test/test_local.py
--rw-r--r--   0        0        0     2865 2024-03-26 14:13:20.514828 fluiddyn-0.6.1/fluiddyn/clusters/test/test_oar.py
--rw-r--r--   0        0        0     2797 2024-02-17 22:43:56.185003 fluiddyn-0.6.1/fluiddyn/clusters/test/test_pbs.py
--rw-r--r--   0        0        0     3479 2024-02-17 22:43:56.185003 fluiddyn-0.6.1/fluiddyn/clusters/test/test_slurm_snic.py
--rw-r--r--   0        0        0     2115 2024-03-20 15:24:08.394333 fluiddyn-0.6.1/fluiddyn/io/__init__.py
--rw-r--r--   0        0        0     5138 2024-02-17 22:43:56.185003 fluiddyn-0.6.1/fluiddyn/io/binary.py
--rw-r--r--   0        0        0     3822 2024-02-17 22:43:56.185003 fluiddyn-0.6.1/fluiddyn/io/dantec.py
--rw-r--r--   0        0        0     3779 2024-02-17 22:43:56.189003 fluiddyn-0.6.1/fluiddyn/io/davis.py
--rw-r--r--   0        0        0    19554 2024-02-17 22:43:56.189003 fluiddyn-0.6.1/fluiddyn/io/digiflow.py
--rw-r--r--   0        0        0     4052 2024-02-17 22:43:56.189003 fluiddyn-0.6.1/fluiddyn/io/dump.py
--rw-r--r--   0        0        0     4758 2024-02-17 22:43:56.189003 fluiddyn-0.6.1/fluiddyn/io/hdf5.py
--rw-r--r--   0        0        0     5683 2024-02-17 22:43:56.189003 fluiddyn-0.6.1/fluiddyn/io/image.py
--rw-r--r--   0        0        0     1378 2024-02-17 22:43:56.193003 fluiddyn-0.6.1/fluiddyn/io/in_py.py
--rw-r--r--   0        0        0    13149 2024-02-17 22:43:56.193003 fluiddyn-0.6.1/fluiddyn/io/multitiff.py
--rw-r--r--   0        0        0     1762 2024-02-17 22:43:56.193003 fluiddyn-0.6.1/fluiddyn/io/mycsv.py
--rw-r--r--   0        0        0    12165 2024-02-17 22:43:56.193003 fluiddyn-0.6.1/fluiddyn/io/ns3d.py
--rw-r--r--   0        0        0     2539 2024-02-17 22:43:56.197003 fluiddyn-0.6.1/fluiddyn/io/query.py
--rw-r--r--   0        0        0     2809 2024-02-17 22:43:56.197003 fluiddyn-0.6.1/fluiddyn/io/rdvision.py
--rw-r--r--   0        0        0     1142 2024-02-17 22:43:56.197003 fluiddyn-0.6.1/fluiddyn/io/redirect_stdout.py
--rw-r--r--   0        0        0      620 2024-02-17 22:43:56.197003 fluiddyn-0.6.1/fluiddyn/io/tee.py
--rw-r--r--   0        0        0        0 2024-02-17 22:43:56.197003 fluiddyn-0.6.1/fluiddyn/io/test/__init__.py
--rw-r--r--   0        0        0     2460 2024-02-17 22:43:56.197003 fluiddyn-0.6.1/fluiddyn/io/test/ns3d_files/PV.t=0000.000
--rw-r--r--   0        0        0      284 2024-02-17 22:43:56.201003 fluiddyn-0.6.1/fluiddyn/io/test/ns3d_files/forcing_2D_info.in_L=30x30_nh=48_expLO_b=1.8_Ti=7.0_nbgene=4_d=4_T=28
--rw-r--r--   0        0        0      284 2024-02-17 22:43:56.201003 fluiddyn-0.6.1/fluiddyn/io/test/ns3d_files/forcing_2D_info.in_L=30x30_nh=48_expLO_b=1.8_Ti=7.0_nbgene=4_d=4_T=28_little-endian
--rw-r--r--   0        0        0      429 2024-02-17 22:43:56.201003 fluiddyn-0.6.1/fluiddyn/io/test/rdvision_files/Dalsa2.seq
--rw-r--r--   0        0        0       48 2024-02-17 22:43:56.201003 fluiddyn-0.6.1/fluiddyn/io/test/rdvision_files/Dalsa2.sqb
--rw-r--r--   0        0        0     1267 2024-02-17 22:43:56.201003 fluiddyn-0.6.1/fluiddyn/io/test/rdvision_files/Dalsa2.xml
--rw-r--r--   0        0        0     1137 2024-02-17 22:43:56.201003 fluiddyn-0.6.1/fluiddyn/io/test/test_binary.py
--rw-r--r--   0        0        0      525 2024-02-17 22:43:56.205003 fluiddyn-0.6.1/fluiddyn/io/test/test_dantec.py
--rw-r--r--   0        0        0      660 2024-02-17 22:43:56.205003 fluiddyn-0.6.1/fluiddyn/io/test/test_digiflow.py
--rw-r--r--   0        0        0     1456 2024-02-17 22:43:56.205003 fluiddyn-0.6.1/fluiddyn/io/test/test_dump.py
--rw-r--r--   0        0        0     2123 2024-02-17 22:43:56.205003 fluiddyn-0.6.1/fluiddyn/io/test/test_hdf5.py
--rw-r--r--   0        0        0     2909 2024-02-17 22:43:56.205003 fluiddyn-0.6.1/fluiddyn/io/test/test_image.py
--rw-r--r--   0        0        0     1224 2024-02-17 22:43:56.205003 fluiddyn-0.6.1/fluiddyn/io/test/test_in_py.py
--rw-r--r--   0        0        0     2411 2024-02-17 22:43:56.209003 fluiddyn-0.6.1/fluiddyn/io/test/test_multitiff.py
--rw-r--r--   0        0        0      746 2024-02-17 22:43:56.209003 fluiddyn-0.6.1/fluiddyn/io/test/test_mycsv.py
--rw-r--r--   0        0        0     1855 2024-02-17 22:43:56.209003 fluiddyn-0.6.1/fluiddyn/io/test/test_ns3d.py
--rw-r--r--   0        0        0     1232 2024-02-17 22:43:56.209003 fluiddyn-0.6.1/fluiddyn/io/test/test_query.py
--rw-r--r--   0        0        0     1027 2024-02-17 22:43:56.209003 fluiddyn-0.6.1/fluiddyn/io/test/test_rdvision.py
--rw-r--r--   0        0        0      739 2024-02-17 22:43:56.209003 fluiddyn-0.6.1/fluiddyn/io/test/test_tee.py
--rw-r--r--   0        0        0     1095 2024-02-17 22:43:56.213003 fluiddyn-0.6.1/fluiddyn/io/test/test_txt.py
--rw-r--r--   0        0        0     3342 2024-02-17 22:43:56.213003 fluiddyn-0.6.1/fluiddyn/io/txt.py
--rw-r--r--   0        0        0      533 2024-02-17 22:43:56.213003 fluiddyn-0.6.1/fluiddyn/output/__init__.py
--rw-r--r--   0        0        0     6098 2024-02-17 22:43:56.213003 fluiddyn-0.6.1/fluiddyn/output/colorchart.py
--rw-r--r--   0        0        0     5323 2024-02-17 22:43:56.213003 fluiddyn-0.6.1/fluiddyn/output/figs.py
--rw-r--r--   0        0        0     1177 2024-02-17 22:43:56.217003 fluiddyn-0.6.1/fluiddyn/output/rcparams.py
--rw-r--r--   0        0        0        0 2024-02-17 22:43:56.217003 fluiddyn-0.6.1/fluiddyn/output/test/__init__.py
--rw-r--r--   0        0        0      307 2024-02-17 22:43:56.217003 fluiddyn-0.6.1/fluiddyn/output/test/test_colorchart.py
--rw-r--r--   0        0        0     1052 2024-02-17 22:43:56.217003 fluiddyn-0.6.1/fluiddyn/output/test/test_figs.py
--rw-r--r--   0        0        0      721 2024-02-17 22:43:56.217003 fluiddyn-0.6.1/fluiddyn/output/util.py
--rw-r--r--   0        0        0     1135 2024-02-17 22:43:56.217003 fluiddyn-0.6.1/fluiddyn/util/__init__.py
--rw-r--r--   0        0        0      133 2024-02-17 22:43:56.217003 fluiddyn-0.6.1/fluiddyn/util/compat.py
--rw-r--r--   0        0        0      304 2024-02-17 22:43:56.221003 fluiddyn-0.6.1/fluiddyn/util/constants.py
--rw-r--r--   0        0        0     1068 2024-02-17 22:43:56.221003 fluiddyn-0.6.1/fluiddyn/util/daemons.py
--rw-r--r--   0        0        0    15219 2024-02-17 22:43:56.221003 fluiddyn-0.6.1/fluiddyn/util/info.py
--rw-r--r--   0        0        0     4282 2024-02-17 22:43:56.221003 fluiddyn-0.6.1/fluiddyn/util/logger.py
--rw-r--r--   0        0        0     3513 2024-02-17 22:43:56.225003 fluiddyn-0.6.1/fluiddyn/util/mail.py
--rw-r--r--   0        0        0     1971 2024-02-17 22:43:56.225003 fluiddyn-0.6.1/fluiddyn/util/matlab2py/__init__.py
--rw-r--r--   0        0        0     5860 2024-02-17 22:43:56.225003 fluiddyn-0.6.1/fluiddyn/util/matlab2py/cleanmat.py
--rw-r--r--   0        0        0     3238 2024-02-17 22:43:56.225003 fluiddyn-0.6.1/fluiddyn/util/matlab2py/mat2wrongpy.py
--rw-r--r--   0        0        0        0 2024-02-17 22:43:56.225003 fluiddyn-0.6.1/fluiddyn/util/matlab2py/test/__init__.py
--rw-r--r--   0        0        0      810 2024-02-17 22:43:56.225003 fluiddyn-0.6.1/fluiddyn/util/matlab2py/test/courant.m
--rw-r--r--   0        0        0      519 2024-02-17 22:43:56.229003 fluiddyn-0.6.1/fluiddyn/util/matlab2py/test/test_matlab2py.py
--rw-r--r--   0        0        0     3780 2024-02-17 22:43:56.229003 fluiddyn-0.6.1/fluiddyn/util/mpi.py
--rw-r--r--   0        0        0    23542 2024-02-17 22:43:56.229003 fluiddyn-0.6.1/fluiddyn/util/numpy_distutils_cpuinfo.py
--rw-r--r--   0        0        0      964 2024-02-17 22:43:56.229003 fluiddyn-0.6.1/fluiddyn/util/opencv.py
--rw-r--r--   0        0        0    23221 2024-02-17 22:43:56.233003 fluiddyn-0.6.1/fluiddyn/util/paramcontainer.py
--rw-r--r--   0        0        0     7281 2024-02-17 22:43:56.233003 fluiddyn-0.6.1/fluiddyn/util/paramcontainer_gui.py
--rw-r--r--   0        0        0    30269 2024-03-03 14:18:58.297248 fluiddyn-0.6.1/fluiddyn/util/serieofarrays.py
--rw-r--r--   0        0        0     4724 2024-02-17 22:43:56.233003 fluiddyn-0.6.1/fluiddyn/util/terminal_colors.py
--rw-r--r--   0        0        0        0 2024-02-17 22:43:56.233003 fluiddyn-0.6.1/fluiddyn/util/test/__init__.py
--rw-r--r--   0        0        0     1814 2024-02-17 22:43:56.237002 fluiddyn-0.6.1/fluiddyn/util/test/file.xml
--rw-r--r--   0        0        0      808 2024-02-17 22:43:56.237002 fluiddyn-0.6.1/fluiddyn/util/test/test_daemons.py
--rw-r--r--   0        0        0      974 2024-02-17 22:43:56.237002 fluiddyn-0.6.1/fluiddyn/util/test/test_info.py
--rw-r--r--   0        0        0      942 2024-02-17 22:43:56.237002 fluiddyn-0.6.1/fluiddyn/util/test/test_logger.py
--rw-r--r--   0        0        0     2194 2024-02-17 22:43:56.237002 fluiddyn-0.6.1/fluiddyn/util/test/test_mpi.py
--rw-r--r--   0        0        0     4725 2024-02-17 22:43:56.241002 fluiddyn-0.6.1/fluiddyn/util/test/test_paramcontainer.py
--rw-r--r--   0        0        0     6484 2024-03-03 14:18:58.297248 fluiddyn-0.6.1/fluiddyn/util/test/test_serieofarrays.py
--rw-r--r--   0        0        0      797 2024-02-17 22:43:56.241002 fluiddyn-0.6.1/fluiddyn/util/test/test_timer.py
--rw-r--r--   0        0        0     2734 2024-02-17 22:43:56.241002 fluiddyn-0.6.1/fluiddyn/util/test/test_util.py
--rw-r--r--   0        0        0     4522 2024-02-17 22:43:56.241002 fluiddyn-0.6.1/fluiddyn/util/timer.py
--rw-r--r--   0        0        0     1200 2024-02-17 22:43:56.241002 fluiddyn-0.6.1/fluiddyn/util/userconfig.py
--rw-r--r--   0        0        0     9277 2024-02-17 22:43:56.245002 fluiddyn-0.6.1/fluiddyn/util/util.py
--rw-r--r--   0        0        0     4443 2024-02-17 22:43:56.245002 fluiddyn-0.6.1/fluiddyn/util/xmltotext.py
--rw-r--r--   0        0        0     4238 2024-04-02 13:10:35.881428 fluiddyn-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     7114 1970-01-01 00:00:00.000000 fluiddyn-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      314 2024-01-17 16:37:56.387718 fluiddyn-0.6.2/AUTHORS.md
+-rw-r--r--   0        0        0    21394 2023-07-04 19:04:38.313096 fluiddyn-0.6.2/LICENSE.txt
+-rw-r--r--   0        0        0     5322 2024-01-17 16:37:56.387718 fluiddyn-0.6.2/README.rst
+-rw-r--r--   0        0        0     1136 2023-07-04 19:04:38.345096 fluiddyn-0.6.2/fluiddoc/__init__.py
+-rw-r--r--   0        0        0     4408 2024-01-18 13:20:32.401745 fluiddyn-0.6.2/fluiddoc/fluiddocset.py
+-rw-r--r--   0        0        0     2344 2023-07-04 19:04:38.349096 fluiddyn-0.6.2/fluiddoc/fluidnbstripout.py
+-rw-r--r--   0        0        0     3096 2023-07-06 09:48:56.909088 fluiddyn-0.6.2/fluiddoc/ipynb_maker.py
+-rw-r--r--   0        0        0     5174 2023-07-04 19:04:38.349096 fluiddyn-0.6.2/fluiddoc/mathmacro.py
+-rw-r--r--   0        0        0     1127 2023-07-06 09:48:56.913088 fluiddyn-0.6.2/fluiddyn/__init__.py
+-rw-r--r--   0        0        0      343 2024-02-18 20:17:29.053325 fluiddyn-0.6.2/fluiddyn/_version.py
+-rw-r--r--   0        0        0      144 2023-07-04 19:04:38.353096 fluiddyn-0.6.2/fluiddyn/calcul/__init__.py
+-rw-r--r--   0        0        0    18805 2023-07-04 19:04:38.353096 fluiddyn-0.6.2/fluiddyn/calcul/easypyfft.py
+-rw-r--r--   0        0        0     4223 2024-02-18 20:17:29.053325 fluiddyn-0.6.2/fluiddyn/calcul/setofvariables.py
+-rw-r--r--   0        0        0     5250 2024-02-18 20:17:29.053325 fluiddyn-0.6.2/fluiddyn/calcul/signal.py
+-rw-r--r--   0        0        0    24798 2024-02-18 20:17:29.053325 fluiddyn-0.6.2/fluiddyn/calcul/sphericalharmo.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:04:38.357096 fluiddyn-0.6.2/fluiddyn/calcul/test/__init__.py
+-rw-r--r--   0        0        0     5783 2023-07-06 09:48:56.913088 fluiddyn-0.6.2/fluiddyn/calcul/test/test_easypyfft.py
+-rw-r--r--   0        0        0      330 2023-07-04 19:04:38.357096 fluiddyn-0.6.2/fluiddyn/calcul/test/test_setofvariables.py
+-rw-r--r--   0        0        0      660 2023-07-04 19:04:38.361096 fluiddyn-0.6.2/fluiddyn/calcul/test/test_signal.py
+-rw-r--r--   0        0        0      895 2023-07-06 09:48:56.913088 fluiddyn-0.6.2/fluiddyn/calcul/test/test_sphericalharmo.py
+-rw-r--r--   0        0        0     2887 2023-07-04 19:04:38.361096 fluiddyn-0.6.2/fluiddyn/clusters/__init__.py
+-rw-r--r--   0        0        0      875 2023-07-04 19:04:38.361096 fluiddyn-0.6.2/fluiddyn/clusters/azzurra.py
+-rw-r--r--   0        0        0      995 2024-02-18 20:17:29.057325 fluiddyn-0.6.2/fluiddyn/clusters/ciment.py
+-rw-r--r--   0        0        0     1274 2023-07-06 09:48:56.913088 fluiddyn-0.6.2/fluiddyn/clusters/cines.py
+-rw-r--r--   0        0        0      834 2023-07-04 19:04:38.365096 fluiddyn-0.6.2/fluiddyn/clusters/idris.py
+-rw-r--r--   0        0        0     1045 2024-03-26 14:06:06.131975 fluiddyn-0.6.2/fluiddyn/clusters/legi.py
+-rw-r--r--   0        0        0      716 2023-07-04 19:04:38.365096 fluiddyn-0.6.2/fluiddyn/clusters/licallo.py
+-rw-r--r--   0        0        0     8102 2023-07-06 09:48:56.913088 fluiddyn-0.6.2/fluiddyn/clusters/local.py
+-rw-r--r--   0        0        0     9408 2024-02-18 20:17:29.057325 fluiddyn-0.6.2/fluiddyn/clusters/oar.py
+-rw-r--r--   0        0        0     8351 2023-07-04 19:04:38.369096 fluiddyn-0.6.2/fluiddyn/clusters/pbs.py
+-rw-r--r--   0        0        0    16542 2023-07-06 09:48:56.917088 fluiddyn-0.6.2/fluiddyn/clusters/slurm.py
+-rw-r--r--   0        0        0     4178 2023-07-04 19:04:38.369096 fluiddyn-0.6.2/fluiddyn/clusters/snic.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:04:38.369096 fluiddyn-0.6.2/fluiddyn/clusters/test/__init__.py
+-rw-r--r--   0        0        0     1026 2024-02-18 20:17:29.057325 fluiddyn-0.6.2/fluiddyn/clusters/test/test_local.py
+-rw-r--r--   0        0        0     2865 2024-03-26 14:06:06.131975 fluiddyn-0.6.2/fluiddyn/clusters/test/test_oar.py
+-rw-r--r--   0        0        0     2797 2024-02-18 20:17:29.061325 fluiddyn-0.6.2/fluiddyn/clusters/test/test_pbs.py
+-rw-r--r--   0        0        0     3479 2024-02-18 20:17:29.061325 fluiddyn-0.6.2/fluiddyn/clusters/test/test_slurm_snic.py
+-rw-r--r--   0        0        0     2115 2024-03-26 14:06:06.135975 fluiddyn-0.6.2/fluiddyn/io/__init__.py
+-rw-r--r--   0        0        0     5138 2024-02-18 20:17:29.061325 fluiddyn-0.6.2/fluiddyn/io/binary.py
+-rw-r--r--   0        0        0     3822 2024-02-18 20:17:29.061325 fluiddyn-0.6.2/fluiddyn/io/dantec.py
+-rw-r--r--   0        0        0     3779 2024-01-11 10:47:04.851740 fluiddyn-0.6.2/fluiddyn/io/davis.py
+-rw-r--r--   0        0        0    19554 2024-02-18 20:17:29.065325 fluiddyn-0.6.2/fluiddyn/io/digiflow.py
+-rw-r--r--   0        0        0     4052 2024-02-18 20:17:29.065325 fluiddyn-0.6.2/fluiddyn/io/dump.py
+-rw-r--r--   0        0        0     4758 2024-02-18 20:17:29.065325 fluiddyn-0.6.2/fluiddyn/io/hdf5.py
+-rw-r--r--   0        0        0     5683 2023-07-04 19:04:38.381096 fluiddyn-0.6.2/fluiddyn/io/image.py
+-rw-r--r--   0        0        0     1378 2023-07-04 19:04:38.381096 fluiddyn-0.6.2/fluiddyn/io/in_py.py
+-rw-r--r--   0        0        0    13149 2023-07-06 09:48:56.921088 fluiddyn-0.6.2/fluiddyn/io/multitiff.py
+-rw-r--r--   0        0        0     1762 2023-07-04 19:04:38.381096 fluiddyn-0.6.2/fluiddyn/io/mycsv.py
+-rw-r--r--   0        0        0    12165 2024-02-18 20:17:29.065325 fluiddyn-0.6.2/fluiddyn/io/ns3d.py
+-rw-r--r--   0        0        0     2539 2023-07-04 19:04:38.385096 fluiddyn-0.6.2/fluiddyn/io/query.py
+-rw-r--r--   0        0        0     2809 2023-07-04 19:04:38.385096 fluiddyn-0.6.2/fluiddyn/io/rdvision.py
+-rw-r--r--   0        0        0     1142 2024-02-18 20:17:29.069325 fluiddyn-0.6.2/fluiddyn/io/redirect_stdout.py
+-rw-r--r--   0        0        0      620 2023-07-04 19:04:38.385096 fluiddyn-0.6.2/fluiddyn/io/tee.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:04:38.385096 fluiddyn-0.6.2/fluiddyn/io/test/__init__.py
+-rw-r--r--   0        0        0     2460 2023-07-04 19:04:38.385096 fluiddyn-0.6.2/fluiddyn/io/test/ns3d_files/PV.t=0000.000
+-rw-r--r--   0        0        0      284 2023-07-04 19:04:38.389096 fluiddyn-0.6.2/fluiddyn/io/test/ns3d_files/forcing_2D_info.in_L=30x30_nh=48_expLO_b=1.8_Ti=7.0_nbgene=4_d=4_T=28
+-rw-r--r--   0        0        0      284 2023-07-04 19:04:38.389096 fluiddyn-0.6.2/fluiddyn/io/test/ns3d_files/forcing_2D_info.in_L=30x30_nh=48_expLO_b=1.8_Ti=7.0_nbgene=4_d=4_T=28_little-endian
+-rw-r--r--   0        0        0      429 2023-07-04 19:04:38.389096 fluiddyn-0.6.2/fluiddyn/io/test/rdvision_files/Dalsa2.seq
+-rw-r--r--   0        0        0       48 2023-07-04 19:04:38.389096 fluiddyn-0.6.2/fluiddyn/io/test/rdvision_files/Dalsa2.sqb
+-rw-r--r--   0        0        0     1267 2023-07-04 19:04:38.389096 fluiddyn-0.6.2/fluiddyn/io/test/rdvision_files/Dalsa2.xml
+-rw-r--r--   0        0        0     1137 2023-07-04 19:04:38.389096 fluiddyn-0.6.2/fluiddyn/io/test/test_binary.py
+-rw-r--r--   0        0        0      525 2023-07-04 19:04:38.393096 fluiddyn-0.6.2/fluiddyn/io/test/test_dantec.py
+-rw-r--r--   0        0        0      660 2023-07-04 19:04:38.393096 fluiddyn-0.6.2/fluiddyn/io/test/test_digiflow.py
+-rw-r--r--   0        0        0     1456 2023-07-04 19:04:38.393096 fluiddyn-0.6.2/fluiddyn/io/test/test_dump.py
+-rw-r--r--   0        0        0     2123 2023-07-04 19:04:38.393096 fluiddyn-0.6.2/fluiddyn/io/test/test_hdf5.py
+-rw-r--r--   0        0        0     2909 2023-07-04 19:04:38.393096 fluiddyn-0.6.2/fluiddyn/io/test/test_image.py
+-rw-r--r--   0        0        0     1224 2023-07-04 19:04:38.393096 fluiddyn-0.6.2/fluiddyn/io/test/test_in_py.py
+-rw-r--r--   0        0        0     2411 2023-07-04 19:04:38.397096 fluiddyn-0.6.2/fluiddyn/io/test/test_multitiff.py
+-rw-r--r--   0        0        0      746 2023-07-04 19:04:38.397096 fluiddyn-0.6.2/fluiddyn/io/test/test_mycsv.py
+-rw-r--r--   0        0        0     1855 2023-07-04 19:04:38.397096 fluiddyn-0.6.2/fluiddyn/io/test/test_ns3d.py
+-rw-r--r--   0        0        0     1232 2023-07-06 09:48:56.921088 fluiddyn-0.6.2/fluiddyn/io/test/test_query.py
+-rw-r--r--   0        0        0     1027 2023-07-04 19:04:38.397096 fluiddyn-0.6.2/fluiddyn/io/test/test_rdvision.py
+-rw-r--r--   0        0        0      739 2023-07-04 19:04:38.401096 fluiddyn-0.6.2/fluiddyn/io/test/test_tee.py
+-rw-r--r--   0        0        0     1095 2023-07-04 19:04:38.401096 fluiddyn-0.6.2/fluiddyn/io/test/test_txt.py
+-rw-r--r--   0        0        0     3342 2024-02-18 20:17:29.069325 fluiddyn-0.6.2/fluiddyn/io/txt.py
+-rw-r--r--   0        0        0      533 2023-07-06 09:48:56.925088 fluiddyn-0.6.2/fluiddyn/output/__init__.py
+-rw-r--r--   0        0        0     6098 2023-07-04 19:04:38.401096 fluiddyn-0.6.2/fluiddyn/output/colorchart.py
+-rw-r--r--   0        0        0     5323 2024-02-18 20:17:29.069325 fluiddyn-0.6.2/fluiddyn/output/figs.py
+-rw-r--r--   0        0        0     1177 2023-07-04 19:04:38.405096 fluiddyn-0.6.2/fluiddyn/output/rcparams.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:04:38.405096 fluiddyn-0.6.2/fluiddyn/output/test/__init__.py
+-rw-r--r--   0        0        0      307 2023-07-04 19:04:38.405096 fluiddyn-0.6.2/fluiddyn/output/test/test_colorchart.py
+-rw-r--r--   0        0        0     1052 2023-07-06 09:48:56.925088 fluiddyn-0.6.2/fluiddyn/output/test/test_figs.py
+-rw-r--r--   0        0        0      721 2023-07-04 19:04:38.405096 fluiddyn-0.6.2/fluiddyn/output/util.py
+-rw-r--r--   0        0        0     1135 2023-07-06 09:48:56.925088 fluiddyn-0.6.2/fluiddyn/util/__init__.py
+-rw-r--r--   0        0        0      133 2023-07-04 19:04:38.409096 fluiddyn-0.6.2/fluiddyn/util/compat.py
+-rw-r--r--   0        0        0      304 2023-07-04 19:04:38.409096 fluiddyn-0.6.2/fluiddyn/util/constants.py
+-rw-r--r--   0        0        0     1068 2024-02-18 20:17:29.069325 fluiddyn-0.6.2/fluiddyn/util/daemons.py
+-rw-r--r--   0        0        0    15219 2024-02-18 20:17:29.073325 fluiddyn-0.6.2/fluiddyn/util/info.py
+-rw-r--r--   0        0        0     4282 2023-07-04 19:04:38.409096 fluiddyn-0.6.2/fluiddyn/util/logger.py
+-rw-r--r--   0        0        0     3513 2023-07-04 19:04:38.413096 fluiddyn-0.6.2/fluiddyn/util/mail.py
+-rw-r--r--   0        0        0     1971 2023-07-06 09:48:56.925088 fluiddyn-0.6.2/fluiddyn/util/matlab2py/__init__.py
+-rw-r--r--   0        0        0     5860 2024-02-18 20:17:29.073325 fluiddyn-0.6.2/fluiddyn/util/matlab2py/cleanmat.py
+-rw-r--r--   0        0        0     3238 2024-02-18 20:17:29.073325 fluiddyn-0.6.2/fluiddyn/util/matlab2py/mat2wrongpy.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:04:38.413096 fluiddyn-0.6.2/fluiddyn/util/matlab2py/test/__init__.py
+-rw-r--r--   0        0        0      810 2023-07-04 19:04:38.413096 fluiddyn-0.6.2/fluiddyn/util/matlab2py/test/courant.m
+-rw-r--r--   0        0        0      519 2023-07-04 19:04:38.417096 fluiddyn-0.6.2/fluiddyn/util/matlab2py/test/test_matlab2py.py
+-rw-r--r--   0        0        0     3780 2023-07-04 19:04:38.417096 fluiddyn-0.6.2/fluiddyn/util/mpi.py
+-rw-r--r--   0        0        0    23542 2024-02-18 20:17:29.073325 fluiddyn-0.6.2/fluiddyn/util/numpy_distutils_cpuinfo.py
+-rw-r--r--   0        0        0      964 2024-02-18 20:17:29.077325 fluiddyn-0.6.2/fluiddyn/util/opencv.py
+-rw-r--r--   0        0        0    23221 2024-01-18 13:20:32.405745 fluiddyn-0.6.2/fluiddyn/util/paramcontainer.py
+-rw-r--r--   0        0        0     7281 2024-01-18 13:20:32.405745 fluiddyn-0.6.2/fluiddyn/util/paramcontainer_gui.py
+-rw-r--r--   0        0        0    32191 2024-04-16 08:16:22.836543 fluiddyn-0.6.2/fluiddyn/util/serieofarrays.py
+-rw-r--r--   0        0        0     4724 2023-07-04 19:04:38.421096 fluiddyn-0.6.2/fluiddyn/util/terminal_colors.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:04:38.421096 fluiddyn-0.6.2/fluiddyn/util/test/__init__.py
+-rw-r--r--   0        0        0     1814 2023-07-04 19:04:38.421096 fluiddyn-0.6.2/fluiddyn/util/test/file.xml
+-rw-r--r--   0        0        0      808 2023-07-04 19:04:38.421096 fluiddyn-0.6.2/fluiddyn/util/test/test_daemons.py
+-rw-r--r--   0        0        0      974 2024-02-18 20:17:29.077325 fluiddyn-0.6.2/fluiddyn/util/test/test_info.py
+-rw-r--r--   0        0        0      942 2024-01-18 13:20:32.409745 fluiddyn-0.6.2/fluiddyn/util/test/test_logger.py
+-rw-r--r--   0        0        0     2194 2023-07-06 09:48:56.929088 fluiddyn-0.6.2/fluiddyn/util/test/test_mpi.py
+-rw-r--r--   0        0        0     4725 2023-07-06 09:48:56.929088 fluiddyn-0.6.2/fluiddyn/util/test/test_paramcontainer.py
+-rw-r--r--   0        0        0     7447 2024-04-16 08:16:22.840543 fluiddyn-0.6.2/fluiddyn/util/test/test_serieofarrays.py
+-rw-r--r--   0        0        0      797 2023-07-04 19:04:38.425096 fluiddyn-0.6.2/fluiddyn/util/test/test_timer.py
+-rw-r--r--   0        0        0     2734 2023-07-06 09:48:56.929088 fluiddyn-0.6.2/fluiddyn/util/test/test_util.py
+-rw-r--r--   0        0        0     4522 2023-07-04 19:04:38.429096 fluiddyn-0.6.2/fluiddyn/util/timer.py
+-rw-r--r--   0        0        0     1200 2023-07-04 19:04:38.429096 fluiddyn-0.6.2/fluiddyn/util/userconfig.py
+-rw-r--r--   0        0        0     9277 2024-02-18 20:17:29.081325 fluiddyn-0.6.2/fluiddyn/util/util.py
+-rw-r--r--   0        0        0     4443 2023-07-04 19:04:38.429096 fluiddyn-0.6.2/fluiddyn/util/xmltotext.py
+-rw-r--r--   0        0        0     4238 2024-04-16 08:16:57.716501 fluiddyn-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     7114 1970-01-01 00:00:00.000000 fluiddyn-0.6.2/PKG-INFO
```

### Comparing `fluiddyn-0.6.1/LICENSE.txt` & `fluiddyn-0.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/README.rst` & `fluiddyn-0.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddoc/__init__.py` & `fluiddyn-0.6.2/fluiddoc/__init__.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddoc/fluiddocset.py` & `fluiddyn-0.6.2/fluiddoc/fluiddocset.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddoc/fluidnbstripout.py` & `fluiddyn-0.6.2/fluiddoc/fluidnbstripout.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddoc/ipynb_maker.py` & `fluiddyn-0.6.2/fluiddoc/ipynb_maker.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddoc/mathmacro.py` & `fluiddyn-0.6.2/fluiddoc/mathmacro.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/__init__.py` & `fluiddyn-0.6.2/fluiddyn/__init__.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/calcul/easypyfft.py` & `fluiddyn-0.6.2/fluiddyn/calcul/easypyfft.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/calcul/setofvariables.py` & `fluiddyn-0.6.2/fluiddyn/calcul/setofvariables.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/calcul/signal.py` & `fluiddyn-0.6.2/fluiddyn/calcul/signal.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/calcul/sphericalharmo.py` & `fluiddyn-0.6.2/fluiddyn/calcul/sphericalharmo.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/calcul/test/test_easypyfft.py` & `fluiddyn-0.6.2/fluiddyn/calcul/test/test_easypyfft.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/calcul/test/test_signal.py` & `fluiddyn-0.6.2/fluiddyn/calcul/test/test_signal.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/calcul/test/test_sphericalharmo.py` & `fluiddyn-0.6.2/fluiddyn/calcul/test/test_sphericalharmo.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/clusters/__init__.py` & `fluiddyn-0.6.2/fluiddyn/clusters/__init__.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/clusters/azzurra.py` & `fluiddyn-0.6.2/fluiddyn/clusters/azzurra.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/clusters/ciment.py` & `fluiddyn-0.6.2/fluiddyn/clusters/ciment.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/clusters/cines.py` & `fluiddyn-0.6.2/fluiddyn/clusters/cines.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/clusters/idris.py` & `fluiddyn-0.6.2/fluiddyn/clusters/idris.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/clusters/legi.py` & `fluiddyn-0.6.2/fluiddyn/clusters/legi.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/clusters/licallo.py` & `fluiddyn-0.6.2/fluiddyn/clusters/licallo.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/clusters/local.py` & `fluiddyn-0.6.2/fluiddyn/clusters/local.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/clusters/oar.py` & `fluiddyn-0.6.2/fluiddyn/clusters/oar.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/clusters/pbs.py` & `fluiddyn-0.6.2/fluiddyn/clusters/pbs.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/clusters/slurm.py` & `fluiddyn-0.6.2/fluiddyn/clusters/slurm.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/clusters/snic.py` & `fluiddyn-0.6.2/fluiddyn/clusters/snic.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/clusters/test/test_local.py` & `fluiddyn-0.6.2/fluiddyn/clusters/test/test_local.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/clusters/test/test_oar.py` & `fluiddyn-0.6.2/fluiddyn/clusters/test/test_oar.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/clusters/test/test_pbs.py` & `fluiddyn-0.6.2/fluiddyn/clusters/test/test_pbs.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/clusters/test/test_slurm_snic.py` & `fluiddyn-0.6.2/fluiddyn/clusters/test/test_slurm_snic.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/__init__.py` & `fluiddyn-0.6.2/fluiddyn/io/__init__.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/binary.py` & `fluiddyn-0.6.2/fluiddyn/io/binary.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/dantec.py` & `fluiddyn-0.6.2/fluiddyn/io/dantec.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/davis.py` & `fluiddyn-0.6.2/fluiddyn/io/davis.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/digiflow.py` & `fluiddyn-0.6.2/fluiddyn/io/digiflow.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/dump.py` & `fluiddyn-0.6.2/fluiddyn/io/dump.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/hdf5.py` & `fluiddyn-0.6.2/fluiddyn/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/image.py` & `fluiddyn-0.6.2/fluiddyn/io/image.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/in_py.py` & `fluiddyn-0.6.2/fluiddyn/io/in_py.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/multitiff.py` & `fluiddyn-0.6.2/fluiddyn/io/multitiff.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/mycsv.py` & `fluiddyn-0.6.2/fluiddyn/io/mycsv.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/ns3d.py` & `fluiddyn-0.6.2/fluiddyn/io/ns3d.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/query.py` & `fluiddyn-0.6.2/fluiddyn/io/query.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/rdvision.py` & `fluiddyn-0.6.2/fluiddyn/io/rdvision.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/redirect_stdout.py` & `fluiddyn-0.6.2/fluiddyn/io/redirect_stdout.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/tee.py` & `fluiddyn-0.6.2/fluiddyn/io/tee.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/test/ns3d_files/PV.t=0000.000` & `fluiddyn-0.6.2/fluiddyn/io/test/ns3d_files/PV.t=0000.000`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/test/rdvision_files/Dalsa2.xml` & `fluiddyn-0.6.2/fluiddyn/io/test/rdvision_files/Dalsa2.xml`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/test/test_binary.py` & `fluiddyn-0.6.2/fluiddyn/io/test/test_binary.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/test/test_dantec.py` & `fluiddyn-0.6.2/fluiddyn/io/test/test_dantec.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/test/test_digiflow.py` & `fluiddyn-0.6.2/fluiddyn/io/test/test_digiflow.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/test/test_dump.py` & `fluiddyn-0.6.2/fluiddyn/io/test/test_dump.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/test/test_hdf5.py` & `fluiddyn-0.6.2/fluiddyn/io/test/test_hdf5.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/test/test_image.py` & `fluiddyn-0.6.2/fluiddyn/io/test/test_image.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/test/test_in_py.py` & `fluiddyn-0.6.2/fluiddyn/io/test/test_in_py.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/test/test_multitiff.py` & `fluiddyn-0.6.2/fluiddyn/io/test/test_multitiff.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/test/test_mycsv.py` & `fluiddyn-0.6.2/fluiddyn/io/test/test_mycsv.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/test/test_ns3d.py` & `fluiddyn-0.6.2/fluiddyn/io/test/test_ns3d.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/test/test_query.py` & `fluiddyn-0.6.2/fluiddyn/io/test/test_query.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/test/test_rdvision.py` & `fluiddyn-0.6.2/fluiddyn/io/test/test_rdvision.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/test/test_tee.py` & `fluiddyn-0.6.2/fluiddyn/io/test/test_tee.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/test/test_txt.py` & `fluiddyn-0.6.2/fluiddyn/io/test/test_txt.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/io/txt.py` & `fluiddyn-0.6.2/fluiddyn/io/txt.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/output/__init__.py` & `fluiddyn-0.6.2/fluiddyn/output/__init__.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/output/colorchart.py` & `fluiddyn-0.6.2/fluiddyn/output/colorchart.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/output/figs.py` & `fluiddyn-0.6.2/fluiddyn/output/figs.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/output/rcparams.py` & `fluiddyn-0.6.2/fluiddyn/output/rcparams.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/output/test/test_figs.py` & `fluiddyn-0.6.2/fluiddyn/output/test/test_figs.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/output/util.py` & `fluiddyn-0.6.2/fluiddyn/output/util.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/__init__.py` & `fluiddyn-0.6.2/fluiddyn/util/__init__.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/daemons.py` & `fluiddyn-0.6.2/fluiddyn/util/daemons.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/info.py` & `fluiddyn-0.6.2/fluiddyn/util/info.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/logger.py` & `fluiddyn-0.6.2/fluiddyn/util/logger.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/mail.py` & `fluiddyn-0.6.2/fluiddyn/util/mail.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/matlab2py/__init__.py` & `fluiddyn-0.6.2/fluiddyn/util/matlab2py/__init__.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/matlab2py/cleanmat.py` & `fluiddyn-0.6.2/fluiddyn/util/matlab2py/cleanmat.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/matlab2py/mat2wrongpy.py` & `fluiddyn-0.6.2/fluiddyn/util/matlab2py/mat2wrongpy.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/matlab2py/test/courant.m` & `fluiddyn-0.6.2/fluiddyn/util/matlab2py/test/courant.m`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/matlab2py/test/test_matlab2py.py` & `fluiddyn-0.6.2/fluiddyn/util/matlab2py/test/test_matlab2py.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/mpi.py` & `fluiddyn-0.6.2/fluiddyn/util/mpi.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/numpy_distutils_cpuinfo.py` & `fluiddyn-0.6.2/fluiddyn/util/numpy_distutils_cpuinfo.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/opencv.py` & `fluiddyn-0.6.2/fluiddyn/util/opencv.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/paramcontainer.py` & `fluiddyn-0.6.2/fluiddyn/util/paramcontainer.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/paramcontainer_gui.py` & `fluiddyn-0.6.2/fluiddyn/util/paramcontainer_gui.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/serieofarrays.py` & `fluiddyn-0.6.2/fluiddyn/util/serieofarrays.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,14 +38,55 @@
 
 
 def get_nb_arrays_in_file(fname):
     with pims.open(fname) as images:
         return images.len()
 
 
+ALPHABET_SIZE = 26
+
+
+def _decompose_in_alpha_base(number):
+    """Generate digits from `number` in base alphabet,
+    least significant bits first.
+
+    """
+    while number:
+        number, remainder = divmod(number, ALPHABET_SIZE)
+        yield remainder
+
+
+def _letters_from_number(number):
+    """Convert a number in base 26 to letters"""
+    word = [_letter_from_number(idx) for idx in _decompose_in_alpha_base(number)]
+    return "".join(word[::-1])
+
+
+def _number_from_letters(letters):
+    """Convert letters to an integer in base 26"""
+    # assert ord("a") == 97
+    letters = letters.lower()
+    number = 0
+    for i_letter, letter in enumerate(letters[::-1]):
+        number += (ord(letter) - 97) * ALPHABET_SIZE**i_letter
+    return number
+
+
+def _number_from_letter(letter):
+    """Convert a letter to a number in base 26"""
+    # assert ord("a") == 97
+    return ord(letter) - 97
+
+
+def _letter_from_number(number):
+    """Convert a number in base 26 to a letter"""
+    # assert ord("a") == 97
+    return chr(97 + number)
+
+
 MAX_SEARCH_INDEX_START = 100000
 
 
 def compute_slices(str_slices):
     """Return a tuple of slices"""
     slices = []
     parts = str_slices.split(",")
@@ -134,28 +175,28 @@
 
     Parameters
     ----------
 
     path : str
         The path of the base directory or of a file example.
 
-    slicing_tuples : None or iterable of iterables or str
+    slicing : None or iterable of iterables or str
 
         Iterable of slides (start, stop, step).
 
         Can also be a string of the form "0:2:6, 1" (in this case for two
         indexes).
 
     Attributes
     ----------
     path_dir : str
         The path of the base directory.
 
-    slicing_tuples : list of list
-        Lists of slides "[start, stop, step]" (one for each index).
+    get_slicing_tuples/set_slicing_tuples : list of tuples
+        Lists of slicing tuples "(start, stop, step)" (one for each index).
         This list can be changed to loop over different sets of files.
 
     Notes
     -----
 
     An instance of SerieOfArraysFromFiles is an iterable and provides
     other iterables.
@@ -191,21 +232,24 @@
             remains = remains[1:]
         else:
             self._separator_base_index = ""
 
         self._index_types = []
         self._index_lens = []
         self._index_separators = []
+        self._index_capitalized = []
         while len(remains) != 0:
             if remains[0].isdigit():
                 test_type = str.isdigit
                 self._index_types.append("digit")
+                self._index_capitalized.append(None)
             elif remains[0].isalpha():
                 test_type = str.isalpha
                 self._index_types.append("alpha")
+                self._index_capitalized.append(not remains[0].islower())
             str_index = "".join(itertools.takewhile(test_type, remains))
             self._index_lens.append(len(str_index))
             remains = remains[len(str_index) :]
             if len(remains) > 0:
                 if not str.isalnum(remains[0]):
                     self._index_separators.append(remains[0])
                     remains = remains[1:]
@@ -335,14 +379,15 @@
           As many indices as used in the serie. For example with names of the
           form 'im100a.png', 2 indices are needed.
 
         """
         return self.get_array_from_name(self.compute_name_from_indices(*indices))
 
     def get_tuples_indices(self):
+        """Get a list of tuples containing the indices computed from `self._slicing_tuples`"""
         return [
             tuple(range(*start_stop_step))
             for start_stop_step in self._slicing_tuples
         ]
 
     def get_indices_from_index(self, index):
         """Get indices from a flatten index"""
@@ -395,14 +440,15 @@
 
         """
         return (
             os.path.join(self.path_dir, name) for name in self.get_name_arrays()
         )
 
     def get_name_path_arrays(self):
+        """Iterable returning tuples ``(name, path)``"""
         return (
             (name, os.path.join(self.path_dir, name))
             for name in self.get_name_arrays()
         )
 
     def check_all_files_exist(self):
         """Check that all files exist."""
@@ -479,25 +525,34 @@
     def get_tuple_array_name_from_index(self, index: int = 0):
         """Get an array and its name"""
         indices = self.get_indices_from_index(index)
         name = self.compute_name_from_indices(*indices)
         return self.get_array_from_name(name), name
 
     def get_str_for_name_from_idim_idx(self, idim, idx):
+        """Compute the str corresponding to the index ``idx`` for the dimension ``idim``"""
         if self._from_movies and idim == self.nb_indices - 1:
             return str(idx)
 
         if self._index_types[idim] == "digit":
             code_format = "{:0" + str(self._index_lens[idim]) + "d}"
             str_index = code_format.format(idx)
         elif self._index_types[idim] == "alpha":
-            if idx > 25:
-                raise ValueError('"alpha" index larger than 25.')
+            if idx <= 25:
+                str_index = _letter_from_number(idx)
+            else:
+                str_index = _letters_from_number(idx)
+
+            if len(str_index) != self._index_lens[idim]:
+                str_index = (
+                    "a" * (self._index_lens[idim] - len(str_index)) + str_index
+                )
+            if self._index_capitalized[idim]:
+                str_index = str_index.upper()
 
-            str_index = chr(ord("a") + idx)
         else:
             raise ValueError('The type should be "digit" or "alpha".')
 
         return str_index
 
     def compute_str_indices_from_indices(self, *indices):
         """Compute the string corresponding to the indices.
@@ -581,16 +636,19 @@
             remains = remains[len(index) :]
             if self._index_separators[i_ind] != "":
                 remains = remains[1:]
 
             if self._index_types[i_ind] == "digit":
                 index = int(index)
             elif self._index_types[i_ind] == "alpha":
-                index = ord(index) - ord("a")
-
+                index = index.lower()
+                if len(index) == 1:
+                    index = _number_from_letter(index)
+                else:
+                    index = _number_from_letters(index)
             indices.append(index)
 
         if internal_index is not None:
             indices.append(internal_index)
 
         assert len(remains) == 0
         return indices
```

### Comparing `fluiddyn-0.6.1/fluiddyn/util/terminal_colors.py` & `fluiddyn-0.6.2/fluiddyn/util/terminal_colors.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/test/file.xml` & `fluiddyn-0.6.2/fluiddyn/util/test/file.xml`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/test/test_daemons.py` & `fluiddyn-0.6.2/fluiddyn/util/test/test_daemons.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/test/test_info.py` & `fluiddyn-0.6.2/fluiddyn/util/test/test_info.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/test/test_logger.py` & `fluiddyn-0.6.2/fluiddyn/util/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/test/test_mpi.py` & `fluiddyn-0.6.2/fluiddyn/util/test/test_mpi.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/test/test_paramcontainer.py` & `fluiddyn-0.6.2/fluiddyn/util/test/test_paramcontainer.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/test/test_serieofarrays.py` & `fluiddyn-0.6.2/fluiddyn/util/test/test_serieofarrays.py`

 * *Files 16% similar despite different names*

```diff
@@ -234,7 +234,36 @@
 
     series = SeriesOfArrays(path_dir, "pairs")
     assert len(series) == 8
     serie = series.get_serie_from_index(0)
     assert len(serie) == 2
 
     check_all1by1(path_dir, 16)
+
+
+def test_two_letters(tmp_path):
+    for index in range(60, 62):
+        (tmp_path / f"piv{index}bb.h5").touch()
+    serie = SerieOfArraysFromFiles(tmp_path)
+    assert serie.get_name_files()[0] == "piv60bb.h5"
+    assert serie.compute_name_from_indices(2, 1) == "piv02ab.h5"
+    assert serie.compute_name_from_indices(2, 27) == "piv02bb.h5"
+
+
+def test_two_capital_letters(tmp_path):
+    for index in range(60, 62):
+        (tmp_path / f"piv{index}BB.h5").touch()
+    serie = SerieOfArraysFromFiles(tmp_path)
+    assert serie.get_name_files()[0] == "piv60BB.h5"
+    assert serie.compute_name_from_indices(2, 1) == "piv02AB.h5"
+    assert serie.compute_name_from_indices(2, 27) == "piv02BB.h5"
+
+
+def test_convert_letters_number():
+
+    from fluiddyn.util.serieofarrays import (
+        _letters_from_number,
+        _number_from_letters,
+    )
+
+    for letters in ("bc", "oh", "cba"):
+        assert _letters_from_number(_number_from_letters(letters)) == letters
```

### Comparing `fluiddyn-0.6.1/fluiddyn/util/test/test_timer.py` & `fluiddyn-0.6.2/fluiddyn/util/test/test_timer.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/test/test_util.py` & `fluiddyn-0.6.2/fluiddyn/util/test/test_util.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/timer.py` & `fluiddyn-0.6.2/fluiddyn/util/timer.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/userconfig.py` & `fluiddyn-0.6.2/fluiddyn/util/userconfig.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/util.py` & `fluiddyn-0.6.2/fluiddyn/util/util.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/fluiddyn/util/xmltotext.py` & `fluiddyn-0.6.2/fluiddyn/util/xmltotext.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.1/pyproject.toml` & `fluiddyn-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "fluiddyn"
-version = "0.6.1"
+version = "0.6.2"
 description = "Framework for studying fluid dynamics."
 keywords = [
     "Fluid dynamics",
     "research",
 ]
 authors = [
     { name = "Pierre Augier", email = "pierre.augier@legi.cnrs.fr" },
```

### Comparing `fluiddyn-0.6.1/PKG-INFO` & `fluiddyn-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: fluiddyn
-Version: 0.6.1
+Version: 0.6.2
 Summary: Framework for studying fluid dynamics.
-Keywords: Fluid dynamics research
+Keywords: Fluid dynamics,research
 Home-page: https://foss.heptapod.net/fluiddyn/fluiddyn
 Author-Email: Pierre Augier <pierre.augier@legi.cnrs.fr>
 License: CeCILL-B License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

