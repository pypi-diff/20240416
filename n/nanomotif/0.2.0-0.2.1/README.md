# Comparing `tmp/nanomotif-0.2.0.tar.gz` & `tmp/nanomotif-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanomotif-0.2.0.tar", last modified: Fri Mar 29 17:14:37 2024, max compression
+gzip compressed data, was "nanomotif-0.2.1.tar", last modified: Tue Apr 16 09:18:22 2024, max compression
```

## Comparing `nanomotif-0.2.0.tar` & `nanomotif-0.2.1.tar`

### file list

```diff
@@ -1,64 +1,66 @@
-drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-03-29 17:14:37.031970 nanomotif-0.2.0/
--rw-rw-r--   0 shei      (1000) shei      (1000)     1084 2023-11-30 15:56:56.000000 nanomotif-0.2.0/LICENSE
--rw-r--r--   0 shei      (1000) shei      (1000)    17430 2024-03-29 17:14:37.031970 nanomotif-0.2.0/PKG-INFO
--rw-rw-r--   0 shei      (1000) shei      (1000)    16907 2024-03-29 17:14:10.000000 nanomotif-0.2.0/README.md
-drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-03-29 17:14:36.995970 nanomotif-0.2.0/nanomotif/
--rw-rw-r--   0 shei      (1000) shei      (1000)      278 2024-03-29 12:58:11.000000 nanomotif-0.2.0/nanomotif/__init__.py
--rw-rw-r--   0 shei      (1000) shei      (1000)       22 2024-03-29 17:14:10.000000 nanomotif-0.2.0/nanomotif/_version.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     8055 2024-03-29 17:14:10.000000 nanomotif-0.2.0/nanomotif/argparser.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     6009 2024-03-29 12:58:11.000000 nanomotif-0.2.0/nanomotif/bin_consensus.py
-drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-03-29 17:14:36.995970 nanomotif-0.2.0/nanomotif/binnary/
--rw-rw-r--   0 shei      (1000) shei      (1000)        0 2024-03-29 17:14:10.000000 nanomotif-0.2.0/nanomotif/binnary/__init__.py
--rw-rw-r--   0 shei      (1000) shei      (1000)    13167 2024-03-29 17:14:10.000000 nanomotif-0.2.0/nanomotif/binnary/analysis.py
--rw-rw-r--   0 shei      (1000) shei      (1000)    15541 2024-03-29 17:14:10.000000 nanomotif-0.2.0/nanomotif/binnary/data_processing.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     4254 2024-03-29 17:14:10.000000 nanomotif-0.2.0/nanomotif/binnary/detect_contamination.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     3545 2024-03-29 17:14:10.000000 nanomotif-0.2.0/nanomotif/binnary/include_contigs.py
--rw-rw-r--   0 shei      (1000) shei      (1000)      890 2024-03-29 17:14:10.000000 nanomotif-0.2.0/nanomotif/binnary/logging.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     7543 2024-03-29 17:14:10.000000 nanomotif-0.2.0/nanomotif/binnary/scoring.py
--rw-rw-r--   0 shei      (1000) shei      (1000)      522 2024-03-29 17:14:10.000000 nanomotif-0.2.0/nanomotif/binnary/utils.py
--rw-rw-r--   0 shei      (1000) shei      (1000)    14165 2024-03-29 12:58:11.000000 nanomotif-0.2.0/nanomotif/candidate.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     1061 2024-03-29 12:58:11.000000 nanomotif-0.2.0/nanomotif/constants.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     1698 2024-03-29 12:58:11.000000 nanomotif-0.2.0/nanomotif/dataload.py
-drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-03-29 17:14:36.999970 nanomotif-0.2.0/nanomotif/datasets/
--rw-rw-r--   0 shei      (1000) shei      (1000)       27 2024-03-29 17:14:10.000000 nanomotif-0.2.0/nanomotif/datasets/geobacillus-contig-bin.tsv
--rw-rw-r--   0 shei      (1000) shei      (1000)   176247 2024-03-29 17:14:10.000000 nanomotif-0.2.0/nanomotif/datasets/geobacillus-plasmids.assembly.fasta
--rw-rw-r--   0 shei      (1000) shei      (1000) 26479844 2024-03-29 17:14:10.000000 nanomotif-0.2.0/nanomotif/datasets/geobacillus-plasmids.pileup.bed
--rw-rw-r--   0 shei      (1000) shei      (1000)     1106 2024-03-29 17:14:10.000000 nanomotif-0.2.0/nanomotif/datasets.py
--rw-rw-r--   0 shei      (1000) shei      (1000)    28677 2024-03-29 12:58:11.000000 nanomotif-0.2.0/nanomotif/evaluate.py
--rw-rw-r--   0 shei      (1000) shei      (1000)      539 2024-03-29 12:58:11.000000 nanomotif-0.2.0/nanomotif/feature.py
--rw-rw-r--   0 shei      (1000) shei      (1000)      321 2024-03-29 12:58:11.000000 nanomotif-0.2.0/nanomotif/logger.py
--rw-rw-r--   0 shei      (1000) shei      (1000)    17742 2024-03-29 17:14:10.000000 nanomotif-0.2.0/nanomotif/main.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     1037 2024-03-29 12:58:11.000000 nanomotif-0.2.0/nanomotif/model.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     5639 2024-03-29 12:58:11.000000 nanomotif-0.2.0/nanomotif/old_search_method.py
--rw-rw-r--   0 shei      (1000) shei      (1000)      850 2024-03-29 12:58:11.000000 nanomotif-0.2.0/nanomotif/parallel.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     6202 2024-03-29 12:58:11.000000 nanomotif-0.2.0/nanomotif/postprocess.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     7193 2024-03-29 12:58:11.000000 nanomotif-0.2.0/nanomotif/scoremotifs.py
--rw-rw-r--   0 shei      (1000) shei      (1000)      197 2024-03-29 12:58:11.000000 nanomotif-0.2.0/nanomotif/seed.py
--rw-rw-r--   0 shei      (1000) shei      (1000)    20090 2024-03-29 12:58:11.000000 nanomotif-0.2.0/nanomotif/seq.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     2677 2024-03-29 12:58:11.000000 nanomotif-0.2.0/nanomotif/utils.py
-drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-03-29 17:14:37.031970 nanomotif-0.2.0/nanomotif.egg-info/
--rw-r--r--   0 shei      (1000) shei      (1000)    17430 2024-03-29 17:14:36.000000 nanomotif-0.2.0/nanomotif.egg-info/PKG-INFO
--rw-rw-r--   0 shei      (1000) shei      (1000)     1538 2024-03-29 17:14:36.000000 nanomotif-0.2.0/nanomotif.egg-info/SOURCES.txt
--rw-rw-r--   0 shei      (1000) shei      (1000)        1 2024-03-29 17:14:36.000000 nanomotif-0.2.0/nanomotif.egg-info/dependency_links.txt
--rw-rw-r--   0 shei      (1000) shei      (1000)       50 2024-03-29 17:14:36.000000 nanomotif-0.2.0/nanomotif.egg-info/entry_points.txt
--rw-rw-r--   0 shei      (1000) shei      (1000)        1 2023-11-30 15:56:57.000000 nanomotif-0.2.0/nanomotif.egg-info/not-zip-safe
--rw-rw-r--   0 shei      (1000) shei      (1000)      132 2024-03-29 17:14:36.000000 nanomotif-0.2.0/nanomotif.egg-info/requires.txt
--rw-rw-r--   0 shei      (1000) shei      (1000)       16 2024-03-29 17:14:36.000000 nanomotif-0.2.0/nanomotif.egg-info/top_level.txt
--rw-rw-r--   0 shei      (1000) shei      (1000)       38 2024-03-29 17:14:37.031970 nanomotif-0.2.0/setup.cfg
--rw-rw-r--   0 shei      (1000) shei      (1000)      918 2024-03-29 17:14:10.000000 nanomotif-0.2.0/setup.py
-drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-03-29 17:14:37.027970 nanomotif-0.2.0/tests/
--rw-rw-r--   0 shei      (1000) shei      (1000)        0 2023-11-30 15:56:56.000000 nanomotif-0.2.0/tests/__init__.py
-drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-03-29 17:14:37.031970 nanomotif-0.2.0/tests/binnary/
--rw-rw-r--   0 shei      (1000) shei      (1000)        0 2024-03-29 17:14:10.000000 nanomotif-0.2.0/tests/binnary/__init__.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     2056 2024-03-29 17:14:10.000000 nanomotif-0.2.0/tests/binnary/conftest.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     1019 2024-03-29 17:14:10.000000 nanomotif-0.2.0/tests/binnary/test_arg_parser.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     6352 2024-03-29 17:14:10.000000 nanomotif-0.2.0/tests/binnary/test_data_processing_functions.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     2585 2024-03-29 17:14:10.000000 nanomotif-0.2.0/tests/binnary/test_detect_contamination.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     1404 2024-03-29 17:14:10.000000 nanomotif-0.2.0/tests/binnary/test_generate_output.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     2132 2024-03-29 17:14:10.000000 nanomotif-0.2.0/tests/binnary/test_include_contigs.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     3829 2024-03-29 17:14:10.000000 nanomotif-0.2.0/tests/binnary/test_scoring.py
--rw-rw-r--   0 shei      (1000) shei      (1000)      744 2024-03-29 17:14:10.000000 nanomotif-0.2.0/tests/binnary/test_utils.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     7236 2023-11-30 15:56:57.000000 nanomotif-0.2.0/tests/test_candidate.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     1365 2024-03-29 11:56:23.000000 nanomotif-0.2.0/tests/test_dataload.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     2933 2024-03-29 11:56:23.000000 nanomotif-0.2.0/tests/test_motif_find.py
--rw-rw-r--   0 shei      (1000) shei      (1000)        0 2024-03-29 11:56:23.000000 nanomotif-0.2.0/tests/test_motif_score.py
+drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-04-16 09:18:22.096362 nanomotif-0.2.1/
+-rw-rw-r--   0 shei      (1000) shei      (1000)     1084 2023-11-30 15:56:56.000000 nanomotif-0.2.1/LICENSE
+-rw-r--r--   0 shei      (1000) shei      (1000)    18166 2024-04-16 09:18:22.096362 nanomotif-0.2.1/PKG-INFO
+-rw-rw-r--   0 shei      (1000) shei      (1000)    17643 2024-04-16 09:16:26.000000 nanomotif-0.2.1/README.md
+drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-04-16 09:18:22.048362 nanomotif-0.2.1/nanomotif/
+-rw-rw-r--   0 shei      (1000) shei      (1000)      278 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/__init__.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)       22 2024-04-16 09:16:45.000000 nanomotif-0.2.1/nanomotif/_version.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     8496 2024-04-16 09:16:26.000000 nanomotif-0.2.1/nanomotif/argparser.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     6009 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/bin_consensus.py
+drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-04-16 09:18:22.052362 nanomotif-0.2.1/nanomotif/binnary/
+-rw-rw-r--   0 shei      (1000) shei      (1000)        0 2024-03-29 17:14:10.000000 nanomotif-0.2.1/nanomotif/binnary/__init__.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)    13167 2024-03-29 17:14:10.000000 nanomotif-0.2.1/nanomotif/binnary/analysis.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)    15629 2024-04-16 09:16:26.000000 nanomotif-0.2.1/nanomotif/binnary/data_processing.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     3729 2024-04-16 09:16:26.000000 nanomotif-0.2.1/nanomotif/binnary/detect_contamination.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     3014 2024-04-16 09:16:26.000000 nanomotif-0.2.1/nanomotif/binnary/include_contigs.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)      890 2024-03-29 17:14:10.000000 nanomotif-0.2.1/nanomotif/binnary/logging.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     9127 2024-04-16 09:16:26.000000 nanomotif-0.2.1/nanomotif/binnary/scoring.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)      522 2024-03-29 17:14:10.000000 nanomotif-0.2.1/nanomotif/binnary/utils.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)    14165 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/candidate.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     1061 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/constants.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     1698 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/dataload.py
+drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-04-16 09:18:22.052362 nanomotif-0.2.1/nanomotif/datasets/
+-rw-rw-r--   0 shei      (1000) shei      (1000)       27 2024-03-29 17:14:10.000000 nanomotif-0.2.1/nanomotif/datasets/geobacillus-contig-bin.tsv
+-rw-rw-r--   0 shei      (1000) shei      (1000)   176247 2024-03-29 17:14:10.000000 nanomotif-0.2.1/nanomotif/datasets/geobacillus-plasmids.assembly.fasta
+-rw-rw-r--   0 shei      (1000) shei      (1000) 26479844 2024-03-29 17:14:10.000000 nanomotif-0.2.1/nanomotif/datasets/geobacillus-plasmids.pileup.bed
+-rw-rw-r--   0 shei      (1000) shei      (1000)     1106 2024-03-29 17:14:10.000000 nanomotif-0.2.1/nanomotif/datasets.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)    28677 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/evaluate.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)      539 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/feature.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)      321 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/logger.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)    18855 2024-04-16 09:16:26.000000 nanomotif-0.2.1/nanomotif/main.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     1037 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/model.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     5639 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/old_search_method.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)      850 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/parallel.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     6202 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/postprocess.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     7193 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/scoremotifs.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)      197 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/seed.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)    20090 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/seq.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     2677 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/utils.py
+drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-04-16 09:18:22.092362 nanomotif-0.2.1/nanomotif.egg-info/
+-rw-r--r--   0 shei      (1000) shei      (1000)    18166 2024-04-16 09:18:22.000000 nanomotif-0.2.1/nanomotif.egg-info/PKG-INFO
+-rw-rw-r--   0 shei      (1000) shei      (1000)     1606 2024-04-16 09:18:22.000000 nanomotif-0.2.1/nanomotif.egg-info/SOURCES.txt
+-rw-rw-r--   0 shei      (1000) shei      (1000)        1 2024-04-16 09:18:22.000000 nanomotif-0.2.1/nanomotif.egg-info/dependency_links.txt
+-rw-rw-r--   0 shei      (1000) shei      (1000)       50 2024-04-16 09:18:22.000000 nanomotif-0.2.1/nanomotif.egg-info/entry_points.txt
+-rw-rw-r--   0 shei      (1000) shei      (1000)        1 2023-11-30 15:56:57.000000 nanomotif-0.2.1/nanomotif.egg-info/not-zip-safe
+-rw-rw-r--   0 shei      (1000) shei      (1000)      132 2024-04-16 09:18:22.000000 nanomotif-0.2.1/nanomotif.egg-info/requires.txt
+-rw-rw-r--   0 shei      (1000) shei      (1000)       16 2024-04-16 09:18:22.000000 nanomotif-0.2.1/nanomotif.egg-info/top_level.txt
+-rw-rw-r--   0 shei      (1000) shei      (1000)       38 2024-04-16 09:18:22.096362 nanomotif-0.2.1/setup.cfg
+-rw-rw-r--   0 shei      (1000) shei      (1000)      918 2024-03-29 17:14:10.000000 nanomotif-0.2.1/setup.py
+drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-04-16 09:18:22.092362 nanomotif-0.2.1/tests/
+-rw-rw-r--   0 shei      (1000) shei      (1000)        0 2023-11-30 15:56:56.000000 nanomotif-0.2.1/tests/__init__.py
+drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-04-16 09:18:22.092362 nanomotif-0.2.1/tests/binnary/
+-rw-rw-r--   0 shei      (1000) shei      (1000)        0 2024-03-29 17:14:10.000000 nanomotif-0.2.1/tests/binnary/__init__.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     2089 2024-04-16 09:16:26.000000 nanomotif-0.2.1/tests/binnary/conftest.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     1019 2024-03-29 17:14:10.000000 nanomotif-0.2.1/tests/binnary/test_arg_parser.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)    11132 2024-04-16 09:16:26.000000 nanomotif-0.2.1/tests/binnary/test_cli_commands.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     6352 2024-03-29 17:14:10.000000 nanomotif-0.2.1/tests/binnary/test_data_processing_functions.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     2585 2024-03-29 17:14:10.000000 nanomotif-0.2.1/tests/binnary/test_detect_contamination.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     1404 2024-03-29 17:14:10.000000 nanomotif-0.2.1/tests/binnary/test_generate_output.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     2132 2024-03-29 17:14:10.000000 nanomotif-0.2.1/tests/binnary/test_include_contigs.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     3317 2024-04-16 09:16:26.000000 nanomotif-0.2.1/tests/binnary/test_scoring.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)      744 2024-03-29 17:14:10.000000 nanomotif-0.2.1/tests/binnary/test_utils.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     5405 2024-04-16 09:16:26.000000 nanomotif-0.2.1/tests/binnary/test_write_bins.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     7236 2023-11-30 15:56:57.000000 nanomotif-0.2.1/tests/test_candidate.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     1365 2024-03-29 11:56:23.000000 nanomotif-0.2.1/tests/test_dataload.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     2933 2024-03-29 11:56:23.000000 nanomotif-0.2.1/tests/test_motif_find.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)        0 2024-03-29 11:56:23.000000 nanomotif-0.2.1/tests/test_motif_score.py
```

### Comparing `nanomotif-0.2.0/LICENSE` & `nanomotif-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/PKG-INFO` & `nanomotif-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomotif
-Version: 0.2.0
+Version: 0.2.1
 Summary: Identifying methlyation motifs in nanopore data
 Author: AAU_DarkScience
 Author-email: shei@bio.aau.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wheel
