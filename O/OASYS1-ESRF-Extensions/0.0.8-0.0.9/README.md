# Comparing `tmp/OASYS1-ESRF-Extensions-0.0.8.tar.gz` & `tmp/OASYS1-ESRF-Extensions-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/OASYS1-ESRF-Extensions-0.0.8.tar", last modified: Tue Oct 13 15:24:26 2020, max compression
+gzip compressed data, was "dist/OASYS1-ESRF-Extensions-0.0.9.tar", last modified: Fri Oct 16 14:51:12 2020, max compression
```

## Comparing `OASYS1-ESRF-Extensions-0.0.8.tar` & `OASYS1-ESRF-Extensions-0.0.9.tar`

### file list

```diff
@@ -1,118 +1,120 @@
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/
--rw-r--r--   0 srio      (4230) soft      (3401)     1071 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/LICENSE
--rw-r--r--   0 srio      (4230) soft      (3401)      602 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/MANIFEST.in
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/OASYS1_ESRF_Extensions.egg-info/
--rw-r--r--   0 srio      (4230) soft      (3401)     2590 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/OASYS1_ESRF_Extensions.egg-info/PKG-INFO
--rw-r--r--   0 srio      (4230) soft      (3401)     3879 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/OASYS1_ESRF_Extensions.egg-info/SOURCES.txt
--rw-r--r--   0 srio      (4230) soft      (3401)        1 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/OASYS1_ESRF_Extensions.egg-info/dependency_links.txt
--rw-r--r--   0 srio      (4230) soft      (3401)      768 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/OASYS1_ESRF_Extensions.egg-info/entry_points.txt
--rw-r--r--   0 srio      (4230) soft      (3401)      379 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/OASYS1_ESRF_Extensions.egg-info/namespace_packages.txt
--rw-r--r--   0 srio      (4230) soft      (3401)        1 2020-10-13 15:19:15.000000 OASYS1-ESRF-Extensions-0.0.8/OASYS1_ESRF_Extensions.egg-info/not-zip-safe
--rw-r--r--   0 srio      (4230) soft      (3401)       25 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/OASYS1_ESRF_Extensions.egg-info/requires.txt
--rw-r--r--   0 srio      (4230) soft      (3401)       14 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/OASYS1_ESRF_Extensions.egg-info/top_level.txt
--rw-r--r--   0 srio      (4230) soft      (3401)     2590 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/PKG-INFO
--rw-r--r--   0 srio      (4230) soft      (3401)     1503 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/README.md
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/
--rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/
--rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/menu/
--rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/menu/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/oasys/
--rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/oasys/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/oasys/widgets/
--rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/oasys/widgets/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/oasys/widgets/extension/
--rw-r--r--   0 srio      (4230) soft      (3401)      181 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/oasys/widgets/extension/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/oasys/widgets/extension/icons/
--rw-r--r--   0 srio      (4230) soft      (3401)   300738 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/oasys/widgets/extension/icons/esrf2.png
--rw-r--r--   0 srio      (4230) soft      (3401)    23757 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/oasys/widgets/extension/icons/surface_merger.png
--rw-r--r--   0 srio      (4230) soft      (3401)    21241 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/oasys/widgets/extension/ow_surface_file_merger.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/
--rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/util/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/util/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)    11082 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/util/python_script.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/widgets/
--rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/widgets/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/widgets/extension/
--rw-r--r--   0 srio      (4230) soft      (3401)      188 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/widgets/extension/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/widgets/extension/icons/
--rw-r--r--   0 srio      (4230) soft      (3401)    34177 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/widgets/extension/icons/caustic.png
--rw-r--r--   0 srio      (4230) soft      (3401)   451995 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/widgets/extension/icons/esrf.png
--rw-r--r--   0 srio      (4230) soft      (3401)   300738 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/widgets/extension/icons/esrf2.png
--rw-r--r--   0 srio      (4230) soft      (3401)     9813 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/widgets/extension/icons/python_script.png
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/widgets/extension/miscellanea/
--rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/widgets/extension/miscellanea/test_first_widget.txt
--rw-r--r--   0 srio      (4230) soft      (3401)     8848 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/widgets/extension/ow_als_caustic.py
--rwxr-xr-x   0 srio      (4230) soft      (3401)    22757 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/widgets/extension/ow_shadow_python_script.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/widgets/gui/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/widgets/gui/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)     4220 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/widgets/gui/plots.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/srw/
--rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/srw/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/srw/util/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/srw/util/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/srw/widgets/
--rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/srw/widgets/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/srw/widgets/extension/
--rw-r--r--   0 srio      (4230) soft      (3401)      175 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/srw/widgets/extension/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/srw/widgets/extension/icons/
--rw-r--r--   0 srio      (4230) soft      (3401)   300738 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/srw/widgets/extension/icons/esrf2.png
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/syned/
--rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/syned/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/syned/util/
--rw-r--r--   0 srio      (4230) soft      (3401)    19863 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/syned/util/FEA_File.py
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/syned/util/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/syned/widgets/
--rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/syned/widgets/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/syned/widgets/extension/
--rw-r--r--   0 srio      (4230) soft      (3401)      196 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/syned/widgets/extension/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/syned/widgets/extension/icons/
--rw-r--r--   0 srio      (4230) soft      (3401)   300738 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/syned/widgets/extension/icons/esrf2.png
--rw-r--r--   0 srio      (4230) soft      (3401)    82709 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/syned/widgets/extension/icons/hhlo.png
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/syned/widgets/extension/misc/
--rw-r--r--   0 srio      (4230) soft      (3401)    24524 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/syned/widgets/extension/misc/finite_element_usage.png
--rw-r--r--   0 srio      (4230) soft      (3401)    27860 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/syned/widgets/extension/ow_esrf_finite_element_reader.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/util/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/util/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)     1283 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/util/esrf_util.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/util/gui/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/util/gui/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)    19268 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/util/gui/ow_esrf_widget.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/wofry/
--rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/wofry/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/wofry/util/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/wofry/util/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/wofry/widgets/
--rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/wofry/widgets/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/wofry/widgets/extension/
--rw-r--r--   0 srio      (4230) soft      (3401)      178 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/wofry/widgets/extension/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/wofry/widgets/extension/icons/
--rw-r--r--   0 srio      (4230) soft      (3401)   196722 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/wofry/widgets/extension/icons/esrf2.png
--rw-r--r--   0 srio      (4230) soft      (3401)     6049 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/wofry/widgets/extension/icons/lens.png
--rw-r--r--   0 srio      (4230) soft      (3401)    41557 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/wofry/widgets/extension/ow_lens_1D.py
--rw-r--r--   0 srio      (4230) soft      (3401)    19459 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/wofry/widgets/extension/ow_refractive_corrector_1D.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/
--rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/util/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/util/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/
--rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/extension/
--rw-r--r--   0 srio      (4230) soft      (3401)    29509 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/extension/ID19AttenuatorsBox.py
--rw-r--r--   0 srio      (4230) soft      (3401)    18914 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/extension/Monochromator.py
--rw-r--r--   0 srio      (4230) soft      (3401)    18710 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/extension/Scintillator.py
--rw-r--r--   0 srio      (4230) soft      (3401)    17190 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/extension/Transfocator.py
--rw-r--r--   0 srio      (4230) soft      (3401)    17078 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/extension/Transfocator_test.py
--rw-r--r--   0 srio      (4230) soft      (3401)      180 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/extension/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/extension/icons/
--rw-r--r--   0 srio      (4230) soft      (3401)   300738 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/extension/icons/esrf2.png
--rw-r--r--   0 srio      (4230) soft      (3401)     9405 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/extension/icons/id19_attenuator.png
--rw-r--r--   0 srio      (4230) soft      (3401)    46639 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/extension/icons/id19_monochromator.png
--rw-r--r--   0 srio      (4230) soft      (3401)    34373 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/extension/icons/id19_scintillator.png
--rw-r--r--   0 srio      (4230) soft      (3401)    15141 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/extension/icons/id19_trasnfocator.png
--rw-r--r--   0 srio      (4230) soft      (3401)    31892 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/extension/icons/ws_id19_hpw150.png
--rw-r--r--   0 srio      (4230) soft      (3401)    14975 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/extension/wsID19.py
--rw-r--r--   0 srio      (4230) soft      (3401)       38 2020-10-13 15:24:26.000000 OASYS1-ESRF-Extensions-0.0.8/setup.cfg
--rw-r--r--   0 srio      (4230) soft      (3401)     4617 2020-10-13 15:24:17.000000 OASYS1-ESRF-Extensions-0.0.8/setup.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/
+-rw-r--r--   0 srio      (4230) soft      (3401)     1071 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/LICENSE
+-rw-r--r--   0 srio      (4230) soft      (3401)      602 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/MANIFEST.in
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/OASYS1_ESRF_Extensions.egg-info/
+-rw-r--r--   0 srio      (4230) soft      (3401)     2590 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/OASYS1_ESRF_Extensions.egg-info/PKG-INFO
+-rw-r--r--   0 srio      (4230) soft      (3401)     4010 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/OASYS1_ESRF_Extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 srio      (4230) soft      (3401)        1 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/OASYS1_ESRF_Extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 srio      (4230) soft      (3401)      768 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/OASYS1_ESRF_Extensions.egg-info/entry_points.txt
+-rw-r--r--   0 srio      (4230) soft      (3401)      379 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/OASYS1_ESRF_Extensions.egg-info/namespace_packages.txt
+-rw-r--r--   0 srio      (4230) soft      (3401)        1 2020-10-13 15:19:15.000000 OASYS1-ESRF-Extensions-0.0.9/OASYS1_ESRF_Extensions.egg-info/not-zip-safe
+-rw-r--r--   0 srio      (4230) soft      (3401)       25 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/OASYS1_ESRF_Extensions.egg-info/requires.txt
+-rw-r--r--   0 srio      (4230) soft      (3401)       14 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/OASYS1_ESRF_Extensions.egg-info/top_level.txt
+-rw-r--r--   0 srio      (4230) soft      (3401)     2590 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/PKG-INFO
+-rw-r--r--   0 srio      (4230) soft      (3401)     1503 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/README.md
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/
+-rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/
+-rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/menu/
+-rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/menu/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/oasys/
+-rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/oasys/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/oasys/widgets/
+-rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/oasys/widgets/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/oasys/widgets/extension/
+-rw-r--r--   0 srio      (4230) soft      (3401)      181 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/oasys/widgets/extension/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/oasys/widgets/extension/icons/
+-rw-r--r--   0 srio      (4230) soft      (3401)   300738 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/oasys/widgets/extension/icons/esrf2.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    23757 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/oasys/widgets/extension/icons/surface_merger.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    21241 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/oasys/widgets/extension/ow_surface_file_merger.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/
+-rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/util/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/util/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    11082 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/util/python_script.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/widgets/
+-rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/widgets/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/widgets/extension/
+-rw-r--r--   0 srio      (4230) soft      (3401)      188 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/widgets/extension/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/widgets/extension/icons/
+-rw-r--r--   0 srio      (4230) soft      (3401)    34177 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/widgets/extension/icons/caustic.png
+-rw-r--r--   0 srio      (4230) soft      (3401)   451995 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/widgets/extension/icons/esrf.png
+-rw-r--r--   0 srio      (4230) soft      (3401)   300738 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/widgets/extension/icons/esrf2.png
+-rw-r--r--   0 srio      (4230) soft      (3401)     9813 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/widgets/extension/icons/python_script.png
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/widgets/extension/miscellanea/
+-rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/widgets/extension/miscellanea/test_first_widget.txt
+-rw-r--r--   0 srio      (4230) soft      (3401)     8848 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/widgets/extension/ow_als_caustic.py
+-rwxr-xr-x   0 srio      (4230) soft      (3401)    22757 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/widgets/extension/ow_shadow_python_script.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/widgets/gui/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/widgets/gui/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     4220 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/widgets/gui/plots.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/srw/
+-rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/srw/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/srw/util/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/srw/util/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/srw/widgets/
+-rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/srw/widgets/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/srw/widgets/extension/
+-rw-r--r--   0 srio      (4230) soft      (3401)      175 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/srw/widgets/extension/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/srw/widgets/extension/icons/
+-rw-r--r--   0 srio      (4230) soft      (3401)   300738 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/srw/widgets/extension/icons/esrf2.png
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/syned/
+-rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/syned/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/syned/util/
+-rw-r--r--   0 srio      (4230) soft      (3401)    19863 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/syned/util/FEA_File.py
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/syned/util/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/syned/widgets/
+-rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/syned/widgets/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/syned/widgets/extension/
+-rw-r--r--   0 srio      (4230) soft      (3401)      196 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/syned/widgets/extension/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/syned/widgets/extension/icons/
+-rw-r--r--   0 srio      (4230) soft      (3401)   300738 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/syned/widgets/extension/icons/esrf2.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    82709 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/syned/widgets/extension/icons/hhlo.png
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/syned/widgets/extension/misc/
+-rw-r--r--   0 srio      (4230) soft      (3401)    24524 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/syned/widgets/extension/misc/finite_element_usage.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    27860 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/syned/widgets/extension/ow_esrf_finite_element_reader.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/util/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/util/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     1283 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/util/esrf_util.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/util/gui/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/util/gui/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    19268 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/util/gui/ow_esrf_widget.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/wofry/
+-rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/wofry/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/wofry/util/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/wofry/util/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/wofry/widgets/
+-rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/wofry/widgets/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/wofry/widgets/extension/
+-rw-r--r--   0 srio      (4230) soft      (3401)      178 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/wofry/widgets/extension/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/wofry/widgets/extension/icons/
+-rw-r--r--   0 srio      (4230) soft      (3401)   196722 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/wofry/widgets/extension/icons/esrf2.png
+-rw-r--r--   0 srio      (4230) soft      (3401)     7263 2020-10-16 14:27:53.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/wofry/widgets/extension/icons/eyeglasses.png
+-rw-r--r--   0 srio      (4230) soft      (3401)     6049 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/wofry/widgets/extension/icons/lens.png
+-rw-r--r--   0 srio      (4230) soft      (3401)     8664 2020-10-16 14:35:36.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/wofry/widgets/extension/icons/lenscorrector.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    41557 2020-10-16 13:35:35.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/wofry/widgets/extension/ow_lens_1D.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    23587 2020-10-16 14:47:30.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/wofry/widgets/extension/ow_refractive_corrector_1D.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/
+-rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/util/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/util/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/
+-rw-r--r--   0 srio      (4230) soft      (3401)       56 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/extension/
+-rw-r--r--   0 srio      (4230) soft      (3401)    29509 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/extension/ID19AttenuatorsBox.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    18914 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/extension/Monochromator.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    18710 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/extension/Scintillator.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    17190 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/extension/Transfocator.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    17078 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/extension/Transfocator_test.py
+-rw-r--r--   0 srio      (4230) soft      (3401)      180 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/extension/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/extension/icons/
+-rw-r--r--   0 srio      (4230) soft      (3401)   300738 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/extension/icons/esrf2.png
+-rw-r--r--   0 srio      (4230) soft      (3401)     9405 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/extension/icons/id19_attenuator.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    46639 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/extension/icons/id19_monochromator.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    34373 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/extension/icons/id19_scintillator.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    15141 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/extension/icons/id19_trasnfocator.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    31892 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/extension/icons/ws_id19_hpw150.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    14975 2020-10-13 15:12:11.000000 OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/extension/wsID19.py
+-rw-r--r--   0 srio      (4230) soft      (3401)       38 2020-10-16 14:51:11.000000 OASYS1-ESRF-Extensions-0.0.9/setup.cfg
+-rw-r--r--   0 srio      (4230) soft      (3401)     4617 2020-10-16 14:51:04.000000 OASYS1-ESRF-Extensions-0.0.9/setup.py
```

### Comparing `OASYS1-ESRF-Extensions-0.0.8/LICENSE` & `OASYS1-ESRF-Extensions-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/MANIFEST.in` & `OASYS1-ESRF-Extensions-0.0.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/OASYS1_ESRF_Extensions.egg-info/PKG-INFO` & `OASYS1-ESRF-Extensions-0.0.9/OASYS1_ESRF_Extensions.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: OASYS1-ESRF-Extensions
-Version: 0.0.8
+Version: 0.0.9
 Summary: OASYS extension for the ESRF
 Home-page: https://github.com/oasys-esrf-kit/OASYS1-ESRF-Extensions
 Author: Luca Rebuffi, Manuel Sanchez del Rio
 Author-email: lrebuffi@anl.gov, srio@serf.eu
 License: GPLv3
 Download-URL: https://github.com/oasys-esrf-kit/OASYS1-ESRF-Extensions
 Description: # OASYS1-ESRF-Extensions
