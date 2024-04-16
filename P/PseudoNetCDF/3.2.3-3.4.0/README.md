# Comparing `tmp/PseudoNetCDF-3.2.3.tar.gz` & `tmp/pseudonetcdf-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PseudoNetCDF-3.2.3.tar", last modified: Mon Mar  4 18:36:04 2024, max compression
+gzip compressed data, was "pseudonetcdf-3.4.0.tar", last modified: Tue Apr 16 14:07:57 2024, max compression
```

## Comparing `PseudoNetCDF-3.2.3.tar` & `pseudonetcdf-3.4.0.tar`

### file list

```diff
@@ -1,298 +1,300 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.954155 PseudoNetCDF-3.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-03-04 18:36:04.954155 PseudoNetCDF-3.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.914155 PseudoNetCDF-3.2.3/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3160 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/scripts/pnc1d.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      525 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/scripts/pnc2d.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5168 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/scripts/pncaqsraw4pnceval.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7355 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/scripts/pncaqsrest4pnceval.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7467 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/scripts/pncasos4pnceval.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12399 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/scripts/pncboundaries.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2566 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/scripts/pncdiurnal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      160 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/scripts/pncdump
--rwxr-xr-x   0 runner    (1001) docker     (127)       67 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/scripts/pncdump.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      160 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/scripts/pnceval
--rwxr-xr-x   0 runner    (1001) docker     (127)       67 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/scripts/pnceval.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/scripts/pncgen
--rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/scripts/pncgen.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    71580 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/scripts/pncglobal2cmaq.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      160 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/scripts/pncload
--rwxr-xr-x   0 runner    (1001) docker     (127)    12034 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/scripts/pncmadis2pnceval.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      452 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/scripts/pncmap.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2152 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/scripts/pncqq.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      502 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/scripts/pncscatter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      479 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/scripts/pncts.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      418 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/scripts/pncvertprofile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      160 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/scripts/pncview
--rwxr-xr-x   0 runner    (1001) docker     (127)       67 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/scripts/pncview.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4798 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/scripts/pncwindrose.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 18:36:04.954155 PseudoNetCDF-3.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.902155 PseudoNetCDF-3.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.918155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/ArrayTransforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    14189 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/MetaNetCDF.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5449 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/_getreader.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/_getwriter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.918155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/aermodfiles/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/aermodfiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/aermodfiles/_aermod_plotfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.922155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/
--rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/ArrayTransforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    14145 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/FortranFileUtil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/Memmaps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/Readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/Writers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/aerosol_names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.922155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/cloud_rain/
--rw-r--r--   0 runner    (1001) docker     (127)    11075 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/cloud_rain/Memmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/cloud_rain/Transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/cloud_rain/Write.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/cloud_rain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.922155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/finst/
--rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/finst/Memmap.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/finst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.922155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/height_pressure/
--rw-r--r--   0 runner    (1001) docker     (127)     9053 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/height_pressure/Memmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/height_pressure/Read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/height_pressure/Transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/height_pressure/Write.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/height_pressure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.922155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/humidity/
--rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/humidity/Memmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/humidity/Read.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/humidity/Transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/humidity/Write.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/humidity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.926155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/ipr/
--rw-r--r--   0 runner    (1001) docker     (127)    12509 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/ipr/Memmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    15329 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/ipr/Read.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/ipr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.926155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/irr/
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/irr/Memmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    13702 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/irr/Read.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/irr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.926155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/landuse/
--rw-r--r--   0 runner    (1001) docker     (127)    10532 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/landuse/Memmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/landuse/Write.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/landuse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.926155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/lateral_boundary/
--rw-r--r--   0 runner    (1001) docker     (127)    15633 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/lateral_boundary/Memmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/lateral_boundary/Write.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/lateral_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/lateral_boundary/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.926155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/one3d/
--rw-r--r--   0 runner    (1001) docker     (127)     8853 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/one3d/Memmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    12605 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/one3d/Read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/one3d/Write.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/one3d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.902155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/pig/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.926155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/pig/greasd/
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/pig/greasd/Memmap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.926155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/point_source/
--rw-r--r--   0 runner    (1001) docker     (127)    13524 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/point_source/Memmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    12530 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/point_source/Read.py
--rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/point_source/Write.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/point_source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.930155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/temperature/
--rw-r--r--   0 runner    (1001) docker     (127)     9446 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/temperature/Memmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    10841 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/temperature/Read.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/temperature/Transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/temperature/Write.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/temperature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/timetuple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.930155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/uamiv/
--rw-r--r--   0 runner    (1001) docker     (127)    14853 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/uamiv/Memmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    13617 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/uamiv/Read.py
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/uamiv/Transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    12358 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/uamiv/Write.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/uamiv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/uamiv/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/units.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.930155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/vertical_diffusivity/
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/vertical_diffusivity/Memmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/vertical_diffusivity/Read.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/vertical_diffusivity/Transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/vertical_diffusivity/Write.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/vertical_diffusivity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.930155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/wind/
--rw-r--r--   0 runner    (1001) docker     (127)     9201 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/wind/Memmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    14339 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/wind/Read.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/wind/Transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/wind/Write.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/wind/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.934155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/ceilometerfiles/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/ceilometerfiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/ceilometerfiles/_vaisala.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.934155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/cmaqfiles/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/cmaqfiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/cmaqfiles/_cmaqomidat.py
--rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/cmaqfiles/_griddesc.py
--rw-r--r--   0 runner    (1001) docker     (127)    44603 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/cmaqfiles/_ioapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/cmaqfiles/_jtable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/cmaqfiles/boxmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/cmaqfiles/pa.py
--rw-r--r--   0 runner    (1001) docker     (127)     9173 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/cmaqfiles/profile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.934155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/conventions/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/conventions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.934155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/conventions/cdo/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/conventions/cdo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/conventions/cdo/_grids.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.934155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/conventions/cf/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/conventions/cf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/conventions/cf/_cf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.934155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/conventions/ioapi/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/conventions/ioapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16605 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/conventions/ioapi/_ioapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/conventions/ioapi/_wrfioapi.py
--rw-r--r--   0 runner    (1001) docker     (127)    30605 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/coordutil.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.938155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/core/_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (127)    94088 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/core/_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    40342 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/core/_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/core/_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/core/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    15189 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/core/_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/core/_wrapnc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.938155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/derived/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/derived/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/derived/met.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.938155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/epafiles/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/epafiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8283 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/epafiles/_aqsraw.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.938155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/geoschemfiles/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/geoschemfiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    58670 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/geoschemfiles/_bpch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8371 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/geoschemfiles/_bpchmaster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/geoschemfiles/_cspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/geoschemfiles/_gcnc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15681 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/geoschemfiles/_geos.py
--rw-r--r--   0 runner    (1001) docker     (127)    20530 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/geoschemfiles/_newbpch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/geoschemfiles/_planelog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/geoschemfiles/_vertcoord.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.938155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/icarttfiles/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/icarttfiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16281 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/icarttfiles/ffi1001.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.938155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/morphofiles/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4760 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/morphofiles/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/net_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/netcdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.942155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/noaafiles/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/noaafiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34682 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/noaafiles/_arl.py
--rw-r--r--   0 runner    (1001) docker     (127)    12953 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/noaafiles/_cdump.py
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/noaafiles/_l100.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/noaafiles/_pdump.py
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/noaafiles/_tdump.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/noaafiles/arltime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.942155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/plotutil/
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/plotutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/plotutil/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/plotutil/pnc2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/plotutil/pncmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/plotutil/pncscatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/plotutil/pncts.py
--rw-r--r--   0 runner    (1001) docker     (127)    15538 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/plotutil/vertprofile.py
--rw-r--r--   0 runner    (1001) docker     (127)    13004 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/pncdump.py
--rw-r--r--   0 runner    (1001) docker     (127)    18724 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/pnceval.py
--rw-r--r--   0 runner    (1001) docker     (127)     9935 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/pncgen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/pncload.py
--rw-r--r--   0 runner    (1001) docker     (127)    35668 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/pncparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    24710 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/pncview.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/pncwarn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.942155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/racmfiles/
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/racmfiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/racmfiles/boxmodel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.942155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/raob/
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/raob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/sci_var.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.946155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/test/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/test/test_arraytransforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/test/test_camxfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/test/test_ceilometer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13114 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/test/test_cmaqfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    38216 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/test/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/test/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/test/test_geoschemfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/test/test_icarttfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/test/test_pncopen.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/test/test_textfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/test/test_toms.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/test/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/test/test_woudc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.946155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.906155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.946155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/cloud_rain/
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/cloud_rain/test.cloud_rain
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.946155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/height_pressure/
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/height_pressure/test.height_pressure
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.946155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/humidity/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/humidity/test.humidity
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.946155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/landuse/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/landuse/test.landuse
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.946155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/lateral_boundary/
--rw-r--r--   0 runner    (1001) docker     (127)    46828 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/lateral_boundary/test.lateral_boundary
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.946155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/point_source/
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/point_source/test.point_source
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.946155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/temperature/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/temperature/test.temperature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.946155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/uamiv/
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/uamiv/test.uamiv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.946155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/vertical_diffusivity/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/vertical_diffusivity/test.vertical_diffusivity
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.946155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/wind/
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/wind/test.wind
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.950155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/ceilometerfiles/
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/ceilometerfiles/VAISALA_CEILOMETER_1_LEVEL2_20.his
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.906155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/cmaqfiles/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.950155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/cmaqfiles/griddesc/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/cmaqfiles/griddesc/GRIDDESC
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.950155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/cmaqfiles/profiles/
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/cmaqfiles/profiles/test.bcon_profile
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/cmaqfiles/profiles/test.icon_profile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.950155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/geoschemfiles/
--rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/geoschemfiles/diaginfo.dat
--rw-r--r--   0 runner    (1001) docker     (127)    27748 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/geoschemfiles/test.bpch
--rw-r--r--   0 runner    (1001) docker     (127)    28016 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/geoschemfiles/tracerinfo.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.950155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/icarttfiles/
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/icarttfiles/test.ffi1001
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.950155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/net_balance/
--rw-r--r--   0 runner    (1001) docker     (127)    92505 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/net_balance/test.mrg_file
--rw-r--r--   0 runner    (1001) docker     (127)    39939 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/net_balance/test.net_file
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.950155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/toms/
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/toms/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.950155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/woudcfiles/
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/woudcfiles/test_woudc.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.950155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/textfiles/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/textfiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/textfiles/_delimited.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/textfiles/esrl_sonde.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/textfiles/shadoz_sonde.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.950155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/toms/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/toms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/toms/level3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/userfuncs.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.950155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/woudcfiles/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/woudcfiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7717 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/woudcfiles/_woudc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.950155 PseudoNetCDF-3.2.3/src/PseudoNetCDF/wrffiles/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/wrffiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-03-04 18:35:52.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF/wrffiles/_wrfioapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:36:04.950155 PseudoNetCDF-3.2.3/src/PseudoNetCDF.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-03-04 18:36:04.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-03-04 18:36:04.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 18:36:04.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-04 18:36:04.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-03-04 18:36:04.000000 PseudoNetCDF-3.2.3/src/PseudoNetCDF.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.883072 pseudonetcdf-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-16 14:07:57.883072 pseudonetcdf-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.843072 pseudonetcdf-3.4.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3160 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/scripts/pnc1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      525 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/scripts/pnc2d.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5168 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/scripts/pncaqsraw4pnceval.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7355 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/scripts/pncaqsrest4pnceval.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7467 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/scripts/pncasos4pnceval.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12399 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/scripts/pncboundaries.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2566 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/scripts/pncdiurnal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      160 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/scripts/pncdump
+-rwxr-xr-x   0 runner    (1001) docker     (127)       67 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/scripts/pncdump.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      160 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/scripts/pnceval
+-rwxr-xr-x   0 runner    (1001) docker     (127)       67 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/scripts/pnceval.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/scripts/pncgen
+-rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/scripts/pncgen.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    71580 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/scripts/pncglobal2cmaq.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      160 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/scripts/pncload
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12034 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/scripts/pncmadis2pnceval.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      452 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/scripts/pncmap.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2152 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/scripts/pncqq.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      502 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/scripts/pncscatter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      479 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/scripts/pncts.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      418 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/scripts/pncvertprofile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      160 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/scripts/pncview
+-rwxr-xr-x   0 runner    (1001) docker     (127)       67 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/scripts/pncview.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4798 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/scripts/pncwindrose.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 14:07:57.883072 pseudonetcdf-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.831072 pseudonetcdf-3.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.847072 pseudonetcdf-3.4.0/src/PseudoNetCDF/
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/ArrayTransforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14189 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/MetaNetCDF.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/_getreader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/_getwriter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.851072 pseudonetcdf-3.4.0/src/PseudoNetCDF/aermodfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/aermodfiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/aermodfiles/_aermod_plotfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.851072 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/ArrayTransforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14149 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/FortranFileUtil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/Memmaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/Readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/Writers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/aerosol_names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.851072 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/cloud_rain/
+-rw-r--r--   0 runner    (1001) docker     (127)    11075 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/cloud_rain/Memmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/cloud_rain/Transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/cloud_rain/Write.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/cloud_rain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.851072 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/finst/
+-rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/finst/Memmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/finst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.855072 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/height_pressure/
+-rw-r--r--   0 runner    (1001) docker     (127)     9053 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/height_pressure/Memmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/height_pressure/Read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/height_pressure/Transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/height_pressure/Write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/height_pressure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.855072 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/humidity/
+-rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/humidity/Memmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/humidity/Read.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/humidity/Transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/humidity/Write.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/humidity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.855072 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/ipr/
+-rw-r--r--   0 runner    (1001) docker     (127)    12509 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/ipr/Memmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15329 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/ipr/Read.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/ipr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.855072 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/irr/
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/irr/Memmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13702 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/irr/Read.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/irr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.855072 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/landuse/
+-rw-r--r--   0 runner    (1001) docker     (127)    10532 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/landuse/Memmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/landuse/Write.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/landuse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.855072 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/lateral_boundary/
+-rw-r--r--   0 runner    (1001) docker     (127)    15633 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/lateral_boundary/Memmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/lateral_boundary/Write.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/lateral_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/lateral_boundary/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.859072 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/one3d/
+-rw-r--r--   0 runner    (1001) docker     (127)     8853 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/one3d/Memmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12605 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/one3d/Read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/one3d/Write.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/one3d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.835072 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/pig/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.859072 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/pig/greasd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/pig/greasd/Memmap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.859072 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/point_source/
+-rw-r--r--   0 runner    (1001) docker     (127)    13524 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/point_source/Memmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12530 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/point_source/Read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/point_source/Write.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/point_source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.859072 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/temperature/
+-rw-r--r--   0 runner    (1001) docker     (127)     9446 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/temperature/Memmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10841 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/temperature/Read.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/temperature/Transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/temperature/Write.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/temperature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/timetuple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.859072 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/uamiv/
+-rw-r--r--   0 runner    (1001) docker     (127)    14853 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/uamiv/Memmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13617 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/uamiv/Read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/uamiv/Transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/uamiv/Write.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/uamiv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/uamiv/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.859072 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/vertical_diffusivity/
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/vertical_diffusivity/Memmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/vertical_diffusivity/Read.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/vertical_diffusivity/Transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/vertical_diffusivity/Write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/vertical_diffusivity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.863072 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/wind/
+-rw-r--r--   0 runner    (1001) docker     (127)     9201 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/wind/Memmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14355 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/wind/Read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/wind/Transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/wind/Write.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/wind/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.863072 pseudonetcdf-3.4.0/src/PseudoNetCDF/ceilometerfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/ceilometerfiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/ceilometerfiles/_vaisala.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.863072 pseudonetcdf-3.4.0/src/PseudoNetCDF/cmaqfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/cmaqfiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/cmaqfiles/_cmaqomidat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/cmaqfiles/_griddesc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44621 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/cmaqfiles/_ioapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/cmaqfiles/_jtable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/cmaqfiles/boxmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/cmaqfiles/pa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9173 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/cmaqfiles/profile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.863072 pseudonetcdf-3.4.0/src/PseudoNetCDF/conventions/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/conventions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.863072 pseudonetcdf-3.4.0/src/PseudoNetCDF/conventions/cdo/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/conventions/cdo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/conventions/cdo/_grids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.863072 pseudonetcdf-3.4.0/src/PseudoNetCDF/conventions/cf/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/conventions/cf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/conventions/cf/_cf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.863072 pseudonetcdf-3.4.0/src/PseudoNetCDF/conventions/ioapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/conventions/ioapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18703 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/conventions/ioapi/_ioapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/conventions/ioapi/_wrfioapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30605 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/coordutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.867072 pseudonetcdf-3.4.0/src/PseudoNetCDF/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/core/_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    94088 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/core/_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40342 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/core/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/core/_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/core/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15189 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/core/_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/core/_wrapnc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.867072 pseudonetcdf-3.4.0/src/PseudoNetCDF/derived/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/derived/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/derived/met.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.867072 pseudonetcdf-3.4.0/src/PseudoNetCDF/epafiles/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/epafiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8283 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/epafiles/_aqsraw.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.867072 pseudonetcdf-3.4.0/src/PseudoNetCDF/geoschemfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/geoschemfiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58670 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/geoschemfiles/_bpch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8371 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/geoschemfiles/_bpchmaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/geoschemfiles/_cspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/geoschemfiles/_gcnc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15681 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/geoschemfiles/_geos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20530 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/geoschemfiles/_newbpch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/geoschemfiles/_planelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/geoschemfiles/_vertcoord.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.871072 pseudonetcdf-3.4.0/src/PseudoNetCDF/icarttfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/icarttfiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16281 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/icarttfiles/ffi1001.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.871072 pseudonetcdf-3.4.0/src/PseudoNetCDF/morphofiles/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4760 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/morphofiles/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/net_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/netcdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.871072 pseudonetcdf-3.4.0/src/PseudoNetCDF/noaafiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/noaafiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34682 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/noaafiles/_arl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12953 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/noaafiles/_cdump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/noaafiles/_l100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/noaafiles/_pdump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/noaafiles/_tdump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/noaafiles/arltime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.871072 pseudonetcdf-3.4.0/src/PseudoNetCDF/plotutil/
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/plotutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/plotutil/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/plotutil/pnc2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/plotutil/pncmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/plotutil/pncscatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/plotutil/pncts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15538 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/plotutil/vertprofile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13004 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/pncdump.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18724 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/pnceval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9935 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/pncgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/pncload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35668 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/pncparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24710 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/pncview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/pncwarn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.871072 pseudonetcdf-3.4.0/src/PseudoNetCDF/racmfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/racmfiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/racmfiles/boxmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.871072 pseudonetcdf-3.4.0/src/PseudoNetCDF/raob/
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/raob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/sci_var.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.875072 pseudonetcdf-3.4.0/src/PseudoNetCDF/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/test/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/test/test_arraytransforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/test/test_camxfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/test/test_ceilometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13114 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/test/test_cmaqfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38216 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/test/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/test/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/test/test_geoschemfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/test/test_icarttfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/test/test_pncopen.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/test/test_textfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/test/test_toms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/test/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/test/test_woudc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.875072 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.839072 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.875072 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/cloud_rain/
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/cloud_rain/test.cloud_rain
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.875072 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/height_pressure/
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/height_pressure/test.height_pressure
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.875072 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/humidity/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/humidity/test.humidity
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.875072 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/landuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/landuse/test.landuse
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.875072 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/lateral_boundary/
+-rw-r--r--   0 runner    (1001) docker     (127)    46828 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/lateral_boundary/test.lateral_boundary
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.875072 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/point_source/
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/point_source/test.point_source
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.875072 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/temperature/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/temperature/test.temperature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.875072 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/uamiv/
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/uamiv/test.uamiv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.875072 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/vertical_diffusivity/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/vertical_diffusivity/test.vertical_diffusivity
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.875072 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/wind/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/wind/test.wind
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.875072 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/ceilometerfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/ceilometerfiles/VAISALA_CEILOMETER_1_LEVEL2_20.his
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.839072 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/cmaqfiles/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.879072 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/cmaqfiles/griddesc/
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/cmaqfiles/griddesc/GRIDDESC
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.879072 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/cmaqfiles/profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/cmaqfiles/profiles/test.bcon_profile
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/cmaqfiles/profiles/test.icon_profile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.879072 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/geoschemfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/geoschemfiles/diaginfo.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    27748 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/geoschemfiles/test.bpch
+-rw-r--r--   0 runner    (1001) docker     (127)    28016 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/geoschemfiles/tracerinfo.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.879072 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/icarttfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/icarttfiles/test.ffi1001
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.879072 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/net_balance/
+-rw-r--r--   0 runner    (1001) docker     (127)    92505 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/net_balance/test.mrg_file
+-rw-r--r--   0 runner    (1001) docker     (127)    39939 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/net_balance/test.net_file
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.879072 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/toms/
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/toms/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.879072 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/woudcfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/woudcfiles/test_woudc.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.879072 pseudonetcdf-3.4.0/src/PseudoNetCDF/textfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/textfiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/textfiles/_delimited.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/textfiles/esrl_sonde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/textfiles/shadoz_sonde.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.879072 pseudonetcdf-3.4.0/src/PseudoNetCDF/toms/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/toms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/toms/level3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/userfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.879072 pseudonetcdf-3.4.0/src/PseudoNetCDF/woudcfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/woudcfiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7717 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/woudcfiles/_woudc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.879072 pseudonetcdf-3.4.0/src/PseudoNetCDF/wrffiles/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/wrffiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/wrffiles/_wrfioapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-16 14:07:49.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF/xarray_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:07:57.879072 pseudonetcdf-3.4.0/src/PseudoNetCDF.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-16 14:07:57.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-04-16 14:07:57.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:07:57.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-16 14:07:57.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-16 14:07:57.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-16 14:07:57.000000 pseudonetcdf-3.4.0/src/PseudoNetCDF.egg-info/top_level.txt
```

### Comparing `PseudoNetCDF-3.2.3/LICENSE` & `pseudonetcdf-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/PKG-INFO` & `pseudonetcdf-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PseudoNetCDF
-Version: 3.2.3
+Version: 3.4.0
 Summary: Like NetCDF and NCO, but works with NetCDF and other scientific formats.
 Home-page: http://github.com/barronh/pseudonetcdf/
 Author: Barron Henderson
 Author-email: barronh@gmail.com
 Maintainer: Barron Henderson
 Maintainer-email: barronh@gmail.com
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `PseudoNetCDF-3.2.3/README.md` & `pseudonetcdf-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/scripts/pnc1d.py` & `pseudonetcdf-3.4.0/scripts/pnc1d.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/scripts/pnc2d.py` & `pseudonetcdf-3.4.0/scripts/pnc2d.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/scripts/pncaqsraw4pnceval.py` & `pseudonetcdf-3.4.0/scripts/pncaqsraw4pnceval.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/scripts/pncaqsrest4pnceval.py` & `pseudonetcdf-3.4.0/scripts/pncaqsrest4pnceval.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/scripts/pncasos4pnceval.py` & `pseudonetcdf-3.4.0/scripts/pncasos4pnceval.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/scripts/pncboundaries.py` & `pseudonetcdf-3.4.0/scripts/pncboundaries.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/scripts/pncdiurnal.py` & `pseudonetcdf-3.4.0/scripts/pncdiurnal.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/scripts/pncglobal2cmaq.py` & `pseudonetcdf-3.4.0/scripts/pncglobal2cmaq.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/scripts/pncmadis2pnceval.py` & `pseudonetcdf-3.4.0/scripts/pncmadis2pnceval.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/scripts/pncqq.py` & `pseudonetcdf-3.4.0/scripts/pncqq.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/scripts/pncwindrose.py` & `pseudonetcdf-3.4.0/scripts/pncwindrose.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/setup.py` & `pseudonetcdf-3.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     'textfiles': ['pandas'],
     'projections': ['pyproj'],
     'mapping': ['basemap'],
 }
 
 setup(
     name='PseudoNetCDF',
-    version='3.2.3',
+    version='3.4.0',
     author='Barron Henderson',
     author_email='barronh@gmail.com',
     maintainer='Barron Henderson',
     maintainer_email='barronh@gmail.com',
     description=(
         'Like NetCDF and NCO, but works with NetCDF and other ' +
         'scientific formats.'
@@ -96,14 +96,17 @@
     packages=packages,
     package_dir={'': 'src'},
     include_package_data=True,
     package_data={'PseudoNetCDF': data},
     scripts=script_list,
     install_requires=requires_list,
     extras_require=extra_requires_dict,
+    entry_points={
+        "xarray.backends": ["pseudonetcdf=PseudoNetCDF.xarray_plugin:PseudoNetCDFBackend"],
+    },
     url='http://github.com/barronh/pseudonetcdf/',
     classifiers=[
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Operating System :: MacOS',
         'Operating System :: Microsoft :: Windows',
         'Operating System :: POSIX',
```

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/ArrayTransforms.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/ArrayTransforms.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/MetaNetCDF.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/MetaNetCDF.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/__init__.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/__init__.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/_getreader.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/_getreader.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,32 +78,33 @@
             newdoc = '\n        - '.join([pncopen.__doc__, name])
             pncopen.__doc__ = newdoc
         return True
     else:
         return False
 
 
