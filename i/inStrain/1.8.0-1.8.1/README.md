# Comparing `tmp/inStrain-1.8.0.tar.gz` & `tmp/inStrain-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inStrain-1.8.0.tar", last modified: Fri Aug 25 00:19:07 2023, max compression
+gzip compressed data, was "inStrain-1.8.1.tar", last modified: Tue Apr 16 20:06:55 2024, max compression
```

## Comparing `inStrain-1.8.0.tar` & `inStrain-1.8.1.tar`

### file list

```diff
@@ -1,68 +1,75 @@
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-08-25 00:19:07.353091 inStrain-1.8.0/
--rw-r--r--   0 mattolm    (501) staff       (20)     1065 2021-03-26 22:19:41.000000 inStrain-1.8.0/LICENSE
--rw-r--r--   0 mattolm    (501) staff       (20)       25 2023-08-25 00:17:39.000000 inStrain-1.8.0/MANIFEST.in
--rw-r--r--   0 mattolm    (501) staff       (20)      279 2023-08-25 00:19:07.352950 inStrain-1.8.0/PKG-INFO
--rw-r--r--   0 mattolm    (501) staff       (20)     1416 2023-02-21 01:15:19.000000 inStrain-1.8.0/README.md
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-08-25 00:19:07.335745 inStrain-1.8.0/bin/
--rwxr-xr-x   0 mattolm    (501) staff       (20)      962 2021-01-21 18:18:24.000000 inStrain-1.8.0/bin/inStrain
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-08-25 00:19:07.336651 inStrain-1.8.0/docker/
--rw-r--r--   0 mattolm    (501) staff       (20)        0 2021-01-21 18:18:24.000000 inStrain-1.8.0/docker/__init__.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)     1688 2021-01-21 18:18:24.000000 inStrain-1.8.0/docker/job_utils.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)    10928 2022-06-10 19:12:50.000000 inStrain-1.8.0/docker/run_instrain.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)     5153 2021-01-21 18:18:24.000000 inStrain-1.8.0/docker/s3_utils.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-08-25 00:19:07.343445 inStrain-1.8.0/inStrain/
--rwxr-xr-x   0 mattolm    (501) staff       (20)    31954 2023-02-24 17:32:05.000000 inStrain-1.8.0/inStrain/GeneProfile.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)    42885 2023-08-24 22:02:53.000000 inStrain-1.8.0/inStrain/SNVprofile.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)       34 2021-01-21 18:18:24.000000 inStrain-1.8.0/inStrain/__init__.py
--rw-r--r--   0 mattolm    (501) staff       (20)       22 2023-08-24 20:56:03.000000 inStrain-1.8.0/inStrain/_version.py
--rw-r--r--   0 mattolm    (501) staff       (20)    23404 2023-08-24 21:40:49.000000 inStrain-1.8.0/inStrain/argumentParser.py
--rw-r--r--   0 mattolm    (501) staff       (20)    25579 2023-07-26 21:10:33.000000 inStrain-1.8.0/inStrain/compare_controller.py
--rw-r--r--   0 mattolm    (501) staff       (20)     4897 2021-01-21 18:18:24.000000 inStrain-1.8.0/inStrain/compare_greedy.py
--rw-r--r--   0 mattolm    (501) staff       (20)     8480 2023-02-25 01:32:59.000000 inStrain-1.8.0/inStrain/compare_utils.py
--rw-r--r--   0 mattolm    (501) staff       (20)    18260 2023-08-24 22:04:23.000000 inStrain-1.8.0/inStrain/controller.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-08-25 00:19:07.345577 inStrain-1.8.0/inStrain/deprecated/
--rw-r--r--   0 mattolm    (501) staff       (20)     2257 2023-02-24 18:53:38.000000 inStrain-1.8.0/inStrain/deprecated/DEPRECATEDmapping_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)    34343 2021-02-12 01:00:32.000000 inStrain-1.8.0/inStrain/deprecated/__init__.py
--rw-r--r--   0 mattolm    (501) staff       (20)    22971 2021-01-21 18:18:24.000000 inStrain-1.8.0/inStrain/deprecated/deprecated_filter_reads.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)     9651 2021-01-21 18:18:24.000000 inStrain-1.8.0/inStrain/deprecated/deprecated_gene_statistics.py
--rw-r--r--   0 mattolm    (501) staff       (20)    58073 2023-02-25 01:32:59.000000 inStrain-1.8.0/inStrain/deprecated/plottingUtilities.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)    35695 2023-02-25 01:48:27.000000 inStrain-1.8.0/inStrain/filter_reads.py
--rw-r--r--   0 mattolm    (501) staff       (20)    34630 2023-08-24 21:18:50.000000 inStrain-1.8.0/inStrain/genomeUtilities.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-08-25 00:19:07.346618 inStrain-1.8.0/inStrain/helper_files/
--rw-r--r--   0 mattolm    (501) staff       (20)  1256610 2021-01-21 18:18:24.000000 inStrain-1.8.0/inStrain/helper_files/NullModel.txt
--rw-r--r--   0 mattolm    (501) staff       (20)     8957 2021-02-12 01:00:32.000000 inStrain-1.8.0/inStrain/irep_utilities.py
--rw-r--r--   0 mattolm    (501) staff       (20)    38401 2021-03-26 21:19:02.000000 inStrain-1.8.0/inStrain/logUtils.py
--rw-r--r--   0 mattolm    (501) staff       (20)    15346 2023-05-16 21:08:22.000000 inStrain-1.8.0/inStrain/parse_annotations.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-08-25 00:19:07.350511 inStrain-1.8.0/inStrain/plotting/
--rw-r--r--   0 mattolm    (501) staff       (20)     2524 2023-02-24 18:53:38.000000 inStrain-1.8.0/inStrain/plotting/SNV_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)      662 2021-02-12 01:00:32.000000 inStrain-1.8.0/inStrain/plotting/__init__.py
--rw-r--r--   0 mattolm    (501) staff       (20)     9260 2023-02-25 01:38:35.000000 inStrain-1.8.0/inStrain/plotting/compare_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)     2548 2021-02-12 01:00:32.000000 inStrain-1.8.0/inStrain/plotting/gene_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)     6638 2023-02-24 18:50:29.000000 inStrain-1.8.0/inStrain/plotting/linkage_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)     9075 2023-02-25 00:47:19.000000 inStrain-1.8.0/inStrain/plotting/mapping_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)     5332 2023-02-25 00:49:14.000000 inStrain-1.8.0/inStrain/plotting/plotting_controller.py
--rw-r--r--   0 mattolm    (501) staff       (20)    18496 2023-07-26 21:15:53.000000 inStrain-1.8.0/inStrain/plotting/positional_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)     2831 2021-02-12 01:00:32.000000 inStrain-1.8.0/inStrain/plotting/utilities.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)    20770 2023-07-26 21:10:50.000000 inStrain-1.8.0/inStrain/polymorpher.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-08-25 00:19:07.352421 inStrain-1.8.0/inStrain/profile/
--rw-r--r--   0 mattolm    (501) staff       (20)      636 2021-01-21 18:18:24.000000 inStrain-1.8.0/inStrain/profile/__init__.py
--rw-r--r--   0 mattolm    (501) staff       (20)     5822 2021-02-12 01:00:32.000000 inStrain-1.8.0/inStrain/profile/fasta.py
--rw-r--r--   0 mattolm    (501) staff       (20)     9115 2021-01-21 18:18:24.000000 inStrain-1.8.0/inStrain/profile/linkage.py
--rw-r--r--   0 mattolm    (501) staff       (20)    15636 2021-01-21 18:18:24.000000 inStrain-1.8.0/inStrain/profile/profile_controller.py
--rw-r--r--   0 mattolm    (501) staff       (20)    32898 2023-08-24 20:15:12.000000 inStrain-1.8.0/inStrain/profile/profile_utilities.py
--rw-r--r--   0 mattolm    (501) staff       (20)     4682 2023-08-24 22:21:03.000000 inStrain-1.8.0/inStrain/profile/samtools_ops.py
--rw-r--r--   0 mattolm    (501) staff       (20)    10361 2021-02-12 01:00:32.000000 inStrain-1.8.0/inStrain/profile/snv_utilities.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)     5332 2021-02-12 01:00:32.000000 inStrain-1.8.0/inStrain/quickProfile.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)    16916 2022-06-10 19:12:50.000000 inStrain-1.8.0/inStrain/readComparer.py
--rw-r--r--   0 mattolm    (501) staff       (20)     2641 2023-08-24 20:54:04.000000 inStrain-1.8.0/inStrain/utils.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-08-25 00:19:07.344227 inStrain-1.8.0/inStrain.egg-info/
--rw-r--r--   0 mattolm    (501) staff       (20)      279 2023-08-25 00:19:07.000000 inStrain-1.8.0/inStrain.egg-info/PKG-INFO
--rw-r--r--   0 mattolm    (501) staff       (20)     1575 2023-08-25 00:19:07.000000 inStrain-1.8.0/inStrain.egg-info/SOURCES.txt
--rw-r--r--   0 mattolm    (501) staff       (20)        1 2023-08-25 00:19:07.000000 inStrain-1.8.0/inStrain.egg-info/dependency_links.txt
--rw-r--r--   0 mattolm    (501) staff       (20)        1 2023-08-25 00:19:07.000000 inStrain-1.8.0/inStrain.egg-info/not-zip-safe
--rw-r--r--   0 mattolm    (501) staff       (20)      113 2023-08-25 00:19:07.000000 inStrain-1.8.0/inStrain.egg-info/requires.txt
--rw-r--r--   0 mattolm    (501) staff       (20)       16 2023-08-25 00:19:07.000000 inStrain-1.8.0/inStrain.egg-info/top_level.txt
--rw-r--r--   0 mattolm    (501) staff       (20)       38 2023-08-25 00:19:07.353125 inStrain-1.8.0/setup.cfg
--rw-r--r--   0 mattolm    (501) staff       (20)     1050 2023-08-25 00:13:07.000000 inStrain-1.8.0/setup.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-08-25 00:19:07.352671 inStrain-1.8.0/test/
--rwxr-xr-x   0 mattolm    (501) staff       (20)     1215 2023-08-24 18:38:00.000000 inStrain-1.8.0/test/test_suite.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-04-16 20:06:55.628996 inStrain-1.8.1/
+-rw-r--r--   0 mattolm    (501) staff       (20)    10244 2023-02-08 00:15:21.000000 inStrain-1.8.1/.DS_Store
+-rw-r--r--   0 mattolm    (501) staff       (20)       74 2021-01-21 18:18:24.000000 inStrain-1.8.1/.gitignore
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-04-16 20:06:55.617672 inStrain-1.8.1/.vscode/
+-rw-r--r--   0 mattolm    (501) staff       (20)       36 2022-10-22 22:33:02.000000 inStrain-1.8.1/.vscode/settings.json
+-rw-r--r--   0 mattolm    (501) staff       (20)    26571 2024-04-12 21:02:12.000000 inStrain-1.8.1/CHANGELOG.md
+-rw-r--r--   0 mattolm    (501) staff       (20)     1065 2021-03-26 22:19:41.000000 inStrain-1.8.1/LICENSE
+-rw-r--r--   0 mattolm    (501) staff       (20)       76 2024-04-16 20:05:57.000000 inStrain-1.8.1/MANIFEST.in
+-rw-r--r--   0 mattolm    (501) staff       (20)      572 2024-04-16 20:06:55.628631 inStrain-1.8.1/PKG-INFO
+-rw-r--r--   0 mattolm    (501) staff       (20)     1416 2023-02-21 01:15:19.000000 inStrain-1.8.1/README.md
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-04-16 20:06:55.618006 inStrain-1.8.1/auxiliary_scripts/
+-rwxr-xr-x   0 mattolm    (501) staff       (20)    13618 2023-08-24 21:29:51.000000 inStrain-1.8.1/auxiliary_scripts/rarefaction_curve.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)     5020 2023-02-25 01:32:59.000000 inStrain-1.8.1/auxiliary_scripts/recluster_instrain_compare.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-04-16 20:06:55.618167 inStrain-1.8.1/bin/
+-rwxr-xr-x   0 mattolm    (501) staff       (20)      962 2021-01-21 18:18:24.000000 inStrain-1.8.1/bin/inStrain
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-04-16 20:06:55.618310 inStrain-1.8.1/dist/
+-rw-r--r--   0 mattolm    (501) staff       (20)    85716 2021-01-21 18:18:24.000000 inStrain-1.8.1/dist/inStrain-1.0.0.tar.gz
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-04-16 20:06:55.621378 inStrain-1.8.1/inStrain/
+-rwxr-xr-x   0 mattolm    (501) staff       (20)    31954 2023-02-24 17:32:05.000000 inStrain-1.8.1/inStrain/GeneProfile.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)    42879 2024-04-12 21:01:13.000000 inStrain-1.8.1/inStrain/SNVprofile.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)       34 2021-01-21 18:18:24.000000 inStrain-1.8.1/inStrain/__init__.py
+-rw-r--r--   0 mattolm    (501) staff       (20)       22 2024-04-12 21:01:21.000000 inStrain-1.8.1/inStrain/_version.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    23404 2023-08-24 21:40:49.000000 inStrain-1.8.1/inStrain/argumentParser.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    25579 2023-07-26 21:10:33.000000 inStrain-1.8.1/inStrain/compare_controller.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     4897 2021-01-21 18:18:24.000000 inStrain-1.8.1/inStrain/compare_greedy.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     8480 2023-02-25 01:32:59.000000 inStrain-1.8.1/inStrain/compare_utils.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    18260 2023-08-24 22:04:23.000000 inStrain-1.8.1/inStrain/controller.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-04-16 20:06:55.622961 inStrain-1.8.1/inStrain/deprecated/
+-rw-r--r--   0 mattolm    (501) staff       (20)     2257 2023-02-24 18:53:38.000000 inStrain-1.8.1/inStrain/deprecated/DEPRECATEDmapping_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    34343 2021-02-12 01:00:32.000000 inStrain-1.8.1/inStrain/deprecated/__init__.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    22971 2021-01-21 18:18:24.000000 inStrain-1.8.1/inStrain/deprecated/deprecated_filter_reads.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)     9651 2021-01-21 18:18:24.000000 inStrain-1.8.1/inStrain/deprecated/deprecated_gene_statistics.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    58073 2023-02-25 01:32:59.000000 inStrain-1.8.1/inStrain/deprecated/plottingUtilities.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)    35695 2023-02-25 01:48:27.000000 inStrain-1.8.1/inStrain/filter_reads.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    34630 2023-08-24 21:18:50.000000 inStrain-1.8.1/inStrain/genomeUtilities.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-04-16 20:06:55.623144 inStrain-1.8.1/inStrain/helper_files/
+-rw-r--r--   0 mattolm    (501) staff       (20)  1256610 2021-01-21 18:18:24.000000 inStrain-1.8.1/inStrain/helper_files/NullModel.txt
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-04-16 20:06:55.625562 inStrain-1.8.1/inStrain/helper_scripts/
+-rw-r--r--   0 mattolm    (501) staff       (20)  1256610 2021-01-21 18:18:24.000000 inStrain-1.8.1/inStrain/helper_scripts/NullModel_1000000.txt
+-rw-r--r--   0 mattolm    (501) staff       (20)  1072260 2021-01-21 18:18:24.000000 inStrain-1.8.1/inStrain/helper_scripts/NullModel_50000.txt
+-rwxr-xr-x   0 mattolm    (501) staff       (20)     2711 2023-02-25 01:31:38.000000 inStrain-1.8.1/inStrain/helper_scripts/calculate_null.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     8957 2021-02-12 01:00:32.000000 inStrain-1.8.1/inStrain/irep_utilities.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    38401 2021-03-26 21:19:02.000000 inStrain-1.8.1/inStrain/logUtils.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    15346 2023-05-16 21:08:22.000000 inStrain-1.8.1/inStrain/parse_annotations.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-04-16 20:06:55.626895 inStrain-1.8.1/inStrain/plotting/
+-rw-r--r--   0 mattolm    (501) staff       (20)     2524 2023-02-24 18:53:38.000000 inStrain-1.8.1/inStrain/plotting/SNV_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)      662 2021-02-12 01:00:32.000000 inStrain-1.8.1/inStrain/plotting/__init__.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     9260 2023-02-25 01:38:35.000000 inStrain-1.8.1/inStrain/plotting/compare_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     2548 2021-02-12 01:00:32.000000 inStrain-1.8.1/inStrain/plotting/gene_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     6638 2023-02-24 18:50:29.000000 inStrain-1.8.1/inStrain/plotting/linkage_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     9075 2023-02-25 00:47:19.000000 inStrain-1.8.1/inStrain/plotting/mapping_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     5332 2023-02-25 00:49:14.000000 inStrain-1.8.1/inStrain/plotting/plotting_controller.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    18496 2023-07-26 21:15:53.000000 inStrain-1.8.1/inStrain/plotting/positional_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     2831 2021-02-12 01:00:32.000000 inStrain-1.8.1/inStrain/plotting/utilities.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)    20770 2023-07-26 21:10:50.000000 inStrain-1.8.1/inStrain/polymorpher.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-04-16 20:06:55.627940 inStrain-1.8.1/inStrain/profile/
+-rw-r--r--   0 mattolm    (501) staff       (20)      636 2021-01-21 18:18:24.000000 inStrain-1.8.1/inStrain/profile/__init__.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     5822 2021-02-12 01:00:32.000000 inStrain-1.8.1/inStrain/profile/fasta.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     9115 2021-01-21 18:18:24.000000 inStrain-1.8.1/inStrain/profile/linkage.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    15636 2021-01-21 18:18:24.000000 inStrain-1.8.1/inStrain/profile/profile_controller.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    32898 2023-08-24 20:15:12.000000 inStrain-1.8.1/inStrain/profile/profile_utilities.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     4682 2023-08-24 22:21:03.000000 inStrain-1.8.1/inStrain/profile/samtools_ops.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    10361 2021-02-12 01:00:32.000000 inStrain-1.8.1/inStrain/profile/snv_utilities.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)     5332 2021-02-12 01:00:32.000000 inStrain-1.8.1/inStrain/quickProfile.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)    16916 2022-06-10 19:12:50.000000 inStrain-1.8.1/inStrain/readComparer.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     2641 2023-08-24 20:54:04.000000 inStrain-1.8.1/inStrain/utils.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-04-16 20:06:55.628159 inStrain-1.8.1/inStrain.egg-info/
+-rw-r--r--   0 mattolm    (501) staff       (20)      572 2024-04-16 20:06:54.000000 inStrain-1.8.1/inStrain.egg-info/PKG-INFO
+-rw-r--r--   0 mattolm    (501) staff       (20)     1777 2024-04-16 20:06:55.000000 inStrain-1.8.1/inStrain.egg-info/SOURCES.txt
+-rw-r--r--   0 mattolm    (501) staff       (20)        1 2024-04-16 20:06:54.000000 inStrain-1.8.1/inStrain.egg-info/dependency_links.txt
+-rw-r--r--   0 mattolm    (501) staff       (20)        1 2024-04-16 20:06:54.000000 inStrain-1.8.1/inStrain.egg-info/not-zip-safe
+-rw-r--r--   0 mattolm    (501) staff       (20)      113 2024-04-16 20:06:54.000000 inStrain-1.8.1/inStrain.egg-info/requires.txt
+-rw-r--r--   0 mattolm    (501) staff       (20)       16 2024-04-16 20:06:54.000000 inStrain-1.8.1/inStrain.egg-info/top_level.txt
+-rw-r--r--   0 mattolm    (501) staff       (20)       38 2024-04-16 20:06:55.629055 inStrain-1.8.1/setup.cfg
+-rw-r--r--   0 mattolm    (501) staff       (20)     1020 2024-04-16 20:04:18.000000 inStrain-1.8.1/setup.py
```

### Comparing `inStrain-1.8.0/LICENSE` & `inStrain-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/README.md` & `inStrain-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/bin/inStrain` & `inStrain-1.8.1/bin/inStrain`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/GeneProfile.py` & `inStrain-1.8.1/inStrain/GeneProfile.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/SNVprofile.py` & `inStrain-1.8.1/inStrain/SNVprofile.py`

 * *Files 0% similar despite different names*