@@ -187,16 +187,16 @@
 
 ### Bin contamination
 #### Usage
 After motif identification it is possible to identify contamination in bins using the bin-motifs, contig-bin and motif-scored files. 
 
 ```
 usage: nanomotif detect_contamination [-h] --motifs_scored MOTIFS_SCORED --bin_motifs BIN_MOTIFS --contig_bins CONTIG_BINS [-t THREADS] [--mean_methylation_cutoff MEAN_METHYLATION_CUTOFF]
-                                      [--n_motif_contig_cutoff N_MOTIF_CONTIG_CUTOFF] [--n_motif_bin_cutoff N_MOTIF_BIN_CUTOFF] [--ambiguous_motif_percentage_cutoff AMBIGUOUS_MOTIF_PERCENTAGE_CUTOFF] --out
-                                      OUT
+                                      [--n_motif_contig_cutoff N_MOTIF_CONTIG_CUTOFF] [--n_motif_bin_cutoff N_MOTIF_BIN_CUTOFF] [--ambiguous_motif_percentage_cutoff AMBIGUOUS_MOTIF_PERCENTAGE_CUTOFF]
+                                      [--write_bins] [--assembly_file ASSEMBLY_FILE] --out OUT [--contamination_file CONTAMINATION_FILE]
 
 optional arguments:
   -h, --help            show this help message and exit
   --motifs_scored MOTIFS_SCORED
                         Path to motifs-scored.tsv from nanomotif
   --bin_motifs BIN_MOTIFS
                         Path to bin-motifs.tsv file
@@ -209,34 +209,42 @@
   --n_motif_contig_cutoff N_MOTIF_CONTIG_CUTOFF
                         Number of motifs that needs to be observed in a contig before it is considered valid for scoring
   --n_motif_bin_cutoff N_MOTIF_BIN_CUTOFF
                         Number of motifs that needs to be observed in a bin to be considered valid for scoring
   --ambiguous_motif_percentage_cutoff AMBIGUOUS_MOTIF_PERCENTAGE_CUTOFF
                         Percentage of ambiguous motifs defined as mean methylation between 0.05 and 0.40 in a bin. Motifs with an ambiguous methylation percentage of more than this value are removed from
                         scoring. Default is 0.40
+  --write_bins          If specified, new bins will be written to a bins folder. Requires --assembly_file to be specified.
+  --assembly_file ASSEMBLY_FILE
+                        Path to assembly.fasta file
   --out OUT             Path to output directory
+  --contamination_file CONTAMINATION_FILE
+                        Path to an existing contamination file if bins should be outputtet as a post-processing step
 ```
 