```

### Comparing `OASYS1-ESRF-Extensions-0.0.8/OASYS1_ESRF_Extensions.egg-info/SOURCES.txt` & `OASYS1-ESRF-Extensions-0.0.9/OASYS1_ESRF_Extensions.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,17 @@
 orangecontrib/esrf/wofry/__init__.py
 orangecontrib/esrf/wofry/util/__init__.py
 orangecontrib/esrf/wofry/widgets/__init__.py
 orangecontrib/esrf/wofry/widgets/extension/__init__.py
 orangecontrib/esrf/wofry/widgets/extension/ow_lens_1D.py
 orangecontrib/esrf/wofry/widgets/extension/ow_refractive_corrector_1D.py
 orangecontrib/esrf/wofry/widgets/extension/icons/esrf2.png
+orangecontrib/esrf/wofry/widgets/extension/icons/eyeglasses.png
 orangecontrib/esrf/wofry/widgets/extension/icons/lens.png
+orangecontrib/esrf/wofry/widgets/extension/icons/lenscorrector.png
 orangecontrib/esrf/xoppy/__init__.py
 orangecontrib/esrf/xoppy/util/__init__.py
 orangecontrib/esrf/xoppy/widgets/__init__.py
 orangecontrib/esrf/xoppy/widgets/extension/ID19AttenuatorsBox.py
 orangecontrib/esrf/xoppy/widgets/extension/Monochromator.py
 orangecontrib/esrf/xoppy/widgets/extension/Scintillator.py
 orangecontrib/esrf/xoppy/widgets/extension/Transfocator.py