-def pncmfopen(*args, stackdim=None, **kwds):
+def pncmfopen(paths, *args, stackdim=None, **kwds):
     """Open any PNC supported format using pncopen on all files
     passed as teh first argument of pncmfopen. See pncopen
 
     Parameters
     ----------
+    paths : list
+        List of paths to open
     args : arguments
-        args[0] must be a list of paths, other arguments are format specific
+        pncopen arguments (see pncopen)
     stackdim : str
         dimension upon which to stack files
     kwds : dict
-        see pncopen for more details
+        pncopen and format-specific keywords (see pncopen for more details)
 
     Returns
     -------
     pfile : PseudoNetCDF
     """
-    paths = args[0]
     files = [pncopen(path, *args[1:], **kwds) for path in paths]
     file1 = files[0]
     return file1.stack(files[1:], stackdim=stackdim)
 
 
 def pncopen(*args, **kwds):
     """Open any PNC supported format using args and kwds, which
@@ -117,15 +118,16 @@
         keywords for reader (see format)
     format : string
         name of reader (not passed to reader), default auto-detect
         see Format Options for formats
     addcf : boolean
         to add CF conventions (not passed to reader; default: False)
     diskless : boolean
-        to add CF conventions (not passed to reader; default: False)
+        If addcf (default: False), the file must either be wrapped or loaded
+        into memory (diskless) to add attributes.
     help : boolean
         without format, returns help of pncopen and with format keyword,
         returns help of that class. See the __init__ interface for help
         with keywords that are not in the class __doc__.
 
     Returns
     -------
```

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/_getwriter.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/_getwriter.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/aermodfiles/_aermod_plotfile.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/aermodfiles/_aermod_plotfile.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/ArrayTransforms.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/ArrayTransforms.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/FortranFileUtil.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/FortranFileUtil.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,15 +316,15 @@
     """All CAMx files use FortranFileUtil.RecordFiles
     as inputs.  This function decides if the input was
     of the right type.  If not, it tries to make a RecordFile
     from the input.
 
     rf - str, unicode, file, RecordFile
     """
-    if type(rf) == RecordFile:
+    if isinstance(rf, RecordFile):
         pass
     else:
         rf = RecordFile(rf)
     rf._newrecord(0)
     return rf
```

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/Memmaps.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/Memmaps.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/Readers.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/Readers.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/Writers.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/Writers.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/__init__.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/__init__.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/aerosol_names.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/aerosol_names.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/cloud_rain/Memmap.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/cloud_rain/Memmap.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/cloud_rain/Transforms.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/cloud_rain/Transforms.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/cloud_rain/Write.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/cloud_rain/Write.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/cloud_rain/__init__.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/cloud_rain/__init__.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/finst/Memmap.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/finst/Memmap.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/finst/__init__.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/finst/__init__.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/height_pressure/Memmap.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/height_pressure/Memmap.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/height_pressure/Read.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/height_pressure/Read.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/height_pressure/Transforms.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/height_pressure/Transforms.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/height_pressure/Write.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/height_pressure/Write.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/height_pressure/__init__.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/height_pressure/__init__.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/humidity/Memmap.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/humidity/Memmap.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/humidity/Read.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/humidity/Read.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/humidity/Transforms.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/humidity/Transforms.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/humidity/Write.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/humidity/Write.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/humidity/__init__.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/humidity/__init__.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/ipr/Memmap.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/ipr/Memmap.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/ipr/Read.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/ipr/Read.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/ipr/__init__.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/ipr/__init__.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/irr/Memmap.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/irr/Memmap.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/irr/Read.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/irr/Read.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/irr/__init__.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/irr/__init__.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/landuse/Memmap.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/landuse/Memmap.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/landuse/Write.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/landuse/Write.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/landuse/__init__.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/landuse/__init__.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/lateral_boundary/Memmap.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/lateral_boundary/Memmap.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/lateral_boundary/Write.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/lateral_boundary/Write.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/lateral_boundary/__init__.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/lateral_boundary/__init__.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/lateral_boundary/__main__.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/lateral_boundary/__main__.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/one3d/Memmap.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/one3d/Memmap.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/one3d/Read.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/one3d/Read.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/one3d/Write.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/one3d/Write.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/pig/greasd/Memmap.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/pig/greasd/Memmap.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/point_source/Memmap.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/point_source/Memmap.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/point_source/Read.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/point_source/Read.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/point_source/Write.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/point_source/Write.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/point_source/__init__.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/point_source/__init__.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/temperature/Memmap.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/temperature/Memmap.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/temperature/Read.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/temperature/Read.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/temperature/Transforms.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/temperature/Transforms.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/temperature/Write.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/temperature/Write.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/temperature/__init__.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/temperature/__init__.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/timetuple.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/timetuple.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/uamiv/Memmap.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/uamiv/Memmap.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/uamiv/Read.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/uamiv/Read.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/uamiv/Transforms.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/uamiv/Transforms.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,18 +55,18 @@
              if k[:3] in ('NOX', 'VOC', 'O3V', 'O3N')])
 
         # Create global keys
         self.__sourcesbyNm[''] = tuple(self.__sourcesbyNm.keys())
         self.__regionsbyNm[''] = tuple(self.__regionsbyNm.keys())
 
         for k, v in sources.items():
-            if type(v) == str:
+            if isinstance(v, str):
                 sources[k] = (v,)
         for k, v in regions.items():
-            if type(v) == str:
+            if isinstance(v, str):
                 regions[k] = (v,)
 
         # Update with user supplied keys
         self.__sourcesbyNm.update(sources)
         self.__regionsbyNm.update(regions)
 
         self.dimensions = self.__child.dimensions.copy()
```

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/uamiv/Write.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/uamiv/Write.py`

 * *Files 5% similar despite different names*

```diff
@@ -107,42 +107,62 @@
                     diffidx = np.where(~check)
                 print(old.variables[k][diffidx])
                 print(new.variables[k][diffidx])
 
     """
 
     emiss_hdr = np.zeros(shape=(1,), dtype=_emiss_hdr_fmt)
