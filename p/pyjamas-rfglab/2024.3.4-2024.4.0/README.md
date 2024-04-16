# Comparing `tmp/pyjamas-rfglab-2024.3.4.tar.gz` & `tmp/pyjamas-rfglab-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjamas-rfglab-2024.3.4.tar", last modified: Fri Mar 22 23:49:36 2024, max compression
+gzip compressed data, was "pyjamas-rfglab-2024.4.0.tar", last modified: Tue Apr 16 21:39:53 2024, max compression
```

## Comparing `pyjamas-rfglab-2024.3.4.tar` & `pyjamas-rfglab-2024.4.0.tar`

### file list

```diff
@@ -1,95 +1,96 @@
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-03-22 23:49:36.116340 pyjamas-rfglab-2024.3.4/
--rw-r--r--   0 rodrigo    (501) staff       (20)      265 2023-01-17 21:44:31.000000 pyjamas-rfglab-2024.3.4/MANIFEST.in
--rw-r--r--   0 rodrigo    (501) staff       (20)     1686 2024-03-22 23:49:36.115229 pyjamas-rfglab-2024.3.4/PKG-INFO
--rw-r--r--   0 rodrigo    (501) staff       (20)     1202 2023-07-11 19:12:22.000000 pyjamas-rfglab-2024.3.4/README.md
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-03-22 23:49:36.048400 pyjamas-rfglab-2024.3.4/pyjamas/
--rw-r--r--   0 rodrigo    (501) staff       (20)    33144 2020-02-04 05:51:32.000000 pyjamas-rfglab-2024.3.4/pyjamas/LICENSE
--rw-r--r--   0 rodrigo    (501) staff       (20)     1088 2020-01-17 04:15:16.000000 pyjamas-rfglab-2024.3.4/pyjamas/__init__.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-03-22 23:49:36.069755 pyjamas-rfglab-2024.3.4/pyjamas/dialogs/
--rw-r--r--   0 rodrigo    (501) staff       (20)     1645 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.3.4/pyjamas/dialogs/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    17593 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.3.4/pyjamas/dialogs/adjustcontrast.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    31465 2024-03-22 23:06:04.000000 pyjamas-rfglab-2024.3.4/pyjamas/dialogs/batchanalysis.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     5509 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.3.4/pyjamas/dialogs/batchprojectconcat.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     6900 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.3.4/pyjamas/dialogs/batchresize.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     2980 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.3.4/pyjamas/dialogs/classifierdialogABC.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3199 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.3.4/pyjamas/dialogs/classifiertype.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     6437 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.3.4/pyjamas/dialogs/expandnpropagateseeds.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     5227 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.3.4/pyjamas/dialogs/expandseeds.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    13000 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.3.4/pyjamas/dialogs/findseeds.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    11361 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.3.4/pyjamas/dialogs/logregression.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3453 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.3.4/pyjamas/dialogs/matplotlibdialog.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     8858 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.3.4/pyjamas/dialogs/measurepoly.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    13277 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.3.4/pyjamas/dialogs/neuralnet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     8699 2024-03-12 21:08:54.000000 pyjamas-rfglab-2024.3.4/pyjamas/dialogs/nonmax_suppr.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     5533 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.3.4/pyjamas/dialogs/propagateseeds.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    14588 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.3.4/pyjamas/dialogs/rescuneuralnet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    12510 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.3.4/pyjamas/dialogs/svm.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     2243 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.3.4/pyjamas/dialogs/textdialog.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     2817 2023-12-27 20:45:04.000000 pyjamas-rfglab-2024.3.4/pyjamas/dialogs/texteditdialog.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     4082 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.3.4/pyjamas/dialogs/timepoints.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1806 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.3.4/pyjamas/dragdropmainwindow.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-03-22 23:49:36.071184 pyjamas-rfglab-2024.3.4/pyjamas/external/
--rw-r--r--   0 rodrigo    (501) staff       (20)      899 2021-05-09 22:07:44.000000 pyjamas-rfglab-2024.3.4/pyjamas/external/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     6852 2020-07-11 20:09:58.000000 pyjamas-rfglab-2024.3.4/pyjamas/external/pascal_voc_io.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     4930 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.3.4/pyjamas/orthogonalviewswindow.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    52323 2024-03-22 23:49:13.000000 pyjamas-rfglab-2024.3.4/pyjamas/pjscore.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    33519 2023-11-22 14:41:28.000000 pyjamas-rfglab-2024.3.4/pyjamas/pjseventfilter.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     2123 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.3.4/pyjamas/pjsthreads.py
--rw-r--r--   0 rodrigo    (501) staff       (20)  2950837 2023-06-21 15:47:44.000000 pyjamas-rfglab-2024.3.4/pyjamas/pyjamas.tif
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-03-22 23:49:36.074692 pyjamas-rfglab-2024.3.4/pyjamas/rannotations/
--rw-r--r--   0 rodrigo    (501) staff       (20)      924 2022-06-20 21:44:00.000000 pyjamas-rfglab-2024.3.4/pyjamas/rannotations/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)      856 2020-01-17 04:15:16.000000 pyjamas-rfglab-2024.3.4/pyjamas/rannotations/rannotation.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    16818 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.3.4/pyjamas/rannotations/rpolyline.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     2288 2022-08-14 20:59:38.000000 pyjamas-rfglab-2024.3.4/pyjamas/rannotations/rvector2d.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-03-22 23:49:36.087397 pyjamas-rfglab-2024.3.4/pyjamas/rcallbacks/
--rw-r--r--   0 rodrigo    (501) staff       (20)     1257 2020-01-17 04:15:16.000000 pyjamas-rfglab-2024.3.4/pyjamas/rcallbacks/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     7690 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.3.4/pyjamas/rcallbacks/rcallback.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1658 2023-02-07 15:13:59.000000 pyjamas-rfglab-2024.3.4/pyjamas/rcallbacks/rcbabout.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    14800 2023-11-02 21:21:06.000000 pyjamas-rfglab-2024.3.4/pyjamas/rcallbacks/rcbannotations.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    71349 2024-03-22 23:49:13.000000 pyjamas-rfglab-2024.3.4/pyjamas/rcallbacks/rcbbatchprocess.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    66584 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.3.4/pyjamas/rcallbacks/rcbclassifiers.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    77584 2024-03-12 21:08:54.000000 pyjamas-rfglab-2024.3.4/pyjamas/rcallbacks/rcbimage.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    50542 2024-03-01 22:58:24.000000 pyjamas-rfglab-2024.3.4/pyjamas/rcallbacks/rcbio.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    11360 2024-03-12 21:08:54.000000 pyjamas-rfglab-2024.3.4/pyjamas/rcallbacks/rcbmeasure.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    13844 2023-11-22 14:41:28.000000 pyjamas-rfglab-2024.3.4/pyjamas/rcallbacks/rcboptions.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3617 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.3.4/pyjamas/rcallbacks/rcbplugins.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-03-22 23:49:36.090603 pyjamas-rfglab-2024.3.4/pyjamas/rimage/
--rw-r--r--   0 rodrigo    (501) staff       (20)      913 2020-05-28 03:02:49.000000 pyjamas-rfglab-2024.3.4/pyjamas/rimage/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3091 2021-08-22 22:13:16.000000 pyjamas-rfglab-2024.3.4/pyjamas/rimage/csgraph.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3774 2024-03-01 22:58:24.000000 pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimcore.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-03-22 23:49:36.106257 pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/
--rw-r--r--   0 rodrigo    (501) staff       (20)     1484 2021-02-14 22:27:21.000000 pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3557 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/batchclassifier.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1585 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/batchml.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     2740 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/batchneuralnet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     7409 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/batchrecurrentneuralnet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)      275 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/classifier_types.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1173 2020-08-28 21:52:01.000000 pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/featurecalculator.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1387 2020-12-27 23:49:18.000000 pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/featurecalculator_rawimage.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1289 2020-12-27 23:49:18.000000 pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/featurecalculator_rowofpixels.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3104 2024-03-12 21:08:54.000000 pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/featurecalculator_sog.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    17339 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/rimclassifier.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1824 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/rimlr.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1382 2021-10-27 20:01:04.000000 pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/rimml.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1857 2021-10-27 20:01:04.000000 pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/rimneuralnet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1960 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/rimrecurrentneuralnet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    20979 2023-07-11 19:12:22.000000 pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/rimrescunet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     2084 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/rimsvm.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    15508 2023-07-11 19:12:22.000000 pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/rimunet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    69198 2024-03-01 22:58:24.000000 pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimutils.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-03-22 23:49:36.108110 pyjamas-rfglab-2024.3.4/pyjamas/rplugins/
--rw-r--r--   0 rodrigo    (501) staff       (20)      847 2020-01-17 04:15:16.000000 pyjamas-rfglab-2024.3.4/pyjamas/rplugins/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1249 2023-02-19 02:47:05.000000 pyjamas-rfglab-2024.3.4/pyjamas/rplugins/base.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    28427 2024-03-14 22:30:31.000000 pyjamas-rfglab-2024.3.4/pyjamas/rutils.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-03-22 23:49:36.110710 pyjamas-rfglab-2024.3.4/pyjamas/tests/
--rw-r--r--   0 rodrigo    (501) staff       (20)      796 2023-01-02 00:28:47.000000 pyjamas-rfglab-2024.3.4/pyjamas/tests/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)      857 2023-01-19 20:27:03.000000 pyjamas-rfglab-2024.3.4/pyjamas/tests/conftest.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-03-22 23:49:36.113689 pyjamas-rfglab-2024.3.4/pyjamas/tests/unit/
--rw-r--r--   0 rodrigo    (501) staff       (20)        0 2022-12-25 02:03:19.000000 pyjamas-rfglab-2024.3.4/pyjamas/tests/unit/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     6339 2023-12-27 20:45:04.000000 pyjamas-rfglab-2024.3.4/pyjamas/tests/unit/pjsfixtures.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    12484 2023-11-22 14:41:28.000000 pyjamas-rfglab-2024.3.4/pyjamas/tests/unit/test_image.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    16029 2023-12-07 19:48:58.000000 pyjamas-rfglab-2024.3.4/pyjamas/tests/unit/test_io.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-03-22 23:49:36.114640 pyjamas-rfglab-2024.3.4/pyjamas_rfglab.egg-info/
--rw-r--r--   0 rodrigo    (501) staff       (20)     2528 2024-03-22 23:49:35.000000 pyjamas-rfglab-2024.3.4/pyjamas_rfglab.egg-info/SOURCES.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)       38 2024-03-22 23:49:36.116534 pyjamas-rfglab-2024.3.4/setup.cfg
--rw-r--r--   0 rodrigo    (501) staff       (20)     2923 2024-03-12 21:08:54.000000 pyjamas-rfglab-2024.3.4/setup.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-16 21:39:53.600836 pyjamas-rfglab-2024.4.0/
+-rw-r--r--   0 rodrigo    (501) staff       (20)      265 2023-01-17 21:44:31.000000 pyjamas-rfglab-2024.4.0/MANIFEST.in
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1686 2024-04-16 21:39:53.600077 pyjamas-rfglab-2024.4.0/PKG-INFO
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1202 2023-07-11 19:12:22.000000 pyjamas-rfglab-2024.4.0/README.md
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-16 21:39:53.482471 pyjamas-rfglab-2024.4.0/pyjamas/
+-rw-r--r--   0 rodrigo    (501) staff       (20)    33144 2020-02-04 05:51:32.000000 pyjamas-rfglab-2024.4.0/pyjamas/LICENSE
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1088 2020-01-17 04:15:16.000000 pyjamas-rfglab-2024.4.0/pyjamas/__init__.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-16 21:39:53.501663 pyjamas-rfglab-2024.4.0/pyjamas/dialogs/
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1645 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.0/pyjamas/dialogs/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    17593 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.0/pyjamas/dialogs/adjustcontrast.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    31465 2024-03-22 23:06:04.000000 pyjamas-rfglab-2024.4.0/pyjamas/dialogs/batchanalysis.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    12069 2024-04-16 14:02:15.000000 pyjamas-rfglab-2024.4.0/pyjamas/dialogs/batchflatfield.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     5509 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.0/pyjamas/dialogs/batchprojectconcat.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     6823 2024-04-16 14:02:15.000000 pyjamas-rfglab-2024.4.0/pyjamas/dialogs/batchresize.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2980 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.0/pyjamas/dialogs/classifierdialogABC.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3199 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.0/pyjamas/dialogs/classifiertype.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     6437 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.0/pyjamas/dialogs/expandnpropagateseeds.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     5227 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.0/pyjamas/dialogs/expandseeds.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    13000 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.0/pyjamas/dialogs/findseeds.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    11361 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.0/pyjamas/dialogs/logregression.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3453 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.0/pyjamas/dialogs/matplotlibdialog.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     8858 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.0/pyjamas/dialogs/measurepoly.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    13277 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.0/pyjamas/dialogs/neuralnet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     8699 2024-03-12 21:08:54.000000 pyjamas-rfglab-2024.4.0/pyjamas/dialogs/nonmax_suppr.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     5533 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.0/pyjamas/dialogs/propagateseeds.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    14588 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.0/pyjamas/dialogs/rescuneuralnet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    12510 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.0/pyjamas/dialogs/svm.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2243 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.0/pyjamas/dialogs/textdialog.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2817 2023-12-27 20:45:04.000000 pyjamas-rfglab-2024.4.0/pyjamas/dialogs/texteditdialog.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     4082 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.0/pyjamas/dialogs/timepoints.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1806 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.0/pyjamas/dragdropmainwindow.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-16 21:39:53.503857 pyjamas-rfglab-2024.4.0/pyjamas/external/
+-rw-r--r--   0 rodrigo    (501) staff       (20)      899 2021-05-09 22:07:44.000000 pyjamas-rfglab-2024.4.0/pyjamas/external/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     6852 2020-07-11 20:09:58.000000 pyjamas-rfglab-2024.4.0/pyjamas/external/pascal_voc_io.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     4930 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.0/pyjamas/orthogonalviewswindow.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    52457 2024-04-16 14:02:15.000000 pyjamas-rfglab-2024.4.0/pyjamas/pjscore.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    33519 2023-11-22 14:41:28.000000 pyjamas-rfglab-2024.4.0/pyjamas/pjseventfilter.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2123 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.0/pyjamas/pjsthreads.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)  2950837 2023-06-21 15:47:44.000000 pyjamas-rfglab-2024.4.0/pyjamas/pyjamas.tif
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-16 21:39:53.509591 pyjamas-rfglab-2024.4.0/pyjamas/rannotations/
+-rw-r--r--   0 rodrigo    (501) staff       (20)      924 2022-06-20 21:44:00.000000 pyjamas-rfglab-2024.4.0/pyjamas/rannotations/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)      856 2020-01-17 04:15:16.000000 pyjamas-rfglab-2024.4.0/pyjamas/rannotations/rannotation.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    16818 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.0/pyjamas/rannotations/rpolyline.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2288 2022-08-14 20:59:38.000000 pyjamas-rfglab-2024.4.0/pyjamas/rannotations/rvector2d.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-16 21:39:53.533524 pyjamas-rfglab-2024.4.0/pyjamas/rcallbacks/
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1257 2020-01-17 04:15:16.000000 pyjamas-rfglab-2024.4.0/pyjamas/rcallbacks/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     7690 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.0/pyjamas/rcallbacks/rcallback.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1658 2023-02-07 15:13:59.000000 pyjamas-rfglab-2024.4.0/pyjamas/rcallbacks/rcbabout.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    14800 2023-11-02 21:21:06.000000 pyjamas-rfglab-2024.4.0/pyjamas/rcallbacks/rcbannotations.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    82102 2024-04-16 14:02:15.000000 pyjamas-rfglab-2024.4.0/pyjamas/rcallbacks/rcbbatchprocess.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    66584 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.0/pyjamas/rcallbacks/rcbclassifiers.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    77584 2024-03-12 21:08:54.000000 pyjamas-rfglab-2024.4.0/pyjamas/rcallbacks/rcbimage.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    50542 2024-03-01 22:58:24.000000 pyjamas-rfglab-2024.4.0/pyjamas/rcallbacks/rcbio.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    11360 2024-03-12 21:08:54.000000 pyjamas-rfglab-2024.4.0/pyjamas/rcallbacks/rcbmeasure.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    13844 2023-11-22 14:41:28.000000 pyjamas-rfglab-2024.4.0/pyjamas/rcallbacks/rcboptions.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3617 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.0/pyjamas/rcallbacks/rcbplugins.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-16 21:39:53.538001 pyjamas-rfglab-2024.4.0/pyjamas/rimage/
+-rw-r--r--   0 rodrigo    (501) staff       (20)      913 2020-05-28 03:02:49.000000 pyjamas-rfglab-2024.4.0/pyjamas/rimage/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3091 2021-08-22 22:13:16.000000 pyjamas-rfglab-2024.4.0/pyjamas/rimage/csgraph.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3774 2024-03-01 22:58:24.000000 pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimcore.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-16 21:39:53.589079 pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1484 2021-02-14 22:27:21.000000 pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3557 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/batchclassifier.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1585 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/batchml.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2740 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/batchneuralnet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     7409 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/batchrecurrentneuralnet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)      275 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/classifier_types.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1173 2020-08-28 21:52:01.000000 pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/featurecalculator.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1387 2020-12-27 23:49:18.000000 pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/featurecalculator_rawimage.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1289 2020-12-27 23:49:18.000000 pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/featurecalculator_rowofpixels.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3104 2024-03-12 21:08:54.000000 pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/featurecalculator_sog.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    17339 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/rimclassifier.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1824 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/rimlr.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1382 2021-10-27 20:01:04.000000 pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/rimml.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1857 2021-10-27 20:01:04.000000 pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/rimneuralnet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1960 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/rimrecurrentneuralnet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    20979 2023-07-11 19:12:22.000000 pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/rimrescunet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2084 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/rimsvm.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    15508 2023-07-11 19:12:22.000000 pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/rimunet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    69198 2024-03-01 22:58:24.000000 pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimutils.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-16 21:39:53.590678 pyjamas-rfglab-2024.4.0/pyjamas/rplugins/
+-rw-r--r--   0 rodrigo    (501) staff       (20)      847 2020-01-17 04:15:16.000000 pyjamas-rfglab-2024.4.0/pyjamas/rplugins/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1249 2023-02-19 02:47:05.000000 pyjamas-rfglab-2024.4.0/pyjamas/rplugins/base.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    28427 2024-03-14 22:30:31.000000 pyjamas-rfglab-2024.4.0/pyjamas/rutils.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-16 21:39:53.595617 pyjamas-rfglab-2024.4.0/pyjamas/tests/
+-rw-r--r--   0 rodrigo    (501) staff       (20)      796 2023-01-02 00:28:47.000000 pyjamas-rfglab-2024.4.0/pyjamas/tests/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)      857 2023-01-19 20:27:03.000000 pyjamas-rfglab-2024.4.0/pyjamas/tests/conftest.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-16 21:39:53.598859 pyjamas-rfglab-2024.4.0/pyjamas/tests/unit/
+-rw-r--r--   0 rodrigo    (501) staff       (20)        0 2022-12-25 02:03:19.000000 pyjamas-rfglab-2024.4.0/pyjamas/tests/unit/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     7461 2024-04-16 14:02:15.000000 pyjamas-rfglab-2024.4.0/pyjamas/tests/unit/pjsfixtures.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    12484 2023-11-22 14:41:28.000000 pyjamas-rfglab-2024.4.0/pyjamas/tests/unit/test_image.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    16029 2023-12-07 19:48:58.000000 pyjamas-rfglab-2024.4.0/pyjamas/tests/unit/test_io.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-16 21:39:53.599578 pyjamas-rfglab-2024.4.0/pyjamas_rfglab.egg-info/
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2562 2024-04-16 21:39:52.000000 pyjamas-rfglab-2024.4.0/pyjamas_rfglab.egg-info/SOURCES.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)       38 2024-04-16 21:39:53.601119 pyjamas-rfglab-2024.4.0/setup.cfg
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2923 2024-03-12 21:08:54.000000 pyjamas-rfglab-2024.4.0/setup.py
```

### Comparing `pyjamas-rfglab-2024.3.4/PKG-INFO` & `pyjamas-rfglab-2024.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjamas-rfglab
-Version: 2024.3.4
+Version: 2024.4.0
 Summary: PyJAMAS is Just A More Awesome SIESTA
 Home-page: https://bitbucket.org/rfg_lab/pyjamas
 Author: Rodrigo Fernandez-Gonzalez
 Author-email: rodrigo.fernandez.gonzalez@utoronto.ca
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `pyjamas-rfglab-2024.3.4/README.md` & `pyjamas-rfglab-2024.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/LICENSE` & `pyjamas-rfglab-2024.4.0/pyjamas/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/__init__.py` & `pyjamas-rfglab-2024.4.0/pyjamas/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/dialogs/__init__.py` & `pyjamas-rfglab-2024.4.0/pyjamas/dialogs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/dialogs/adjustcontrast.py` & `pyjamas-rfglab-2024.4.0/pyjamas/dialogs/adjustcontrast.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/dialogs/batchanalysis.py` & `pyjamas-rfglab-2024.4.0/pyjamas/dialogs/batchanalysis.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/dialogs/batchprojectconcat.py` & `pyjamas-rfglab-2024.4.0/pyjamas/dialogs/batchprojectconcat.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/dialogs/batchresize.py` & `pyjamas-rfglab-2024.4.0/pyjamas/dialogs/batchresize.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-from typing import List, Optional
+from typing import Optional
 
 from PyQt6 import QtCore, QtWidgets
 
 from pyjamas.rutils import RUtils
 
 
 class BatchResizeDialog(object):
@@ -29,15 +29,14 @@
     recurr: bool = None
     im_size: tuple = None
 
     def __init__(self):
         super().__init__()
 
     def setupUi(self, Dialog, parameters: Optional[dict] = None):
-        from pyjamas.rcallbacks.rcbbatchprocess import RCBBatchProcess
 
         if (parameters is None or parameters is False) and BatchResizeDialog.input_folder is None:
             parameters = {'input_folder': '',
                           'save_folder': '',
                           'recurr': True,
                           'im_size': (512, 512)}
```

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/dialogs/classifierdialogABC.py` & `pyjamas-rfglab-2024.4.0/pyjamas/dialogs/classifierdialogABC.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/dialogs/classifiertype.py` & `pyjamas-rfglab-2024.4.0/pyjamas/dialogs/classifiertype.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/dialogs/expandnpropagateseeds.py` & `pyjamas-rfglab-2024.4.0/pyjamas/dialogs/expandnpropagateseeds.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/dialogs/expandseeds.py` & `pyjamas-rfglab-2024.4.0/pyjamas/dialogs/expandseeds.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/dialogs/findseeds.py` & `pyjamas-rfglab-2024.4.0/pyjamas/dialogs/findseeds.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/dialogs/logregression.py` & `pyjamas-rfglab-2024.4.0/pyjamas/dialogs/logregression.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/dialogs/matplotlibdialog.py` & `pyjamas-rfglab-2024.4.0/pyjamas/dialogs/matplotlibdialog.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/dialogs/measurepoly.py` & `pyjamas-rfglab-2024.4.0/pyjamas/dialogs/measurepoly.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/dialogs/neuralnet.py` & `pyjamas-rfglab-2024.4.0/pyjamas/dialogs/neuralnet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/dialogs/nonmax_suppr.py` & `pyjamas-rfglab-2024.4.0/pyjamas/dialogs/nonmax_suppr.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/dialogs/propagateseeds.py` & `pyjamas-rfglab-2024.4.0/pyjamas/dialogs/propagateseeds.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/dialogs/rescuneuralnet.py` & `pyjamas-rfglab-2024.4.0/pyjamas/dialogs/rescuneuralnet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/dialogs/svm.py` & `pyjamas-rfglab-2024.4.0/pyjamas/dialogs/svm.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/dialogs/textdialog.py` & `pyjamas-rfglab-2024.4.0/pyjamas/dialogs/textdialog.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/dialogs/texteditdialog.py` & `pyjamas-rfglab-2024.4.0/pyjamas/dialogs/texteditdialog.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/dialogs/timepoints.py` & `pyjamas-rfglab-2024.4.0/pyjamas/dialogs/timepoints.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/dragdropmainwindow.py` & `pyjamas-rfglab-2024.4.0/pyjamas/dragdropmainwindow.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/external/__init__.py` & `pyjamas-rfglab-2024.4.0/pyjamas/external/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/external/pascal_voc_io.py` & `pyjamas-rfglab-2024.4.0/pyjamas/external/pascal_voc_io.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/orthogonalviewswindow.py` & `pyjamas-rfglab-2024.4.0/pyjamas/orthogonalviewswindow.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/pjscore.py` & `pyjamas-rfglab-2024.4.0/pyjamas/pjscore.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     livewire_gaussian_sigma: float = 0.
     balloon_crop_size: int = 50  # crop size used to inflate balloons
     livewire_shortest_path_fn = tuple(rimcore.rimage.livewire_shortest_path_fns.values())[0]  # fn to calculate shortest path between two pixels
 
     undo_stack_size: int = 500
 
     # Read version.