+If `detect_contamination` was run without the `--write_bins` flag, bins can be written as a post processing step if the `--contamination_file` is specified along with the `--write_bins` flag and the `--assembly_file` flag.
+
 The output is a `bin_contamination.tsv` file with the following columns:
 
 | **Column**       | **Description**                                                                                       |
 |------------------|-------------------------------------------------------------------------------------------------------|
 | **bin**          | bin to which the motif belong                                                                         |
 | **bin_contig_compare** | The contig for which the methylation pattern is compared. The name is a concatenation of bin + "_" + contig. |
 | **binary_methylation_missmatch_score** | Number of methylation missmatches between the contig and the bin_consensus pattern. |
 | **non_na_comparisons** | Number of non-NA comparisons between the contig and the bin_consensus pattern. |
 | **contig** | The contig for which the methylation pattern is compared. | 
 
 ### Include unbinned contigs
-This module tries to assign contigs in the assembly file to bins by comparing the methylation pattern of the contig to the bin consensus. the contig must have a unique perfect match to the bin consensus to be assigned to a bin. Additionally, the `include_contigs` assigns all the contigs in the `bin_contamination.tsv` file to as unbinned. If decontamination should not be performed, the `include_contigs` can be run with an empty `bin_contamination.tsv` file with just the column. 
+This module tries to assign contigs in the assembly file to bins by comparing the methylation pattern of the contig to the bin consensus. the contig must have a unique perfect match to the bin consensus to be assigned to a bin. Additionally, the `include_contigs` assigns all the contigs in the `bin_contamination.tsv` file to as unbinned. If decontamination should not be performed, the `include_contigs` can be run without the `--run_detect_contamination` flag or without the `--contamination_file` flag.
 
 ```
 usage: nanomotif include_contigs [-h] --motifs_scored MOTIFS_SCORED --bin_motifs BIN_MOTIFS --contig_bins CONTIG_BINS [-t THREADS] [--mean_methylation_cutoff MEAN_METHYLATION_CUTOFF]
-                                 [--n_motif_contig_cutoff N_MOTIF_CONTIG_CUTOFF] [--n_motif_bin_cutoff N_MOTIF_BIN_CUTOFF] [--ambiguous_motif_percentage_cutoff AMBIGUOUS_MOTIF_PERCENTAGE_CUTOFF] --out OUT
-                                 (--contamination_file CONTAMINATION_FILE | --run_detect_contamination) [--write_bins] [--assembly_file ASSEMBLY_FILE] [--min_motif_comparisons MIN_MOTIF_COMPARISONS]
+                                 [--n_motif_contig_cutoff N_MOTIF_CONTIG_CUTOFF] [--n_motif_bin_cutoff N_MOTIF_BIN_CUTOFF] [--ambiguous_motif_percentage_cutoff AMBIGUOUS_MOTIF_PERCENTAGE_CUTOFF]
+                                 [--write_bins] [--assembly_file ASSEMBLY_FILE] --out OUT [--contamination_file CONTAMINATION_FILE | --run_detect_contamination]
+                                 [--min_motif_comparisons MIN_MOTIF_COMPARISONS]
 
 optional arguments:
   -h, --help            show this help message and exit
   --motifs_scored MOTIFS_SCORED
                         Path to motifs-scored.tsv from nanomotif
   --bin_motifs BIN_MOTIFS
                         Path to bin-motifs.tsv file
@@ -249,22 +257,22 @@
   --n_motif_contig_cutoff N_MOTIF_CONTIG_CUTOFF
                         Number of motifs that needs to be observed in a contig before it is considered valid for scoring
   --n_motif_bin_cutoff N_MOTIF_BIN_CUTOFF
                         Number of motifs that needs to be observed in a bin to be considered valid for scoring
   --ambiguous_motif_percentage_cutoff AMBIGUOUS_MOTIF_PERCENTAGE_CUTOFF
                         Percentage of ambiguous motifs defined as mean methylation between 0.05 and 0.40 in a bin. Motifs with an ambiguous methylation percentage of more than this value are removed from
                         scoring. Default is 0.40
+  --write_bins          If specified, new bins will be written to a bins folder. Requires --assembly_file to be specified.
+  --assembly_file ASSEMBLY_FILE
+                        Path to assembly.fasta file
   --out OUT             Path to output directory
   --contamination_file CONTAMINATION_FILE
                         Path to an existing contamination file to include in the analysis
   --run_detect_contamination
                         Indicate that the detect_contamination workflow should be run first
-  --write_bins          If specified, new bins will be written to a bins folder. Requires --assembly_file to be specified.
-  --assembly_file ASSEMBLY_FILE
-                        Path to assembly.fasta file
   --min_motif_comparisons MIN_MOTIF_COMPARISONS
                         Minimum number of non-NA motif comparisons required to include a contig in the analysis. Default is 5
 ```
 
 The output is two files: `include_contigs.tsv` and `new_contig_bin.tsv`. The `include_contigs.tsv` file is the contigs that were assigned based on the methylation pattern and the `new_contig_bin.tsv` is the updated contig-bin file.
 
 The `include_contigs.tsv` file has the following columns:
```

### Comparing `nanomotif-0.2.0/README.md` & `nanomotif-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -167,16 +167,16 @@
 
 ### Bin contamination
 #### Usage
 After motif identification it is possible to identify contamination in bins using the bin-motifs, contig-bin and motif-scored files. 
 
 ```
 usage: nanomotif detect_contamination [-h] --motifs_scored MOTIFS_SCORED --bin_motifs BIN_MOTIFS --contig_bins CONTIG_BINS [-t THREADS] [--mean_methylation_cutoff MEAN_METHYLATION_CUTOFF]
-                                      [--n_motif_contig_cutoff N_MOTIF_CONTIG_CUTOFF] [--n_motif_bin_cutoff N_MOTIF_BIN_CUTOFF] [--ambiguous_motif_percentage_cutoff AMBIGUOUS_MOTIF_PERCENTAGE_CUTOFF] --out
-                                      OUT
+                                      [--n_motif_contig_cutoff N_MOTIF_CONTIG_CUTOFF] [--n_motif_bin_cutoff N_MOTIF_BIN_CUTOFF] [--ambiguous_motif_percentage_cutoff AMBIGUOUS_MOTIF_PERCENTAGE_CUTOFF]
+                                      [--write_bins] [--assembly_file ASSEMBLY_FILE] --out OUT [--contamination_file CONTAMINATION_FILE]
 
 optional arguments:
   -h, --help            show this help message and exit
   --motifs_scored MOTIFS_SCORED
                         Path to motifs-scored.tsv from nanomotif
   --bin_motifs BIN_MOTIFS
                         Path to bin-motifs.tsv file
@@ -189,34 +189,42 @@
   --n_motif_contig_cutoff N_MOTIF_CONTIG_CUTOFF
                         Number of motifs that needs to be observed in a contig before it is considered valid for scoring
   --n_motif_bin_cutoff N_MOTIF_BIN_CUTOFF
                         Number of motifs that needs to be observed in a bin to be considered valid for scoring
   --ambiguous_motif_percentage_cutoff AMBIGUOUS_MOTIF_PERCENTAGE_CUTOFF
                         Percentage of ambiguous motifs defined as mean methylation between 0.05 and 0.40 in a bin. Motifs with an ambiguous methylation percentage of more than this value are removed from
                         scoring. Default is 0.40
+  --write_bins          If specified, new bins will be written to a bins folder. Requires --assembly_file to be specified.
+  --assembly_file ASSEMBLY_FILE
+                        Path to assembly.fasta file
   --out OUT             Path to output directory
+  --contamination_file CONTAMINATION_FILE
+                        Path to an existing contamination file if bins should be outputtet as a post-processing step
 ```
 
