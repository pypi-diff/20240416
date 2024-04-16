# Comparing `tmp/astro-tiptop-1.3.7.tar.gz` & `tmp/astro_tiptop-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-tiptop-1.3.7.tar", last modified: Thu Mar  7 11:56:24 2024, max compression
+gzip compressed data, was "astro_tiptop-1.3.8.tar", last modified: Tue Apr 16 14:43:20 2024, max compression
```

## Comparing `astro-tiptop-1.3.7.tar` & `astro_tiptop-1.3.8.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:56:24.340969 astro-tiptop-1.3.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:56:24.288970 astro-tiptop-1.3.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:56:24.292970 astro-tiptop-1.3.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/.github/workflows/run_tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-03-07 11:56:24.340969 astro-tiptop-1.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/TIPTOP-AST-EXAMPLE.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10572 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/TIPTOP-AST-GEN-RECARRAY.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/TIPTOP-AST-READ.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/TIPTOP-EXAMPLE.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/TIPTOP-EXAMPLE.py
--rw-r--r--   0 runner    (1001) docker     (127)    12147 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/TIPTOP-GUI.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:56:24.332970 astro-tiptop-1.3.7/astTest/
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/astTest/ERISast10.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/astTest/ERISast100.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/astTest/ERISast1000.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/astTest/ERISastMonads.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/astTest/ERISastRandom.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/astTest/ERISastSingles1.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/astTest/MAVISast.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/astTest/MAVISastGenerate.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/astTest/MAVISastSingles.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/astTest/MAVISastTriplets.ini
--rw-r--r--   0 runner    (1001) docker     (127)   204688 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/astTest/rec_array10.npy
--rw-r--r--   0 runner    (1001) docker     (127)  2685346 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/astTest/rec_array100.npy
--rw-r--r--   0 runner    (1001) docker     (127) 26962531 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/astTest/rec_array100_e.npy
--rw-r--r--   0 runner    (1001) docker     (127)  2935683 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/astTest/rec_array10_e.npy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:56:24.340969 astro-tiptop-1.3.7/astro_tiptop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-03-07 11:56:24.000000 astro-tiptop-1.3.7/astro_tiptop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-03-07 11:56:24.000000 astro-tiptop-1.3.7/astro_tiptop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 11:56:24.000000 astro-tiptop-1.3.7/astro_tiptop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-07 11:56:24.000000 astro-tiptop-1.3.7/astro_tiptop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-07 11:56:24.000000 astro-tiptop-1.3.7/astro_tiptop.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:56:24.336969 astro-tiptop-1.3.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:56:24.336969 astro-tiptop-1.3.7/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/docs/source/howto.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    22201 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/docs/source/parameterFile.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7852 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/docs/source/wishList.rst
--rw-r--r--   0 runner    (1001) docker     (127)   165545 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/main_sphere_test.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:56:24.340969 astro-tiptop-1.3.7/perfTest/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/perfTest/ERIS.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/perfTest/ERIS_LGS.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)     7610 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/perfTest/HarmoniLTAO_1.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)     7496 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/perfTest/HarmoniLTAO_2.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)     7520 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/perfTest/HarmoniLTAO_3.ini
--rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/perfTest/HarmoniSCAO_1.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)     5777 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/perfTest/HarmoniSCAO_2.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)     5777 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/perfTest/HarmoniSCAO_3.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/perfTest/MAVIS.ini
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/perfTest/SOUL.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/perfTest/SPHERE.ini
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/perfTest.sh
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 11:56:24.340969 astro-tiptop-1.3.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:56:24.340969 astro-tiptop-1.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/tests/allTests.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/tests/mavisResult0.npy
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/tests/mavisResult1.npy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:56:24.340969 astro-tiptop-1.3.7/tiptop/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/tiptop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-07 11:56:24.000000 astro-tiptop-1.3.7/tiptop/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    40848 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/tiptop/asterismSimulation.py
--rw-r--r--   0 runner    (1001) docker     (127)    32742 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/tiptop/baseSimulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/tiptop/tiptop.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1419 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/tiptop/tiptopCLT.py
--rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/tiptop/tiptopGUI.py
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-03-07 11:56:14.000000 astro-tiptop-1.3.7/tiptop/tiptopUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:43:20.270354 astro_tiptop-1.3.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:43:20.214354 astro_tiptop-1.3.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:43:20.218354 astro_tiptop-1.3.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/.github/workflows/run_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-16 14:43:20.266354 astro_tiptop-1.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/TIPTOP-AST-EXAMPLE.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10572 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/TIPTOP-AST-GEN-RECARRAY.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/TIPTOP-AST-READ.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/TIPTOP-EXAMPLE.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/TIPTOP-EXAMPLE.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12147 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/TIPTOP-GUI.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:43:20.258354 astro_tiptop-1.3.8/astTest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/ERISast10.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/ERISast100.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/ERISast1000.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/ERISastMonads.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/ERISastRandom.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/ERISastSingles1.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/MAVISast.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/MAVISastGenerate.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/MAVISastSingles.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/MAVISastTriplets.ini
+-rw-r--r--   0 runner    (1001) docker     (127)   204688 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/rec_array10.npy
+-rw-r--r--   0 runner    (1001) docker     (127)  2685346 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/rec_array100.npy
+-rw-r--r--   0 runner    (1001) docker     (127) 26962531 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/rec_array100_e.npy
+-rw-r--r--   0 runner    (1001) docker     (127)  2935683 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/rec_array10_e.npy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:43:20.266354 astro_tiptop-1.3.8/astro_tiptop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-16 14:43:20.000000 astro_tiptop-1.3.8/astro_tiptop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-16 14:43:20.000000 astro_tiptop-1.3.8/astro_tiptop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:43:20.000000 astro_tiptop-1.3.8/astro_tiptop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-16 14:43:20.000000 astro_tiptop-1.3.8/astro_tiptop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 14:43:20.000000 astro_tiptop-1.3.8/astro_tiptop.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:43:20.262354 astro_tiptop-1.3.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:43:20.262354 astro_tiptop-1.3.8/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/docs/source/howto.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    22546 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/docs/source/parameterFile.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7852 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/docs/source/wishList.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   165545 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/main_sphere_test.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:43:20.266354 astro_tiptop-1.3.8/perfTest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/perfTest/ERIS.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/perfTest/ERIS_LGS.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7610 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/perfTest/HarmoniLTAO_1.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7496 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/perfTest/HarmoniLTAO_2.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7520 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/perfTest/HarmoniLTAO_3.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/perfTest/HarmoniSCAO_1.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5777 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/perfTest/HarmoniSCAO_2.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5777 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/perfTest/HarmoniSCAO_3.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/perfTest/MAVIS.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/perfTest/MORFEO.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/perfTest/SOUL.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/perfTest/SPHERE.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/perfTest.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 14:43:20.270354 astro_tiptop-1.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:43:20.266354 astro_tiptop-1.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/tests/allTests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/tests/mavisResult0.npy
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/tests/mavisResult1.npy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:43:20.266354 astro_tiptop-1.3.8/tiptop/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/tiptop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-16 14:43:19.000000 astro_tiptop-1.3.8/tiptop/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40846 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/tiptop/asterismSimulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35034 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/tiptop/baseSimulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/tiptop/tiptop.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1419 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/tiptop/tiptopCLT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/tiptop/tiptopGUI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/tiptop/tiptopUtils.py
```

### Comparing `astro-tiptop-1.3.7/.github/workflows/publish.yml` & `astro_tiptop-1.3.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/.github/workflows/run_tests.yml` & `astro_tiptop-1.3.8/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/.gitignore` & `astro_tiptop-1.3.8/.gitignore`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/LICENSE` & `astro_tiptop-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/PKG-INFO` & `astro_tiptop-1.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: astro-tiptop
-Version: 1.3.7
+Version: 1.3.8
 Author-email: Fabio Rossi <fabio.rossi@inaf.it>
 License: MIT License
 Project-URL: repository, https://github.com/astro-tiptop/TIPTOP
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pyyaml
-Requires-Dist: astro-p3>=1.2.10
-Requires-Dist: mastsel>=1.2.6
+Requires-Dist: astro-p3>=1.2.11
+Requires-Dist: mastsel>=1.2.7
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Provides-Extra: gpu
 Requires-Dist: mastsel[gpu]; extra == "gpu"
 Provides-Extra: gui
 Requires-Dist: ipywidgets; extra == "gui"
```