+    # name is a tricky attribute, so CAMx_NAME was used to
+    # replace it. The FILEDESC property often has the name.
+    # otherwise, default to AVERAGE
+    nametxt = getattr(
+        ncffile, 'NAME', getattr(
+            ncffile, 'CAMx_NAME', getattr(
+                ncffile, 'FILEDESC', 'AVERAGE'
+            )
+        )
+    )
+    # The name must be exactly 10 characters long
+    nametxt = nametxt.ljust(10)[:10]
     emiss_hdr[0]['name'][:, :] = ' '
-    emiss_hdr[0]['name'][:, 0] = np.array(ncffile.NAME, dtype='>c')
+    emiss_hdr[0]['name'][:, 0] = np.array(nametxt, dtype='>c')
+    # Note should be there, but FILEDESC is used as a backup
+    notetxt = getattr(ncffile, 'NOTE', getattr(ncffile, 'FILEDESC', ''))
+    # Note must be exactly 40 characters long
+    notetxt = nametxt.ljust(60)[:60]
     emiss_hdr[0]['note'][:, :] = ' '
-    emiss_hdr[0]['note'][:, 0] = np.array(ncffile.NOTE, dtype='>c')
+    emiss_hdr[0]['note'][:, 0] = np.array(notetxt, dtype='>c')
     # gdtype = getattr(ncffile, 'GDTYP', -999)
