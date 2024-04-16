# Comparing `tmp/ailist-2.1.2.tar.gz` & `tmp/ailist-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ailist-2.1.2.tar", max compression
+gzip compressed data, was "ailist-2.1.3.tar", max compression
```

## Comparing `ailist-2.1.2.tar` & `ailist-2.1.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rwxr-xr-x   0        0        0    17895 2019-08-12 18:05:36.000000 ailist-2.1.2/LICENSE.md
--rwxr-xr-x   0        0        0     4923 2021-08-28 14:14:30.000000 ailist-2.1.2/README.md
--rw-r--r--   0        0        0   416960 2023-05-16 20:29:10.000000 ailist-2.1.2/ailist/AIList_core.cpython-310-darwin.so
--rw-r--r--   0        0        0   462464 2024-04-16 03:09:00.301263 ailist-2.1.2/ailist/AIList_core.cpython-311-darwin.so
--rwxr-xr-x   0        0        0    15363 2023-11-17 02:41:12.095548 ailist-2.1.2/ailist/AIList_core.pxd
--rwxr-xr-x   0        0        0    39564 2023-11-17 02:49:17.040909 ailist-2.1.2/ailist/AIList_core.pyx
--rw-r--r--   0        0        0    34745 2023-01-20 20:29:03.224385 ailist-2.1.2/ailist/IntervalArray_core.py
--rw-r--r--   0        0        0    83496 2023-05-16 20:29:10.000000 ailist-2.1.2/ailist/Interval_core.cpython-310-darwin.so
--rw-r--r--   0        0        0   100840 2024-04-16 03:09:00.300197 ailist-2.1.2/ailist/Interval_core.cpython-311-darwin.so
--rwxr-xr-x   0        0        0      721 2023-01-19 03:35:55.179175 ailist-2.1.2/ailist/Interval_core.pxd
--rwxr-xr-x   0        0        0     1452 2023-04-12 15:43:30.386933 ailist-2.1.2/ailist/Interval_core.pyx
--rw-r--r--   0        0        0   650600 2023-05-16 20:29:10.000000 ailist-2.1.2/ailist/LabeledIntervalArray_core.cpython-310-darwin.so
--rw-r--r--   0        0        0   712976 2024-04-16 03:09:00.302446 ailist-2.1.2/ailist/LabeledIntervalArray_core.cpython-311-darwin.so
--rw-r--r--   0        0        0    28088 2023-04-24 14:57:56.149081 ailist-2.1.2/ailist/LabeledIntervalArray_core.pxd
--rw-r--r--   0        0        0    79246 2023-11-17 01:43:22.248023 ailist-2.1.2/ailist/LabeledIntervalArray_core.pyx
--rwxr-xr-x   0        0        0      536 2024-04-16 03:05:44.921277 ailist-2.1.2/ailist/__init__.py
--rw-r--r--   0        0        0    59928 2023-05-16 20:29:10.000000 ailist-2.1.2/ailist/array_query_core.cpython-310-darwin.so
--rw-r--r--   0        0        0    61656 2024-04-16 03:09:00.303122 ailist-2.1.2/ailist/array_query_core.cpython-311-darwin.so
--rwxr-xr-x   0        0        0     1086 2022-05-02 21:15:59.000000 ailist-2.1.2/ailist/array_query_core.pxd
--rwxr-xr-x   0        0        0     1304 2023-04-12 15:43:58.852105 ailist-2.1.2/ailist/array_query_core.pyx
--rw-r--r--   0        0        0     2228 2023-04-13 02:36:16.801973 ailist-2.1.2/ailist/src/ailist/ailist_add.c
--rw-r--r--   0        0        0     2157 2023-08-03 19:18:26.303892 ailist-2.1.2/ailist/src/ailist/ailist_closest.c
--rw-r--r--   0        0        0     7229 2022-09-15 17:32:49.000000 ailist-2.1.2/ailist/src/ailist/ailist_construct.c
--rw-r--r--   0        0        0     5233 2023-02-10 20:43:05.058096 ailist-2.1.2/ailist/src/ailist/ailist_coverage.c
--rw-r--r--   0        0        0     1004 2021-02-01 19:00:33.000000 ailist-2.1.2/ailist/src/ailist/ailist_extract.c
--rw-r--r--   0        0        0     1582 2022-06-06 03:22:03.000000 ailist-2.1.2/ailist/src/ailist/ailist_filter.c
--rw-r--r--   0        0        0     2011 2022-06-16 14:20:03.000000 ailist-2.1.2/ailist/src/ailist/ailist_get_id.c
--rw-r--r--   0        0        0     3186 2023-11-17 17:21:44.709714 ailist-2.1.2/ailist/src/ailist/ailist_iter.c
--rw-r--r--   0        0        0     2009 2023-02-21 20:12:11.742021 ailist-2.1.2/ailist/src/ailist/ailist_merge.c
--rw-r--r--   0        0        0     2758 2022-09-07 00:38:08.000000 ailist-2.1.2/ailist/src/ailist/ailist_nhits.c
--rw-r--r--   0        0        0     5077 2023-05-04 15:00:47.219735 ailist-2.1.2/ailist/src/ailist/ailist_ops.c
--rw-r--r--   0        0        0    16745 2023-05-04 15:30:28.093848 ailist-2.1.2/ailist/src/ailist/ailist_query.c
--rw-r--r--   0        0        0     1066 2022-07-26 17:40:19.000000 ailist-2.1.2/ailist/src/ailist/ailist_simulate.c
--rw-r--r--   0        0        0     3612 2020-10-19 17:27:23.000000 ailist-2.1.2/ailist/src/ailist/ailist_wps.c
--rwxr-xr-x   0        0        0     2748 2024-03-18 20:54:27.075576 ailist-2.1.2/ailist/src/ailist/augmented_interval_list.c
--rwxr-xr-x   0        0        0    11320 2023-08-03 19:27:55.876838 ailist-2.1.2/ailist/src/ailist/augmented_interval_list.h
--rw-r--r--   0        0        0      804 2021-02-03 17:09:02.000000 ailist-2.1.2/ailist/src/ailist/interval.c
--rwxr-xr-x   0        0        0     1088 2021-02-03 17:08:42.000000 ailist-2.1.2/ailist/src/ailist/interval.h
--rwxr-xr-x   0        0        0     1714 2022-02-12 16:20:01.000000 ailist-2.1.2/ailist/src/ailist/overlap_index.c
--rwxr-xr-x   0        0        0      981 2023-01-26 15:09:47.831548 ailist-2.1.2/ailist/src/array_query/array_query_utilities.c
--rwxr-xr-x   0        0        0     2105 2023-01-26 15:08:56.094844 ailist-2.1.2/ailist/src/array_query/array_query_utilities.h
--rw-r--r--   0        0        0    21510 2021-04-26 19:06:11.000000 ailist-2.1.2/ailist/src/labeled_aiarray/khash.h
--rw-r--r--   0        0        0     2872 2023-01-25 18:17:24.561022 ailist-2.1.2/ailist/src/labeled_aiarray/kvec.h
--rw-r--r--   0        0        0     4759 2023-05-04 15:01:55.664279 ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_add.c
--rw-r--r--   0        0        0     1207 2023-05-01 20:57:05.670200 ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_construct.c
--rw-r--r--   0        0        0     3846 2023-02-10 20:40:34.313629 ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_coverage.c
--rw-r--r--   0        0        0     1293 2022-05-11 19:58:25.000000 ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_extract.c
--rw-r--r--   0        0        0     2333 2023-02-01 22:05:01.741865 ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_filter.c
--rw-r--r--   0        0        0     6944 2023-05-02 02:19:37.520386 ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_get.c
--rw-r--r--   0        0        0     6160 2024-03-07 20:14:40.729847 ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_index.c
--rw-r--r--   0        0        0     4160 2023-02-26 21:23:15.841726 ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_iter.c
--rw-r--r--   0        0        0     9856 2023-05-02 02:17:46.112410 ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_match.c
--rw-r--r--   0        0        0      937 2022-05-11 16:24:30.000000 ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_merge.c
--rw-r--r--   0        0        0     7199 2023-02-10 20:45:56.368299 ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_nhits.c
--rw-r--r--   0        0        0     2424 2023-05-04 14:53:06.390402 ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_ops.c
--rw-r--r--   0        0        0     1956 2023-02-26 21:24:15.672922 ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_percent.c
--rw-r--r--   0        0        0     5350 2023-01-26 15:10:01.828428 ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_query_array.c
--rw-r--r--   0        0        0     4338 2023-05-02 02:17:29.334654 ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_query_index.c
--rw-r--r--   0        0        0     6240 2023-01-25 16:50:52.952858 ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_query_single.c
--rw-r--r--   0        0        0     1013 2022-07-26 19:33:03.000000 ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_simulate.c
--rw-r--r--   0        0        0     2210 2023-11-17 01:21:10.282550 ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_sort.c
--rw-r--r--   0        0        0     1299 2022-05-02 16:48:19.000000 ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_wps.c
--rw-r--r--   0        0        0     5281 2022-09-14 17:13:56.000000 ailist-2.1.2/ailist/src/labeled_aiarray/labeled_augmented_array.c
--rwxr-xr-x   0        0        0    20346 2023-06-19 16:37:48.241380 ailist-2.1.2/ailist/src/labeled_aiarray/labeled_augmented_array.h
--rwxr-xr-x   0        0        0     2298 2023-05-02 02:18:32.335127 ailist-2.1.2/ailist/src/labeled_aiarray/overlap_label_index.c
--rwxr-xr-x   0        0        0     3103 2021-02-20 22:03:14.000000 ailist-2.1.2/ailist/src/utilities/utilities.h
--rw-r--r--   0        0        0     3447 2023-04-12 15:10:52.847444 ailist-2.1.2/build.py
--rw-r--r--   0        0        0     2109 2024-04-16 03:06:21.640155 ailist-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     6538 1970-01-01 00:00:00.000000 ailist-2.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0    17895 2019-08-12 18:05:36.000000 ailist-2.1.3/LICENSE.md
+-rwxr-xr-x   0        0        0     4923 2021-08-28 14:14:30.000000 ailist-2.1.3/README.md
+-rw-r--r--   0        0        0   416960 2023-05-16 20:29:10.000000 ailist-2.1.3/ailist/AIList_core.cpython-310-darwin.so
+-rw-r--r--   0        0        0   462464 2024-04-16 03:12:08.516647 ailist-2.1.3/ailist/AIList_core.cpython-311-darwin.so
+-rwxr-xr-x   0        0        0    15363 2023-11-17 02:41:12.095548 ailist-2.1.3/ailist/AIList_core.pxd
+-rwxr-xr-x   0        0        0    39564 2023-11-17 02:49:17.040909 ailist-2.1.3/ailist/AIList_core.pyx
+-rw-r--r--   0        0        0    34745 2023-01-20 20:29:03.224385 ailist-2.1.3/ailist/IntervalArray_core.py
+-rw-r--r--   0        0        0    83496 2023-05-16 20:29:10.000000 ailist-2.1.3/ailist/Interval_core.cpython-310-darwin.so
+-rw-r--r--   0        0        0   100840 2024-04-16 03:12:08.516003 ailist-2.1.3/ailist/Interval_core.cpython-311-darwin.so
+-rwxr-xr-x   0        0        0      721 2023-01-19 03:35:55.179175 ailist-2.1.3/ailist/Interval_core.pxd
+-rwxr-xr-x   0        0        0     1452 2023-04-12 15:43:30.386933 ailist-2.1.3/ailist/Interval_core.pyx
+-rw-r--r--   0        0        0   650600 2023-05-16 20:29:10.000000 ailist-2.1.3/ailist/LabeledIntervalArray_core.cpython-310-darwin.so
+-rw-r--r--   0        0        0   712976 2024-04-16 03:12:08.517806 ailist-2.1.3/ailist/LabeledIntervalArray_core.cpython-311-darwin.so
+-rw-r--r--   0        0        0    28088 2023-04-24 14:57:56.149081 ailist-2.1.3/ailist/LabeledIntervalArray_core.pxd
+-rw-r--r--   0        0        0    79246 2023-11-17 01:43:22.248023 ailist-2.1.3/ailist/LabeledIntervalArray_core.pyx
+-rwxr-xr-x   0        0        0      536 2024-04-16 03:05:44.921277 ailist-2.1.3/ailist/__init__.py
+-rw-r--r--   0        0        0    59928 2023-05-16 20:29:10.000000 ailist-2.1.3/ailist/array_query_core.cpython-310-darwin.so
+-rw-r--r--   0        0        0    61656 2024-04-16 03:12:08.518203 ailist-2.1.3/ailist/array_query_core.cpython-311-darwin.so
+-rwxr-xr-x   0        0        0     1086 2022-05-02 21:15:59.000000 ailist-2.1.3/ailist/array_query_core.pxd
+-rwxr-xr-x   0        0        0     1304 2023-04-12 15:43:58.852105 ailist-2.1.3/ailist/array_query_core.pyx
+-rw-r--r--   0        0        0     2228 2023-04-13 02:36:16.801973 ailist-2.1.3/ailist/src/ailist/ailist_add.c
+-rw-r--r--   0        0        0     2157 2023-08-03 19:18:26.303892 ailist-2.1.3/ailist/src/ailist/ailist_closest.c
+-rw-r--r--   0        0        0     7229 2022-09-15 17:32:49.000000 ailist-2.1.3/ailist/src/ailist/ailist_construct.c
+-rw-r--r--   0        0        0     5233 2023-02-10 20:43:05.058096 ailist-2.1.3/ailist/src/ailist/ailist_coverage.c
+-rw-r--r--   0        0        0     1004 2021-02-01 19:00:33.000000 ailist-2.1.3/ailist/src/ailist/ailist_extract.c
+-rw-r--r--   0        0        0     1582 2022-06-06 03:22:03.000000 ailist-2.1.3/ailist/src/ailist/ailist_filter.c
+-rw-r--r--   0        0        0     2011 2022-06-16 14:20:03.000000 ailist-2.1.3/ailist/src/ailist/ailist_get_id.c
+-rw-r--r--   0        0        0     3186 2023-11-17 17:21:44.709714 ailist-2.1.3/ailist/src/ailist/ailist_iter.c
+-rw-r--r--   0        0        0     2009 2023-02-21 20:12:11.742021 ailist-2.1.3/ailist/src/ailist/ailist_merge.c
+-rw-r--r--   0        0        0     2758 2022-09-07 00:38:08.000000 ailist-2.1.3/ailist/src/ailist/ailist_nhits.c
+-rw-r--r--   0        0        0     5077 2023-05-04 15:00:47.219735 ailist-2.1.3/ailist/src/ailist/ailist_ops.c
+-rw-r--r--   0        0        0    16745 2023-05-04 15:30:28.093848 ailist-2.1.3/ailist/src/ailist/ailist_query.c
+-rw-r--r--   0        0        0     1066 2022-07-26 17:40:19.000000 ailist-2.1.3/ailist/src/ailist/ailist_simulate.c
+-rw-r--r--   0        0        0     3612 2020-10-19 17:27:23.000000 ailist-2.1.3/ailist/src/ailist/ailist_wps.c
+-rwxr-xr-x   0        0        0     2748 2024-03-18 20:54:27.075576 ailist-2.1.3/ailist/src/ailist/augmented_interval_list.c
+-rwxr-xr-x   0        0        0    11320 2023-08-03 19:27:55.876838 ailist-2.1.3/ailist/src/ailist/augmented_interval_list.h
+-rw-r--r--   0        0        0      804 2021-02-03 17:09:02.000000 ailist-2.1.3/ailist/src/ailist/interval.c
+-rwxr-xr-x   0        0        0     1088 2021-02-03 17:08:42.000000 ailist-2.1.3/ailist/src/ailist/interval.h
+-rwxr-xr-x   0        0        0     1714 2022-02-12 16:20:01.000000 ailist-2.1.3/ailist/src/ailist/overlap_index.c
+-rwxr-xr-x   0        0        0      981 2023-01-26 15:09:47.831548 ailist-2.1.3/ailist/src/array_query/array_query_utilities.c
+-rwxr-xr-x   0        0        0     2105 2023-01-26 15:08:56.094844 ailist-2.1.3/ailist/src/array_query/array_query_utilities.h
+-rw-r--r--   0        0        0    21510 2021-04-26 19:06:11.000000 ailist-2.1.3/ailist/src/labeled_aiarray/khash.h
+-rw-r--r--   0        0        0     2872 2023-01-25 18:17:24.561022 ailist-2.1.3/ailist/src/labeled_aiarray/kvec.h
+-rw-r--r--   0        0        0     4759 2023-05-04 15:01:55.664279 ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_add.c
+-rw-r--r--   0        0        0     1207 2023-05-01 20:57:05.670200 ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_construct.c
+-rw-r--r--   0        0        0     3846 2023-02-10 20:40:34.313629 ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_coverage.c
+-rw-r--r--   0        0        0     1293 2022-05-11 19:58:25.000000 ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_extract.c
+-rw-r--r--   0        0        0     2333 2023-02-01 22:05:01.741865 ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_filter.c
+-rw-r--r--   0        0        0     6944 2023-05-02 02:19:37.520386 ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_get.c
+-rw-r--r--   0        0        0     6160 2024-03-07 20:14:40.729847 ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_index.c
+-rw-r--r--   0        0        0     4160 2023-02-26 21:23:15.841726 ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_iter.c
+-rw-r--r--   0        0        0     9856 2023-05-02 02:17:46.112410 ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_match.c
+-rw-r--r--   0        0        0      937 2022-05-11 16:24:30.000000 ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_merge.c
+-rw-r--r--   0        0        0     7199 2023-02-10 20:45:56.368299 ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_nhits.c
+-rw-r--r--   0        0        0     2424 2023-05-04 14:53:06.390402 ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_ops.c
+-rw-r--r--   0        0        0     1956 2023-02-26 21:24:15.672922 ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_percent.c
+-rw-r--r--   0        0        0     5350 2023-01-26 15:10:01.828428 ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_query_array.c
+-rw-r--r--   0        0        0     4338 2023-05-02 02:17:29.334654 ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_query_index.c
+-rw-r--r--   0        0        0     6240 2023-01-25 16:50:52.952858 ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_query_single.c
+-rw-r--r--   0        0        0     1013 2022-07-26 19:33:03.000000 ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_simulate.c
+-rw-r--r--   0        0        0     2210 2023-11-17 01:21:10.282550 ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_sort.c
+-rw-r--r--   0        0        0     1299 2022-05-02 16:48:19.000000 ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_wps.c
+-rw-r--r--   0        0        0     5281 2022-09-14 17:13:56.000000 ailist-2.1.3/ailist/src/labeled_aiarray/labeled_augmented_array.c
+-rwxr-xr-x   0        0        0    20346 2023-06-19 16:37:48.241380 ailist-2.1.3/ailist/src/labeled_aiarray/labeled_augmented_array.h
+-rwxr-xr-x   0        0        0     2298 2023-05-02 02:18:32.335127 ailist-2.1.3/ailist/src/labeled_aiarray/overlap_label_index.c
+-rwxr-xr-x   0        0        0     3103 2021-02-20 22:03:14.000000 ailist-2.1.3/ailist/src/utilities/utilities.h
+-rw-r--r--   0        0        0     3447 2023-04-12 15:10:52.847444 ailist-2.1.3/build.py
+-rw-r--r--   0        0        0     2105 2024-04-16 11:52:11.193301 ailist-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6535 1970-01-01 00:00:00.000000 ailist-2.1.3/PKG-INFO
```

### Comparing `ailist-2.1.2/LICENSE.md` & `ailist-2.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/README.md` & `ailist-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/AIList_core.cpython-310-darwin.so` & `ailist-2.1.3/ailist/AIList_core.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/AIList_core.cpython-311-darwin.so` & `ailist-2.1.3/ailist/AIList_core.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/AIList_core.pxd` & `ailist-2.1.3/ailist/AIList_core.pxd`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/AIList_core.pyx` & `ailist-2.1.3/ailist/AIList_core.pyx`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/IntervalArray_core.py` & `ailist-2.1.3/ailist/IntervalArray_core.py`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/Interval_core.cpython-310-darwin.so` & `ailist-2.1.3/ailist/Interval_core.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/Interval_core.cpython-311-darwin.so` & `ailist-2.1.3/ailist/Interval_core.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/Interval_core.pxd` & `ailist-2.1.3/ailist/Interval_core.pxd`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/Interval_core.pyx` & `ailist-2.1.3/ailist/Interval_core.pyx`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/LabeledIntervalArray_core.cpython-310-darwin.so` & `ailist-2.1.3/ailist/LabeledIntervalArray_core.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/LabeledIntervalArray_core.cpython-311-darwin.so` & `ailist-2.1.3/ailist/LabeledIntervalArray_core.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/LabeledIntervalArray_core.pxd` & `ailist-2.1.3/ailist/LabeledIntervalArray_core.pxd`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/LabeledIntervalArray_core.pyx` & `ailist-2.1.3/ailist/LabeledIntervalArray_core.pyx`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/__init__.py` & `ailist-2.1.3/ailist/__init__.py`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/array_query_core.cpython-310-darwin.so` & `ailist-2.1.3/ailist/array_query_core.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/array_query_core.cpython-311-darwin.so` & `ailist-2.1.3/ailist/array_query_core.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/array_query_core.pxd` & `ailist-2.1.3/ailist/array_query_core.pxd`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/array_query_core.pyx` & `ailist-2.1.3/ailist/array_query_core.pyx`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/ailist/ailist_add.c` & `ailist-2.1.3/ailist/src/ailist/ailist_add.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/ailist/ailist_closest.c` & `ailist-2.1.3/ailist/src/ailist/ailist_closest.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/ailist/ailist_construct.c` & `ailist-2.1.3/ailist/src/ailist/ailist_construct.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/ailist/ailist_coverage.c` & `ailist-2.1.3/ailist/src/ailist/ailist_coverage.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/ailist/ailist_extract.c` & `ailist-2.1.3/ailist/src/ailist/ailist_extract.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/ailist/ailist_filter.c` & `ailist-2.1.3/ailist/src/ailist/ailist_filter.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/ailist/ailist_get_id.c` & `ailist-2.1.3/ailist/src/ailist/ailist_get_id.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/ailist/ailist_iter.c` & `ailist-2.1.3/ailist/src/ailist/ailist_iter.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/ailist/ailist_merge.c` & `ailist-2.1.3/ailist/src/ailist/ailist_merge.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/ailist/ailist_nhits.c` & `ailist-2.1.3/ailist/src/ailist/ailist_nhits.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/ailist/ailist_ops.c` & `ailist-2.1.3/ailist/src/ailist/ailist_ops.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/ailist/ailist_query.c` & `ailist-2.1.3/ailist/src/ailist/ailist_query.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/ailist/ailist_simulate.c` & `ailist-2.1.3/ailist/src/ailist/ailist_simulate.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/ailist/ailist_wps.c` & `ailist-2.1.3/ailist/src/ailist/ailist_wps.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/ailist/augmented_interval_list.c` & `ailist-2.1.3/ailist/src/ailist/augmented_interval_list.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/ailist/augmented_interval_list.h` & `ailist-2.1.3/ailist/src/ailist/augmented_interval_list.h`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/ailist/interval.c` & `ailist-2.1.3/ailist/src/ailist/interval.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/ailist/interval.h` & `ailist-2.1.3/ailist/src/ailist/interval.h`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/ailist/overlap_index.c` & `ailist-2.1.3/ailist/src/ailist/overlap_index.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/array_query/array_query_utilities.c` & `ailist-2.1.3/ailist/src/array_query/array_query_utilities.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/array_query/array_query_utilities.h` & `ailist-2.1.3/ailist/src/array_query/array_query_utilities.h`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/labeled_aiarray/khash.h` & `ailist-2.1.3/ailist/src/labeled_aiarray/khash.h`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/labeled_aiarray/kvec.h` & `ailist-2.1.3/ailist/src/labeled_aiarray/kvec.h`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_add.c` & `ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_add.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_construct.c` & `ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_construct.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_coverage.c` & `ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_coverage.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_extract.c` & `ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_extract.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_filter.c` & `ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_filter.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_get.c` & `ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_get.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_index.c` & `ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_index.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_iter.c` & `ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_iter.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_match.c` & `ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_match.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_merge.c` & `ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_merge.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_nhits.c` & `ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_nhits.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_ops.c` & `ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_ops.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_percent.c` & `ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_percent.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_query_array.c` & `ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_query_array.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_query_index.c` & `ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_query_index.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_query_single.c` & `ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_query_single.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_simulate.c` & `ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_simulate.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_sort.c` & `ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_sort.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/labeled_aiarray/labeled_aiarray_wps.c` & `ailist-2.1.3/ailist/src/labeled_aiarray/labeled_aiarray_wps.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/labeled_aiarray/labeled_augmented_array.c` & `ailist-2.1.3/ailist/src/labeled_aiarray/labeled_augmented_array.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/labeled_aiarray/labeled_augmented_array.h` & `ailist-2.1.3/ailist/src/labeled_aiarray/labeled_augmented_array.h`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/labeled_aiarray/overlap_label_index.c` & `ailist-2.1.3/ailist/src/labeled_aiarray/overlap_label_index.c`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/ailist/src/utilities/utilities.h` & `ailist-2.1.3/ailist/src/utilities/utilities.h`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/build.py` & `ailist-2.1.3/build.py`

 * *Files identical despite different names*

### Comparing `ailist-2.1.2/pyproject.toml` & `ailist-2.1.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ailist"
-version = "2.1.2"
+version = "2.1.3"
 description = "Python package for Augmented Interval List"
 authors = ["Kyle S. Smith <kyle.smith@stjude.org>"]
 maintainers = ["Kyle S. Smith <kyle.smith@stjude.org>"]
 repository = "https://github.com/kylessmith/ailist"
 documentation = "https://www.biosciencestack.com/static/ailist/docs/index.html"
 keywords = ["cython", "interval", "ailist", "c"]
 readme = 'README.md'
