# Comparing `tmp/xfem-2.1.2303.post72.dev0.tar.gz` & `tmp/xfem-2.1.2303.post8.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xfem-2.1.2303.post72.dev0.tar", last modified: Wed Apr 10 09:00:57 2024, max compression
+gzip compressed data, was "xfem-2.1.2303.post8.dev0.tar", last modified: Sun Jul  9 06:12:59 2023, max compression
```

## Comparing `xfem-2.1.2303.post72.dev0.tar` & `xfem-2.1.2303.post8.dev0.tar`

### file list

```diff
@@ -1,118 +1,132 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:00:57.910616 xfem-2.1.2303.post72.dev0/
--rw-r--r--   0 root         (0) root         (0)     7708 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     7650 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      241 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      644 2024-04-10 09:00:57.910616 xfem-2.1.2303.post72.dev0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8498 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:00:57.878616 xfem-2.1.2303.post72.dev0/build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:00:57.878616 xfem-2.1.2303.post72.dev0/build/temp.linux-x86_64-cpython-310/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:00:57.878616 xfem-2.1.2303.post72.dev0/build/temp.linux-x86_64-cpython-310/CMakeFiles/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:00:57.878616 xfem-2.1.2303.post72.dev0/build/temp.linux-x86_64-cpython-310/CMakeFiles/3.25.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:00:57.882616 xfem-2.1.2303.post72.dev0/build/temp.linux-x86_64-cpython-310/CMakeFiles/3.25.0/CompilerIdCXX/
--rw-r--r--   0 root         (0) root         (0)    26294 2024-04-10 08:58:24.000000 xfem-2.1.2303.post72.dev0/build/temp.linux-x86_64-cpython-310/CMakeFiles/3.25.0/CompilerIdCXX/CMakeCXXCompilerId.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:00:57.882616 xfem-2.1.2303.post72.dev0/cmake_modules/
--rw-r--r--   0 root         (0) root         (0)     1035 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/cmake_modules/cmake_uninstall.cmake.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:00:57.886616 xfem-2.1.2303.post72.dev0/cutint/
--rw-r--r--   0 root         (0) root         (0)      214 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/cutint/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     7745 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/cutint/cutintegral.cpp
--rw-r--r--   0 root         (0) root         (0)     4544 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/cutint/cutintegral.hpp
--rw-r--r--   0 root         (0) root         (0)     4241 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/cutint/fieldeval.cpp
--rw-r--r--   0 root         (0) root         (0)     4187 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/cutint/fieldeval.hpp
--rw-r--r--   0 root         (0) root         (0)    12108 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/cutint/lsetintdomain.cpp
--rw-r--r--   0 root         (0) root         (0)     6001 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/cutint/lsetintdomain.hpp
--rw-r--r--   0 root         (0) root         (0)     8046 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/cutint/mlsetintegration.cpp
--rw-r--r--   0 root         (0) root         (0)     1250 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/cutint/mlsetintegration.hpp
--rw-r--r--   0 root         (0) root         (0)    16622 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/cutint/python_cutint.cpp
--rw-r--r--   0 root         (0) root         (0)    18133 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/cutint/spacetimecutrule.cpp
--rw-r--r--   0 root         (0) root         (0)     1516 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/cutint/spacetimecutrule.hpp
--rw-r--r--   0 root         (0) root         (0)    39707 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/cutint/straightcutrule.cpp
--rw-r--r--   0 root         (0) root         (0)     7898 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/cutint/straightcutrule.hpp
--rw-r--r--   0 root         (0) root         (0)     1107 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/cutint/xdecompose.cpp
--rw-r--r--   0 root         (0) root         (0)     3460 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/cutint/xdecompose.hpp
--rw-r--r--   0 root         (0) root         (0)    62846 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/cutint/xintegration.cpp
--rw-r--r--   0 root         (0) root         (0)    30845 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/cutint/xintegration.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:00:57.886616 xfem-2.1.2303.post72.dev0/demos/
--rw-r--r--   0 root         (0) root         (0)      503 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/demos/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:00:57.890616 xfem-2.1.2303.post72.dev0/lsetcurving/
--rw-r--r--   0 root         (0) root         (0)      158 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/lsetcurving/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6959 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/lsetcurving/calcpointshift.cpp
--rw-r--r--   0 root         (0) root         (0)     1911 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/lsetcurving/calcpointshift.hpp
--rw-r--r--   0 root         (0) root         (0)     1391 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/lsetcurving/lsetrefine.cpp
--rw-r--r--   0 root         (0) root         (0)      633 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/lsetcurving/lsetrefine.hpp
--rw-r--r--   0 root         (0) root         (0)     7410 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/lsetcurving/projshift.cpp
--rw-r--r--   0 root         (0) root         (0)      634 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/lsetcurving/projshift.hpp
--rw-r--r--   0 root         (0) root         (0)     6600 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/lsetcurving/python_lsetcurving.cpp
--rw-r--r--   0 root         (0) root         (0)     9919 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/lsetcurving/shiftedevaluate.cpp
--rw-r--r--   0 root         (0) root         (0)     2208 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/lsetcurving/shiftedevaluate.hpp
--rw-r--r--   0 root         (0) root         (0)     4356 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/lsetcurving/shiftintegrators.cpp
--rw-r--r--   0 root         (0) root         (0)     1595 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/lsetcurving/shiftintegrators.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:00:57.906616 xfem-2.1.2303.post72.dev0/python/
--rw-r--r--   0 root         (0) root         (0)     2645 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/python/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    39498 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/python/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15725 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/python/cutmg.py
--rw-r--r--   0 root         (0) root         (0)     4922 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/python/lset_smoothblend.py
--rw-r--r--   0 root         (0) root         (0)    21357 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/python/lset_spacetime.py
--rw-r--r--   0 root         (0) root         (0)    12837 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/python/lsetcurv.py
--rw-r--r--   0 root         (0) root         (0)    18823 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/python/mlset.py
--rw-r--r--   0 root         (0) root         (0)     1224 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/python/ngs_check.py
--rw-r--r--   0 root         (0) root         (0)     1413 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/python/python_ngsxfem.cpp
--rw-r--r--   0 root         (0) root         (0)     1517 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/python/utils.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 09:00:57.910616 xfem-2.1.2303.post72.dev0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     5366 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:00:57.894616 xfem-2.1.2303.post72.dev0/spacetime/
--rw-r--r--   0 root         (0) root         (0)      152 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/spacetime/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    12850 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/spacetime/SpaceTimeFE.cpp
--rw-r--r--   0 root         (0) root         (0)     4721 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/spacetime/SpaceTimeFE.hpp
--rw-r--r--   0 root         (0) root         (0)     9545 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/spacetime/SpaceTimeFESpace.cpp
--rw-r--r--   0 root         (0) root         (0)     2672 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/spacetime/SpaceTimeFESpace.hpp
--rw-r--r--   0 root         (0) root         (0)     4536 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/spacetime/diffopDt.cpp
--rw-r--r--   0 root         (0) root         (0)     4729 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/spacetime/diffopDt.hpp
--rw-r--r--   0 root         (0) root         (0)    17332 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/spacetime/python_spacetime.cpp
--rw-r--r--   0 root         (0) root         (0)    11123 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/spacetime/spacetime_vtk.cpp
--rw-r--r--   0 root         (0) root         (0)     1766 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/spacetime/spacetime_vtk.hpp
--rw-r--r--   0 root         (0) root         (0)     5304 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/spacetime/timecf.cpp
--rw-r--r--   0 root         (0) root         (0)     2514 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/spacetime/timecf.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:00:57.894616 xfem-2.1.2303.post72.dev0/tests/
--rw-r--r--   0 root         (0) root         (0)     6002 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/tests/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:00:57.898616 xfem-2.1.2303.post72.dev0/utils/
--rw-r--r--   0 root         (0) root         (0)      175 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/utils/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1055 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/utils/bitarraycf.cpp
--rw-r--r--   0 root         (0) root         (0)      622 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/utils/bitarraycf.hpp
--rw-r--r--   0 root         (0) root         (0)     3248 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/utils/ngsxstd.cpp
--rw-r--r--   0 root         (0) root         (0)     3563 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/utils/ngsxstd.hpp
--rw-r--r--   0 root         (0) root         (0)     4075 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/utils/p1interpol.cpp
--rw-r--r--   0 root         (0) root         (0)     1302 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/utils/p1interpol.hpp
--rw-r--r--   0 root         (0) root         (0)    17275 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/utils/python_utils.cpp
--rw-r--r--   0 root         (0) root         (0)     5782 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/utils/restrictedblf.cpp
--rw-r--r--   0 root         (0) root         (0)     2073 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/utils/restrictedblf.hpp
--rw-r--r--   0 root         (0) root         (0)     9444 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/utils/restrictedfespace.cpp
--rw-r--r--   0 root         (0) root         (0)     6629 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/utils/restrictedfespace.hpp
--rw-r--r--   0 root         (0) root         (0)    13017 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/utils/xprolongation.cpp
--rw-r--r--   0 root         (0) root         (0)     3078 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/utils/xprolongation.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:00:57.902616 xfem-2.1.2303.post72.dev0/xfem/
--rw-r--r--   0 root         (0) root         (0)      226 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/xfem/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    24796 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/xfem/aggregates.cpp
--rw-r--r--   0 root         (0) root         (0)     3377 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/xfem/aggregates.hpp
--rw-r--r--   0 root         (0) root         (0)    22027 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/xfem/cutinfo.cpp
--rw-r--r--   0 root         (0) root         (0)     6707 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/xfem/cutinfo.hpp
--rw-r--r--   0 root         (0) root         (0)    13722 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/xfem/ghostpenalty.cpp
--rw-r--r--   0 root         (0) root         (0)     3652 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/xfem/ghostpenalty.hpp
--rw-r--r--   0 root         (0) root         (0)    45551 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/xfem/python_xfem.cpp
--rw-r--r--   0 root         (0) root         (0)     4155 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/xfem/sFESpace.cpp
--rw-r--r--   0 root         (0) root         (0)     1612 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/xfem/sFESpace.hpp
--rw-r--r--   0 root         (0) root         (0)    76189 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/xfem/symboliccutbfi.cpp
--rw-r--r--   0 root         (0) root         (0)    19371 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/xfem/symboliccutbfi.hpp
--rw-r--r--   0 root         (0) root         (0)     4362 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/xfem/symboliccutlfi.cpp
--rw-r--r--   0 root         (0) root         (0)     1256 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/xfem/symboliccutlfi.hpp
--rw-r--r--   0 root         (0) root         (0)    19223 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/xfem/xFESpace.cpp
--rw-r--r--   0 root         (0) root         (0)     5786 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/xfem/xFESpace.hpp
--rw-r--r--   0 root         (0) root         (0)     2926 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/xfem/xfemdiffops.cpp
--rw-r--r--   0 root         (0) root         (0)     2150 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/xfem/xfemdiffops.hpp
--rw-r--r--   0 root         (0) root         (0)     1689 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/xfem/xfiniteelement.cpp
--rw-r--r--   0 root         (0) root         (0)     2272 2024-04-10 08:57:58.000000 xfem-2.1.2303.post72.dev0/xfem/xfiniteelement.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:00:57.910616 xfem-2.1.2303.post72.dev0/xfem.egg-info/
--rw-r--r--   0 root         (0) root         (0)      644 2024-04-10 09:00:57.000000 xfem-2.1.2303.post72.dev0/xfem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2615 2024-04-10 09:00:57.000000 xfem-2.1.2303.post72.dev0/xfem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 09:00:57.000000 xfem-2.1.2303.post72.dev0/xfem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-10 09:00:57.000000 xfem-2.1.2303.post72.dev0/xfem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-10 09:00:57.000000 xfem-2.1.2303.post72.dev0/xfem.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.629639 xfem-2.1.2303.post8.dev0/
+-rw-r--r--   0 root         (0) root         (0)     7455 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     7650 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      241 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-09 06:12:59.629639 xfem-2.1.2303.post8.dev0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8526 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.589639 xfem-2.1.2303.post8.dev0/build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.589639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-310/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.589639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-310/CMakeFiles/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.589639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-310/CMakeFiles/3.25.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.593639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-310/CMakeFiles/3.25.0/CompilerIdCXX/
+-rw-r--r--   0 root         (0) root         (0)    26294 2023-07-09 06:04:20.000000 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-310/CMakeFiles/3.25.0/CompilerIdCXX/CMakeCXXCompilerId.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.589639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-311/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.589639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-311/CMakeFiles/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.589639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-311/CMakeFiles/3.25.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.593639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-311/CMakeFiles/3.25.0/CompilerIdCXX/
+-rw-r--r--   0 root         (0) root         (0)    26294 2023-07-09 06:08:52.000000 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-311/CMakeFiles/3.25.0/CompilerIdCXX/CMakeCXXCompilerId.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.589639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-38/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.589639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-38/CMakeFiles/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.589639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-38/CMakeFiles/3.25.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.593639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-38/CMakeFiles/3.25.0/CompilerIdCXX/
+-rw-r--r--   0 root         (0) root         (0)    26294 2023-07-09 05:59:46.000000 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-38/CMakeFiles/3.25.0/CompilerIdCXX/CMakeCXXCompilerId.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.589639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-39/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.589639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-39/CMakeFiles/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.589639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-39/CMakeFiles/3.25.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.597639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-39/CMakeFiles/3.25.0/CompilerIdCXX/
+-rw-r--r--   0 root         (0) root         (0)    26294 2023-07-09 05:55:12.000000 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-39/CMakeFiles/3.25.0/CompilerIdCXX/CMakeCXXCompilerId.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.597639 xfem-2.1.2303.post8.dev0/cmake_modules/
+-rw-r--r--   0 root         (0) root         (0)     1035 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cmake_modules/cmake_uninstall.cmake.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.605639 xfem-2.1.2303.post8.dev0/cutint/
+-rw-r--r--   0 root         (0) root         (0)      214 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     7745 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/cutintegral.cpp
+-rw-r--r--   0 root         (0) root         (0)     4544 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/cutintegral.hpp
+-rw-r--r--   0 root         (0) root         (0)     4241 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/fieldeval.cpp
+-rw-r--r--   0 root         (0) root         (0)     4187 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/fieldeval.hpp
+-rw-r--r--   0 root         (0) root         (0)    12108 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/lsetintdomain.cpp
+-rw-r--r--   0 root         (0) root         (0)     6001 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/lsetintdomain.hpp
+-rw-r--r--   0 root         (0) root         (0)     8068 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/mlsetintegration.cpp
+-rw-r--r--   0 root         (0) root         (0)     1250 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/mlsetintegration.hpp
+-rw-r--r--   0 root         (0) root         (0)    16622 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/python_cutint.cpp
+-rw-r--r--   0 root         (0) root         (0)    18133 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/spacetimecutrule.cpp
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/spacetimecutrule.hpp
+-rw-r--r--   0 root         (0) root         (0)    39707 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/straightcutrule.cpp
+-rw-r--r--   0 root         (0) root         (0)     7898 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/straightcutrule.hpp
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/xdecompose.cpp
+-rw-r--r--   0 root         (0) root         (0)     3460 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/xdecompose.hpp
+-rw-r--r--   0 root         (0) root         (0)    62867 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/xintegration.cpp
+-rw-r--r--   0 root         (0) root         (0)    30845 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/xintegration.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.605639 xfem-2.1.2303.post8.dev0/demos/
+-rw-r--r--   0 root         (0) root         (0)      503 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/demos/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.609639 xfem-2.1.2303.post8.dev0/lsetcurving/
+-rw-r--r--   0 root         (0) root         (0)      158 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/lsetcurving/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     6959 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/lsetcurving/calcpointshift.cpp
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/lsetcurving/calcpointshift.hpp
+-rw-r--r--   0 root         (0) root         (0)     1391 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/lsetcurving/lsetrefine.cpp
+-rw-r--r--   0 root         (0) root         (0)      633 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/lsetcurving/lsetrefine.hpp
+-rw-r--r--   0 root         (0) root         (0)     7410 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/lsetcurving/projshift.cpp
+-rw-r--r--   0 root         (0) root         (0)      634 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/lsetcurving/projshift.hpp
+-rw-r--r--   0 root         (0) root         (0)     6600 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/lsetcurving/python_lsetcurving.cpp
+-rw-r--r--   0 root         (0) root         (0)     9915 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/lsetcurving/shiftedevaluate.cpp
+-rw-r--r--   0 root         (0) root         (0)     2204 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/lsetcurving/shiftedevaluate.hpp
+-rw-r--r--   0 root         (0) root         (0)     4351 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/lsetcurving/shiftintegrators.cpp
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/lsetcurving/shiftintegrators.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.625639 xfem-2.1.2303.post8.dev0/python/
+-rw-r--r--   0 root         (0) root         (0)     2673 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/python/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)    39498 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/python/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15725 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/python/cutmg.py
+-rw-r--r--   0 root         (0) root         (0)    19045 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/python/lset_spacetime.py
+-rw-r--r--   0 root         (0) root         (0)    12837 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/python/lsetcurv.py
+-rw-r--r--   0 root         (0) root         (0)    18823 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/python/mlset.py
+-rw-r--r--   0 root         (0) root         (0)     1224 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/python/ngs_check.py
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/python/python_ngsxfem.cpp
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/python/utils.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 06:12:59.629639 xfem-2.1.2303.post8.dev0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     5366 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.613639 xfem-2.1.2303.post8.dev0/spacetime/
+-rw-r--r--   0 root         (0) root         (0)      152 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/spacetime/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)    12850 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/spacetime/SpaceTimeFE.cpp
+-rw-r--r--   0 root         (0) root         (0)     4721 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/spacetime/SpaceTimeFE.hpp
+-rw-r--r--   0 root         (0) root         (0)     9545 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/spacetime/SpaceTimeFESpace.cpp
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/spacetime/SpaceTimeFESpace.hpp
+-rw-r--r--   0 root         (0) root         (0)     4530 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/spacetime/diffopDt.cpp
+-rw-r--r--   0 root         (0) root         (0)     4725 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/spacetime/diffopDt.hpp
+-rw-r--r--   0 root         (0) root         (0)    17384 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/spacetime/python_spacetime.cpp
+-rw-r--r--   0 root         (0) root         (0)    11113 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/spacetime/spacetime_vtk.cpp
+-rw-r--r--   0 root         (0) root         (0)     1763 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/spacetime/spacetime_vtk.hpp
+-rw-r--r--   0 root         (0) root         (0)     5304 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/spacetime/timecf.cpp
+-rw-r--r--   0 root         (0) root         (0)     2514 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/spacetime/timecf.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.613639 xfem-2.1.2303.post8.dev0/tests/
+-rw-r--r--   0 root         (0) root         (0)     6002 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/tests/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.617639 xfem-2.1.2303.post8.dev0/utils/
+-rw-r--r--   0 root         (0) root         (0)      175 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/bitarraycf.cpp
+-rw-r--r--   0 root         (0) root         (0)      622 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/bitarraycf.hpp
+-rw-r--r--   0 root         (0) root         (0)     3248 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/ngsxstd.cpp
+-rw-r--r--   0 root         (0) root         (0)     3563 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/ngsxstd.hpp
+-rw-r--r--   0 root         (0) root         (0)     3960 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/p1interpol.cpp
+-rw-r--r--   0 root         (0) root         (0)     1302 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/p1interpol.hpp
+-rw-r--r--   0 root         (0) root         (0)    17275 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/python_utils.cpp
+-rw-r--r--   0 root         (0) root         (0)     5777 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/restrictedblf.cpp
+-rw-r--r--   0 root         (0) root         (0)     2073 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/restrictedblf.hpp
+-rw-r--r--   0 root         (0) root         (0)     9284 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/restrictedfespace.cpp
+-rw-r--r--   0 root         (0) root         (0)     6619 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/restrictedfespace.hpp
+-rw-r--r--   0 root         (0) root         (0)    13017 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/xprolongation.cpp
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/xprolongation.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.625639 xfem-2.1.2303.post8.dev0/xfem/
+-rw-r--r--   0 root         (0) root         (0)      226 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)    24796 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/aggregates.cpp
+-rw-r--r--   0 root         (0) root         (0)     3377 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/aggregates.hpp
+-rw-r--r--   0 root         (0) root         (0)    21010 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/cutinfo.cpp
+-rw-r--r--   0 root         (0) root         (0)     6587 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/cutinfo.hpp
+-rw-r--r--   0 root         (0) root         (0)    13722 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/ghostpenalty.cpp
+-rw-r--r--   0 root         (0) root         (0)     3652 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/ghostpenalty.hpp
+-rw-r--r--   0 root         (0) root         (0)    45185 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/python_xfem.cpp
+-rw-r--r--   0 root         (0) root         (0)     4151 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/sFESpace.cpp
+-rw-r--r--   0 root         (0) root         (0)     1612 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/sFESpace.hpp
+-rw-r--r--   0 root         (0) root         (0)    76187 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/symboliccutbfi.cpp
+-rw-r--r--   0 root         (0) root         (0)    19371 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/symboliccutbfi.hpp
+-rw-r--r--   0 root         (0) root         (0)     4362 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/symboliccutlfi.cpp
+-rw-r--r--   0 root         (0) root         (0)     1256 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/symboliccutlfi.hpp
+-rw-r--r--   0 root         (0) root         (0)    19223 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/xFESpace.cpp
+-rw-r--r--   0 root         (0) root         (0)     5786 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/xFESpace.hpp
+-rw-r--r--   0 root         (0) root         (0)     2926 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/xfemdiffops.cpp
+-rw-r--r--   0 root         (0) root         (0)     2150 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/xfemdiffops.hpp
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/xfiniteelement.cpp
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/xfiniteelement.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.629639 xfem-2.1.2303.post8.dev0/xfem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-09 06:12:59.000000 xfem-2.1.2303.post8.dev0/xfem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2865 2023-07-09 06:12:59.000000 xfem-2.1.2303.post8.dev0/xfem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 06:12:59.000000 xfem-2.1.2303.post8.dev0/xfem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-09 06:12:59.000000 xfem-2.1.2303.post8.dev0/xfem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-09 06:12:59.000000 xfem-2.1.2303.post8.dev0/xfem.egg-info/top_level.txt
```

### Comparing `xfem-2.1.2303.post72.dev0/CMakeLists.txt` & `xfem-2.1.2303.post8.dev0/CMakeLists.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 cmake_minimum_required(VERSION 2.8)
 
 project(xfem)
 