-    emiss_hdr['itzon'][0] = ncffile.ITZON
+    emiss_hdr['itzon'][0] = getattr(ncffile, 'ITZON', 0)
     nspec = len(ncffile.dimensions['VAR'])
     emiss_hdr['nspec'] = nspec
 
     NCOLS = len(ncffile.dimensions['COL'])
     NROWS = len(ncffile.dimensions['ROW'])
     NLAYS = len(ncffile.dimensions['LAY'])
     grid_hdr = np.zeros(shape=(1,), dtype=_grid_hdr_fmt)
     grid_hdr['SPAD'] = grid_hdr.itemsize - 8
-    grid_hdr['plon'] = ncffile.PLON
-    grid_hdr['plat'] = ncffile.PLAT
-    grid_hdr['iutm'][0] = ncffile.IUTM
+    plon = getattr(ncffile, 'PLON', getattr(ncffile, 'XCENT'))
+    plat = getattr(ncffile, 'PLAT', getattr(ncffile, 'YCENT'))
+    tlat1 = getattr(ncffile, 'TLAT1', getattr(ncffile, 'P_ALP'))
+    tlat2 = getattr(ncffile, 'TLAT2', getattr(ncffile, 'P_BET'))
+    grid_hdr['plon'] = plon
+    grid_hdr['plat'] = plat
+    grid_hdr['iutm'][0] = getattr(ncffile, 'IUTM', 0)
     grid_hdr['xorg'] = ncffile.XORIG
     grid_hdr['yorg'] = ncffile.YORIG
     grid_hdr['delx'] = ncffile.XCELL
     grid_hdr['dely'] = ncffile.YCELL
     grid_hdr['nx'] = NCOLS
     grid_hdr['ny'] = NROWS
     grid_hdr['nz'] = NLAYS
     grid_hdr['iproj'] = ncffile.CPROJ