```diff
@@ -636,15 +636,15 @@
     def _get_covt_keys(self):
         '''
         A special method for getting the keys to covT
         '''
         Adb = self._get_attributes_file()
 
         scaffs = set()
-        filename = self.get_location('raw_data') + '/' + os.path.basename(Adb.loc['covT', 'value'])
+        filename = self.get_location('raw_data') + os.path.basename(Adb.loc['covT', 'value'])
         f = h5py.File(filename, 'r')
         for thing in list(f.keys()):
             scaff, mm = thing.split('::')
             scaffs.add(scaff)
         return scaffs
```

### Comparing `inStrain-1.8.0/inStrain/argumentParser.py` & `inStrain-1.8.1/inStrain/argumentParser.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/compare_controller.py` & `inStrain-1.8.1/inStrain/compare_controller.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/compare_greedy.py` & `inStrain-1.8.1/inStrain/compare_greedy.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/compare_utils.py` & `inStrain-1.8.1/inStrain/compare_utils.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/controller.py` & `inStrain-1.8.1/inStrain/controller.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/deprecated/DEPRECATEDmapping_plots.py` & `inStrain-1.8.1/inStrain/deprecated/DEPRECATEDmapping_plots.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/deprecated/__init__.py` & `inStrain-1.8.1/inStrain/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/deprecated/deprecated_filter_reads.py` & `inStrain-1.8.1/inStrain/deprecated/deprecated_filter_reads.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/deprecated/deprecated_gene_statistics.py` & `inStrain-1.8.1/inStrain/deprecated/deprecated_gene_statistics.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/deprecated/plottingUtilities.py` & `inStrain-1.8.1/inStrain/deprecated/plottingUtilities.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/filter_reads.py` & `inStrain-1.8.1/inStrain/filter_reads.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/genomeUtilities.py` & `inStrain-1.8.1/inStrain/genomeUtilities.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/helper_files/NullModel.txt` & `inStrain-1.8.1/inStrain/helper_files/NullModel.txt`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/irep_utilities.py` & `inStrain-1.8.1/inStrain/irep_utilities.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/logUtils.py` & `inStrain-1.8.1/inStrain/logUtils.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/parse_annotations.py` & `inStrain-1.8.1/inStrain/parse_annotations.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/plotting/SNV_plots.py` & `inStrain-1.8.1/inStrain/plotting/SNV_plots.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/plotting/__init__.py` & `inStrain-1.8.1/inStrain/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/plotting/compare_plots.py` & `inStrain-1.8.1/inStrain/plotting/compare_plots.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/plotting/gene_plots.py` & `inStrain-1.8.1/inStrain/plotting/gene_plots.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/plotting/linkage_plots.py` & `inStrain-1.8.1/inStrain/plotting/linkage_plots.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/plotting/mapping_plots.py` & `inStrain-1.8.1/inStrain/plotting/mapping_plots.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/plotting/plotting_controller.py` & `inStrain-1.8.1/inStrain/plotting/plotting_controller.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/plotting/positional_plots.py` & `inStrain-1.8.1/inStrain/plotting/positional_plots.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/plotting/utilities.py` & `inStrain-1.8.1/inStrain/plotting/utilities.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/polymorpher.py` & `inStrain-1.8.1/inStrain/polymorpher.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/profile/__init__.py` & `inStrain-1.8.1/inStrain/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/profile/fasta.py` & `inStrain-1.8.1/inStrain/profile/fasta.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/profile/linkage.py` & `inStrain-1.8.1/inStrain/profile/linkage.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/profile/profile_controller.py` & `inStrain-1.8.1/inStrain/profile/profile_controller.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/profile/profile_utilities.py` & `inStrain-1.8.1/inStrain/profile/profile_utilities.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/profile/samtools_ops.py` & `inStrain-1.8.1/inStrain/profile/samtools_ops.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/profile/snv_utilities.py` & `inStrain-1.8.1/inStrain/profile/snv_utilities.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/quickProfile.py` & `inStrain-1.8.1/inStrain/quickProfile.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/readComparer.py` & `inStrain-1.8.1/inStrain/readComparer.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain/utils.py` & `inStrain-1.8.1/inStrain/utils.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.0/inStrain.egg-info/SOURCES.txt` & `inStrain-1.8.1/inStrain.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+.DS_Store
+.gitignore
+CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 setup.py
+.vscode/settings.json
+auxiliary_scripts/rarefaction_curve.py
+auxiliary_scripts/recluster_instrain_compare.py
 bin/inStrain