### Comparing `astro-tiptop-1.3.7/README.md` & `astro_tiptop-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/TIPTOP-AST-EXAMPLE.ipynb` & `astro_tiptop-1.3.8/TIPTOP-AST-EXAMPLE.ipynb`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/TIPTOP-AST-GEN-RECARRAY.ipynb` & `astro_tiptop-1.3.8/TIPTOP-AST-GEN-RECARRAY.ipynb`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/TIPTOP-AST-READ.ipynb` & `astro_tiptop-1.3.8/TIPTOP-AST-READ.ipynb`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/TIPTOP-EXAMPLE.ipynb` & `astro_tiptop-1.3.8/TIPTOP-EXAMPLE.ipynb`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/TIPTOP-GUI.ipynb` & `astro_tiptop-1.3.8/TIPTOP-GUI.ipynb`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/astTest/ERISast10.ini` & `astro_tiptop-1.3.8/astTest/ERISast10.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/astTest/ERISast100.ini` & `astro_tiptop-1.3.8/astTest/ERISast100.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/astTest/ERISast1000.ini` & `astro_tiptop-1.3.8/astTest/ERISast1000.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/astTest/ERISastMonads.ini` & `astro_tiptop-1.3.8/astTest/ERISastMonads.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/astTest/ERISastRandom.ini` & `astro_tiptop-1.3.8/astTest/ERISastRandom.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/astTest/ERISastSingles1.ini` & `astro_tiptop-1.3.8/astTest/ERISastSingles1.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/astTest/MAVISast.ini` & `astro_tiptop-1.3.8/astTest/MAVISast.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/astTest/MAVISastGenerate.ini` & `astro_tiptop-1.3.8/astTest/MAVISastGenerate.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/astTest/MAVISastSingles.ini` & `astro_tiptop-1.3.8/astTest/MAVISastSingles.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/astTest/MAVISastTriplets.ini` & `astro_tiptop-1.3.8/astTest/MAVISastTriplets.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/astTest/rec_array10.npy` & `astro_tiptop-1.3.8/astTest/rec_array10.npy`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/astTest/rec_array100.npy` & `astro_tiptop-1.3.8/astTest/rec_array100.npy`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/astTest/rec_array100_e.npy` & `astro_tiptop-1.3.8/astTest/rec_array100_e.npy`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/astTest/rec_array10_e.npy` & `astro_tiptop-1.3.8/astTest/rec_array10_e.npy`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/astro_tiptop.egg-info/PKG-INFO` & `astro_tiptop-1.3.8/astro_tiptop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: astro-tiptop
-Version: 1.3.7
+Version: 1.3.8
 Author-email: Fabio Rossi <fabio.rossi@inaf.it>
 License: MIT License
 Project-URL: repository, https://github.com/astro-tiptop/TIPTOP
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pyyaml
-Requires-Dist: astro-p3>=1.2.10
-Requires-Dist: mastsel>=1.2.6
+Requires-Dist: astro-p3>=1.2.11
+Requires-Dist: mastsel>=1.2.7
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Provides-Extra: gpu
 Requires-Dist: mastsel[gpu]; extra == "gpu"
 Provides-Extra: gui
 Requires-Dist: ipywidgets; extra == "gui"
```

### Comparing `astro-tiptop-1.3.7/astro_tiptop.egg-info/SOURCES.txt` & `astro_tiptop-1.3.8/astro_tiptop.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 perfTest/HarmoniLTAO_1.ini
 perfTest/HarmoniLTAO_2.ini
 perfTest/HarmoniLTAO_3.ini
 perfTest/HarmoniSCAO_1.ini
 perfTest/HarmoniSCAO_2.ini
 perfTest/HarmoniSCAO_3.ini
 perfTest/MAVIS.ini