-    __version__: str = '2024.3.4'
+    __version__: str = '2024.4.0'
 
     def __init__(self):
         self.initData()  # Initialize object variables.
         self.setupUI()  # Build the GUI.
 
     def setupUI(self):
         self.app = QtWidgets.QApplication(sys.argv)
@@ -574,14 +574,17 @@
         self.addMenuItem(self.menuBatch, "Sum project and concatenate ...", None,
                          partial(self.batch.cbBatchProjectConcat,
                                  projection_type=rcallbacks.rcbimage.projection_types.SUM))
 
         # Resize images.
         self.addMenuItem(self.menuBatch, "Resize images ...", None, self.batch.cbBatchResize)
 
+        # Resize images.
+        self.addMenuItem(self.menuBatch, "Correct images ...", None, self.batch.cbBatchFlatFieldCorrection)
+
         self.menuBatch.addSeparator()
 
         # Measure.
         self.addMenuItem(self.menuBatch, "Measure ...", 'Ctrl+M',
                          self.batch.cbMeasureBatch)
 
         self.menubar.addMenu(self.menuBatch)
```

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/pjseventfilter.py` & `pyjamas-rfglab-2024.4.0/pyjamas/pjseventfilter.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/pjsthreads.py` & `pyjamas-rfglab-2024.4.0/pyjamas/pjsthreads.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/pyjamas.tif` & `pyjamas-rfglab-2024.4.0/pyjamas/pyjamas.tif`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rannotations/__init__.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rannotations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rannotations/rannotation.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rannotations/rannotation.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rannotations/rpolyline.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rannotations/rpolyline.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rannotations/rvector2d.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rannotations/rvector2d.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rcallbacks/__init__.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rcallbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rcallbacks/rcallback.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rcallbacks/rcallback.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rcallbacks/rcbabout.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rcallbacks/rcbabout.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rcallbacks/rcbannotations.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rcallbacks/rcbannotations.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rcallbacks/rcbbatchprocess.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rcallbacks/rcbbatchprocess.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,22 +24,25 @@
 import warnings
 
 import matplotlib.pyplot as plt
 import nbformat as nbf
 from nbformat.notebooknode import NotebookNode
 import numpy
 import pandas as pd