-    grid_hdr['tlat1'] = ncffile.TLAT1
-    grid_hdr['tlat2'] = ncffile.TLAT2
-    grid_hdr['istag'] = ncffile.ISTAG
+    grid_hdr['tlat1'] = tlat1
+    grid_hdr['tlat2'] = tlat2
+    grid_hdr['istag'] = getattr(ncffile, 'ISTAG', 0)
     grid_hdr['rdum5'] = 0.
     grid_hdr['EPAD'] = grid_hdr.itemsize - 8
 
     cell_hdr = np.zeros(shape=(1,), dtype=_cell_hdr_fmt)
     cell_hdr['SPAD'] = cell_hdr.itemsize - 8
     cell_hdr['ione1'] = 1
     cell_hdr['ione2'] = 1
```

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/uamiv/__init__.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/uamiv/__init__.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/uamiv/__main__.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/uamiv/__main__.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/units.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/units.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/util.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/util.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/vertical_diffusivity/Memmap.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/vertical_diffusivity/Memmap.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/vertical_diffusivity/Read.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/vertical_diffusivity/Read.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/vertical_diffusivity/Transforms.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/vertical_diffusivity/Transforms.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/vertical_diffusivity/Write.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/vertical_diffusivity/Write.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/vertical_diffusivity/__init__.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/vertical_diffusivity/__init__.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/wind/Memmap.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/wind/Memmap.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/wind/Read.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/wind/Read.py`

 * *Files 5% similar despite different names*

```diff
@@ -295,18 +295,18 @@
         for d, t, k in self.keys():
             y1, y2 = self.seekandread(d, t, k, 1), self.seekandread(d, t, k, 2)
             yield d, t, k, y1, y2
 
     __iter__ = keys
 
     def getArray(self, krange=slice(1, None)):
-        if type(krange) != slice:
-            if type(krange) == tuple:
+        if not isinstance(krange, slice):
+            if isinstance(krange, tuple):
                 krange = slice(*krange)
-            if type(krange) == int:
+            if isinstance(krange, int):
                 krange = slice(krange, krange + 1)
         a = zeros(
             (
                 self.time_step_count,
                 2,
                 len(range(*krange.indices(self.nlayers + 1))),
                 len(self.dimensions['ROW']),
```

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/wind/Transforms.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/wind/Transforms.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/wind/Write.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/wind/Write.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/camxfiles/wind/__init__.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/camxfiles/wind/__init__.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/ceilometerfiles/_vaisala.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/ceilometerfiles/_vaisala.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/cmaqfiles/__init__.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/cmaqfiles/__init__.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/cmaqfiles/_cmaqomidat.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/cmaqfiles/_cmaqomidat.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/cmaqfiles/_griddesc.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/cmaqfiles/_griddesc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import PseudoNetCDF as pnc
 from PseudoNetCDF.pncwarn import warn
 import os
 import io