@@ -26,25 +26,25 @@
                   ]
 packages = [{ include = "ailist" }]
 include = ["ailist/*.pyx", "ailist/*.pxd", "ailist/src/*.h", "ailist/src/*.c", "ailist/**/*.so"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.23.5"
-cython = "^0.29.32"
-pandas = "^1.5.2"
+cython = "^3.0.0"
+pandas = "^2.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0",
-            "cython>=0.29.32",
+            "cython>=3.0.0",
             "numpy>=1.23.5",
-            "pandas>=1.5.2",
+            "pandas>=2.0.0",
             "setuptools>=65.5.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.build]
 generate-setup-file = false
 script = "build.py"
```

### Comparing `ailist-2.1.2/PKG-INFO` & `ailist-2.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ailist
-Version: 2.1.2
+Version: 2.1.3
 Summary: Python package for Augmented Interval List
 Home-page: https://github.com/kylessmith/ailist
 License: GPL-2.0-or-later
 Keywords: cython,interval,ailist,c
 Author: Kyle S. Smith
 Author-email: kyle.smith@stjude.org
 Maintainer: Kyle S. Smith
@@ -24,17 +24,17 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: cython (>=0.29.32,<0.30.0)
+Requires-Dist: cython (>=3.0.0,<4.0.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
-Requires-Dist: pandas (>=1.5.2,<2.0.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Project-URL: Documentation, https://www.biosciencestack.com/static/ailist/docs/index.html
 Project-URL: Repository, https://github.com/kylessmith/ailist
 Description-Content-Type: text/markdown
 
 # Augmented Interval List
 
 [![Build Status](https://travis-ci.org/kylessmith/ailist.svg?branch=master)](https://travis-ci.org/kylessmith/ailist) [![PyPI version](https://badge.fury.io/py/ailist.svg)](https://badge.fury.io/py/ailist)
```