+pd.options.mode.copy_on_write = True  # avoid "setting with copy" warnings: https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#returning-a-view-versus-a-copy
 # import pylustrator
 from PyQt6 import QtWidgets
 import seaborn as sns
 from scipy.optimize import leastsq
+from scipy import stats
 import skimage.io as sio
 import skimage.transform as st
 
 from pyjamas.dialogs.batchanalysis import BatchMeasureDialog
+from pyjamas.dialogs.batchflatfield import BatchFlatFieldCorrectionDialog
 from pyjamas.dialogs.batchresize import BatchResizeDialog
 from pyjamas.dialogs.batchprojectconcat import BatchProjectConcatenateDialog
 from pyjamas.pjscore import PyJAMAS
 from pyjamas.pjsthreads import ThreadSignals
 from pyjamas.rcallbacks.rcallback import RCallback
 from pyjamas.rcallbacks.rcbimage import projection_types
 from pyjamas.rimage.rimutils import rimutils as rimutils
@@ -55,17 +58,25 @@
     BACKGROUND_PHOTOBLEACHING_MEAN_IMAGE: int = 2
     PHOTOBLEACHING_MEAN_SAMPLE: int = 3
     BACKGROUND_PHOTOBLEACHING_MEAN_SAMPLE: int = 4
     BACKGROUND_PHOTOBLEACHING_MEAN_FILE: int = 5
 
 
 class RCBBatchProcess(RCallback):