-set(BUILD_NGSOLVE OFF CACHE BOOL "build NGSolve from scratch")
+set(BUILD_NGSOLVE ON CACHE BOOL "build NGSolve from scratch")
 set(CHECK_NGSOLVE_VERSION ON CACHE BOOL "Check if installed NGSolve (if exist) is compatible")
 set(CMAKE_BUILD_TYPE RELWITHDEBINFO CACHE STRING "release type")
 set(USE_CCACHE OFF CACHE BOOL "use ccache")
 set(USE_GUI ON CACHE BOOL "use Netgen GUI")
 set(BUILD_STUB_FILES OFF CACHE BOOL "Build stub files for better autocompletion")
 set(SPACETIME_SANITY_CHECKS ON CACHE BOOL "use space-time sanity checks (abuses ngsolve's intrule nr)")
 
@@ -82,25 +82,16 @@
       message(FATAL_ERROR "
 NGSolve version is smaller than required.
 Update NGSolve or downgrade ngsxfem!
 If you know what you are doing you can turn off this check by setting the cmake option CHECK_NGSOLVE_VERSION off: \"cmake -DCHECK_NGSOLVE_VERSION=OFF ...\"
 ")
     endif (NOT ${ngsfits} EQUAL 1)
   endif (CHECK_NGSOLVE_VERSION)
-  if(CMAKE_CROSSCOMPILING)
-  else(CMAKE_CROSSCOMPILING)
-    if (CMAKE_CXX_COMPILER)
-    else (CMAKE_CXX_COMPILER)
-      set(CMAKE_CXX_COMPILER "ngscxx" CACHE STRING "Default CXX compiler" FORCE)
-    endif (CMAKE_CXX_COMPILER)
-    if (CMAKE_LINKER)
-    else (CMAKE_LINKER)
-      set(CMAKE_LINKER "ngsld" CACHE STRING "Default linker" FORCE)
-    endif(CMAKE_LINKER)
-  endif(CMAKE_CROSSCOMPILING)
+  set(CMAKE_CXX_COMPILER "ngscxx" CACHE STRING "Default CXX compiler" FORCE)
+  set(CMAKE_LINKER "ngsld" CACHE STRING "Default linker" FORCE)
 
 endif(BUILD_NGSOLVE)
 
 if(USE_CCACHE)
   find_program(CCACHE_FOUND ccache)
   if(CCACHE_FOUND)
     set_property(GLOBAL PROPERTY RULE_LAUNCH_COMPILE ccache)
@@ -165,14 +156,15 @@
 function(message)
     _MESSAGE("${BoldBlue}${ARGV}${ColorReset}")
 endfunction()
 
 string(TOUPPER "CMAKE_CXX_FLAGS_${CMAKE_BUILD_TYPE}" name)
 set(flags "${${name}} ${CMAKE_CXX_FLAGS}")
 
+
 message("
 ------------------------------------------------------------------------
   ${PROJECT_NAME} ${PACKAGE_VERSION}:  Automatic configuration OK.
 
   Install directory:
     ${CMAKE_INSTALL_PREFIX}
```

### Comparing `xfem-2.1.2303.post72.dev0/LICENSE` & `xfem-2.1.2303.post8.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/README.md` & `xfem-2.1.2303.post8.dev0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,32 +4,31 @@
 
  
 
 [![PyPI](https://img.shields.io/pypi/v/xfem?color=blue&label=latest%20PyPI%20version&logo=pypi&logoColor=white)](https://pypi.org/project/xfem/)
 [![PyPI - Implementation](https://img.shields.io/pypi/implementation/xfem?logo=pypi&logoColor=white)](https://pypi.org/project/xfem/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/xfem?color=green&label=PyPI%20downloads&logo=pypi&logoColor=white)](https://pypi.org/project/xfem/)
 
+[![docker build](https://img.shields.io/docker/cloud/build/ngsxfem/ngsxfem?logo=docker&logoColor=white)](https://hub.docker.com/repository/docker/ngsxfem/ngsxfem) 
 [![Docker Pulls](https://img.shields.io/docker/pulls/ngsxfem/ngsxfem?logo=docker&logoColor=white)](https://hub.docker.com/repository/docker/ngsxfem/ngsxfem) 
 [![badge](https://img.shields.io/badge/launch-jupyter--tutorials-579ACA.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFkAAABZCAMAAABi1XidAAAB8lBMVEX///9XmsrmZYH1olJXmsr1olJXmsrmZYH1olJXmsr1olJXmsrmZYH1olL1olJXmsr1olJXmsrmZYH1olL1olJXmsrmZYH1olJXmsr1olL1olJXmsrmZYH1olL1olJXmsrmZYH1olL1olL0nFf1olJXmsrmZYH1olJXmsq8dZb1olJXmsrmZYH1olJXmspXmspXmsr1olL1olJXmsrmZYH1olJXmsr1olL1olJXmsrmZYH1olL1olLeaIVXmsrmZYH1olL1olL1olJXmsrmZYH1olLna31Xmsr1olJXmsr1olJXmsrmZYH1olLqoVr1olJXmsr1olJXmsrmZYH1olL1olKkfaPobXvviGabgadXmsqThKuofKHmZ4Dobnr1olJXmsr1olJXmspXmsr1olJXmsrfZ4TuhWn1olL1olJXmsqBi7X1olJXmspZmslbmMhbmsdemsVfl8ZgmsNim8Jpk8F0m7R4m7F5nLB6jbh7jbiDirOEibOGnKaMhq+PnaCVg6qWg6qegKaff6WhnpKofKGtnomxeZy3noG6dZi+n3vCcpPDcpPGn3bLb4/Mb47UbIrVa4rYoGjdaIbeaIXhoWHmZYHobXvpcHjqdHXreHLroVrsfG/uhGnuh2bwj2Hxk17yl1vzmljzm1j0nlX1olL3AJXWAAAAbXRSTlMAEBAQHx8gICAuLjAwMDw9PUBAQEpQUFBXV1hgYGBkcHBwcXl8gICAgoiIkJCQlJicnJ2goKCmqK+wsLC4usDAwMjP0NDQ1NbW3Nzg4ODi5+3v8PDw8/T09PX29vb39/f5+fr7+/z8/Pz9/v7+zczCxgAABC5JREFUeAHN1ul3k0UUBvCb1CTVpmpaitAGSLSpSuKCLWpbTKNJFGlcSMAFF63iUmRccNG6gLbuxkXU66JAUef/9LSpmXnyLr3T5AO/rzl5zj137p136BISy44fKJXuGN/d19PUfYeO67Znqtf2KH33Id1psXoFdW30sPZ1sMvs2D060AHqws4FHeJojLZqnw53cmfvg+XR8mC0OEjuxrXEkX5ydeVJLVIlV0e10PXk5k7dYeHu7Cj1j+49uKg7uLU61tGLw1lq27ugQYlclHC4bgv7VQ+TAyj5Zc/UjsPvs1sd5cWryWObtvWT2EPa4rtnWW3JkpjggEpbOsPr7F7EyNewtpBIslA7p43HCsnwooXTEc3UmPmCNn5lrqTJxy6nRmcavGZVt/3Da2pD5NHvsOHJCrdc1G2r3DITpU7yic7w/7Rxnjc0kt5GC4djiv2Sz3Fb2iEZg41/ddsFDoyuYrIkmFehz0HR2thPgQqMyQYb2OtB0WxsZ3BeG3+wpRb1vzl2UYBog8FfGhttFKjtAclnZYrRo9ryG9uG/FZQU4AEg8ZE9LjGMzTmqKXPLnlWVnIlQQTvxJf8ip7VgjZjyVPrjw1te5otM7RmP7xm+sK2Gv9I8Gi++BRbEkR9EBw8zRUcKxwp73xkaLiqQb+kGduJTNHG72zcW9LoJgqQxpP3/Tj//c3yB0tqzaml05/+orHLksVO+95kX7/7qgJvnjlrfr2Ggsyx0eoy9uPzN5SPd86aXggOsEKW2Prz7du3VID3/tzs/sSRs2w7ovVHKtjrX2pd7ZMlTxAYfBAL9jiDwfLkq55Tm7ifhMlTGPyCAs7RFRhn47JnlcB9RM5T97ASuZXIcVNuUDIndpDbdsfrqsOppeXl5Y+XVKdjFCTh+zGaVuj0d9zy05PPK3QzBamxdwtTCrzyg/2Rvf2EstUjordGwa/kx9mSJLr8mLLtCW8HHGJc2R5hS219IiF6PnTusOqcMl57gm0Z8kanKMAQg0qSyuZfn7zItsbGyO9QlnxY0eCuD1XL2ys/MsrQhltE7Ug0uFOzufJFE2PxBo/YAx8XPPdDwWN0MrDRYIZF0mSMKCNHgaIVFoBbNoLJ7tEQDKxGF0kcLQimojCZopv0OkNOyWCCg9XMVAi7ARJzQdM2QUh0gmBozjc3Skg6dSBRqDGYSUOu66Zg+I2fNZs/M3/f/Grl/XnyF1Gw3VKCez0PN5IUfFLqvgUN4C0qNqYs5YhPL+aVZYDE4IpUk57oSFnJm4FyCqqOE0jhY2SMyLFoo56zyo6becOS5UVDdj7Vih0zp+tcMhwRpBeLyqtIjlJKAIZSbI8SGSF3k0pA3mR5tHuwPFoa7N7reoq2bqCsAk1HqCu5uvI1n6JuRXI+S1Mco54YmYTwcn6Aeic+kssXi8XpXC4V3t7/ADuTNKaQJdScAAAAAElFTkSuQmCC)](https://mybinder.org/v2/gh/ngsxfem/ngsxfem-jupyter/HEAD?filepath=tutorials.ipynb)
 
-[![lite-badge](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://lehrenfeld.pages.gwdg.de/ngsxfem-jupyter/lab/index.html)
-
 ### Documentation
 
 A *preliminary* collection of documentation (demos, tutorials, API) can be found [here](https://lehrenfeld.pages.gwdg.de/ngsxfem/).
 
 # About `ngsxfem`
 
 `ngsxfem` is an add-on library to the finite element package [Netgen/NGSolve](https://ngsolve.org) which enables the use of unfitted finite element technologies known as XFEM, CutFEM, TraceFEM, Finite Cell, ... . `ngsxfem` is an academic software. Its primary intention is to facilitate the development and validation of new numerical methods for partial differential equations.
 
 # The features of `ngsxfem`
 
 The main features of `ngsxfem` are:
 
-* Tools to work on a subset of the triangulation, the \"active mesh\" only
+* Tools to work on an a subset of the triangulation, the \"active mesh\" only
 * Numerical integration on geometries that are (implicitly) described through level set functions.
 * Higher order representation of level set geometries
 * Space-Time Finite Elements for the treatment of moving domain problems
 * All these features combined with the usual flexibility and power of [NGSolve](https://ngsolve.org).
 
 `ngsxfem` has been used in a variety of applications. In the document [doc/feature-details.md](doc/feature-details.md) (see also [compiled pdf](https://nightly.link/ngsxfem/ngsxfem/workflows/extras-workflow/master/doc-features.zip) ) more details on the features is given and in [doc/literature.md](doc/literature.md) (see also [literature](https://nightly.link/ngsxfem/ngsxfem/workflows/extras-workflow/master/doc-literature.zip) ) an overview of the scientific literature where `ngsxfem` is used is provided.
```

### Comparing `xfem-2.1.2303.post72.dev0/build/temp.linux-x86_64-cpython-310/CMakeFiles/3.25.0/CompilerIdCXX/CMakeCXXCompilerId.cpp` & `xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-310/CMakeFiles/3.25.0/CompilerIdCXX/CMakeCXXCompilerId.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/cmake_modules/cmake_uninstall.cmake.in` & `xfem-2.1.2303.post8.dev0/cmake_modules/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/cutint/cutintegral.cpp` & `xfem-2.1.2303.post8.dev0/cutint/cutintegral.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/cutint/cutintegral.hpp` & `xfem-2.1.2303.post8.dev0/cutint/cutintegral.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/cutint/fieldeval.cpp` & `xfem-2.1.2303.post8.dev0/cutint/fieldeval.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/cutint/fieldeval.hpp` & `xfem-2.1.2303.post8.dev0/cutint/fieldeval.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/cutint/lsetintdomain.cpp` & `xfem-2.1.2303.post8.dev0/cutint/lsetintdomain.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/cutint/lsetintdomain.hpp` & `xfem-2.1.2303.post8.dev0/cutint/lsetintdomain.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/cutint/mlsetintegration.cpp` & `xfem-2.1.2303.post8.dev0/cutint/mlsetintegration.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 #include "mlsetintegration.hpp"
 #include "straightcutrule.hpp"
 
 namespace xintegration
 {
+  using ngfem::INT;
+
+
   tuple<const IntegrationRule *, Array<double> > CreateMultiLevelsetCutIntegrationRule(const LevelsetIntegrationDomain & lsetintdom,
                                                                                        const ElementTransformation & trafo,
                                                                                        LocalHeap & lh)
   {
     bool debug_out = false;
 
     ArrayMem<const IntegrationRule *, 20> ir_parts; //static/dynamic memory allocation
```

### Comparing `xfem-2.1.2303.post72.dev0/cutint/mlsetintegration.hpp` & `xfem-2.1.2303.post8.dev0/cutint/mlsetintegration.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/cutint/python_cutint.cpp` & `xfem-2.1.2303.post8.dev0/cutint/python_cutint.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/cutint/spacetimecutrule.cpp` & `xfem-2.1.2303.post8.dev0/cutint/spacetimecutrule.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/cutint/spacetimecutrule.hpp` & `xfem-2.1.2303.post8.dev0/cutint/spacetimecutrule.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/cutint/straightcutrule.cpp` & `xfem-2.1.2303.post8.dev0/cutint/straightcutrule.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/cutint/straightcutrule.hpp` & `xfem-2.1.2303.post8.dev0/cutint/straightcutrule.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/cutint/xdecompose.cpp` & `xfem-2.1.2303.post8.dev0/cutint/xdecompose.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/cutint/xdecompose.hpp` & `xfem-2.1.2303.post8.dev0/cutint/xdecompose.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/cutint/xintegration.cpp` & `xfem-2.1.2303.post8.dev0/cutint/xintegration.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 #include "spacetimecutrule.hpp"
 #include "../spacetime/SpaceTimeFE.hpp"
 #include "../spacetime/SpaceTimeFESpace.hpp"
 
 
 namespace xintegration
 {
+  using ngfem::INT;
+
+
   tuple<const IntegrationRule *, Array<double>> CreateCutIntegrationRule(const LevelsetIntegrationDomain & lsetintdom,
                                                                          const ElementTransformation & trafo,
                                                                          LocalHeap & lh)
   {
     static Timer timer("CreateCutIntegrationRule");
     RegionTimer reg (timer);
     if (lsetintdom.IsMultiLevelsetDomain())
@@ -606,15 +609,15 @@
     switch (ET_SPACE)
     {
     case ET_SEGM:
     case ET_TRIG:
     case ET_TET:
     {
       // int sum = 0;
-      IVec< D > I;
+      INT< D > I;
       Vec< SD > position;
       for (int i = 0; i < D; ++i)
         I[i] = 0;
 
       // cout << " index = ";
       // for (int i = 0; i < ET_trait<ET_SPACE>::DIM; ++i)
       //   cout << I[i] << ", \t";
```

### Comparing `xfem-2.1.2303.post72.dev0/cutint/xintegration.hpp` & `xfem-2.1.2303.post8.dev0/cutint/xintegration.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/lsetcurving/calcpointshift.cpp` & `xfem-2.1.2303.post8.dev0/lsetcurving/calcpointshift.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/lsetcurving/calcpointshift.hpp` & `xfem-2.1.2303.post8.dev0/lsetcurving/calcpointshift.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/lsetcurving/lsetrefine.cpp` & `xfem-2.1.2303.post8.dev0/lsetcurving/lsetrefine.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/lsetcurving/lsetrefine.hpp` & `xfem-2.1.2303.post8.dev0/lsetcurving/lsetrefine.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/lsetcurving/projshift.cpp` & `xfem-2.1.2303.post8.dev0/lsetcurving/projshift.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/lsetcurving/projshift.hpp` & `xfem-2.1.2303.post8.dev0/lsetcurving/projshift.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/lsetcurving/python_lsetcurving.cpp` & `xfem-2.1.2303.post8.dev0/lsetcurving/python_lsetcurving.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/lsetcurving/shiftedevaluate.cpp` & `xfem-2.1.2303.post8.dev0/lsetcurving/shiftedevaluate.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 namespace ngfem
 {
 
   template <int SpaceD>
   void DiffOpShiftedEval<SpaceD> ::
   CalcMatrix (const FiniteElement & bfel,
               const BaseMappedIntegrationPoint & bmip,
-              BareSliceMatrix<double,ColMajor> mat,
+              SliceMatrix<double,ColMajor> mat,
               LocalHeap & lh) const
   {
     const MappedIntegrationPoint<SpaceD,SpaceD> & mip =
       static_cast<const MappedIntegrationPoint<SpaceD,SpaceD>&> (bmip);
 
     //const ScalarFiniteElement<SpaceD> & scafe =
             //dynamic_cast<const ScalarFiniteElement<SpaceD> & > (bfel);
```

### Comparing `xfem-2.1.2303.post72.dev0/lsetcurving/shiftedevaluate.hpp` & `xfem-2.1.2303.post8.dev0/lsetcurving/shiftedevaluate.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     virtual bool operator== (const DifferentialOperator & diffop2) const
     { return typeid(*this) == typeid(diffop2); }
 
 
     virtual void
     CalcMatrix (const FiniteElement & bfel,
         const BaseMappedIntegrationPoint & bmip,
-        BareSliceMatrix<double,ColMajor> mat,
+        SliceMatrix<double,ColMajor> mat,
         LocalHeap & lh) const;
 
 
     virtual void
     Apply (const FiniteElement & fel,
            const BaseMappedIntegrationPoint & mip,
            BareSliceVector<double> x,
```

### Comparing `xfem-2.1.2303.post72.dev0/lsetcurving/shiftintegrators.cpp` & `xfem-2.1.2303.post8.dev0/lsetcurving/shiftintegrators.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
       // const double h = D == 2 ? sqrt(2) * sqrt(mip.GetMeasure()) : sqrt(3) * cbrt(mip.GetMeasure());
       // double alpha = abs(lsetp1val / h) * abs(lsetp1val / h);
 
       double alpha = 0.0; // blending factor, 0.0 means: find phi_lin, 1.0 means: find phi (i.e. goal value = start value)
       if (coef_blending)
         alpha = coef_blending->Evaluate(mip);
 
-      if (alpha > 1+1e-6)
+      if (alpha > 1)
         throw Exception("alpha should not be larger than 1");
       
       double goal_val = (1.0-alpha) * lsetp1val + alpha * lseteval->Evaluate(mip.IP(),lh);
 
       // double goal_val = coef_lset_p1->Evaluate(mip);
       
       Vec<D> final_point;
```

### Comparing `xfem-2.1.2303.post72.dev0/lsetcurving/shiftintegrators.hpp` & `xfem-2.1.2303.post8.dev0/lsetcurving/shiftintegrators.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/python/CMakeLists.txt` & `xfem-2.1.2303.post8.dev0/python/CMakeLists.txt`

 * *Files 7% similar despite different names*

```diff
@@ -39,26 +39,26 @@
     set_target_properties(ngsxfem_py PROPERTIES INSTALL_RPATH "${NETGEN_RPATH_TOKEN}/../${NETGEN_PYTHON_RPATH}")
     install(TARGETS ngsxfem_py DESTINATION ${NGSOLVE_INSTALL_DIR_PYTHON}/xfem COMPONENT xfem)
 
     target_include_directories(ngsxfem_py PUBLIC ${NGSOLVE_INCLUDE_DIRS})
     # target_link_libraries(ngsxfem_py ngsxfem_lsetcurving ngsxfem_utils ngsxfem_cutint ngsxfem_xfem ngsxfem_spacetime)
 
     install (FILES
-        __init__.py cutmg.py mlset.py lset_spacetime.py lset_smoothblend.py lsetcurv.py utils.py ngs_check.py
+        __init__.py cutmg.py mlset.py lset_spacetime.py lsetcurv.py utils.py ngs_check.py
         DESTINATION ${NGSOLVE_INSTALL_DIR_PYTHON}/xfem
         COMPONENT xfem
     )
 
 # build stub files for pybind11 packages
 if(BUILD_STUB_FILES)
   execute_process(COMMAND ${NETGEN_PYTHON_EXECUTABLE} -c "import pybind11_stubgen; print(pybind11_stubgen.__file__)" OUTPUT_VARIABLE stubgen_path RESULT_VARIABLE pybind11_stubgen)
 if(pybind11_stubgen AND NOT ${pybind11_stubgen} EQUAL 0)
   message(WARNING "pybind11-stubgen not found, if you want to create stub files
 for better autocompletion support install it with pip.")
 else()
   message("-- Found pybind11-stubgen: ${stubgen_path}")
-  install(CODE "execute_process(COMMAND ${NETGEN_PYTHON_EXECUTABLE} -m pybind11_stubgen --ignore-all-errors xfem)") 
-  install(DIRECTORY ${CMAKE_CURRENT_BINARY_DIR}/../stubs/xfem/ DESTINATION ${NGSOLVE_INSTALL_DIR_PYTHON}/xfem/ COMPONENT xfem)
+  install(CODE "execute_process(COMMAND ${NETGEN_PYTHON_EXECUTABLE} -m pybind11_stubgen --ignore-invalid=all --skip-signature-downgrade --no-setup-py xfem)") 
+  install(DIRECTORY ${CMAKE_CURRENT_BINARY_DIR}/../stubs/xfem-stubs/ DESTINATION ${NGSOLVE_INSTALL_DIR_PYTHON}/xfem/ COMPONENT xfem)
 endif()
 endif(BUILD_STUB_FILES)
 
 endif(NETGEN_USE_PYTHON)
```

### Comparing `xfem-2.1.2303.post72.dev0/python/__init__.py` & `xfem-2.1.2303.post8.dev0/python/__init__.py`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/python/cutmg.py` & `xfem-2.1.2303.post8.dev0/python/cutmg.py`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/python/lset_spacetime.py` & `xfem-2.1.2303.post8.dev0/python/lset_spacetime.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from netgen.geom2d import SplineGeometry
 from netgen.meshing import MeshingParameters
 
 from ngsolve.internal import *
 from xfem import *
 from math import pi
 
-from xfem.lset_smoothblend import *
 
 class LevelSetMeshAdaptation_Spacetime:
     """
 Class to compute a proper mesh deformation to improve a piecewise (multi-) 
 linear (in space!) level set approximation to obtain a higher order 
 accurate approximation.
 
@@ -21,17 +20,17 @@
 order accurate approximation. The transformation is only applied on elements 
 where a level value inside a certain interval (lower,upper) exists.
 
 The result is a space-time finite element deformation (`deform`). For each 
 fixed time the behavior is as for an `LevelSetMeshAdaptation` object, i.e.
 
 
-  (1-b)*phi_h(x,t) + b*phi_lin( x,t ) = phi_h(Psi(x,t))
+1)phi_lin( Psi(x) ) = phi_h(x)
 
-  with Psi(x,t) = x + d(x,t) qn(x,t) =: D(x,t)
+  with Psi(x) = x + d(x) qn(x) =: D(x)
 
 for all x on 'cut' elements
 
 with
 
   phi_h : self.lset_ho
     the higher order space-time level set function
@@ -41,25 +40,14 @@
 
   Psi : Id + self.deform
     the resulting deformation
 
   qn : self.qn
     normal direction field
 
-  b: self.smooth_blend
-    an optional space-time CoefficientFunction to ensure a smooth transition
-    between curved and uncurved elements. This class offers the options of
-    1) a finite element blending, in which case b is assumed as b=0 and shall
-    not be specified in the constructor, and 2) a smooth blending, in which the
-    sufficiently regular function b ranging from 0 at cut locations to 1 outside
-    with zero deformation is taken into consideration. Check out
-    https://arxiv.org/abs/2311.02348 for a detailed mathematical description,
-    the constructor of this class for specification, and the class
-    LevelSet_SmoothBlending for generating function b in a pre-defined way.
-
 This class holds its own members for the higher order and lower order
  (P1-in-space) space-time approximation of the level set function and 
  only depends on the input of a mesh and a CoefficientFunction 
  (the levelset function) (and options).
 
  A LevelSetMeshAdaptation_Spacetime can also be used as a context
  manager. In this case, the mesh deformation is applied on the mesh
@@ -69,16 +57,15 @@
     order_deform = 2
     order_qn = 2
     order_lset = 2
 
 
     @TimeFunction
     def __init__(self, mesh, order_space = 2, order_time = 1, lset_lower_bound = 0,
-                 lset_upper_bound = 0, threshold = -1, smooth_blend=None,
-                 discontinuous_qn = False, heapsize=1000000,periodic=False):
+                 lset_upper_bound = 0, threshold = -1, discontinuous_qn = False, heapsize=1000000,periodic=False):
 
         """
 The computed deformation depends on different options:
 
   order_space : int
     order of deformation GridFunction (ideally) order + 1 is the accuracy of the geometry
     approximation after applying the deformation on the mesh
@@ -96,31 +83,28 @@
     
   threshold: float
     maximum (pointwise) value for d(x)/h in the mapping
       Psi(x) = x + d(x) qn(x)
     of the mesh transformation. A small value might be necessary if the geometry is only coarsely
     approximated to avoid irregular meshes after a corresponding mesh deformation.
 
-  smooth_blend : CoefficientFunction or None(default)
-    If a smooth blending function is specified, the deformation to be calculated will involve
-    the smooth blending stemming from this function. Provide a space-time function such as the
-    member function LevelSet_SmoothBlending.CF. If this is None, the finite element blending
-    will be applied, amounting formally to an overall function of b=0. Check out
-    https://arxiv.org/abs/2311.02348 for a detailed mathematical description. Note that in
-    the case of the smooth blending, the function b will also be used to define all the elements
-    where the deformation is calculated firstly locally; those are the elements with b<1
-    at one of the time nodes of the ScalarTimeFE with order time_order.
-
   discontinuous_qn: boolean
     As an approximation for the normal direction we use n_h = nabla phi_h (gradient of higher order
     level set approximation) depending on the discontinuous_qn flag this normal field will be
     projected onto a continuous finite element space or not.
 
+  eps_perturbation: float
+    epsilon perturbation that is used to interpolate to P1
+
   heapsize : int
     heapsize for local computations.
+
+  levelset : CoefficientFunction or None(default)
+    If a level set function is prescribed the deformation is computed right away. Otherwise the 
+    computation is triggered only at calls for `CalcDeformation`.
         """
 
         self.gf_to_project = []
         self.gf_to_project_tmp = [] # list for temporary copies
         
         self.order_deform = order_space
         self.order_qn = order_space
@@ -206,18 +190,14 @@
                 self.lsetadap_st.mesh.UnsetDeformation()
         self.top = MeshDeformationContext(self,"top")
         self.bottom = MeshDeformationContext(self,"bottom")
 
         self.levelsetp1 = {INTERVAL : self.lset_p1, BOTTOM : self.lset_p1_bottom, TOP : self.lset_p1_top}
         self.deformation = {INTERVAL : self.deform, BOTTOM : self.deform_bottom, TOP : self.deform_top}
 
-        if (smooth_blend != None) and (smooth_blend != "None"):
-          self.smooth_blend = smooth_blend
-        else:
-          self.smooth_blend = None
         
     def ProjectOnUpdate(self,gf,update_domain=None):
         """
 When the LevelsetMeshAdaptation class generates a new deformation (due to 
 a new level set function) all GridFunction that have been stored through
 `ProjectOnUpdate` will be projected from the previous to the new mesh
 by an essentially local projection (Oswald projection of the shifted 
@@ -309,49 +289,35 @@
         self.v_kappa.Update()
         self.kappa.Update()
         self.deform_last_top.Update()               
         self.interpol_ho(levelset)
         self.interpol_p1()
         RestrictGFInTime(spacetime_gf=self.deform,reference_time=1.0,space_gf=self.deform_last_top)   
 
+
         for i in  range(len(self.v_ho_st.TimeFE_nodes())):
             self.lset_p1_node.vec[:].data = self.lset_p1.vec[i*self.ndof_node_p1 : (i+1)*self.ndof_node_p1]
             if calc_kappa:
                 self.ci.Update(self.lset_p1_node)
                 self.kappa.vec[i*self.v_kappa_node.ndof : (i+1)*self.v_kappa_node.ndof].data = self.ci.GetCutRatios(VOL)
         
         
         self.ci.Update(self.lset_p1,time_order=self.order_time)
         self.hasneg_spacetime[:] = False
         self.hasneg_spacetime |= self.ci.GetElementsOfType(NEG)
         self.haspos_spacetime[:] = False
         self.haspos_spacetime |= self.ci.GetElementsOfType(POS)
         self.hasif_spacetime[:] = False
         self.hasif_spacetime |= self.ci.GetElementsOfType(IF)
-
-        self.blending_forwarded = CF(0.)
-        self.where_projected = BitArray(self.hasif_spacetime)
-        if self.smooth_blend != None:
-            ci_blend_helper = CutInfo(self.mesh, time_order=self.order_time)
-            b_disc_node_p1 = GridFunction(self.v_p1)
-            b_disc_p1 = GridFunction(self.v_p1_st)
-            times = [xi for xi in self.v_p1_st.TimeFE_nodes()]
-            for i,ti in enumerate(times):
-                b_disc_node_p1.Set(fix_tref( self.smooth_blend ,ti) -1 + 1e-6)
-                b_disc_p1.vec[i*self.ndof_node_p1 : (i+1)*self.ndof_node_p1].data = b_disc_node_p1.vec[:]
-            ci_blend_helper.Update(b_disc_p1 , time_order=0)
-            self.where_projected = ci_blend_helper.GetElementsOfType(HASNEG)
-            self.blending_forwarded = self.smooth_blend
-
+        
         for i in range(self.order_time + 1):
             self.lset_ho_node.vec[:].data = self.lset_ho.vec[i*self.ndof_node : (i+1)*self.ndof_node]
             self.qn.Set(self.lset_ho_node.Deriv())
             self.lset_p1_node.vec[:].data = self.lset_p1.vec[i*self.ndof_node_p1 : (i+1)*self.ndof_node_p1]
-            ProjectShift(self.lset_ho_node, self.lset_p1_node, self.deform_node, self.qn, self.where_projected,
-                         fix_tref(self.blending_forwarded, self.v_ho_st.TimeFE_nodes()[i]), self.lset_lower_bound,
+            ProjectShift(self.lset_ho_node, self.lset_p1_node, self.deform_node, self.qn, self.hasif_spacetime, None, self.lset_lower_bound, 
                          self.lset_upper_bound, self.threshold, heapsize=self.heapsize)
             self.deform.vec[i*self.ndof_node : (i+1)*self.ndof_node].data = self.deform_node.vec[:]
 
 
         RestrictGFInTime(spacetime_gf=self.lset_p1,reference_time=0.0,space_gf=self.lset_p1_bottom)
         RestrictGFInTime(spacetime_gf=self.lset_p1,reference_time=1.0,space_gf=self.lset_p1_top)
         RestrictGFInTime(spacetime_gf=self.deform,reference_time=0.0,space_gf=self.deform_bottom)
```

### Comparing `xfem-2.1.2303.post72.dev0/python/lsetcurv.py` & `xfem-2.1.2303.post8.dev0/python/lsetcurv.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 Computes a continuous function that describes a shift between points that are on the (P1 )
 approximated level set function and its higher order accurate approximation. The transformation is
 only applied on elements where a level value inside a certain interval (lower,upper) exists.
 
 The result is a deform function (D) which is computed pointwise as
 
-1)phi_lin( x ) = phi_h(Psi(x))
+1)phi_lin( Psi(x) ) = phi_h(x)
 
   with Psi(x) = x + d(x) qn(x) =: D(x)
 
 for all x on 'cut' elements
 
 with
```

### Comparing `xfem-2.1.2303.post72.dev0/python/mlset.py` & `xfem-2.1.2303.post8.dev0/python/mlset.py`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/python/ngs_check.py` & `xfem-2.1.2303.post8.dev0/python/ngs_check.py`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/python/python_ngsxfem.cpp` & `xfem-2.1.2303.post8.dev0/python/python_ngsxfem.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/python/utils.py` & `xfem-2.1.2303.post8.dev0/python/utils.py`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/setup.py` & `xfem-2.1.2303.post8.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/spacetime/SpaceTimeFE.cpp` & `xfem-2.1.2303.post8.dev0/spacetime/SpaceTimeFE.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/spacetime/SpaceTimeFE.hpp` & `xfem-2.1.2303.post8.dev0/spacetime/SpaceTimeFE.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/spacetime/SpaceTimeFESpace.cpp` & `xfem-2.1.2303.post8.dev0/spacetime/SpaceTimeFESpace.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/spacetime/SpaceTimeFESpace.hpp` & `xfem-2.1.2303.post8.dev0/spacetime/SpaceTimeFESpace.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/spacetime/diffopDt.cpp` & `xfem-2.1.2303.post8.dev0/spacetime/diffopDt.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -83,19 +83,19 @@
   template class T_DifferentialOperator<DiffOpFixt<3, 0>>;
   template class T_DifferentialOperator<DiffOpFixt<3, 1>>;
 
   template<int SpaceD>
   void DiffOpFixAnyTime<SpaceD> ::
   CalcMatrix (const FiniteElement & bfel,
               const BaseMappedIntegrationPoint & bmip,
-              BareSliceMatrix<double,ColMajor> mat,
+              SliceMatrix<double,ColMajor> mat,
               LocalHeap & lh) const
   {
 
-      //mat = 0.0;
+      mat = 0.0;
       const MappedIntegrationPoint<DIM_ELEMENT,DIM_SPACE> & mip =
       static_cast<const MappedIntegrationPoint<DIM_ELEMENT,DIM_SPACE>&> (bmip);
 
       IntegrationPoint ip(mip.IP()(0),mip.IP()(1),mip.IP()(2), time);
       MarkAsSpaceTimeIntegrationPoint(ip);
 
       const SpaceTimeFE<SpaceD>& scafed = dynamic_cast<const SpaceTimeFE<SpaceD> &> (bfel);
```

### Comparing `xfem-2.1.2303.post72.dev0/spacetime/diffopDt.hpp` & `xfem-2.1.2303.post8.dev0/spacetime/diffopDt.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     virtual bool operator== (const DifferentialOperator & diffop2) const
     { return typeid(*this) == typeid(diffop2); }
 
 
     virtual void
     CalcMatrix (const FiniteElement & bfel,
         const BaseMappedIntegrationPoint & bmip,
-        BareSliceMatrix<double,ColMajor> mat,
+        SliceMatrix<double,ColMajor> mat,
         LocalHeap & lh) const;
 
     virtual void
     ApplyTrans (const FiniteElement & fel,
         const BaseMappedIntegrationPoint & mip,
         FlatVector<double> flux,
         FlatVector<double> x,
```

### Comparing `xfem-2.1.2303.post72.dev0/spacetime/python_spacetime.cpp` & `xfem-2.1.2303.post8.dev0/spacetime/python_spacetime.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -60,20 +60,20 @@
     if (py::isinstance<py::list>(dirichlet)) {
         flags.SetFlag("dirichlet", makeCArray<double>(py::list(dirichlet)));
 
     }
 
     if (py::isinstance<py::str>(dirichlet))
     {
-        Array<double> dirlist;
-        Region dir(ma, BND, dirichlet.cast<string>());
-        for (int i = 0; i < ma->GetNBoundaries(); i++)
-            if (dir.Mask()[i])
-              dirlist.Append (i+1);
-        flags.SetFlag("dirichlet", dirlist);
+          std::regex pattern(dirichlet.cast<string>());
+          Array<double> dirlist;
+          for (int i = 0; i < ma->GetNBoundaries(); i++)
+             if (std::regex_match (ma->GetMaterial(BND, i), pattern))
+               dirlist.Append (i+1);
+               flags.SetFlag("dirichlet", dirlist);
     }
 
     auto tfe = dynamic_pointer_cast<ScalarFiniteElement<1>>(fe);
     //cout << tfe << endl;
     if(tfe == nullptr)
       cout << IM(1) << "Warning! tfe == nullptr" << endl;
```

### Comparing `xfem-2.1.2303.post72.dev0/spacetime/spacetime_vtk.cpp` & `xfem-2.1.2303.post8.dev0/spacetime/spacetime_vtk.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -35,26 +35,26 @@
     cells.SetSize(0);
     for (auto field : value_field)
       field->SetSize(0);
   }
     
 
   /// Fill principil lattices (points and connections on subdivided reference hexahedron) in 3D
-  void SpaceTimeVTKOutput::FillReferenceHex(Array<IntegrationPoint> & ref_coords,Array<IVec<ELEMENT_MAXPOINTS+1>> & ref_elems)
+  void SpaceTimeVTKOutput::FillReferenceHex(Array<IntegrationPoint> & ref_coords,Array<INT<ELEMENT_MAXPOINTS+1>> & ref_elems)
   {
     if(subdivisionx == 0 && subdivisiont == 0)
     {
       double p[8][3] = { {0,0,0}, {1,0,0}, {1,1,0}, {0,1,0}, {0,0,1}, {1,0,1}, {1,1,1}, {0,1,1} };
       for (int i = 0; i < 8; i++)
       {
         auto tmp = IntegrationPoint(p[i][0],p[i][1],0.0,p[i][2]);
         MarkAsSpaceTimeIntegrationPoint(tmp);
         ref_coords.Append(tmp);
       }
-      IVec<ELEMENT_MAXPOINTS+1> elem;
+      INT<ELEMENT_MAXPOINTS+1> elem;
       elem[0] = 8;
       for(int i=0; i<ElementTopology::GetNVertices(ET_HEX); i++)
         elem[i+1] = i;
       ref_elems.Append(elem);
       
     }
     else
@@ -81,36 +81,36 @@
         int incr_i = (rx+1)*(rt+1);
         for(int j = 0; j < rx; ++j)
         {
           int incr_j = rt+1;
           pidx = i*incr_i + j*incr_j;
           for(int k = 0; k < rt; ++k, pidx++)
           {
-            ref_elems.Append(IVec<ELEMENT_MAXPOINTS+1>(8, pidx, pidx+1, pidx+incr_j+1, pidx+incr_j,
+            ref_elems.Append(INT<ELEMENT_MAXPOINTS+1>(8, pidx, pidx+1, pidx+incr_j+1, pidx+incr_j,
                                                          pidx+incr_i, pidx+incr_i+1, pidx+incr_i+incr_j+1, pidx+incr_j+incr_i));
           }          
         } 
       }
     }
   }
 
   
-  void SpaceTimeVTKOutput::FillReferencePrism(Array<IntegrationPoint> & ref_coords,Array<IVec<ELEMENT_MAXPOINTS+1>> & ref_elems)
+  void SpaceTimeVTKOutput::FillReferencePrism(Array<IntegrationPoint> & ref_coords,Array<INT<ELEMENT_MAXPOINTS+1>> & ref_elems)
   {
     if(subdivisionx == 0 && subdivisiont == 0)
     {
 
       double p[6][3] = { {0,0,0}, {1,0,0}, {0,1,0}, {0,0,1}, {1,0,1}, {0,1,1} };
       for (int i = 0; i < 6; i++)
       {
         auto tmp = IntegrationPoint(p[i][0],p[i][1],0.0,p[i][2]);
         MarkAsSpaceTimeIntegrationPoint(tmp);
         ref_coords.Append(tmp);
       }
-      IVec<ELEMENT_MAXPOINTS+1> elem;
+      INT<ELEMENT_MAXPOINTS+1> elem;
       elem[0] = 6;
       for(int i=0; i<ElementTopology::GetNVertices(ET_PRISM); i++)
         elem[i+1] = i;
       ref_elems.Append(elem);
     }
     else
     {
@@ -140,20 +140,20 @@
           for(int j = 0; i+j <= rx; ++j,pidx++)
           {
             // int pidx_curr = pidx;
             if(i+j == rx) continue;
             int pidx_incr_i = pidx+1;
             int pidx_incr_j = pidx+s-i;
 
-            ref_elems.Append(IVec<ELEMENT_MAXPOINTS+1>(6, pidx, pidx_incr_i, pidx_incr_j, pidx+incr_k, pidx_incr_i+incr_k, pidx_incr_j+incr_k, 0, 0 ));
+            ref_elems.Append(INT<ELEMENT_MAXPOINTS+1>(6, pidx, pidx_incr_i, pidx_incr_j, pidx+incr_k, pidx_incr_i+incr_k, pidx_incr_j+incr_k, 0, 0 ));
               
             int pidx_incr_ij = pidx_incr_j + 1;
 
             if(i+j+1<rx)
-              ref_elems.Append(IVec<ELEMENT_MAXPOINTS+1>(6, pidx_incr_i, pidx_incr_ij, pidx_incr_j, pidx_incr_i+incr_k, pidx_incr_ij+incr_k, pidx_incr_j+incr_k,0,0));
+              ref_elems.Append(INT<ELEMENT_MAXPOINTS+1>(6, pidx_incr_i, pidx_incr_ij, pidx_incr_j, pidx_incr_i+incr_k, pidx_incr_ij+incr_k, pidx_incr_j+incr_k,0,0));
           }
       }
     }
   }
 
   /// output of data points
   void SpaceTimeVTKOutput::PrintPoints()
@@ -251,17 +251,17 @@
     cout << IM(4) << ":" << flush;
     
     output_cnt++;
 
     ResetArrays();
 
     Array<IntegrationPoint> ref_vertices_prism(0), ref_vertices_hex(0);
-    Array<IVec<ELEMENT_MAXPOINTS+1>> ref_prisms(0), ref_hexes(0);
+    Array<INT<ELEMENT_MAXPOINTS+1>> ref_prisms(0), ref_hexes(0);
     FlatArray<IntegrationPoint> ref_vertices;
-    FlatArray<IVec<ELEMENT_MAXPOINTS+1>> ref_elems;
+    FlatArray<INT<ELEMENT_MAXPOINTS+1>> ref_elems;
     FillReferencePrism(ref_vertices_prism,ref_prisms);
     FillReferenceHex(ref_vertices_hex,ref_hexes);
       
     // header:
     *fileout << "# vtk DataFile Version 3.0" << endl;
     *fileout << "vtk output" << endl;
     *fileout << "ASCII" << endl;
@@ -339,15 +339,15 @@
               value_field[i]->Append(tmp(d));
           }
         }
       }
       
       for ( auto elem : ref_elems)
       {
-        IVec<ELEMENT_MAXPOINTS+1> new_elem = elem;
+        INT<ELEMENT_MAXPOINTS+1> new_elem = elem;
         for (int i = 1; i <= new_elem[0]; ++i)
           new_elem[i] += offset;
         cells.Append(new_elem);
       }
 
     }
```

### Comparing `xfem-2.1.2303.post72.dev0/spacetime/spacetime_vtk.hpp` & `xfem-2.1.2303.post8.dev0/spacetime/spacetime_vtk.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     Array<string> fieldnames;
     string filename;
     int subdivisionx, subdivisiont;
     int only_element = -1;
 
     Array<shared_ptr<ValueField>> value_field;
     Array<Vec<3>> points;
-    Array<IVec<ELEMENT_MAXPOINTS+1>> cells;
+    Array<INT<ELEMENT_MAXPOINTS+1>> cells;
 
     int output_cnt = 0;
     
     shared_ptr<ofstream> fileout;
     
   public:
 
@@ -36,16 +36,16 @@
 
     SpaceTimeVTKOutput (shared_ptr<MeshAccess>, const Array<shared_ptr<CoefficientFunction>> &,
                         const Array<string> &, string, int, int, int);
     virtual ~SpaceTimeVTKOutput() { ; }
     
     void ResetArrays();
     
-    void FillReferenceHex(Array<IntegrationPoint> & ref_coords,Array<IVec<ELEMENT_MAXPOINTS+1>> & ref_elems); 
-    void FillReferencePrism(Array<IntegrationPoint> & ref_coords,Array<IVec<ELEMENT_MAXPOINTS+1>> & ref_elems);    
+    void FillReferenceHex(Array<IntegrationPoint> & ref_coords,Array<INT<ELEMENT_MAXPOINTS+1>> & ref_elems); 
+    void FillReferencePrism(Array<IntegrationPoint> & ref_coords,Array<INT<ELEMENT_MAXPOINTS+1>> & ref_elems);    
 
     void PrintPoints();
     void PrintCells();
     void PrintCellTypes(VorB vb, const BitArray * drawelems=nullptr);
     void PrintFieldData();    
 
     virtual void Do (LocalHeap & lh, VorB vb = VOL, const BitArray * drawelems = 0, double t_start = 0, double t_end = 1);
```

### Comparing `xfem-2.1.2303.post72.dev0/spacetime/timecf.cpp` & `xfem-2.1.2303.post8.dev0/spacetime/timecf.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/spacetime/timecf.hpp` & `xfem-2.1.2303.post8.dev0/spacetime/timecf.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/tests/CMakeLists.txt` & `xfem-2.1.2303.post8.dev0/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/utils/bitarraycf.cpp` & `xfem-2.1.2303.post8.dev0/utils/bitarraycf.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/utils/bitarraycf.hpp` & `xfem-2.1.2303.post8.dev0/utils/bitarraycf.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/utils/ngsxstd.cpp` & `xfem-2.1.2303.post8.dev0/utils/ngsxstd.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/utils/ngsxstd.hpp` & `xfem-2.1.2303.post8.dev0/utils/ngsxstd.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/utils/p1interpol.cpp` & `xfem-2.1.2303.post8.dev0/utils/p1interpol.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -34,20 +34,17 @@
     for (int vnr = 0; vnr < nv; ++vnr)
     {
       HeapReset hr(lh);
 
       double val_lset;
       if (coef)
       {
-        /*
         Array<int> elnums;
         ma -> GetVertexElements (vnr, elnums);
         Ngs_Element ngel = ma -> GetElement (ElementId(VOL,elnums[0]));
-        */
-        Ngs_Element ngel = ma -> GetElement (ElementId(VOL,ma->GetVertexElements (vnr)[0]));
         auto & eltrans = ma -> GetTrafo (ngel, lh);
 
         if( ma -> GetDimension() == 2)
         {
           Vec<2> point;
           ma->GetPoint<2>(vnr,point);
           IntegrationPoint ip(0,0,0,0);
```

### Comparing `xfem-2.1.2303.post72.dev0/utils/p1interpol.hpp` & `xfem-2.1.2303.post8.dev0/utils/p1interpol.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/utils/python_utils.cpp` & `xfem-2.1.2303.post8.dev0/utils/python_utils.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/utils/restrictedblf.cpp` & `xfem-2.1.2303.post8.dev0/utils/restrictedblf.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -155,14 +155,14 @@
     {
       auto table2 = MeshEntityToDofTable(this->fespace2, el_restriction, fac_restriction, this->eliminate_internal, this->eliminate_hidden, &(this->specialelements));
       size_t ndof2 = this->fespace2->GetNDof();
       graph = new MatrixGraph (ndof2, ndof, table2, table, symmetric);
     }
     
     graph -> FindSameNZE();
-    return std::move(*graph);
+    return move(*graph);
   }
 
 template class RestrictedBilinearForm<double,double>;
 template class RestrictedBilinearForm<Complex,Complex>; 
 }
```

### Comparing `xfem-2.1.2303.post72.dev0/utils/restrictedblf.hpp` & `xfem-2.1.2303.post8.dev0/utils/restrictedblf.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/utils/restrictedfespace.cpp` & `xfem-2.1.2303.post8.dev0/utils/restrictedfespace.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -117,53 +117,53 @@
 #include "diffop_impl.hpp"
 
 namespace ngfem
 {
   void RestrictedDifferentialOperator ::
   CalcMatrix (const FiniteElement & fel,
               const BaseMappedIntegrationPoint & mip,
-              BareSliceMatrix<double,ColMajor> mat, 
+              SliceMatrix<double,ColMajor> mat, 
               LocalHeap & lh) const 
   {
     if (fel.GetNDof() == 0)
-      ; // mat = 0;
+      mat = 0;
     else
       diffop->CalcMatrix (fel, mip, mat, lh);
   }
   
   void RestrictedDifferentialOperator ::
   CalcMatrix (const FiniteElement & fel,
               const BaseMappedIntegrationPoint & mip,
-              BareSliceMatrix<Complex,ColMajor> mat, 
+              SliceMatrix<Complex,ColMajor> mat, 
               LocalHeap & lh) const 
   {
     if (fel.GetNDof() == 0)
-      ; // mat = 0;
+      mat = 0;
     else
       diffop->CalcMatrix (fel, mip, mat, lh);
   }
   
   void RestrictedDifferentialOperator ::
   CalcMatrix (const FiniteElement & fel,
               const SIMD_BaseMappedIntegrationRule & mir,
               BareSliceMatrix<SIMD<double>> mat) const
   {
     if (fel.GetNDof() == 0)
-      mat.AddSize(fel.GetNDof(),fel.GetNDof()) = 0.0;
+      mat *= 0.0;
     else
       diffop->CalcMatrix(fel, mir, mat);
   }
   
   void RestrictedDifferentialOperator ::
   CalcMatrix (const FiniteElement & fel,
               const SIMD_BaseMappedIntegrationRule & mir,
               BareSliceMatrix<SIMD<Complex>> mat) const
   {
     if (fel.GetNDof() == 0)
-      mat.AddSize(fel.GetNDof(),fel.GetNDof()) = 0.0;
+      mat *= 0.0;
     else
       diffop->CalcMatrix(fel, mir, mat);
   }
 
   void RestrictedDifferentialOperator ::
   Apply (const FiniteElement & fel,
          const BaseMappedIntegrationPoint & mip,
@@ -194,54 +194,54 @@
   Apply (const FiniteElement & fel,
          const SIMD_BaseMappedIntegrationRule & mir,
          BareSliceVector<double> x, 
          BareSliceMatrix<SIMD<double>> flux) const
   // LocalHeap & lh) const
   {
     if (fel.GetNDof() == 0)
-      flux.AddSize(fel.GetNDof(),diffop->Dim()) = 0.0;
+      flux *= 0.0;
     else
       diffop->Apply(fel, mir, x, flux);
   }
  
   void RestrictedDifferentialOperator ::
   Apply (const FiniteElement & fel,
          const SIMD_BaseMappedIntegrationRule & mir,
          BareSliceVector<Complex> x, 
          BareSliceMatrix<SIMD<Complex>> flux) const
   // LocalHeap & lh) const
   {
     if (fel.GetNDof() == 0)
-      flux.AddSize(fel.GetNDof(),diffop->Dim()) = 0.0;
+      flux *= 0.0;
     else
       diffop->Apply(fel, mir, x, flux);
   }
  
   void RestrictedDifferentialOperator ::
   ApplyTrans (const FiniteElement & fel,
               const BaseMappedIntegrationPoint & mip,
               FlatVector<double> flux,
               BareSliceVector<double> x, 
               LocalHeap & lh) const
   {
     if (fel.GetNDof() == 0)
-      flux = 0.0;
+      flux *= 0.0;
     else
       diffop->ApplyTrans(fel, mip, flux, x, lh);
   }
 
   void RestrictedDifferentialOperator ::
   ApplyTrans (const FiniteElement & fel,
               const BaseMappedIntegrationPoint & mip,
               FlatVector<Complex> flux,
               BareSliceVector<Complex> x, 
               LocalHeap & lh) const
   {
     if (fel.GetNDof() == 0)
-      flux = 0.0;
+      flux *= 0.0;
     else
       diffop->ApplyTrans(fel, mip, flux, x, lh);
   }
 
   void RestrictedDifferentialOperator ::
   ApplyTrans (const FiniteElement & fel,
 	      const BaseMappedIntegrationRule & mir,
```

### Comparing `xfem-2.1.2303.post72.dev0/utils/restrictedfespace.hpp` & `xfem-2.1.2303.post8.dev0/utils/restrictedfespace.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -93,21 +93,21 @@
       else
         return nullptr;
     }
     
     NGS_DLL_HEADER virtual void
     CalcMatrix (const FiniteElement & fel,
 		const BaseMappedIntegrationPoint & mip,
-		BareSliceMatrix<double,ColMajor> mat, 
+		SliceMatrix<double,ColMajor> mat, 
 		LocalHeap & lh) const override;    
     
     NGS_DLL_HEADER virtual void
     CalcMatrix (const FiniteElement & fel,
 		const BaseMappedIntegrationPoint & mip,
-    BareSliceMatrix<Complex,ColMajor> mat, 
+		SliceMatrix<Complex,ColMajor> mat, 
 		LocalHeap & lh) const override;    
 
     NGS_DLL_HEADER virtual void
     CalcMatrix (const FiniteElement & fel,
 		const SIMD_BaseMappedIntegrationRule & mir,
 		BareSliceMatrix<SIMD<double>> mat) const override;
```

### Comparing `xfem-2.1.2303.post72.dev0/utils/xprolongation.cpp` & `xfem-2.1.2303.post8.dev0/utils/xprolongation.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/utils/xprolongation.hpp` & `xfem-2.1.2303.post8.dev0/utils/xprolongation.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/xfem/aggregates.cpp` & `xfem-2.1.2303.post8.dev0/xfem/aggregates.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/xfem/aggregates.hpp` & `xfem-2.1.2303.post8.dev0/xfem/aggregates.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/xfem/cutinfo.cpp` & `xfem-2.1.2303.post8.dev0/xfem/cutinfo.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -553,53 +553,21 @@
       (nf, lh,
       [&] (int facnr, LocalHeap & lh)
     {
       if (a->Test(facnr))
       {
         Array<int> elnums(0,lh);
         ma->GetFacetElements (facnr, elnums);
-
         for (auto elnr : elnums)
           ret->SetBitAtomic(elnr);
       }
     });
     return ret;
   }
 
-  shared_ptr<BitArray> GetElementsWithSharedVertex(shared_ptr<MeshAccess> ma, shared_ptr<BitArray> a, LocalHeap & lh)
-  {
-    if (ma->GetCommunicator().Size() > 1)
-      throw Exception("GetElementsWithNeighborFacets:: No GetElementsWithSharedVertex for MPI yet");
-    int ne = ma->GetNE();
-    shared_ptr<BitArray> ret = make_shared<BitArray> (ne);
-    ret->Clear();
-    IterateRange
-      (ne, lh,
-      [&] (int elnr, LocalHeap & lh)
-    {
-        if(a->Test(elnr)){
-            ElementId elid(VOL,elnr);
-            Array<int> nodenums(0,lh);
-            nodenums = ma->GetElVertices(elid);
-            for (int node : nodenums) {
-              /*
-                Array<int> elnums(0,lh);
-                ma->GetVertexElements(node, elnums);
-                for (auto elnr : elnums)
-                    ret->SetBitAtomic(elnr);
-              */
-              for (auto elnr : ma->GetVertexElements(node))
-                ret->SetBitAtomic(elnr);
-              
-            }
-        }
-    });
-    return ret;
-}
-
   shared_ptr<BitArray> GetDofsOfElements(shared_ptr<FESpace> fes,
                                          shared_ptr<BitArray> a,
                                          LocalHeap & lh)
   {
     int ne = fes->GetMeshAccess()->GetNE();
     int ndof = fes->GetNDof();
     shared_ptr<BitArray> ret = make_shared<BitArray> (ndof);
```

### Comparing `xfem-2.1.2303.post72.dev0/xfem/cutinfo.hpp` & `xfem-2.1.2303.post8.dev0/xfem/cutinfo.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -157,16 +157,14 @@
                                                   bool ask_and,
                                                   LocalHeap & lh);
 
   shared_ptr<BitArray> GetElementsWithNeighborFacets(shared_ptr<MeshAccess> ma,
                                                      shared_ptr<BitArray> a,
                                                      LocalHeap & lh);
 
-  shared_ptr<BitArray> GetElementsWithSharedVertex(shared_ptr<MeshAccess> ma, shared_ptr<BitArray> a, LocalHeap & lh);
-
   shared_ptr<BitArray> GetDofsOfElements(shared_ptr<FESpace> fes,
                                          shared_ptr<BitArray> a,
                                          LocalHeap & lh);
 
   shared_ptr<BitArray> GetDofsOfFacets(shared_ptr<FESpace> fes,
                                        shared_ptr<BitArray> a,
                                        LocalHeap & lh);
```

### Comparing `xfem-2.1.2303.post72.dev0/xfem/ghostpenalty.cpp` & `xfem-2.1.2303.post8.dev0/xfem/ghostpenalty.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/xfem/ghostpenalty.hpp` & `xfem-2.1.2303.post8.dev0/xfem/ghostpenalty.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/xfem/python_xfem.cpp` & `xfem-2.1.2303.post8.dev0/xfem/python_xfem.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -436,26 +436,14 @@
   BitArray for marked facets
 
 heapsize : int
   heapsize of local computations.
 )raw_string")
     );
 
-  m.def("GetElementsWithSharedVertex",
-      [] (shared_ptr<MeshAccess> ma,
-         shared_ptr<BitArray> a,
-         int heapsize)
-      {
-          LocalHeap lh (heapsize, "GetElementsWithNeighborFacets-heap", true);
-          return GetElementsWithSharedVertex(ma,a,lh);
-      } ,
-      py::arg("mesh"),
-      py::arg("a"),
-      py::arg("heapsize") = 1000000);
-
   m.def("GetDofsOfElements",
         [] (PyFES fes,
             PyBA a,
             int heapsize)
         {
           LocalHeap lh (heapsize, "GetDofsOfElements-heap", true);
           return GetDofsOfElements(fes,a,lh);
```

### Comparing `xfem-2.1.2303.post72.dev0/xfem/sFESpace.cpp` & `xfem-2.1.2303.post8.dev0/xfem/sFESpace.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -112,15 +112,15 @@
                          coef_lset->Evaluate(mip3)};
       // cout << lsets[0] << endl;
       // cout << lsets[1] << endl;
       // cout << lsets[2] << endl << endl;
 
       Array<Vec<2>> cuts(0);
 
-      Array<IVec<2>> edges = { IVec<2>(0,1), IVec<2>(0,2), IVec<2>(1,2)};
+      Array<INT<2>> edges = { INT<2>(0,1), INT<2>(0,2), INT<2>(1,2)};
       for (auto e: edges)
       {
         const double lset1 = lsets[e[0]];
         const double lset2 = lsets[e[1]];
         if ((lset1>0 && lset2>0) || (lset1<0 && lset2<0))
           continue;
         double cut_scalar = -lsets[e[0]]/(lsets[e[1]]-lsets[e[0]]);
```

### Comparing `xfem-2.1.2303.post72.dev0/xfem/sFESpace.hpp` & `xfem-2.1.2303.post8.dev0/xfem/sFESpace.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/xfem/symboliccutbfi.cpp` & `xfem-2.1.2303.post8.dev0/xfem/symboliccutbfi.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -739,15 +739,15 @@
       //if (lsetintdom->GetDomainType() != IF) throw Exception("No Neg/pos facet ints in 3D yet");
       // so far only : Codim 2 special case (3D -> 1D)
       //if (time_order > -1) throw Exception("This is not possible for space_time");
       
       static Timer t("symbolicCutBFI - CoDim2", NoTracing);
       RegionTimer reg (t);
 
-      IVec<4> int_tuple = 
+      INT<4> int_tuple = 
         SwitchET<ET_HEX,ET_TET,ET_PRISM,ET_PYRAMID> (eltype1, [&LocalFacetNr1, &ElVertices1] (auto et)
          { return ET_trait<et>::GetFaceSort(LocalFacetNr1,ElVertices1); });
 
       // for(int i=0; i<NV; i++)
       //     if(abs(lset_fv[i]) < globxvar.EPS_INTERPOLATE_TO_P1 ) throw Exception("lset val 0 in SymbolicCutFacetBilinearFormIntegrator");
 
       FlatVector<> lset_fv(NV,lh);
@@ -796,15 +796,15 @@
             ip.SetWeight((*ir_scr)[i].Weight() * ratio_meas1D);
         }
       }
     }
     else if (Dim(etfacet) == 1) 
     {
 
-        IVec<2> int_tuple = 
+        INT<2> int_tuple = 
           SwitchET<ET_TRIG,ET_QUAD> (eltype1, [&LocalFacetNr1, &ElVertices1] (auto et) { return ET_trait<et>::GetEdgeSort(LocalFacetNr1,ElVertices1); });
 
         if(time_order < 0) {
             Vec<2> lset_vals_edge = {elvec[int_tuple[0]],elvec[int_tuple[1]]}; 
             ir_scr = StraightCutIntegrationRuleUntransformed(lset_vals_edge, etfacet, lsetintdom->GetDomainType(), 2*maxorder, FIND_OPTIMAL, lh);
         }
         else {
```

### Comparing `xfem-2.1.2303.post72.dev0/xfem/symboliccutbfi.hpp` & `xfem-2.1.2303.post8.dev0/xfem/symboliccutbfi.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/xfem/symboliccutlfi.cpp` & `xfem-2.1.2303.post8.dev0/xfem/symboliccutlfi.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/xfem/symboliccutlfi.hpp` & `xfem-2.1.2303.post8.dev0/xfem/symboliccutlfi.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/xfem/xFESpace.cpp` & `xfem-2.1.2303.post8.dev0/xfem/xFESpace.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/xfem/xFESpace.hpp` & `xfem-2.1.2303.post8.dev0/xfem/xFESpace.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/xfem/xfemdiffops.cpp` & `xfem-2.1.2303.post8.dev0/xfem/xfemdiffops.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/xfem/xfemdiffops.hpp` & `xfem-2.1.2303.post8.dev0/xfem/xfemdiffops.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/xfem/xfiniteelement.cpp` & `xfem-2.1.2303.post8.dev0/xfem/xfiniteelement.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/xfem/xfiniteelement.hpp` & `xfem-2.1.2303.post8.dev0/xfem/xfiniteelement.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post72.dev0/xfem.egg-info/SOURCES.txt` & `xfem-2.1.2303.post8.dev0/xfem.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 ./CMakeLists.txt
 ./MANIFEST.in
 ./build/temp.linux-x86_64-cpython-310/CMakeFiles/3.25.0/CompilerIdCXX/CMakeCXXCompilerId.cpp
+./build/temp.linux-x86_64-cpython-311/CMakeFiles/3.25.0/CompilerIdCXX/CMakeCXXCompilerId.cpp
+./build/temp.linux-x86_64-cpython-38/CMakeFiles/3.25.0/CompilerIdCXX/CMakeCXXCompilerId.cpp
+./build/temp.linux-x86_64-cpython-39/CMakeFiles/3.25.0/CompilerIdCXX/CMakeCXXCompilerId.cpp
 ./cmake_modules/cmake_uninstall.cmake.in
 ./cutint/CMakeLists.txt
 ./cutint/cutintegral.cpp
 ./cutint/cutintegral.hpp
 ./cutint/fieldeval.cpp
 ./cutint/fieldeval.hpp
 ./cutint/lsetintdomain.cpp
@@ -85,15 +88,14 @@
 ./xfem/xFESpace.hpp
 ./xfem/xfemdiffops.cpp
 ./xfem/xfemdiffops.hpp
 ./xfem/xfiniteelement.cpp
 ./xfem/xfiniteelement.hpp
 python/__init__.py
 python/cutmg.py
-python/lset_smoothblend.py
 python/lset_spacetime.py
 python/lsetcurv.py
 python/mlset.py
 python/ngs_check.py
 python/utils.py
 xfem.egg-info/PKG-INFO
 xfem.egg-info/SOURCES.txt
```