```

### Comparing `OASYS1-ESRF-Extensions-0.0.8/OASYS1_ESRF_Extensions.egg-info/entry_points.txt` & `OASYS1-ESRF-Extensions-0.0.9/OASYS1_ESRF_Extensions.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/PKG-INFO` & `OASYS1-ESRF-Extensions-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: OASYS1-ESRF-Extensions
-Version: 0.0.8
+Version: 0.0.9
 Summary: OASYS extension for the ESRF
 Home-page: https://github.com/oasys-esrf-kit/OASYS1-ESRF-Extensions
 Author: Luca Rebuffi, Manuel Sanchez del Rio
 Author-email: lrebuffi@anl.gov, srio@serf.eu
 License: GPLv3
 Download-URL: https://github.com/oasys-esrf-kit/OASYS1-ESRF-Extensions
 Description: # OASYS1-ESRF-Extensions
```

### Comparing `OASYS1-ESRF-Extensions-0.0.8/README.md` & `OASYS1-ESRF-Extensions-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/oasys/widgets/extension/icons/esrf2.png` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/oasys/widgets/extension/icons/esrf2.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/oasys/widgets/extension/icons/surface_merger.png` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/oasys/widgets/extension/icons/surface_merger.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/oasys/widgets/extension/ow_surface_file_merger.py` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/oasys/widgets/extension/ow_surface_file_merger.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/util/python_script.py` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/util/python_script.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/widgets/extension/icons/caustic.png` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/widgets/extension/icons/caustic.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/widgets/extension/icons/esrf.png` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/widgets/extension/icons/esrf.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/widgets/extension/icons/esrf2.png` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/widgets/extension/icons/esrf2.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/widgets/extension/icons/python_script.png` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/widgets/extension/icons/python_script.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/widgets/extension/ow_als_caustic.py` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/widgets/extension/ow_als_caustic.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/widgets/extension/ow_shadow_python_script.py` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/widgets/extension/ow_shadow_python_script.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/shadow/widgets/gui/plots.py` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/shadow/widgets/gui/plots.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/srw/widgets/extension/icons/esrf2.png` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/srw/widgets/extension/icons/esrf2.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/syned/util/FEA_File.py` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/syned/util/FEA_File.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/syned/widgets/extension/icons/esrf2.png` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/syned/widgets/extension/icons/esrf2.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/syned/widgets/extension/icons/hhlo.png` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/syned/widgets/extension/icons/hhlo.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/syned/widgets/extension/misc/finite_element_usage.png` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/syned/widgets/extension/misc/finite_element_usage.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/syned/widgets/extension/ow_esrf_finite_element_reader.py` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/syned/widgets/extension/ow_esrf_finite_element_reader.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/util/esrf_util.py` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/util/esrf_util.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/util/gui/ow_esrf_widget.py` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/util/gui/ow_esrf_widget.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/wofry/widgets/extension/icons/esrf2.png` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/wofry/widgets/extension/icons/esrf2.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/wofry/widgets/extension/icons/lens.png` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/wofry/widgets/extension/icons/lens.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/wofry/widgets/extension/ow_lens_1D.py` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/wofry/widgets/extension/ow_lens_1D.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/wofry/widgets/extension/ow_refractive_corrector_1D.py` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/wofry/widgets/extension/ow_refractive_corrector_1D.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,24 +14,26 @@
 from orangecontrib.wofry.widgets.gui.ow_wofry_widget import WofryWidget
 from orangecontrib.xoppy.util.python_script import PythonScript  # TODO: change import from wofry!!!
 
 from syned.widget.widget_decorator import WidgetDecorator
 
 from wofry.propagator.wavefront1D.generic_wavefront import GenericWavefront1D
 
+import xraylib
+
 import os
 import orangecanvas.resources as resources
 from scipy import interpolate
 
 class OWRefractiveCorrector1D(WofryWidget):
 
     name = "Corrector (reflector) 1D"
     id = "WofryCorrectorByReflection1D"
     description = "ALS Corrector (reflector) 1D"
-    icon = "icons/eyeglasses.png"
+    icon = "icons/lenscorrector.png"
     priority = 5
 
     category = "Wofry Wavefront Propagation"
     keywords = ["data", "file", "load", "read"]
 
     outputs = [{"name":"WofryData",
                 "type":WofryData,
@@ -47,16 +49,19 @@
                 "id":"Trigger"}]
 
     inputs = [("WofryData", WofryData, "set_input"),
               ("GenericWavefront1D", GenericWavefront1D, "set_input"),
               WidgetDecorator.syned_input_data()[0]]
 
     correction_method = Setting(1)
-    grazing_angle = Setting(1.5e-3)
     focus_at = Setting(10.0)
+    material = Setting(0)
+    refraction_index_delta = Setting(5.3e-7)
+    att_coefficient = Setting(0.00357382)
+    wall_thickness = Setting(0.0)
     apodization = Setting(0)
     apodization_ratio = Setting(0.1)
     apply_correction_to_wavefront = Setting(0)
     write_correction_profile = Setting(0)
     file_correction_profile = Setting("correction_profile1D.dat")
     write_input_wavefront = Setting(0)
 
@@ -110,21 +115,41 @@
                      items=["None","Focus to waist with reflector"],
                      callback=self.set_visible,
                      sendSelectedValue=False, orientation="horizontal")
 
 
         self.box_corrector_1 = oasysgui.widgetBox(box_corrector, "", addSpace=False, orientation="vertical")
 
-        oasysgui.lineEdit(self.box_corrector_1, self, "grazing_angle", "Grazing angle [rad]",
-                          labelWidth=300, valueType=float, orientation="horizontal")
-
         oasysgui.widgetBox(self.box_corrector_1, "", addSpace=False, orientation="horizontal")
         oasysgui.lineEdit(self.box_corrector_1, self, "focus_at", "Distance to waist [m]",
                           labelWidth=300, valueType=float, orientation="horizontal")
 
+
+        gui.comboBox(self.box_corrector_1, self, "material", label="Material",
+                     items=["External", "Be", "Al", "Diamond"],
+                     callback=self.set_visible,
+                     sendSelectedValue=False, orientation="horizontal")
+
+        self.box_refraction_index_id = oasysgui.widgetBox(self.box_corrector_1, "", addSpace=False, orientation="horizontal")
+        tmp = oasysgui.lineEdit(self.box_refraction_index_id, self, "refraction_index_delta", "Refraction index delta",
+                          labelWidth=300, valueType=float, orientation="horizontal")
+        tmp.setToolTip("refraction_index_delta")
+
+        self.box_att_coefficient_id = oasysgui.widgetBox(self.box_corrector_1, "", addSpace=False, orientation="horizontal")
+        tmp = oasysgui.lineEdit(self.box_att_coefficient_id, self, "att_coefficient", "Attenuation coefficient [m-1]",
+                          labelWidth=300, valueType=float, orientation="horizontal")
+        tmp.setToolTip("att_coefficient")
+
+
+        self.box_wall_thickness_id = oasysgui.widgetBox(self.box_corrector_1, "", addSpace=False, orientation="horizontal")
+        tmp = oasysgui.lineEdit(self.box_wall_thickness_id, self, "wall_thickness", "Wall thickness [m]",
+                          labelWidth=300, valueType=float, orientation="horizontal")
+        tmp.setToolTip("wall_thickness")
+
+
         gui.comboBox(self.box_corrector_1, self, "apodization", label="Modify correction profile", labelWidth=350,
                      items=["No","Apodization with intensity","Apodization with Gaussian"],
                      sendSelectedValue=False, orientation="horizontal",callback=self.set_visible)
         self.apodization_ratio_id = oasysgui.widgetBox(self.box_corrector_1, "", addSpace=False, orientation="horizontal")
         oasysgui.lineEdit(self.apodization_ratio_id, self, "apodization_ratio", "Apodization sigma/window ratio",
                           labelWidth=300, valueType=float, orientation="horizontal")
 
@@ -152,14 +177,17 @@
 
         self.file_box_id = oasysgui.widgetBox(self.box_corrector_1, "", addSpace=True, orientation="horizontal", width=400, height=35)
 
 
         self.set_visible()
 
     def set_visible(self):
+        self.box_refraction_index_id.setVisible(self.material in [0])
+        self.box_att_coefficient_id.setVisible(self.material in [0])
+
         if self.correction_method == 0:
             self.box_corrector_1.setVisible(False)
         else:
             self.box_corrector_1.setVisible(True)
 
             if self.apodization == 2:
                 self.apodization_ratio_id.setVisible(True)
@@ -183,18 +211,21 @@
             self.plot_canvas.append(None)
 
         for tab in self.tab:
             tab.setFixedHeight(self.IMAGE_HEIGHT)
             tab.setFixedWidth(self.IMAGE_WIDTH)
 
     def check_fields(self):
-        self.grazing_angle = congruence.checkStrictlyPositiveNumber(self.grazing_angle, "Grazing angle")
         self.focus_at = congruence.checkStrictlyPositiveNumber(numpy.abs(self.focus_at), "Distance to waist")
         self.apodization_ratio = congruence.checkStrictlyPositiveNumber(numpy.abs(self.apodization_ratio), "Apodzation radio")
 
+        self.wall_thickness = congruence.checkPositiveNumber(self.wall_thickness, "Wall thickness")
+        self.refraction_index_delta = congruence.checkPositiveNumber(self.refraction_index_delta, "Refraction index delta")
+        self.att_coefficient = congruence.checkPositiveNumber(self.att_coefficient, "Attenuation coefficient")
+
     def receive_syned_data(self):
         raise Exception(NotImplementedError)
 
     def set_input(self, wofry_data):
         if not wofry_data is None:
             if isinstance(wofry_data, WofryData):
                 self.input_data = wofry_data
@@ -223,36 +254,66 @@
 
         if self.correction_method == 0: # no correction
             output_wavefront = input_wavefront.duplicate()
             target_wavefront = input_wavefront.duplicate()
             abscissas_on_mirror = target_wavefront.get_abscissas()
             height = numpy.zeros_like(abscissas_on_mirror)
         else:
-            output_wavefront, target_wavefront, abscissas_on_mirror, height = self.calculate_output_wavefront_after_corrector1D(
+            photon_energy = self.input_data.get_wavefront().get_photon_energy()
+            wave_length = self.input_data.get_wavefront().get_wavelength()
+            if self.material == 0:  # external
+                refraction_index_delta = self.refraction_index_delta
+                att_coefficient = self.att_coefficient
+            else:
+                if self.material == 1:  # Be
+                    element = "Be"
+                    density = xraylib.ElementDensity(4)
+                elif self.material == 2:  # Al
+                    element = "Al"
+                    density = xraylib.ElementDensity(13)
+                elif self.material == 3:  # Diamond
+                    element = "C"
+                    density = 3.51
+                print("Element: %s" % element)
+                print("        density = %g " % density)
+                print("        photon energy = %g eV " % photon_energy)
+
+                refraction_index = xraylib.Refractive_Index(element, photon_energy / 1000, density)
+                refraction_index_delta = 1 - refraction_index.real
+                att_coefficient = 4*numpy.pi * (xraylib.Refractive_Index(element, \
+                                photon_energy/1000, density)).imag / wave_length
+
+            print("Refracion index delta = %g " % (refraction_index_delta))
+            print("Attenuation coeff mu = %g m^-1" % (att_coefficient))
+
+            output_wavefront, target_wavefront, abscissas_on_mirror, height = self.calculate_output_wavefront_after_refractive_corrector1D(
                     input_wavefront,
-                    grazing_angle=self.grazing_angle,
                     focus_at=self.focus_at,
                     apodization=self.apodization,
                     apodization_ratio=self.apodization_ratio,
-                    file_correction_profile=file_correction_profile)
+                    file_correction_profile=file_correction_profile,
+                    refraction_index_delta=refraction_index_delta,
+                    att_coefficient=att_coefficient,
+                    wall_thickness=self.wall_thickness)
 
         self.progressBarSet(50)
         if self.view_type > 0:
             self.do_plot_wavefront(output_wavefront, target_wavefront, abscissas_on_mirror, height)
 
 
 
         if self.write_input_wavefront:
             self.input_data.get_wavefront().save_h5_file("wavefront_input.h5",subgroupname="wfr",intensity=True,phase=True,
                                           overwrite=True,verbose=True)
 
         # script
-        dict_parameters = {"grazing_angle": self.grazing_angle,
-                           "focus_at": self.focus_at,
-                           "focus_at":self.focus_at,
+        dict_parameters = {"focus_at": self.focus_at,
+                           "wall_thickness": self.wall_thickness,
+                           "refraction_index_delta": refraction_index_delta,
+                           "att_coefficient": att_coefficient,
                            "apodization": self.apodization,
                            "apodization_ratio":self.apodization_ratio,
                            "file_correction_profile":file_correction_profile}
 
         script_template = self.script_template_output_wavefront_after_correction1D()
         self.wofry_script.set_code(script_template.format_map(dict_parameters))
 
@@ -275,47 +336,55 @@
 
 
 
 
 
 
     @classmethod
-    def calculate_output_wavefront_after_corrector1D(cls, input_wavefront,grazing_angle=1.5e-3, focus_at=10.0,
-                                                     apodization=0, apodization_ratio=0.1, file_correction_profile=""):
+    def calculate_output_wavefront_after_refractive_corrector1D(cls, input_wavefront, focus_at=10.0,
+                                                     apodization=0, apodization_ratio=0.1, file_correction_profile="",
+                                                     refraction_index_delta=1e-7,
+                                                     att_coefficient=0.0,
+                                                     wall_thickness=0.0):
 
         output_wavefront = input_wavefront.duplicate()
         target_wavefront = input_wavefront.duplicate()
         target_wavefront.set_spherical_wave(radius=-focus_at, center=0.0, complex_amplitude=1.0)
 
         phase_input = input_wavefront.get_phase(unwrap=True)
         phase_target = target_wavefront.get_phase(unwrap=True)
         phase_correction = phase_target - phase_input
         abscissas = target_wavefront.get_abscissas()
-        abscissas_on_mirror = abscissas / numpy.sin(grazing_angle)
+        abscissas_on_mirror = abscissas
 
         # output_wavefront.add_phase_shift(phase_correction)
-        height = - phase_correction / (2 * output_wavefront.get_wavenumber() * numpy.sin(grazing_angle))
+        height = - phase_correction / (output_wavefront.get_wavenumber() * refraction_index_delta)
 
         if apodization == 0:
+            # pass
             height -= height[height.size // 2]
         elif apodization == 1:
             apodization = input_wavefront.get_intensity()
             apodization = (apodization / apodization.max())
             height *= apodization
             height -= height[0]
         elif apodization == 2:
             sigma = numpy.abs(abscissas[-1] - abscissas[0]) * apodization_ratio
             apodization = numpy.exp( - abscissas**2 / 2 / sigma**2)
             apodization /= apodization.max()
             height *= apodization
             height -= height[0]
 
-        # calculate phase shift from new profile
-        phi = -2 * output_wavefront.get_wavenumber() * height * numpy.sin(grazing_angle)
-        output_wavefront.add_phase_shift(phi)
+        height += wall_thickness
+
+        amp_factors = numpy.sqrt(numpy.exp(-1.0 * att_coefficient * height))
+        phase_shifts = -1.0 * output_wavefront.get_wavenumber() * refraction_index_delta * height
+
+        output_wavefront.rescale_amplitudes(amp_factors)
+        output_wavefront.add_phase_shifts(phase_shifts)
 
         # output files
         if file_correction_profile != "":
             f = open(file_correction_profile,"w")
             if apodization <= 2:
                 for i in range(height.size):
                     f.write("%g %g\n"%(abscissas_on_mirror[i],height[i]))
@@ -325,30 +394,34 @@
         return output_wavefront, target_wavefront, abscissas_on_mirror, height
 
     # warning: pay attention to the double backslash in \\n
     def script_template_output_wavefront_after_correction1D(self):
         return \
 """
 
+import numpy
+
+def calculate_output_wavefront_after_refractive_corrector1D(input_wavefront, focus_at=10.0,
+                                                 apodization=0, apodization_ratio=0.1, file_correction_profile="",
+                                                 refraction_index_delta=1e-7,
+                                                 att_coefficient=0.0,
+                                                 wall_thickness=0.0):
 
-def calculate_output_wavefront_after_corrector1D(input_wavefront,grazing_angle=1.5e-3, focus_at=10.0, apodization=0, apodization_ratio=0.1, file_correction_profile=""):
-    import numpy
-    from scipy import interpolate
     output_wavefront = input_wavefront.duplicate()
     target_wavefront = input_wavefront.duplicate()
     target_wavefront.set_spherical_wave(radius=-focus_at, center=0.0, complex_amplitude=1.0)
 
     phase_input = input_wavefront.get_phase(unwrap=True)
     phase_target = target_wavefront.get_phase(unwrap=True)
     phase_correction = phase_target - phase_input
     abscissas = target_wavefront.get_abscissas()
-    abscissas_on_mirror = abscissas / numpy.sin(grazing_angle)
+    abscissas_on_mirror = abscissas
 
     # output_wavefront.add_phase_shift(phase_correction)
-    height = - phase_correction / (2 * output_wavefront.get_wavenumber() * numpy.sin(grazing_angle))
+    height = - phase_correction / (output_wavefront.get_wavenumber() * refraction_index_delta)
 
     if apodization == 0:
         height -= height[height.size // 2]
     elif apodization == 1:
         apodization = input_wavefront.get_intensity()
         apodization = (apodization / apodization.max())
         height *= apodization
@@ -356,34 +429,48 @@
     elif apodization == 2:
         sigma = numpy.abs(abscissas[-1] - abscissas[0]) * apodization_ratio
         apodization = numpy.exp( - abscissas**2 / 2 / sigma**2)
         apodization /= apodization.max()
         height *= apodization
         height -= height[0]
 
-    # calculate phase shift from new profile
-    phi = -2 * output_wavefront.get_wavenumber() * height * numpy.sin(grazing_angle)
-    output_wavefront.add_phase_shift(phi)
+    height += wall_thickness
+
+    amp_factors = numpy.sqrt(numpy.exp(-1.0 * att_coefficient * height))
+    phase_shifts = -1.0 * output_wavefront.get_wavenumber() * refraction_index_delta * height
+
+    output_wavefront.rescale_amplitudes(amp_factors)
+    output_wavefront.add_phase_shifts(phase_shifts)
 
     # output files
     if file_correction_profile != "":
         f = open(file_correction_profile,"w")
         if apodization <= 2:
             for i in range(height.size):
                 f.write("%g %g\\n"%(abscissas_on_mirror[i],height[i]))
         f.close()
         print("File written to disk: %s " % file_correction_profile)
 
     return output_wavefront, target_wavefront, abscissas_on_mirror, height
+
+
 #
 # main
 #
 from wofry.propagator.wavefront1D.generic_wavefront import GenericWavefront1D
 input_wavefront = GenericWavefront1D.load_h5_file("wavefront_input.h5","wfr")
-output_wavefront, target_wavefront, abscissas_on_mirror, height = calculate_output_wavefront_after_corrector1D(input_wavefront,grazing_angle={grazing_angle}, focus_at={focus_at}, apodization={apodization}, apodization_ratio={apodization_ratio}, file_correction_profile="{file_correction_profile}")
+output_wavefront, target_wavefront, abscissas, height = calculate_output_wavefront_after_refractive_corrector1D(input_wavefront,
+        focus_at={focus_at},
+        apodization={apodization},
+        apodization_ratio={apodization_ratio}, 
+        file_correction_profile="{file_correction_profile}",
+        refraction_index_delta={refraction_index_delta},
+        att_coefficient={att_coefficient},
+        wall_thickness={wall_thickness})
+
 
 from srxraylib.plot.gol import plot
 plot(output_wavefront.get_abscissas(),output_wavefront.get_intensity())
 """
 
     def do_plot_results(self, progressBarValue): # required by parent
         pass
```

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/extension/ID19AttenuatorsBox.py` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/extension/ID19AttenuatorsBox.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/extension/Monochromator.py` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/extension/Monochromator.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/extension/Scintillator.py` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/extension/Scintillator.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/extension/Transfocator.py` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/extension/Transfocator.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/extension/Transfocator_test.py` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/extension/Transfocator_test.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/extension/icons/esrf2.png` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/extension/icons/esrf2.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/extension/icons/id19_attenuator.png` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/extension/icons/id19_attenuator.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/extension/icons/id19_monochromator.png` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/extension/icons/id19_monochromator.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/extension/icons/id19_scintillator.png` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/extension/icons/id19_scintillator.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/extension/icons/id19_trasnfocator.png` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/extension/icons/id19_trasnfocator.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/extension/icons/ws_id19_hpw150.png` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/extension/icons/ws_id19_hpw150.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/orangecontrib/esrf/xoppy/widgets/extension/wsID19.py` & `OASYS1-ESRF-Extensions-0.0.9/orangecontrib/esrf/xoppy/widgets/extension/wsID19.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ESRF-Extensions-0.0.8/setup.py` & `OASYS1-ESRF-Extensions-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 try:
     from setuptools import find_packages, setup
 except AttributeError:
     from setuptools import find_packages, setup
 
 NAME = 'OASYS1-ESRF-Extensions'
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 ISRELEASED = True
 
 DESCRIPTION = 'OASYS extension for the ESRF'
 README_FILE = os.path.join(os.path.dirname(__file__), 'README.md')
 LONG_DESCRIPTION = open(README_FILE).read()
 AUTHOR = 'Luca Rebuffi, Manuel Sanchez del Rio'
 AUTHOR_EMAIL = 'lrebuffi@anl.gov, srio@serf.eu'
```