-    VALID_EXTENSIONS: Tuple[str] = ('.tif', '.tiff')
+    VALID_EXTENSIONS: Tuple[str] = ('.tif', '.tiff', '.TIF', '.TIFF')
     OUTPUT_EXTENSION: str = '.tif'
 
+    FFC_INPUT: str = '.'
+    FFC_DARKFILE: str = ''
+    FFC_FLATFILE: str = ''
+    FFC_CROPDIMS: Tuple[int, int] = (512, 512)
+    FFC_BG: str = 'mode'
+    FFC_INPUTSUBSTR: str = ''
+    FFC_FILESUFFIX: str = '_ffc_corrected'
+
     BATCH_MEASURE_SCRIPT: str = f"import sys\nsys.path.extend(['{PyJAMAS.folder.rstrip('/pyjamas')}'])\nfrom pyjamas.pjscore import PyJAMAS\na = PyJAMAS()\na.batch.cbMeasureBatch(parameters)"
 
     DIRS1_BM: str = '.'
     DIRS2_BM: str = ''
     ANALYZE_FLAG_BM: bool = True
     ANALYSIS_FILENAME_APPENDIX_BM: str = '_analysis'
     ANALYSIS_EXTENSION_BM: str = '.csv'
@@ -167,15 +178,15 @@
             if return_value:
                 self.pjs.cwd = os.path.abspath(theparameters['input_folder'])
 
             return return_value
         else:
             return False
 