+import re
 from datetime import datetime
 from collections import OrderedDict
 import numpy as np
 from ._ioapi import ioapi_base
 
 _prjp = ('GDTYP', 'P_ALP', 'P_BET', 'P_GAM', 'XCENT', 'YCENT')
 _grdp = (
@@ -36,15 +37,16 @@
     ):
         """
         Arguments
         ---------
         path : str or file-like
             If path is has a read method, it will be used directly.
             If path is a path to a file on disk, it will be read.
-            If none of these, it will try to treat the path as content.
+            If none of these, treat the path as text content.
+            If path is None, load a griddesc using properties provided.
         GDNAM : str
             Name the grid to be used. If not provided, the first will be used
         VGLVLS : tuple
             Iterable of layer edge (k+1) values for the vertical grid.
         VGTOP : float
             Top of vertical grid.
         VGTYP : int
@@ -73,51 +75,66 @@
         now = datetime.now()
         prj = {}
         grd = OrderedDict()
         if hasattr(path, 'read'):
             gdf = path
             path = '<inline>'
         elif path is None:
-            required_props = _prjp[1:] + _grdp[1:] + ('GDNAM',)
+            required_props = _prjp[:] + _grdp[1:] + ('GDNAM',)
             grid_kw = prop_kw.copy()
             if GDNAM is None:
                 grid_kw['GDNAM'] = 'UNKNOWN'
             else:
                 grid_kw['GDNAM'] = GDNAM
             grid_kw.setdefault('NTHIK', 1)
             grid_kw.setdefault('PRJNAME', 'UNKNOWN')
             for rpk in required_props:
                 if rpk not in grid_kw:
+                    if path is None and 'GRIDDESC' in os.environ:
+                        path = os.environ['GRIDDESC']
+                        gdf = open(path, 'r')
+                        break
                     raise KeyError(
                         f'{rpk} not found.'
                         + f'If path is None, {required_props} are required'
                     )
-            gdf = io.StringIO("""
+            else:
+                gdf = io.StringIO("""
 ' '
 '{PRJNAME}'
 {GDTYP} {P_ALP} {P_BET} {P_GAM} {XCENT} {YCENT}
 ' '
 '{GDNAM}'
 '{PRJNAME}' {XORIG} {YORIG} {XCELL} {YCELL} {NCOLS} {NROWS} {NTHIK}
 ' '""".format(**grid_kw))
             path = '<inline>'
         elif os.path.exists(path):
             gdf = open(path, 'r')
         else:
             gdf = io.StringIO(path)
             path = '<inline>'
-        gdlines = gdf.read().strip().split('\n')
+
+        gdtxt = gdf.read().replace(',', ' ').strip()
+        # Fortran allows exponential notation to use D or d
+        # instead of E or e, while Python does not.
+        dble = re.compile('([\d.])[Dd]([\d])')
+        gdtxt = dble.sub(r'\1e\2', gdtxt)
+        gdlines = gdtxt.split('\n')
         gdlines = [line.strip() for line in gdlines]
-        assert (gdlines[0] == "' '")
-        assert (gdlines[-1] == "' '")
+        # Remove comments that start with !
+        gdlines = [line.split('!')[0].strip() for line in gdlines]
+        # IOAPI does not verify first line, simply discards.
+        # dscgrid.f#L153
+        # assert (gdlines[0].replace(' ', '') == "''")
+        assert (gdlines[-1].replace(' ', '') == "''")
         i = 0
         blanks = []
         while i < len(gdlines):
             line = gdlines[i]
-            if line.strip() == "' '":
+            if line.strip() in ("' '", "''", ""):
                 blanks.append(i)
             else:
                 i += 1
                 parts = [eval(p) for p in gdlines[i].split()]
                 key = eval(line)
                 if len(blanks) == 1:
                     prj[key] = dict(zip(_prjp, parts))
```

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/cmaqfiles/_ioapi.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/cmaqfiles/_ioapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
             dimlens[dk] = len(dv)
 
         for dk in ['TSTEP', 'DATE-TIME', 'PERIM', 'LAY', 'VAR', 'ROW', 'COL']:
             audit[f'has_{dk}'] = dk in dimlens
             if dk in ('TSTEP', 'DATE-TIME', 'PERIM'):
                 continue
             audit[f'has_N{dk}S'] = hasattr(self, f'N{dk}S')
-            if audit[f'has_N{dk}S']:
+            if audit[f'has_N{dk}S'] and dk in dimlens:
                 audit[dk] = getattr(self, f'N{dk}S', 0) == dimlens[dk]
 
         if audit['has_ROW'] and audit['has_COL'] and not audit['has_PERIM']:
             del audit['has_PERIM']
             hdims = ('ROW', 'COL')
         elif audit['has_PERIM'] and not (audit['has_COL'] or audit['has_ROW']):
             del audit['has_ROW']
```

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/cmaqfiles/_jtable.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/cmaqfiles/_jtable.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/cmaqfiles/boxmodel.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/cmaqfiles/boxmodel.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/cmaqfiles/pa.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/cmaqfiles/pa.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/cmaqfiles/profile.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/cmaqfiles/profile.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/conventions/cdo/_grids.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/conventions/cdo/_grids.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/conventions/ioapi/_ioapi.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/conventions/ioapi/_ioapi.py`

 * *Files 11% similar despite different names*

```diff
@@ -166,43 +166,77 @@
     elif isph_parts[0] >= 0 and isph_parts[0] < _AXIS.size:
         return _AXIS[isph_parts[0]], _BXIS[isph_parts[0]]
     else:
         return isph_parts * 2
 
 
 _gdnames = {1: "latitude_longitude", 2: "lambert_conformal_conic",
+            3: "mercator", 5: "transverse_mercator",
             7: "mercator", 6: "polar_stereographic"}
 
 
 def getmapdef(ifileo, add=True):
-    gridname = _gdnames[ifileo.GDTYP]
+    gdtyp = ifileo.GDTYP
+    gridname = _gdnames[gdtyp]
     if add:
         mapdef = ifileo.createVariable(gridname, 'i', ())
     else:
         from PseudoNetCDF import PseudoNetCDFVariable
         mapdef = PseudoNetCDFVariable(ifileo, gridname, 'i', ())
     mapdef.grid_mapping_name = gridname
     if mapdef.grid_mapping_name == "latitude_longitude":
         mapdef.latitude_of_projection_origin = ifileo.YORIG
         mapdef.longitude_of_central_meridian = ifileo.XORIG
     elif mapdef.grid_mapping_name == "polar_stereographic":
         mapdef.latitude_of_projection_origin = ifileo.P_ALP * 90
         mapdef.straight_vertical_longitude_from_pole = ifileo.P_GAM
         mapdef.standard_parallel = np.array([ifileo.P_BET], dtype='d')
-        # mapdef.standard_parallel = np.array([ifileo.P_BET], dtype = 'f')
+    elif mapdef.grid_mapping_name == "mercator" and gdtyp == 3:
+        from PseudoNetCDF.pncwarn import warn
+        warn('mercator is untested. Be cautious.')
+        # IOAPI documentation sys YCENT/XCENT same as P_ALP/P_BET
+        assert (ifileo.P_ALP == ifileo.YCENT)
+        assert (ifileo.P_BET == ifileo.XCENT)
+        mapdef.standard_parallel = np.array([ifileo.P_GAM], dtype='d')
+    elif mapdef.grid_mapping_name == "mercator" and gdtyp == 7:
+        assert (ifileo.P_ALP == ifileo.YCENT)
+        assert (ifileo.P_GAM == ifileo.XCENT)
+    elif mapdef.grid_mapping_name == "transverse_mercator" and gdtyp == 5:
+        from PseudoNetCDF.pncwarn import warn
+        warn('UTM is untested. Be cautious.')
+        # diagnosted using
+        # proj = pyproj.Proj('+proj=utm +zone=18 +R=6370000')
+        # cf = proj.crs.to_cf()
+        # {k: v for k, v in cf.items() if k not in ('crs_wkt',)}
+        mapdef.latitude_of_projection_origin = 0.0
+        mapdef.longitude_of_central_meridian = ifileo.P_ALP * 6 + -183
+        # where did this come from?
+        # mapdef.scale_factor_at_central_meridian: 0.9996
+    elif mapdef.grid_mapping_name == "transverse_mercator" and gdtyp == 8:
+        from PseudoNetCDF.pncwarn import warn
+        warn('transverse_mercator is untested. Be cautious.')
+        mapdef.standard_parallel = np.array([ifileo.P_ALP], dtype='d')
+        mapdef.scale_factor_at_central_meridian = ifileo.P_BET
+        mapdef.longitude_of_central_meridian = ifileo.P_GAM
+        assert (ifileo.P_ALP == ifileo.YCENT)
+        assert (ifileo.P_GAM == ifileo.XCENT)
     else:
         mapdef.standard_parallel = np.array(
             [ifileo.P_ALP, ifileo.P_BET], dtype='d')