-docker/__init__.py
-docker/job_utils.py
-docker/run_instrain.py
-docker/s3_utils.py
+dist/inStrain-1.0.0.tar.gz
 inStrain/GeneProfile.py
 inStrain/SNVprofile.py
 inStrain/__init__.py
 inStrain/_version.py
 inStrain/argumentParser.py
 inStrain/compare_controller.py
 inStrain/compare_greedy.py
@@ -33,14 +36,17 @@
 inStrain.egg-info/top_level.txt
 inStrain/deprecated/DEPRECATEDmapping_plots.py
 inStrain/deprecated/__init__.py
 inStrain/deprecated/deprecated_filter_reads.py
 inStrain/deprecated/deprecated_gene_statistics.py
 inStrain/deprecated/plottingUtilities.py
 inStrain/helper_files/NullModel.txt
+inStrain/helper_scripts/NullModel_1000000.txt
+inStrain/helper_scripts/NullModel_50000.txt
+inStrain/helper_scripts/calculate_null.py
 inStrain/plotting/SNV_plots.py
 inStrain/plotting/__init__.py
 inStrain/plotting/compare_plots.py
 inStrain/plotting/gene_plots.py
 inStrain/plotting/linkage_plots.py
 inStrain/plotting/mapping_plots.py
 inStrain/plotting/plotting_controller.py
@@ -48,9 +54,8 @@
 inStrain/plotting/utilities.py
 inStrain/profile/__init__.py
 inStrain/profile/fasta.py
 inStrain/profile/linkage.py
 inStrain/profile/profile_controller.py
 inStrain/profile/profile_utilities.py
 inStrain/profile/samtools_ops.py
-inStrain/profile/snv_utilities.py
-test/test_suite.py
+inStrain/profile/snv_utilities.py
```

### Comparing `inStrain-1.8.0/setup.py` & `inStrain-1.8.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,14 @@
       version=__version__,
       description='Calculation of strain-level metrics',
       url='https://github.com/MrOlm/inStrain',
       author='Matt Olm and Alex Crits-Christoph',
       author_email='mattolm@berkeley.edu',
       license='MIT',
       package_data={'inStrain': ['helper_files/NullModel.txt']},
-      #packages=['inStrain'],
       packages=find_packages(exclude=["test"]),
       scripts=['bin/inStrain'],
       python_requires='>=3.4.0',
       install_requires=[
           'numpy',
           'pandas>=0.25,!=1.1.3',
           'seaborn',
```