+If `detect_contamination` was run without the `--write_bins` flag, bins can be written as a post processing step if the `--contamination_file` is specified along with the `--write_bins` flag and the `--assembly_file` flag.
+
 The output is a `bin_contamination.tsv` file with the following columns:
 
 | **Column**       | **Description**                                                                                       |
 |------------------|-------------------------------------------------------------------------------------------------------|
 | **bin**          | bin to which the motif belong                                                                         |
 | **bin_contig_compare** | The contig for which the methylation pattern is compared. The name is a concatenation of bin + "_" + contig. |
 | **binary_methylation_missmatch_score** | Number of methylation missmatches between the contig and the bin_consensus pattern. |
 | **non_na_comparisons** | Number of non-NA comparisons between the contig and the bin_consensus pattern. |
 | **contig** | The contig for which the methylation pattern is compared. | 
 
 ### Include unbinned contigs
-This module tries to assign contigs in the assembly file to bins by comparing the methylation pattern of the contig to the bin consensus. the contig must have a unique perfect match to the bin consensus to be assigned to a bin. Additionally, the `include_contigs` assigns all the contigs in the `bin_contamination.tsv` file to as unbinned. If decontamination should not be performed, the `include_contigs` can be run with an empty `bin_contamination.tsv` file with just the column. 
+This module tries to assign contigs in the assembly file to bins by comparing the methylation pattern of the contig to the bin consensus. the contig must have a unique perfect match to the bin consensus to be assigned to a bin. Additionally, the `include_contigs` assigns all the contigs in the `bin_contamination.tsv` file to as unbinned. If decontamination should not be performed, the `include_contigs` can be run without the `--run_detect_contamination` flag or without the `--contamination_file` flag.
 
 ```
 usage: nanomotif include_contigs [-h] --motifs_scored MOTIFS_SCORED --bin_motifs BIN_MOTIFS --contig_bins CONTIG_BINS [-t THREADS] [--mean_methylation_cutoff MEAN_METHYLATION_CUTOFF]
-                                 [--n_motif_contig_cutoff N_MOTIF_CONTIG_CUTOFF] [--n_motif_bin_cutoff N_MOTIF_BIN_CUTOFF] [--ambiguous_motif_percentage_cutoff AMBIGUOUS_MOTIF_PERCENTAGE_CUTOFF] --out OUT
-                                 (--contamination_file CONTAMINATION_FILE | --run_detect_contamination) [--write_bins] [--assembly_file ASSEMBLY_FILE] [--min_motif_comparisons MIN_MOTIF_COMPARISONS]
+                                 [--n_motif_contig_cutoff N_MOTIF_CONTIG_CUTOFF] [--n_motif_bin_cutoff N_MOTIF_BIN_CUTOFF] [--ambiguous_motif_percentage_cutoff AMBIGUOUS_MOTIF_PERCENTAGE_CUTOFF]
+                                 [--write_bins] [--assembly_file ASSEMBLY_FILE] --out OUT [--contamination_file CONTAMINATION_FILE | --run_detect_contamination]
+                                 [--min_motif_comparisons MIN_MOTIF_COMPARISONS]
 
 optional arguments:
   -h, --help            show this help message and exit
   --motifs_scored MOTIFS_SCORED
                         Path to motifs-scored.tsv from nanomotif
   --bin_motifs BIN_MOTIFS
                         Path to bin-motifs.tsv file
@@ -229,22 +237,22 @@
   --n_motif_contig_cutoff N_MOTIF_CONTIG_CUTOFF
                         Number of motifs that needs to be observed in a contig before it is considered valid for scoring
   --n_motif_bin_cutoff N_MOTIF_BIN_CUTOFF
                         Number of motifs that needs to be observed in a bin to be considered valid for scoring
   --ambiguous_motif_percentage_cutoff AMBIGUOUS_MOTIF_PERCENTAGE_CUTOFF
                         Percentage of ambiguous motifs defined as mean methylation between 0.05 and 0.40 in a bin. Motifs with an ambiguous methylation percentage of more than this value are removed from
                         scoring. Default is 0.40
+  --write_bins          If specified, new bins will be written to a bins folder. Requires --assembly_file to be specified.
+  --assembly_file ASSEMBLY_FILE
+                        Path to assembly.fasta file
   --out OUT             Path to output directory
   --contamination_file CONTAMINATION_FILE
                         Path to an existing contamination file to include in the analysis
   --run_detect_contamination
                         Indicate that the detect_contamination workflow should be run first
-  --write_bins          If specified, new bins will be written to a bins folder. Requires --assembly_file to be specified.
-  --assembly_file ASSEMBLY_FILE
-                        Path to assembly.fasta file
   --min_motif_comparisons MIN_MOTIF_COMPARISONS
                         Minimum number of non-NA motif comparisons required to include a contig in the analysis. Default is 5
 ```
 
 The output is two files: `include_contigs.tsv` and `new_contig_bin.tsv`. The `include_contigs.tsv` file is the contigs that were assigned based on the methylation pattern and the `new_contig_bin.tsv` is the updated contig-bin file.
 
 The `include_contigs.tsv` file has the following columns:
```

### Comparing `nanomotif-0.2.0/nanomotif/argparser.py` & `nanomotif-0.2.1/nanomotif/argparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,52 +97,64 @@
     
     parser_binnary_shared.add_argument(
         "--ambiguous_motif_percentage_cutoff",
         type=float,
         default=0.40,
         help="Percentage of ambiguous motifs defined as mean methylation between 0.05 and 0.40 in a bin. Motifs with an ambiguous methylation percentage of more than this value are removed from scoring. Default is 0.40",
     )
+    parser_binnary_shared.add_argument(
+        "--write_bins",
+        action='store_true',
+        help="If specified, new bins will be written to a bins folder. Requires --assembly_file to be specified.",
+    )
+    parser_binnary_shared.add_argument(
+        "--assembly_file",
+        type=str,
+        help="Path to assembly.fasta file"
+    )
+    parser_binnary_shared.add_argument(
+        "--save_scores",
+        action='store_true',
+        help="If specified, the scores for each comparison will be saved to a scores folder in the output directory"
+    )
+    
     parser_binnary_shared.add_argument("--out", type=str, help="Path to output directory", required=True, default="nanomotif")
     
     # Binnary contamination
     parser_contamination = subparsers.add_parser(
         'detect_contamination', 
         help="Detect contamination in bins",
         parents=[parser_binnary_shared]
     )  
     
+    parser_contamination.add_argument(
+        '--contamination_file',
+        type=str,
+        help="Path to an existing contamination file if bins should be outputtet as a post-processing step"
+    )
+    
     # Binnary inclusion
     parser_inclusion = subparsers.add_parser(
         'include_contigs', 
         help="Include contigs in bins",
         parents=[parser_binnary_shared]
     )
     
-    group = parser_inclusion.add_mutually_exclusive_group(required=True)
+    group = parser_inclusion.add_mutually_exclusive_group(required=False)
     group.add_argument(
         "--contamination_file",
         type=str,
         help="Path to an existing contamination file to include in the analysis"
     )
     group.add_argument(
         "--run_detect_contamination",
         action='store_true',
         help="Indicate that the detect_contamination workflow should be run first"
     )
     parser_inclusion.add_argument(
-        "--write_bins",
-        action='store_true',
-        help="If specified, new bins will be written to a bins folder. Requires --assembly_file to be specified.",
-    )
-    parser_inclusion.add_argument(
-        "--assembly_file",
-        type=str,
-        help="Path to assembly.fasta file"
-    )
-    parser_inclusion.add_argument(
         "--min_motif_comparisons",
         type=int,
         default=5,
         help="Minimum number of non-NA motif comparisons required to include a contig in the analysis. Default is 5",
     )