-    if mapdef.grid_mapping_name != "latitude_longitude":
+
+    if gdtyp not in (1, 5):  # not in latitude_longitude UTM
         mapdef.latitude_of_projection_origin = ifileo.YCENT
         mapdef.longitude_of_central_meridian = ifileo.XCENT
+
+    if gdtyp not in (1,):  # not in latitude_longitude
         mapdef.false_northing = -ifileo.YORIG
         mapdef.false_easting = -ifileo.XORIG
         mapdef._CoordinateTransformType = "Projection"
         mapdef._CoordinateAxes = "x y"
+
     ioapi_sphere = get_ioapi_sphere()
     mapdef.semi_major_axis = getattr(ifileo, 'semi_major_axis', getattr(
         ifileo, 'earth_radius', ioapi_sphere[0]))
     mapdef.semi_minor_axis = getattr(ifileo, 'semi_minor_axis', getattr(
         ifileo, 'earth_radius', ioapi_sphere[1]))
     return mapdef
 
@@ -255,24 +289,32 @@
         x = np.arange(0, ifileo.NCOLS) * ifileo.XCELL + \
             ifileo.XCELL / 2. + ifileo.XORIG
         y = np.arange(0, ifileo.NROWS) * ifileo.YCELL + \
             ifileo.YCELL / 2. + ifileo.YORIG
         lcc_x, lcc_y = np.meshgrid(x, y)
 
     if _withlatlon:
+        props = {k: mapdef.getncattr(k) for k in mapdef.ncattrs()}
         if ifileo.GDTYP == 2:
             mapstrs = ['+proj=lcc',
                        '+a=%s' % mapdef.semi_major_axis,
                        '+b=%s' % mapdef.semi_minor_axis,
                        '+lon_0=%s' % mapdef.longitude_of_central_meridian,
                        '+lat_1=%s' % mapdef.standard_parallel[0],
                        '+lat_2=%s' % mapdef.standard_parallel[1],
                        '+lat_0=%s' % mapdef.latitude_of_projection_origin]
             mapstr = ' '.join(mapstrs)
             mapproj = pyproj.Proj(mapstr)