+perfTest/MORFEO.ini
 perfTest/SOUL.ini
 perfTest/SPHERE.ini
 tests/allTests.py
 tests/mavisResult0.npy
 tests/mavisResult1.npy
 tiptop/__init__.py
 tiptop/_version.py
```

### Comparing `astro-tiptop-1.3.7/docs/Makefile` & `astro_tiptop-1.3.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/docs/make.bat` & `astro_tiptop-1.3.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/docs/source/conf.py` & `astro_tiptop-1.3.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/docs/source/howto.rst` & `astro_tiptop-1.3.8/docs/source/howto.rst`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/docs/source/index.rst` & `astro_tiptop-1.3.8/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/docs/source/parameterFile.rst` & `astro_tiptop-1.3.8/docs/source/parameterFile.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,19 @@
 
    **Required**, 
    *type : float*, 
    Set the outer diameter of the telescope pupil in unit of meters.
 
 .. option:: ObscurationRatio
 
-   **Optionnal**, 
+   **Optional**, 
    *type : float*, 
    *Default : 0.0*,
    Defines the central obstruction due to the secondary as a ratio of the TelescopeDiameter
+
    *Warning* : MavisLO.py does not have a defualt value for this parameter 
 
 .. option:: Resolution
 
    **Required**, 
    *type : int*, 
    Number of pixels across the pupil diameter
@@ -53,14 +54,15 @@
 
 .. option:: TechnicalFoV
 
    **Optional**, 
    *type : float*, 
    *default: ??*, 
    set the size of the technical field of view
+
    *Warning* : This is not optional in MavisLO.py
 
 .. option:: PathPupil
 
    **Optional**, 
    *type : str*, 
    *default: ''*, 
@@ -97,15 +99,15 @@
 .. option:: PathStatModes
    
    **Optional**, 
    *type : str*, 
    *default: ''*, 
    path to a .fits file that contain a cube of map of mode in amplitude which lead to a rms of 1 in nanometer of static aberation. if absent or '', not used. Unsure how this works.
 
-.. option:: coeficientOfTheStaticMode
+.. option:: coefficientOfTheStaticMode
    
    **not used**, 
    *type : str*, 
    *default: ''*, 
    place holder 
    (TBC) need to find how does the pathStatModes fits file work.
 
@@ -139,14 +141,15 @@
 
 .. option:: extraErrorLoNm
    
    **Optional**, 
    *type : float*, 
    *default: 0*, 
    nm RMS of the additional error to be added (an error that is not otherwise considered) on LO directions only
+
    Note: (1) only makes sense if [sensor_LO] is present (2) if not present extraErrorNm is used on LO directions
 
 .. option:: extraErrorLoExp
    
    **Optional**, 
    *type : float*, 
    *default: -2*, 
@@ -161,16 +164,24 @@
 
 .. option:: extraErrorLoMax
    
    **Optional**, 
    *type : float*, 
    *default: 0*, 
    maximum spatial frequency for which PSD associated with extraErrorLoNm is > 0
+
    Note: 0 means maximum frequency is the one present in the spatial frequncy array of the PSDs 
 
+.. option:: jitter_FWHM
+
+   **Optional**, 
+   *type : float*, 
+   *default: None*, 
+   additional kernel to be convolved with PSF, it could be a scalar (FWHM in mas) for a round kernel or a list of three values [FWHM_mas_max, FWHM_mas_min, angle_rad]
+
 [atmosphere]
 ^^^^^^^^^^^^
 
 .. option:: Seeing
 
    **Required**, 
    *type : float*, 
@@ -179,63 +190,73 @@
 
 .. option:: Wavelength
 
    **Optional**, 
    *type : float*, 
    *Default : 500e-9*, 
    Wavelength of definition of the atmosphere statistics
-   Warning: not optional in MavisLO.py
+
+   *Warning* : not optional in MavisLO.py
 
 .. option:: L0
 
    **Optional**, 
    *type : float*, 
    *Default : 25.0*, 
    Outer Scale of the atmosphere  in meters
-   Warning: not optionnal in MavisLO.py
+
+   *Warning* : not optionnal in MavisLO.py
 
 .. option:: Cn2Weights
 
    **Optional**, 
    *type : list of float*, 
    *Default : [1.0]*, 
    Relative contribution of each layer. The sum of all the list element must be 1. 
    Must have the same length as ``Cn2Heights``, ``WindSpeed`` and ``WindDirection``.
-   Warning : required if ``Cn2Heights``, ``WindSpeed`` or ``WindDirection`` are defined
-   Warning : extremly confusing error message if absent when it must be defined
+
+   *Warning* : required if ``Cn2Heights``, ``WindSpeed`` or ``WindDirection`` are defined
+
+   *Warning* : extremly confusing error message if absent when it must be defined
 
 .. option:: Cn2Heights
 
    **Optional**, 
    *type : list of float*, 
    *Default : [0.0]*, 
    altitude of layers in meters.
    Must have the same length as ``Cn2Weights``, ``WindSpeed`` and ``WindDirection``.
-   Warning : required if ``Cn2Weights``, ``WindSpeed`` or ``WindDirection`` are defined
-   Warning : extremly confusing error message if absent when it must be defined
+
+   *Warning* : required if ``Cn2Weights``, ``WindSpeed`` or ``WindDirection`` are defined
+
+   *Warning* : extremly confusing error message if absent when it must be defined
 
 .. option:: WindSpeed
 
    **Optional**, 
    *Type : list of float*, 
    *Default : [10.0]*, 
    Wind speed values for each layer in m/s. 
    Must have the same length as ``Cn2Weights``, ``Cn2Heights`` and ``WindDirection``.
-   Warning : required if ``Cn2Weights``, ``Cn2Heights`` or ``WindDirection`` are defined
-   Warning : extremly confusing error message if absent when it must be defined
+
+   *Warning* : required if ``Cn2Weights``, ``Cn2Heights`` or ``WindDirection`` are defined
+
+   *Warning* : extremly confusing error message if absent when it must be defined
 
 .. option:: WindDirection
 
    **Optional**, 
    *Type : list of float*, 
    *Default : [0.0]*, 
    wind direction for each layer in degrees. 0 degree is ?? then anticlockwise.
    Must have the same length as ``Cn2Weights``, ``Cn2Heights`` and ``WindSpeed``.
-   Warning : required if ``Cn2Weights``, ``Cn2Heights`` or ``WindSpeed`` are defined
-   Warning : extremly confusing error message if absent when it must be defined
+
+   *Warning* : required if ``Cn2Weights``, ``Cn2Heights`` or ``WindSpeed`` are defined
+
+   *Warning* : extremly confusing error message if absent when it must be defined
 
 .. option:: r0_Value
    
    **Optionnal**, 
    *type : float*, 
    set the atmospere Fried parameter.
    If not set TIPTOP uses ``seeing`` .
@@ -275,15 +296,16 @@
 Typically the wavelength is the same for all guide star (at least in Laser guide star)
 
 .. option:: Wavelength
 
    **Required**, 
    *type : float*, 
    Sensing wavelength for Hight Order modes in meters
-   Warning : gives a confusing error message if absent
+
+   *Warning* : gives a confusing error message if absent
 
 .. option:: Zenith
 
    **Optional**, 
    *Type : list of float*, 
    *Default : [0.0]*
    Zenithal coordinate of each guide stars in arcsec.
@@ -336,23 +358,25 @@
 ^^^^^^^^^^^^^^^^
 
 .. option:: PixelScale
 
    **Required**, 
    *type : float*, 
    pixel/spaxel scale in mili arcsec
-   Warning: confusing error message if missing
+
+   *Warning* : confusing error message if missing
 
 
 .. option:: FieldOfView
 
    **Required**, 
    *type : float*, 
    Field of view of the camera in pixel/spaxel. need confirmation on the optionality of this paramiter. 
-   Warning: confusing error massage if missing
+
+   *Warning* : confusing error massage if missing
 
 .. note::
 
     Following parameters was added to uniform all the sensor (HO and LO), but they are not used.
 
     Binning, NumberPhotons, SpotFWHM, SpectralBandwidth, Transmittance, Dispersion, SigmaRON, Dark, SkyBackground, Gain, ExcessNoiseFactor, Wavelength, FieldOfView
 
@@ -376,22 +400,24 @@
    Size of WFS lenslets in meters. used, why a list of float? This overrides the ratio between telescope size and Number of lenslet used to compute the matrix size.
 
 .. option:: PixelScale
 
    **Required**, 
    *type: int*, 
    High Order WFS pixel scale in [mas], unclear what are the units if we chose a pyramid wavefront sensor
-   Warning: gives a confusing error message if missing 
+
+   *Warning* : gives a confusing error message if missing 
 
 .. option:: FieldOfView
 
    **Required**, 
    *type: int*, 
    Number of pixels per subaperture. 
-   Warning: gives a confusing error message if missing 
+
+   *Warning* : gives a confusing error message if missing 
 
 .. option:: Binning
    
    **Optional**, 
    *type: int*, 
    *default: 1*, 
    Binning factor of the detector, only used in the pyramid case, optional for pyramid
@@ -405,15 +431,16 @@
    Other available option: 'Pyramid'
 
 .. option:: NumberPhotons  
 
    **Required**, 
    *type: list of int*, 
    Flux return in [nph/frame/subaperture]
-   Warning: extremly confusing error message if missing
+
+   *Warning* : extremly confusing error message if missing
 
 .. option:: SpotFWHM    
    
    **Optional**, 
    *type: list of list of float*, 
    *defaut: [[0.0, 0.0, 0.0]]*, 
    High Order spot parameters: two axes scale values in milliarcsec (only max value is used) and angle (angle is not used). Why list?
@@ -494,15 +521,16 @@
 
 .. option:: Modulation
    
    **Required if WfsType == 'Pyramid'**, 
    *type: float*, 
    *default : None*, 
    If the chosen wavefront sensor is the ``'Pyramid'``, Spot modulation radius in lambda/D units. This is ignored if the WFS is `'Shack-Hartmann'`
-   Warning : gives really confusing message if missing when required
+
+   *Warning* : gives really confusing message if missing when required
 
 Can be set but not used
 """""""""""""""""""""""
 
 .. option:: Dark
    
    **not used**, 
@@ -540,23 +568,25 @@
    This section is optional, if this section is not present only the HO part will be used (for ex. to simulate a SCAO NGS).
 
 .. option:: PixelScale
 
    **Required**, 
    *type: float*, 
    LO WFS pixel scale in [mas]
-   Warning: gives a confusing error message if missing
+
+   *Warning* : gives a confusing error message if missing
 
 .. option:: FieldOfView 
 
    **Required**, 
    *type: int*, 
    not used. 
    Number of pixels per subaperture
-   Warning: gives a confusing error message if missing
+
+   *Warning* : gives a confusing error message if missing
 
 .. option:: NumberPhotons 
 
    **Required**, 
    *type: list of int*, 
    detected flux in [nph/frame/subaperture]
    Must be the same length as NumberLenslet
@@ -598,15 +628,16 @@
    excess noise factor
 
 .. option:: WindowRadiusWCoG
 
    **Optional**, 
    *type: int*, 
    Radius in pixel of the HWHM of the weights map of the weighted CoG the low order WFS pixels
-   Warning: if set to 'optimize', gain is automatically optimized by TIPTOP (closest int to half of PSF FWHM), otherwise the float value set is used.
+
+   *Warning* : if set to 'optimize', gain is automatically optimized by TIPTOP (closest int to half of PSF FWHM), otherwise the float value set is used.
     
 .. option:: ThresholdWCoG
 
    **Optional**, 
    *type: float*, 
    *default: 0.0*,
    Threshold Number of pixels for windowing the low order WFS pixels
@@ -654,24 +685,26 @@
 
 .. option:: NumberActuators
 
    **Required**, 
    *type: list of int*, 
    Number of actuator on the pupil diameter. why a list of int?
    Must be the same length as DmPitchs
-   Warning: gives a confusing error message if missing
-   Warning: not used in TIPTOP!
+
+   *Warning* : gives a confusing error message if missing
+   *Warning* : not used in TIPTOP!
 
 .. option:: DmPitchs
 
    **Required**, 
    *type: list of float*, 
    DM actuators pitch in meters, on the meta pupil at the conjugasion altitude, used for fitting error computation.
    Must be the same length as NumberActuators?
-   Warning: gives a confusing error message if missing
+
+   *Warning* : gives a confusing error message if missing
 
 .. option:: InfModel
 
    **Optional**, 
    *type: str*, 
    *default: 'gaussian'*,
    DM influence function model. Not used in TIPTOP but used in the psf reconstruction. What are the other possible one?
@@ -746,15 +779,16 @@
 
 .. option:: LoopGain_HO
 
    **Optional**, 
    *Type : float*, 
    *Default : 0.5*, 
    High Order Loop gain.
-   Warning: if system to be simulated is a multi-conjugate system this parameter is not used.
+
+   *Warning* : if system to be simulated is a multi-conjugate system this parameter is not used.
 
 .. option:: SensorFrameRate_HO
 
    **Optional**, 
    *type: float*, 
    *Default : 500.0*,
    High Order loop frequency in [Hz]
@@ -768,15 +802,16 @@
 
 .. option:: LoopGain_LO
 
    **Optional**, 
    *type: float or string*, 
    *default: None*,
    Low Order loop gain
-   Warning: if set to 'optimize', gain is automatically optimized by tiptop, otherwise the float value set is used.
+
+   *Warning* : if set to 'optimize', gain is automatically optimized by tiptop, otherwise the float value set is used.
 
 .. option:: SensorFrameRate_LO
 
    **Required**, 
    *type: float*, 
    *default: None*,
    Loop frequency in [Hz]
```