```

### Comparing `nanomotif-0.2.0/nanomotif/bin_consensus.py` & `nanomotif-0.2.1/nanomotif/bin_consensus.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/nanomotif/binnary/analysis.py` & `nanomotif-0.2.1/nanomotif/binnary/analysis.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/nanomotif/binnary/data_processing.py` & `nanomotif-0.2.1/nanomotif/binnary/data_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,16 +60,16 @@
     - new_contig_bins (DataFrame): DataFrame with contig and bin assignments.
     - assembly_dict (dict): Dictionary with contig IDs as keys and sequences as values, from the assembly file.
     - output_dir (str): Path to the directory where the new bin files will be saved.
     """
     logger = logging.getLogger(__name__)
     
     # check if the output directory exists
-    logger.info(f"Writing bins to {output_dir}/bins/...")
-    output_bins_dir = os.path.join(output_dir, "bins")
+    logger.info(f"Writing bins to {output_dir}")
+    output_bins_dir = os.path.join(output_dir)
     if not os.path.exists(output_bins_dir):
         os.makedirs(output_bins_dir)
     
     # Group the DataFrame by 'bin'
     grouped = new_contig_bins.groupby('bin')
 
     for bin_name, group in grouped:
@@ -188,14 +188,15 @@
     return motifs_scored_in_bins
 
 
 def remove_ambiguous_motifs_from_bin_consensus(motifs_scored_in_bins, args):
     # Remove motifs in bins where the majority of the mean methylation of motifs is in the range of 0.05-0.4
     contig_motif_mean_density = motifs_scored_in_bins \
         .filter(pl.col("bin") != "unbinned") \
+        .filter(pl.col("n_motifs") >= args.n_motif_contig_cutoff) \
         .with_columns(
             ((pl.col("mean") > 0.05) & (pl.col("mean") < 0.4)).alias("is_ambiguous")
         )
 
     # Count the number of ambiguous motifs per bin
     # Group by 'bin' and 'motif_mod' and calculate the sum of 'is_ambiguous' and the total count in each group
     bin_consensus_ambiguous_motifs = contig_motif_mean_density.group_by(["bin", "motif_mod"]) \
@@ -330,21 +331,22 @@
     required_columns = ["bin", "bin_contig_compare", "binary_methylation_missmatch_score", "non_na_comparisons", "contig"]
     if not all(column in contamination.columns for column in required_columns):
         raise ValueError("The contamination file does not contain the required columns.")
     
     return contamination
 
 
-def create_contig_bin_file(contig_bins, include, contamination):
+def create_contig_bin_file(contig_bins, contamination, include=None):
     """
     Create a new contig_bin file based on the analysis results and contamination file.
     """
     # Remove contigs in the contamination file from the contig_bins
     contig_bins = contig_bins[~contig_bins["contig"].isin(contamination["contig"])]
     
     # Add the contigs in the include DataFrame to the contig_bins
-    contig_bins = pd.concat([contig_bins, include[["contig", "bin"]]], ignore_index=True)
+    if include is not None:
+        contig_bins = pd.concat([contig_bins, include[["contig", "bin"]]], ignore_index=True)
     
     # Sort the contig_bins by bin and contig
     contig_bins = contig_bins.sort_values(by=["bin", "contig"])
     
     return contig_bins
```

### Comparing `nanomotif-0.2.0/nanomotif/binnary/detect_contamination.py` & `nanomotif-0.2.1/nanomotif/binnary/detect_contamination.py`

 * *Files 23% similar despite different names*

```diff
@@ -22,29 +22,19 @@
         args: argparse.Namespace - Namespace containing the arguments passed to the script
     """
     logger = logging.getLogger(__name__)
     logger.info("Starting contamination detection analysis...")
     motifs_scored_in_bins_wo_unbinned = motifs_scored_in_bins \
         .filter(~pl.col("bin_contig").str.contains("unbinned"))
     
-    # Define the corresponding choices for each condition
-    choices = [
-        0,  # bin motif is methylated, contig motif is methylated
-        1,  # bin motif is methylated, contig motif is not methylated
-        1,  # bin motif is not methylated, contig motif is methylated
-        0,  # bin motif is not methylated, contig motif is not methylated
-        0,  # bin motif is methylated, contig motif is not observed
-        0,  # bin motif is not methylated, contig motif is not observed
-    ]
 
     contig_bin_comparison_score, contigs_w_no_methylation = sc.compare_methylation_pattern_multiprocessed(
         motifs_scored_in_bins=motifs_scored_in_bins_wo_unbinned,
         bin_consensus=bin_consensus,
         mode="contamination",
-        choices=choices,
         args=args,
         num_processes=args.threads
     )
 
     logger.info("Finding contamination in bins")
     
     contig_bin_comparison_score = split_bin_contig(contig_bin_comparison_score)
```

### Comparing `nanomotif-0.2.0/nanomotif/binnary/include_contigs.py` & `nanomotif-0.2.1/nanomotif/binnary/include_contigs.py`

 * *Files 18% similar despite different names*

```diff
@@ -40,30 +40,18 @@
     contigs_for_comparison = motifs_scored_in_bins \
         .filter(
             (pl.col("bin_contig").str.contains("unbinned")) |
             (pl.col("bin_contig").is_in(contamination["bin_contig_compare"]))
         )
     
 
-    
-    # Define the corresponding choices for each condition
-    choices = [
-        0,  # bin motif is methylated, contig motif is methylated
-        1,  # bin motif is methylated, contig motif is not methylated
-        1,  # bin motif is not methylated, contig motif is methylated
-        0,  # bin motif is not methylated, contig motif is not methylated
-        0,  # bin motif is methylated, contig motif is not observed
-        0,  # bin motif is not methylated, contig motif is not observed
-    ]
-
     contig_bin_comparison_score, contigs_w_no_methylation = sc.compare_methylation_pattern_multiprocessed(
         motifs_scored_in_bins=contigs_for_comparison,
         bin_consensus=bin_consensus,
         mode="include",
-        choices=choices,
         args=args,
         num_processes=args.threads
     )
     
     contig_bin_comparison_score = ut.split_bin_contig(contig_bin_comparison_score)
     
     logger.info("Assigning contigs to bins...")
```

### Comparing `nanomotif-0.2.0/nanomotif/binnary/logging.py` & `nanomotif-0.2.1/nanomotif/binnary/logging.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/nanomotif/binnary/scoring.py` & `nanomotif-0.2.1/nanomotif/binnary/scoring.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from nanomotif.binnary import data_processing as dp
 from nanomotif.binnary import utils as ut
+import os
 import polars as pl
 from multiprocessing import Pool, Queue, Process, get_context
 import logging
 from logging.handlers import QueueHandler, QueueListener
 
 # Set up logging
 ## Create queue for logging
-log_queue = Queue()
+# log_queue = Queue()
 
-## Set up a listener to handle logs from the queue
-def setup_logging_queue(queue):
-    while True:
-        record = queue.get()
-        if record is None:  # Use None as a sentinel to stop the listener
-            break
-        logger = logging.getLogger(record.name)
-        logger.handle(record)
-
-def worker_setup_logging(queue):
-    q_handler = QueueHandler(queue)
-    logger = logging.getLogger()
-    logger.setLevel(logging.INFO)
-    logger.addHandler(q_handler)
+# ## Set up a listener to handle logs from the queue
+# def setup_logging_queue(queue):
+#     while True:
+#         record = queue.get()
+#         if record is None:  # Use None as a sentinel to stop the listener
+#             break
+#         logger = logging.getLogger(record.name)
+#         logger.handle(record)
+
+# def worker_setup_logging(queue):
+#     q_handler = QueueHandler(queue)
+#     logger = logging.getLogger()
+#     logger.setLevel(logging.INFO)
+#     logger.addHandler(q_handler)
 
 def define_mean_methylation_thresholds(motif_binary_compare):
     """
     Define mean methylation thresholds for bin and contig motifs
     """
     # Calculate the mean methylation value for each motif in each bin
     motif_binary_compare = motif_binary_compare.with_columns([
@@ -65,15 +66,15 @@
         .alias("methylation_binary_compare")
     ])
     
     return motif_binary_compare
 
 
 
-def compare_methylation_pattern(motif_binary_compare, choices):
+def compare_methylation_pattern(motif_binary_compare):
     """
     Compares the methylation pattern between bin and contig motifs using Polars and calculates the motif_comparison_score.
     """
     motif_comparison_score = (
         pl.when((motif_binary_compare['methylation_binary'] == 1) & (motif_binary_compare['methylation_binary_compare'] == 1))
         .then(0)
         .when((motif_binary_compare['methylation_binary'] == 1) & (motif_binary_compare['methylation_binary_compare'] == 0))
@@ -99,82 +100,122 @@
             pl.sum("motif_comparison_score").alias("binary_methylation_missmatch_score"),
             pl.count("motif_comparison_score").alias("non_na_comparisons")
         ])
         
     return contig_bin_comparison_score
 
 