+        elif ifileo.GDTYP == 5:
+            props['zone'] = ifileo.P_ALP
+            mapstr = (
+                '+proj=utm +zone={zone:.0f} +a={semi_major_axis}'
+                + ' +b={semi_minor_axis}'
+            ).format(**props)
+            mapproj = pyproj.Proj(mapstr)
         elif ifileo.GDTYP == 6:
             mapstr = ('+proj=stere +a={3} +b={4} ' +
                       '+lon_0={0} +lat_0={1} +lat_ts={2}').format(
                           mapdef.straight_vertical_longitude_from_pole,
                           mapdef.latitude_of_projection_origin,
                           mapdef.standard_parallel[0],
                           mapdef.semi_major_axis,
@@ -282,14 +324,18 @@
             mapstr = '+proj=merc +a=%s +b=%s +lat_ts=0 +lon_0=%s' % (
                 mapdef.semi_major_axis, mapdef.semi_minor_axis,
                 mapdef.longitude_of_central_meridian)
             mapproj = pyproj.Proj(mapstr)
         elif ifileo.GDTYP == 1:
             def mapproj(x, y, inverse):
                 return (x, y)
+        else:
+            CRS = pyproj.CRS.from_cf(props)
+            mapproj = pyproj.Proj(CRS)
+
         lon, lat = mapproj(lcc_x, lcc_y, inverse=True)
         lone, late = mapproj(lcc_xe.ravel(), lcc_ye.ravel(), inverse=True)
         lone = lone.reshape(*lcc_xe.shape)
         late = late.reshape(*lcc_ye.shape)
 
     if 'x' not in ifileo.variables.keys() and xdim in ifileo.dimensions:
         """
@@ -413,9 +459,10 @@
     try:
         add_time_variables(ifileo)
     except Exception:
         pass
     if ifileo.GDTYP in _gdnames:
         add_lcc_coordinates(ifileo)
     else:
-        raise TypeError('IOAPI is only aware of LCC (GDTYP=2)')
+        raise TypeError(f'PNC IOAPI aware of {_gdnames}; got {ifileo.GDTYP}')
+
     ifileo.Conventions = 'CF-1.6'
```

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/conventions/ioapi/_wrfioapi.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/conventions/ioapi/_wrfioapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         var.latitude_of_projection_origin = ifile.MOAD_CEN_LAT
     elif projname == 'polar_stereographic':
         var.straight_vertical_longitude_from_pole = ifile.STAND_LON
         var.latitude_of_projection_origin = ifile.MOAD_CEN_LAT
         var.standard_parallel = ifile.TRUELAT1
 
     from PseudoNetCDF.coordutil import getproj4_from_cf_var
-    from mpl_toolkits.basemap import pyproj
+    import pyproj
     projstr = getproj4_from_cf_var(var)
     proj = pyproj.Proj(projstr)
     gcx, gcy = proj(ifile.CEN_LON, ifile.CEN_LAT)
     glx = gcx - x0_from_cen
     gly = gcy - y0_from_cen
     var.false_easting = -glx
     var.false_northing = -gly
```

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/coordutil.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/coordutil.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/core/__init__.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/core/__init__.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/core/_dimensions.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/core/_dimensions.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/core/_files.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/core/_files.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/core/_functions.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/core/_functions.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/core/_transforms.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/core/_transforms.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/core/_util.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/core/_util.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/core/_variables.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/core/_variables.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/core/_wrapnc.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/core/_wrapnc.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/derived/met.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/derived/met.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/epafiles/_aqsraw.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/epafiles/_aqsraw.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/geoschemfiles/_bpch.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/geoschemfiles/_bpch.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/geoschemfiles/_bpchmaster.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/geoschemfiles/_bpchmaster.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/geoschemfiles/_cspec.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/geoschemfiles/_cspec.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/geoschemfiles/_gcnc.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/geoschemfiles/_gcnc.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         else:
             missi, = np.where(i.mask)
             missj, = np.where(j.mask)
             outb = i.mask | j.mask
             nout = outb.sum()
             if nout > 0:
                 message = '{} Points out of bounds {:.1%}; {}'.format(
-                    nout, nout/i.size, np.where(outb))
+                    nout, nout / i.size, np.where(outb))
                 if bounds == 'error':
                     raise ValueError(message)
                 else:
                     warn(message)
 
         if clean == 'clip':
             highi, = np.where(easter[:].all(1))
```

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/geoschemfiles/_geos.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/geoschemfiles/_geos.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/geoschemfiles/_newbpch.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/geoschemfiles/_newbpch.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/geoschemfiles/_planelog.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/geoschemfiles/_planelog.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/geoschemfiles/_vertcoord.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/geoschemfiles/_vertcoord.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/icarttfiles/ffi1001.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/icarttfiles/ffi1001.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/morphofiles/_core.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/morphofiles/_core.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/net_balance.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/net_balance.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 class sum_reader(pncf):
     @classmethod
     def isMine(cls, *args, **kwds):
         return False
 
     def __init__(self, sumfile):
-        if type(sumfile) == str:
+        if isinstance(sumfile, str):
             self.sumfile = open(sumfile, 'r')
         else:
             self.sumfile = sumfile
         if not 'Sum'.lower() in self.sumfile.readline().lower():
             raise IOError('Not a sum file')
         self.sumfile.seek(0, 0)
         time, var_names, values = self.parse()
@@ -84,26 +84,28 @@
         if v == 0:
             pass
         elif v > 0:
             products.extend((v, spc))
         elif v < 0:
             reactants.extend((-1 * v, spc))
 
-    return ((" + ".join([tmp for i in reactants if type(i) == str]) + " <-> " +
-             " + ".join([tmp for i in products if type(i) == str])) %
-            tuple(reactants + products))
+    out = (
+        " + ".join([tmp for i in reactants if isinstance(i, str)]) + " <-> "
+        + " + ".join([tmp for i in products if isinstance(i, str)])
+    ) % tuple(reactants + products)
+    return out
 
 
 class ctb_reader(pncf):
     @classmethod
     def isMine(cls, *args, **kwds):
         return False
 
     def __init__(self, file):
-        if type(file) == str:
+        if isinstance(file, str):
             file = open(file)
         lines = file.readlines()
         parameters, daily, peak = self.parse(lines)
 
         self.createDimension('PARAMETERS', len(parameters))
         self.createDimension('PEAK_DAILY', 2)
 
@@ -131,15 +133,15 @@
         return False
 
     def __init__(self, infile):
         self.spc = []
         self.nrxns = []
         self.time = []
 
-        if type(infile) == str:
+        if isinstance(infile, str):
             infile = open(infile)
         lines = infile.readlines()
         self.parse(lines, False)
         self.createDimension('NET_RXN', len(self.nrxns))
         self.createDimension('SPECIES', len(self.spc))
         self.createDimension('TSTEP', len(self.time))
         self.createVariable('NET', 'f', ('TSTEP', 'NET_RXN', 'SPECIES'))
```

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/noaafiles/_arl.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/noaafiles/_arl.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/noaafiles/_cdump.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/noaafiles/_cdump.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/noaafiles/_l100.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/noaafiles/_l100.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/noaafiles/_pdump.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/noaafiles/_pdump.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/noaafiles/_tdump.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/noaafiles/_tdump.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/noaafiles/arltime.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/noaafiles/arltime.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/plotutil/__init__.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/plotutil/__init__.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/plotutil/colors.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/plotutil/colors.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/plotutil/pnc2d.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/plotutil/pnc2d.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/plotutil/pncmap.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/plotutil/pncmap.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/plotutil/pncscatter.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/plotutil/pncscatter.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/plotutil/pncts.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/plotutil/pncts.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/plotutil/vertprofile.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/plotutil/vertprofile.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/pncdump.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/pncdump.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/pnceval.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/pnceval.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/pncgen.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/pncgen.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/pncload.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/pncload.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/pncparse.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/pncparse.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/pncview.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/pncview.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/pncwarn.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/pncwarn.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/racmfiles/boxmodel.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/racmfiles/boxmodel.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/raob/__init__.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/raob/__init__.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/sci_var.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/sci_var.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/test/__init__.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/test/__init__.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/test/__main__.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/test/__main__.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/test/test_camxfiles.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/test/test_camxfiles.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/test/test_cmaqfiles.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/test/test_cmaqfiles.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/test/test_core.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/test/test_core.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/test/test_functions.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/test/test_functions.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/test/test_woudc.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/test/test_woudc.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/__init__.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/__init__.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/cloud_rain/test.cloud_rain` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/cloud_rain/test.cloud_rain`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/height_pressure/test.height_pressure` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/height_pressure/test.height_pressure`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/humidity/test.humidity` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/humidity/test.humidity`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/landuse/test.landuse` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/landuse/test.landuse`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/lateral_boundary/test.lateral_boundary` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/lateral_boundary/test.lateral_boundary`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/point_source/test.point_source` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/point_source/test.point_source`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/temperature/test.temperature` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/temperature/test.temperature`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/uamiv/test.uamiv` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/uamiv/test.uamiv`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/vertical_diffusivity/test.vertical_diffusivity` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/vertical_diffusivity/test.vertical_diffusivity`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/camxfiles/wind/test.wind` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/camxfiles/wind/test.wind`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/ceilometerfiles/VAISALA_CEILOMETER_1_LEVEL2_20.his` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/ceilometerfiles/VAISALA_CEILOMETER_1_LEVEL2_20.his`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/cmaqfiles/griddesc/GRIDDESC` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/cmaqfiles/griddesc/GRIDDESC`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/cmaqfiles/profiles/test.bcon_profile` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/cmaqfiles/profiles/test.bcon_profile`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/cmaqfiles/profiles/test.icon_profile` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/cmaqfiles/profiles/test.icon_profile`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/geoschemfiles/diaginfo.dat` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/geoschemfiles/diaginfo.dat`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/geoschemfiles/test.bpch` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/geoschemfiles/test.bpch`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/geoschemfiles/tracerinfo.dat` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/geoschemfiles/tracerinfo.dat`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/icarttfiles/test.ffi1001` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/icarttfiles/test.ffi1001`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/net_balance/test.mrg_file` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/net_balance/test.mrg_file`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/net_balance/test.net_file` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/net_balance/test.net_file`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/toms/test.txt` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/toms/test.txt`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/testcase/woudcfiles/test_woudc.csv` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/testcase/woudcfiles/test_woudc.csv`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/textfiles/_delimited.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/textfiles/_delimited.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/textfiles/esrl_sonde.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/textfiles/esrl_sonde.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/textfiles/shadoz_sonde.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/textfiles/shadoz_sonde.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/toms/level3.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/toms/level3.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/units.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/units.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
 class converters_dict(defaultdict):
     def __init__(self, dct):
         for k, v in dct.items():
             self[k] = v
 
     def __missing__(self, key):
-        if type(key) == tuple and key[0] == key[1]:
+        if isinstance(key, tuple) and key[0] == key[1]:
             return lambda a: a
 
 
 converter = converters_dict({
     ('s', 'min'): s2min,
     ('min', 'h'): min2h,
     ('s', 'h'): s2h,
```

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/userfuncs.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/userfuncs.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/woudcfiles/_woudc.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/woudcfiles/_woudc.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF/wrffiles/_wrfioapi.py` & `pseudonetcdf-3.4.0/src/PseudoNetCDF/wrffiles/_wrfioapi.py`

 * *Files identical despite different names*

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF.egg-info/PKG-INFO` & `pseudonetcdf-3.4.0/src/PseudoNetCDF.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PseudoNetCDF
-Version: 3.2.3
+Version: 3.4.0
 Summary: Like NetCDF and NCO, but works with NetCDF and other scientific formats.
 Home-page: http://github.com/barronh/pseudonetcdf/
 Author: Barron Henderson
 Author-email: barronh@gmail.com
 Maintainer: Barron Henderson
 Maintainer-email: barronh@gmail.com
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF.egg-info/SOURCES.txt` & `pseudonetcdf-3.4.0/src/PseudoNetCDF.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -42,17 +42,19 @@
 src/PseudoNetCDF/pncview.py
 src/PseudoNetCDF/pncwarn.py
 src/PseudoNetCDF/register.py
 src/PseudoNetCDF/sci_var.py
 src/PseudoNetCDF/units.py
 src/PseudoNetCDF/userfuncs.py
 src/PseudoNetCDF/version.py
+src/PseudoNetCDF/xarray_plugin.py
 src/PseudoNetCDF.egg-info/PKG-INFO
 src/PseudoNetCDF.egg-info/SOURCES.txt
 src/PseudoNetCDF.egg-info/dependency_links.txt
+src/PseudoNetCDF.egg-info/entry_points.txt
 src/PseudoNetCDF.egg-info/requires.txt
 src/PseudoNetCDF.egg-info/top_level.txt
 src/PseudoNetCDF/aermodfiles/__init__.py
 src/PseudoNetCDF/aermodfiles/_aermod_plotfile.py
 src/PseudoNetCDF/camxfiles/ArrayTransforms.py
 src/PseudoNetCDF/camxfiles/FortranFileUtil.py
 src/PseudoNetCDF/camxfiles/Memmaps.py
```

### Comparing `PseudoNetCDF-3.2.3/src/PseudoNetCDF.egg-info/top_level.txt` & `pseudonetcdf-3.4.0/src/PseudoNetCDF.egg-info/top_level.txt`

 * *Files identical despite different names*