### Comparing `astro-tiptop-1.3.7/docs/source/usage.rst` & `astro_tiptop-1.3.8/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/docs/source/wishList.rst` & `astro_tiptop-1.3.8/docs/source/wishList.rst`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/main_sphere_test.ipynb` & `astro_tiptop-1.3.8/main_sphere_test.ipynb`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/perfTest/ERIS.ini` & `astro_tiptop-1.3.8/perfTest/ERIS.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/perfTest/ERIS_LGS.ini` & `astro_tiptop-1.3.8/perfTest/ERIS_LGS.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/perfTest/HarmoniLTAO_1.ini` & `astro_tiptop-1.3.8/perfTest/HarmoniLTAO_1.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/perfTest/HarmoniLTAO_2.ini` & `astro_tiptop-1.3.8/perfTest/HarmoniLTAO_2.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/perfTest/HarmoniLTAO_3.ini` & `astro_tiptop-1.3.8/perfTest/HarmoniLTAO_3.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/perfTest/HarmoniSCAO_1.ini` & `astro_tiptop-1.3.8/perfTest/HarmoniSCAO_1.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/perfTest/HarmoniSCAO_2.ini` & `astro_tiptop-1.3.8/perfTest/HarmoniSCAO_2.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/perfTest/HarmoniSCAO_3.ini` & `astro_tiptop-1.3.8/perfTest/HarmoniSCAO_3.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/perfTest/MAVIS.ini` & `astro_tiptop-1.3.8/perfTest/MAVIS.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/perfTest/SOUL.ini` & `astro_tiptop-1.3.8/perfTest/SOUL.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/perfTest/SPHERE.ini` & `astro_tiptop-1.3.8/perfTest/SPHERE.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/pyproject.toml` & `astro_tiptop-1.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 urls = {repository = "https://github.com/astro-tiptop/TIPTOP"}
 requires-python = ">=3.9"
 license = {text = "MIT License"}
 dependencies = [
     "matplotlib",
     "numpy",
     "pyyaml",
-    "astro-p3>=1.2.10",
-    "mastsel>=1.2.6",
+    "astro-p3>=1.2.11",
+    "mastsel>=1.2.7",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 docs = ["sphinx"]
 gpu = ["mastsel[gpu]"]
 gui = ["ipywidgets"]
```

### Comparing `astro-tiptop-1.3.7/tests/allTests.py` & `astro_tiptop-1.3.8/tests/allTests.py`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/tiptop/asterismSimulation.py` & `astro_tiptop-1.3.8/tiptop/asterismSimulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -619,15 +619,15 @@
 
     def plotField(self, fieldIndex1):
         self.selectData(fieldIndex1)
         print("*")
         print("* Plotting Field " + str(fieldIndex1) + " - number of asterisms :" + str(self.currentFieldsize))
         print("*")
         print('self.covsarray.shape', self.covsarray.shape)
-        print('self.cov_ellipses_Asterism.shape', self.cov_ellipses_Asterism.shape)
+        print('len(self.cov_ellipses_Asterism)', len(self.cov_ellipses_Asterism))
         if self.covsarray.shape[0]!=0:
             self.twoPlots()
 
 
     def computeAsterisms(self, eeRadiusInMas):
         self.sr_Asterism = []
         self.fwhm_Asterism = []
```

### Comparing `astro-tiptop-1.3.7/tiptop/baseSimulation.py` & `astro_tiptop-1.3.8/tiptop/baseSimulation.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,16 @@
             return False
     
     def __init__(self, path, parametersFile, outputDir, outputFile, doConvolve=False,
                           doPlot=False, addSrAndFwhm=False,
                           verbose=False, getHoErrorBreakDown=False,
                           savePSDs=False):
 
+        if verbose: np.set_printoptions(precision=3)
+        
         # copy the parameters in state vars
         self.path = path
         self.parametersFile = parametersFile
         self.outputDir = outputDir
         self.outputFile = outputFile
         self.doPlot = doPlot
         self.doConvolve = doConvolve
@@ -74,25 +76,28 @@
             #Verify the presence of parameters called in TIPTOP before they are verified 
             #in P3 or in MASTSEL
             if not self.check_section_key('telescope'):
                 self.raiseMissingRequiredSec('telescope')
                 
             if not self.check_config_key('telescope','TelescopeDiameter'):
                 self.raiseMissingRequiredOpt('telescope','TelescopeDiameter')
-                
+            
+            if not self.check_config_key('telescope','glFocusOnNGS'):
+                self.my_data_map['telescope']['glFocusOnNGS'] = False
+            
             if not self.check_section_key('sources_science') :
                 self.raiseMissingRequiredSec('sources_science') 
-                
+            
             if not self.check_config_key('sources_science','Wavelength'):
                 self.raiseMissingRequiredOpt('sources_science', 'Wavelength')
             
             if not self.check_config_key('sources_science','Zenith'):
                 #In P3.aoSystem this is optionnal, to remain consistent it is optionnal here too
                 self.my_data_map['sources_science']['Zenith'] = [0.0]
-                
+            
             if not self.check_config_key('sources_science','Azimuth'):
                 #In P3.aoSystem this is optionnal, to remain consistent it is optionnal here too
                 self.my_data_map['sources_science']['Azimuth'] = [0.0]
             
             if (len(self.my_data_map['sources_science']['Zenith']) != 
                 len(self.my_data_map['sources_science']['Azimuth'])):
                 self.raiseNotSameLength('sources_science', ['Zenith','Azimuth'])
@@ -150,15 +155,19 @@
             self.LOisOn = False
             self.nNaturalGS_field = 0
             if self.verbose: print('LO part is not present')
             
         # initialize self.jitter_FWHM variable with a default value
         self.jitter_FWHM = None
         if 'jitter_FWHM' in self.my_data_map['telescope'].keys():
-            self.jitter_FWHM = self.my_data_map['telescope']['jitter_FWHM']            
+            self.jitter_FWHM = self.my_data_map['telescope']['jitter_FWHM']  
+            
+        self.addFocusError = self.my_data_map['telescope']['glFocusOnNGS']
+        if self.addFocusError and max(self.my_data_map['sensor_LO']['NumberLenslets']) == 1:
+            raise ValueError("[telescope] glFocusOnNGS (that is focus correction with NGS) is available only if NGS WFSs have more than one sub-aperture")
 
 
     def configLO(self, astIndex=None):      
         self.cartSciencePointingCoords = np.dstack( (self.xxSciencePointigs, self.yySciencePointigs) ).reshape(-1, 2)
         # Here we assume the same wavelenght for all the phon counts of the stars in the asterism
         LO_wvl_temp = self.my_data_map['sources_LO']['Wavelength']
 
@@ -324,16 +333,16 @@
             sources_SR.append(SR)
             FWHMx,FWHMy  = getFWHM( psfLE.sampling, pixelscale, method='contour', nargout=2)
             FWHM         = np.sqrt(FWHMx*FWHMy) #max(FWHMx, FWHMy) #0.5*(FWHMx+FWHMy) #average over major and minor axes
 
             # note : the uncertainities on the FWHM seems to create a bug in mavisLO
             sources_FWHM_mas.append(FWHM)
             if self.verbose:
-                print('SR(@',int(wavelength*1e9),'nm)  :', SR)
-                print('FWHM(@',int(wavelength*1e9),'nm):', FWHM)
+                print('SR(@',int(wavelength*1e9),'nm)        :', "%.5f" % SR)
+                print('FWHM(@',int(wavelength*1e9),'nm) [mas]:', "%.3f" % FWHM)
             i += 1
 
         return sources_SR, psdArray, psfLongExpArr, sources_FWHM_mas
 
 
     def computeOL_PSD(self):
         # OPEN-LOOP PSD
@@ -375,15 +384,23 @@
             for n in range(self.cov_ellipses.shape[0]):
                 print('cov_ellipses #',n,': ', self.cov_ellipses[n,:], ' (unit: rad, mas, mas)')
             print('******** FINAL CONVOLUTION')
         # FINAl CONVOLUTION
         # Optimization: Non NEED to perform this convolutions if this is the asterism selection procedure ???
         for ellp, psfLongExp in zip(self.cov_ellipses, self.psfLongExpPointingsArr):
             resSpec = residualToSpectrum(ellp, self.wvl, self.nPixPSF, 1/(self.fao.ao.cam.fovInPix * self.psInMas[0]))
-            self.results.append(convolve(psfLongExp, resSpec))
+            temp = convolve(psfLongExp, resSpec)
+            if self.jitter_FWHM is not None:
+                if isinstance(self.jitter_FWHM, list):
+                    ellpJ = [self.jitter_FWHM[2], sigma_from_FWHM(self.jitter_FWHM[0]), sigma_from_FWHM(self.jitter_FWHM[1])]
+                else:
+                    ellpJ = [0, sigma_from_FWHM(self.jitter_FWHM), sigma_from_FWHM(self.jitter_FWHM)]
+                resSpecJ = residualToSpectrum(ellpJ, self.wvl, self.nPixPSF, 1/(self.fao.ao.cam.fovInPix * self.psInMas[0]))
+                temp = convolve(temp, resSpecJ)
+            self.results.append(temp)
 
 
     def computeMetrics(self, eeRadiusInMas=50):
         if self.verbose:
             print('EE is computed for a radius of ', eeRadiusInMas,' mas')            
         self.sr, self.fwhm, self.ee = [], [], []
         for img in self.results:
@@ -396,14 +413,16 @@
 
     def doOverallSimulation(self, astIndex=None):
 
         if self.LOisOn:        
             self.configLO(astIndex)
         
         self.results = []
+        
+        # ------------------------------------------------------------------------
         # HO Part with P3 PSDs
         if self.verbose:
             print('******** HO PSD science and NGSs directions')
         if astIndex is None or astIndex==0:
             self.fao = fourierModel( self.fullPathFilename, calcPSF=False, verbose=self.verbose
                                , display=False, getPSDatNGSpositions=self.LOisOn
                                , computeFocalAnisoCov=False, TiltFilter=self.LOisOn
@@ -414,16 +433,17 @@
                 self.fao.ao.my_data_map['sensor_LO']['NumberPhotons'] = self.my_data_map['sensor_LO']['NumberPhotons']
             if 'sources_LO' in self.my_data_map.keys():
                 self.fao.my_data_map['sources_LO'] = self.my_data_map['sources_LO']
                 self.fao.ao.my_data_map['sources_LO'] = self.my_data_map['sources_LO']
                 self.fao.ao.configLOsensor()
                 self.fao.ao.configLO()
                 self.fao.ao.configLO_SC()
-
+            
             self.fao.initComputations()
+                 
             # High-order PSD caculations at the science directions and NGSs directions
             self.PSD           = self.fao.PSD # in nm^2
             self.PSD           = self.PSD.transpose()
             self.N             = self.PSD[0].shape[0]
             self.nPointings    = self.pointings.shape[1]
             self.nPixPSF       = int(self.fao.freq.nOtf /self.fao.freq.kRef_)
             if isinstance(self.fao.freq.k_, list):
@@ -437,15 +457,24 @@
             self.dk            = 1e9*self.fao.freq.kcMax_/self.fao.freq.resAO
             # Define the pupil shape
             self.mask = Field(self.wvl, self.N, self.grid_diameter)
             self.psInMas = cpuArray(self.fao.freq.psInMas)
             self.mask.sampling = congrid(arrayP3toMastsel(self.fao.ao.tel.pupil), [self.sx, self.sx])
             self.mask.sampling = zeroPad(self.mask.sampling, (self.N-self.sx)//2)
             
+            if self.verbose:
+                print('fao.samp:', self.fao.freq.samp)
+                print('fao.PSD.shape:', self.fao.PSD.shape)
+                print('fao.freq.psInMas:', self.psInMas)
+            
+            # ------------------------------------------------------------------------
+            # optional LO part
             if self.LOisOn:
+                if self.verbose:
+                    print('******** LO PART')
                 # Define the LO sub-aperture shape
                 nSA = self.my_data_map['sensor_LO']['NumberLenslets']
                 pupilSidePix = int(self.fao.ao.tel.pupil.shape[0])
                 saMask = np.zeros((pupilSidePix,pupilSidePix))
                 if len(nSA) == self.nNaturalGS_field:
                     self.maskLO = []
                     nMaskLO = self.nNaturalGS_field
@@ -475,85 +504,58 @@
                         else:
                             maskLO.sampling = congrid(saMask, [self.sx, self.sx])
                         maskLO.sampling = zeroPad(maskLO.sampling, (self.N-self.sx)//2)
                         if nMaskLO > 1:
                             self.maskLO.append(maskLO)
                         else:
                             self.maskLO = maskLO
-            if self.verbose:
-                print('fao.samp:', self.fao.freq.samp)
-                print('fao.PSD.shape:', self.fao.PSD.shape)
-                print('fao.freq.psInMas:', self.psInMas)
-            # HO PSF
-            if self.verbose:
-                print('******** HO PSF')
-            pointings_SR, psdPointingsArray, psfLongExpPointingsArr, pointings_FWHM_mas = self.psdSetToPsfSet(self.N, 
-                                                                                                         self.freq_range, 
-                                                                                                         self.dk,
-                                                                                                         self.mask, 
-                                                                                                         arrayP3toMastsel(self.PSD[0:self.nPointings]),
-                                                                                                         self.wvl,
-                                                                                                         self.psInMas[0],
-                                                                                                         self.nPixPSF,
-                                                                                                         scaleFactor=(2*np.pi*1e-9/self.wvl)**2,
-                                                                                                         oversampling=self.oversampling)
-            self.psfLongExpPointingsArr = psfLongExpPointingsArr
-            
-        # old version: if not self.LOisOn or (not self.doConvolve and not self.returnRes):
-        if not self.LOisOn:
-            for psfLongExp in self.psfLongExpPointingsArr:
-                if self.jitter_FWHM is not None:
-                    if isinstance(self.jitter_FWHM, list):
-                        ellp = [self.jitter_FWHM[2], sigma_from_FWHM(self.jitter_FWHM[0]), sigma_from_FWHM(self.jitter_FWHM[1])]
-                    else:
-                        ellp = [0, sigma_from_FWHM(self.jitter_FWHM), sigma_from_FWHM(self.jitter_FWHM)]
-                        
-                    self.results.append(convolve(psfLongExp,
-                                   residualToSpectrum(ellp, self.wvl, self.nPixPSF, 1/(self.fao.ao.cam.fovInPix * self.psInMas[0]))))
-                else:
-                    self.results.append(psfLongExp)
-        else:
-            if astIndex is None or astIndex==0:
-                # LOW ORDER PART
-                if self.verbose:
-                    print('******** LO PART')
+
                 self.psInMas_NGS        = self.psInMas[0] * (self.LO_wvl/self.wvl) # airy pattern PSF FWHM
                 if self.verbose:
-                    print('******** HO PSF - NGS directions')
+                    print('******** HO PSF - NGS directions (1 sub-aperture)')
 
-                NGS_SR, psdArray, psfLE_NGS, NGS_FWHM_mas = self.psdSetToPsfSet(self.N, 
-                                                                           self.freq_range, 
-                                                                           self.dk, 
-                                                                           self.maskLO, 
-                                                                           arrayP3toMastsel(self.PSD[-self.nNaturalGS_field:]), 
-                                                                           self.LO_wvl, 
-                                                                           self.psInMas_NGS, 
+                NGS_SR, psdArray, psfLE_NGS, NGS_FWHM_mas = self.psdSetToPsfSet(self.N,
+                                                                           self.freq_range,
+                                                                           self.dk,
+                                                                           self.maskLO,
+                                                                           arrayP3toMastsel(self.PSD[-self.nNaturalGS_field:]),
+                                                                           self.LO_wvl,
+                                                                           self.psInMas_NGS,
                                                                            self.nPixPSF,
                                                                            scaleFactor=(2*np.pi*1e-9/self.LO_wvl)**2,
                                                                            oversampling=self.oversampling)
                 self.NGS_SR_field           = NGS_SR
                 self.NGS_FWHM_mas_field     = NGS_FWHM_mas
                 self.NGS_EE_field = []
                 idx = 0
                 for img in psfLE_NGS:
                     ee_,rr_ = getEncircledEnergy(img.sampling, pixelscale=self.psInMas[0], center=(self.fao.ao.cam.fovInPix/2,self.fao.ao.cam.fovInPix/2), nargout=2)
                     ee_ *= 1/np.max(ee_)
                     ee_at_radius_fn = interp1d(rr_, ee_, kind='cubic', bounds_error=False)
                     self.NGS_EE_field.append(ee_at_radius_fn(NGS_FWHM_mas[idx]))
                     if self.verbose:
-                        print('ee:', ee_at_radius_fn(NGS_FWHM_mas[idx]))
-                        print('fwhm:',NGS_FWHM_mas[idx])
+                        print('EE                   :', "%.5f" % ee_at_radius_fn(NGS_FWHM_mas[idx]))
                     idx += 1
                 self.mLO           = MavisLO(self.path, self.parametersFile, verbose=self.verbose)
 
             if astIndex is None:
                 self.Ctot          = self.mLO.computeTotalResidualMatrix(np.array(self.cartSciencePointingCoords),
                                                                          self.cartNGSCoords_field, self.NGS_fluxes_field,
                                                                          self.LO_freqs_field,
                                                                          self.NGS_SR_field, self.NGS_EE_field, self.NGS_FWHM_mas_field, doAll=True)
+                if self.addFocusError:
+                    # compute focus error
+                    self.CtotFocus = self.mLO.computeFocusTotalResidualMatrix(self.cartNGSCoords_field, self.NGS_fluxes_field,
+                                                                         self.LO_freqs_field,
+                                                                         self.NGS_SR_field, self.NGS_EE_field, self.NGS_FWHM_mas_field)
+                    # add focus error to PSD using P3 FocusFilter
+                    for PSDho in self.PSD:
+                        FocusFilter = self.fao.FocusFilter()
+                        FocusFilter *= 1/FocusFilter.sum()
+                        PSDho += self.CtotFocus[0] * FocusFilter
 
             else:
                 self.NGS_SR_asterism = []
                 for iid in self.currentAsterismIndices:
                     self.NGS_SR_asterism.append(self.NGS_SR_field[iid])
                 self.NGS_FWHM_mas_asterism = []
                 for iid in self.currentAsterismIndices:
@@ -564,24 +566,58 @@
                                                         self.LO_freqs_field,
                                                         self.NGS_SR_field, self.NGS_EE_field, self.NGS_FWHM_mas_field, doAll=False)
                 self.Ctot          = self.mLO.computeTotalResidualMatrixI(self.currentAsterismIndices,
                                                                           np.array(self.cartSciencePointingCoords),
                                                                           np.array(self.cartNGSCoords_asterism), self.NGS_fluxes_asterism,
                                                                           self.LO_freqs_asterism,
                                                                           self.NGS_SR_asterism, self.NGS_EE_field, self.NGS_FWHM_mas_asterism)
-                
+                #TODO add self.CtotFocus computation only for the best asterism
+                #if self.addFocusError:
+                #    ...
+        
+        # ------------------------------------------------------------------------
+        # HO PSF
+        if self.verbose:
+            print('******** HO PSF')
+        pointings_SR, psdPointingsArray, psfLongExpPointingsArr, pointings_FWHM_mas = self.psdSetToPsfSet(self.N, 
+                                                                                                     self.freq_range, 
+                                                                                                     self.dk,
+                                                                                                     self.mask, 
+                                                                                                     arrayP3toMastsel(self.PSD[0:self.nPointings]),
+                                                                                                     self.wvl,
+                                                                                                     self.psInMas[0],
+                                                                                                     self.nPixPSF,
+                                                                                                     scaleFactor=(2*np.pi*1e-9/self.wvl)**2,
+                                                                                                     oversampling=self.oversampling)
+        self.psfLongExpPointingsArr = psfLongExpPointingsArr
+        
+        # ------------------------------------------------------------------------
+        # final results computation after optional convolution with jitter kernels
+        if not self.LOisOn:
+            for psfLongExp in self.psfLongExpPointingsArr:
+                if self.jitter_FWHM is not None:
+                    if isinstance(self.jitter_FWHM, list):
+                        ellp = [self.jitter_FWHM[2], sigma_from_FWHM(self.jitter_FWHM[0]), sigma_from_FWHM(self.jitter_FWHM[1])]
+                    else:
+                        ellp = [0, sigma_from_FWHM(self.jitter_FWHM), sigma_from_FWHM(self.jitter_FWHM)]
+                    self.results.append(convolve(psfLongExp,
+                                   residualToSpectrum(ellp, self.wvl, self.nPixPSF, 1/(self.fao.ao.cam.fovInPix * self.psInMas[0]))))
+                else:
+                    self.results.append(psfLongExp)
+        else:
             if self.doConvolve:
                 if astIndex is None:
                     self.finalConvolution()
                 else:
                     self.cov_ellipses = self.mLO.ellipsesFromCovMats(self.Ctot)
             else:
                 for psfLongExp in self.psfLongExpPointingsArr:
                     self.results.append(psfLongExp)
- 
+        # ------------------------------------------------------------------------
+        
         if self.doPlot:
             if self.LOisOn and self.doConvolve:
                 tiledDisplay(self.results)
                 plotEllipses(self.cartSciencePointingCoords, self.cov_ellipses, 0.4)
             else:
                 self.results[0].standardPlot(True)
```

### Comparing `astro-tiptop-1.3.7/tiptop/tiptop.py` & `astro_tiptop-1.3.8/tiptop/tiptop.py`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/tiptop/tiptopCLT.py` & `astro_tiptop-1.3.8/tiptop/tiptopCLT.py`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/tiptop/tiptopGUI.py` & `astro_tiptop-1.3.8/tiptop/tiptopGUI.py`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.3.7/tiptop/tiptopUtils.py` & `astro_tiptop-1.3.8/tiptop/tiptopUtils.py`

 * *Files identical despite different names*