-    def cbBatchResize(self, parameters: Optional[dict] = None):
+    def cbBatchResize(self, parameters: Optional[dict] = None) -> bool:
         """
         Resizes all images within a given folder or folder tree to a specified size and saves them to a new folder.
 
         :param parameters: dictionary with parameters, a dialog will open if the value is none.
 
             ``input_folder``: absolute path to the folder containing all images to be resized.
             ``save_folder``: absolute path to the folder that resized images will be saved to.
@@ -209,20 +220,21 @@
             recurr = parameters.get('recurr')
             if save_folder == '':
                 save_folder = input_folder + f"_resized_{im_size[0]}x{im_size[1]}"
             if not os.path.exists(save_folder):
                 os.mkdir(save_folder)
             self.batch_resize_images(input_folder, save_folder, im_size, recurr)
             self.pjs.statusbar.showMessage('Finished.')
+
+            return True
         else:
-            self.pjs.statusbar.showMessage('Error during resizing.')
             return False
 
     def batch_resize_images(self, input_folder: Optional[str] = None, save_folder: Optional[str] = None,
-                            im_size: Optional[tuple] = (512, 512), recurr: Optional[bool] = True):
+                            im_size: Optional[tuple] = (512, 512), recurr: Optional[bool] = True) -> bool:
         for subfile in os.listdir(input_folder):
             subfile_path = os.path.join(input_folder, subfile)
             if os.path.isdir(subfile_path) and recurr:
                 if not os.path.exists(os.path.join(save_folder, subfile)):
                     os.mkdir(os.path.join(save_folder, subfile))
                 self.batch_resize_images(subfile_path, os.path.join(save_folder, subfile), im_size, recurr)
             elif os.path.splitext(subfile_path)[1] == '.tif':
@@ -238,14 +250,205 @@
                     img = numpy.maximum(img, numpy.zeros((im_size[0], im_size[1], 1)))
                 sio.imsave(os.path.join(save_folder, subfile), img[:, :, 0], check_contrast=False)
             else:  # Not an acceptable image type or sub-directory
                 continue
 
         return True
 
+    def cbBatchFlatFieldCorrection(self, parameters: Optional[dict] = None) -> bool:
+        """
+        Flat field correction of all images within a given folder or folder tree.
+
+        :param parameters: dictionary with parameters, a dialog will open if the value is none.
+
+            ``input_folder``: absolute path to the folder containing all images to be resized.
+            ``darkfield_file``: path to the file containing the image to correct for darkfield, '' or None of no darkfield correction.
+            ``flatfield_file``: path to the file containing the image to correct for flatfield, '' or None of no flatfield correction.
+            ``crop_dims``: tuple with (row, col) dimensions to crop the images before applying any corrections, None for no cropping.
+            ``bg_mode``: background subtraction, None if no background subtraction, 'mode' if the background is the volume mode.
+            ``input_substr``: substring to refine input files corrected, '' to correct all images.
+            ``file_suffix``: suffix to add to the file name of the corrected images.
+
+        :return: True if resizing complete, False otherwise.
+        """
+        # Get folder name.
+        continue_flag: bool = True
+
+        if parameters is None or parameters is False:
+            dialog = QtWidgets.QDialog()
+            ui = BatchFlatFieldCorrectionDialog()
+            ui.setupUi(dialog)
+
+            dialog.exec()
+            dialog.show()
+
+            continue_flag = dialog.result() == QtWidgets.QDialog.DialogCode.Accepted
+
+            if continue_flag:
+                parameters = ui.parameters()
+
+            dialog.close()
+
+        if continue_flag:
+            input_folder = parameters.get('input_folder')
+            darkfield_file = parameters.get('darkfield_file')
+            flatfield_file = parameters.get('flatfield_file')
+            crop_dims = parameters.get('crop_dims')
+            bg_mode = parameters.get('bg_mode')
+            input_substr = parameters.get('input_substr')
+            file_suffix = parameters.get('file_suffix')
+
+            self.batch_correct_images(input_folder, darkfield_file, flatfield_file, crop_dims, bg_mode, input_substr,
+                                      file_suffix)
+            self.pjs.statusbar.showMessage('Finished.')
+
+            return True
+        else:
+            return False
+
+    def batch_correct_images(self, input_folder: Optional[str] = None, darkfield_file: Optional[str] = None,
+                             flatfield_file: Optional[str] = None, crop_dims: Optional[tuple] = FFC_CROPDIMS,
+                             bg_mode: Optional[str] = None, input_substr: Optional[str] = FFC_INPUTSUBSTR,
+                             file_suffix: Optional[str] = FFC_FILESUFFIX):
+        ffc_corr: bool = False
+        dark_corr: bool = False
+        crop_flag: bool = False
+        crop_start_rows: int = -1
+        crop_start_cols: int = -1
+        nrows: int = -1  # number of rows to crop
+        ncols: int = -1  # number of cols to crop
+
+        if os.path.exists(flatfield_file):
+            ffc_img = rimutils.read_stack(flatfield_file)
+
+            # The images to be corrected will be divided by this one. Thus, there should be no zeros.
+            if numpy.any(numpy.isclose(ffc_img, 0.)):
+                print(f'The image in {flatfield_file} contains zeros and therefore is not a valid flat field image.')
+                return False
+
+            ffc_corr = True
+
+        if os.path.exists(darkfield_file):
+            dark_img = rimutils.read_stack(darkfield_file).astype(numpy.float32)
+            dark_corr = True
+
+        if crop_dims is not None and len(crop_dims) == 2:
+            nrows = crop_dims[0]
+            ncols = crop_dims[1]
+            if ffc_corr:
+                crop_start_rows = int((ffc_img.shape[0] - nrows) / 2)
+                crop_start_cols = int((ffc_img.shape[1] - ncols) / 2)
+                ffc_img = ffc_img[crop_start_rows:crop_start_rows + nrows, crop_start_cols:crop_start_cols + ncols]
+            if dark_corr:
+                if crop_start_rows == -1:
+                    crop_start_rows = int((dark_img.shape[0] - nrows) / 2)
+                    crop_start_cols = int((dark_img.shape[1] - ncols) / 2)
+                dark_img = dark_img[crop_start_rows:crop_start_rows + nrows, crop_start_cols:crop_start_cols + ncols]
+            crop_flag = True
+        else:
+            crop_start_rows = 0
+            crop_start_cols = 0
+
+            if ffc_corr:
+                nrows = ffc_img.shape[0]
+                ncols = ffc_img.shape[1]
+            elif dark_corr:
+                nrows = dark_img.shape[0]
+                ncols = dark_img.shape[1]
+            else:
+                print(f'Nothing to do.')
+                return False
+
+        if file_suffix == '':
+            thenow = datetime.now()
+            thesuffix = thenow.strftime(
+                f"{thenow.year:04}{thenow.month:02}{thenow.day:02}_{thenow.hour:02}{thenow.minute:02}{thenow.second:02}")
+            file_suffix = f'_{thesuffix}'
+
+        file_list: List[str] = RUtils.extract_file_paths(input_folder, self.VALID_EXTENSIONS)
+
+        for file_path in file_list:
+            folder_name, full_file_name = os.path.split(file_path)
+            file_name, ext = os.path.splitext(full_file_name)
+
+            if input_substr in file_name:
+                img = rimutils.read_stack(file_path)
+
+                if crop_flag and crop_start_rows == -1:
+                    crop_start_rows = int((img.shape[1] - nrows) / 2)
+                    crop_start_cols = int((img.shape[2] - ncols) / 2)
+
+                new_img: numpy.ndarray = numpy.empty((img.shape[0], nrows, ncols), dtype=float)
+
+                for anindex, aslice in enumerate(img):
+                    tmp_img: numpy.ndarray = aslice.copy()
+
+                    if crop_flag and nrows < tmp_img.shape[0] and ncols < tmp_img.shape[1]:
+                        tmp_img = tmp_img[crop_start_rows:crop_start_rows + nrows,
+                                  crop_start_cols:crop_start_cols + ncols]
+
+                    if dark_corr:
+                        tmp_img = numpy.clip(tmp_img - dark_img, 0, None)
+
+                    if ffc_corr:
+                        tmp_img = tmp_img / ffc_img
+
+                        ## This code here deals with nan's. We are not using this because the function returns an
+                        ## error if the ffc_image contains 0s.
+                        # # need to deal with pixels that are nan after being divided by zero ... usic cubic interpolation.
+                        # # this should not run if the ffc image does not have zero values.
+                        # x = numpy.arange(0, tmp_img.shape[1])
+                        # y = numpy.arange(0, tmp_img.shape[0])
+                        # xx, yy = numpy.meshgrid(x, y)
+                        # # mask invalid values
+                        # masked_img = numpy.ma.masked_invalid(tmp_img)
+                        #
+                        # # get coordinates with valid/invalid values
+                        # x_invalid = xx[masked_img.mask]
+                        #
+                        # if x_invalid.size > 0:
+                        #     print(
+                        #         f'WARNING: {x_invalid.size} pixels divided by zero in flat field correction of slice {anindex} in {afile}.')
+                        #
+                        #     y_invalid = yy[masked_img.mask]
+                        #     x_valid = xx[~masked_img.mask]
+                        #     y_valid = yy[~masked_img.mask]
+                        #
+                        #     valid_array = masked_img.data[~masked_img.mask]
+                        #
+                        #     interp_values = interpolate.griddata((x_valid, y_valid), valid_array.ravel(),
+                        #                                          (x_invalid, y_invalid), method='cubic')
+                        #
+                        #     tmp_img[y_invalid, x_invalid] = interp_values
+
+                    new_img[anindex, :, :] = tmp_img.copy()
+
+                match bg_mode:
+                    case 'mode':
+                        stack_mode = stats.mode(new_img.reshape(-1))[0]
+                        new_img = numpy.clip(new_img - stack_mode, 0, None)
+
+                corrected_file_path = os.path.join(folder_name, file_name+file_suffix+ext)
+                rimutils.write_stack(corrected_file_path, new_img.astype(numpy.uint16))
+
+        return True
+
+    @classmethod
+    def _default_batchflatfield_parameters(cls) -> dict:
+        return {
+            'input_folder': RCBBatchProcess.FFC_INPUT,
+            'darkfield_file': RCBBatchProcess.FFC_DARKFILE,
+            'flatfield_file': RCBBatchProcess.FFC_FLATFILE,
+            'crop_dims': RCBBatchProcess.FFC_CROPDIMS,
+            'bg_mode': RCBBatchProcess.FFC_BG,
+            'input_substr': RCBBatchProcess.FFC_INPUTSUBSTR,
+            'file_suffix': RCBBatchProcess.FFC_FILESUFFIX
+        }
+
+
     def cbMeasureBatch(self, parameters: Optional[dict] = None) -> bool:
         """
         Measures image data sets and produces plots and CSV files that combine all the data. A Python script to reproduce the analysis, and a Jupyter notebook to reproduce the analysis and generate the plots can also be generated.
 
         :param parameters: dictionary containing measurement parameters; a dialog will open if the value is set to None; dictionary keys are:
 
             ``folders``:
@@ -607,118 +810,127 @@
 
             # min_ind and max_ind delimit the rows in all_data that correspond to the time points for the current folder.
             min_ind = max_ind
             max_ind = min_ind + self.ntp
 
             # Determine both the experimental group and the experiment index within that group.
             dirs_group = [annotations_file in this_dir for this_dir in self.dirs].index(True)
-            all_data['experimental group'].iloc[min_ind:max_ind] = self.group_labels[dirs_group]
-            all_data['experiment index'].iloc[min_ind:max_ind] = self.dirs[dirs_group].index(annotations_file)
+            all_data.iloc[min_ind:max_ind, all_data.columns.get_loc('experimental group')] = self.group_labels[dirs_group]  # this triggers a copy of a slice warning: all_data['experimental group'].iloc[min_ind:max_ind] = self.group_labels[dirs_group]
+            all_data.iloc[min_ind:max_ind, all_data.columns.get_loc('experiment index')] = self.dirs[dirs_group].index(annotations_file)
 
-            all_data['time (min)'].values[min_ind + index_list] = self.t[0:index_list.size]
-            all_data['file name'].iloc[min_ind:max_ind] = full_analysis_file_name
+            all_data.iloc[min_ind+index_list, all_data.columns.get_loc('time (min)')] = self.t[0:index_list.size]
+            all_data.iloc[min_ind:max_ind, all_data.columns.get_loc('file name')] = full_analysis_file_name
 
             # REMEMBER: index_list is an ndarray with the relative indexes to use.