-def process_bin_contig(bin_contig, bin_motifs_from_motifs_scored_in_bins, motifs_scored_in_contigs, mode, choices):
-    worker_setup_logging(log_queue)
-    logger = logging.getLogger(__name__)
-    logger.info(f"Processing {bin_contig}")
-    
-    bin = ut.get_bin(bin_contig)
+def process_bin_contig(
+    bin_contig, 
+    bin_motifs_from_motifs_scored_in_bins, 
+    motifs_scored_in_contigs, 
+    mode, 
+    args
+):
+    """
+    This function processes a single contig and compares the methylation pattern between the contig and the bin.
+    Depending on the mode, the function will either look for contamination or include contigs.
     
-    if mode == "contamination":
-        motif_binary_compare = bin_motifs_from_motifs_scored_in_bins \
-            .filter(pl.col("bin") == bin) \
-            .join(
-                motifs_scored_in_contigs.filter(pl.col("bin_compare") == bin_contig),
-                on="motif_mod"
-            )
-    if mode == "include":
-        motif_binary_compare = bin_motifs_from_motifs_scored_in_bins \
-            .filter(pl.col("bin") != bin) \
-            .join(
-                motifs_scored_in_contigs.filter(pl.col("bin_compare") == bin_contig),
-                on="motif_mod"
-            )
-    
-    # Define methylation thresholds
-    motif_binary_compare = define_mean_methylation_thresholds(motif_binary_compare)
-
-    # Calculate the comparison score regardless of methylation presence
-    contig_bin_comparison_score = compare_methylation_pattern(motif_binary_compare, choices)
-    
-    # Check if the contig has no methylation and note it, but do not exclude it from further processing
-    contigHasNMethylation = motif_binary_compare.filter(pl.col("methylation_binary_compare") == 1).height
-    logger.info(f"Finished processing {bin_contig}. Contig has {contigHasNMethylation} positive methylation comparisons.")
-    
-    if mode == "include":
-        contig_bin_comparison_score = contig_bin_comparison_score \
-            .filter(
-                pl.col("binary_methylation_missmatch_score") == 0
-            )
-    if mode == "contamination":
-        contig_bin_comparison_score = contig_bin_comparison_score \
-            .filter(
-                pl.col("binary_methylation_missmatch_score") > 0
-            )
+    Parameters:
+    - bin_contig: str
+        The contig to process
+    - bin_motifs_from_motifs_scored_in_bins: polars.DataFrame
+        The motifs scored in the bin
+    - motifs_scored_in_contigs: polars.DataFrame
+        The motifs scored in the contigs
+    - mode: str
+        The mode to run the comparison in. Either "contamination" or "include"
+    - args: argparse.Namespace
+        The arguments passed to the script
+    
+    Returns:
+    - contig_bin_comparison_score: polars.DataFrame
+        The comparison score for the contig
+    """
+    # worker_setup_logging(log_queue)
+    # logger = logging.getLogger(__name__)
+    # logger.info(f"Processing {bin_contig}")
+    try:
+        bin = ut.get_bin(bin_contig)
+        
+        if mode == "contamination":
+            motif_binary_compare = bin_motifs_from_motifs_scored_in_bins \
+                .filter(pl.col("bin") == bin) \
+                .join(
+                    motifs_scored_in_contigs.filter(pl.col("bin_compare") == bin_contig),
+                    on="motif_mod"
+                )
+        if mode == "include":
+            motif_binary_compare = bin_motifs_from_motifs_scored_in_bins \
+                .filter(pl.col("bin") != bin) \
+                .join(
+                    motifs_scored_in_contigs.filter(pl.col("bin_compare") == bin_contig),
+                    on="motif_mod"
+                )
+        
+        # Define methylation thresholds
+        motif_binary_compare = define_mean_methylation_thresholds(motif_binary_compare)
+
+        if args.save_scores:
+            path = os.path.join(args.out, "scores", args.command, "binary_compare" + bin_contig + ".csv")
+            motif_binary_compare.write_csv(path)
+
+        # Calculate the comparison score regardless of methylation presence
+        contig_bin_comparison_score = compare_methylation_pattern(motif_binary_compare)
+        
+        # Check if the contig has no methylation and note it, but do not exclude it from further processing
+        contigHasNMethylation = motif_binary_compare.filter(pl.col("methylation_binary_compare") == 1).height
+        # logger.info(f"Finished processing {bin_contig}. Contig has {contigHasNMethylation} positive methylation comparisons.")
+        
+        if mode == "include":
+            contig_bin_comparison_score = contig_bin_comparison_score \
+                .filter(
+                    pl.col("binary_methylation_missmatch_score") == 0
+                )
+        if mode == "contamination":
+            contig_bin_comparison_score = contig_bin_comparison_score \
+                .filter(
+                    pl.col("binary_methylation_missmatch_score") > 0
+                )
+                
             
+        if contigHasNMethylation == 0:
+            return contig_bin_comparison_score, bin_contig
         
-    if contigHasNMethylation == 0:
-        return contig_bin_comparison_score, bin_contig
-    
-    return contig_bin_comparison_score, None
+        return contig_bin_comparison_score, None
+    except Exception as e:
+        error_log_path = os.path.join(args.out, "logs", f"{args.command}_{bin_contig}_error.err")
+        
+        with open(error_log_path, 'w') as error_file:
+            error_file.write(f"Error processing {bin_contig}: {str(e)}\n")
+        return None, None
 
-def compare_methylation_pattern_multiprocessed(motifs_scored_in_bins, bin_consensus, choices, mode, args, num_processes=1):
+def compare_methylation_pattern_multiprocessed(motifs_scored_in_bins, bin_consensus, mode, args, num_processes=1):
     logger = logging.getLogger(__name__)
     logger.info("Starting comparison of methylation patterns")
     
     motifs_scored_in_contigs = motifs_scored_in_bins \
         .filter(pl.col("n_motifs") >= args.n_motif_contig_cutoff) \
         .select(["bin_contig", "motif_mod", "mean"]) \
         .rename({"bin_contig": "bin_compare"})
     
+    if args.save_scores:
+        dir = os.path.join(args.out, "scores", args.command)
+        if not os.path.exists(dir):
+            os.makedirs(dir)
 
     comparison_score = pl.DataFrame()
     contigs_w_no_methylation = []
 
     with get_context("spawn").Pool(processes=num_processes) as pool:
         results = pool.starmap(
             process_bin_contig,
             [
-                (bin_contig, bin_consensus, motifs_scored_in_contigs, mode, choices)
-                for bin_contig in motifs_scored_in_contigs.select("bin_compare").unique().to_pandas()["bin_compare"].tolist()
+                (bin_contig, bin_consensus, motifs_scored_in_contigs, mode, args)
+                for bin_contig in motifs_scored_in_contigs.select("bin_compare").unique()["bin_compare"]
             ]
         )
         
     for result, no_methylation in results:
         if result is not None:
             comparison_score = pl.concat([comparison_score, result])
         if no_methylation is not None:
```

### Comparing `nanomotif-0.2.0/nanomotif/binnary/utils.py` & `nanomotif-0.2.1/nanomotif/binnary/utils.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/nanomotif/candidate.py` & `nanomotif-0.2.1/nanomotif/candidate.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/nanomotif/constants.py` & `nanomotif-0.2.1/nanomotif/constants.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/nanomotif/dataload.py` & `nanomotif-0.2.1/nanomotif/dataload.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/nanomotif/datasets/geobacillus-plasmids.assembly.fasta` & `nanomotif-0.2.1/nanomotif/datasets/geobacillus-plasmids.assembly.fasta`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/nanomotif/datasets/geobacillus-plasmids.pileup.bed` & `nanomotif-0.2.1/nanomotif/datasets/geobacillus-plasmids.pileup.bed`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/nanomotif/datasets.py` & `nanomotif-0.2.1/nanomotif/datasets.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/nanomotif/evaluate.py` & `nanomotif-0.2.1/nanomotif/evaluate.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/nanomotif/feature.py` & `nanomotif-0.2.1/nanomotif/feature.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/nanomotif/main.py` & `nanomotif-0.2.1/nanomotif/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -321,35 +321,34 @@
 def binnary(args):
     """
     binnary entry point for the DNA Methylation Pattern Analysis tool.
     Orchestrates the workflow of the tool based on the provided arguments.
     """
     
     # Conditional check for --write_bins and --assembly_file
-    if args.command == "include_contigs":
-        if args.write_bins and not args.assembly_file:
-            print("Error: --assembly_file must be specified when --write_bins is used.")
-            sys.exit(1)
-        elif not args.write_bins and args.assembly_file:
-            print("Error: --assembly_file can only be used when --write_bins is specified.")
-            sys.exit(1)
+    if args.write_bins and not args.assembly_file:
+        print("Error: --assembly_file must be specified when --write_bins is used.")
+        sys.exit(1)
+    elif not args.write_bins and args.assembly_file:
+        print("Error: --assembly_file can only be used when --write_bins is specified.")
+        sys.exit(1)
     
     print("Starting Binnary ", args.command, " analysis...")
 
     
     # Settting up the logger
     # set_logger_config(args)
-    logger = log.getLogger(__name__)
-    logger.info("Starting Binnary analysis...")
+    # logger = log.getLogger(__name__)
+    log.info("Starting Binnary analysis...")
     
     # Set number of threads for polars
     os.environ['POLARS_MAX_THREADS'] = str(args.threads)
     
     POLAR_THREADS = pl.threadpool_size()
-    logger.info(f"Polars is using {POLAR_THREADS} threads.")
+    log.info(f"Polars is using {POLAR_THREADS} threads.")
     
     # Step 1: Load and preprocess data
     # These functions would be defined in your data_processing module
     (
         motifs_scored,
         bin_motifs,
         contig_bins,
@@ -366,56 +365,87 @@
         motifs_scored,
         motifs_in_bin_consensus,
         contig_bins
     )
     
     
     # Create the bin_consensus dataframe for scoring
-    logger.info("Creating bin_consensus dataframe for scoring...")
+    log.info("Creating bin_consensus dataframe for scoring...")
     bin_motifs_from_motifs_scored_in_bins = data_processing.construct_bin_consensus_from_motifs_scored_in_bins(
         motifs_scored_in_bins,
         args
     )
 
