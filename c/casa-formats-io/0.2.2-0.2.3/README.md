# Comparing `tmp/casa-formats-io-0.2.2.tar.gz` & `tmp/casa_formats_io-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casa-formats-io-0.2.2.tar", last modified: Tue Oct 24 11:08:19 2023, max compression
+gzip compressed data, was "casa_formats_io-0.2.3.tar", last modified: Tue Apr 16 13:26:36 2024, max compression
```

## Comparing `casa-formats-io-0.2.2.tar` & `casa_formats_io-0.2.3.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.942307 casa-formats-io-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.914307 casa-formats-io-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.918307 casa-formats-io-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      921 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      568 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      632 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      714 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)    25432 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      316 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2023-10-24 11:08:19.942307 casa-formats-io-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      552 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.918307 casa-formats-io-0.2.2/casa_formats_io/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/_casa_chunking.c
--rw-r--r--   0 runner    (1001) docker     (127)    11092 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_dask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.918307 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/casa_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/dask_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.918307 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/data_managers/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/data_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/data_managers/aipsio.py
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/data_managers/incremental.py
--rw-r--r--   0 runner    (1001) docker     (127)     9596 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/data_managers/standard.py
--rw-r--r--   0 runner    (1001) docker     (127)    11017 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/data_managers/tiled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/record.py
--rw-r--r--   0 runner    (1001) docker     (127)    15905 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.922307 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.914307 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.922307 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/floatarray.image/
--rw-r--r--   0 runner    (1001) docker     (127)    62302 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/floatarray.image/table.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.922307 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/gt32bit.image/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/gt32bit.image/table.f0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.922307 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/lt32bit.image/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/lt32bit.image/table.f0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.930307 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.930307 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/ANTENNA/
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/ANTENNA/table.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10508 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/ANTENNA/table.f0
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/ANTENNA/table.info
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/ANTENNA/table.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.930307 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/CALDEVICE/
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/CALDEVICE/table.dat
--rw-r--r--   0 runner    (1001) docker     (127)     7424 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/CALDEVICE/table.f0
--rw-r--r--   0 runner    (1001) docker     (127)      268 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/CALDEVICE/table.f0i
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/CALDEVICE/table.info
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/CALDEVICE/table.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.930307 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/DATA_DESCRIPTION/
--rw-r--r--   0 runner    (1001) docker     (127)      997 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/DATA_DESCRIPTION/table.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/DATA_DESCRIPTION/table.f0
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/DATA_DESCRIPTION/table.info
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/DATA_DESCRIPTION/table.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.930307 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FEED/
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FEED/table.dat
--rw-r--r--   0 runner    (1001) docker     (127)     9728 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FEED/table.f0
--rw-r--r--   0 runner    (1001) docker     (127)      976 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FEED/table.f0i
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FEED/table.info
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FEED/table.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.930307 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FIELD/
--rw-r--r--   0 runner    (1001) docker     (127)     6365 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FIELD/table.dat
--rw-r--r--   0 runner    (1001) docker     (127)    14876 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FIELD/table.f0
--rw-r--r--   0 runner    (1001) docker     (127)      300 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FIELD/table.f0i
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FIELD/table.info
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FIELD/table.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.934307 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FLAG_CMD/
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FLAG_CMD/table.dat
--rw-r--r--   0 runner    (1001) docker     (127)    31296 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FLAG_CMD/table.f0
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FLAG_CMD/table.info
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FLAG_CMD/table.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.934307 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/HISTORY/
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/HISTORY/table.dat
--rw-r--r--   0 runner    (1001) docker     (127)    25856 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/HISTORY/table.f0
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/HISTORY/table.info
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/HISTORY/table.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.934307 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/OBSERVATION/
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/OBSERVATION/table.dat
--rw-r--r--   0 runner    (1001) docker     (127)     9740 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/OBSERVATION/table.f0
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/OBSERVATION/table.info
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/OBSERVATION/table.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.934307 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POINTING/
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POINTING/table.dat
--rw-r--r--   0 runner    (1001) docker     (127)    33362 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POINTING/table.f0
--rw-r--r--   0 runner    (1001) docker     (127)    33280 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POINTING/table.f1
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POINTING/table.f1i
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POINTING/table.info
--rw-r--r--   0 runner    (1001) docker     (127)      329 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POINTING/table.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.934307 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POLARIZATION/
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POLARIZATION/table.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POLARIZATION/table.f0
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POLARIZATION/table.f0i
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POLARIZATION/table.info
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POLARIZATION/table.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.934307 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/PROCESSOR/
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/PROCESSOR/table.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/PROCESSOR/table.f0
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/PROCESSOR/table.info
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/PROCESSOR/table.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.934307 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SOURCE/
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SOURCE/table.dat
--rw-r--r--   0 runner    (1001) docker     (127)    20224 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SOURCE/table.f0
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SOURCE/table.f0i
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SOURCE/table.info
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SOURCE/table.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.938307 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SPECTRAL_WINDOW/
--rw-r--r--   0 runner    (1001) docker     (127)     6489 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SPECTRAL_WINDOW/table.dat
--rw-r--r--   0 runner    (1001) docker     (127)    24096 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SPECTRAL_WINDOW/table.f0
--rw-r--r--   0 runner    (1001) docker     (127)      272 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SPECTRAL_WINDOW/table.f0i
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SPECTRAL_WINDOW/table.info
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SPECTRAL_WINDOW/table.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.938307 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/STATE/
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/STATE/table.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/STATE/table.f0
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/STATE/table.info
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/STATE/table.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.938307 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSCAL/
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSCAL/table.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSCAL/table.f0
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSCAL/table.f0i
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSCAL/table.info
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSCAL/table.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.942307 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSPOWER/
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSPOWER/table.dat
--rw-r--r--   0 runner    (1001) docker     (127)   611200 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSPOWER/table.f0
--rw-r--r--   0 runner    (1001) docker     (127)   557872 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSPOWER/table.f0i
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSPOWER/table.info
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSPOWER/table.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.942307 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/WEATHER/
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/WEATHER/table.dat
--rw-r--r--   0 runner    (1001) docker     (127)    15232 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/WEATHER/table.f0
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/WEATHER/table.info
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/WEATHER/table.lock
--rw-r--r--   0 runner    (1001) docker     (127)    10667 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.dat
--rw-r--r--   0 runner    (1001) docker     (127)    33362 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f1
--rw-r--r--   0 runner    (1001) docker     (127)    33362 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f10
--rw-r--r--   0 runner    (1001) docker     (127)    33362 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f11
--rw-r--r--   0 runner    (1001) docker     (127)    33362 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f12
--rw-r--r--   0 runner    (1001) docker     (127)    33362 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f13
--rw-r--r--   0 runner    (1001) docker     (127)    66048 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f14
--rw-r--r--   0 runner    (1001) docker     (127)    66048 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f15
--rw-r--r--   0 runner    (1001) docker     (127)    66048 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f16
--rw-r--r--   0 runner    (1001) docker     (127)      647 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f17
--rw-r--r--   0 runner    (1001) docker     (127)  1048576 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f17_TSM1
--rw-r--r--   0 runner    (1001) docker     (127)  1048576 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f17_TSM2
--rw-r--r--   0 runner    (1001) docker     (127)      331 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f18
--rw-r--r--   0 runner    (1001) docker     (127)      276 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f19
--rw-r--r--   0 runner    (1001) docker     (127)  1048560 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f19_TSM0
--rw-r--r--   0 runner    (1001) docker     (127)    33362 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f2
--rw-r--r--   0 runner    (1001) docker     (127)      647 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f20
--rw-r--r--   0 runner    (1001) docker     (127)   131072 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f20_TSM1
--rw-r--r--   0 runner    (1001) docker     (127)   131072 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f20_TSM2
--rw-r--r--   0 runner    (1001) docker     (127)      470 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f21
--rw-r--r--   0 runner    (1001) docker     (127)   524288 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f21_TSM1
--rw-r--r--   0 runner    (1001) docker     (127)      472 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f22
--rw-r--r--   0 runner    (1001) docker     (127)   524288 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f22_TSM1
--rw-r--r--   0 runner    (1001) docker     (127)    33362 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f3
--rw-r--r--   0 runner    (1001) docker     (127)    33362 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f4
--rw-r--r--   0 runner    (1001) docker     (127)    33362 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f5
--rw-r--r--   0 runner    (1001) docker     (127)    16896 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f6
--rw-r--r--   0 runner    (1001) docker     (127)    33362 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f7
--rw-r--r--   0 runner    (1001) docker     (127)    33362 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f8
--rw-r--r--   0 runner    (1001) docker     (127)    33362 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f9
--rw-r--r--   0 runner    (1001) docker     (127)      176 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.info
--rw-r--r--   0 runner    (1001) docker     (127)      409 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.lock
--rw-r--r--   0 runner    (1001) docker     (127)    10624 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/test_casa_low_level_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8304 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/casa_wcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6397 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/glue_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/table_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.942307 casa-formats-io-0.2.2/casa_formats_io/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.942307 casa-formats-io-0.2.2/casa_formats_io/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/tests/data/header_jybeam.hdr
--rw-r--r--   0 runner    (1001) docker     (127)     4945 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/tests/test_casa_dask.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/tests/test_casa_wcs.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/casa_formats_io/tests/test_glue_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-24 11:08:19.000000 casa-formats-io-0.2.2/casa_formats_io/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.918307 casa-formats-io-0.2.2/casa_formats_io.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2023-10-24 11:08:19.000000 casa-formats-io-0.2.2/casa_formats_io.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9776 2023-10-24 11:08:19.000000 casa-formats-io-0.2.2/casa_formats_io.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-24 11:08:19.000000 casa-formats-io-0.2.2/casa_formats_io.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-10-24 11:08:19.000000 casa-formats-io-0.2.2/casa_formats_io.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-24 11:08:19.000000 casa-formats-io-0.2.2/casa_formats_io.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-10-24 11:08:19.000000 casa-formats-io-0.2.2/casa_formats_io.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-24 11:08:19.000000 casa-formats-io-0.2.2/casa_formats_io.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:08:19.942307 casa-formats-io-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      795 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2023-10-24 11:08:19.946307 casa-formats-io-0.2.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      479 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2023-10-24 11:07:58.000000 casa-formats-io-0.2.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.658246 casa_formats_io-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.622246 casa_formats_io-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.626246 casa_formats_io-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    25432 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-16 13:26:36.658246 casa_formats_io-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.626246 casa_formats_io-0.2.3/casa_formats_io/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/_casa_chunking.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11092 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_dask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.630246 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/casa_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/dask_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.630246 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/data_managers/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/data_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/data_managers/aipsio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/data_managers/incremental.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9596 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/data_managers/standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11017 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/data_managers/tiled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15905 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.630246 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.622246 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.630246 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/floatarray.image/
+-rw-r--r--   0 runner    (1001) docker     (127)    62302 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/floatarray.image/table.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.630246 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/gt32bit.image/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/gt32bit.image/table.f0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.630246 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/lt32bit.image/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/lt32bit.image/table.f0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.642246 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.642246 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/ANTENNA/
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/ANTENNA/table.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10508 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/ANTENNA/table.f0
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/ANTENNA/table.info
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/ANTENNA/table.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.646246 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/CALDEVICE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/CALDEVICE/table.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     7424 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/CALDEVICE/table.f0
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/CALDEVICE/table.f0i
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/CALDEVICE/table.info
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/CALDEVICE/table.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.646246 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/DATA_DESCRIPTION/
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/DATA_DESCRIPTION/table.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/DATA_DESCRIPTION/table.f0
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/DATA_DESCRIPTION/table.info
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/DATA_DESCRIPTION/table.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.646246 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FEED/
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FEED/table.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FEED/table.f0
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FEED/table.f0i
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FEED/table.info
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FEED/table.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.646246 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FIELD/
+-rw-r--r--   0 runner    (1001) docker     (127)     6365 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FIELD/table.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    14876 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FIELD/table.f0
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FIELD/table.f0i
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FIELD/table.info
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FIELD/table.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.646246 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FLAG_CMD/
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FLAG_CMD/table.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    31296 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FLAG_CMD/table.f0
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FLAG_CMD/table.info
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FLAG_CMD/table.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.646246 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/HISTORY/
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/HISTORY/table.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    25856 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/HISTORY/table.f0
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/HISTORY/table.info
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/HISTORY/table.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.650246 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/OBSERVATION/
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/OBSERVATION/table.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     9740 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/OBSERVATION/table.f0
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/OBSERVATION/table.info
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/OBSERVATION/table.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.650246 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POINTING/
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POINTING/table.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    33362 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POINTING/table.f0
+-rw-r--r--   0 runner    (1001) docker     (127)    33280 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POINTING/table.f1
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POINTING/table.f1i
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POINTING/table.info
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POINTING/table.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.650246 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POLARIZATION/
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POLARIZATION/table.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POLARIZATION/table.f0
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POLARIZATION/table.f0i
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POLARIZATION/table.info
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POLARIZATION/table.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.650246 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/PROCESSOR/
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/PROCESSOR/table.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/PROCESSOR/table.f0
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/PROCESSOR/table.info
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/PROCESSOR/table.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.650246 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SOURCE/
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SOURCE/table.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    20224 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SOURCE/table.f0
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SOURCE/table.f0i
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SOURCE/table.info
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SOURCE/table.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.654246 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SPECTRAL_WINDOW/
+-rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SPECTRAL_WINDOW/table.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    24096 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SPECTRAL_WINDOW/table.f0
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SPECTRAL_WINDOW/table.f0i
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SPECTRAL_WINDOW/table.info
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SPECTRAL_WINDOW/table.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.654246 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/STATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/STATE/table.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/STATE/table.f0
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/STATE/table.info
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/STATE/table.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.654246 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSCAL/
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSCAL/table.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSCAL/table.f0
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSCAL/table.f0i
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSCAL/table.info
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSCAL/table.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.658246 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSPOWER/
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSPOWER/table.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   611200 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSPOWER/table.f0
+-rw-r--r--   0 runner    (1001) docker     (127)   557872 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSPOWER/table.f0i
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSPOWER/table.info
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSPOWER/table.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.658246 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/WEATHER/
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/WEATHER/table.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    15232 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/WEATHER/table.f0
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/WEATHER/table.info
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/WEATHER/table.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    10667 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    33362 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f1
+-rw-r--r--   0 runner    (1001) docker     (127)    33362 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f10
+-rw-r--r--   0 runner    (1001) docker     (127)    33362 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f11
+-rw-r--r--   0 runner    (1001) docker     (127)    33362 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f12
+-rw-r--r--   0 runner    (1001) docker     (127)    33362 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f13
+-rw-r--r--   0 runner    (1001) docker     (127)    66048 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f14
+-rw-r--r--   0 runner    (1001) docker     (127)    66048 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f15
+-rw-r--r--   0 runner    (1001) docker     (127)    66048 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f16
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f17
+-rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f17_TSM1
+-rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f17_TSM2
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f18
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f19
+-rw-r--r--   0 runner    (1001) docker     (127)  1048560 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f19_TSM0
+-rw-r--r--   0 runner    (1001) docker     (127)    33362 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f2
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f20
+-rw-r--r--   0 runner    (1001) docker     (127)   131072 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f20_TSM1
+-rw-r--r--   0 runner    (1001) docker     (127)   131072 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f20_TSM2
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f21
+-rw-r--r--   0 runner    (1001) docker     (127)   524288 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f21_TSM1
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f22
+-rw-r--r--   0 runner    (1001) docker     (127)   524288 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f22_TSM1
+-rw-r--r--   0 runner    (1001) docker     (127)    33362 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f3
+-rw-r--r--   0 runner    (1001) docker     (127)    33362 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f4
+-rw-r--r--   0 runner    (1001) docker     (127)    33362 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f5
+-rw-r--r--   0 runner    (1001) docker     (127)    16896 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f6
+-rw-r--r--   0 runner    (1001) docker     (127)    33362 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f7
+-rw-r--r--   0 runner    (1001) docker     (127)    33362 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f8
+-rw-r--r--   0 runner    (1001) docker     (127)    33362 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f9
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.info
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/test_casa_low_level_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8304 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/casa_wcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/glue_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/table_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.658246 casa_formats_io-0.2.3/casa_formats_io/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.658246 casa_formats_io-0.2.3/casa_formats_io/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/tests/data/header_jybeam.hdr
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/tests/test_casa_dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/tests/test_casa_wcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/casa_formats_io/tests/test_glue_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-16 13:26:36.000000 casa_formats_io-0.2.3/casa_formats_io/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.658246 casa_formats_io-0.2.3/casa_formats_io.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-16 13:26:36.000000 casa_formats_io-0.2.3/casa_formats_io.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9776 2024-04-16 13:26:36.000000 casa_formats_io-0.2.3/casa_formats_io.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:26:36.000000 casa_formats_io-0.2.3/casa_formats_io.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-16 13:26:36.000000 casa_formats_io-0.2.3/casa_formats_io.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:26:36.000000 casa_formats_io-0.2.3/casa_formats_io.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-16 13:26:36.000000 casa_formats_io-0.2.3/casa_formats_io.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-16 13:26:36.000000 casa_formats_io-0.2.3/casa_formats_io.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:26:36.658246 casa_formats_io-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-16 13:26:36.662246 casa_formats_io-0.2.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      479 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-16 13:26:23.000000 casa_formats_io-0.2.3/tox.ini
```

### Comparing `casa-formats-io-0.2.2/.github/workflows/main.yml` & `casa_formats_io-0.2.3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/.github/workflows/publish.yml` & `casa_formats_io-0.2.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/.gitignore` & `casa_formats_io-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/CHANGES.rst` & `casa_formats_io-0.2.3/CHANGES.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+0.2.3 (2024-04-16)
+------------------
+
+- Fixed compatibility with Numpy 2.0. [#61]
+
 0.2.2 (2023-10-24)
 ------------------
 
 - Fixed compatibility of wheels with PyPy. [#59]
 
 0.2.1 (2022-09-29)
 ------------------
```

### Comparing `casa-formats-io-0.2.2/LICENSE` & `casa_formats_io-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/PKG-INFO` & `casa_formats_io-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casa-formats-io
-Version: 0.2.2
+Version: 0.2.3
 Summary: Dask-based reader for CASA data
 Home-page: http://casa-formats-io.readthedocs.org
 Author: Thomas Robitaille, Adam Ginsburg, and Eric Koch
 Author-email: thomas.robitaille@gmail.com
 License: LGPLv2
 Requires-Python: >=3.8
 License-File: LICENSE
```

### Comparing `casa-formats-io-0.2.2/README.rst` & `casa_formats_io-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/_casa_chunking.c` & `casa_formats_io-0.2.3/casa_formats_io/_casa_chunking.c`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_dask.py` & `casa_formats_io-0.2.3/casa_formats_io/casa_dask.py`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/casa_functions.py` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/casa_functions.py`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/core.py` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/core.py`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/dask_mixin.py` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/dask_mixin.py`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/data_managers/aipsio.py` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/data_managers/aipsio.py`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/data_managers/incremental.py` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/data_managers/incremental.py`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/data_managers/standard.py` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/data_managers/standard.py`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/data_managers/tiled.py` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/data_managers/tiled.py`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/record.py` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/record.py`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/table.py` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/table.py`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/floatarray.image/table.dat` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/floatarray.image/table.dat`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/ANTENNA/table.dat` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/ANTENNA/table.dat`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/ANTENNA/table.f0` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/ANTENNA/table.f0`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/CALDEVICE/table.dat` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/CALDEVICE/table.dat`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/CALDEVICE/table.f0` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/CALDEVICE/table.f0`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/DATA_DESCRIPTION/table.dat` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/DATA_DESCRIPTION/table.dat`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/DATA_DESCRIPTION/table.f0` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/DATA_DESCRIPTION/table.f0`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FEED/table.dat` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FEED/table.dat`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FEED/table.f0` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FEED/table.f0`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FEED/table.f0i` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FEED/table.f0i`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FIELD/table.dat` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FIELD/table.dat`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FIELD/table.f0` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FIELD/table.f0`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FLAG_CMD/table.dat` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FLAG_CMD/table.dat`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FLAG_CMD/table.f0` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/FLAG_CMD/table.f0`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/HISTORY/table.dat` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/HISTORY/table.dat`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/HISTORY/table.f0` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/HISTORY/table.f0`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/OBSERVATION/table.dat` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/OBSERVATION/table.dat`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/OBSERVATION/table.f0` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/OBSERVATION/table.f0`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POINTING/table.dat` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POINTING/table.dat`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POINTING/table.f0` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POINTING/table.f0`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POINTING/table.f1` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POINTING/table.f1`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POLARIZATION/table.dat` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POLARIZATION/table.dat`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POLARIZATION/table.f0` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/POLARIZATION/table.f0`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/PROCESSOR/table.dat` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/PROCESSOR/table.dat`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/PROCESSOR/table.f0` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/PROCESSOR/table.f0`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SOURCE/table.dat` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SOURCE/table.dat`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SOURCE/table.f0` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SOURCE/table.f0`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SPECTRAL_WINDOW/table.dat` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SPECTRAL_WINDOW/table.dat`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SPECTRAL_WINDOW/table.f0` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SPECTRAL_WINDOW/table.f0`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/STATE/table.dat` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/STATE/table.dat`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/STATE/table.f0` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/STATE/table.f0`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSCAL/table.dat` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSCAL/table.dat`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSCAL/table.f0` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSCAL/table.f0`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSPOWER/table.dat` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSPOWER/table.dat`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSPOWER/table.f0` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSPOWER/table.f0`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSPOWER/table.f0i` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/SYSPOWER/table.f0i`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/WEATHER/table.dat` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/WEATHER/table.dat`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/WEATHER/table.f0` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/WEATHER/table.f0`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.dat` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.dat`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f1` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f1`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f10` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f10`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f11` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f11`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f12` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f12`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f13` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f13`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f14` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f14`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f15` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f15`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f16` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f16`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f17` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f17`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f17_TSM1` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f17_TSM1`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f17_TSM2` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f17_TSM2`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f19_TSM0` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f19_TSM0`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f2` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f2`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f20` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f20`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f3` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f3`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f4` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f4`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f5` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f5`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f6` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f6`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f7` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f7`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f8` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f8`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f9` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/data/simple.ms/table.f9`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_low_level_io/tests/test_casa_low_level_io.py` & `casa_formats_io-0.2.3/casa_formats_io/casa_low_level_io/tests/test_casa_low_level_io.py`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/casa_wcs.py` & `casa_formats_io-0.2.3/casa_formats_io/casa_wcs.py`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/glue_factory.py` & `casa_formats_io-0.2.3/casa_formats_io/glue_factory.py`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/table_reader.py` & `casa_formats_io-0.2.3/casa_formats_io/table_reader.py`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/tests/data/header_jybeam.hdr` & `casa_formats_io-0.2.3/casa_formats_io/tests/data/header_jybeam.hdr`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/tests/test_casa_dask.py` & `casa_formats_io-0.2.3/casa_formats_io/tests/test_casa_dask.py`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/tests/test_casa_wcs.py` & `casa_formats_io-0.2.3/casa_formats_io/tests/test_casa_wcs.py`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io/tests/test_glue_factory.py` & `casa_formats_io-0.2.3/casa_formats_io/tests/test_glue_factory.py`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/casa_formats_io.egg-info/PKG-INFO` & `casa_formats_io-0.2.3/casa_formats_io.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casa-formats-io
-Version: 0.2.2
+Version: 0.2.3
 Summary: Dask-based reader for CASA data
 Home-page: http://casa-formats-io.readthedocs.org
 Author: Thomas Robitaille, Adam Ginsburg, and Eric Koch
 Author-email: thomas.robitaille@gmail.com
 License: LGPLv2
 Requires-Python: >=3.8
 License-File: LICENSE
```

### Comparing `casa-formats-io-0.2.2/casa_formats_io.egg-info/SOURCES.txt` & `casa_formats_io-0.2.3/casa_formats_io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/docs/Makefile` & `casa_formats_io-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/docs/conf.py` & `casa_formats_io-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/docs/index.rst` & `casa_formats_io-0.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/docs/make.bat` & `casa_formats_io-0.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/setup.cfg` & `casa_formats_io-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `casa-formats-io-0.2.2/tox.ini` & `casa_formats_io-0.2.3/tox.ini`

 * *Files identical despite different names*