-            all_data['area (\u03BCm\u00B2)'].values[min_ind + index_list] = numpy.asarray(msr_df.loc['area_1']) * (
+            all_data.iloc[min_ind+index_list, all_data.columns.get_loc('area (\u03BCm\u00B2)')] = numpy.asarray(msr_df.loc['area_1']) * (
                     self.xy_res ** 2)
 
-            areas = all_data['area (\u03BCm\u00B2)'].values[min_ind + index_list]
-            times = all_data['time (min)'].values[min_ind + index_list]
+            areas = all_data['area (\u03BCm\u00B2)'].values[min_ind+index_list]
+            times = all_data['time (min)'].values[min_ind+index_list]
             max_area_ind = numpy.argmax(areas)
 
             # Fits exponential from maximum (if there are at least 3 time points).
             if areas.size >= 3 and areas[max_area_ind:].size >= 3:
                 x, flag = leastsq(RUtils.residuals, (areas[max_area_ind], 1.0),
                                   args=(RUtils.func_exp_2params, areas[max_area_ind:], times[max_area_ind:]))
 
                 # Verify fits.
                 # plt.figure()
                 # ax = sns.lineplot(x=times, y=areas)
                 # ax = sns.lineplot(x=times[max_area_ind:], y=RUtils.func_exp_2params(times[max_area_ind:], x), marker="o")
                 # r, p = numpy.corrcoef(areas[max_area_ind:], RUtils.func_exp_2params(times[max_area_ind:], x))
-                all_data['closure rate constant - area (1/min)'].values[min_ind + index_list] = 1./x[1]
 
+                if flag == 1:
+                    all_data.iloc[min_ind+index_list, all_data.columns.get_loc('closure rate constant - area (1/min)')] = 1./x[1]
+                else:
+                    print(f"WARNING: could not fit an exponential to the area data for {annotations_file}.")
+                    all_data.iloc[
+                        min_ind + index_list, all_data.columns.get_loc('closure rate constant - area (1/min)')] = numpy.nan
             else:
                 self.box_plot_measurements.pop(self.box_plot_measurements.index('closure rate constant - area (1/min)'))
 
             mean_area_beg: float = numpy.nanmean(numpy.asarray(msr_df.loc['area_1'])[0:self.index_time_zero])
             mean_area_end: float = numpy.nanmean(numpy.asarray(msr_df.loc['area_1'][-self.index_time_zero:]))
 
-            all_data['area (%)'].values[min_ind + index_list] = 100. * numpy.asarray(
+            all_data.iloc[min_ind+index_list, all_data.columns.get_loc('area (%)')] = 100. * numpy.asarray(
                 msr_df.loc['area_1']) / mean_area_beg
 
-            all_data['area (% change)'].values[min_ind + index_list] = 100. * (
+            all_data.iloc[min_ind+index_list, all_data.columns.get_loc('area (% change)')] = 100. * (
                     mean_area_end - mean_area_beg) / mean_area_beg
 
-            all_data['perimeter (\u03BCm)'].values[min_ind + index_list] = numpy.asarray(
+            all_data.iloc[min_ind+index_list, all_data.columns.get_loc('perimeter (\u03BCm)')] = numpy.asarray(
                 msr_df.loc['perimeter_1']) * self.xy_res
 
-            perimeters = all_data['perimeter (\u03BCm)'].values[min_ind + index_list]
+            perimeters = all_data['perimeter (\u03BCm)'].values[min_ind+index_list]
             max_perimeter_ind = numpy.argmax(perimeters)
 
             # Fits exponential from maximum (if there are at least 3 time points).
             if perimeters.size >= 3 and perimeters[max_perimeter_ind:].size >= 3:
                 x, flag = leastsq(RUtils.residuals, (perimeters[max_perimeter_ind], 1.0),
                                   args=(RUtils.func_exp_2params, perimeters[max_perimeter_ind:], times[max_perimeter_ind:]))
 
                 # Verify fits.
                 # plt.figure()
                 # ax = sns.lineplot(x=times, y=areas)
                 # ax = sns.lineplot(x=times[max_area_ind:], y=RUtils.func_exp_2params(times[max_area_ind:], x), marker="o")
                 # r, p = numpy.corrcoef(areas[max_area_ind:], RUtils.func_exp_2params(times[max_area_ind:], x))
-                all_data['closure rate constant - perimeter (1/min)'].values[min_ind + index_list] = 1./x[1]
-
+                if flag == 1:
+                    all_data.iloc[min_ind+index_list, all_data.columns.get_loc('closure rate constant - perimeter (1/min)')] = 1./x[1]
+                else:
+                    print(f"WARNING: could not fit an exponential to the perimeter data for {annotations_file}.")
+                    all_data.iloc[min_ind + index_list, all_data.columns.get_loc(
+                        'closure rate constant - perimeter (1/min)')] = numpy.nan
             else:
                 self.box_plot_measurements.pop(self.box_plot_measurements.index('closure rate constant - perimeter (1/min)'))
 
             mean_perimeter_beg: float = numpy.nanmean(numpy.asarray(msr_df.loc['perimeter_1'])[0:self.index_time_zero])
             mean_perimeter_end: float = numpy.nanmean(numpy.asarray(msr_df.loc['perimeter_1'][-self.index_time_zero:]))
 
-            all_data['perimeter (%)'].values[min_ind + index_list] = 100. * numpy.asarray(
+            all_data.iloc[min_ind+index_list, all_data.columns.get_loc('perimeter (%)')] = 100. * numpy.asarray(
                 msr_df.loc['perimeter_1']) / mean_perimeter_beg
-            all_data['perimeter (% change)'].values[min_ind + index_list] = 100. * (
+            all_data.iloc[min_ind+index_list, all_data.columns.get_loc('perimeter (% change)')] = 100. * (
                     mean_perimeter_end - mean_perimeter_beg) / mean_perimeter_beg
 
             mean_circularity_beg: float = numpy.nanmean(
                 numpy.asarray(msr_df.loc['area_1'])[0:self.index_time_zero] * (self.xy_res ** 2) / (
                         numpy.asarray(msr_df.loc['perimeter_1'])[
                         0:self.index_time_zero] * self.xy_res))
             mean_circularity_end: float = numpy.nanmean(
                 numpy.asarray(msr_df.loc['area_1'])[-self.index_time_zero] * (self.xy_res ** 2) / (
                         numpy.asarray(msr_df.loc['perimeter_1'])[
                         -self.index_time_zero:] * self.xy_res))
 
-            all_data['circularity (%)'].values[min_ind + index_list] = 100. * (
+            all_data.iloc[min_ind+index_list, all_data.columns.get_loc('circularity (%)')] = 100. * (
                     all_data['area (\u03BCm\u00B2)'].values[
-                        min_ind + index_list] /
+                        min_ind+index_list] /
                     all_data['perimeter (\u03BCm)'].values[
-                        min_ind + index_list]) / mean_circularity_beg
+                        min_ind+index_list]) / mean_circularity_beg
 
-            all_data['circularity (% change)'].values[min_ind + index_list] = 100. * (
+            all_data.iloc[min_ind+index_list, all_data.columns.get_loc('circularity (% change)')] = 100. * (
                     mean_circularity_end - mean_circularity_beg) / mean_circularity_beg
 
-            all_data['raw pixel values interior'].values[min_ind + index_list] = numpy.asarray(
+            all_data.iloc[min_ind+index_list, all_data.columns.get_loc('raw pixel values interior')] = numpy.asarray(
                 msr_df.loc['pixel_values_interior_1'])
-            all_data['raw pixel values interior (%)'].values[min_ind + index_list] = 100. * numpy.asarray(
+            all_data.iloc[min_ind+index_list, all_data.columns.get_loc('raw pixel values interior (%)')] = 100. * numpy.asarray(
                 msr_df.loc['pixel_values_interior_1']) / numpy.nanmean(
                 numpy.asarray(msr_df.loc['pixel_values_interior_1'])[0:self.index_time_zero])
 
-            all_data['raw pixel values perimeter'].values[min_ind + index_list] = numpy.asarray(
+            all_data.iloc[min_ind+index_list, all_data.columns.get_loc('raw pixel values perimeter')] = numpy.asarray(
                 msr_df.loc['pixel_values_perimeter_1'])
-            all_data['raw pixel values perimeter (%)'].values[min_ind + index_list] = 100. * numpy.asarray(
+            all_data.iloc[min_ind+index_list, all_data.columns.get_loc('raw pixel values perimeter (%)')] = 100. * numpy.asarray(
                 msr_df.loc['pixel_values_perimeter_1']) / numpy.nanmean(
                 numpy.asarray(msr_df.loc['pixel_values_perimeter_1'])[0:self.index_time_zero])
 
-            all_data['std interior'].values[min_ind + index_list] = numpy.asarray(
+            all_data.iloc[min_ind+index_list, all_data.columns.get_loc('std interior')] = numpy.asarray(
                 msr_df.loc['std_interior_1'])
-            all_data['std perimeter'].values[min_ind + index_list] = numpy.asarray(
+            all_data.iloc[min_ind+index_list, all_data.columns.get_loc('std perimeter')] = numpy.asarray(
                 msr_df.loc['std_perimeter_1'])
 
-            all_data['image mean'].values[min_ind + index_list] = numpy.asarray(msr_df.loc['image_mean'])
-            all_data['image mode'].values[min_ind + index_list] = numpy.asarray(msr_df.loc['image_mode'])
+            all_data.iloc[min_ind+index_list, all_data.columns.get_loc('image mean')] = numpy.asarray(msr_df.loc['image_mean'])
+            all_data.iloc[min_ind+index_list, all_data.columns.get_loc('image mode')] = numpy.asarray(msr_df.loc['image_mode'])
 
         all_data['circularity (dimensionless)'] = 4 * numpy.pi * all_data['area (\u03BCm\u00B2)'].values / numpy.square(
             all_data['perimeter (\u03BCm)'].values)
 
         if self.normalize_intensity_flag == normalization_modes.RAW_INTENSITIES:
             all_data['normalized pixel values interior'] = all_data['raw pixel values interior'].values
             all_data['normalized pixel values perimeter'] = all_data['raw pixel values perimeter'].values
```

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rcallbacks/rcbclassifiers.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rcallbacks/rcbclassifiers.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rcallbacks/rcbimage.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rcallbacks/rcbimage.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rcallbacks/rcbio.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rcallbacks/rcbio.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rcallbacks/rcbmeasure.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rcallbacks/rcbmeasure.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rcallbacks/rcboptions.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rcallbacks/rcboptions.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rcallbacks/rcbplugins.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rcallbacks/rcbplugins.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rimage/__init__.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rimage/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rimage/csgraph.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rimage/csgraph.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimcore.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimcore.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/__init__.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/batchclassifier.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/batchclassifier.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/batchml.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/batchml.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/batchneuralnet.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/batchneuralnet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/batchrecurrentneuralnet.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/batchrecurrentneuralnet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/featurecalculator.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/featurecalculator.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/featurecalculator_rawimage.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/featurecalculator_rawimage.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/featurecalculator_rowofpixels.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/featurecalculator_rowofpixels.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/featurecalculator_sog.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/featurecalculator_sog.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/rimclassifier.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/rimclassifier.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/rimlr.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/rimlr.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/rimml.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/rimml.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/rimneuralnet.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/rimneuralnet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/rimrecurrentneuralnet.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/rimrecurrentneuralnet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/rimrescunet.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/rimrescunet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/rimsvm.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/rimsvm.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimml/rimunet.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimml/rimunet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rimage/rimutils.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rimage/rimutils.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rplugins/__init__.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rplugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rplugins/base.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rplugins/base.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/rutils.py` & `pyjamas-rfglab-2024.4.0/pyjamas/rutils.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/tests/__init__.py` & `pyjamas-rfglab-2024.4.0/pyjamas/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/tests/conftest.py` & `pyjamas-rfglab-2024.4.0/pyjamas/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/tests/unit/pjsfixtures.py` & `pyjamas-rfglab-2024.4.0/pyjamas/tests/unit/pjsfixtures.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os.path
-from typing import Tuple
+from typing import List, Tuple
 
 import cv2
 import numpy
 import pytest
 import skimage
 
 FIXTURE_DIR: str = '/Users/rodrigo/src/pyjamas_dev/pyjamas/tests/unit/fixtures/'
@@ -45,15 +45,22 @@
 FINDSEEDS_ANNOTATIONSPATH: str = 'fiducials_sigma2_window16_closings2_mindist3.pjs'
 PROPAGATESEEDS_ANNOTATIONSPATH: str = 'propagatedfiducials_sigma2_window16_closings2_mindist3.pjs'
 PROPAGATESEEDS0_ANNOTATIONSPATH: str = 'propagatedfiducials0_sigma2_window16_closings2_mindist3.pjs'
 EXPANDSEEDS_ANNOTATIONSPATH: str = 'expandedfiducials_sigma2_window16_closings2_mindist3.pjs'
 EXPANDNPROPAGATESEEDS_ANNOTATIONSPATH: str = 'expandedpropagatedfiducials_sigma2_window16_closings2_mindist3.pjs'
 PROJECT_CONCAT_DIR: str = 'projcat'
 TMP_PROJCAT_FILE: str = 'projcat.tif'
-
+BATCH_MEASURE_DIR: str = 'batch_measure/results'
+BATCH_FLATFIELD_DIR: str = 'batch_ffc/images_for_correction'
+BATCH_FLATFIELD_OUTPUTDIR: str = 'batch_ffc/corrected_images'
+BATCH_FLATFIELD_FLATFIELDIMAGEPATH: str = 'batch_ffc/ffc_image.tif'
+BATCH_FLATFIELD_DARKIMAGEPATH: str = 'batch_ffc/dark_field_image.tif'
+BATCH_FLATFIELD_SUBSTR: str = ''
+BATCH_FLATFIELD_FILESUFFIX: str = '_ffc_corrected'
+BATCH_FLATFIELD_CROPDIMS: Tuple[int, int] = (512, 512)
 @pytest.fixture
 def image_fixture():
     return skimage.io.imread(os.path.join(FIXTURE_DIR, IMAGE_FIXTURE))
 
 
 @pytest.fixture
 def display_fixture():
@@ -220,7 +227,24 @@
 def expandnpropagateseeds_parameters():
     return 1, 20, FINDSEEDS_SIGMA, FINDSEEDS_WINDOWSIZE
 
 
 @pytest.fixture
 def projcatfolder_fixture():
     return os.path.join(FIXTURE_DIR, PROJECT_CONCAT_DIR)
+
+
+@pytest.fixture
+def batchmeasurefolder_fixture():
+    return os.path.join(FIXTURE_DIR, BATCH_MEASURE_DIR)
+
+@pytest.fixture
+def fieldcorrection_fixture():
+    return {'input_folder': os.path.join(FIXTURE_DIR, BATCH_FLATFIELD_DIR),
+            'darkfield_file': os.path.join(FIXTURE_DIR, BATCH_FLATFIELD_DARKIMAGEPATH),
+            'flatfield_file': os.path.join(FIXTURE_DIR, BATCH_FLATFIELD_FLATFIELDIMAGEPATH),
+            'crop_dims': BATCH_FLATFIELD_CROPDIMS,
+            'file_suffix': BATCH_FLATFIELD_FILESUFFIX,
+            'input_substr': BATCH_FLATFIELD_SUBSTR,
+            'output_folder': os.path.join(FIXTURE_DIR, BATCH_FLATFIELD_OUTPUTDIR)
+            }
+
```

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/tests/unit/test_image.py` & `pyjamas-rfglab-2024.4.0/pyjamas/tests/unit/test_image.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas/tests/unit/test_io.py` & `pyjamas-rfglab-2024.4.0/pyjamas/tests/unit/test_io.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.3.4/pyjamas_rfglab.egg-info/SOURCES.txt` & `pyjamas-rfglab-2024.4.0/pyjamas_rfglab.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 pyjamas/pjseventfilter.py
 pyjamas/pjsthreads.py
 pyjamas/pyjamas.tif
 pyjamas/rutils.py
 pyjamas/dialogs/__init__.py
 pyjamas/dialogs/adjustcontrast.py
 pyjamas/dialogs/batchanalysis.py
+pyjamas/dialogs/batchflatfield.py
 pyjamas/dialogs/batchprojectconcat.py
 pyjamas/dialogs/batchresize.py
 pyjamas/dialogs/classifierdialogABC.py
 pyjamas/dialogs/classifiertype.py
 pyjamas/dialogs/expandnpropagateseeds.py
 pyjamas/dialogs/expandseeds.py
 pyjamas/dialogs/findseeds.py
```

### Comparing `pyjamas-rfglab-2024.3.4/setup.py` & `pyjamas-rfglab-2024.4.0/setup.py`

 * *Files identical despite different names*