-    # Functions from the analysis module
-    if args.command == "detect_contamination" or (args.command == "include_contigs" and args.run_detect_contamination):
+    # Setting up the contamination analysis
+    if (args.command == "detect_contamination" and not args.contamination_file) or (args.command == "include_contigs" and args.run_detect_contamination):
         contamination = detect_contamination.detect_contamination(
             motifs_scored_in_bins, bin_motifs_from_motifs_scored_in_bins, args
         )
         data_processing.generate_output(contamination.to_pandas(), args.out, "bin_contamination.tsv")
+    elif args.contamination_file:
+        log.info("Loading contamination file...")
+        contamination = data_processing.load_contamination_file(args.contamination_file)
         
+    if args.command == "detect_contamination":
+        # Create a decontaminated contig_bin file
+        new_contig_bins = data_processing.create_contig_bin_file(
+            contig_bins=contig_bins.to_pandas(), 
+            contamination=contamination.to_pandas(),
+            include=None
+        )
+        data_processing.generate_output(new_contig_bins, args.out, "decontaminated_contig_bin.tsv")
 
     if args.command == "include_contigs":
-        # User provided contamination file
-        if args.contamination_file:
-            print("Loading contamination file...")
-            contamination = data_processing.load_contamination_file(args.contamination_file)
+        # # User provided contamination file
+        # if args.contamination_file:
+        #     log.info("Loading contamination file...")
+        #     contamination = data_processing.load_contamination_file(args.contamination_file)
+        
+        ## If run_detect_contamination is false and contamination file is not provided, then set contamination to None
+        if not args.run_detect_contamination and not args.contamination_file:
+            contamination = pl.DataFrame(
+                {
+                    "bin": [],
+                    "bin_contig_compare": [],
+                    "binary_methylation_missmatch_score": [],
+                    "non_na_comparisons": [],
+                    "contig": []
+                }
+            )
+        
+        
         
         # Run the include_contigs analysis    
         include_contigs_df = include_contigs.include_contigs(
             motifs_scored_in_bins, bin_motifs_from_motifs_scored_in_bins, contamination, args
         )
         
         # Save the include_contigs_df results
         data_processing.generate_output(include_contigs_df.to_pandas(), args.out, "include_contigs.tsv")
         
         # Create a new contig_bin file
-        new_contig_bins = data_processing.create_contig_bin_file(contig_bins.to_pandas(), include_contigs_df.to_pandas(), contamination.to_pandas())
+        
+        
+        new_contig_bins = data_processing.create_contig_bin_file(
+            contig_bins=contig_bins.to_pandas(), 
+            contamination= contamination.to_pandas(),
+            include=include_contigs_df.to_pandas()
+        )
         data_processing.generate_output(new_contig_bins, args.out, "new_contig_bin.tsv")
         
-        if args.write_bins:
-            logger.info("Write bins flag is set. Writing bins to file...")
-            print("Loading assembly file...")
-            logger.info("Loading assembly file...")
-            assembly = data_processing.read_fasta(args.assembly_file)
-            
-            logger.info(f"Writing bins to {args.out}/bins/...")
-            data_processing.write_bins_from_contigs(new_contig_bins, assembly, args.out)
+    if args.write_bins:
+        log.info("Write bins flag is set. Writing bins to file...")
+        log.info("Loading assembly file...")
+        assembly = data_processing.read_fasta(args.assembly_file)
+        
+        bin_dir = os.path.join(args.out, args.command + "_bins")
+        
+        data_processing.write_bins_from_contigs(new_contig_bins, assembly, bin_dir)
     
-    logger.info(f"Analysis Completed. Results are saved to: {args.out}")
+    log.info(f"Analysis Completed. Results are saved to: {args.out}")
     print("Analysis Completed. Results are saved to:", args.out)
 
 
 
 
 
 def main():
```

### Comparing `nanomotif-0.2.0/nanomotif/model.py` & `nanomotif-0.2.1/nanomotif/model.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/nanomotif/old_search_method.py` & `nanomotif-0.2.1/nanomotif/old_search_method.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/nanomotif/parallel.py` & `nanomotif-0.2.1/nanomotif/parallel.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/nanomotif/postprocess.py` & `nanomotif-0.2.1/nanomotif/postprocess.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/nanomotif/scoremotifs.py` & `nanomotif-0.2.1/nanomotif/scoremotifs.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/nanomotif/seq.py` & `nanomotif-0.2.1/nanomotif/seq.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/nanomotif/utils.py` & `nanomotif-0.2.1/nanomotif/utils.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/nanomotif.egg-info/PKG-INFO` & `nanomotif-0.2.1/nanomotif.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomotif
-Version: 0.2.0
+Version: 0.2.1
 Summary: Identifying methlyation motifs in nanopore data
 Author: AAU_DarkScience
 Author-email: shei@bio.aau.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wheel
@@ -187,16 +187,16 @@
 
 ### Bin contamination
 #### Usage
 After motif identification it is possible to identify contamination in bins using the bin-motifs, contig-bin and motif-scored files. 
 
 ```
 usage: nanomotif detect_contamination [-h] --motifs_scored MOTIFS_SCORED --bin_motifs BIN_MOTIFS --contig_bins CONTIG_BINS [-t THREADS] [--mean_methylation_cutoff MEAN_METHYLATION_CUTOFF]
-                                      [--n_motif_contig_cutoff N_MOTIF_CONTIG_CUTOFF] [--n_motif_bin_cutoff N_MOTIF_BIN_CUTOFF] [--ambiguous_motif_percentage_cutoff AMBIGUOUS_MOTIF_PERCENTAGE_CUTOFF] --out
-                                      OUT
+                                      [--n_motif_contig_cutoff N_MOTIF_CONTIG_CUTOFF] [--n_motif_bin_cutoff N_MOTIF_BIN_CUTOFF] [--ambiguous_motif_percentage_cutoff AMBIGUOUS_MOTIF_PERCENTAGE_CUTOFF]
+                                      [--write_bins] [--assembly_file ASSEMBLY_FILE] --out OUT [--contamination_file CONTAMINATION_FILE]
 
 optional arguments:
   -h, --help            show this help message and exit
   --motifs_scored MOTIFS_SCORED
                         Path to motifs-scored.tsv from nanomotif
   --bin_motifs BIN_MOTIFS
                         Path to bin-motifs.tsv file
@@ -209,34 +209,42 @@
   --n_motif_contig_cutoff N_MOTIF_CONTIG_CUTOFF
                         Number of motifs that needs to be observed in a contig before it is considered valid for scoring
   --n_motif_bin_cutoff N_MOTIF_BIN_CUTOFF
                         Number of motifs that needs to be observed in a bin to be considered valid for scoring
   --ambiguous_motif_percentage_cutoff AMBIGUOUS_MOTIF_PERCENTAGE_CUTOFF
                         Percentage of ambiguous motifs defined as mean methylation between 0.05 and 0.40 in a bin. Motifs with an ambiguous methylation percentage of more than this value are removed from
                         scoring. Default is 0.40
+  --write_bins          If specified, new bins will be written to a bins folder. Requires --assembly_file to be specified.
+  --assembly_file ASSEMBLY_FILE
+                        Path to assembly.fasta file
   --out OUT             Path to output directory
+  --contamination_file CONTAMINATION_FILE
+                        Path to an existing contamination file if bins should be outputtet as a post-processing step
 ```
 
+If `detect_contamination` was run without the `--write_bins` flag, bins can be written as a post processing step if the `--contamination_file` is specified along with the `--write_bins` flag and the `--assembly_file` flag.
+
 The output is a `bin_contamination.tsv` file with the following columns:
 
 | **Column**       | **Description**                                                                                       |
 |------------------|-------------------------------------------------------------------------------------------------------|
 | **bin**          | bin to which the motif belong                                                                         |
 | **bin_contig_compare** | The contig for which the methylation pattern is compared. The name is a concatenation of bin + "_" + contig. |
 | **binary_methylation_missmatch_score** | Number of methylation missmatches between the contig and the bin_consensus pattern. |
 | **non_na_comparisons** | Number of non-NA comparisons between the contig and the bin_consensus pattern. |
 | **contig** | The contig for which the methylation pattern is compared. | 
 
 ### Include unbinned contigs
-This module tries to assign contigs in the assembly file to bins by comparing the methylation pattern of the contig to the bin consensus. the contig must have a unique perfect match to the bin consensus to be assigned to a bin. Additionally, the `include_contigs` assigns all the contigs in the `bin_contamination.tsv` file to as unbinned. If decontamination should not be performed, the `include_contigs` can be run with an empty `bin_contamination.tsv` file with just the column. 
+This module tries to assign contigs in the assembly file to bins by comparing the methylation pattern of the contig to the bin consensus. the contig must have a unique perfect match to the bin consensus to be assigned to a bin. Additionally, the `include_contigs` assigns all the contigs in the `bin_contamination.tsv` file to as unbinned. If decontamination should not be performed, the `include_contigs` can be run without the `--run_detect_contamination` flag or without the `--contamination_file` flag.
 
 ```
 usage: nanomotif include_contigs [-h] --motifs_scored MOTIFS_SCORED --bin_motifs BIN_MOTIFS --contig_bins CONTIG_BINS [-t THREADS] [--mean_methylation_cutoff MEAN_METHYLATION_CUTOFF]
-                                 [--n_motif_contig_cutoff N_MOTIF_CONTIG_CUTOFF] [--n_motif_bin_cutoff N_MOTIF_BIN_CUTOFF] [--ambiguous_motif_percentage_cutoff AMBIGUOUS_MOTIF_PERCENTAGE_CUTOFF] --out OUT
-                                 (--contamination_file CONTAMINATION_FILE | --run_detect_contamination) [--write_bins] [--assembly_file ASSEMBLY_FILE] [--min_motif_comparisons MIN_MOTIF_COMPARISONS]
+                                 [--n_motif_contig_cutoff N_MOTIF_CONTIG_CUTOFF] [--n_motif_bin_cutoff N_MOTIF_BIN_CUTOFF] [--ambiguous_motif_percentage_cutoff AMBIGUOUS_MOTIF_PERCENTAGE_CUTOFF]
+                                 [--write_bins] [--assembly_file ASSEMBLY_FILE] --out OUT [--contamination_file CONTAMINATION_FILE | --run_detect_contamination]
+                                 [--min_motif_comparisons MIN_MOTIF_COMPARISONS]
 
 optional arguments:
   -h, --help            show this help message and exit
   --motifs_scored MOTIFS_SCORED
                         Path to motifs-scored.tsv from nanomotif
   --bin_motifs BIN_MOTIFS
                         Path to bin-motifs.tsv file
@@ -249,22 +257,22 @@
   --n_motif_contig_cutoff N_MOTIF_CONTIG_CUTOFF
                         Number of motifs that needs to be observed in a contig before it is considered valid for scoring
   --n_motif_bin_cutoff N_MOTIF_BIN_CUTOFF
                         Number of motifs that needs to be observed in a bin to be considered valid for scoring
   --ambiguous_motif_percentage_cutoff AMBIGUOUS_MOTIF_PERCENTAGE_CUTOFF
                         Percentage of ambiguous motifs defined as mean methylation between 0.05 and 0.40 in a bin. Motifs with an ambiguous methylation percentage of more than this value are removed from
                         scoring. Default is 0.40
+  --write_bins          If specified, new bins will be written to a bins folder. Requires --assembly_file to be specified.
+  --assembly_file ASSEMBLY_FILE
+                        Path to assembly.fasta file
   --out OUT             Path to output directory
   --contamination_file CONTAMINATION_FILE
                         Path to an existing contamination file to include in the analysis
   --run_detect_contamination
                         Indicate that the detect_contamination workflow should be run first
-  --write_bins          If specified, new bins will be written to a bins folder. Requires --assembly_file to be specified.
-  --assembly_file ASSEMBLY_FILE
-                        Path to assembly.fasta file
   --min_motif_comparisons MIN_MOTIF_COMPARISONS
                         Minimum number of non-NA motif comparisons required to include a contig in the analysis. Default is 5
 ```
 
 The output is two files: `include_contigs.tsv` and `new_contig_bin.tsv`. The `include_contigs.tsv` file is the contigs that were assigned based on the methylation pattern and the `new_contig_bin.tsv` is the updated contig-bin file.
 
 The `include_contigs.tsv` file has the following columns:
```

### Comparing `nanomotif-0.2.0/nanomotif.egg-info/SOURCES.txt` & `nanomotif-0.2.1/nanomotif.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,13 +43,15 @@
 tests/test_candidate.py
 tests/test_dataload.py
 tests/test_motif_find.py
 tests/test_motif_score.py
 tests/binnary/__init__.py
 tests/binnary/conftest.py
 tests/binnary/test_arg_parser.py
+tests/binnary/test_cli_commands.py
 tests/binnary/test_data_processing_functions.py
 tests/binnary/test_detect_contamination.py
 tests/binnary/test_generate_output.py
 tests/binnary/test_include_contigs.py
 tests/binnary/test_scoring.py
-tests/binnary/test_utils.py
+tests/binnary/test_utils.py
+tests/binnary/test_write_bins.py
```

### Comparing `nanomotif-0.2.0/setup.py` & `nanomotif-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/tests/binnary/conftest.py` & `nanomotif-0.2.1/tests/binnary/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
         self.bin_motifs = "datasets/binnary_testdata/bin-motifs.tsv"
         self.contig_bins = "datasets/binnary_testdata/contig_bin.tsv"
         self.mean_methylation_cutoff = 0.25
         self.n_motif_bin_cutoff = 500
         self.n_motif_contig_cutoff = 10
         self.ambiguous_motif_percentage_cutoff = 0.40
         self.min_motif_comparisons = 2
+        self.save_scores = False
         self.out = "tests/binnary/test_output"
         self.threads = 1
 
 # Remove tests/test_output directory
 import shutil
 shutil.rmtree("tests/binnary/test_output", ignore_errors=True)
```

### Comparing `nanomotif-0.2.0/tests/binnary/test_arg_parser.py` & `nanomotif-0.2.1/tests/binnary/test_arg_parser.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/tests/binnary/test_data_processing_functions.py` & `nanomotif-0.2.1/tests/binnary/test_data_processing_functions.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/tests/binnary/test_detect_contamination.py` & `nanomotif-0.2.1/tests/binnary/test_detect_contamination.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/tests/binnary/test_generate_output.py` & `nanomotif-0.2.1/tests/binnary/test_generate_output.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/tests/binnary/test_include_contigs.py` & `nanomotif-0.2.1/tests/binnary/test_include_contigs.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/tests/binnary/test_scoring.py` & `nanomotif-0.2.1/tests/binnary/test_scoring.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,28 +19,28 @@
     
     bin_consensus = dp.construct_bin_consensus_from_motifs_scored_in_bins(
         motifs_scored_in_bins,
         args
     )
     
     # Define the corresponding choices for each condition
-    choices = [
-        0,  # bin motif is methylated, contig motif is methylated
-        1,  # bin motif is methylated, contig motif is not methylated
-        1,  # bin motif is not methylated, contig motif is methylated
-        0,  # bin motif is not methylated, contig motif is not methylated
-        0,  # bin motif is methylated, contig motif is not observed
-        0,  # bin motif is not methylated, contig motif is not observed
-    ]
+    # choices = [
+    #     0,  # bin motif is methylated, contig motif is methylated
+    #     1,  # bin motif is methylated, contig motif is not methylated
+    #     1,  # bin motif is not methylated, contig motif is methylated
+    #     0,  # bin motif is not methylated, contig motif is not methylated
+    #     0,  # bin motif is methylated, contig motif is not observed
+    #     0,  # bin motif is not methylated, contig motif is not observed
+    # ]
     
     contig_bin_comparison_score, contigs_w_no_methylation = sc.compare_methylation_pattern_multiprocessed(
         motifs_scored_in_bins=motifs_scored_in_bins,
         bin_consensus=bin_consensus,
         mode="contamination",
-        choices=choices,
+        # choices=choices,
         args=args
     )
     contig_bin_comparison_score = split_bin_contig(contig_bin_comparison_score)
     print(contig_bin_comparison_score)
     print(contigs_w_no_methylation)
     
     contig_bin_comparison_score = contig_bin_comparison_score.to_pandas()
@@ -63,29 +63,18 @@
         .filter(~pl.col("bin_contig").str.contains("unbinned"))
     
     bin_consensus = dp.construct_bin_consensus_from_motifs_scored_in_bins(
         motifs_scored_in_bins,
         args
     )
     
-    # Define the corresponding choices for each condition
-    choices = [
-        0,  # bin motif is methylated, contig motif is methylated
-        1,  # bin motif is methylated, contig motif is not methylated
-        1,  # bin motif is not methylated, contig motif is methylated
-        0,  # bin motif is not methylated, contig motif is not methylated
-        0,  # bin motif is methylated, contig motif is not observed
-        0,  # bin motif is not methylated, contig motif is not observed
-    ]
-    
     contig_bin_comparison_score, contigs_w_no_methylation = sc.compare_methylation_pattern_multiprocessed(
         motifs_scored_in_bins=motifs_scored_in_bins,
         bin_consensus=bin_consensus,
         mode="include",
-        choices=choices,
         args=args
     )
     contig_bin_comparison_score = split_bin_contig(contig_bin_comparison_score)
     print(contig_bin_comparison_score)
     print(contigs_w_no_methylation)
     
     contig_bin_comparison_score = contig_bin_comparison_score.to_pandas()
```

### Comparing `nanomotif-0.2.0/tests/binnary/test_utils.py` & `nanomotif-0.2.1/tests/binnary/test_utils.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/tests/test_candidate.py` & `nanomotif-0.2.1/tests/test_candidate.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/tests/test_dataload.py` & `nanomotif-0.2.1/tests/test_dataload.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.0/tests/test_motif_find.py` & `nanomotif-0.2.1/tests/test_motif_find.py`

 * *Files identical despite different names*

